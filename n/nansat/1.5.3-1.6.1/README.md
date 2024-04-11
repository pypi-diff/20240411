# Comparing `tmp/nansat-1.5.3.tar.gz` & `tmp/nansat-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nansat-1.5.3.tar", last modified: Tue Dec 13 12:48:57 2022, max compression
+gzip compressed data, was "nansat-1.6.1.tar", last modified: Thu Apr 11 12:34:28 2024, max compression
```

## Comparing `nansat-1.5.3.tar` & `nansat-1.6.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (122)    35127 2022-12-13 12:48:56.000000 nansat-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-12-13 12:48:56.000000 nansat-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1400 2022-12-13 12:48:57.000000 nansat-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5336 2022-12-13 12:48:56.000000 nansat-1.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat/
--rw-r--r--   0 runner    (1001) docker     (122)     1736 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32792 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/domain.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    18899 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (122)    35567 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   720012 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/fonts/DejaVuSans.ttf
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/geolocation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat/mappers/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19395 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/envisat.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3439 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/get_grib.pl
--rwxr-xr-x   0 runner    (1001) docker     (122)     3150 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/get_inv.pl
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/globcolour.py
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/hdf4_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    10643 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_aapp_l1b.py
--rw-r--r--   0 runner    (1001) docker     (122)     9490 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_aapp_l1c.py
--rw-r--r--   0 runner    (1001) docker     (122)     5111 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_amsr2_l1r.py
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_amsr2_l3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_amsre_uham_leadfraction.py
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_arome.py
--rw-r--r--   0 runner    (1001) docker     (122)    13280 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_asar.py
--rw-r--r--   0 runner    (1001) docker     (122)     2532 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_ascat.py
--rw-r--r--   0 runner    (1001) docker     (122)     5647 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_aster_l1a.py
--rw-r--r--   0 runner    (1001) docker     (122)     5494 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_aster_l1b.py
--rw-r--r--   0 runner    (1001) docker     (122)     2618 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_case2reg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2269 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_cmems.py
--rw-r--r--   0 runner    (1001) docker     (122)     7937 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_csks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_ecmwf_metno.py
--rw-r--r--   0 runner    (1001) docker     (122)     2955 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_emodnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    15618 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)    24579 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_geostationary.py
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_globcolour_l3b.py
--rw-r--r--   0 runner    (1001) docker     (122)     6274 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_globcolour_l3m.py
--rw-r--r--   0 runner    (1001) docker     (122)     2523 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_goci_l1.py
--rw-r--r--   0 runner    (1001) docker     (122)     4095 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_hirlam.py
--rw-r--r--   0 runner    (1001) docker     (122)     4217 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_hirlam_wind_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2428 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_kmss.py
--rw-r--r--   0 runner    (1001) docker     (122)     6591 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)     7318 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_meris_l1.py
--rw-r--r--   0 runner    (1001) docker     (122)     9725 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_meris_l2.py
--rw-r--r--   0 runner    (1001) docker     (122)     6968 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_metno_hfr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3882 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_metno_hires_seaice.py
--rw-r--r--   0 runner    (1001) docker     (122)     2772 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_metno_local_hires_seaice.py
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_mod44w.py
--rw-r--r--   0 runner    (1001) docker     (122)    20692 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_modis_l1.py
--rw-r--r--   0 runner    (1001) docker     (122)     5439 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_ncep.py
--rw-r--r--   0 runner    (1001) docker     (122)     4046 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_ncep_wind.py
--rw-r--r--   0 runner    (1001) docker     (122)     6319 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_ncep_wind_online.py
--rw-r--r--   0 runner    (1001) docker     (122)    19066 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_netcdf_cf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_netcdf_cf_sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (122)     5106 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_nora10_local_vpv.py
--rw-r--r--   0 runner    (1001) docker     (122)    13311 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_obpg_l2.py
--rw-r--r--   0 runner    (1001) docker     (122)     6122 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_obpg_l2_nc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8499 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_obpg_l3.py
--rw-r--r--   0 runner    (1001) docker     (122)     5327 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_ocean_productivity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3837 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_arome.py
--rw-r--r--   0 runner    (1001) docker     (122)     3045 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_globcurrent.py
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_globcurrent_thredds.py
--rw-r--r--   0 runner    (1001) docker     (122)     3091 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_mywave.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_occci.py
--rw-r--r--   0 runner    (1001) docker     (122)     3073 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_osisaf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6131 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_ostia.py
--rw-r--r--   0 runner    (1001) docker     (122)     4824 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_sentinel1_wind.py
--rw-r--r--   0 runner    (1001) docker     (122)     3006 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_sentinel2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_siwtacsst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2333 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_opendap_sstcci.py
--rw-r--r--   0 runner    (1001) docker     (122)     3711 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_pathfinder52.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_quikscat.py
--rw-r--r--   0 runner    (1001) docker     (122)    15452 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_radarsat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    25487 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_sentinel1_l1.py
--rw-r--r--   0 runner    (1001) docker     (122)     8233 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_sentinel1_l2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2831 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_topography.py
--rw-r--r--   0 runner    (1001) docker     (122)     4859 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/mapper_viirs_l1.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/obpg.py
--rw-r--r--   0 runner    (1001) docker     (122)    13143 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/opendap.py
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/scatterometers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7613 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/mappers/sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (122)    60720 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/nansat.py
--rw-r--r--   0 runner    (1001) docker     (122)    11570 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/node.py
--rw-r--r--   0 runner    (1001) docker     (122)     3256 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/nsr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat/pixelfunctions/
--rw-r--r--   0 runner    (1001) docker     (122)      793 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      574 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/MakefileWin
--rw-r--r--   0 runner    (1001) docker     (122)      783 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/README.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/README_Nansat
--rw-r--r--   0 runner    (1001) docker     (122)      836 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/_pixfun_py2.c
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/_pixfun_py3.c
--rw-r--r--   0 runner    (1001) docker     (122)    57315 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/pixelfunctions.c
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pixelfunctions/pixfunplugin.c
--rw-r--r--   0 runner    (1001) docker     (122)     6428 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/pointbrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)   350912 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/arctic.nc
--rw-r--r--   0 runner    (1001) docker     (122)   327344 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/complex.nc
--rw-r--r--   0 runner    (1001) docker     (122)   126224 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/gcps.tif
--rw-r--r--   0 runner    (1001) docker     (122)  2164298 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/map.tif
--rw-r--r--   0 runner    (1001) docker     (122)     7534 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/nansat_logo_s.png
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/points.dbf
--rw-r--r--   0 runner    (1001) docker     (122)      212 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/points.shp
--rw-r--r--   0 runner    (1001) docker     (122)      132 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/points.shx
--rw-r--r--   0 runner    (1001) docker     (122)      197 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/some_xml_file.xml
--rw-r--r--   0 runner    (1001) docker     (122)   218690 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/data/stere.tif
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat/tests/mappers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16960 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/mappers/test_mapper_netcdf_cf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8767 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/mappers/test_mapper_opendap.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/mappers/test_mapper_opendap_arome.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/mappers/test_mapper_opendap_mywave.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/mappers/test_mapper_opendap_ostia.py
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/nansat_test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/nansat_test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    26206 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (122)    19088 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_geolocation.py
--rw-r--r--   0 runner    (1001) docker     (122)    34081 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_nansat.py
--rw-r--r--   0 runner    (1001) docker     (122)     5838 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_nsr.py
--rw-r--r--   0 runner    (1001) docker     (122)      410 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_pixelfunctions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3888 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_pointbrowser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3948 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2250 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    29775 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tests/test_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     7406 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     9214 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    71074 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)      357 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1400 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4667 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       52 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/nansat_integration_tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat_integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6401 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat_integration_tests/mapper_test_archive.py
--rw-r--r--   0 runner    (1001) docker     (122)     4636 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat_integration_tests/test_mappers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6464 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat_integration_tests/test_netcdf_cf_mappers.py
--rw-r--r--   0 runner    (1001) docker     (122)      816 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat_integration_tests/test_open_issues.py
--rw-r--r--   0 runner    (1001) docker     (122)     4314 2022-12-13 12:48:56.000000 nansat-1.5.3/nansat_integration_tests/test_radarsat2.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-13 12:48:57.000000 nansat-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     9264 2022-12-13 12:48:56.000000 nansat-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-13 12:48:57.000000 nansat-1.5.3/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1653 2022-12-13 12:48:56.000000 nansat-1.5.3/utilities/nansat_add_coastline
--rwxr-xr-x   0 runner    (1001) docker     (122)      697 2022-12-13 12:48:56.000000 nansat-1.5.3/utilities/nansat_geotiffimage
--rwxr-xr-x   0 runner    (1001) docker     (122)      814 2022-12-13 12:48:56.000000 nansat-1.5.3/utilities/nansat_show
--rwxr-xr-x   0 runner    (1001) docker     (122)      728 2022-12-13 12:48:56.000000 nansat-1.5.3/utilities/nansat_translate
--rwxr-xr-x   0 runner    (1001) docker     (122)      416 2022-12-13 12:48:56.000000 nansat-1.5.3/utilities/nansatinfo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.088415 nansat-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35127 2024-04-11 12:34:26.000000 nansat-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 12:34:26.000000 nansat-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-11 12:34:28.088415 nansat-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-11 12:34:26.000000 nansat-1.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.068415 nansat-1.6.1/nansat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21060 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35475 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/figure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.068415 nansat-1.6.1/nansat/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   720012 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/fonts/DejaVuSans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/geolocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.076415 nansat-1.6.1/nansat/mappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19395 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/envisat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3439 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/get_grib.pl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3150 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/get_inv.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/globcolour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/hdf4_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aapp_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aapp_l1c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_amsr2_l1r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_amsr2_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_amsre_uham_leadfraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_arome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_asar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ascat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aster_l1a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_aster_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_case2reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_cmems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_csks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ecmwf_metno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_emodnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_geostationary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_globcolour_l3b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_globcolour_l3m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_goci_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_hirlam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_hirlam_wind_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_kmss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_meris_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_meris_l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_metno_hfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_metno_hires_seaice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_metno_local_hires_seaice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_mod44w.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20692 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_modis_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ncep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ncep_wind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ncep_wind_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19296 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_netcdf_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_netcdf_cf_sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_nora10_local_vpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_obpg_l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_obpg_l2_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_obpg_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_ocean_productivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_arome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent_thredds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_mywave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_occci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_osisaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_ostia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1_wind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_siwtacsst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_opendap_sstcci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_pathfinder52.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_quikscat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_radarsat2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25487 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_sentinel1_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_sentinel1_l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_topography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/mapper_viirs_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/obpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/scatterometers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/mappers/sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60463 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/nansat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/nsr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.076415 nansat-1.6.1/nansat/pixelfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/MakefileWin
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/README_Nansat
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/_pixfun_py2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/_pixfun_py3.c
+-rw-r--r--   0 runner    (1001) docker     (127)    57315 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/pixelfunctions.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pixelfunctions/pixfunplugin.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/pointbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.080415 nansat-1.6.1/nansat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.084415 nansat-1.6.1/nansat/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   350912 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/arctic.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   327344 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/complex.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   126224 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/gcps.tif
+-rw-r--r--   0 runner    (1001) docker     (127)  2164298 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/map.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/nansat_logo_s.png
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/points.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/points.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/points.shx
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/some_xml_file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   218690 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/data/stere.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.084415 nansat-1.6.1/nansat/tests/mappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_netcdf_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap_arome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap_mywave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap_ostia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/nansat_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/nansat_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_geolocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34081 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_nansat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_nsr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_pixelfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_pointbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29775 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tests/test_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71148 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/vrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.068415 nansat-1.6.1/nansat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 12:34:28.000000 nansat-1.6.1/nansat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.088415 nansat-1.6.1/nansat_integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/mapper_test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_netcdf_cf_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_open_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-11 12:34:26.000000 nansat-1.6.1/nansat_integration_tests/test_radarsat2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:34:28.088415 nansat-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-11 12:34:26.000000 nansat-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:34:28.088415 nansat-1.6.1/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1653 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_add_coastline
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_geotiffimage
+-rwxr-xr-x   0 runner    (1001) docker     (127)      814 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_show
+-rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansat_translate
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-04-11 12:34:26.000000 nansat-1.6.1/utilities/nansatinfo
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nansat-1.5.3/LICENSE` & `nansat-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/PKG-INFO` & `nansat-1.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: nansat
-Version: 1.5.3
+Version: 1.6.1
 Summary: A scientist friendly Python toolbox for processing 2D satellite Earth observation data
 Home-page: https://github.com/nansencenter/nansat
+Download-URL: https://github.com/nansencenter/nansat
 Author: Anton Korosov, Morten W. Hansen, Kunt-Frode Dagestad, Aleksander Vines, Asuka Yamakawa, Artem Moiseev, Mohamed Babiker
 Author-email: nansat-dev@googlegroups.com
 Maintainer: Nansat Developers
 Maintainer-email: nansat-dev@googlegroups.com
 License: GNU General Public License
-Download-URL: https://github.com/nansencenter/nansat
-Description: A scientist friendly Python toolbox for processing 2D satellite Earth observation data
 Platform: Linux
 Platform: OS X
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -23,7 +22,10 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+A scientist friendly Python toolbox for processing 2D satellite Earth observation data
```

### Comparing `nansat-1.5.3/README.rst` & `nansat-1.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 +---------+------------------------+---------------------------+------------+
 
 .. NOTE: include statements doesn't work with github README.rst - the first section here is repeated
 .. in docs/source/about.rst as well...
 
 .. BEGIN REPETITION ===============================
 
-.. image:: https://www.nersc.no/sites/www.nersc.no/files/images/nansat_logo_transp.png
+.. image:: docs/source/images/nansat_logo_transp.png
    :align: right
    :width: 250px
    :target: https://github.com/nansencenter/nansat
 
 **Nansat** is a scientist friendly Python toolbox for processing 2D
 satellite earth observation data.
```

### Comparing `nansat-1.5.3/nansat/__init__.py` & `nansat-1.6.1/nansat/__init__.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/domain.py` & `nansat-1.6.1/nansat/domain.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/exceptions.py` & `nansat-1.6.1/nansat/exceptions.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/exporter.py` & `nansat-1.6.1/nansat/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 
 class Exporter(object):
     """Abstract class for export functions """
     DEFAULT_INSTITUTE = 'NERSC'
     DEFAULT_SOURCE = 'satellite remote sensing'
 
     UNWANTED_METADATA = ['dataType', 'SourceFilename', 'SourceBand', '_Unsigned', 'FillValue',
-                                'time', '_FillValue', 'type', 'scale', 'offset']
+                         '_FillValue', 'type', 'scale', 'offset', 'NETCDF_VARNAME']
 
     def export(self, filename='', bands=None, rm_metadata=None, add_geolocation=True,
-               driver='netCDF', options=None, hardcopy=False):
+               driver='netCDF', options='FORMAT=NC4', hardcopy=False):
         """Export Nansat object into netCDF or GTiff file
 
         Parameters
         -----------
         filename : str
             output file name
         bands: list (default=None)
@@ -53,32 +53,28 @@
         rm_metadata : list
             metadata names for removal before export.
             e.g. ['name', 'colormap', 'source', 'sourceBands']
         add_geolocation : bool
             add geolocation array datasets to exported file?
         driver : str
             Name of GDAL driver (format)
-        options : str or list
+        options : str or list (default: 'FORMAT=NC4' for NetCDF 4
+                  file format)
             GDAL export options in format of: 'OPT=VAL', or
             ['OPT1=VAL1', 'OP2='VAL2']
             See also http://www.gdal.org/frmt_netcdf.html
         hardcopy : bool
             Evaluate all bands just before export?
 
         Returns
         -------
         filename : netCDF or GTiff
 
         Notes
         ------
-        If number of bands is more than one, serial numbers are added at the end of each band name.
-        It is possible to fix it by changing line.4605 in GDAL/frmts/netcdf/netcdfdataset.cpp :
-        'if( nBands > 1 ) sprintf(szBandName,"%s%d",tmpMetadata,iBand);'
-        --> 'if( nBands > 1 ) sprintf(szBandName,"%s",tmpMetadata);'
-
         CreateCopy fails in case the band name has special characters,
         e.g. the slash in 'HH/VV'.
 
         Metadata strings with special characters are escaped with XML/HTML
         encoding.
 
         Examples
@@ -112,22 +108,83 @@
 
         if driver == 'GTiff':
             add_gcps = export_vrt.prepare_export_gtiff()
         else:
             add_gcps = export_vrt.prepare_export_netcdf()
 
         # Create output file using GDAL
-        dataset = gdal.GetDriverByName(driver).CreateCopy(filename, export_vrt.dataset, options=options)
+        dataset = gdal.GetDriverByName(driver).CreateCopy(filename, export_vrt.dataset,
+                                                          options=options)
         del dataset
         # add GCPs into netCDF file as separate float variables
         if add_gcps:
             Exporter._add_gcps(filename, export_vrt.dataset.GetGCPs())
 
+        if driver=='netCDF':
+            # Rename variable names to get rid of the band numbers
+            self.rename_variables(filename)
+            # Rename attributes to get rid of "GDAL_" added by gdal
+            self.rename_attributes(filename)
+
         self.logger.debug('Export - OK!')
 
+    @staticmethod
+    def rename_attributes(filename):
+        """ Rename global attributes to get rid of the "GDAL_"-string
+        added by gdal.
+        """
+        GDAL = "GDAL_"
+        del_attrs = []
+        rename_attrs = []
+        # Open new file to edit attribute names
+        with Dataset(filename, 'r+') as ds:
+            """ The netcdf driver adds the Conventions attribute with
+            value CF-1.5. This may be wrong, so it is better to use the
+            Conventions metadata from the Nansat object. Other attributes
+            added by gdal that are already present in Nansat, should also
+            be deleted."""
+            for attr in ds.ncattrs():
+                if GDAL in attr:
+                    if attr.replace(GDAL, "") in ds.ncattrs():
+                        # Mark the attribute created by the netcdf driver
+                        # for deletion - ref above comment
+                        del_attrs.append(attr.replace(GDAL, ""))
+                    # Mark for renaming
+                    rename_attrs.append(attr)
+
+            # Delete repeated attributes..
+            for attr in del_attrs:
+                ds.delncattr(attr)
+            # Rename attributes:
+            for attr in rename_attrs:
+                ds.renameAttribute(attr, attr.replace(GDAL, ""))
+
+    @staticmethod
+    def rename_variables(filename):
+        """ Rename variable names to reflect the name attribute of
+        the variable's metadata.
+
+        Parameters
+        ----------
+        filename : str
+            NetCDF file name
+        """
+        # Open new file to edit variable names
+        with Dataset(filename, 'r+') as ds:
+            # Decide which variables to rename
+            rename_vars = []
+            for var in ds.variables.keys():
+                if ('name' in ds.variables[var].ncattrs()) and (
+                        var != ds.variables[var].getncattr('name')):
+                    rename_vars.append(var)
+
+            # Rename selected variables
+            for var in rename_vars:
+                ds.renameVariable(var, ds.variables[var].getncattr('name'))
+
     def export2thredds(self,
         filename,
         bands=None,
         metadata=None,
         mask_name=None,
         no_mask_value=64,
         rm_metadata=None,
```

### Comparing `nansat-1.5.3/nansat/figure.py` & `nansat-1.6.1/nansat/figure.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,16 +771,14 @@
             # write text each line onto pilImgCanvas
             textHeight = int(self.pilImgLegend.size[1] *
                              self.TITLE_LOCATION_Y)
             for line in self.titleString.splitlines():
                 draw.text((int(self.pilImgLegend.size[0] *
                                self.TITLE_LOCATION_X),
                            textHeight), line, fill=black, font=font)
-                text = draw.textsize(line, font=font)
-                textHeight += text[1]
 
     def create_pilImage(self, **kwargs):
         """self.create_pilImage is replaced from None to PIL image
 
         If three images are given, create a image with RGB mode.
         if self.pilImgLegend is not None, it is pasted.
```

### Comparing `nansat-1.5.3/nansat/fonts/DejaVuSans.ttf` & `nansat-1.6.1/nansat/fonts/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/geolocation.py` & `nansat-1.6.1/nansat/geolocation.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/envisat.py` & `nansat-1.6.1/nansat/mappers/envisat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/get_grib.pl` & `nansat-1.6.1/nansat/mappers/get_grib.pl`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/get_inv.pl` & `nansat-1.6.1/nansat/mappers/get_inv.pl`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/globcolour.py` & `nansat-1.6.1/nansat/mappers/globcolour.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/hdf4_mapper.py` & `nansat-1.6.1/nansat/mappers/hdf4_mapper.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_aapp_l1b.py` & `nansat-1.6.1/nansat/mappers/mapper_aapp_l1b.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_aapp_l1c.py` & `nansat-1.6.1/nansat/mappers/mapper_aapp_l1c.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_amsr2_l1r.py` & `nansat-1.6.1/nansat/mappers/mapper_amsr2_l1r.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_amsr2_l3.py` & `nansat-1.6.1/nansat/mappers/mapper_amsr2_l3.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_amsre_uham_leadfraction.py` & `nansat-1.6.1/nansat/mappers/mapper_amsre_uham_leadfraction.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_arome.py` & `nansat-1.6.1/nansat/mappers/mapper_arome.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_asar.py` & `nansat-1.6.1/nansat/mappers/mapper_asar.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_ascat.py` & `nansat-1.6.1/nansat/mappers/mapper_ascat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_aster_l1a.py` & `nansat-1.6.1/nansat/mappers/mapper_aster_l1a.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_aster_l1b.py` & `nansat-1.6.1/nansat/mappers/mapper_aster_l1b.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_case2reg.py` & `nansat-1.6.1/nansat/mappers/mapper_case2reg.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_cmems.py` & `nansat-1.6.1/nansat/mappers/mapper_cmems.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_csks.py` & `nansat-1.6.1/nansat/mappers/mapper_csks.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_ecmwf_metno.py` & `nansat-1.6.1/nansat/mappers/mapper_ecmwf_metno.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_emodnet.py` & `nansat-1.6.1/nansat/mappers/mapper_emodnet.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_generic.py` & `nansat-1.6.1/nansat/mappers/mapper_generic.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_geostationary.py` & `nansat-1.6.1/nansat/mappers/mapper_geostationary.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_globcolour_l3b.py` & `nansat-1.6.1/nansat/mappers/mapper_globcolour_l3b.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_globcolour_l3m.py` & `nansat-1.6.1/nansat/mappers/mapper_globcolour_l3m.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class Mapper(VRT, Globcolour):
     """Mapper for GLOBCOLOR L3M products"""
 
     def __init__(self, filename, gdalDataset, gdalMetadata, **kwargs):
         ''' GLOBCOLOR L3M VRT '''
 
         try:
-            print("=>%s<=" % gdalMetadata['NC_GLOBAL#title'])
+            x = "=>%s<=" % gdalMetadata['NC_GLOBAL#title']
         except (TypeError, KeyError):
             raise WrongMapperError
 
         if 'GlobColour' not in gdalMetadata['NC_GLOBAL#title']:
             raise WrongMapperError
 
         # get list of similar (same date) files in the directory
```

### Comparing `nansat-1.5.3/nansat/mappers/mapper_goci_l1.py` & `nansat-1.6.1/nansat/mappers/mapper_goci_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_hirlam.py` & `nansat-1.6.1/nansat/mappers/mapper_hirlam.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_hirlam_wind_netcdf.py` & `nansat-1.6.1/nansat/mappers/mapper_hirlam_wind_netcdf.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_kmss.py` & `nansat-1.6.1/nansat/mappers/mapper_kmss.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_landsat.py` & `nansat-1.6.1/nansat/mappers/mapper_landsat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_meris_l1.py` & `nansat-1.6.1/nansat/mappers/mapper_meris_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_meris_l2.py` & `nansat-1.6.1/nansat/mappers/mapper_meris_l2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_metno_hfr.py` & `nansat-1.6.1/nansat/mappers/mapper_metno_hfr.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_metno_hires_seaice.py` & `nansat-1.6.1/nansat/mappers/mapper_metno_hires_seaice.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_metno_local_hires_seaice.py` & `nansat-1.6.1/nansat/mappers/mapper_metno_local_hires_seaice.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_mod44w.py` & `nansat-1.6.1/nansat/mappers/mapper_mod44w.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_modis_l1.py` & `nansat-1.6.1/nansat/mappers/mapper_modis_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_ncep.py` & `nansat-1.6.1/nansat/mappers/mapper_ncep.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_ncep_wind.py` & `nansat-1.6.1/nansat/mappers/mapper_ncep_wind.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_ncep_wind_online.py` & `nansat-1.6.1/nansat/mappers/mapper_ncep_wind_online.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_netcdf_cf.py` & `nansat-1.6.1/nansat/mappers/mapper_netcdf_cf.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,18 @@
 
         self.input_filename = filename
 
         if not gdal_metadata:
             raise WrongMapperError
 
         if 'NC_GLOBAL#GDAL_NANSAT_GCPY_000' in list(gdal_metadata.keys()) or \
-                'NC_GLOBAL#GDAL_NANSAT_GCPProjection' in list(gdal_metadata.keys()):
-            # Probably Nansat generated netcdf of swath data - see issue #192
+                'NC_GLOBAL#GDAL_NANSAT_GCPProjection' in list(gdal_metadata.keys()) or \
+                'NC_GLOBAL#NANSAT_GCPY_000' in list(gdal_metadata.keys()) or \
+                'NC_GLOBAL#NANSAT_GCPProjection' in list(gdal_metadata.keys()):
+            # Nansat generated netcdf of swath data is not standard CF
             raise WrongMapperError
 
         metadata = VRT._remove_strings_in_metadata_keys(gdal_metadata,
                                                         ['NC_GLOBAL#', 'NANSAT_', 'GDAL_'])
 
         # Set origin metadata (TODO: agree on keyword...)
         origin = ''
@@ -273,14 +275,15 @@
             get_band_number()
 
         get_band_number()
 
         subds = gdal.Open(fn)
         band = subds.GetRasterBand(Context.band_number)
         band_metadata = self._clean_band_metadata(band)
+        band_metadata['_FillValue'] = band.GetNoDataValue()
 
         return self._band_dict(fn, Context.band_number, subds, band=band,
                         band_metadata=band_metadata)
 
     def _clean_band_metadata(self, band, remove = ['_Unsigned', 'ScaleRatio',
         'ScaleOffset', 'PixelFunctionType']):
 
@@ -313,15 +316,15 @@
             if self._timevarname() in list(band_metadata.keys()):
                 timecountname = self._timevarname()
             else:
                 timecountname = 'NETCDF_DIM_'+self._timevarname()
             try:
                 band_metadata['time_iso_8601'] = self._time_count_to_np_datetime64(
                     band_metadata[timecountname])
-            except KeyError as e:
+            except (ValueError, KeyError) as e:
                 # No timing information available for this band - it is
                 # probably a constant, such as land area fraction or similar.
                 # Then we don't need time for this band...
                 # The following warning is not really understandable..
                 tttt = 0 # do nothing...
                 #warnings.warn(
                 #        '%s: %s - %s Continuing without time metadata for band %s'
```

### Comparing `nansat-1.5.3/nansat/mappers/mapper_netcdf_cf_sentinel1.py` & `nansat-1.6.1/nansat/mappers/mapper_netcdf_cf_sentinel1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_nora10_local_vpv.py` & `nansat-1.6.1/nansat/mappers/mapper_nora10_local_vpv.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_obpg_l2.py` & `nansat-1.6.1/nansat/mappers/mapper_obpg_l2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_obpg_l2_nc.py` & `nansat-1.6.1/nansat/mappers/mapper_obpg_l2_nc.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_obpg_l3.py` & `nansat-1.6.1/nansat/mappers/mapper_obpg_l3.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_ocean_productivity.py` & `nansat-1.6.1/nansat/mappers/mapper_ocean_productivity.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_arome.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_arome.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_globcurrent.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_globcurrent_thredds.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_globcurrent_thredds.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_mywave.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_mywave.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_occci.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_occci.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_osisaf.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_osisaf.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_ostia.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_ostia.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_sentinel1.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from nansat.nsr import NSR
 from nansat.utils import initial_bearing
 
 
 class Mapper(Opendap, Sentinel1):
 
     baseURLs = [
+            'https://nbstds.met.no/thredds/dodsC/NBS/S1A',
+            'https://nbstds.met.no/thredds/dodsC/NBS/S1B',
             'http://nbstds.met.no/thredds/dodsC/NBS/S1A',
             'http://nbstds.met.no/thredds/dodsC/NBS/S1B',
     ]
 
     timeVarName = 'time'
     xName = 'x'
     yName = 'y'
```

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_sentinel1_wind.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel1_wind.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_sentinel2.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_sentinel2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_siwtacsst.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_siwtacsst.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_opendap_sstcci.py` & `nansat-1.6.1/nansat/mappers/mapper_opendap_sstcci.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_pathfinder52.py` & `nansat-1.6.1/nansat/mappers/mapper_pathfinder52.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_quikscat.py` & `nansat-1.6.1/nansat/mappers/mapper_quikscat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_radarsat2.py` & `nansat-1.6.1/nansat/mappers/mapper_radarsat2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_sentinel1_l1.py` & `nansat-1.6.1/nansat/mappers/mapper_sentinel1_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_sentinel1_l2.py` & `nansat-1.6.1/nansat/mappers/mapper_sentinel1_l2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_topography.py` & `nansat-1.6.1/nansat/mappers/mapper_topography.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/mapper_viirs_l1.py` & `nansat-1.6.1/nansat/mappers/mapper_viirs_l1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/obpg.py` & `nansat-1.6.1/nansat/mappers/obpg.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/opendap.py` & `nansat-1.6.1/nansat/mappers/opendap.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/scatterometers.py` & `nansat-1.6.1/nansat/mappers/scatterometers.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/mappers/sentinel1.py` & `nansat-1.6.1/nansat/mappers/sentinel1.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/nansat.py` & `nansat-1.6.1/nansat/nansat.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,14 @@
 
     Nansat inherits from Domain (container of geo-reference information)
     Nansat uses instance of VRT (wraper around GDAL VRT-files)
     Nansat uses instance of Figure (collection of methods for visualization)
 
     """
 
-    FILL_VALUE = 9.96921e+36
-    ALT_FILL_VALUE = -10000.
-
     # instance attributes
     logger = None
     filename = None
     name = None
     path = None
     vrt = None
     mapper = None
@@ -261,18 +258,14 @@
         if array is not None:
             self.add_band(array=array, parameters=parameters)
 
     def _fill_with_nan(self, band, band_data):
         """Fill input array with fill value taen from input band metadata"""
         fill_value = float(band.GetMetadata()['_FillValue'])
         band_data[band_data == fill_value] = np.nan
-        # quick hack to avoid problem with wrong _FillValue - see issue
-        # #123
-        if fill_value == self.FILL_VALUE:
-            band_data[band_data == self.ALT_FILL_VALUE] = np.nan
 
         return band_data
 
 
     def add_band(self, array, parameters=None, nomem=False):
         """Add band from numpy array with metadata.
 
@@ -1063,15 +1056,15 @@
     def _get_dataset_metadata(self):
         # open GDAL dataset. It will be parsed to all mappers for testing
         gdal_dataset, metadata = None, dict()
         if not self.filename.startswith('http'):
             try:
                 gdal_dataset = gdal.Open(self.filename)
             except RuntimeError:
-                self.logger.error('GDAL could not open %s, trying to read with Nansat mappers...'
+                self.logger.debug('GDAL could not open %s, trying to read with Nansat mappers...'
                                   % self.filename)
         if gdal_dataset is not None:
             # get metadata from the GDAL dataset
             metadata = gdal_dataset.GetMetadata()
 
         return gdal_dataset, metadata
 
@@ -1118,15 +1111,15 @@
             nansatMappers = _import_mappers()
 
         # open GDAL dataset. It will be parsed to all mappers for testing
         gdal_dataset, metadata = self._get_dataset_metadata()
         tmp_vrt = None
 
         # TODO: There seems to be code repetition in this if-test - should be avoided...
-        if mappername is not '':
+        if mappername != '':
             # If a specific mapper is requested, we test only this one.
             # get the module name
             mappername = 'mapper_' + mappername.replace('mapper_', '').replace('.py', '').lower()
             # check if the mapper is available
             if mappername not in nansatMappers:
                 raise ValueError('Mapper ' + mappername + ' not found')
```

### Comparing `nansat-1.5.3/nansat/node.py` & `nansat-1.6.1/nansat/node.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/nsr.py` & `nansat-1.6.1/nansat/nsr.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # http://www.gnu.org/licenses/gpl-3.0.html
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 from __future__ import absolute_import, unicode_literals
 import sys
 from nansat.utils import osr
+osr.UseExceptions()
 
 from nansat.exceptions import NansatProjectionError
 
 
 class NSR(osr.SpatialReference, object):
     """Nansat Spatial Reference. Overrides constructor of osr.SpatialReference.
 
@@ -55,34 +56,37 @@
             str_types = (str, unicode)
         else:
             str_types = str
         # create SRS
         osr.SpatialReference.__init__(self)
 
         # parse input parameters
-        status = 1
         if srs is 0:
             # generate default WGS84 SRS
-            status = self.ImportFromEPSG(4326)
+            self.ImportFromEPSG(4326)
         elif isinstance(srs, str_types):
             # parse as proj4 string
-            status = self.ImportFromProj4(str(srs))
-            if status > 0:
+            try:
+                self.ImportFromProj4(str(srs))
+            except RuntimeError:
                 # parse as WKT string
-                status = self.ImportFromWkt(str(srs))
-            if status > 0:
-                raise NansatProjectionError('Proj4 or WKT (%s) is wrong' % srs)
+                try:
+                    self.ImportFromWkt(str(srs))
+                except RuntimeError:
+                    raise NansatProjectionError('Proj4 or WKT (%s) is wrong' % srs)
         elif isinstance(srs, int):
             # parse as EPSG code
-            status = self.ImportFromEPSG(srs)
-            if status > 0:
+            try:
+                self.ImportFromEPSG(srs)
+            except RuntimeError:
                 raise NansatProjectionError('EPSG %d is wrong' % srs)
         elif type(srs) in [osr.SpatialReference, NSR]:
             # parse from input Spatial Reference
-            status = self.ImportFromWkt(srs.ExportToWkt())
-            if status > 0:
+            try:
+                self.ImportFromWkt(srs.ExportToWkt())
+            except RuntimeError:
                 raise NansatProjectionError('NSR %s is wrong' % srs)
 
     @property
     def wkt(self):
         """Well Known Text representation of SRS"""
         return self.ExportToWkt()
```

### Comparing `nansat-1.5.3/nansat/pixelfunctions/Makefile` & `nansat-1.6.1/nansat/pixelfunctions/Makefile`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pixelfunctions/MakefileWin` & `nansat-1.6.1/nansat/pixelfunctions/MakefileWin`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pixelfunctions/README.txt` & `nansat-1.6.1/nansat/pixelfunctions/README.txt`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pixelfunctions/README_Nansat` & `nansat-1.6.1/nansat/pixelfunctions/README_Nansat`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pixelfunctions/_pixfun_py2.c` & `nansat-1.6.1/nansat/pixelfunctions/_pixfun_py2.c`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pixelfunctions/_pixfun_py3.c` & `nansat-1.6.1/nansat/pixelfunctions/_pixfun_py3.c`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pixelfunctions/pixelfunctions.c` & `nansat-1.6.1/nansat/pixelfunctions/pixelfunctions.c`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pixelfunctions/pixfunplugin.c` & `nansat-1.6.1/nansat/pixelfunctions/pixfunplugin.c`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/pointbrowser.py` & `nansat-1.6.1/nansat/pointbrowser.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/data/arctic.nc` & `nansat-1.6.1/nansat/tests/data/arctic.nc`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/data/complex.nc` & `nansat-1.6.1/nansat/tests/data/complex.nc`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/data/gcps.tif` & `nansat-1.6.1/nansat/tests/data/gcps.tif`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/data/map.tif` & `nansat-1.6.1/nansat/tests/data/map.tif`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/data/nansat_logo_s.png` & `nansat-1.6.1/nansat/tests/data/nansat_logo_s.png`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/data/stere.tif` & `nansat-1.6.1/nansat/tests/data/stere.tif`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/mappers/test_mapper_netcdf_cf.py` & `nansat-1.6.1/nansat/tests/mappers/test_mapper_netcdf_cf.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/mappers/test_mapper_opendap.py` & `nansat-1.6.1/nansat/tests/mappers/test_mapper_opendap.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/nansat_test_base.py` & `nansat-1.6.1/nansat/tests/nansat_test_base.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/nansat_test_data.py` & `nansat-1.6.1/nansat/tests/nansat_test_data.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_domain.py` & `nansat-1.6.1/nansat/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_exporter.py` & `nansat-1.6.1/nansat/tests/test_exporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,23 +33,78 @@
 except ImportError:
     MATPLOTLIB_IS_INSTALLED = False
 else:
     MATPLOTLIB_IS_INSTALLED = True
 
 from netCDF4 import Dataset
 
-from nansat import Nansat, Domain, NSR
+from nansat import Nansat, Domain, NSR, exporter
 from nansat.utils import gdal
 from nansat.tests.nansat_test_base import NansatTestBase
 
 warnings.simplefilter("always", UserWarning)
 
 
 class ExporterTest(NansatTestBase):
 
+    def test_export__with_nan_values(self):
+        """Test that a band with nan-values is masked as expected,
+        that global attribute names are the same as the Nansat
+        metadata, and that variable names are the same as the Nansat
+        band names without appended numbers."""
+        n = Nansat(self.test_file_arctic)
+        aa = n['Bootstrap'].astype(float)
+        aa = np.ma.masked_where(
+            aa == float(n.get_metadata(band_id='Bootstrap', key='_FillValue')), aa)
+        aa.data[aa.mask] = np.nan
+        bb = aa.data.copy()
+        bb[2,:] = np.nan
+        n.add_band(bb, parameters={'name': 'test_band_with_nans'})
+    
+        cc = np.zeros(bb.shape)
+        cc[np.isnan(bb)] = 1
+        sumnan = cc.sum()
+
+        # temp file for exported netcdf
+        fd, tmp_ncfile = tempfile.mkstemp(suffix='.nc')
+
+        # export with nansat
+        n.export(tmp_ncfile)
+
+        ds = Dataset(tmp_ncfile)
+        # Check that the number of elements in bb and the new file
+        # equal to np.nan is the same when opened with netCDF4.Dataset:
+        dd = ds.variables['test_band_with_nans'][:]
+        ee = np.zeros(dd.shape)
+        ee[np.isnan(dd)] = 1
+        self.assertEqual(ee.sum(), sumnan)
+
+        # Check that the global metadata attribute names are the same
+        orig_metadata = list(n.get_metadata().keys())
+        ncattrs = ds.ncattrs()
+        for attr in orig_metadata:
+            self.assertIn(attr, ncattrs)
+
+        # Check that variable names don't contain band numbers
+        self.assertEqual(list(ds.variables.keys()), ['polar_stereographic', 'x', 'y',
+            'UMass_AES', 'Bootstrap', 'Bristol', 'test_band_with_nans'])
+
+        # Open the tmp file using nansat, and check that the Bootstrap
+        # band from the tmp file is the same as the one in the original
+        n = Nansat(tmp_ncfile)
+        ff = n['Bootstrap']
+        ff = np.ma.masked_where(
+                ff == float(n.get_metadata(band_id='Bootstrap', key='_FillValue')), ff)
+        # This only works when the fill value (-10000) in arctic.nc is
+        # treated correctly (with python3.9 and GDAL3.4.1)
+        self.assertEqual(ff.mask[0,239], aa.mask[0,239])
+
+        os.close(fd)
+        os.unlink(tmp_ncfile)
+
     def test_geolocation_of_exportedNC_vs_original(self):
         """ Lon/lat in original and exported file should coincide """
         orig = Nansat(self.test_file_gcps, mapper=self.default_mapper)
         orig.export(self.tmp_filename)
 
         copy = Nansat(self.tmp_filename, mapper=self.default_mapper)
         lon0, lat0 = orig.get_geolocation_grids()
@@ -281,15 +336,15 @@
 
         tmpfilename = os.path.join(self.tmp_data_path,
                                    'nansat_export2thredds_longlat.nc')
         n.export2thredds(tmpfilename, {'L_469': {'type': '>i1'}})
         ncI = Dataset(tmpfilename, 'r')
         ncIVar = ncI.variables['L_469']
         self.assertTrue(ncIVar.grid_mapping in ncI.variables.keys())
-        self.assertEqual(ncIVar[:].dtype, np.int8)
+        self.assertEqual(ncIVar[:].dtype, np.uint8)
 
     def test_export_netcdf_complex_remove_meta(self):
         n = Nansat(self.test_file_complex, mapper=self.default_mapper)
         self.assertEqual(n.get_metadata('PRODUCT_TYPE'), 'SLC')
         n.export(self.tmp_filename, rm_metadata=['PRODUCT_TYPE'])
         exported = Nansat(self.tmp_filename, mapper=self.default_mapper)
         with self.assertRaises(ValueError):
@@ -405,15 +460,17 @@
         self.assertTrue(os.path.exists(self.filename_exported))
         ds = Dataset(self.filename_exported)
         self.assertEqual(ds.variables['x_wind_10m'][0,0,0].data, 9)
         self.assertTrue(np.isnan(ds.variables['x_wind_10m'][0,-1,0].data))
 
     def test_example2(self):
         n = Nansat(self.tmp_ncfile)
-        res = n.export2thredds(self.filename_exported, {'x_wind_10m': {'description': 'example'}})
+        res = n.export2thredds(
+            self.filename_exported,
+            {'x_wind_10m': {'description': 'example'}})
         self.assertEqual(res, None)
 
     def test_example3(self):
         n = Nansat(self.tmp_ncfile)
         res = n.export2thredds(self.filename_exported, {
             'x_wind_10m': {'type': '>i2', 'scale': 0.1, 'offset': 0},
             'y_wind_10m': {'type': '>i2', 'scale': 0.1, 'offset': 0}
```

### Comparing `nansat-1.5.3/nansat/tests/test_figure.py` & `nansat-1.6.1/nansat/tests/test_figure.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_geolocation.py` & `nansat-1.6.1/nansat/tests/test_geolocation.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_nansat.py` & `nansat-1.6.1/nansat/tests/test_nansat.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_node.py` & `nansat-1.6.1/nansat/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_nsr.py` & `nansat-1.6.1/nansat/tests/test_nsr.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.assertEqual(type(nsr), NSR)
         self.assertEqual(nsr.Validate(), 0)
 
     def test_init_from_none(self):
         nsr = NSR(None)
 
         self.assertEqual(type(nsr), NSR)
-        self.assertEqual(nsr.Validate(), 5)
+        self.assertRaises(RuntimeError, nsr.Validate)
 
     def test_init_from_0(self):
         nsr = NSR(0)
 
         self.assertEqual(type(nsr), NSR)
         self.assertEqual(nsr.Validate(), 0)
```

### Comparing `nansat-1.5.3/nansat/tests/test_pointbrowser.py` & `nansat-1.6.1/nansat/tests/test_pointbrowser.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_tools.py` & `nansat-1.6.1/nansat/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_utils.py` & `nansat-1.6.1/nansat/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tests/test_vrt.py` & `nansat-1.6.1/nansat/tests/test_vrt.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/tools.py` & `nansat-1.6.1/nansat/tools.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat/utils.py` & `nansat-1.6.1/nansat/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,80 +59,80 @@
         keys = []
     for key in keys:
         dict.pop(key, None)
     return dict
 
 def register_colormaps():
     ''' Create custom colormaps and register them '''
-    obpg = {'red': [(0.00, 0.56, 0.56),
+    colormaps = {
+        'obpg': {
+            'red': [(0.00, 0.56, 0.56),
                     (0.19, 0.00, 0.00),
                     (0.38, 0.00, 0.00),
                     (0.50, 0.00, 0.00),
                     (0.63, 1.00, 1.00),
                     (0.88, 1.00, 1.00),
                     (1.00, 0.40, 0.40)],
-
             'green': [(0.00, 0.00, 0.00),
                       (0.19, 0.00, 0.00),
                       (0.38, 1.00, 1.00),
                       (0.50, 1.00, 1.00),
                       (0.63, 1.00, 1.00),
                       (0.88, 0.00, 0.00),
                       (1.00, 0.00, 0.00)],
-
             'blue': [(0.00, 0.43, 0.43),
                      (0.19, 1.00, 1.00),
                      (0.38, 1.00, 1.00),
                      (0.50, 0.00, 0.00),
                      (0.63, 0.00, 0.00),
                      (0.88, 0.00, 0.00),
                      (1.00, 0.00, 0.00)],
-            }
-
-
-    ak01 = {'red': [(0, 0.1, 0.1,),
+        },
+        'ak01': {
+            'red': [(0, 0.1, 0.1,),
                     (0.1, 0.56, 0.56,),
                     (0.22, 0, 0,),
                     (0.27, 0, 0,),
                     (0.37, 0.3, 0.3,),
                     (0.47, 0, 0,),
                     (0.52, 0, 0,),
                     (0.64, 1, 1,),
                     (0.76, 1, 1,),
                     (0.88, 0.4, 0.4,),
                     (1, 1, 1,)],
-
             'green': [(0, 0, 0,),
-                      (0.1, 0, 0,),
-                      (0.22, 0, 0,),
-                      (0.27, 0, 0,),
-                      (0.37, 0.6, 0.6,),
-                      (0.47, 0.6, 0.6,),
-                      (0.52, 1, 1,),
-                      (0.64, 1, 1,),
-                      (0.76, 0, 0,),
-                      (0.88, 0, 0,),
-                      (1, 0.5, 0.5,)],
-
+                    (0.1, 0, 0,),
+                    (0.22, 0, 0,),
+                    (0.27, 0, 0,),
+                    (0.37, 0.6, 0.6,),
+                    (0.47, 0.6, 0.6,),
+                    (0.52, 1, 1,),
+                    (0.64, 1, 1,),
+                    (0.76, 0, 0,),
+                    (0.88, 0, 0,),
+                    (1, 0.5, 0.5,)],
             'blue': [(0, 0.1, 0.1,),
-                     (0.1, 0.5, 0.5,),
-                     (0.22, 0.5, 0.5,),
-                     (0.27, 1, 1,),
-                     (0.37, 1, 1,),
-                     (0.47, 0, 0,),
-                     (0.52, 0, 0,),
-                     (0.64, 0, 0,),
-                     (0.76, 0, 0,),
-                     (0.88, 0, 0,),
-                     (1, 0.5, 0.5,)],
-            }
+                    (0.1, 0.5, 0.5,),
+                    (0.22, 0.5, 0.5,),
+                    (0.27, 1, 1,),
+                    (0.37, 1, 1,),
+                    (0.47, 0, 0,),
+                    (0.52, 0, 0,),
+                    (0.64, 0, 0,),
+                    (0.76, 0, 0,),
+                    (0.88, 0, 0,),
+                    (1, 0.5, 0.5,)],
+        }
+    }
 
     if MATPLOTLIB_IS_INSTALLED:
-        cm.register_cmap(cmap=LinearSegmentedColormap('obpg', obpg, 256))
-        cm.register_cmap(cmap=LinearSegmentedColormap('ak01', ak01, 256))
+        for name, colormap in colormaps.items():
+            if name not in matplotlib.colormaps:
+                cm.register_cmap(cmap=LinearSegmentedColormap(name, colormap, 256))
+
 
 def initial_bearing(lon1, lat1, lon2, lat2):
         """Initial bearing when traversing from point1 (lon1, lat1)
         to point2 (lon2, lat2)
 
         See http://www.movable-type.co.uk/scripts/latlong.html
```

### Comparing `nansat-1.5.3/nansat/vrt.py` & `nansat-1.6.1/nansat/vrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,17 @@
         # get metadata from input and gdal_dataset
         # metadata = kwargs.pop('metadata', dict())
         # metadata.update(gdal_dataset.GetMetadata())
         # set dataset parameters and metadata
         VRT.__init__(self, gdal_dataset.RasterXSize, gdal_dataset.RasterYSize, **kwargs)
         self.dataset.SetGCPs(gdal_dataset.GetGCPs(), gdal_dataset.GetGCPProjection())
         self.dataset.SetProjection(gdal_dataset.GetProjection())
-        self.dataset.SetGeoTransform(gdal_dataset.GetGeoTransform())
+        geotransform = gdal_dataset.GetGeoTransform(can_return_null=1)
+        if geotransform:
+            self.dataset.SetGeoTransform(geotransform)
         if geolocation is None:
             geolocation = Geolocation.from_dataset(gdal_dataset)
         self._add_geolocation(geolocation)
         self.dataset.SetMetadataItem(str('filename'), self.filename)
 
         # write XML file contents
         self.dataset.FlushCache()
@@ -376,15 +378,15 @@
         batch_size = 0x20000000 # 512 MB
         for i in range(0,len(array_bytes),batch_size):
             ind_start = i
             ind_end   = min(i+batch_size,len(array_bytes))
             gdal.VSIFWriteL(array_bytes[ind_start:ind_end],ind_end-ind_start,1,ofile)
         gdal.VSIFCloseL(ofile)
         array_bytes = None
-        
+
         # convert Numpy datatype to gdal datatype and pixel offset
         gdal_data_type = numpy_to_gdal_type[array_type]
         pixel_offset = gdal_type_to_offset[gdal_data_type]
 
         # create XML contents of VRT-file
         line_offset = str(int(pixel_offset) * array_shape[1])
         contents = self.RAW_RASTER_BAND_SOURCE_XML.substitute(
```

### Comparing `nansat-1.5.3/nansat.egg-info/PKG-INFO` & `nansat-1.6.1/nansat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: nansat
-Version: 1.5.3
+Version: 1.6.1
 Summary: A scientist friendly Python toolbox for processing 2D satellite Earth observation data
 Home-page: https://github.com/nansencenter/nansat
+Download-URL: https://github.com/nansencenter/nansat
 Author: Anton Korosov, Morten W. Hansen, Kunt-Frode Dagestad, Aleksander Vines, Asuka Yamakawa, Artem Moiseev, Mohamed Babiker
 Author-email: nansat-dev@googlegroups.com
 Maintainer: Nansat Developers
 Maintainer-email: nansat-dev@googlegroups.com
 License: GNU General Public License
-Download-URL: https://github.com/nansencenter/nansat
-Description: A scientist friendly Python toolbox for processing 2D satellite Earth observation data
 Platform: Linux
 Platform: OS X
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -23,7 +22,10 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+A scientist friendly Python toolbox for processing 2D satellite Earth observation data
```

### Comparing `nansat-1.5.3/nansat.egg-info/SOURCES.txt` & `nansat-1.6.1/nansat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat_integration_tests/mapper_test_archive.py` & `nansat-1.6.1/nansat_integration_tests/mapper_test_archive.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat_integration_tests/test_mappers.py` & `nansat-1.6.1/nansat_integration_tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat_integration_tests/test_netcdf_cf_mappers.py` & `nansat-1.6.1/nansat_integration_tests/test_netcdf_cf_mappers.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat_integration_tests/test_open_issues.py` & `nansat-1.6.1/nansat_integration_tests/test_open_issues.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/nansat_integration_tests/test_radarsat2.py` & `nansat-1.6.1/nansat_integration_tests/test_radarsat2.py`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/setup.py` & `nansat-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,18 @@
     try:
         files = os.listdir(path)
     except:
         extra_link_args = []
     else:
         if 'gdal_i.lib' in files:
             extra_link_args = [path + '\gdal_i.lib']
+        elif 'gdal.lib' in files:
+            extra_link_args = [path + '\gdal.lib']
+        else:
+            extra_link_args = []
 else:
     extra_compile_args = ['-fPIC', '-Wall', '-Wno-long-long', '-pedantic', '-O3']
     extra_link_args = [] # not used currently
 
 
 def _ask_gdal_config(resultlist, option, result_prefix):
     p = Popen(['gdal-config', option], stdout=subprocess.PIPE)
```

### Comparing `nansat-1.5.3/utilities/nansat_add_coastline` & `nansat-1.6.1/utilities/nansat_add_coastline`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/utilities/nansat_geotiffimage` & `nansat-1.6.1/utilities/nansat_geotiffimage`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/utilities/nansat_show` & `nansat-1.6.1/utilities/nansat_show`

 * *Files identical despite different names*

### Comparing `nansat-1.5.3/utilities/nansat_translate` & `nansat-1.6.1/utilities/nansat_translate`

 * *Files identical despite different names*

