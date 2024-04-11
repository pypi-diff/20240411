# Comparing `tmp/tmart-2.3.0.tar.gz` & `tmp/tmart-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmart-2.3.0.tar", last modified: Thu Mar 28 22:00:56 2024, max compression
+gzip compressed data, was "tmart-2.3.1.tar", last modified: Thu Apr 11 14:40:23 2024, max compression
```

## Comparing `tmart-2.3.0.tar` & `tmart-2.3.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.951095 tmart-2.3.0/
--rw-r--r--   0 yw         (501) staff       (20)       51 2023-10-19 15:57:58.000000 tmart-2.3.0/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     5204 2024-03-28 22:00:56.950852 tmart-2.3.0/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     4357 2024-03-17 13:59:52.000000 tmart-2.3.0/README.md
--rw-r--r--   0 yw         (501) staff       (20)       38 2024-03-28 22:00:56.951170 tmart-2.3.0/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)     2045 2024-03-28 21:57:36.000000 tmart-2.3.0/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.930284 tmart-2.3.0/tests/
--rwxrwxrwx   0 yw         (501) staff       (20)      413 2023-10-19 16:51:10.000000 tmart-2.3.0/tests/test_AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     2960 2023-05-23 22:19:27.000000 tmart-2.3.0/tests/test_AE_modelling.py
--rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-2.3.0/tests/test_E_diffuse.py
--rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-2.3.0/tests/test_L_sky.py
--rw-r--r--   0 yw         (501) staff       (20)     2569 2024-01-30 23:00:00.000000 tmart-2.3.0/tests/test_basic.py
--rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-2.3.0/tests/test_basic_import.py
--rw-r--r--   0 yw         (501) staff       (20)      824 2023-05-26 03:52:15.000000 tmart-2.3.0/tests/test_calc_rho.py
--rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-2.3.0/tests/test_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     1172 2023-05-26 22:25:30.000000 tmart-2.3.0/tests/test_fresnel.py
--rwxrwxrwx   0 yw         (501) staff       (20)     1489 2023-10-19 16:51:11.000000 tmart-2.3.0/tests/test_modelling.py
--rw-r--r--   0 yw         (501) staff       (20)     2036 2023-05-23 20:57:30.000000 tmart-2.3.0/tests/test_plot.py
--rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-2.3.0/tests/test_quickstart.py
--rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-2.3.0/tests/test_specular_contribution.py
--rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-2.3.0/tests/test_typical_ocean.py
--rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-2.3.0/tests/test_whales_SR.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.933108 tmart-2.3.0/tmart/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.937836 tmart-2.3.0/tmart/AEC/
--rw-r--r--   0 yw         (501) staff       (20)     9444 2024-03-28 18:17:03.000000 tmart-2.3.0/tmart/AEC/AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     1016 2024-03-28 20:07:38.000000 tmart-2.3.0/tmart/AEC/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     1758 2023-10-20 19:50:31.000000 tmart-2.3.0/tmart/AEC/anci_download.py
--rw-r--r--   0 yw         (501) staff       (20)     3546 2024-03-10 16:18:02.000000 tmart-2.3.0/tmart/AEC/anci_get_AER.py
--rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 tmart-2.3.0/tmart/AEC/anci_get_OWV.py
--rw-r--r--   0 yw         (501) staff       (20)     1788 2024-03-10 16:16:09.000000 tmart-2.3.0/tmart/AEC/anci_list_files.py
--rw-r--r--   0 yw         (501) staff       (20)     1628 2024-03-10 16:14:25.000000 tmart-2.3.0/tmart/AEC/compute_gas_transmittance.py
--rw-r--r--   0 yw         (501) staff       (20)     9844 2024-03-28 18:15:37.000000 tmart-2.3.0/tmart/AEC/compute_masks.py
--rw-r--r--   0 yw         (501) staff       (20)      648 2023-10-18 00:57:41.000000 tmart-2.3.0/tmart/AEC/fillnan.py
--rw-r--r--   0 yw         (501) staff       (20)     9982 2024-03-10 16:15:20.000000 tmart-2.3.0/tmart/AEC/get_AOT.py
--rw-r--r--   0 yw         (501) staff       (20)     1579 2023-12-14 02:45:52.000000 tmart-2.3.0/tmart/AEC/get_ancillary.py
--rw-r--r--   0 yw         (501) staff       (20)     6588 2024-03-10 16:17:43.000000 tmart-2.3.0/tmart/AEC/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)      995 2024-03-10 16:16:22.000000 tmart-2.3.0/tmart/AEC/identify_sensor.py
--rw-r--r--   0 yw         (501) staff       (20)     4553 2024-03-10 16:14:57.000000 tmart-2.3.0/tmart/AEC/irradiance_correction.py
--rw-r--r--   0 yw         (501) staff       (20)     1184 2024-01-11 18:18:13.000000 tmart-2.3.0/tmart/AEC/read_PRISMA_north.py
--rw-r--r--   0 yw         (501) staff       (20)     2886 2023-10-18 01:13:05.000000 tmart-2.3.0/tmart/AEC/read_PRISMA_vaa.py
--rw-r--r--   0 yw         (501) staff       (20)     1060 2024-03-10 16:17:04.000000 tmart-2.3.0/tmart/AEC/read_config.py
--rw-r--r--   0 yw         (501) staff       (20)    11907 2024-03-28 21:59:35.000000 tmart-2.3.0/tmart/AEC/read_metadata_Landsat.py
--rw-r--r--   0 yw         (501) staff       (20)     6684 2024-03-10 16:17:00.000000 tmart-2.3.0/tmart/AEC/read_metadata_S2.py
--rw-r--r--   0 yw         (501) staff       (20)     2036 2023-10-18 01:15:47.000000 tmart-2.3.0/tmart/AEC/read_xml_S2.py
--rw-r--r--   0 yw         (501) staff       (20)     1331 2023-10-18 01:14:23.000000 tmart-2.3.0/tmart/AEC/read_xml_S2_scene.py
--rw-r--r--   0 yw         (501) staff       (20)     4798 2024-03-28 17:56:28.000000 tmart-2.3.0/tmart/AEC/run.py
--rw-r--r--   0 yw         (501) staff       (20)    12038 2024-01-14 03:26:49.000000 tmart-2.3.0/tmart/AEC/run_acoliteL1R.py
--rw-r--r--   0 yw         (501) staff       (20)     2743 2024-03-28 20:00:23.000000 tmart-2.3.0/tmart/AEC/run_regular.py
--rw-r--r--   0 yw         (501) staff       (20)     1144 2024-01-11 21:20:16.000000 tmart-2.3.0/tmart/AEC/write_atm_info.py
--rw-r--r--   0 yw         (501) staff       (20)     1811 2024-01-18 16:28:44.000000 tmart-2.3.0/tmart/Aerosol.py
--rw-r--r--   0 yw         (501) staff       (20)    11377 2024-03-10 16:08:40.000000 tmart-2.3.0/tmart/Atmosphere.py
--rw-r--r--   0 yw         (501) staff       (20)     9961 2024-01-18 16:27:41.000000 tmart-2.3.0/tmart/Surface.py
--rw-r--r--   0 yw         (501) staff       (20)    13680 2024-01-18 16:35:11.000000 tmart-2.3.0/tmart/Tmart.py
--rw-r--r--   0 yw         (501) staff       (20)    38169 2024-03-10 16:13:38.000000 tmart-2.3.0/tmart/Tmart2.py
--rw-r--r--   0 yw         (501) staff       (20)      550 2023-12-28 20:42:03.000000 tmart-2.3.0/tmart/__init__.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.939888 tmart-2.3.0/tmart/ancillary/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.946024 tmart-2.3.0/tmart/ancillary/aerosolSPF/
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-2.3.0/tmart/ancillary/aerosolSPF/BiomassBurning.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-2.3.0/tmart/ancillary/aerosolSPF/Continental.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-2.3.0/tmart/ancillary/aerosolSPF/Desert.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-2.3.0/tmart/ancillary/aerosolSPF/Maritime.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-2.3.0/tmart/ancillary/aerosolSPF/Stratospheric.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-2.3.0/tmart/ancillary/aerosolSPF/Urban.csv
--rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-2.3.0/tmart/ancillary/conifer_forest.csv
--rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-2.3.0/tmart/ancillary/dry_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-2.3.0/tmart/ancillary/lawn_grass.csv
--rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-2.3.0/tmart/ancillary/soil.csv
--rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-2.3.0/tmart/ancillary/vegetation.csv
--rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-2.3.0/tmart/ancillary/water.csv
--rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-2.3.0/tmart/ancillary/water_chl1.csv
--rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-2.3.0/tmart/ancillary/wet_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-2.3.0/tmart/ancillary/whitecap_factor.csv
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.946691 tmart-2.3.0/tmart/config/
--rw-r--r--   0 yw         (501) staff       (20)     1303 2024-03-28 18:02:22.000000 tmart-2.3.0/tmart/config/config.txt
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.948620 tmart-2.3.0/tmart/surface_rho/
--rw-r--r--   0 yw         (501) staff       (20)      341 2023-05-23 22:27:30.000000 tmart-2.3.0/tmart/surface_rho/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     5038 2023-05-26 07:42:38.000000 tmart-2.3.0/tmart/surface_rho/calculate.py
--rw-r--r--   0 yw         (501) staff       (20)     2003 2024-03-10 16:10:22.000000 tmart-2.3.0/tmart/tm_OT.py
--rw-r--r--   0 yw         (501) staff       (20)     3195 2024-01-18 16:28:32.000000 tmart-2.3.0/tmart/tm_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     3976 2024-03-10 16:09:31.000000 tmart-2.3.0/tmart/tm_geometry.py
--rw-r--r--   0 yw         (501) staff       (20)    12883 2024-03-10 16:09:57.000000 tmart-2.3.0/tmart/tm_intersect.py
--rw-r--r--   0 yw         (501) staff       (20)    11243 2024-03-10 16:10:06.000000 tmart-2.3.0/tmart/tm_move.py
--rw-r--r--   0 yw         (501) staff       (20)     6748 2024-01-18 16:33:59.000000 tmart-2.3.0/tmart/tm_sampling.py
--rw-r--r--   0 yw         (501) staff       (20)    12102 2024-03-10 16:10:58.000000 tmart-2.3.0/tmart/tm_water.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-28 22:00:56.934015 tmart-2.3.0/tmart.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     5204 2024-03-28 22:00:56.000000 tmart-2.3.0/tmart.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     2067 2024-03-28 22:00:56.000000 tmart-2.3.0/tmart.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2024-03-28 22:00:56.000000 tmart-2.3.0/tmart.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       70 2024-03-28 22:00:56.000000 tmart-2.3.0/tmart.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2024-03-28 22:00:56.000000 tmart-2.3.0/tmart.egg-info/top_level.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.802264 tmart-2.3.1/
+-rw-r--r--   0 yw         (501) staff       (20)       51 2023-10-19 15:57:58.000000 tmart-2.3.1/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     5204 2024-04-11 14:40:23.802050 tmart-2.3.1/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     4357 2024-03-17 13:59:52.000000 tmart-2.3.1/README.md
+-rw-r--r--   0 yw         (501) staff       (20)       38 2024-04-11 14:40:23.802315 tmart-2.3.1/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)     2045 2024-04-11 14:27:23.000000 tmart-2.3.1/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.779645 tmart-2.3.1/tests/
+-rwxrwxrwx   0 yw         (501) staff       (20)      413 2023-10-19 16:51:10.000000 tmart-2.3.1/tests/test_AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     2960 2023-05-23 22:19:27.000000 tmart-2.3.1/tests/test_AE_modelling.py
+-rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-2.3.1/tests/test_E_diffuse.py
+-rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-2.3.1/tests/test_L_sky.py
+-rw-r--r--   0 yw         (501) staff       (20)     2569 2024-01-30 23:00:00.000000 tmart-2.3.1/tests/test_basic.py
+-rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-2.3.1/tests/test_basic_import.py
+-rw-r--r--   0 yw         (501) staff       (20)      824 2023-05-26 03:52:15.000000 tmart-2.3.1/tests/test_calc_rho.py
+-rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-2.3.1/tests/test_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     1172 2023-05-26 22:25:30.000000 tmart-2.3.1/tests/test_fresnel.py
+-rwxrwxrwx   0 yw         (501) staff       (20)     1489 2023-10-19 16:51:11.000000 tmart-2.3.1/tests/test_modelling.py
+-rw-r--r--   0 yw         (501) staff       (20)     2047 2024-04-11 14:38:23.000000 tmart-2.3.1/tests/test_plot.py
+-rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-2.3.1/tests/test_quickstart.py
+-rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-2.3.1/tests/test_specular_contribution.py
+-rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-2.3.1/tests/test_typical_ocean.py
+-rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-2.3.1/tests/test_whales_SR.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.782755 tmart-2.3.1/tmart/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.790061 tmart-2.3.1/tmart/AEC/
+-rw-r--r--   0 yw         (501) staff       (20)     9444 2024-03-28 18:17:03.000000 tmart-2.3.1/tmart/AEC/AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     1016 2024-03-28 20:07:38.000000 tmart-2.3.1/tmart/AEC/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     1758 2023-10-20 19:50:31.000000 tmart-2.3.1/tmart/AEC/anci_download.py
+-rw-r--r--   0 yw         (501) staff       (20)     3546 2024-03-10 16:18:02.000000 tmart-2.3.1/tmart/AEC/anci_get_AER.py
+-rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 tmart-2.3.1/tmart/AEC/anci_get_OWV.py
+-rw-r--r--   0 yw         (501) staff       (20)     1788 2024-03-10 16:16:09.000000 tmart-2.3.1/tmart/AEC/anci_list_files.py
+-rw-r--r--   0 yw         (501) staff       (20)     1628 2024-03-10 16:14:25.000000 tmart-2.3.1/tmart/AEC/compute_gas_transmittance.py
+-rw-r--r--   0 yw         (501) staff       (20)     9844 2024-03-28 18:15:37.000000 tmart-2.3.1/tmart/AEC/compute_masks.py
+-rw-r--r--   0 yw         (501) staff       (20)      648 2023-10-18 00:57:41.000000 tmart-2.3.1/tmart/AEC/fillnan.py
+-rw-r--r--   0 yw         (501) staff       (20)     9982 2024-03-10 16:15:20.000000 tmart-2.3.1/tmart/AEC/get_AOT.py
+-rw-r--r--   0 yw         (501) staff       (20)     1579 2023-12-14 02:45:52.000000 tmart-2.3.1/tmart/AEC/get_ancillary.py
+-rw-r--r--   0 yw         (501) staff       (20)     6588 2024-03-10 16:17:43.000000 tmart-2.3.1/tmart/AEC/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)      995 2024-03-10 16:16:22.000000 tmart-2.3.1/tmart/AEC/identify_sensor.py
+-rw-r--r--   0 yw         (501) staff       (20)     4553 2024-03-10 16:14:57.000000 tmart-2.3.1/tmart/AEC/irradiance_correction.py
+-rw-r--r--   0 yw         (501) staff       (20)     1184 2024-01-11 18:18:13.000000 tmart-2.3.1/tmart/AEC/read_PRISMA_north.py
+-rw-r--r--   0 yw         (501) staff       (20)     2886 2023-10-18 01:13:05.000000 tmart-2.3.1/tmart/AEC/read_PRISMA_vaa.py
+-rw-r--r--   0 yw         (501) staff       (20)     1060 2024-03-10 16:17:04.000000 tmart-2.3.1/tmart/AEC/read_config.py
+-rw-r--r--   0 yw         (501) staff       (20)    11907 2024-03-28 21:59:35.000000 tmart-2.3.1/tmart/AEC/read_metadata_Landsat.py
+-rw-r--r--   0 yw         (501) staff       (20)     6684 2024-03-10 16:17:00.000000 tmart-2.3.1/tmart/AEC/read_metadata_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)     2036 2023-10-18 01:15:47.000000 tmart-2.3.1/tmart/AEC/read_xml_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)     1331 2023-10-18 01:14:23.000000 tmart-2.3.1/tmart/AEC/read_xml_S2_scene.py
+-rw-r--r--   0 yw         (501) staff       (20)     4798 2024-03-28 17:56:28.000000 tmart-2.3.1/tmart/AEC/run.py
+-rw-r--r--   0 yw         (501) staff       (20)    12038 2024-01-14 03:26:49.000000 tmart-2.3.1/tmart/AEC/run_acoliteL1R.py
+-rw-r--r--   0 yw         (501) staff       (20)     2743 2024-03-28 20:00:23.000000 tmart-2.3.1/tmart/AEC/run_regular.py
+-rw-r--r--   0 yw         (501) staff       (20)     1144 2024-01-11 21:20:16.000000 tmart-2.3.1/tmart/AEC/write_atm_info.py
+-rw-r--r--   0 yw         (501) staff       (20)     1811 2024-01-18 16:28:44.000000 tmart-2.3.1/tmart/Aerosol.py
+-rw-r--r--   0 yw         (501) staff       (20)    11377 2024-03-10 16:08:40.000000 tmart-2.3.1/tmart/Atmosphere.py
+-rw-r--r--   0 yw         (501) staff       (20)     9961 2024-01-18 16:27:41.000000 tmart-2.3.1/tmart/Surface.py
+-rw-r--r--   0 yw         (501) staff       (20)    13680 2024-01-18 16:35:11.000000 tmart-2.3.1/tmart/Tmart.py
+-rw-r--r--   0 yw         (501) staff       (20)    38594 2024-04-11 14:37:47.000000 tmart-2.3.1/tmart/Tmart2.py
+-rw-r--r--   0 yw         (501) staff       (20)      550 2023-12-28 20:42:03.000000 tmart-2.3.1/tmart/__init__.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.792044 tmart-2.3.1/tmart/ancillary/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.800608 tmart-2.3.1/tmart/ancillary/aerosolSPF/
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/BiomassBurning.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Continental.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Desert.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Maritime.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Stratospheric.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-2.3.1/tmart/ancillary/aerosolSPF/Urban.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-2.3.1/tmart/ancillary/conifer_forest.csv
+-rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-2.3.1/tmart/ancillary/dry_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-2.3.1/tmart/ancillary/lawn_grass.csv
+-rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-2.3.1/tmart/ancillary/soil.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-2.3.1/tmart/ancillary/vegetation.csv
+-rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-2.3.1/tmart/ancillary/water.csv
+-rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-2.3.1/tmart/ancillary/water_chl1.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-2.3.1/tmart/ancillary/wet_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-2.3.1/tmart/ancillary/whitecap_factor.csv
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.801120 tmart-2.3.1/tmart/config/
+-rw-r--r--   0 yw         (501) staff       (20)     1303 2024-03-28 18:02:22.000000 tmart-2.3.1/tmart/config/config.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.801630 tmart-2.3.1/tmart/surface_rho/
+-rw-r--r--   0 yw         (501) staff       (20)      341 2023-05-23 22:27:30.000000 tmart-2.3.1/tmart/surface_rho/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5038 2023-05-26 07:42:38.000000 tmart-2.3.1/tmart/surface_rho/calculate.py
+-rw-r--r--   0 yw         (501) staff       (20)     2003 2024-03-10 16:10:22.000000 tmart-2.3.1/tmart/tm_OT.py
+-rw-r--r--   0 yw         (501) staff       (20)     3195 2024-01-18 16:28:32.000000 tmart-2.3.1/tmart/tm_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     3976 2024-03-10 16:09:31.000000 tmart-2.3.1/tmart/tm_geometry.py
+-rw-r--r--   0 yw         (501) staff       (20)    12883 2024-03-10 16:09:57.000000 tmart-2.3.1/tmart/tm_intersect.py
+-rw-r--r--   0 yw         (501) staff       (20)    11243 2024-03-10 16:10:06.000000 tmart-2.3.1/tmart/tm_move.py
+-rw-r--r--   0 yw         (501) staff       (20)     6748 2024-01-18 16:33:59.000000 tmart-2.3.1/tmart/tm_sampling.py
+-rw-r--r--   0 yw         (501) staff       (20)    12104 2024-04-11 14:31:53.000000 tmart-2.3.1/tmart/tm_water.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-11 14:40:23.783362 tmart-2.3.1/tmart.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     5204 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     2067 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       70 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2024-04-11 14:40:23.000000 tmart-2.3.1/tmart.egg-info/top_level.txt
```

### Comparing `tmart-2.3.0/PKG-INFO` & `tmart-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 2.3.0
+Version: 2.3.1
 Summary: Modelling and correcting for the adjacency effect in aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tmart-2.3.0/README.md` & `tmart-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/setup.py` & `tmart-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmart",                     # This is the name of the package
-    version="2.3.0",                       
+    version="2.3.1",                       
     author="Yulun Wu",                     # Full name of the author
     description="Modelling and correcting for the adjacency effect in aquatic remote sensing",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),    # List of all python modules to be installed
     packages = ['tmart','tmart.surface_rho','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF','tmart.config'],
     include_package_data=True,
```

### Comparing `tmart-2.3.0/tests/test_AE_modelling.py` & `tmart-2.3.1/tests/test_AE_modelling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_E_diffuse.py` & `tmart-2.3.1/tests/test_E_diffuse.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_L_sky.py` & `tmart-2.3.1/tests/test_L_sky.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_basic.py` & `tmart-2.3.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_basic_import.py` & `tmart-2.3.1/tests/test_basic_import.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_calc_rho.py` & `tmart-2.3.1/tests/test_calc_rho.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_calcref.py` & `tmart-2.3.1/tests/test_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_fresnel.py` & `tmart-2.3.1/tests/test_fresnel.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_modelling.py` & `tmart-2.3.1/tests/test_modelling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_plot.py` & `tmart-2.3.1/tests/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 sys.path.append(two_up)
 
 import tmart
 import numpy as np
 from Py6S.Params.atmosprofile import AtmosProfile
 
 # Specify wavelength in nm
-wl = 400
+wl = 1300
 
 ### DEM and reflectance ###
 
 # Three same-size numpy arrays are needed
 image_DEM = np.full((2, 2), 0) # in meters
 image_reflectance = np.full((2, 2), 0.1) # unitless     
-image_isWater = np.full((2, 2), 0) # 1 is water, 0 is land
+image_isWater = np.full((2, 2), 1) # 1 is water, 0 is land
 
 # pixel width and length, in meters 
 cell_size = 20_000 
 
 # Synthesize a surface object
 my_surface = tmart.Surface(DEM = image_DEM,
                            reflectance = image_reflectance,
@@ -48,24 +48,33 @@
 
 # Synthesize an atmosphere object 
 my_atm = tmart.Atmosphere(atm_profile)
 
 ### Running T-Mart ###
 
 # Make a T-Mart object 
-my_tmart = tmart.Tmart(Surface = my_surface, Atmosphere= my_atm)
+my_tmart = tmart.Tmart(Surface = my_surface, Atmosphere = my_atm)
 
 # Specify the sensor's position (x, y, z), viewing direction relative 
 # to the sensor (zenith, azimuth), sun's direction relative to the target 
 # (zenith, azimuth)
 my_tmart.set_geometry(sensor_coords=[51,50,130_000], 
-                      target_pt_direction=[180,0],
+                      target_pt_direction=[170,0],
                       sun_dir=[0,0])
 
 # Run and plot on a separate window
 %matplotlib qt
 results = my_tmart.run_plot(wl=wl, plot_on=True, plot_range=[0,100_000,0,100_000,0,100_000])
 
 # Calculate reflectances using recorded photon information 
 R = tmart.calc_ref(results)
 for k, v in R.items():
     print(k, '     ' , v)
+
+
+
+
+
+
+
+
+
```

### Comparing `tmart-2.3.0/tests/test_quickstart.py` & `tmart-2.3.1/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_specular_contribution.py` & `tmart-2.3.1/tests/test_specular_contribution.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_typical_ocean.py` & `tmart-2.3.1/tests/test_typical_ocean.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tests/test_whales_SR.py` & `tmart-2.3.1/tests/test_whales_SR.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/AEC.py` & `tmart-2.3.1/tmart/AEC/AEC.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/__init__.py` & `tmart-2.3.1/tmart/AEC/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/anci_download.py` & `tmart-2.3.1/tmart/AEC/anci_download.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/anci_get_AER.py` & `tmart-2.3.1/tmart/AEC/anci_get_AER.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/anci_get_OWV.py` & `tmart-2.3.1/tmart/AEC/anci_get_OWV.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/anci_list_files.py` & `tmart-2.3.1/tmart/AEC/anci_list_files.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/compute_gas_transmittance.py` & `tmart-2.3.1/tmart/AEC/compute_gas_transmittance.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/compute_masks.py` & `tmart-2.3.1/tmart/AEC/compute_masks.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/fillnan.py` & `tmart-2.3.1/tmart/AEC/fillnan.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/get_AOT.py` & `tmart-2.3.1/tmart/AEC/get_AOT.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/get_ancillary.py` & `tmart-2.3.1/tmart/AEC/get_ancillary.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/get_parameters.py` & `tmart-2.3.1/tmart/AEC/get_parameters.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/identify_sensor.py` & `tmart-2.3.1/tmart/AEC/identify_sensor.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/irradiance_correction.py` & `tmart-2.3.1/tmart/AEC/irradiance_correction.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/read_PRISMA_north.py` & `tmart-2.3.1/tmart/AEC/read_PRISMA_north.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/read_PRISMA_vaa.py` & `tmart-2.3.1/tmart/AEC/read_PRISMA_vaa.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/read_config.py` & `tmart-2.3.1/tmart/AEC/read_config.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/read_metadata_Landsat.py` & `tmart-2.3.1/tmart/AEC/read_metadata_Landsat.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/read_metadata_S2.py` & `tmart-2.3.1/tmart/AEC/read_metadata_S2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/read_xml_S2.py` & `tmart-2.3.1/tmart/AEC/read_xml_S2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/read_xml_S2_scene.py` & `tmart-2.3.1/tmart/AEC/read_xml_S2_scene.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/run.py` & `tmart-2.3.1/tmart/AEC/run.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/run_acoliteL1R.py` & `tmart-2.3.1/tmart/AEC/run_acoliteL1R.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/run_regular.py` & `tmart-2.3.1/tmart/AEC/run_regular.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/AEC/write_atm_info.py` & `tmart-2.3.1/tmart/AEC/write_atm_info.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/Aerosol.py` & `tmart-2.3.1/tmart/Aerosol.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/Atmosphere.py` & `tmart-2.3.1/tmart/Atmosphere.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/Surface.py` & `tmart-2.3.1/tmart/Surface.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/Tmart.py` & `tmart-2.3.1/tmart/Tmart.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/Tmart2.py` & `tmart-2.3.1/tmart/Tmart2.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,20 @@
             sampled_tao = -math.log(random.random())
             
             # after moving the sampled_tao, the properties of the photon and the atmosphere layer 
             q1, tao_abs, ot_rayleigh_NA, ot_mie_NA, out = pt_move(atm_profile,q0,pt_direction,sampled_tao)
             # note: ot_rayleigh and ot_mie are replaced later, the accumulated ot should not be used, thus add _NA to mask them
     
             if self.print_on:
-                print ('\nq0: ' +str(q0))
-                print ('q1: ' +str(q1))
-                print ('tao_abs: ' +str(tao_abs))
-                print('sampled_tao: ' + str(sampled_tao))
-                print ('pt_direction: ' +str(pt_direction))
-                print('out: ' + str(out)) 
+                print ('\nInitial position: ' +str(q0))
+                print ('Final position: ' +str(q1))
+                print ('Absorption optical thickness (OT): ' +str(tao_abs))
+                print('Sampled OT: ' + str(sampled_tao))
+                print ('Photon moving direction: ' +str(pt_direction))
+                print('If out of atmosphere: ' + str(out)) 
             
             ### Test triangle collision             
 
             # If the two ends of the movement are both above the max elevation of the DEM, skip the test
             if self.Surface.DEM.max() < q0[2] and self.Surface.DEM.max() < q1[2]:
                 intersect_tri = pd.DataFrame()  
                 
@@ -148,15 +148,15 @@
                 
                 rotated_cm = None
                 
                 # Find triangle with the shortest distance and the exact collision point
                 intersect_tri_chosen = intersect_tri.iloc[intersect_tri.linear_distance.idxmin()] 
                 q_collision = intersect_tri_chosen.tolist()[0:3]  
                 
-                if self.print_on: print('q_collision: ' + str(q_collision))    
+                if self.print_on: print('Collision position: ' + str(q_collision))    
                 
                 # Re-calculate absorption 
                 tao_abs = find_OT(q0,q_collision,atm_profile)
                 tao_abs = tao_abs / abs(math.cos(pt_direction[0]/180*math.pi))  
                 
                 # Avoid intersecting again
                 q_collision[2] = q_collision[2] + 0.01 
@@ -169,26 +169,26 @@
                     print("\nNormal to collision: " + str(q_collision_N))
                     print("Normal to collision polar: " + str(q_collision_N_polar))                
                 
                 # Find the reflectance at the collision point 
                 q_collision_ref = reflectance_intersect(q_collision, self.Surface.reflectance, 
                                                         self.Surface.cell_size, self.Surface.bg_ref, 
                                                         self.Surface.bg_coords)
-                if self.print_on: print("q_collision_ref: " + str(q_collision_ref))    
+                if self.print_on: print("Reflectance at collision position: " + str(q_collision_ref))    
                 
             
                 ### If water --> there is a chance of specular reflectance             
                 # Chance is determined by Fresnel, pt_weight stays as 1
                 # Use pt_direction, q_collision_N and Cox-Munk to calculate the new pt_direction 
                 
                 # Test if it's water at the collision point 
                 q_collision_isWater = reflectance_intersect(q_collision, self.Surface.isWater, 
                                                             self.Surface.cell_size, self.Surface.bg_isWater, 
                                                             self.Surface.bg_coords)    
-                if self.print_on: print('\nq_collision_isWater: '+str(q_collision_isWater))
+                if self.print_on: print('\nIf surface is water: '+str(q_collision_isWater))
                 
     
                 # By default, non-specular. If chance, switch on 
                 specular_on = False
                 
                 # If water, calculate Fresnel reflectance and if specular reflection   
                 # q_collision_ref is now R0+
@@ -240,21 +240,21 @@
                         print("Rotated_cox_munk: " + str(rotated_cm)) 
                         print('Incident angle: ' + str(in_angle))
                         print('F_whitecap: ' + str(self.F_wc_wl))
                         print('R_whitecap: ' + str(self.R_wc_wl))
                         print('R_fresnel: ' + str(R_specular))
                         print('R_surf: ' + str(R_surf))
                         print('specular_on: ' + str(specular_on))
-                        print("Modified q_collision_ref: " + str(q_collision_ref))  
+                        # print("Modified reflectance at collision position: " + str(q_collision_ref))  
                           
                 pt_weight = pt_weight * q_collision_ref
                  
                 # If water and specular 
                 if q_collision_isWater == 1 and specular_on:
-                    if self.print_on: print('\n==Specular reflection==')  
+                    if self.print_on: print('\n== Specular reflection ==')  
                     
                     # Rotate pt_direction_op_C  around rotated_cm by 180 degrees       
                     rotated = np.dot(rotation_matrix(rotated_cm, math.pi), pt_direction_op_C)
        
                     # pt_direction is the specular reflection of the original direction at the new normal 
                     pt_direction = dirC_to_dirP(rotated)[0:2]
                     tpye_collision = 'Ws' # water specular
@@ -277,48 +277,48 @@
                     
                     pt_direction = dirC_to_dirP(rotated)[0:2]
                     tpye_collision = 'W'  # water lambertian 
                     
                     if self.print_on:
                         print("\nRandom_lambertian: " + str(random_lambertian))
                         print("Rotated_lambertian: " + str(rotated)) 
-                        print("q_collision_ref: " + str(q_collision_ref))
+                        # print("q_collision_ref: " + str(q_collision_ref))
                         
-                if self.print_on: print("pt_weight before absorption: " + str(pt_weight))      
+                if self.print_on: print("Photon weight before absorption: " + str(pt_weight))      
                 
                 
             ### Background collision     
             elif scenario == 2:
                 
                 # For plotting, not used 
                 rotated, rotated_cm, intersect_tri_chosen, q_collision_N = None, None, None, None 
                 q_collision_N_polar = [0,0] 
                 
                 
                 q_collision = intersect_bg 
-                if self.print_on: print('q_collision: ' + str(q_collision))  
+                if self.print_on: print('Collision position: ' + str(q_collision))  
                 
                 # re-calculate absorption 
                 tao_abs = find_OT(q0,q_collision,atm_profile)
                 tao_abs = tao_abs / abs(math.cos(pt_direction[0]/180*math.pi))                
                   
                 # Avoid intersecting again
                 q_collision[2] = q_collision[2] + 0.01 
     
                 # Reflectance of the background at the collision point 
                 q_collision_ref = reflectance_background(q_collision,self.Surface.bg_ref, self.Surface.bg_coords)
                 if self.print_on:
                     print ('\nOut of the padded DEM')
-                    print("q_collision_ref: " + str(q_collision_ref))
+                    print("Reflectance at collision position: " + str(q_collision_ref))
                 
                 # Test if it's water at the collision point 
                 q_collision_isWater = reflectance_intersect(q_collision, self.Surface.isWater, 
                                                             self.Surface.cell_size, self.Surface.bg_isWater, 
                                                             self.Surface.bg_coords)    
-                if self.print_on: print('\nq_collision_isWater: '+str(q_collision_isWater))                    
+                if self.print_on: print('\nIf surface is water: '+str(q_collision_isWater))                    
                 specular_on = False
                 
                 # If water, calculate Fresnel reflectance and if specular reflection   
                 # q_collision_ref is now R0-
                 if q_collision_isWater == 1:
                     
                     # Opposite to pt_direction in XYZ coordinates, only for isWater scenarios 
@@ -352,52 +352,52 @@
                         print('random_cox_munk: ' + str(random_cox_munk))
                         print('Incident angle: ' + str(in_angle))
                         print('F_whitecap: ' + str(self.F_wc_wl))
                         print('R_whitecap: ' + str(self.R_wc_wl))
                         print('R_fresnel: ' + str(R_specular))
                         print('R_surf: ' + str(R_surf))
                         print('specular_on: ' + str(specular_on))   
-                        print("Modified q_collision_ref: " + str(q_collision_ref))  
+                        # print("Modified reflectance at collision position: " + str(q_collision_ref))  
                 
                 pt_weight = pt_weight * q_collision_ref   
                 
                 # if water and specular 
                 if q_collision_isWater == 1 and specular_on:
-                    if self.print_on: print('\n==Specular reflection==')  
+                    if self.print_on: print('\n== Specular reflection ==')  
                         
                     rotated = np.dot(rotation_matrix(random_cox_munk, math.pi), pt_direction_op_C)
        
                     pt_direction = dirC_to_dirP(rotated)[0:2]
                     tpye_collision = 'Ws'
                     
                 # else lambertian 
                 else: 
                     # pt_direction = dirC_to_dirP(sample_Lambertian()[0])[0:2] # the line below can be faster???
                     pt_direction = sample_Lambertian()[1]
                     tpye_collision = 'W'
                         
-                if self.print_on: print("pt_weight before absorption: " + str(pt_weight))               
+                if self.print_on: print("Photon weight before absorption: " + str(pt_weight))               
             
             
             ### Photon movement and scattering 
             elif scenario == 3:
                 q_collision = q1
                 
                 ### Find ot_mie and ot_rayleigh
                 ot_rayleigh, ot_mie = find_atm2(atm_profile,q1)
                 pt_direction_op_C = np.negative(dirP_to_coord(1, pt_direction))
                 
                 # regular sampling  
                 if random.random() >= self.VROOM:
-                    if self.print_on: print('\n==Regular Sampling==')  
+                    if self.print_on: print('\n== Regular Sampling ==')  
                     pt_direction, scatt_intensity, type_scat = sample_scattering(ot_mie, ot_rayleigh, pt_direction, self.aerosol_SPF_wl, self.print_on)
     
                 # importance sampling 
                 else:
-                    if self.print_on: print('\n==Importance Sampling==')  
+                    if self.print_on: print('\n== Importance Sampling ==')  
                     
                     # Force mie scattering when importance sampling 
                     pt_direction, scatt_intensity, type_scat = sample_scattering(1, 0, self.sun_dir, self.Atmosphere.aerosol_SPF, self.print_on)
                     
                     
                     # angle between the old direction and the importance-sampled direction --> Scattering angle 
                     angle_impSampling = angle_3d(dirP_to_coord(1,pt_direction), [0,0,0], pt_direction_op_C)
@@ -412,32 +412,33 @@
             
             ###### Calculate absorption 
           
             T_abs = math.exp(-tao_abs) # tao_abs is unchanged if scenario 3 because the whole segment was used
             pt_weight = pt_weight * T_abs
             
             if self.print_on:
-                print('\n= Absorption =')
-                print("tao_abs: " + str(tao_abs))
-                print("T_abs: " + str(T_abs))
-                print("pt_weight: " + str(pt_weight))
-                print('\n= Local estimate =')
+                print('\n== Calculating absorption ==')
+                print("Modified absorption OT: " + str(tao_abs))
+                print("Absorption transmittance: " + str(T_abs))
+                print("Photon weight: " + str(pt_weight))
+                
                       
             
             ###### Local estimates 
             
             # Every movement has a row of local_est
             # Columes: pt_id, movement, L_cox-munk, L_whitecap, L_water, L_land, L_rayleigh, L_mie, surface xyz, shadowed, if_env, type of collision
             # Type of collision: W (water leaving), Ws (water specular), L (land), M (mie), R (Rayleigh)
             
             
             if_shadow = False
             
             # Reflection 
             if scenario == 1 or scenario == 2: 
+                if self.print_on: print('\n== Calculating local estimate ==')
                 
                 if movement == 0:
                     is_env = 0
                 else: # move>0 means at least one atmospheric scattering happened
                     is_env = 1
                 
                 if self.shadow: if_shadow = self.detect_shadow(q_collision)
@@ -455,14 +456,15 @@
                 
                 if if_shadow: local_est[11] = 1
                 if self.print_on: print("local_est: " + str(local_est))
                 pt_stat = np.vstack([pt_stat, local_est])     
                 
             # Scattering 
             if scenario == 3 and out == False:
+                if self.print_on: print('\n== Calculating local estimate ==')
                 
                 if self.shadow: if_shadow = self.detect_shadow(q_collision)
                 le_scatt = self.local_est_scat(pt_direction_op_C, q_collision, pt_weight, ot_mie, ot_rayleigh)
                 local_est = [pt_id, movement,0,0,0,0] + le_scatt + q_collision.tolist() + [0,0,type_scat]
                 if if_shadow: local_est[11] = 1
                 if self.print_on: print("local_est: " + str(local_est))
                 pt_stat = np.vstack([pt_stat, local_est])            
@@ -477,16 +479,15 @@
                     self._plot(q0, q_collision, scenario, intersect_tri_chosen, rotated, q_collision_N, specular_on, rotated_cm) 
                 
                 else: 
                     self._plot(q0, q_collision, scenario)
         
             # Exit if out 
             if out:
-                    
-                # Record information ???
+                if self.print_on: print('\nPhoton out of atmosphere \n')
                 break
         
             if self.print_on: print("\n------- Movement {} -------".format(movement+2))  
             # the last print won't show because the code breaks above
             # +2 because it starts from the 2nd one 
     
             # starting the next movement at the collision         
@@ -576,15 +577,15 @@
         
     def local_est_scat(self,pt_direction_op_C,q_collision, pt_weight, ot_mie, ot_rayleigh):
         
         # calculate remaining Transmittance 
         OT = self._local_est_OT(q_collision)
         OT = OT / math.cos(self.sun_dir[0]/180*math.pi)
         T = math.exp(-OT)
-        if self.print_on: print ('\nT_total for local_est: ' +str(T))
+        if self.print_on: print ('\nTotal transmittance for local_est: ' +str(T))
         
         # total scattering in that layer 
         ot_scattering = ot_mie + ot_rayleigh
         
         # angle between pt_direction and the sun 
         angle_pt_sun = angle_3d(dirP_to_coord(1,self.sun_dir), [0,0,0], pt_direction_op_C)
         
@@ -610,43 +611,44 @@
 
     def local_est_land(self, q_collision, pt_weight): 
     
         # Direct transmittance 
         OT = self._local_est_OT(q_collision)
         OT = OT / math.cos(self.sun_dir[0]/180*math.pi)
         T = math.exp(-OT)
-        if self.print_on: print ('\nT_total for local_est: ' +str(T))
+        if self.print_on: print ('\nTotal transmittance for local_est: ' +str(T))
         
         local_est = pt_weight * T / 1_000_000
         return [local_est]
    
     def local_est_water(self, pt_weight, pt_direction_op_C, q_collision, q_collision_N_polar, R_specular, q_collision_ref, R_surf):   
         
         R_wc = self.R_wc_wl
         
         # Cox-Munk and Fresnel, this one tells us nothing about the actual flux reflectance!
         R_cm = find_R_cm(pt_direction_op_C, self.sun_dir, q_collision_N_polar, 
                          self.wind_dir, self.wind_speed, self.water_refraIdx_wl, self.print_on)
         
         # Average = (regular + wind 90 degrees) / 2
         if self.wind_azi_avg:
-            if self.print_on: print ('\nSampling R_cm again...')
+            if self.print_on: print ('\nSampling R_cm again for azimuthally averaged values')
             
             R_cm2 = find_R_cm(pt_direction_op_C, self.sun_dir, q_collision_N_polar, 
                               self.wind_dir + 90, self.wind_speed, self.water_refraIdx_wl, self.print_on)
             R_cm = (R_cm + R_cm2) / 2
-        
+            
         R_cm = (1-self.F_wc_wl) * R_cm # remove whitecaps from cox-munk reflection 
+        if self.print_on:print('\nFinal cox_munk reflectance: '+str(R_cm))
         
         # Dicrect transmittance 
         OT = self._local_est_OT(q_collision)
         OT = OT / math.cos(self.sun_dir[0]/180*math.pi)
         T = math.exp(-OT)
         
-        if self.print_on: print ('\nT_total for local_est: ' +str(T))
+        if self.print_on: print ('\nTotal transmittance for local_est: ' +str(T))
             
         # cox-munk
         pt_weight_cm = pt_weight * (R_cm / q_collision_ref) 
         
         # whitecap
         pt_weight_wc = pt_weight * (R_wc / q_collision_ref)
         
@@ -666,15 +668,15 @@
         dist_120000 = (120_000 - q_collision[2]) / np.cos(self.sun_dir[0]/180*np.pi) 
         q_sun = dirP_to_coord(dist_120000, self.sun_dir) + q_collision
         
         intersect_tri = intersect_line_DEMtri2(q_collision, q_sun, self.Surface.DEM_triangulated, self.print_on)  
         
         if_shadow = intersect_tri.shape[0] > 0
         
-        if self.print_on: print ('\nif_shadow: ' +str(if_shadow))
+        if self.print_on: print ('\nIf shaded: ' +str(if_shadow))
         
         return if_shadow
         
 
     # finds OT between TOA and z
     def _local_est_OT(self,q_collision): 
         
@@ -734,33 +736,30 @@
         ax.set_ylabel('Y axis (m)')
         ax.set_zlabel('Z axis (m)')
         
         # Plotting DEM_tri
         for tri in self.Surface.DEM_triangulated:
             for row in range (0, tri.shape[2]):
                 for col in range (0, tri.shape[3]):
-                    # print (row, col)
             
                     p0 = tri[0,:,row,col] 
                     p1 = tri[1,:,row,col]
                     p2 = tri[2,:,row,col]
                     
-                    plot_tri = [p0,p1,p2]
-                    plot_tri = np.array([p0,p1,p2])
+                    plot_tri = np.array([[p0,p1,p2]])
                     
                     p_centre = (p0 + p1 + p2)/3
                     
                     q_collision_ref = reflectance_intersect(p_centre, self.Surface.reflectance, 
                                                             self.Surface.cell_size, self.Surface.bg_ref, 
                                                             self.Surface.bg_coords)    
                     
                     if q_collision_ref>1: q_collision_ref=1
                     if q_collision_ref<0: q_collision_ref=0
                     
-                    
                     poly = Poly3DCollection(plot_tri,
                                 #facecolors='ivory',
                                 facecolors=str(q_collision_ref),
                                 linewidths=0.5,
                                 edgecolors='black',
                                 alpha=0.9
                                 )
@@ -817,12 +816,12 @@
                     [triangle[1] ,  reflected_viz_q1[1]],
                     zs=[triangle[2] ,  reflected_viz_q1[2]],
                     color = 'orange',
                     zorder=100,
                     linewidth = linewidth
                     )
             
-            if self.print_on: print("Angle between normal and new pt_direction is: " + 
+            if self.print_on: print("Angle between normal and new moving direction is: " + 
                                     str(angle_3d(rotated,[0,0,0],q_collision_N)))
     
         # Plot atmospheres to the same extend as the surface 
         plt.show()
```

### Comparing `tmart-2.3.0/tmart/__init__.py` & `tmart-2.3.1/tmart/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/aerosolSPF/BiomassBurning.csv` & `tmart-2.3.1/tmart/ancillary/aerosolSPF/BiomassBurning.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/aerosolSPF/Continental.csv` & `tmart-2.3.1/tmart/ancillary/aerosolSPF/Continental.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/aerosolSPF/Desert.csv` & `tmart-2.3.1/tmart/ancillary/aerosolSPF/Desert.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/aerosolSPF/Maritime.csv` & `tmart-2.3.1/tmart/ancillary/aerosolSPF/Maritime.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/aerosolSPF/Stratospheric.csv` & `tmart-2.3.1/tmart/ancillary/aerosolSPF/Stratospheric.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/aerosolSPF/Urban.csv` & `tmart-2.3.1/tmart/ancillary/aerosolSPF/Urban.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/conifer_forest.csv` & `tmart-2.3.1/tmart/ancillary/conifer_forest.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/dry_beach_sand.csv` & `tmart-2.3.1/tmart/ancillary/dry_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/lawn_grass.csv` & `tmart-2.3.1/tmart/ancillary/lawn_grass.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/soil.csv` & `tmart-2.3.1/tmart/ancillary/soil.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/vegetation.csv` & `tmart-2.3.1/tmart/ancillary/vegetation.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/water_chl1.csv` & `tmart-2.3.1/tmart/ancillary/water_chl1.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/ancillary/wet_beach_sand.csv` & `tmart-2.3.1/tmart/ancillary/wet_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/config/config.txt` & `tmart-2.3.1/tmart/config/config.txt`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/surface_rho/calculate.py` & `tmart-2.3.1/tmart/surface_rho/calculate.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/tm_OT.py` & `tmart-2.3.1/tmart/tm_OT.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/tm_calcref.py` & `tmart-2.3.1/tmart/tm_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/tm_geometry.py` & `tmart-2.3.1/tmart/tm_geometry.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/tm_intersect.py` & `tmart-2.3.1/tmart/tm_intersect.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/tm_move.py` & `tmart-2.3.1/tmart/tm_move.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/tm_sampling.py` & `tmart-2.3.1/tmart/tm_sampling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.0/tmart/tm_water.py` & `tmart-2.3.1/tmart/tm_water.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         DESCRIPTION.
 
     '''
 
     # Find eta relative to q_collision_N_polar, wind-corrected 
     # AKA the needed angle for CM
     eta_P = find_eta_P(pt_direction_op_C,sun_dir,q_collision_N_polar,wind_dir)
-    if print_on: print('\neta_P, needed CM slopes in polar: '+str(eta_P))
+    if print_on: print('\neta_P, or needed Cox-Munk slope in polar: '+str(eta_P))
     
     # beta: steepest slope of the water surface facet
     beta = eta_P[0]/180*math.pi
     
     # eta_polar ==> coords ==> slopes 
     
     eta_coord = dirP_to_coord(1, eta_P[0:2])
@@ -351,15 +351,15 @@
     
     if print_on: 
         print('angle_pt_sun: '+str(angle_pt_sun))
         print('R_fresnel: '+str(R_specular))
         print('p_cox_munk: '+str(p_cox_munk))
         print('cos_solar_zenith: '+str(math.cos(solar_zenith)))
         print('cos_beta**4: '+str(math.cos(beta)**4))
-        print('Final cox_munk reflectance: '+str(rho_glint))
+        print('cox_munk reflectance: '+str(rho_glint))
     
     return rho_glint 
 
 
 
 # Sample a random slope, not related to the sun, correct to X direction  
 def sample_cox_munk(wind_speed, wind_dir):
```

### Comparing `tmart-2.3.0/tmart.egg-info/PKG-INFO` & `tmart-2.3.1/tmart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 2.3.0
+Version: 2.3.1
 Summary: Modelling and correcting for the adjacency effect in aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tmart-2.3.0/tmart.egg-info/SOURCES.txt` & `tmart-2.3.1/tmart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

