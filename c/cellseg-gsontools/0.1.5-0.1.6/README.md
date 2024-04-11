# Comparing `tmp/cellseg_gsontools-0.1.5.tar.gz` & `tmp/cellseg_gsontools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellseg_gsontools-0.1.5.tar", max compression
+gzip compressed data, was "cellseg_gsontools-0.1.6.tar", max compression
```

## Comparing `cellseg_gsontools-0.1.5.tar` & `cellseg_gsontools-0.1.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1065 2024-02-28 12:24:08.128316 cellseg_gsontools-0.1.5/LICENSE
--rw-r--r--   0        0        0     2500 2024-02-28 12:24:08.128316 cellseg_gsontools-0.1.5/README.md
--rw-r--r--   0        0        0      465 2024-02-28 12:24:08.128316 cellseg_gsontools-0.1.5/cellseg_gsontools/__init__.py
--rw-r--r--   0        0        0     2389 2024-02-28 12:24:08.128316 cellseg_gsontools-0.1.5/cellseg_gsontools/apply.py
--rw-r--r--   0        0        0    11369 2024-02-28 12:24:08.128316 cellseg_gsontools-0.1.5/cellseg_gsontools/character.py
--rw-r--r--   0        0        0     3538 2024-02-28 12:24:08.128316 cellseg_gsontools-0.1.5/cellseg_gsontools/clustering.py
--rw-r--r--   0        0        0      420 2024-02-28 12:24:08.128316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/__init__.py
--rw-r--r--   0        0        0  2454778 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/cervix_cells.feather
--rw-r--r--   0        0        0   165010 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/cervix_tissue.feather
--rw-r--r--   0        0        0     3043 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/fetch.py
--rw-r--r--   0        0        0    17890 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/gland_areas.feather
--rw-r--r--   0        0        0   244298 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/gland_cells.feather
--rw-r--r--   0        0        0     5690 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-41000_y-82000_areas.feather
--rw-r--r--   0        0        0    16266 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-41000_y-83000_areas.feather
--rw-r--r--   0        0        0    18882 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-41000_y-84000_areas.feather
--rw-r--r--   0        0        0    15090 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-42000_y-82000_areas.feather
--rw-r--r--   0        0        0    13754 2024-02-28 12:24:08.148316 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-42000_y-83000_areas.feather
--rw-r--r--   0        0        0    16946 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-42000_y-84000_areas.feather
--rw-r--r--   0        0        0     9818 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-43000_y-82000_areas.feather
--rw-r--r--   0        0        0    10466 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-43000_y-83000_areas.feather
--rw-r--r--   0        0        0    26890 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-43000_y-84000_areas.feather
--rw-r--r--   0        0        0    74578 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-41000_y-87000_cells.feather
--rw-r--r--   0        0        0    90178 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-41000_y-88000_cells.feather
--rw-r--r--   0        0        0    79578 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-41000_y-89000_cells.feather
--rw-r--r--   0        0        0    77930 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-42000_y-86000_cells.feather
--rw-r--r--   0        0        0    92386 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-42000_y-87000_cells.feather
--rw-r--r--   0        0        0    63234 2024-02-28 12:24:08.152317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-42000_y-88000_cells.feather
--rw-r--r--   0        0        0    91578 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-43000_y-86000_cells.feather
--rw-r--r--   0        0        0    79570 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-43000_y-87000_cells.feather
--rw-r--r--   0        0        0    67642 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-43000_y-88000_cells.feather
--rw-r--r--   0        0        0    13402 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/ts_iface_areas.feather
--rw-r--r--   0        0        0   270042 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/data/ts_iface_cells.feather
--rw-r--r--   0        0        0    13740 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/diversity.py
--rw-r--r--   0        0        0      787 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/__init__.py
--rw-r--r--   0        0        0     2660 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/axis.py
--rw-r--r--   0        0        0     2132 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/circle.py
--rw-r--r--   0        0        0     5528 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/mean_shape.py
--rw-r--r--   0        0        0    17521 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/shape_metrics.py
--rw-r--r--   0        0        0     9664 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/graphs.py
--rw-r--r--   0        0        0    16249 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/grid.py
--rw-r--r--   0        0        0     3805 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/intensity.py
--rw-r--r--   0        0        0     8781 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/lines.py
--rw-r--r--   0        0        0     7336 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/links.py
--rw-r--r--   0        0        0     2132 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/mask_utils.py
--rw-r--r--   0        0        0      156 2024-02-28 12:24:08.156317 cellseg_gsontools-0.1.5/cellseg_gsontools/merging/__init__.py
--rw-r--r--   0        0        0     2892 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/merging/_base_merger.py
--rw-r--r--   0        0        0     8346 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/merging/area_merger.py
--rw-r--r--   0        0        0    11538 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/merging/cell_merger.py
--rw-r--r--   0        0        0     6959 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/merging/gson_tile.py
--rw-r--r--   0        0        0     3363 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/merging/poly_utils.py
--rw-r--r--   0        0        0     6030 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/merging/save_utils.py
--rw-r--r--   0        0        0     4391 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/multiproc.py
--rw-r--r--   0        0        0    14993 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/neighbors.py
--rwxr-xr-x   0        0        0      122 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/plotting/__init__.py
--rwxr-xr-x   0        0        0     5991 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/plotting/plot.py
--rwxr-xr-x   0        0        0     2646 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/plotting/plot_graph.py
--rw-r--r--   0        0        0     2408 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/rasterize.py
--rw-r--r--   0        0        0      193 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/__init__.py
--rw-r--r--   0        0        0      149 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/__init__.py
--rw-r--r--   0        0        0     3141 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_base_backend.py
--rw-r--r--   0        0        0     7037 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_dgp_backend.py
--rw-r--r--   0        0        0     3444 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_gp_backend.py
--rw-r--r--   0        0        0     8859 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_sp_backend.py
--rw-r--r--   0        0        0    23057 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/interface.py
--rw-r--r--   0        0        0     7057 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/ops.py
--rw-r--r--   0        0        0     9375 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/point_cluster.py
--rw-r--r--   0        0        0    17908 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/within.py
--rw-r--r--   0        0        0    12508 2024-02-28 12:24:08.160317 cellseg_gsontools-0.1.5/cellseg_gsontools/utils.py
--rw-r--r--   0        0        0     5335 2024-02-28 12:24:08.376320 cellseg_gsontools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 cellseg_gsontools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-11 15:40:01.366225 cellseg_gsontools-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2500 2024-04-11 15:40:01.366225 cellseg_gsontools-0.1.6/README.md
+-rw-r--r--   0        0        0      465 2024-04-11 15:40:01.366225 cellseg_gsontools-0.1.6/cellseg_gsontools/__init__.py
+-rw-r--r--   0        0        0     2389 2024-04-11 15:40:01.366225 cellseg_gsontools-0.1.6/cellseg_gsontools/apply.py
+-rw-r--r--   0        0        0    11369 2024-04-11 15:40:01.366225 cellseg_gsontools-0.1.6/cellseg_gsontools/character.py
+-rw-r--r--   0        0        0     3538 2024-04-11 15:40:01.366225 cellseg_gsontools-0.1.6/cellseg_gsontools/clustering.py
+-rw-r--r--   0        0        0      420 2024-04-11 15:40:01.366225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/__init__.py
+-rw-r--r--   0        0        0  2454778 2024-04-11 15:40:01.382225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/cervix_cells.feather
+-rw-r--r--   0        0        0   165010 2024-04-11 15:40:01.382225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/cervix_tissue.feather
+-rw-r--r--   0        0        0     3043 2024-04-11 15:40:01.382225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/fetch.py
+-rw-r--r--   0        0        0    17890 2024-04-11 15:40:01.382225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/gland_areas.feather
+-rw-r--r--   0        0        0   244298 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/gland_cells.feather
+-rw-r--r--   0        0        0     5690 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-41000_y-82000_areas.feather
+-rw-r--r--   0        0        0    16266 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-41000_y-83000_areas.feather
+-rw-r--r--   0        0        0    18882 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-41000_y-84000_areas.feather
+-rw-r--r--   0        0        0    15090 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-42000_y-82000_areas.feather
+-rw-r--r--   0        0        0    13754 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-42000_y-83000_areas.feather
+-rw-r--r--   0        0        0    16946 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-42000_y-84000_areas.feather
+-rw-r--r--   0        0        0     9818 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-43000_y-82000_areas.feather
+-rw-r--r--   0        0        0    10466 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-43000_y-83000_areas.feather
+-rw-r--r--   0        0        0    26890 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-43000_y-84000_areas.feather
+-rw-r--r--   0        0        0    74578 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-41000_y-87000_cells.feather
+-rw-r--r--   0        0        0    90178 2024-04-11 15:40:01.386225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-41000_y-88000_cells.feather
+-rw-r--r--   0        0        0    79578 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-41000_y-89000_cells.feather
+-rw-r--r--   0        0        0    77930 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-42000_y-86000_cells.feather
+-rw-r--r--   0        0        0    92386 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-42000_y-87000_cells.feather
+-rw-r--r--   0        0        0    63234 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-42000_y-88000_cells.feather
+-rw-r--r--   0        0        0    91578 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-43000_y-86000_cells.feather
+-rw-r--r--   0        0        0    79570 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-43000_y-87000_cells.feather
+-rw-r--r--   0        0        0    67642 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-43000_y-88000_cells.feather
+-rw-r--r--   0        0        0    13402 2024-04-11 15:40:01.390225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/ts_iface_areas.feather
+-rw-r--r--   0        0        0   270042 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/data/ts_iface_cells.feather
+-rw-r--r--   0        0        0    13740 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/diversity.py
+-rw-r--r--   0        0        0      787 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/__init__.py
+-rw-r--r--   0        0        0     2660 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/axis.py
+-rw-r--r--   0        0        0     2132 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/circle.py
+-rw-r--r--   0        0        0     5528 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/mean_shape.py
+-rw-r--r--   0        0        0    17521 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/shape_metrics.py
+-rw-r--r--   0        0        0     9664 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/graphs.py
+-rw-r--r--   0        0        0    16249 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/grid.py
+-rw-r--r--   0        0        0     3805 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/intensity.py
+-rw-r--r--   0        0        0     8781 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/lines.py
+-rw-r--r--   0        0        0     7336 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/links.py
+-rw-r--r--   0        0        0     2132 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/mask_utils.py
+-rw-r--r--   0        0        0      156 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/merging/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/merging/_base_merger.py
+-rw-r--r--   0        0        0     8346 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/merging/area_merger.py
+-rw-r--r--   0        0        0    11541 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/merging/cell_merger.py
+-rw-r--r--   0        0        0     6959 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/merging/gson_tile.py
+-rw-r--r--   0        0        0     3363 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/merging/poly_utils.py
+-rw-r--r--   0        0        0     6036 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/merging/save_utils.py
+-rw-r--r--   0        0        0     4391 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/multiproc.py
+-rw-r--r--   0        0        0    14993 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/neighbors.py
+-rwxr-xr-x   0        0        0      122 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/plotting/__init__.py
+-rwxr-xr-x   0        0        0     5991 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/plotting/plot.py
+-rwxr-xr-x   0        0        0     2646 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/plotting/plot_graph.py
+-rw-r--r--   0        0        0     2408 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/rasterize.py
+-rw-r--r--   0        0        0      193 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/__init__.py
+-rw-r--r--   0        0        0     3141 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_base_backend.py
+-rw-r--r--   0        0        0     7037 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_dgp_backend.py
+-rw-r--r--   0        0        0     3444 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_gp_backend.py
+-rw-r--r--   0        0        0     8859 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_sp_backend.py
+-rw-r--r--   0        0        0    23057 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/interface.py
+-rw-r--r--   0        0        0     7057 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/ops.py
+-rw-r--r--   0        0        0     9375 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/point_cluster.py
+-rw-r--r--   0        0        0    17908 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/within.py
+-rw-r--r--   0        0        0    12508 2024-04-11 15:40:01.394225 cellseg_gsontools-0.1.6/cellseg_gsontools/utils.py
+-rw-r--r--   0        0        0     5335 2024-04-11 15:40:01.610227 cellseg_gsontools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 cellseg_gsontools-0.1.6/PKG-INFO
```

### Comparing `cellseg_gsontools-0.1.5/LICENSE` & `cellseg_gsontools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/README.md` & `cellseg_gsontools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/apply.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/apply.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/character.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/character.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/clustering.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/clustering.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/cervix_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/cervix_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/cervix_tissue.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/cervix_tissue.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/fetch.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/fetch.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/gland_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/gland_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/gland_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/gland_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-41000_y-82000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-41000_y-82000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-41000_y-83000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-41000_y-83000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-41000_y-84000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-41000_y-84000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-42000_y-82000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-42000_y-82000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-42000_y-83000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-42000_y-83000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-42000_y-84000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-42000_y-84000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-43000_y-82000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-43000_y-82000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-43000_y-83000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-43000_y-83000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/area/x-43000_y-84000_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/area/x-43000_y-84000_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-41000_y-87000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-41000_y-87000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-41000_y-88000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-41000_y-88000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-41000_y-89000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-41000_y-89000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-42000_y-86000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-42000_y-86000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-42000_y-87000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-42000_y-87000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-42000_y-88000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-42000_y-88000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-43000_y-86000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-43000_y-86000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-43000_y-87000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-43000_y-87000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/merge_data/cell/x-43000_y-88000_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/merge_data/cell/x-43000_y-88000_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/ts_iface_areas.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/ts_iface_areas.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/data/ts_iface_cells.feather` & `cellseg_gsontools-0.1.6/cellseg_gsontools/data/ts_iface_cells.feather`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/diversity.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/diversity.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/__init__.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/axis.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/axis.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/circle.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/circle.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/mean_shape.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/mean_shape.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/geometry/shape_metrics.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/geometry/shape_metrics.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/graphs.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/graphs.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/grid.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/grid.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/intensity.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/intensity.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/lines.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/lines.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/links.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/links.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/mask_utils.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/mask_utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/merging/_base_merger.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/merging/_base_merger.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/merging/area_merger.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/merging/area_merger.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/merging/cell_merger.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/merging/cell_merger.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         """Merge all the instance segmentation files in the input directory.
 
         Parameters:
             out_fn (Union[Path, str]):
                 Filename for the output file. If None, the merged gdf is saved to the
                 class attribute `self.annots` only.
             format (str):
-                The format of the output geojson file. One of: "feather", "parquet",
-                "geojson", None. This is ignored if `out_fn` is None.
+                The format of the output geojson file. One of: ".feather", ".parquet",
+                ".geojson", None. This is ignored if `out_fn` is None.
             verbose (bool):
                 Whether to show a progress bar or not.
 
         Examples:
             Write geojson files to a standard '.geojson' file.
             >>> from cellseg_gsontools.merging import CellMerger
             >>> merger = CellMerger("/path/to/geojsons/", tile_size=(1000, 1000))
```

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/merging/gson_tile.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/merging/gson_tile.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/merging/poly_utils.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/merging/poly_utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/merging/save_utils.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/merging/save_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import re
 from pathlib import Path
 from typing import List, Tuple, Union
 
 import geopandas as gpd
 
-from ..apply import gdf_apply
+from cellseg_gsontools.apply import gdf_apply
 
 __all__ = [
     "check_format",
     "get_xy_coords",
     "get_file_from_coords",
     "gdf_to_file",
 ]
 
 
-def _add_qupath_classification(row: gpd.GeoSeries) -> gpd.GeoSeries:
+def _add_qupath_classification(class_name: str) -> gpd.GeoSeries:
     """Add QuPath properties to a row of a gdf."""
-    c = row["class_name"]
-    props = {"name": c, "color": None}
+    props = {"name": class_name, "color": None}
     return props
 
 
 def gdf_to_file(
     gdf: gpd.GeoDataFrame,
     out_fn: Union[str, Path],
     format: str = ".feather",
@@ -60,15 +59,15 @@
     # add objectType col (QuPath)
     if "objectType" not in gdf.columns:
         gdf["objectType"] = "annotation"
 
     # add classification col (QuPath)
     if "classification" not in gdf.columns:
         gdf["classification"] = gdf_apply(
-            gdf, _add_qupath_classification, columns=None, axis=1
+            gdf, _add_qupath_classification, axis=1, columns=["class_name"]
         )
 
     if format == ".feather":
         gdf.to_feather(out_fn.with_suffix(".feather"))
     elif format == ".parquet":
         gdf.to_parquet(out_fn.with_suffix(".parquet"))
     elif format == ".geojson":
```

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/multiproc.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/multiproc.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/neighbors.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/neighbors.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/plotting/plot.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/plotting/plot_graph.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/plotting/plot_graph.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/rasterize.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/rasterize.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_base_backend.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_base_backend.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_dgp_backend.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_dgp_backend.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_gp_backend.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_gp_backend.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/backend/_sp_backend.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/backend/_sp_backend.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/interface.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/interface.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/ops.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/ops.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/point_cluster.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/point_cluster.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/spatial_context/within.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/spatial_context/within.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/cellseg_gsontools/utils.py` & `cellseg_gsontools-0.1.6/cellseg_gsontools/utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_gsontools-0.1.5/pyproject.toml` & `cellseg_gsontools-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cellseg-gsontools"
-version = "0.1.5"
+version = "0.1.6"
 description = "Toolbelt for merging and extracting features from geojson masks."
 authors = ["Okunator <oskari.lehtonen@helsinki.fi>"]
 readme = "README.md"
 homepage = "https://github.com/okunator/cellseg_gsontools"
 repository = "https://github.com/okunator/cellseg_gsontools"
 packages = [{ include = "cellseg_gsontools" }]
```

### Comparing `cellseg_gsontools-0.1.5/PKG-INFO` & `cellseg_gsontools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellseg-gsontools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Toolbelt for merging and extracting features from geojson masks.
 Home-page: https://github.com/okunator/cellseg_gsontools
 Author: Okunator
 Author-email: oskari.lehtonen@helsinki.fi
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

