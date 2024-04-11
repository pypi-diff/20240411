# Comparing `tmp/tomwer-1.3.6.tar.gz` & `tmp/tomwer-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomwer-1.3.6.tar", last modified: Mon Mar 25 10:56:28 2024, max compression
+gzip compressed data, was "tomwer-1.3.7.tar", last modified: Thu Apr 11 07:39:57 2024, max compression
```

## Comparing `tomwer-1.3.6.tar` & `tomwer-1.3.7.tar`

### file list

```diff
@@ -1,899 +1,899 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.933650 tomwer-1.3.6/
--rw-r--r--   0 payno     (1000) payno     (1000)     1877 2023-07-19 16:04:34.000000 tomwer-1.3.6/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/MANIFEST.in
--rw-r--r--   0 payno     (1000) payno     (1000)    11254 2024-03-25 10:56:28.933650 tomwer-1.3.6/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     2709 2024-01-22 10:03:25.000000 tomwer-1.3.6/README.rst
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/orangecontrib/
--rw-r--r--   0 payno     (1000) payno     (1000)      277 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/orangecontrib/tomwer/
--rw-r--r--   0 payno     (1000) payno     (1000)      148 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/orangecontrib/tomwer/orange/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/orange/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4621 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/orange/managedprocess.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2044 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/orange/settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1711 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/state_summary.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/orangecontrib/tomwer/tutorials/
--rw-r--r--   0 payno     (1000) payno     (1000)     4747 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/EBS_tomo_listener.ows
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5485 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/append_raw_darks_and_flats_frames_to_NXtomos.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     2918 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/cast_volume.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     6208 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth1.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     5204 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth2.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     4699 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/default_cor_search.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     3670 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/hello_world_python_script.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     8534 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/icat_publication.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     4435 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_slice_reconstruction.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     6584 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_slice_reconstruction_on_slurm.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     5945 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_volume_local_reconstruction.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     7809 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_volume_to_slurm_reconstruction.ows
--rw-r--r--   0 payno     (1000) payno     (1000)     5192 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/tutorials/using_saaxis_to_find_cor.ows
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/orangecontrib/tomwer/widgets/
--rw-r--r--   0 payno     (1000) payno     (1000)     2526 2024-03-06 14:45:33.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/
--rw-r--r--   0 payno     (1000) payno     (1000)     8961 2024-02-06 10:29:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/FutureSupervisorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4034 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/SlurmClusterOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1614 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)     1995 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurm.png
--rw-r--r--   0 payno     (1000) payno     (1000)     9790 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurm.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3212 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.png
--rw-r--r--   0 payno     (1000) payno     (1000)    56984 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.889650 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/
--rw-r--r--   0 payno     (1000) payno     (1000)     2460 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/AdvancementOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8041 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataDiscoveryOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4774 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataListOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15242 2024-02-28 08:43:13.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataListenerOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5159 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataSelectorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7262 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataTransfertOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7113 2024-02-28 08:43:13.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataValidatorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7403 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataWatcherOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9888 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/EDF2NXTomomillOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2493 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/EmailOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4659 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/FilterOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3271 2024-02-28 08:42:24.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NXTomomillMixIn.py
--rw-r--r--   0 payno     (1000) payno     (1000)    13995 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NXTomomillOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6416 2024-02-28 08:59:33.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NXtomoConcatenate.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4237 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NotifierOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2836 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/ReduceDarkFlatSelectorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6790 2024-02-28 08:42:24.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/SingleTomoObjOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4395 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/TimerOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3203 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/TomoObjSerieOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5144 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/VolumeSelector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6626 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/VolumeSymLinkOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1545 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.889650 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)      729 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/advancement.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5781 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/advancement.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      768 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.png
--rw-r--r--   0 payno     (1000) payno     (1000)    14318 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      598 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datadiscover.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3772 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datadiscover.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2100 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datalistener.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3136 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datalistener.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3351 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datawatcher.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1306 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/edf2nx.png
--rw-r--r--   0 payno     (1000) payno     (1000)     7039 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/edf2nx.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      755 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/email.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1836 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/email.svg
--rw-r--r--   0 payno     (1000) payno     (1000)   105862 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/esrf.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5645 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/folder-transfert.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1077 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/image_key_upgrader.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2072 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/namefilter.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3757 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/namefilter.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2600 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/notification.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4587 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/notification.svg
--rw-r--r--   0 payno     (1000) payno     (1000)    66863 2023-10-02 08:33:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/nxtomomill.png
--rw-r--r--   0 payno     (1000) payno     (1000)    11185 2023-10-02 08:33:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/nxtomomill.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2516 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/progress.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3864 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.png
--rw-r--r--   0 payno     (1000) payno     (1000)    39604 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2873 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/scanlist.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1463 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/scanselector.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2129 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/scanselector.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      351 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/single_tomo_obj.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3615 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/single_tomo_obj.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3641 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/time.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3116 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5900 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     8992 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/tomwer.png
--rw-r--r--   0 payno     (1000) payno     (1000)     9358 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/validator.png
--rw-r--r--   0 payno     (1000) payno     (1000)     9592 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/validatorcrack.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1525 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumeselector.png
--rw-r--r--   0 payno     (1000) payno     (1000)    10936 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumeselector.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1895 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumesymlink.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5786 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumesymlink.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.889650 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/
--rw-r--r--   0 payno     (1000) payno     (1000)     6374 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/DatasetGeneratorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2436 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/ObjectInspectorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1553 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.889650 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)     2034 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/hammer.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3191 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/hammer.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1020 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/inspector.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3943 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/inspector.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.889650 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/
--rw-r--r--   0 payno     (1000) payno     (1000)     6399 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/DarkFlatPatchOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4467 2024-02-23 14:39:44.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/ImageKeyEditorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4820 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/ImageKeyUpgraderOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3817 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/NXtomoEditorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1555 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.889650 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)      878 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.png
--rw-r--r--   0 payno     (1000) payno     (1000)     7396 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      998 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.png
--rw-r--r--   0 payno     (1000) payno     (1000)    13531 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1026 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.png
--rw-r--r--   0 payno     (1000) payno     (1000)     8204 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1522 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.png
--rw-r--r--   0 payno     (1000) payno     (1000)    29749 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.889650 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2832 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_dark_flat_patch.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2129 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_image_key_editor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2211 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_image_key_upgrader.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5888 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_nxtomo_editor.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/
--rw-r--r--   0 payno     (1000) payno     (1000)     3481 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/PublishProcessedDataOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-02-08 13:36:55.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/RawDataScreenshotCreatorOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4532 2024-02-08 13:36:55.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/SaveToGalleryAndPublishOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)      267 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)     1271 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/add_gallery.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5147 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/add_gallery.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2866 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.png
--rw-r--r--   0 payno     (1000) payno     (1000)    22489 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1120 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6358 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)     8992 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6731 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_build.png
--rw-r--r--   0 payno     (1000) payno     (1000)    15969 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_build.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     7491 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_cluster.png
--rw-r--r--   0 payno     (1000) payno     (1000)    22047 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_cluster.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     7057 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_control.png
--rw-r--r--   0 payno     (1000) payno     (1000)    19095 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_control.svg
--rw-r--r--   0 payno     (1000) payno     (1000)    18651 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.png
--rw-r--r--   0 payno     (1000) payno     (1000)    31006 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     7306 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.png
--rw-r--r--   0 payno     (1000) payno     (1000)    15202 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     8172 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_edit.png
--rw-r--r--   0 payno     (1000) payno     (1000)    17150 2023-11-17 08:26:45.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_edit.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     7194 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_other.png
--rw-r--r--   0 payno     (1000) payno     (1000)    16763 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_other.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     8066 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_stitching.png
--rw-r--r--   0 payno     (1000) payno     (1000)    22169 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_stitching.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     8760 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_visu.png
--rw-r--r--   0 payno     (1000) payno     (1000)    18818 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_visu.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/
--rw-r--r--   0 payno     (1000) payno     (1000)    27790 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/PythonScriptOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)      886 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/TomoObjsHub.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1512 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)     5501 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/icons/PythonScript.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1122 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/icons/hub.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3735 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/other/icons/hub.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/
--rw-r--r--   0 payno     (1000) payno     (1000)    22342 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/AxisOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9604 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/CastNabuVolumeOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10988 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/DarkRefAndCopyOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5967 2024-02-28 08:59:33.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/NabuHelicalPrepareWeightsDoubleOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12673 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/NabuOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19195 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/NabuVolumeOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)    18724 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/SAAxisOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15480 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/SADeltaBetaOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10720 2024-03-25 10:55:06.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/SinoNormOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1601 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)     1286 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/axis.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5426 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/axis.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     8121 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/bricks.png
--rw-r--r--   0 payno     (1000) payno     (1000)    24845 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.png
--rw-r--r--   0 payno     (1000) payno     (1000)    33704 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     5509 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.png
--rw-r--r--   0 payno     (1000) payno     (1000)    14957 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.svg
--rw-r--r--   0 payno     (1000) payno     (1000)   105862 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/esrf.png
--rw-r--r--   0 payno     (1000) payno     (1000)      176 2023-10-02 08:33:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_2d.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3999 2023-10-02 08:33:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_2d.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2940 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6178 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3023 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.png
--rw-r--r--   0 payno     (1000) payno     (1000)    11959 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      163 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_prepare_weights_double.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5136 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_prepare_weights_double.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2784 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.png
--rw-r--r--   0 payno     (1000) payno     (1000)     7303 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      791 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6778 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3305 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.png
--rw-r--r--   0 payno     (1000) payno     (1000)    13025 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     4107 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.png
--rw-r--r--   0 payno     (1000) payno     (1000)    14712 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     6846 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/tomogui.png
--rw-r--r--   0 payno     (1000) payno     (1000)     8992 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/tomwer.png
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/stitching/
--rw-r--r--   0 payno     (1000) payno     (1000)     2351 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/stitching/StitcherOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3252 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/stitching/ZStitchingConfigOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)      262 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/stitching/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2339 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.893650 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/
--rw-r--r--   0 payno     (1000) payno     (1000)     5382 2024-02-29 12:22:09.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/DataViewerOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2855 2024-02-08 13:36:55.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/DiffViewerOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3145 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/LivesliceOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1918 2024-01-24 11:58:19.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/NXtomoMetadataViewerOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3421 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/RadioStackOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4093 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/SampleMovedOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3211 2024-02-08 13:36:55.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/SinogramViewerOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4092 2024-01-22 10:03:25.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/SliceStackOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1865 2024-02-23 07:52:09.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/VolumeViewerOW.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1604 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.897650 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)      378 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/diff.png
--rw-r--r--   0 payno     (1000) payno     (1000)     7693 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/diff.svg
--rw-r--r--   0 payno     (1000) payno     (1000)   105862 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/esrf.png
--rw-r--r--   0 payno     (1000) payno     (1000)    11631 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/eye.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4279 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/eyecrack.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1392 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/liveslice.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3349 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/liveslice.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1114 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.png
--rw-r--r--   0 payno     (1000) payno     (1000)    22650 2023-10-02 08:41:00.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2704 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2498 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1281 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1228 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.svg
--rw-r--r--   0 payno     (1000) payno     (1000)   134176 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/sinogramviewer.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2454 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6967 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     8992 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/tomwer.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4372 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.png
--rw-r--r--   0 payno     (1000) payno     (1000)     8454 2023-07-19 16:04:34.000000 tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3267 2024-03-25 10:56:28.933650 tomwer-1.3.6/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)     1474 2023-10-02 08:41:00.000000 tomwer-1.3.6/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.897650 tomwer-1.3.6/tomwer/
--rw-r--r--   0 payno     (1000) payno     (1000)     1745 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8575 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/__main__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.897650 tomwer-1.3.6/tomwer/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/app/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6004 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/axis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1561 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/app/canvas.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.897650 tomwer-1.3.6/tomwer/app/canvas_launcher/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/app/canvas_launcher/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7164 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/app/canvas_launcher/config.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2501 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/app/canvas_launcher/environ.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19146 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/app/canvas_launcher/mainwindow.py
--rw-r--r--   0 payno     (1000) payno     (1000)      560 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/app/canvas_launcher/splash.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2859 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/app/canvas_launcher/widgetsscheme.py
--rw-r--r--   0 payno     (1000) payno     (1000)      276 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/app/darkref.py
--rw-r--r--   0 payno     (1000) payno     (1000)      285 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/app/darkrefpatch.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3166 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/diffframe.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2821 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/app/imagekeyeditor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3217 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/app/imagekeyupgrader.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6660 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/app/intensitynormalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9940 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/multicor.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12799 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/app/multipag.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7646 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/app/nabuapp.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2837 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/app/nxtomoeditor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3827 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/app/patchrawdarkflat.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2587 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/radiostack.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6520 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/app/reducedarkflat.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4081 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/app/rsync.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2527 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/samplemoved.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2708 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/scanviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3677 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/sinogramviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2428 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/slicestack.py
--rw-r--r--   0 payno     (1000) payno     (1000)      957 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/app/stopdatalistener.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12877 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/app/zstitching.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.897650 tomwer-1.3.6/tomwer/core/
--rw-r--r--   0 payno     (1000) payno     (1000)     1373 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.897650 tomwer-1.3.6/tomwer/core/cluster/
--rw-r--r--   0 payno     (1000) payno     (1000)       60 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/cluster/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5744 2024-02-08 12:15:39.000000 tomwer-1.3.6/tomwer/core/cluster/cluster.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6441 2024-02-06 09:55:41.000000 tomwer-1.3.6/tomwer/core/futureobject.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/log/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/log/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4099 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/log/logger.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3697 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/log/processlog.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/cluster/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/cluster/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1755 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/cluster/supervisor.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/conditions/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/conditions/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7156 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/conditions/filters.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/control/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/control/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      377 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/control/datadiscovery.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/control/datalistener/
--rw-r--r--   0 payno     (1000) payno     (1000)       52 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/control/datalistener/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    22087 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/control/datalistener/datalistener.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11104 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/control/datalistener/rpcserver.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/control/datawatcher/
--rw-r--r--   0 payno     (1000) payno     (1000)       50 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/control/datawatcher/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    16822 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/control/datawatcher/datawatcher.py
--rw-r--r--   0 payno     (1000) payno     (1000)    25752 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/control/datawatcher/datawatcherobserver.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9450 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/control/datawatcher/datawatcherprocess.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7209 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/control/datawatcher/edfdwprocess.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3027 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/control/datawatcher/hdf5dwprocess.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3074 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/control/datawatcher/status.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4806 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/control/emailnotifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3826 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/control/nxtomoconcatenate.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9559 2024-02-26 12:35:46.000000 tomwer-1.3.6/tomwer/core/process/control/nxtomomill.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2048 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/control/scanlist.py
--rw-r--r--   0 payno     (1000) payno     (1000)      368 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/control/scanselector.py
--rw-r--r--   0 payno     (1000) payno     (1000)    26592 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/control/scantransfer.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10611 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/control/scanvalidator.py
--rw-r--r--   0 payno     (1000) payno     (1000)      555 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/control/singletomoobj.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/control/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/control/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2176 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/control/test/test_concatenate_nxtomos.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1553 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/control/test/test_email.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5472 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/control/test/test_h52nx_process.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3238 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/control/test/test_volume_link.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3635 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/control/timer.py
--rw-r--r--   0 payno     (1000) payno     (1000)      266 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/control/tomoobjserie.py
--rw-r--r--   0 payno     (1000) payno     (1000)      370 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/control/volumeselector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7626 2024-02-26 12:35:46.000000 tomwer-1.3.6/tomwer/core/process/control/volumesymlink.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/edit/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/edit/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5239 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/core/process/edit/darkflatpatch.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9398 2024-02-28 08:59:33.000000 tomwer-1.3.6/tomwer/core/process/edit/imagekeyeditor.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/icat/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/icat/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3677 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/icat/createscreenshots.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14813 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/icat/gallery.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1066 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/icat/icatbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7828 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/icat/publish.py
--rw-r--r--   0 payno     (1000) payno     (1000)      816 2024-02-07 10:00:26.000000 tomwer-1.3.6/tomwer/core/process/icat/screenshots.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1562 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/output.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/
--rw-r--r--   0 payno     (1000) payno     (1000)     1504 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/axis/
--rw-r--r--   0 payno     (1000) payno     (1000)       80 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/axis/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1896 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/axis/anglemode.py
--rw-r--r--   0 payno     (1000) payno     (1000)    42723 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/axis/axis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6750 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/axis/mode.py
--rw-r--r--   0 payno     (1000) payno     (1000)    33185 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/axis/params.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1543 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/axis/projectiontype.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    20862 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/darkrefs.py
--rw-r--r--   0 payno     (1000) payno     (1000)    13276 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/darkrefscopy.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10080 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/params.py
--rw-r--r--   0 payno     (1000) payno     (1000)      188 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/settings.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10239 2024-02-28 08:42:24.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/castvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1997 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/helical.py
--rw-r--r--   0 payno     (1000) payno     (1000)    24428 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabucommon.py
--rw-r--r--   0 payno     (1000) payno     (1000)    25702 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabuscores.py
--rw-r--r--   0 payno     (1000) payno     (1000)    38731 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabuslices.py
--rw-r--r--   0 payno     (1000) payno     (1000)    21916 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabuvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)      134 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/plane.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2279 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1481 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/target.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17950 2024-02-26 12:35:49.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/normalization/
--rw-r--r--   0 payno     (1000) payno     (1000)      119 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/normalization/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    13210 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/normalization/normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4790 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/normalization/params.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3967 2024-02-23 12:37:18.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/output.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7725 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/paramsbase.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/saaxis/
--rw-r--r--   0 payno     (1000) payno     (1000)      137 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/saaxis/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5583 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/saaxis/params.py
--rw-r--r--   0 payno     (1000) payno     (1000)    31985 2024-02-23 13:43:06.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/saaxis/saaxis.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/sadeltabeta/
--rw-r--r--   0 payno     (1000) payno     (1000)      162 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/sadeltabeta/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4043 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/sadeltabeta/params.py
--rw-r--r--   0 payno     (1000) payno     (1000)    30925 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/sadeltabeta/sadeltabeta.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.901650 tomwer-1.3.6/tomwer/core/process/reconstruction/scores/
--rw-r--r--   0 payno     (1000) payno     (1000)      282 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/scores/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7564 2024-02-07 10:00:26.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/scores/params.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7383 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/scores/scores.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/process/reconstruction/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1614 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_axis_params.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2429 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_darkref.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6090 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_darkref_copy.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1505 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_paramsbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4295 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_saaxis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2555 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_sadeltabeta.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1006 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/process/reconstruction/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      368 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/reconstruction/utils/cor.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/process/script/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/script/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4028 2024-01-26 08:55:40.000000 tomwer-1.3.6/tomwer/core/process/script/python.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/process/stitching/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/stitching/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6527 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/stitching/metadataholder.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6781 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/core/process/stitching/nabustitcher.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15703 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/task.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/process/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11810 2024-02-28 08:42:25.000000 tomwer-1.3.6/tomwer/core/process/test/test_axis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3464 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/test/test_conditions.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15444 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/test/test_dark_and_flat.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3696 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/test/test_data_listener.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15419 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/process/test/test_data_transfer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3138 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/test/test_data_watcher.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19621 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/process/test/test_nabu.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4014 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/process/test/test_normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3027 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/test/test_timer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4010 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/process/visualization/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/process/visualization/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1656 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/dataviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1594 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/diffviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1577 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/imagestackviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)      198 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/process/visualization/liveslice.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1615 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/radiostack.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1601 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/samplemoved.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1569 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/sinogramviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1625 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/slicestack.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1579 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/process/visualization/volumeviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3246 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/progress.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/scan/
--rw-r--r--   0 payno     (1000) payno     (1000)     1392 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/scan/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8244 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/scan/blissscan.py
--rw-r--r--   0 payno     (1000) payno     (1000)    22892 2024-02-28 08:42:25.000000 tomwer-1.3.6/tomwer/core/scan/edfscan.py
--rw-r--r--   0 payno     (1000) payno     (1000)      213 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/scan/futurescan.py
--rw-r--r--   0 payno     (1000) payno     (1000)      980 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/scan/hdf5scan.py
--rw-r--r--   0 payno     (1000) payno     (1000)      472 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/scan/helicalmetadata.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19405 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/scan/nxtomoscan.py
--rw-r--r--   0 payno     (1000) payno     (1000)    32052 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/core/scan/scanbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10521 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/scan/scanfactory.py
--rw-r--r--   0 payno     (1000) payno     (1000)      137 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/scan/scantype.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/scan/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/scan/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2210 2024-02-26 12:35:46.000000 tomwer-1.3.6/tomwer/core/scan/test/test_edf.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2171 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/scan/test/test_future_scan.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3644 2024-02-26 12:35:46.000000 tomwer-1.3.6/tomwer/core/scan/test/test_h5.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3919 2024-02-22 15:41:23.000000 tomwer-1.3.6/tomwer/core/scan/test/test_process_registration.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12228 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/core/scan/test/test_scan.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5358 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/core/settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6115 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/signal.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2197 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/test/test_scanutils.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10668 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/test/test_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1745 2024-02-23 13:43:06.000000 tomwer-1.3.6/tomwer/core/tomwer_object.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)     1559 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/utils/Singleton.py
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-24 11:58:19.000000 tomwer-1.3.6/tomwer/core/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1718 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/utils/char.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4716 2024-03-06 14:13:19.000000 tomwer-1.3.6/tomwer/core/utils/deprecation.py
--rw-r--r--   0 payno     (1000) payno     (1000)      601 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/core/utils/dictutils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2382 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/utils/ftseriesutils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1812 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/utils/gpu.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4979 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/utils/image.py
--rw-r--r--   0 payno     (1000) payno     (1000)      988 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/core/utils/lbsram.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3096 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/utils/locker.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1434 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/utils/logconfig.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2900 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/utils/normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2685 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/core/utils/nxtomoutils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1932 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/core/utils/resource.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15641 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/core/utils/scanutils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1923 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/utils/slurm.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7560 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/core/utils/spec.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3189 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/core/utils/threads.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1845 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/utils/time.py
--rw-r--r--   0 payno     (1000) payno     (1000)      490 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/utils/volumeutils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/core/volume/
--rw-r--r--   0 payno     (1000) payno     (1000)      253 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/volume/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3713 2024-02-07 10:00:26.000000 tomwer-1.3.6/tomwer/core/volume/edfvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4401 2024-02-07 10:00:26.000000 tomwer-1.3.6/tomwer/core/volume/hdf5volume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3717 2024-02-07 10:00:26.000000 tomwer-1.3.6/tomwer/core/volume/jp2kvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4082 2024-02-07 10:00:26.000000 tomwer-1.3.6/tomwer/core/volume/rawvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6040 2024-02-07 10:00:26.000000 tomwer-1.3.6/tomwer/core/volume/tiffvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1539 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/core/volume/volumebase.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7979 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/core/volume/volumefactory.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/gui/
--rw-r--r--   0 payno     (1000) payno     (1000)     1474 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/gui/cluster/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/cluster/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    27604 2024-03-11 14:30:17.000000 tomwer-1.3.6/tomwer/gui/cluster/slurm.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17117 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/gui/cluster/supervisor.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/gui/cluster/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/cluster/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3937 2024-02-28 09:23:56.000000 tomwer-1.3.6/tomwer/gui/cluster/test/test_cluster.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3212 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/cluster/test/test_supervisor.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.905650 tomwer-1.3.6/tomwer/gui/conditions/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/conditions/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5549 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/conditions/filter.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/configuration/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/configuration/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2512 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/configuration/action.py
--rw-r--r--   0 payno     (1000) payno     (1000)      653 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/configuration/level.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/control/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/control/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4677 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/control/actions.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6108 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/control/datadiscovery.py
--rw-r--r--   0 payno     (1000) payno     (1000)    40898 2024-02-22 14:53:54.000000 tomwer-1.3.6/tomwer/gui/control/datalist.py
--rw-r--r--   0 payno     (1000) payno     (1000)    18471 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/control/datalistener.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2572 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/datareacheractions.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5702 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/datatransfert.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14463 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/datavalidator.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/control/datawatcher/
--rw-r--r--   0 payno     (1000) payno     (1000)     1444 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/control/datawatcher/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10193 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/datawatcher/configuration.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3857 2024-02-22 15:41:23.000000 tomwer-1.3.6/tomwer/gui/control/datawatcher/controlwidget.py
--rw-r--r--   0 payno     (1000) payno     (1000)    22592 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/datawatcher/datawatcher.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10543 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/control/datawatcher/datawatcherobserver.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6383 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/control/emailnotifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4826 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/control/history.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7293 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/control/nxtomomill.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7735 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/control/observations.py
--rw-r--r--   0 payno     (1000) payno     (1000)    20536 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/gui/control/reducedarkflatselector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2356 2023-11-27 10:45:57.000000 tomwer-1.3.6/tomwer/gui/control/scanselectorwidget.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5571 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/control/selectorwidgetbase.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/control/serie/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/serie/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3131 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/control/serie/nxtomoconcatenate.py
--rw-r--r--   0 payno     (1000) payno     (1000)    35110 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/control/serie/seriecreator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1374 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/serie/seriewaiter.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6777 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/control/singletomoobj.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/control/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     1368 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/control/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      775 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_datadiscovery.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3508 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_datalist.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3151 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_datalistener.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2017 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_datavalidator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1140 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/control/test/test_email.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3135 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_inputwidget.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2547 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_process_manager.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9430 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/control/test/test_reducedarkflat_selector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2581 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_scanselector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3904 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/control/test/test_scanvalidator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2278 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/control/test/test_single_tomo_obj.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8164 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_volume_dialog.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3407 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/control/test/test_volumeselector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      159 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/control/tomoobjdisplaymode.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2082 2023-11-27 10:15:51.000000 tomwer-1.3.6/tomwer/gui/control/volumeselectorwidget.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/debugtools/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/debugtools/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10641 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/debugtools/datasetgenerator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2925 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/debugtools/objectinspector.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/edit/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/edit/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17533 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/gui/edit/dkrfpatch.py
--rw-r--r--   0 payno     (1000) payno     (1000)    29728 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/edit/imagekeyeditor.py
--rw-r--r--   0 payno     (1000) payno     (1000)    28095 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/edit/nxtomoeditor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2349 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/gui/edit/nxtomowarmer.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/edit/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     1368 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/edit/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8001 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/edit/test/test_dkrf_patch.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5965 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/edit/test/test_image_key_editor.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11285 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/edit/test/test_nx_editor.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/icat/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/icat/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3123 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/icat/createscreenshots.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8700 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/icat/gallery.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6220 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/icat/publish.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12917 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/icons.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5368 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/illustrations.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5501 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/gui/imagefromfile.py
--rw-r--r--   0 payno     (1000) payno     (1000)      713 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/qconfigfile.py
--rw-r--r--   0 payno     (1000) payno     (1000)    22761 2024-02-23 13:43:06.000000 tomwer-1.3.6/tomwer/gui/qfolderdialog.py
--rw-r--r--   0 payno     (1000) payno     (1000)      534 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/qlefilesystem.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/reconstruction/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/reconstruction/axis/
--rw-r--r--   0 payno     (1000) payno     (1000)    12870 2024-03-19 07:33:10.000000 tomwer-1.3.6/tomwer/gui/reconstruction/axis/CompareImages.py
--rw-r--r--   0 payno     (1000) payno     (1000)       94 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/reconstruction/axis/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    27260 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/axis/axis.py
--rw-r--r--   0 payno     (1000) payno     (1000)    92610 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/gui/reconstruction/axis/radioaxis.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/reconstruction/darkref/
--rw-r--r--   0 payno     (1000) payno     (1000)     1373 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/darkref/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11562 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/darkref/darkrefcopywidget.py
--rw-r--r--   0 payno     (1000) payno     (1000)    16468 2024-02-09 09:45:38.000000 tomwer-1.3.6/tomwer/gui/reconstruction/darkref/darkrefwidget.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.909650 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/
--rw-r--r--   0 payno     (1000) payno     (1000)       44 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15003 2024-02-23 13:43:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/castvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4717 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/check.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3708 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/helical.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/
--rw-r--r--   0 payno     (1000) payno     (1000)       77 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3459 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/base.py
--rw-r--r--   0 payno     (1000) payno     (1000)    13085 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/ctf.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11529 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/nabuconfig.py
--rw-r--r--   0 payno     (1000) payno     (1000)    13952 2024-02-23 13:43:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/output.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15368 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/phase.py
--rw-r--r--   0 payno     (1000) payno     (1000)    30942 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/preprocessing.py
--rw-r--r--   0 payno     (1000) payno     (1000)    38981 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/reconstruction.py
--rw-r--r--   0 payno     (1000) payno     (1000)    16941 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuflow.py
--rw-r--r--   0 payno     (1000) payno     (1000)    23549 2024-02-23 13:43:19.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/slices.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2591 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/slurm.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19441 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/nabu/volume.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/reconstruction/normalization/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/normalization/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    33856 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/normalization/intensity.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    32888 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/corrangeselector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9750 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/dimensionwidget.py
--rw-r--r--   0 payno     (1000) payno     (1000)    21065 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/saaxis.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12213 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/sliceselector.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/reconstruction/sadeltabeta/
--rw-r--r--   0 payno     (1000) payno     (1000)       57 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/sadeltabeta/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    20396 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/sadeltabeta/saadeltabeta.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/reconstruction/scores/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/scores/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2826 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/scores/control.py
--rw-r--r--   0 payno     (1000) payno     (1000)    32001 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/reconstruction/scores/scoreplot.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/reconstruction/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/reconstruction/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8867 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/gui/reconstruction/test/test_axis.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14584 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/test/test_nabu.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8128 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/test/test_saaxis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5799 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/reconstruction/test/test_sadeltabeta.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/samplemoved/
--rw-r--r--   0 payno     (1000) payno     (1000)     9669 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/samplemoved/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9401 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/samplemoved/selectiontable.py
--rw-r--r--   0 payno     (1000) payno     (1000)      244 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)    25517 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/stackplot.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8650 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/stacks.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/stitching/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/stitching/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1659 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/stitching/action.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17314 2024-03-25 10:42:08.000000 tomwer-1.3.6/tomwer/gui/stitching/axisorderedlist.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/stitching/config/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/stitching/config/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7578 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/stitching/config/axisparams.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5902 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/stitching/config/output.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6834 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/stitching/config/positionoveraxis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4257 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/stitching/config/stitchingstrategies.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14680 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/stitching/config/tomoobjdetails.py
--rw-r--r--   0 payno     (1000) payno     (1000)      913 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/stitching/metadataholder.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4454 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/stitching/normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5982 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/stitching/stitchandbackground.py
--rw-r--r--   0 payno     (1000) payno     (1000)    57013 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/gui/stitching/stitching.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9669 2024-02-28 08:59:34.000000 tomwer-1.3.6/tomwer/gui/stitching/stitching_preview.py
--rw-r--r--   0 payno     (1000) payno     (1000)    22353 2024-02-28 08:42:25.000000 tomwer-1.3.6/tomwer/gui/stitching/stitching_raw.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/stitching/z_stitching/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/stitching/z_stitching/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8931 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/stitching/z_stitching/fineestimation.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     1368 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1447 2024-02-22 15:41:23.000000 tomwer-1.3.6/tomwer/gui/test/test_axis_gui.py
--rw-r--r--   0 payno     (1000) payno     (1000)      347 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/test/test_qfolder_dialog.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)       66 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6933 2024-02-26 12:45:43.000000 tomwer-1.3.6/tomwer/gui/utils/buttons.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4979 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/utils/completer.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12091 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/utils/flow.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4449 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/utils/illustrations.py
--rw-r--r--   0 payno     (1000) payno     (1000)    24431 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/utils/inputwidget.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/utils/lineselector/
--rw-r--r--   0 payno     (1000) payno     (1000)       75 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/utils/lineselector/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8179 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/utils/lineselector/lineselector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      210 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/utils/qt_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7460 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/utils/sandboxes.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3373 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/utils/scandescription.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2954 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/utils/scrollarea.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3482 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/utils/slider.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1857 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/utils/splashscreen.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5343 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/utils/step.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8117 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/utils/unitsystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2675 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/utils/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19198 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/utils/vignettes.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1844 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/utils/waiterthread.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/visualization/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/visualization/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    27024 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/gui/visualization/dataviewer.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.913650 tomwer-1.3.6/tomwer/gui/visualization/diffviewer/
--rw-r--r--   0 payno     (1000) payno     (1000)       39 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/visualization/diffviewer/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    21812 2024-02-06 14:36:08.000000 tomwer-1.3.6/tomwer/gui/visualization/diffviewer/diffviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)    20928 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/visualization/diffviewer/shiftwidget.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3639 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/visualization/fullscreenplot.py
--rw-r--r--   0 payno     (1000) payno     (1000)      683 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/visualization/nxtomometadata.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10230 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/visualization/reconstructionparameters.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9224 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/visualization/scanoverview.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9707 2024-02-08 13:36:55.000000 tomwer-1.3.6/tomwer/gui/visualization/sinogramviewer.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.917650 tomwer-1.3.6/tomwer/gui/visualization/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     1368 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/gui/visualization/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2446 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/visualization/test/test_dataviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3536 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/visualization/test/test_diffviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2548 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/visualization/test/test_nx_tomo_metadata_viewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3227 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/gui/visualization/test/test_reconstruction_parameters.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3068 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/visualization/test/test_sinogramviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4694 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/visualization/test/test_stacks.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2374 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/gui/visualization/test/test_volumeviewer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1991 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/visualization/tomoobjoverview.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2491 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/gui/visualization/volumeoverview.py
--rw-r--r--   0 payno     (1000) payno     (1000)    16335 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/gui/visualization/volumeviewer.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.917650 tomwer-1.3.6/tomwer/io/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/io/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.917650 tomwer-1.3.6/tomwer/io/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)      272 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/io/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2964 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/io/utils/h5pyutils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3208 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/io/utils/raw_and_processed_data.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2828 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/io/utils/tomoobj.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10678 2024-03-25 10:55:09.000000 tomwer-1.3.6/tomwer/io/utils/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.917650 tomwer-1.3.6/tomwer/resources/
--rw-r--r--   0 payno     (1000) payno     (1000)     5904 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.885650 tomwer-1.3.6/tomwer/resources/gui/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/resources/gui/icons/
--rw-r--r--   0 payno     (1000) payno     (1000)  1618960 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/Imagej_icon.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3858 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/a.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2650 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/a.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      470 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/add.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2254 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/add.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     4639 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/advanced_user.png
--rw-r--r--   0 payno     (1000) payno     (1000)     8162 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/advanced_user.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     8909 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/axis.png
--rw-r--r--   0 payno     (1000) payno     (1000)    12185 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/axis.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3876 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/background.png
--rw-r--r--   0 payno     (1000) payno     (1000)    10778 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/background.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     4694 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/basic_user.png
--rw-r--r--   0 payno     (1000) payno     (1000)     9246 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/basic_user.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2150 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_active.png
--rw-r--r--   0 payno     (1000) payno     (1000)     7344 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_active.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1979 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_inactive.png
--rw-r--r--   0 payno     (1000) payno     (1000)     7519 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_inactive.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3862 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/compare_mode_a_minus_b.png
--rw-r--r--   0 payno     (1000) payno     (1000)     9139 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/compare_mode_a_minus_b.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      873 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/compose.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2813 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/compose.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2443 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_activate.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3472 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_activate.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2588 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_deactivate.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3857 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_deactivate.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1869 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/delta_beta.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2426 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/delta_beta.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1002 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/icons/exit.png
--rw-r--r--   0 payno     (1000) payno     (1000)    10773 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/icons/exit.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      674 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/icons/full_screen.png
--rw-r--r--   0 payno     (1000) payno     (1000)    18573 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/icons/full_screen.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      282 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/hammer.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2472 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/hammer.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2134 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/health.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2817 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/health.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3868 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/high_speed.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2365 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/high_speed.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     4466 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/history.png
--rw-r--r--   0 payno     (1000) payno     (1000)    16464 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/hourglass.npy
--rw-r--r--   0 payno     (1000) payno     (1000)   131152 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/imageNotFound.npy
--rw-r--r--   0 payno     (1000) payno     (1000)     3432 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/information.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4512 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/information.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1022 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/input.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3324 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/input.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      741 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/invisible.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4366 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/invisible.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2968 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/lineselection.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3266 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/lineselection.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1648 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/list_selection.png
--rw-r--r--   0 payno     (1000) payno     (1000)      982 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/list_selection.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      344 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/locked.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2973 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/locked.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      633 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/log.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2207 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/log.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2981 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/loop.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3839 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/low_speed.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2362 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/low_speed.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3836 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/medium_low_speed.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2361 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/medium_low_speed.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3262 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/minimalistic_user.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6855 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/minimalistic_user.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      917 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/icons/multi-document-save.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6072 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/icons/multi-document-save.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      176 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/nabu.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3999 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/nabu.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1025 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/output.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3492 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/output.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2775 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/parameters.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5950 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/icons/parameters.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1623 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/plot-xleft.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6774 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/plot-xleft.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1613 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/plot-xright.png
--rw-r--r--   0 payno     (1000) payno     (1000)     6779 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/plot-xright.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      738 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/range_selection.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1188 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/range_selection.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     9722 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/results.png
--rw-r--r--   0 payno     (1000) payno     (1000)     5148 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/results.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      348 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/rm.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1987 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/rm.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      773 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_four.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4648 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_four.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      302 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_one.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3545 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_one.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      406 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_three.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4573 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_three.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      341 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_two.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4061 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/roman_two.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1694 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/icons/ruler.png
--rw-r--r--   0 payno     (1000) payno     (1000)    10249 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/icons/ruler.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      359 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/icons/short_description.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1857 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/icons/short_description.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      543 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/single_selection.png
--rw-r--r--   0 payno     (1000) payno     (1000)      968 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/single_selection.svg
--rw-r--r--   0 payno     (1000) payno     (1000)   134176 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/sinogram.png
--rw-r--r--   0 payno     (1000) payno     (1000)     7184 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/slurm.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2981 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/slurm_active.png
--rw-r--r--   0 payno     (1000) payno     (1000)    10260 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/slurm_active.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     3126 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/slurm_deactive.png
--rw-r--r--   0 payno     (1000) payno     (1000)    10264 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/slurm_deactive.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     1979 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRaw.png
--rw-r--r--   0 payno     (1000) payno     (1000)     9666 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRaw.svg
--rw-r--r--   0 payno     (1000) payno     (1000)    11417 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRefine.png
--rw-r--r--   0 payno     (1000) payno     (1000)    13156 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRefine.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      491 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/switch.png
--rw-r--r--   0 payno     (1000) payno     (1000)    24955 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/tomwer.png
--rw-r--r--   0 payno     (1000) payno     (1000)   176673 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/tomwer_large.png
--rw-r--r--   0 payno     (1000) payno     (1000)      365 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/unlocked.png
--rw-r--r--   0 payno     (1000) payno     (1000)     2141 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/unlocked.svg
--rw-r--r--   0 payno     (1000) payno     (1000)   100796 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/unsharp_mask.png
--rw-r--r--   0 payno     (1000) payno     (1000)    17140 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/update_stitching_preview.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      346 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/icons/url.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1909 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/icons/url.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      801 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/vignettes.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3252 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/vignettes.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      419 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/visible.png
--rw-r--r--   0 payno     (1000) payno     (1000)     8072 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/resources/gui/icons/visible.svg
--rw-r--r--   0 payno     (1000) payno     (1000)     2348 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/warning.png
--rw-r--r--   0 payno     (1000) payno     (1000)     1462 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/icons/warning.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/resources/gui/illustrations/
--rw-r--r--   0 payno     (1000) payno     (1000)     7752 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/illustrations/ctf_z1.png
--rw-r--r--   0 payno     (1000) payno     (1000)    36320 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/resources/gui/illustrations/ctf_z1.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      551 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_down.png
--rw-r--r--   0 payno     (1000) payno     (1000)     3987 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_down.svg
--rw-r--r--   0 payno     (1000) payno     (1000)      531 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_right.png
--rw-r--r--   0 payno     (1000) payno     (1000)     4235 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_right.svg
--rw-r--r--   0 payno     (1000) payno     (1000)    33290 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/resources/gui/illustrations/no_rot.svg
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/synctools/
--rw-r--r--   0 payno     (1000) payno     (1000)      137 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/synctools/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1958 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/axis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1813 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/darkref.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9717 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/datalistener.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1826 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/synctools/datatransfert.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2860 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/imageloaderthread.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6227 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/rsyncmanager.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1984 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/saaxis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2009 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/sadeltabeta.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/synctools/stacks/
--rw-r--r--   0 payno     (1000) payno     (1000)      165 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/synctools/stacks/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/synctools/stacks/control/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/synctools/stacks/control/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5100 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/synctools/stacks/control/datalistener.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/synctools/stacks/edit/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/synctools/stacks/edit/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6646 2024-02-28 08:43:13.000000 tomwer-1.3.6/tomwer/synctools/stacks/edit/darkflatpatch.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5259 2024-02-23 14:39:44.000000 tomwer-1.3.6/tomwer/synctools/stacks/edit/imagekeyeditor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6873 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/synctools/stacks/processingstack.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8876 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/axis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7552 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/castvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7040 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/dkrefcopy.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7816 2024-03-11 14:33:51.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/nabu.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5362 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7126 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/saaxis.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7114 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/sadeltabeta.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/synctools/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/synctools/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15799 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/synctools/test/test_darkRefs.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14212 2024-03-25 10:55:06.000000 tomwer-1.3.6/tomwer/synctools/test/test_foldertransfer.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/synctools/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.6/tomwer/synctools/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9263 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/synctools/utils/scanstages.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/tests/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/tests/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1912 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/tests/conftest.py
--rw-r--r--   0 payno     (1000) payno     (1000)      335 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/tests/datasets.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5117 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/tests/test_scripts.py
--rw-r--r--   0 payno     (1000) payno     (1000)      305 2023-10-02 08:41:00.000000 tomwer-1.3.6/tomwer/tests/test_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)      107 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/tests/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer/third_part/
--rw-r--r--   0 payno     (1000) payno     (1000)     3906 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/third_part/WaitingOverlay.py
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-24 11:58:20.000000 tomwer-1.3.6/tomwer/third_part/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8465 2024-01-22 10:03:25.000000 tomwer-1.3.6/tomwer/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4386 2024-03-25 10:56:12.000000 tomwer-1.3.6/tomwer/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-25 10:56:28.925650 tomwer-1.3.6/tomwer.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)    11254 2024-03-25 10:56:28.000000 tomwer-1.3.6/tomwer.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)    35717 2024-03-25 10:56:28.000000 tomwer-1.3.6/tomwer.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-03-25 10:56:28.000000 tomwer-1.3.6/tomwer.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      440 2024-03-25 10:56:28.000000 tomwer-1.3.6/tomwer.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       14 2024-03-25 10:56:28.000000 tomwer-1.3.6/tomwer.egg-info/namespace_packages.txt
--rw-r--r--   0 payno     (1000) payno     (1000)     1982 2024-03-25 10:56:28.000000 tomwer-1.3.6/tomwer.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       21 2024-03-25 10:56:28.000000 tomwer-1.3.6/tomwer.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.064374 tomwer-1.3.7/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1877 2023-07-19 16:04:34.000000 tomwer-1.3.7/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 16:04:34.000000 tomwer-1.3.7/MANIFEST.in
+-rw-r--r--   0 payno     (1000) payno     (1000)    11254 2024-04-11 07:39:57.064374 tomwer-1.3.7/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     2709 2024-01-22 10:03:25.000000 tomwer-1.3.7/README.rst
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/orangecontrib/
+-rw-r--r--   0 payno     (1000) payno     (1000)      277 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/orangecontrib/tomwer/
+-rw-r--r--   0 payno     (1000) payno     (1000)      148 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/orangecontrib/tomwer/orange/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/orange/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4621 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/orange/managedprocess.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2044 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/orange/settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1711 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/state_summary.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/orangecontrib/tomwer/tutorials/
+-rw-r--r--   0 payno     (1000) payno     (1000)     4747 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/EBS_tomo_listener.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5485 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/append_raw_darks_and_flats_frames_to_NXtomos.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     2918 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/cast_volume.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     6208 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth1.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     5204 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth2.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     4699 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/default_cor_search.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     3670 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/hello_world_python_script.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     8534 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/icat_publication.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     4435 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_slice_reconstruction.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     6584 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_slice_reconstruction_on_slurm.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     5945 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_volume_local_reconstruction.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     7809 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_volume_to_slurm_reconstruction.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     5192 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/tutorials/using_saaxis_to_find_cor.ows
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/orangecontrib/tomwer/widgets/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2526 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/
+-rw-r--r--   0 payno     (1000) payno     (1000)     8961 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/FutureSupervisorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4034 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/SlurmClusterOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1614 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1995 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurm.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     9790 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurm.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3212 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    56984 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2460 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/AdvancementOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8041 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataDiscoveryOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4774 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataListOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15242 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataListenerOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5159 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataSelectorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7262 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataTransfertOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7113 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataValidatorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7403 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataWatcherOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9888 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/EDF2NXTomomillOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2493 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/EmailOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4659 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/FilterOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3271 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NXTomomillMixIn.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13995 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NXTomomillOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6416 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NXtomoConcatenate.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4237 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NotifierOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2836 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/ReduceDarkFlatSelectorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6790 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/SingleTomoObjOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4395 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/TimerOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3203 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/TomoObjSerieOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5144 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/VolumeSelector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6626 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/VolumeSymLinkOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1545 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)      729 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/advancement.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5781 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/advancement.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      768 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    14318 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      598 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datadiscover.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3772 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datadiscover.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2100 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datalistener.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3136 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datalistener.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3351 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datawatcher.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1306 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/edf2nx.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     7039 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/edf2nx.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      755 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/email.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1836 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/email.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   105862 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/esrf.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5645 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/folder-transfert.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1077 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/image_key_upgrader.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2072 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/namefilter.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3757 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/namefilter.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2600 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/notification.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4587 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/notification.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)    66863 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/nxtomomill.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    11185 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/nxtomomill.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2516 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/progress.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3864 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    39604 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2873 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/scanlist.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1463 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/scanselector.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2129 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/scanselector.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      351 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/single_tomo_obj.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3615 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/single_tomo_obj.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3641 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/time.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3116 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5900 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8992 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/tomwer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     9358 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/validator.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     9592 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/validatorcrack.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1525 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumeselector.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    10936 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumeselector.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1895 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumesymlink.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5786 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumesymlink.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/
+-rw-r--r--   0 payno     (1000) payno     (1000)     6374 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/DatasetGeneratorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2436 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/ObjectInspectorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1553 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2034 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/hammer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3191 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/hammer.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1020 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/inspector.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3943 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/inspector.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/
+-rw-r--r--   0 payno     (1000) payno     (1000)     6399 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/DarkFlatPatchOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4467 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/ImageKeyEditorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4820 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/ImageKeyUpgraderOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3817 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/NXtomoEditorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1555 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)      878 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     7396 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      998 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    13531 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1026 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     8204 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1522 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    29749 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2832 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_dark_flat_patch.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2129 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_image_key_editor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2211 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_image_key_upgrader.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5888 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_nxtomo_editor.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3481 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/PublishProcessedDataOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/RawDataScreenshotCreatorOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4532 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/SaveToGalleryAndPublishOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      267 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.028374 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1271 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/add_gallery.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5147 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/add_gallery.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2866 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    22489 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1120 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6358 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)     8992 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6731 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_build.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    15969 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_build.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     7491 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_cluster.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    22047 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_cluster.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     7057 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_control.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    19095 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_control.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)    18651 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    31006 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     7306 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    15202 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8172 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_edit.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    17150 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_edit.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     7194 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_other.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    16763 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_other.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8066 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_stitching.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    22169 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_stitching.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8760 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_visu.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    18818 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_visu.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/
+-rw-r--r--   0 payno     (1000) payno     (1000)    27790 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/PythonScriptOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      886 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/TomoObjsHub.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1512 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)     5501 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/icons/PythonScript.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1122 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/icons/hub.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3735 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/other/icons/hub.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/
+-rw-r--r--   0 payno     (1000) payno     (1000)    22342 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/AxisOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9604 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/CastNabuVolumeOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10988 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/DarkRefAndCopyOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5967 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/NabuHelicalPrepareWeightsDoubleOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12673 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/NabuOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19195 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/NabuVolumeOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    18724 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/SAAxisOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15480 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/SADeltaBetaOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10720 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/SinoNormOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1601 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1286 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/axis.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5426 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/axis.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8121 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/bricks.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    24845 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    33704 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     5509 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    14957 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   105862 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/esrf.png
+-rw-r--r--   0 payno     (1000) payno     (1000)      176 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_2d.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3999 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_2d.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2940 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6178 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3023 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    11959 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      163 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_prepare_weights_double.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5136 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_prepare_weights_double.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2784 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     7303 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      791 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6778 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3305 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    13025 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     4107 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    14712 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     6846 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/tomogui.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     8992 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/tomwer.png
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/stitching/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2351 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/stitching/StitcherOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3252 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/stitching/ZStitchingConfigOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      262 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/stitching/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2339 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/
+-rw-r--r--   0 payno     (1000) payno     (1000)     5382 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/DataViewerOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2855 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/DiffViewerOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3145 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/LivesliceOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1918 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/NXtomoMetadataViewerOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3421 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/RadioStackOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4093 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/SampleMovedOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3211 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/SinogramViewerOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4092 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/SliceStackOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1865 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/VolumeViewerOW.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1604 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)      378 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/diff.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     7693 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/diff.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   105862 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/esrf.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    11631 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/eye.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4279 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/eyecrack.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1392 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/liveslice.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3349 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/liveslice.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1114 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    22650 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2704 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2498 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1281 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1228 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   134176 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/sinogramviewer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2454 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6967 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8992 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/tomwer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4372 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     8454 2024-04-11 07:10:45.000000 tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3267 2024-04-11 07:39:57.068374 tomwer-1.3.7/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1474 2023-10-02 08:41:00.000000 tomwer-1.3.7/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.032374 tomwer-1.3.7/tomwer/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1745 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8575 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/__main__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6004 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/axis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1561 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/canvas.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/app/canvas_launcher/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/canvas_launcher/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7164 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/canvas_launcher/config.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2501 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/canvas_launcher/environ.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19146 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/canvas_launcher/mainwindow.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      560 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/canvas_launcher/splash.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2859 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/canvas_launcher/widgetsscheme.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      276 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/darkref.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      285 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/darkrefpatch.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3166 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/diffframe.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2821 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/imagekeyeditor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3217 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/imagekeyupgrader.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6660 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/intensitynormalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9940 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/multicor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12799 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/multipag.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7646 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/nabuapp.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2837 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/nxtomoeditor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3827 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/patchrawdarkflat.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2587 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/radiostack.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6520 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/reducedarkflat.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4081 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/rsync.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2527 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/samplemoved.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2708 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/scanviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3677 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/sinogramviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2428 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/slicestack.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      957 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/stopdatalistener.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12877 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/app/zstitching.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1373 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/cluster/
+-rw-r--r--   0 payno     (1000) payno     (1000)       60 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/cluster/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5744 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/cluster/cluster.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6441 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/futureobject.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/log/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/log/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4099 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/log/logger.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3697 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/log/processlog.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/cluster/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/cluster/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1755 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/cluster/supervisor.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/conditions/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/conditions/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7156 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/conditions/filters.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/control/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      377 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datadiscovery.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/control/datalistener/
+-rw-r--r--   0 payno     (1000) payno     (1000)       52 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datalistener/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    22087 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datalistener/datalistener.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11104 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datalistener/rpcserver.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/control/datawatcher/
+-rw-r--r--   0 payno     (1000) payno     (1000)       50 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datawatcher/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16822 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datawatcher/datawatcher.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    25752 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datawatcher/datawatcherobserver.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9450 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datawatcher/datawatcherprocess.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7209 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datawatcher/edfdwprocess.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3027 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datawatcher/hdf5dwprocess.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3074 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/datawatcher/status.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4806 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/emailnotifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3826 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/nxtomoconcatenate.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9559 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/nxtomomill.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2048 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/scanlist.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/scanselector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    26592 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/scantransfer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10611 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/scanvalidator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      555 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/singletomoobj.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/control/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2176 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/test/test_concatenate_nxtomos.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1553 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/test/test_email.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5472 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/test/test_h52nx_process.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3238 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/test/test_volume_link.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3635 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/timer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      266 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/tomoobjserie.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      370 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/volumeselector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7626 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/control/volumesymlink.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/edit/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/edit/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5239 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/edit/darkflatpatch.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9398 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/edit/imagekeyeditor.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/icat/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/icat/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3677 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/icat/createscreenshots.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14813 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/icat/gallery.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1066 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/icat/icatbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7828 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/icat/publish.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      816 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/icat/screenshots.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1562 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/output.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.036374 tomwer-1.3.7/tomwer/core/process/reconstruction/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1504 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/axis/
+-rw-r--r--   0 payno     (1000) payno     (1000)       80 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/axis/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1896 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/axis/anglemode.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    42723 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/axis/axis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6750 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/axis/mode.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    33185 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/axis/params.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1543 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/axis/projectiontype.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    20862 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/darkrefs.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13276 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/darkrefscopy.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10080 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/params.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      188 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/settings.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10239 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/castvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1997 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/helical.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    24428 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabucommon.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    25702 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabuscores.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    38731 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabuslices.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    21916 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabuvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      134 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/plane.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2279 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1481 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/target.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17950 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/normalization/
+-rw-r--r--   0 payno     (1000) payno     (1000)      119 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/normalization/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13210 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/normalization/normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4790 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/normalization/params.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3967 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/output.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7725 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/paramsbase.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/saaxis/
+-rw-r--r--   0 payno     (1000) payno     (1000)      137 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/saaxis/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5583 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/saaxis/params.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    31985 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/saaxis/saaxis.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/sadeltabeta/
+-rw-r--r--   0 payno     (1000) payno     (1000)      162 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/sadeltabeta/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4043 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/sadeltabeta/params.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    30925 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/sadeltabeta/sadeltabeta.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/scores/
+-rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/scores/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7564 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/scores/params.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7383 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/scores/scores.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1614 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_axis_params.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2429 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_darkref.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6090 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_darkref_copy.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1505 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_paramsbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4295 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_saaxis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2555 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_sadeltabeta.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1006 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/reconstruction/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/reconstruction/utils/cor.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/script/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/script/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4028 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/script/python.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/stitching/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/stitching/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6527 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/stitching/metadataholder.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6781 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/stitching/nabustitcher.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15703 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/task.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11810 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_axis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3464 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_conditions.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15444 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_dark_and_flat.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3696 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_data_listener.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15419 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_data_transfer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3138 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_data_watcher.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19621 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_nabu.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4014 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3027 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/test/test_timer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4010 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/process/visualization/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1656 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/dataviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1594 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/diffviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1577 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/imagestackviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      198 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/liveslice.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1615 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/radiostack.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1601 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/samplemoved.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1569 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/sinogramviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1625 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/slicestack.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1579 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/process/visualization/volumeviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3246 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/progress.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/scan/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1392 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8244 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/blissscan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    22892 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/edfscan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      213 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/futurescan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      980 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/hdf5scan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      472 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/helicalmetadata.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19405 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/nxtomoscan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    32052 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/scanbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10521 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/scanfactory.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      137 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/scantype.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/scan/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2210 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/test/test_edf.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2171 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/test/test_future_scan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3644 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/test/test_h5.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3919 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/test/test_process_registration.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12228 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/scan/test/test_scan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5358 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6115 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/signal.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.040374 tomwer-1.3.7/tomwer/core/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2197 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/test/test_scanutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10668 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/test/test_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1745 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/tomwer_object.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/core/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1559 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/Singleton.py
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1718 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/char.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4716 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/deprecation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      601 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/dictutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2382 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/ftseriesutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1812 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/gpu.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4979 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/image.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      988 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/lbsram.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3096 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/locker.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1434 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/logconfig.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2900 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2685 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/nxtomoutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1932 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/resource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15641 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/scanutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1923 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/slurm.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7560 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/spec.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3189 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/threads.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1845 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/time.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      490 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/utils/volumeutils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/core/volume/
+-rw-r--r--   0 payno     (1000) payno     (1000)      253 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3713 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/edfvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4401 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/hdf5volume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3717 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/jp2kvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4082 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/rawvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6040 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/tiffvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1539 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/volumebase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7979 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/core/volume/volumefactory.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1474 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/cluster/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/cluster/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    27604 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/cluster/slurm.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17117 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/cluster/supervisor.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/cluster/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/cluster/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3937 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/cluster/test/test_cluster.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3212 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/cluster/test/test_supervisor.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/conditions/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/conditions/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5549 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/conditions/filter.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/configuration/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/configuration/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2512 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/configuration/action.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      653 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/configuration/level.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/control/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4677 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/actions.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6108 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datadiscovery.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    40898 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datalist.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    18471 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datalistener.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2572 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datareacheractions.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5702 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datatransfert.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14463 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datavalidator.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/control/datawatcher/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1444 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datawatcher/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10193 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datawatcher/configuration.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3857 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datawatcher/controlwidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    22592 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datawatcher/datawatcher.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10543 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/datawatcher/datawatcherobserver.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6383 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/emailnotifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4826 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/history.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7293 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/nxtomomill.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7735 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/observations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    20536 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/reducedarkflatselector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2356 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/scanselectorwidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5571 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/selectorwidgetbase.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/control/serie/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/serie/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3131 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/serie/nxtomoconcatenate.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    35110 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/serie/seriecreator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1374 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/serie/seriewaiter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6777 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/singletomoobj.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/control/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      775 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_datadiscovery.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3508 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_datalist.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3151 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_datalistener.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2017 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_datavalidator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1140 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_email.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3135 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_inputwidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2547 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_process_manager.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9430 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_reducedarkflat_selector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2581 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_scanselector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3904 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_scanvalidator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2278 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_single_tomo_obj.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8164 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_volume_dialog.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3407 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/test/test_volumeselector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      159 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/tomoobjdisplaymode.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2082 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/control/volumeselectorwidget.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.044374 tomwer-1.3.7/tomwer/gui/debugtools/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/debugtools/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10641 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/debugtools/datasetgenerator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2925 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/debugtools/objectinspector.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/edit/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17533 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/dkrfpatch.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    29728 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/imagekeyeditor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    28095 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/nxtomoeditor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2349 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/nxtomowarmer.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/edit/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8001 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/test/test_dkrf_patch.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5965 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/test/test_image_key_editor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11285 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/edit/test/test_nx_editor.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/icat/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/icat/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3123 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/icat/createscreenshots.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8700 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/icat/gallery.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6220 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/icat/publish.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12917 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/icons.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/illustrations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5501 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/imagefromfile.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      713 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/qconfigfile.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    22761 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/qfolderdialog.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      534 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/qlefilesystem.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/axis/
+-rw-r--r--   0 payno     (1000) payno     (1000)    12870 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/axis/CompareImages.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       94 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/axis/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    27260 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/axis/axis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    92610 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/axis/radioaxis.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/darkref/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1373 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/darkref/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11562 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/darkref/darkrefcopywidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16468 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/darkref/darkrefwidget.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/
+-rw-r--r--   0 payno     (1000) payno     (1000)       44 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15003 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/castvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4717 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/check.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3708 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/helical.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/
+-rw-r--r--   0 payno     (1000) payno     (1000)       77 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3459 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/base.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13085 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/ctf.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11529 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/nabuconfig.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13952 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/output.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/phase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    30942 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/preprocessing.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    38981 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/reconstruction.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16941 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuflow.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    23549 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/slices.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2591 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/slurm.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19441 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/nabu/volume.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/normalization/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/normalization/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    33856 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/normalization/intensity.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    32888 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/corrangeselector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9750 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/dimensionwidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    21065 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/saaxis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12213 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/sliceselector.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/sadeltabeta/
+-rw-r--r--   0 payno     (1000) payno     (1000)       57 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/sadeltabeta/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    20396 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/sadeltabeta/saadeltabeta.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/scores/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/scores/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2826 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/scores/control.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    32001 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/scores/scoreplot.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/reconstruction/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8867 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/test/test_axis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14584 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/test/test_nabu.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8128 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/test/test_saaxis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5799 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/reconstruction/test/test_sadeltabeta.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/samplemoved/
+-rw-r--r--   0 payno     (1000) payno     (1000)     9669 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/samplemoved/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9401 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/samplemoved/selectiontable.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      244 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    25517 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stackplot.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8650 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stacks.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/stitching/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1659 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/action.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17314 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/axisorderedlist.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/stitching/config/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/config/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7578 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/config/axisparams.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5902 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/config/output.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6834 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/config/positionoveraxis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4257 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/config/stitchingstrategies.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14680 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/config/tomoobjdetails.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      913 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/metadataholder.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4454 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5982 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/stitchandbackground.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    57013 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/stitching.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9669 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/stitching_preview.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    22353 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/stitching_raw.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/stitching/z_stitching/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/z_stitching/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8931 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/stitching/z_stitching/fineestimation.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1447 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/test/test_axis_gui.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      347 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/test/test_qfolder_dialog.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.048374 tomwer-1.3.7/tomwer/gui/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)       66 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6933 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/buttons.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4979 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/completer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12091 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/flow.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4449 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/illustrations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    24431 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/inputwidget.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.052374 tomwer-1.3.7/tomwer/gui/utils/lineselector/
+-rw-r--r--   0 payno     (1000) payno     (1000)       75 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/lineselector/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8179 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/lineselector/lineselector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      210 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/qt_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7460 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/sandboxes.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3373 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/scandescription.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2954 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/scrollarea.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3482 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/slider.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1857 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/splashscreen.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5343 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/step.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8117 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/unitsystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2675 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19198 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/vignettes.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1844 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/utils/waiterthread.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.052374 tomwer-1.3.7/tomwer/gui/visualization/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    27024 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/dataviewer.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.052374 tomwer-1.3.7/tomwer/gui/visualization/diffviewer/
+-rw-r--r--   0 payno     (1000) payno     (1000)       39 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/diffviewer/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    21812 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/diffviewer/diffviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    20928 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/diffviewer/shiftwidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3639 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/fullscreenplot.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      683 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/nxtomometadata.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10230 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/reconstructionparameters.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9224 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/scanoverview.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9707 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/sinogramviewer.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.052374 tomwer-1.3.7/tomwer/gui/visualization/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1368 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2446 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/test_dataviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3536 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/test_diffviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2548 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/test_nx_tomo_metadata_viewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3227 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/test_reconstruction_parameters.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3068 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/test_sinogramviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4694 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/test_stacks.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2374 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/test/test_volumeviewer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1991 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/tomoobjoverview.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2491 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/volumeoverview.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16335 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/gui/visualization/volumeviewer.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.052374 tomwer-1.3.7/tomwer/io/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/io/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.052374 tomwer-1.3.7/tomwer/io/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)      272 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/io/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2964 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/io/utils/h5pyutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3208 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/io/utils/raw_and_processed_data.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2828 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/io/utils/tomoobj.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10678 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/io/utils/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.052374 tomwer-1.3.7/tomwer/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)     5904 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.024374 tomwer-1.3.7/tomwer/resources/gui/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.056374 tomwer-1.3.7/tomwer/resources/gui/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)  1618960 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/Imagej_icon.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3858 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/a.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2650 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/a.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      470 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/add.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2254 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/add.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     4639 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/advanced_user.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     8162 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/advanced_user.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8909 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/axis.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    12185 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/axis.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3876 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/background.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    10778 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/background.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     4694 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/basic_user.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     9246 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/basic_user.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2150 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_active.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     7344 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_active.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1979 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_inactive.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     7519 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_inactive.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3862 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/compare_mode_a_minus_b.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     9139 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/compare_mode_a_minus_b.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      873 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/compose.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2813 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/compose.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2443 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_activate.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3472 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_activate.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2588 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_deactivate.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3857 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_deactivate.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1869 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/delta_beta.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2426 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/delta_beta.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1002 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/exit.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    10773 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/exit.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      674 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/full_screen.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    18573 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/full_screen.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/hammer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2472 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/hammer.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2134 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/health.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2817 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/health.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3868 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/high_speed.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2365 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/high_speed.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     4466 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/history.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    16464 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/hourglass.npy
+-rw-r--r--   0 payno     (1000) payno     (1000)   131152 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/imageNotFound.npy
+-rw-r--r--   0 payno     (1000) payno     (1000)     3432 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/information.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4512 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/information.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1022 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/input.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3324 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/input.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      741 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/invisible.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4366 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/invisible.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2968 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/lineselection.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3266 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/lineselection.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1648 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/list_selection.png
+-rw-r--r--   0 payno     (1000) payno     (1000)      982 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/list_selection.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      344 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/locked.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2973 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/locked.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      633 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/log.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2207 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/log.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2981 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/loop.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3839 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/low_speed.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2362 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/low_speed.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3836 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/medium_low_speed.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2361 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/medium_low_speed.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3262 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/minimalistic_user.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6855 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/minimalistic_user.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      917 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/multi-document-save.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6072 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/multi-document-save.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      176 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/nabu.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3999 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/nabu.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1025 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/output.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3492 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/output.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2775 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/parameters.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5950 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/parameters.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1623 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/plot-xleft.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6774 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/plot-xleft.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1613 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/plot-xright.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6779 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/plot-xright.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      738 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/range_selection.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1188 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/range_selection.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     9722 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/results.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5148 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/results.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      348 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/rm.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1987 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/rm.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      773 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_four.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4648 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_four.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      302 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_one.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3545 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_one.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      406 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_three.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4573 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_three.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      341 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_two.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4061 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/roman_two.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1694 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/ruler.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    10249 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/ruler.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      359 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/short_description.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1857 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/short_description.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      543 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/single_selection.png
+-rw-r--r--   0 payno     (1000) payno     (1000)      968 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/single_selection.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   134176 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/sinogram.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     7184 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/slurm.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2981 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/slurm_active.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    10260 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/slurm_active.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3126 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/slurm_deactive.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    10264 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/slurm_deactive.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1979 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRaw.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     9666 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRaw.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)    11417 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRefine.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    13156 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRefine.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      491 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/switch.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    24955 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/tomwer.png
+-rw-r--r--   0 payno     (1000) payno     (1000)   176673 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/tomwer_large.png
+-rw-r--r--   0 payno     (1000) payno     (1000)      365 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/unlocked.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2141 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/unlocked.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   100796 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/unsharp_mask.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    17140 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/update_stitching_preview.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      346 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/url.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1909 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/url.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      801 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/vignettes.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3252 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/vignettes.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      419 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/visible.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     8072 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/visible.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2348 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/warning.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     1462 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/icons/warning.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.056374 tomwer-1.3.7/tomwer/resources/gui/illustrations/
+-rw-r--r--   0 payno     (1000) payno     (1000)     7752 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/illustrations/ctf_z1.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    36320 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/illustrations/ctf_z1.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      551 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_down.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3987 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_down.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      531 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_right.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4235 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_right.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)    33290 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/resources/gui/illustrations/no_rot.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.056374 tomwer-1.3.7/tomwer/synctools/
+-rw-r--r--   0 payno     (1000) payno     (1000)      137 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1958 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/axis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1813 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/darkref.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9717 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/datalistener.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1826 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/datatransfert.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2860 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/imageloaderthread.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6227 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/rsyncmanager.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1984 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/saaxis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2009 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/sadeltabeta.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/synctools/stacks/
+-rw-r--r--   0 payno     (1000) payno     (1000)      165 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/synctools/stacks/control/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/control/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5100 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/control/datalistener.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/synctools/stacks/edit/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/edit/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6646 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/edit/darkflatpatch.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5259 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/edit/imagekeyeditor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6873 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/processingstack.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8876 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/axis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8282 2024-04-11 07:38:59.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/castvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7040 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/dkrefcopy.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7816 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/nabu.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5362 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7126 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/saaxis.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7114 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/sadeltabeta.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/synctools/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15799 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/test/test_darkRefs.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14212 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/test/test_foldertransfer.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/synctools/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9263 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/synctools/utils/scanstages.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/tests/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/tests/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1912 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/tests/conftest.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      335 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/tests/datasets.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5117 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/tests/test_scripts.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      305 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/tests/test_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      107 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/tests/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer/third_part/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3906 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/third_part/WaitingOverlay.py
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/third_part/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8465 2024-04-11 07:10:45.000000 tomwer-1.3.7/tomwer/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4386 2024-04-11 07:39:32.000000 tomwer-1.3.7/tomwer/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-11 07:39:57.060374 tomwer-1.3.7/tomwer.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)    11254 2024-04-11 07:39:56.000000 tomwer-1.3.7/tomwer.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)    35717 2024-04-11 07:39:56.000000 tomwer-1.3.7/tomwer.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-11 07:39:56.000000 tomwer-1.3.7/tomwer.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      440 2024-04-11 07:39:56.000000 tomwer-1.3.7/tomwer.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       14 2024-04-11 07:39:56.000000 tomwer-1.3.7/tomwer.egg-info/namespace_packages.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)     1982 2024-04-11 07:39:56.000000 tomwer-1.3.7/tomwer.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       21 2024-04-11 07:39:56.000000 tomwer-1.3.7/tomwer.egg-info/top_level.txt
```

### Comparing `tomwer-1.3.6/LICENSE` & `tomwer-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/PKG-INFO` & `tomwer-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomwer
-Version: 1.3.6
+Version: 1.3.7
 Summary: "tomography workflow tools"
 Home-page: https://gitlab.esrf.fr/tomotools/tomwer
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomwer/-/issues
 Keywords: orange3 add-on,ewoks
```

### Comparing `tomwer-1.3.6/README.rst` & `tomwer-1.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/orange/managedprocess.py` & `tomwer-1.3.7/orangecontrib/tomwer/orange/managedprocess.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/orange/settings.py` & `tomwer-1.3.7/orangecontrib/tomwer/orange/settings.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/state_summary.py` & `tomwer-1.3.7/orangecontrib/tomwer/state_summary.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/EBS_tomo_listener.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/EBS_tomo_listener.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/append_raw_darks_and_flats_frames_to_NXtomos.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/append_raw_darks_and_flats_frames_to_NXtomos.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/cast_volume.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/cast_volume.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth1.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth1.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth2.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/copy_reduced_darks_and_flats_meth2.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/default_cor_search.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/default_cor_search.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/hello_world_python_script.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/hello_world_python_script.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/icat_publication.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/icat_publication.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_slice_reconstruction.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_slice_reconstruction.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_slice_reconstruction_on_slurm.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_slice_reconstruction_on_slurm.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_volume_local_reconstruction.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_volume_local_reconstruction.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/simple_volume_to_slurm_reconstruction.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/simple_volume_to_slurm_reconstruction.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/tutorials/using_saaxis_to_find_cor.ows` & `tomwer-1.3.7/orangecontrib/tomwer/tutorials/using_saaxis_to_find_cor.ows`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/FutureSupervisorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/FutureSupervisorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/SlurmClusterOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/SlurmClusterOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurm.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurm.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurm.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurm.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/cluster/icons/slurmobserver.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/AdvancementOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/AdvancementOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataDiscoveryOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataDiscoveryOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataListOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataListOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataListenerOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataListenerOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataSelectorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataSelectorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataTransfertOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataTransfertOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataValidatorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataValidatorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/DataWatcherOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/DataWatcherOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/EDF2NXTomomillOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/EDF2NXTomomillOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/EmailOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/EmailOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/FilterOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/FilterOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NXTomomillMixIn.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NXTomomillMixIn.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NXTomomillOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NXTomomillOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NXtomoConcatenate.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NXtomoConcatenate.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/NotifierOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/NotifierOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/ReduceDarkFlatSelectorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/ReduceDarkFlatSelectorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/SingleTomoObjOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/SingleTomoObjOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/TimerOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/TimerOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/TomoObjSerieOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/TomoObjSerieOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/VolumeSelector.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/VolumeSelector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/VolumeSymLinkOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/VolumeSymLinkOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/advancement.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/advancement.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/advancement.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/advancement.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/concatenate_nxtomos.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datadiscover.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datadiscover.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datadiscover.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datadiscover.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datalistener.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datalistener.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datalistener.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datalistener.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/datawatcher.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/datawatcher.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/edf2nx.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/edf2nx.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/edf2nx.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/edf2nx.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/email.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/email.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/email.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/email.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/esrf.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/esrf.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/folder-transfert.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/folder-transfert.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/image_key_upgrader.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/image_key_upgrader.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/namefilter.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/namefilter.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/namefilter.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/namefilter.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/notification.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/notification.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/notification.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/notification.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/nxtomomill.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/nxtomomill.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/nxtomomill.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/nxtomomill.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/progress.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/progress.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/reduced_darkflat_selector.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/scanlist.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/scanlist.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/scanselector.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/scanselector.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/scanselector.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/scanselector.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/single_tomo_obj.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/single_tomo_obj.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/time.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/time.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/tomoobjserie.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/tomwer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/tomwer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/validator.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/validator.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/validatorcrack.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/validatorcrack.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumeselector.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumeselector.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumeselector.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumeselector.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumesymlink.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumesymlink.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/control/icons/volumesymlink.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/control/icons/volumesymlink.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/DatasetGeneratorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/DatasetGeneratorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/ObjectInspectorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/ObjectInspectorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/hammer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/hammer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/hammer.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/hammer.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/inspector.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/inspector.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/debugtools/icons/inspector.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/debugtools/icons/inspector.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/DarkFlatPatchOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/DarkFlatPatchOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/ImageKeyEditorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/ImageKeyEditorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/ImageKeyUpgraderOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/ImageKeyUpgraderOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/NXtomoEditorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/NXtomoEditorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_editor.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/image_key_upgrader.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/nx_tomo_editor.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/icons/patch_dark_flat.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_dark_flat_patch.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_dark_flat_patch.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_image_key_editor.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_image_key_editor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_image_key_upgrader.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_image_key_upgrader.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/edit/test/test_nxtomo_editor.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/edit/test/test_nxtomo_editor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/PublishProcessedDataOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/PublishProcessedDataOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/RawDataScreenshotCreatorOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/RawDataScreenshotCreatorOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/SaveToGalleryAndPublishOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/SaveToGalleryAndPublishOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/add_gallery.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/add_gallery.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/add_gallery.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/add_gallery.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/publish_processed_data.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icat/icons/raw_screenshots.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_build.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_build.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_build.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_build.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_cluster.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_cluster.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_cluster.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_cluster.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_control.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_control.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_control.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_control.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_data_portal.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_debug_tools.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_edit.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_edit.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_edit.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_edit.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_other.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_other.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_other.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_other.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_stitching.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_stitching.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_stitching.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_stitching.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_visu.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_visu.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/icons/tomwer_visu.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/icons/tomwer_visu.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/other/PythonScriptOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/other/PythonScriptOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/other/TomoObjsHub.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/other/TomoObjsHub.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/other/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/other/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/other/icons/PythonScript.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/other/icons/PythonScript.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/other/icons/hub.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/other/icons/hub.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/other/icons/hub.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/other/icons/hub.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/AxisOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/AxisOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/CastNabuVolumeOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/CastNabuVolumeOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/DarkRefAndCopyOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/DarkRefAndCopyOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/NabuHelicalPrepareWeightsDoubleOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/NabuHelicalPrepareWeightsDoubleOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/NabuOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/NabuOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/NabuVolumeOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/NabuVolumeOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/SAAxisOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/SAAxisOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/SADeltaBetaOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/SADeltaBetaOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/SinoNormOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/SinoNormOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/axis.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/axis.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/axis.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/axis.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/bricks.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/bricks.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/darkref.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/delta_beta_range.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/esrf.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/esrf.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_2d.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_2d.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_3d.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_cast.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_prepare_weights_double.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/nabu_prepare_weights_double.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/norm_I.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/refCopy.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/saaxis.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/sadeltabeta.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/tomogui.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/tomogui.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/reconstruction/icons/tomwer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/reconstruction/icons/tomwer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/stitching/StitcherOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/stitching/StitcherOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/stitching/ZStitchingConfigOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/stitching/ZStitchingConfigOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/utils.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/DataViewerOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/DataViewerOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/DiffViewerOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/DiffViewerOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/LivesliceOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/LivesliceOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/NXtomoMetadataViewerOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/NXtomoMetadataViewerOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/RadioStackOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/RadioStackOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/SampleMovedOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/SampleMovedOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/SinogramViewerOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/SinogramViewerOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/SliceStackOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/SliceStackOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/VolumeViewerOW.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/VolumeViewerOW.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/__init__.py` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/diff.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/diff.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/esrf.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/esrf.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/eye.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/eye.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/eyecrack.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/eyecrack.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/liveslice.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/liveslice.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/liveslice.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/liveslice.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/nx_tomo_metadata_viewer.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/radiosstack.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/sampleMoved.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/sinogramviewer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/sinogramviewer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/slicesstack.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/tomwer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/tomwer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.png` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.svg` & `tomwer-1.3.7/orangecontrib/tomwer/widgets/visualization/icons/volumeviewer.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/setup.cfg` & `tomwer-1.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/setup.py` & `tomwer-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/__init__.py` & `tomwer-1.3.7/tomwer/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/__main__.py` & `tomwer-1.3.7/tomwer/__main__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/axis.py` & `tomwer-1.3.7/tomwer/app/axis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/canvas.py` & `tomwer-1.3.7/tomwer/app/canvas.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/canvas_launcher/config.py` & `tomwer-1.3.7/tomwer/app/canvas_launcher/config.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/canvas_launcher/environ.py` & `tomwer-1.3.7/tomwer/app/canvas_launcher/environ.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/canvas_launcher/mainwindow.py` & `tomwer-1.3.7/tomwer/app/canvas_launcher/mainwindow.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/canvas_launcher/splash.py` & `tomwer-1.3.7/tomwer/app/canvas_launcher/splash.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/canvas_launcher/widgetsscheme.py` & `tomwer-1.3.7/tomwer/app/canvas_launcher/widgetsscheme.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/diffframe.py` & `tomwer-1.3.7/tomwer/app/diffframe.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/imagekeyeditor.py` & `tomwer-1.3.7/tomwer/app/imagekeyeditor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/imagekeyupgrader.py` & `tomwer-1.3.7/tomwer/app/imagekeyupgrader.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/intensitynormalization.py` & `tomwer-1.3.7/tomwer/app/intensitynormalization.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/multicor.py` & `tomwer-1.3.7/tomwer/app/multicor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/multipag.py` & `tomwer-1.3.7/tomwer/app/multipag.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/nabuapp.py` & `tomwer-1.3.7/tomwer/app/nabuapp.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/nxtomoeditor.py` & `tomwer-1.3.7/tomwer/app/nxtomoeditor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/patchrawdarkflat.py` & `tomwer-1.3.7/tomwer/app/patchrawdarkflat.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/radiostack.py` & `tomwer-1.3.7/tomwer/app/radiostack.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/reducedarkflat.py` & `tomwer-1.3.7/tomwer/app/reducedarkflat.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/rsync.py` & `tomwer-1.3.7/tomwer/app/rsync.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/samplemoved.py` & `tomwer-1.3.7/tomwer/app/samplemoved.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/scanviewer.py` & `tomwer-1.3.7/tomwer/app/scanviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/sinogramviewer.py` & `tomwer-1.3.7/tomwer/app/sinogramviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/slicestack.py` & `tomwer-1.3.7/tomwer/app/slicestack.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/stopdatalistener.py` & `tomwer-1.3.7/tomwer/app/stopdatalistener.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/app/zstitching.py` & `tomwer-1.3.7/tomwer/app/zstitching.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/__init__.py` & `tomwer-1.3.7/tomwer/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/cluster/cluster.py` & `tomwer-1.3.7/tomwer/core/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/futureobject.py` & `tomwer-1.3.7/tomwer/core/futureobject.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/log/logger.py` & `tomwer-1.3.7/tomwer/core/log/logger.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/log/processlog.py` & `tomwer-1.3.7/tomwer/core/log/processlog.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/cluster/supervisor.py` & `tomwer-1.3.7/tomwer/core/process/cluster/supervisor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/conditions/filters.py` & `tomwer-1.3.7/tomwer/core/process/conditions/filters.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datalistener/datalistener.py` & `tomwer-1.3.7/tomwer/core/process/control/datalistener/datalistener.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datalistener/rpcserver.py` & `tomwer-1.3.7/tomwer/core/process/control/datalistener/rpcserver.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datawatcher/datawatcher.py` & `tomwer-1.3.7/tomwer/core/process/control/datawatcher/datawatcher.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datawatcher/datawatcherobserver.py` & `tomwer-1.3.7/tomwer/core/process/control/datawatcher/datawatcherobserver.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datawatcher/datawatcherprocess.py` & `tomwer-1.3.7/tomwer/core/process/control/datawatcher/datawatcherprocess.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datawatcher/edfdwprocess.py` & `tomwer-1.3.7/tomwer/core/process/control/datawatcher/edfdwprocess.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datawatcher/hdf5dwprocess.py` & `tomwer-1.3.7/tomwer/core/process/control/datawatcher/hdf5dwprocess.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/datawatcher/status.py` & `tomwer-1.3.7/tomwer/core/process/control/datawatcher/status.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/emailnotifier.py` & `tomwer-1.3.7/tomwer/core/process/control/emailnotifier.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/nxtomoconcatenate.py` & `tomwer-1.3.7/tomwer/core/process/control/nxtomoconcatenate.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/nxtomomill.py` & `tomwer-1.3.7/tomwer/core/process/control/nxtomomill.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/scanlist.py` & `tomwer-1.3.7/tomwer/core/process/control/scanlist.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/scantransfer.py` & `tomwer-1.3.7/tomwer/core/process/control/scantransfer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/scanvalidator.py` & `tomwer-1.3.7/tomwer/core/process/control/scanvalidator.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/singletomoobj.py` & `tomwer-1.3.7/tomwer/core/process/control/singletomoobj.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/test/test_concatenate_nxtomos.py` & `tomwer-1.3.7/tomwer/core/process/control/test/test_concatenate_nxtomos.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/test/test_email.py` & `tomwer-1.3.7/tomwer/core/process/control/test/test_email.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/test/test_h52nx_process.py` & `tomwer-1.3.7/tomwer/core/process/control/test/test_h52nx_process.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/test/test_volume_link.py` & `tomwer-1.3.7/tomwer/core/process/control/test/test_volume_link.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/timer.py` & `tomwer-1.3.7/tomwer/core/process/control/timer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/control/volumesymlink.py` & `tomwer-1.3.7/tomwer/core/process/control/volumesymlink.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/edit/darkflatpatch.py` & `tomwer-1.3.7/tomwer/core/process/edit/darkflatpatch.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/edit/imagekeyeditor.py` & `tomwer-1.3.7/tomwer/core/process/edit/imagekeyeditor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/icat/createscreenshots.py` & `tomwer-1.3.7/tomwer/core/process/icat/createscreenshots.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/icat/gallery.py` & `tomwer-1.3.7/tomwer/core/process/icat/gallery.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/icat/icatbase.py` & `tomwer-1.3.7/tomwer/core/process/icat/icatbase.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/icat/publish.py` & `tomwer-1.3.7/tomwer/core/process/icat/publish.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/icat/screenshots.py` & `tomwer-1.3.7/tomwer/core/process/icat/screenshots.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/output.py` & `tomwer-1.3.7/tomwer/core/process/output.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/__init__.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/axis/anglemode.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/axis/anglemode.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/axis/axis.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/axis/axis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/axis/mode.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/axis/mode.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/axis/params.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/axis/params.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/axis/projectiontype.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/axis/projectiontype.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/darkrefs.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/darkrefs.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/darkrefscopy.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/darkrefscopy.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/darkref/params.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/darkref/params.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/castvolume.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/castvolume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/helical.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/helical.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabucommon.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabucommon.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabuscores.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabuscores.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabuslices.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabuslices.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/nabuvolume.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/nabuvolume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/settings.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/settings.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/target.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/target.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/nabu/utils.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/nabu/utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/normalization/normalization.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/normalization/normalization.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/normalization/params.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/normalization/params.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/output.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/output.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/paramsbase.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/paramsbase.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/saaxis/params.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/saaxis/params.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/saaxis/saaxis.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/saaxis/saaxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/sadeltabeta/params.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/sadeltabeta/params.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/sadeltabeta/sadeltabeta.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/sadeltabeta/sadeltabeta.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/scores/params.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/scores/params.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/scores/scores.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/scores/scores.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_axis_params.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_axis_params.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_darkref.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_darkref.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_darkref_copy.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_darkref_copy.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_paramsbase.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_paramsbase.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_saaxis.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_saaxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_sadeltabeta.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_sadeltabeta.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/reconstruction/test/test_utils.py` & `tomwer-1.3.7/tomwer/core/process/reconstruction/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/script/python.py` & `tomwer-1.3.7/tomwer/core/process/script/python.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/stitching/metadataholder.py` & `tomwer-1.3.7/tomwer/core/process/stitching/metadataholder.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/stitching/nabustitcher.py` & `tomwer-1.3.7/tomwer/core/process/stitching/nabustitcher.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/task.py` & `tomwer-1.3.7/tomwer/core/process/task.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_axis.py` & `tomwer-1.3.7/tomwer/core/process/test/test_axis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_conditions.py` & `tomwer-1.3.7/tomwer/core/process/test/test_conditions.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_dark_and_flat.py` & `tomwer-1.3.7/tomwer/core/process/test/test_dark_and_flat.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_data_listener.py` & `tomwer-1.3.7/tomwer/core/process/test/test_data_listener.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_data_transfer.py` & `tomwer-1.3.7/tomwer/core/process/test/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_data_watcher.py` & `tomwer-1.3.7/tomwer/core/process/test/test_data_watcher.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_nabu.py` & `tomwer-1.3.7/tomwer/core/process/test/test_nabu.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_normalization.py` & `tomwer-1.3.7/tomwer/core/process/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/test/test_timer.py` & `tomwer-1.3.7/tomwer/core/process/test/test_timer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/utils.py` & `tomwer-1.3.7/tomwer/core/process/utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/dataviewer.py` & `tomwer-1.3.7/tomwer/core/process/visualization/dataviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/diffviewer.py` & `tomwer-1.3.7/tomwer/core/process/visualization/diffviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/imagestackviewer.py` & `tomwer-1.3.7/tomwer/core/process/visualization/imagestackviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/radiostack.py` & `tomwer-1.3.7/tomwer/core/process/visualization/radiostack.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/samplemoved.py` & `tomwer-1.3.7/tomwer/core/process/visualization/samplemoved.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/sinogramviewer.py` & `tomwer-1.3.7/tomwer/core/process/visualization/sinogramviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/slicestack.py` & `tomwer-1.3.7/tomwer/core/process/visualization/slicestack.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/process/visualization/volumeviewer.py` & `tomwer-1.3.7/tomwer/core/process/visualization/volumeviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/progress.py` & `tomwer-1.3.7/tomwer/core/progress.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/__init__.py` & `tomwer-1.3.7/tomwer/core/scan/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/blissscan.py` & `tomwer-1.3.7/tomwer/core/scan/blissscan.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/edfscan.py` & `tomwer-1.3.7/tomwer/core/scan/edfscan.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/hdf5scan.py` & `tomwer-1.3.7/tomwer/core/scan/hdf5scan.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/nxtomoscan.py` & `tomwer-1.3.7/tomwer/core/scan/nxtomoscan.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/scanbase.py` & `tomwer-1.3.7/tomwer/core/scan/scanbase.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/scanfactory.py` & `tomwer-1.3.7/tomwer/core/scan/scanfactory.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/test/test_edf.py` & `tomwer-1.3.7/tomwer/core/scan/test/test_edf.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/test/test_future_scan.py` & `tomwer-1.3.7/tomwer/core/scan/test/test_future_scan.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/test/test_h5.py` & `tomwer-1.3.7/tomwer/core/scan/test/test_h5.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/test/test_process_registration.py` & `tomwer-1.3.7/tomwer/core/scan/test/test_process_registration.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/scan/test/test_scan.py` & `tomwer-1.3.7/tomwer/core/scan/test/test_scan.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/settings.py` & `tomwer-1.3.7/tomwer/core/settings.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/signal.py` & `tomwer-1.3.7/tomwer/core/signal.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/test/test_scanutils.py` & `tomwer-1.3.7/tomwer/core/test/test_scanutils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/test/test_utils.py` & `tomwer-1.3.7/tomwer/core/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/tomwer_object.py` & `tomwer-1.3.7/tomwer/core/tomwer_object.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/Singleton.py` & `tomwer-1.3.7/tomwer/core/utils/Singleton.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/char.py` & `tomwer-1.3.7/tomwer/core/utils/char.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/deprecation.py` & `tomwer-1.3.7/tomwer/core/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/dictutils.py` & `tomwer-1.3.7/tomwer/core/utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/ftseriesutils.py` & `tomwer-1.3.7/tomwer/core/utils/ftseriesutils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/gpu.py` & `tomwer-1.3.7/tomwer/core/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/image.py` & `tomwer-1.3.7/tomwer/core/utils/image.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/lbsram.py` & `tomwer-1.3.7/tomwer/core/utils/lbsram.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/locker.py` & `tomwer-1.3.7/tomwer/core/utils/locker.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/logconfig.py` & `tomwer-1.3.7/tomwer/core/utils/logconfig.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/normalization.py` & `tomwer-1.3.7/tomwer/core/utils/normalization.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/nxtomoutils.py` & `tomwer-1.3.7/tomwer/core/utils/nxtomoutils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/resource.py` & `tomwer-1.3.7/tomwer/core/utils/resource.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/scanutils.py` & `tomwer-1.3.7/tomwer/core/utils/scanutils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/slurm.py` & `tomwer-1.3.7/tomwer/core/utils/slurm.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/spec.py` & `tomwer-1.3.7/tomwer/core/utils/spec.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/threads.py` & `tomwer-1.3.7/tomwer/core/utils/threads.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/utils/time.py` & `tomwer-1.3.7/tomwer/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/volume/edfvolume.py` & `tomwer-1.3.7/tomwer/core/volume/edfvolume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/volume/hdf5volume.py` & `tomwer-1.3.7/tomwer/core/volume/hdf5volume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/volume/jp2kvolume.py` & `tomwer-1.3.7/tomwer/core/volume/jp2kvolume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/volume/rawvolume.py` & `tomwer-1.3.7/tomwer/core/volume/rawvolume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/volume/tiffvolume.py` & `tomwer-1.3.7/tomwer/core/volume/tiffvolume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/volume/volumebase.py` & `tomwer-1.3.7/tomwer/core/volume/volumebase.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/core/volume/volumefactory.py` & `tomwer-1.3.7/tomwer/core/volume/volumefactory.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/__init__.py` & `tomwer-1.3.7/tomwer/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/cluster/slurm.py` & `tomwer-1.3.7/tomwer/gui/cluster/slurm.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/cluster/supervisor.py` & `tomwer-1.3.7/tomwer/gui/cluster/supervisor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/cluster/test/test_cluster.py` & `tomwer-1.3.7/tomwer/gui/cluster/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/cluster/test/test_supervisor.py` & `tomwer-1.3.7/tomwer/gui/cluster/test/test_supervisor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/conditions/filter.py` & `tomwer-1.3.7/tomwer/gui/conditions/filter.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/configuration/action.py` & `tomwer-1.3.7/tomwer/gui/configuration/action.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/configuration/level.py` & `tomwer-1.3.7/tomwer/gui/configuration/level.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/actions.py` & `tomwer-1.3.7/tomwer/gui/control/actions.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datadiscovery.py` & `tomwer-1.3.7/tomwer/gui/control/datadiscovery.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datalist.py` & `tomwer-1.3.7/tomwer/gui/control/datalist.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datalistener.py` & `tomwer-1.3.7/tomwer/gui/control/datalistener.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datareacheractions.py` & `tomwer-1.3.7/tomwer/gui/control/datareacheractions.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datatransfert.py` & `tomwer-1.3.7/tomwer/gui/control/datatransfert.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datavalidator.py` & `tomwer-1.3.7/tomwer/gui/control/datavalidator.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datawatcher/__init__.py` & `tomwer-1.3.7/tomwer/gui/control/datawatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datawatcher/configuration.py` & `tomwer-1.3.7/tomwer/gui/control/datawatcher/configuration.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datawatcher/controlwidget.py` & `tomwer-1.3.7/tomwer/gui/control/datawatcher/controlwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datawatcher/datawatcher.py` & `tomwer-1.3.7/tomwer/gui/control/datawatcher/datawatcher.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/datawatcher/datawatcherobserver.py` & `tomwer-1.3.7/tomwer/gui/control/datawatcher/datawatcherobserver.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/emailnotifier.py` & `tomwer-1.3.7/tomwer/gui/control/emailnotifier.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/history.py` & `tomwer-1.3.7/tomwer/gui/control/history.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/nxtomomill.py` & `tomwer-1.3.7/tomwer/gui/control/nxtomomill.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/observations.py` & `tomwer-1.3.7/tomwer/gui/control/observations.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/reducedarkflatselector.py` & `tomwer-1.3.7/tomwer/gui/control/reducedarkflatselector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/scanselectorwidget.py` & `tomwer-1.3.7/tomwer/gui/control/scanselectorwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/selectorwidgetbase.py` & `tomwer-1.3.7/tomwer/gui/control/selectorwidgetbase.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/serie/nxtomoconcatenate.py` & `tomwer-1.3.7/tomwer/gui/control/serie/nxtomoconcatenate.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/serie/seriecreator.py` & `tomwer-1.3.7/tomwer/gui/control/serie/seriecreator.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/serie/seriewaiter.py` & `tomwer-1.3.7/tomwer/gui/control/serie/seriewaiter.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/singletomoobj.py` & `tomwer-1.3.7/tomwer/gui/control/singletomoobj.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/__init__.py` & `tomwer-1.3.7/tomwer/gui/control/test/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_datadiscovery.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_datadiscovery.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_datalist.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_datalist.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_datalistener.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_datalistener.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_datavalidator.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_datavalidator.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_email.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_email.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_inputwidget.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_inputwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_process_manager.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_process_manager.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_reducedarkflat_selector.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_reducedarkflat_selector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_scanselector.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_scanselector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_scanvalidator.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_scanvalidator.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_single_tomo_obj.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_single_tomo_obj.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_volume_dialog.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_volume_dialog.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/test/test_volumeselector.py` & `tomwer-1.3.7/tomwer/gui/control/test/test_volumeselector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/control/volumeselectorwidget.py` & `tomwer-1.3.7/tomwer/gui/control/volumeselectorwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/debugtools/datasetgenerator.py` & `tomwer-1.3.7/tomwer/gui/debugtools/datasetgenerator.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/debugtools/objectinspector.py` & `tomwer-1.3.7/tomwer/gui/debugtools/objectinspector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/dkrfpatch.py` & `tomwer-1.3.7/tomwer/gui/edit/dkrfpatch.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/imagekeyeditor.py` & `tomwer-1.3.7/tomwer/gui/edit/imagekeyeditor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/nxtomoeditor.py` & `tomwer-1.3.7/tomwer/gui/edit/nxtomoeditor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/nxtomowarmer.py` & `tomwer-1.3.7/tomwer/gui/edit/nxtomowarmer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/test/__init__.py` & `tomwer-1.3.7/tomwer/gui/edit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/test/test_dkrf_patch.py` & `tomwer-1.3.7/tomwer/gui/edit/test/test_dkrf_patch.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/test/test_image_key_editor.py` & `tomwer-1.3.7/tomwer/gui/edit/test/test_image_key_editor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/edit/test/test_nx_editor.py` & `tomwer-1.3.7/tomwer/gui/edit/test/test_nx_editor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/icat/createscreenshots.py` & `tomwer-1.3.7/tomwer/gui/icat/createscreenshots.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/icat/gallery.py` & `tomwer-1.3.7/tomwer/gui/icat/gallery.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/icat/publish.py` & `tomwer-1.3.7/tomwer/gui/icat/publish.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/icons.py` & `tomwer-1.3.7/tomwer/gui/icons.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/illustrations.py` & `tomwer-1.3.7/tomwer/gui/illustrations.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/imagefromfile.py` & `tomwer-1.3.7/tomwer/gui/imagefromfile.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/qconfigfile.py` & `tomwer-1.3.7/tomwer/gui/qconfigfile.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/qfolderdialog.py` & `tomwer-1.3.7/tomwer/gui/qfolderdialog.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/qlefilesystem.py` & `tomwer-1.3.7/tomwer/gui/qlefilesystem.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/axis/CompareImages.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/axis/CompareImages.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/axis/axis.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/axis/axis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/axis/radioaxis.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/axis/radioaxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/darkref/__init__.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/darkref/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/darkref/darkrefcopywidget.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/darkref/darkrefcopywidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/darkref/darkrefwidget.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/darkref/darkrefwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/castvolume.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/castvolume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/check.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/check.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/helical.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/helical.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/base.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/base.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/ctf.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/ctf.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/nabuconfig.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/nabuconfig.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/output.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/output.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/phase.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/phase.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/preprocessing.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuconfig/reconstruction.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuconfig/reconstruction.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/nabuflow.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/nabuflow.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/slices.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/slices.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/slurm.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/slurm.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/nabu/volume.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/nabu/volume.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/normalization/intensity.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/normalization/intensity.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/corrangeselector.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/corrangeselector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/dimensionwidget.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/dimensionwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/saaxis.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/saaxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/saaxis/sliceselector.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/saaxis/sliceselector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/sadeltabeta/saadeltabeta.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/sadeltabeta/saadeltabeta.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/scores/control.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/scores/control.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/scores/scoreplot.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/scores/scoreplot.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/test/test_axis.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/test/test_axis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/test/test_nabu.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/test/test_nabu.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/test/test_saaxis.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/test/test_saaxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/reconstruction/test/test_sadeltabeta.py` & `tomwer-1.3.7/tomwer/gui/reconstruction/test/test_sadeltabeta.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/samplemoved/__init__.py` & `tomwer-1.3.7/tomwer/gui/samplemoved/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/samplemoved/selectiontable.py` & `tomwer-1.3.7/tomwer/gui/samplemoved/selectiontable.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stackplot.py` & `tomwer-1.3.7/tomwer/gui/stackplot.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stacks.py` & `tomwer-1.3.7/tomwer/gui/stacks.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/action.py` & `tomwer-1.3.7/tomwer/gui/stitching/action.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/axisorderedlist.py` & `tomwer-1.3.7/tomwer/gui/stitching/axisorderedlist.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/config/axisparams.py` & `tomwer-1.3.7/tomwer/gui/stitching/config/axisparams.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/config/output.py` & `tomwer-1.3.7/tomwer/gui/stitching/config/output.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/config/positionoveraxis.py` & `tomwer-1.3.7/tomwer/gui/stitching/config/positionoveraxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/config/stitchingstrategies.py` & `tomwer-1.3.7/tomwer/gui/stitching/config/stitchingstrategies.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/config/tomoobjdetails.py` & `tomwer-1.3.7/tomwer/gui/stitching/config/tomoobjdetails.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/metadataholder.py` & `tomwer-1.3.7/tomwer/gui/stitching/metadataholder.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/normalization.py` & `tomwer-1.3.7/tomwer/gui/stitching/normalization.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/stitchandbackground.py` & `tomwer-1.3.7/tomwer/gui/stitching/stitchandbackground.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/stitching.py` & `tomwer-1.3.7/tomwer/gui/stitching/stitching.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/stitching_preview.py` & `tomwer-1.3.7/tomwer/gui/stitching/stitching_preview.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/stitching_raw.py` & `tomwer-1.3.7/tomwer/gui/stitching/stitching_raw.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/stitching/z_stitching/fineestimation.py` & `tomwer-1.3.7/tomwer/gui/stitching/z_stitching/fineestimation.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/test/__init__.py` & `tomwer-1.3.7/tomwer/gui/test/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/test/test_axis_gui.py` & `tomwer-1.3.7/tomwer/gui/test/test_axis_gui.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/buttons.py` & `tomwer-1.3.7/tomwer/gui/utils/buttons.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/completer.py` & `tomwer-1.3.7/tomwer/gui/utils/completer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/flow.py` & `tomwer-1.3.7/tomwer/gui/utils/flow.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/illustrations.py` & `tomwer-1.3.7/tomwer/gui/utils/illustrations.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/inputwidget.py` & `tomwer-1.3.7/tomwer/gui/utils/inputwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/lineselector/lineselector.py` & `tomwer-1.3.7/tomwer/gui/utils/lineselector/lineselector.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/sandboxes.py` & `tomwer-1.3.7/tomwer/gui/utils/sandboxes.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/scandescription.py` & `tomwer-1.3.7/tomwer/gui/utils/scandescription.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/scrollarea.py` & `tomwer-1.3.7/tomwer/gui/utils/scrollarea.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/slider.py` & `tomwer-1.3.7/tomwer/gui/utils/slider.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/splashscreen.py` & `tomwer-1.3.7/tomwer/gui/utils/splashscreen.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/step.py` & `tomwer-1.3.7/tomwer/gui/utils/step.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/unitsystem.py` & `tomwer-1.3.7/tomwer/gui/utils/unitsystem.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/utils.py` & `tomwer-1.3.7/tomwer/gui/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/vignettes.py` & `tomwer-1.3.7/tomwer/gui/utils/vignettes.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/utils/waiterthread.py` & `tomwer-1.3.7/tomwer/gui/utils/waiterthread.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/dataviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/dataviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/diffviewer/diffviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/diffviewer/diffviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/diffviewer/shiftwidget.py` & `tomwer-1.3.7/tomwer/gui/visualization/diffviewer/shiftwidget.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/fullscreenplot.py` & `tomwer-1.3.7/tomwer/gui/visualization/fullscreenplot.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/nxtomometadata.py` & `tomwer-1.3.7/tomwer/gui/visualization/nxtomometadata.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/reconstructionparameters.py` & `tomwer-1.3.7/tomwer/gui/visualization/reconstructionparameters.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/scanoverview.py` & `tomwer-1.3.7/tomwer/gui/visualization/scanoverview.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/sinogramviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/sinogramviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/__init__.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/test_dataviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/test_dataviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/test_diffviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/test_diffviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/test_nx_tomo_metadata_viewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/test_nx_tomo_metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/test_reconstruction_parameters.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/test_reconstruction_parameters.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/test_sinogramviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/test_sinogramviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/test_stacks.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/test_stacks.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/test/test_volumeviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/test/test_volumeviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/tomoobjoverview.py` & `tomwer-1.3.7/tomwer/gui/visualization/tomoobjoverview.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/volumeoverview.py` & `tomwer-1.3.7/tomwer/gui/visualization/volumeoverview.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/gui/visualization/volumeviewer.py` & `tomwer-1.3.7/tomwer/gui/visualization/volumeviewer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/io/utils/h5pyutils.py` & `tomwer-1.3.7/tomwer/io/utils/h5pyutils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/io/utils/raw_and_processed_data.py` & `tomwer-1.3.7/tomwer/io/utils/raw_and_processed_data.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/io/utils/tomoobj.py` & `tomwer-1.3.7/tomwer/io/utils/tomoobj.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/io/utils/utils.py` & `tomwer-1.3.7/tomwer/io/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/__init__.py` & `tomwer-1.3.7/tomwer/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/Imagej_icon.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/Imagej_icon.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/a.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/a.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/a.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/a.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/add.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/add.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/advanced_user.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/advanced_user.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/advanced_user.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/advanced_user.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/axis.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/axis.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/axis.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/axis.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/background.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/background.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/background.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/background.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/basic_user.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/basic_user.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/basic_user.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/basic_user.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_active.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_active.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_active.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_active.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_inactive.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_inactive.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/cfg_file_inactive.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/cfg_file_inactive.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/compare_mode_a_minus_b.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/compare_mode_a_minus_b.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/compare_mode_a_minus_b.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/compare_mode_a_minus_b.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/compose.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/compose.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/compose.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/compose.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_activate.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_activate.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_activate.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_activate.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_deactivate.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_deactivate.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/datalistener_deactivate.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/datalistener_deactivate.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/delta_beta.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/delta_beta.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/delta_beta.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/delta_beta.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/exit.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/exit.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/exit.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/exit.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/full_screen.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/full_screen.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/full_screen.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/full_screen.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/hammer.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/hammer.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/health.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/health.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/health.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/health.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/high_speed.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/high_speed.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/high_speed.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/high_speed.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/history.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/history.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/hourglass.npy` & `tomwer-1.3.7/tomwer/resources/gui/icons/hourglass.npy`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/imageNotFound.npy` & `tomwer-1.3.7/tomwer/resources/gui/icons/imageNotFound.npy`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/information.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/information.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/information.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/information.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/input.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/input.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/input.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/input.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/invisible.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/invisible.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/invisible.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/invisible.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/lineselection.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/lineselection.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/lineselection.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/lineselection.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/list_selection.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/list_selection.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/list_selection.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/list_selection.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/locked.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/locked.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/log.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/log.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/log.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/log.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/loop.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/loop.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/low_speed.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/low_speed.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/low_speed.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/low_speed.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/medium_low_speed.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/medium_low_speed.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/medium_low_speed.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/medium_low_speed.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/minimalistic_user.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/minimalistic_user.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/minimalistic_user.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/minimalistic_user.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/multi-document-save.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/multi-document-save.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/multi-document-save.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/multi-document-save.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/nabu.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/nabu.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/output.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/output.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/output.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/output.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/parameters.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/parameters.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/parameters.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/parameters.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/plot-xleft.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/plot-xleft.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/plot-xleft.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/plot-xleft.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/plot-xright.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/plot-xright.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/plot-xright.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/plot-xright.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/range_selection.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/range_selection.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/range_selection.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/range_selection.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/results.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/results.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/results.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/results.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/rm.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/rm.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/roman_four.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/roman_four.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/roman_four.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/roman_four.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/roman_one.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/roman_one.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/roman_three.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/roman_three.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/roman_two.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/roman_two.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/ruler.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/ruler.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/ruler.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/ruler.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/short_description.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/short_description.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/single_selection.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/single_selection.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/single_selection.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/single_selection.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/sinogram.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/sinogram.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/slurm.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/slurm.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/slurm_active.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/slurm_active.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/slurm_active.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/slurm_active.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/slurm_deactive.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/slurm_deactive.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/slurm_deactive.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/slurm_deactive.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRaw.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRaw.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRaw.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRaw.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRefine.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRefine.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/stitching_modeRefine.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/stitching_modeRefine.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/tomwer.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/tomwer.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/tomwer_large.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/tomwer_large.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/unlocked.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/unlocked.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/unsharp_mask.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/unsharp_mask.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/update_stitching_preview.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/update_stitching_preview.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/url.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/url.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/vignettes.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/vignettes.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/vignettes.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/vignettes.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/visible.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/visible.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/warning.png` & `tomwer-1.3.7/tomwer/resources/gui/icons/warning.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/icons/warning.svg` & `tomwer-1.3.7/tomwer/resources/gui/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/illustrations/ctf_z1.png` & `tomwer-1.3.7/tomwer/resources/gui/illustrations/ctf_z1.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/illustrations/ctf_z1.svg` & `tomwer-1.3.7/tomwer/resources/gui/illustrations/ctf_z1.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_down.png` & `tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_down.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_down.svg` & `tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_down.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_right.png` & `tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_right.png`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/illustrations/flow_right.svg` & `tomwer-1.3.7/tomwer/resources/gui/illustrations/flow_right.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/resources/gui/illustrations/no_rot.svg` & `tomwer-1.3.7/tomwer/resources/gui/illustrations/no_rot.svg`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/axis.py` & `tomwer-1.3.7/tomwer/synctools/axis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/darkref.py` & `tomwer-1.3.7/tomwer/synctools/darkref.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/datalistener.py` & `tomwer-1.3.7/tomwer/synctools/datalistener.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/datatransfert.py` & `tomwer-1.3.7/tomwer/synctools/datatransfert.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/imageloaderthread.py` & `tomwer-1.3.7/tomwer/synctools/imageloaderthread.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/rsyncmanager.py` & `tomwer-1.3.7/tomwer/synctools/rsyncmanager.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/saaxis.py` & `tomwer-1.3.7/tomwer/synctools/saaxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/sadeltabeta.py` & `tomwer-1.3.7/tomwer/synctools/sadeltabeta.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/control/datalistener.py` & `tomwer-1.3.7/tomwer/synctools/stacks/control/datalistener.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/edit/darkflatpatch.py` & `tomwer-1.3.7/tomwer/synctools/stacks/edit/darkflatpatch.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/edit/imagekeyeditor.py` & `tomwer-1.3.7/tomwer/synctools/stacks/edit/imagekeyeditor.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/processingstack.py` & `tomwer-1.3.7/tomwer/synctools/stacks/processingstack.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/axis.py` & `tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/axis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/castvolume.py` & `tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/castvolume.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,19 +90,34 @@
             )
             _logger.processSkipped(mess)
             if callback is not None:
                 callback()
             self.scan_ready(scan=data)
         else:
             self._data_currently_computed = data
-            self._computationThread.init(data=data, configuration=configuration)
-            # need to manage connect before starting it because
-            fct_callback = functools.partial(self._end_threaded_computation, callback)
-            self._computationThread.finished.connect(fct_callback)
-            self._computationThread.start()
+            try:
+                self._computationThread.init(data=data, configuration=configuration)
+            except ValueError as e:
+                # initialization can fail (for example for cast volume is there is no volume or be case this will raise an error)
+                # then we want to keep the thread active
+                self._data_currently_computed = None
+                ProcessManager().notify_dataset_state(
+                    dataset=data, process=self._process_id, state=DatasetState.SKIPPED
+                )
+                _logger.processSkipped(f"thread initialization failed. Error is {e}")
+                if callback is not None:
+                    callback()
+                self.scan_ready(scan=data)
+            else:
+                # need to manage connect before starting it because
+                fct_callback = functools.partial(
+                    self._end_threaded_computation, callback
+                )
+                self._computationThread.finished.connect(fct_callback)
+                self._computationThread.start()
 
     def _end_computation(self, data, future_tomo_obj, callback):
         """
         callback when the computation thread is finished
 
         :param scan: pass if no call to '_computationThread is made'
         """
```

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/dkrefcopy.py` & `tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/dkrefcopy.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/nabu.py` & `tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/nabu.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/normalization.py` & `tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/normalization.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/saaxis.py` & `tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/saaxis.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/stacks/reconstruction/sadeltabeta.py` & `tomwer-1.3.7/tomwer/synctools/stacks/reconstruction/sadeltabeta.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/test/test_darkRefs.py` & `tomwer-1.3.7/tomwer/synctools/test/test_darkRefs.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/test/test_foldertransfer.py` & `tomwer-1.3.7/tomwer/synctools/test/test_foldertransfer.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/synctools/utils/scanstages.py` & `tomwer-1.3.7/tomwer/synctools/utils/scanstages.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/tests/conftest.py` & `tomwer-1.3.7/tomwer/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/tests/test_scripts.py` & `tomwer-1.3.7/tomwer/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/third_part/WaitingOverlay.py` & `tomwer-1.3.7/tomwer/third_part/WaitingOverlay.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/utils.py` & `tomwer-1.3.7/tomwer/utils.py`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer/version.py` & `tomwer-1.3.7/tomwer/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     "gamma": 11,
     "rc": 12,
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 3
-MICRO = 6
+MICRO = 7
 RELEV = "final"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 
 _version_info = namedtuple(
```

### Comparing `tomwer-1.3.6/tomwer.egg-info/PKG-INFO` & `tomwer-1.3.7/tomwer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomwer
-Version: 1.3.6
+Version: 1.3.7
 Summary: "tomography workflow tools"
 Home-page: https://gitlab.esrf.fr/tomotools/tomwer
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomwer/-/issues
 Keywords: orange3 add-on,ewoks
```

### Comparing `tomwer-1.3.6/tomwer.egg-info/SOURCES.txt` & `tomwer-1.3.7/tomwer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tomwer-1.3.6/tomwer.egg-info/requires.txt` & `tomwer-1.3.7/tomwer.egg-info/requires.txt`

 * *Files identical despite different names*

