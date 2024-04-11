# Comparing `tmp/GridCalEngine-5.1.4.tar.gz` & `tmp/GridCalEngine-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCalEngine-5.1.4.tar", last modified: Tue Apr  9 17:48:27 2024, max compression
+gzip compressed data, was "GridCalEngine-5.1.5.tar", last modified: Thu Apr 11 17:55:28 2024, max compression
```

## Comparing `GridCalEngine-5.1.4.tar` & `GridCalEngine-5.1.5.tar`

### file list

```diff
@@ -1,677 +1,678 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)    10942 2024-03-14 19:48:07.696505 GridCalEngine-5.1.4/GridCalEngine/data_logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    38600 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/enumerations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23610 2024-03-14 19:48:07.696505 GridCalEngine-5.1.4/GridCalEngine/basic_structures.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-04-08 13:34:15.975164 GridCalEngine-5.1.4/GridCalEngine/api.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Utils/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/objects_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/timeseries_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9723 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/results_table_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/iwamoto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15007 2024-03-17 11:12:27.697061 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/ips.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/powell.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/autodiff.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/csc_numba.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/csc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Utils/ThirdParty/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.4/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/selected_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/ortools_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/pulp_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/highs.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Topology/topology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21322 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Topology/simulation_indices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9597 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Topology/topology_substation_reduction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.4/GridCalEngine/Topology/admittance_matrices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.4/GridCalEngine/IO/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21444 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/IO/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.4/GridCalEngine/IO/base/base_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.4/GridCalEngine/IO/base/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.4/GridCalEngine/IO/base/units.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.4/GridCalEngine/IO/base/base_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/IO/base/base_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/dgs/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/dgs/dgs_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/raw/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/IO/raw/rawx_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/IO/raw/gridcal_to_raw.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/raw/rawx_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/gne_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/switched_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/system_switching_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/psse_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/facts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/owner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/inter_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/psse_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/psse_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/vsc_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/induction_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/fixed_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_storage_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_gen_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/matpower/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_bus_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_branch_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54205 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/pack_unpack.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16095 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/zip_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    98239 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/json_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/generic_io_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/h5_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    47307 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/excel_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/sqlite_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/contingency_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/epc/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.4/GridCalEngine/IO/epc/epc_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/IO/others/dpx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.4/GridCalEngine/IO/others/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/IO/others/ipa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.4/GridCalEngine/IO/others/pypsa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/IO/others/plx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    49748 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15944 2024-03-28 10:16:48.980877 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2229 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25096 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/base.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12411 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_export.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26275 2024-04-08 13:34:15.971164 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    81740 2024-04-08 13:34:15.971164 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2211 2024-04-08 13:34:15.971164 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4216 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_devices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/base_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/psse_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/db_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2499 2024-04-08 13:34:15.971164 GridCalEngine-5.1.4/GridCalEngine/Devices/types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8637 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/sparse_array.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.4/GridCalEngine/Devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   193160 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/multi_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/Devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14901 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/profile.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/municipality.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/contingency_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1813 2024-04-08 13:34:15.971164 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3022 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4255 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/contingency.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3045 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/emission_gas.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/country.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1332 2024-04-08 13:34:15.971164 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/modelling_authority.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2558 2024-03-28 10:16:48.972877 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2547 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2008 2024-03-14 19:59:31.532490 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2174 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/investments_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3715 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/investment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/community.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/branch_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_path.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8074 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_turbine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_injection_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_p2x.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10753 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/underground_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10243 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/series_reactance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/wire.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5553 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/line_locations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/sequence_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/overhead_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7386 2024-03-14 19:59:31.532490 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/vsc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/upfc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20073 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/hvdc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15880 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9392 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/winding.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21882 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/transformer_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11768 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/transformer3w.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/static_generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5947 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/external_grid.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5295 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/current_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/battery.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15440 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/generator_q_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6879 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/controllable_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6848 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2203 2024-04-01 07:29:23.256927 GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/graphic_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/map_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1078 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/map_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/schematic_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12374 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/base_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14140 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7381 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/injection_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24256 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/editable_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7765 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/generator_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17133 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/controllable_branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7068 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/load_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17273 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8531 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/shunt_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2829 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/generator_emission.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2898 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/generator_technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2741 2024-03-11 19:28:12.179075 GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/generator_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/load_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.4/GridCalEngine/DataStructures/bus_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-01 07:29:23.256927 GridCalEngine-5.1.4/GridCalEngine/DataStructures/branch_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_turbine_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_p2x_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    67032 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/DataStructures/numerical_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10107 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/generator_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_pump_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/battery_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_path_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.4/GridCalEngine/DataStructures/hvdc_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/DataStructures/shunt_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2347 2024-04-08 13:34:15.971164 GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_node_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_newton_pa.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_bentayga.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/Compilers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44207 2024-04-09 17:48:10.240457 GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_optimods.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_pgm.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11185 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/results_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Simulations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Simulations/results_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.4/GridCalEngine/Simulations/driver_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/driver_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/topology_processor_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/node_groups_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/reliability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1312 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11634 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/blackout_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8063 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10299 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.4/GridCalEngine/Simulations/InputsAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.4/GridCalEngine/Simulations/Dynamics/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7391 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29971 2024-04-08 13:34:15.975164 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13984 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1376 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29395 2024-03-28 10:16:48.984877 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8858 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8773 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2710 2024-03-11 19:28:12.207075 GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Simulations/StateEstimation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Simulations/StateEstimation/state_estimation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14766 2024-03-28 10:16:48.988877 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26711 2024-03-28 10:16:48.988877 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    78572 2024-04-08 13:34:15.975164 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/linear_opf_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4148 2024-03-11 19:28:12.215075 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44387 2024-04-09 17:48:10.244457 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54372 2024-04-08 13:34:15.975164 GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12868 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.4/GridCalEngine/Simulations/ATC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.4/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.4/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.4/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6692 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-03-17 12:13:24.384980 GridCalEngine-5.1.4/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-09 17:48:27.340457 GridCalEngine-5.1.4/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-09 17:48:27.340457 GridCalEngine-5.1.4/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11061 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/data_logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39202 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/enumerations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23740 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/basic_structures.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-04-08 13:34:15.975164 GridCalEngine-5.1.5/GridCalEngine/api.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/objects_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/timeseries_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9944 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/results_table_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/iwamoto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15007 2024-03-17 11:12:27.697061 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/ips.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/powell.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/autodiff.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc_numba.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/selected_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/ortools_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/pulp_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/highs.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Topology/topology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21322 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Topology/simulation_indices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10513 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Topology/topology_substation_reduction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4490 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Topology/detect_substations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.5/GridCalEngine/Topology/admittance_matrices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21419 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/base_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/units.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/base_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/base/base_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/dgs/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/dgs/dgs_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/raw/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/gridcal_to_raw.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/gne_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/switched_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/system_switching_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/facts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/owner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/inter_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/vsc_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/induction_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/fixed_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_storage_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_gen_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_bus_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_branch_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    53833 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/pack_unpack.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16095 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/zip_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    98239 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/json_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/generic_io_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/h5_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    47307 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/excel_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/sqlite_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/contingency_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/epc/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/epc/epc_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/IO/others/dpx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/others/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/others/ipa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/others/pypsa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/IO/others/plx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    50379 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15944 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2227 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29743 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/base.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12411 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_export.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26404 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    82071 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2416 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4230 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_devices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/base_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/psse_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/db_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2499 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/Devices/types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8637 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Devices/sparse_array.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/Devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   195588 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Devices/multi_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14901 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Devices/profile.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/municipality.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1813 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2579 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3864 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2641 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/emission_gas.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/country.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1332 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/modelling_authority.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2536 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2069 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1940 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1864 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investments_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3232 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/community.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/branch_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_path.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8074 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_turbine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_injection_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_p2x.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10753 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/underground_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10243 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/series_reactance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/wire.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5553 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line_locations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/sequence_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/overhead_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/vsc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/upfc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20073 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/hvdc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15880 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9392 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/winding.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20777 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11768 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer3w.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/static_generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5947 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/external_grid.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5295 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/current_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/battery.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15440 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator_q_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6879 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/controllable_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6848 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2203 2024-04-01 07:29:23.256927 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/graphic_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1078 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/schematic_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12374 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/base_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14140 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7381 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/injection_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23830 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/editable_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6781 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/generator_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17133 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/controllable_branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5952 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/load_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17273 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7415 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/shunt_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2339 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_emission.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2392 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2260 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/load_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.5/GridCalEngine/DataStructures/bus_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-11 15:31:05.578472 GridCalEngine-5.1.5/GridCalEngine/DataStructures/branch_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_turbine_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_p2x_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    67032 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/DataStructures/numerical_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10107 2024-04-11 15:31:05.578472 GridCalEngine-5.1.5/GridCalEngine/DataStructures/generator_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_pump_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/battery_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_path_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/DataStructures/hvdc_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/shunt_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2347 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_node_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_newton_pa.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_bentayga.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44207 2024-04-11 15:31:05.578472 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_optimods.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_pgm.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11185 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/results_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Simulations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Simulations/results_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_processor_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/node_groups_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1312 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11634 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/blackout_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8063 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10299 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.5/GridCalEngine/Simulations/InputsAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7391 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29971 2024-04-08 13:34:15.975164 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13984 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1376 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29395 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8858 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8773 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2710 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_estimation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14766 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26711 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    78572 2024-04-08 13:34:15.975164 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/linear_opf_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4258 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44173 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54464 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12868 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6692 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-03-17 12:13:24.384980 GridCalEngine-5.1.5/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-11 17:55:28.778307 GridCalEngine-5.1.5/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-11 17:55:28.778307 GridCalEngine-5.1.5/setup.cfg
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/__version__.py` & `GridCalEngine-5.1.5/GridCalEngine/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCalEngine_VERSION__ = "5.1.4"
+__GridCalEngine_VERSION__ = "5.1.5"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCalEngine_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/LICENSE.txt` & `GridCalEngine-5.1.5/GridCalEngine/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/data_logger.py` & `GridCalEngine-5.1.5/GridCalEngine/data_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -137,66 +137,66 @@
         :param device_class:
         :param device_property:
         :param value:
         :param expected_value:
         :param comment:
         :return:
         """
-        self.entries.append(DataLogEntry(msg=msg,
-                                         severity=DataLogSeverity.Warning,
-                                         device=device,
-                                         device_class=device_class,
-                                         property_name=device_property,
+        self.entries.append(DataLogEntry(msg=str(msg),
+                                         severity=DataLogSeverity.Information,
+                                         device=str(device),
+                                         device_class=str(device_class),
+                                         property_name=str(device_property),
                                          value=str(value),
                                          expected_value=str(expected_value),
-                                         comment=comment))
+                                         comment=str(comment)))
 
     def add_warning(self, msg, device="", device_class="", device_property='', value="", expected_value="",
                     comment=""):
         """
 
         :param msg:
         :param device:
         :param device_class:
         :param device_property:
         :param value:
         :param expected_value:
         :param comment:
         :return:
         """
-        self.entries.append(DataLogEntry(msg=msg,
+        self.entries.append(DataLogEntry(msg=str(msg),
                                          severity=DataLogSeverity.Warning,
-                                         device=device,
-                                         device_class=device_class,
-                                         property_name=device_property,
+                                         device=str(device),
+                                         device_class=str(device_class),
+                                         property_name=str(device_property),
                                          value=str(value),
                                          expected_value=str(expected_value),
-                                         comment=comment))
+                                         comment=str(comment)))
 
     def add_error(self, msg: str, device="", device_class="", device_property='', value="", expected_value="",
                   comment=""):
         """
 
         :param msg:
         :param device:
         :param device_class:
         :param device_property:
         :param value:
         :param expected_value:
         :param comment:
         :return:
         """
-        self.entries.append(DataLogEntry(msg=msg,
+        self.entries.append(DataLogEntry(msg=str(msg),
                                          severity=DataLogSeverity.Error,
-                                         device=device,
-                                         device_class=device_class,
-                                         property_name=device_property,
+                                         device=str(device),
+                                         device_class=str(device_class),
+                                         property_name=str(device_property),
                                          value=str(value),
                                          expected_value=str(expected_value),
-                                         comment=comment))
+                                         comment=str(comment)))
 
     def add_divergence(self, msg, device="", device_class="", device_property='', value=0, expected_value=0, tol=1e-6):
         """
 
         :param msg:
         :param device:
         :param device_class:
@@ -204,19 +204,19 @@
         :param value:
         :param expected_value:
         :param tol:
         :return:
         """
 
         if abs(value - expected_value) > tol:
-            self.entries.append(DataLogEntry(msg=msg,
+            self.entries.append(DataLogEntry(msg=str(msg),
                                              severity=DataLogSeverity.Divergence,
-                                             device=device,
-                                             device_class=device_class,
-                                             property_name=device_property,
+                                             device=str(device),
+                                             device_class=str(device_class),
+                                             property_name=str(device_property),
                                              value=str(value),
                                              expected_value=str(expected_value)))
 
     def add(self, msg, severity: DataLogSeverity = DataLogSeverity.Error, device="", device_class="",
             device_property='', value="", expected_value=""):
         """
 
@@ -225,19 +225,19 @@
         :param device:
         :param device_class:
         :param device_property:
         :param value:
         :param expected_value:
         :return:
         """
-        self.entries.append(DataLogEntry(msg=msg,
+        self.entries.append(DataLogEntry(msg=str(msg),
                                          severity=severity,
-                                         device=device,
-                                         device_class=device_class,
-                                         property_name=device_property,
+                                         device=str(device),
+                                         device_class=str(device_class),
+                                         property_name=str(device_property),
                                          value=str(value),
                                          expected_value=str(expected_value)))
 
     def to_dict(self):
         """
         Get the logs sorted by severity and message
         :return: Dictionary[Dictionary[List[time, device, value, expected value]]]
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/enumerations.py` & `GridCalEngine-5.1.5/GridCalEngine/enumerations.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,14 +557,50 @@
         """
 
         :return:
         """
         return list(map(lambda c: c.value, cls))
 
 
+
+class AcOpfMode(Enum):
+    """
+    AC-OPF problem types
+    """
+    ACOPFstd = 'ACOPFstd'
+    ACOPFslacks = 'ACOPFslacks'
+    ACOPFMaxInjections = 'ACOPFMaxInjections'
+
+    def __str__(self) -> str:
+        return str(self.value)
+
+    def __repr__(self):
+        return str(self)
+
+    @staticmethod
+    def argparse(s):
+        """
+
+        :param s:
+        :return:
+        """
+        try:
+            return AcOpfMode[s]
+        except KeyError:
+            return s
+
+    @classmethod
+    def list(cls):
+        """
+
+        :return:
+        """
+        return list(map(lambda c: c.value, cls))
+
+
 class TransformerControlType(Enum):
     """
     Transformer control types
     """
     fixed = '0:Fixed'
     Pf = '1:Pf'
     Qt = '2:Qt'
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/basic_structures.py` & `GridCalEngine-5.1.5/GridCalEngine/basic_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,23 +347,23 @@
         :param device_class:
         :param comment:
         :param device_property:
         :param object_value:
         :param expected_object_value:
         :return:
         """
-        self.entries.append(LogEntry(msg=msg,
+        self.entries.append(LogEntry(msg=str(msg),
                                      severity=LogSeverity.Information,
-                                     device=device,
+                                     device=str(device),
                                      value=str(value),
                                      expected_value=str(expected_value),
-                                     device_class=device_class,
-                                     device_property=device_property,
-                                     object_value=object_value,
-                                     expected_object_value=expected_object_value))
+                                     device_class=str(device_class),
+                                     device_property=str(device_property),
+                                     object_value=str(object_value),
+                                     expected_object_value=str(expected_object_value)))
 
     def add_warning(self, msg: str, device="", value="", expected_value="", device_class='', comment='',
                     device_property='', object_value=None, expected_object_value=None):
         """
         Add warning entry
         :param msg:
         :param device:
@@ -372,23 +372,23 @@
         :param device_class:
         :param comment:
         :param device_property:
         :param object_value:
         :param expected_object_value:
         :return:
         """
-        self.entries.append(LogEntry(msg=msg,
+        self.entries.append(LogEntry(msg=str(msg),
                                      severity=LogSeverity.Warning,
-                                     device=device,
+                                     device=str(device),
                                      value=str(value),
                                      expected_value=str(expected_value),
-                                     device_class=device_class,
-                                     device_property=device_property,
-                                     object_value=object_value,
-                                     expected_object_value=expected_object_value))
+                                     device_class=str(device_class),
+                                     device_property=str(device_property),
+                                     object_value=str(object_value),
+                                     expected_object_value=str(expected_object_value)))
 
     def add_error(self, msg: str, device="", value="", expected_value="", device_class='', comment='',
                   device_property='', object_value=None, expected_object_value=None):
         """
         Add error entry
         :param msg:
         :param device:
@@ -397,39 +397,39 @@
         :param device_class:
         :param comment:
         :param device_property:
         :param object_value:
         :param expected_object_value:
         :return:
         """
-        self.entries.append(LogEntry(msg=msg,
+        self.entries.append(LogEntry(msg=str(msg),
                                      severity=LogSeverity.Error,
-                                     device=device,
+                                     device=str(device),
                                      value=str(value),
                                      expected_value=str(expected_value),
-                                     device_class=device_class,
-                                     device_property=device_property,
-                                     object_value=object_value,
-                                     expected_object_value=expected_object_value))
+                                     device_class=str(device_class),
+                                     device_property=str(device_property),
+                                     object_value=str(object_value),
+                                     expected_object_value=str(expected_object_value)))
 
     def add_divergence(self, msg, device="", value=0, expected_value=0, tol=1e-6):
         """
         Add divergence entry
         :param msg:
         :param device:
         :param value:
         :param expected_value:
         :param tol:
         :return:
         """
 
         if abs(value - expected_value) > tol:
-            self.entries.append(LogEntry(msg=msg,
+            self.entries.append(LogEntry(msg=str(msg),
                                          severity=LogSeverity.Divergence,
-                                         device=device,
+                                         device=str(device),
                                          value=str(value),
                                          expected_value=str(expected_value),
                                          device_class="",
                                          device_property="",
                                          object_value=None,
                                          expected_object_value=None))
 
@@ -446,23 +446,23 @@
         :param comment:
         :param device_property:
         :param object_value:
         :param expected_object_value:
         :return:
         """
         # self.entries.append(LogEntry(msg, severity, device, str(value), str(expected_value)))
-        self.entries.append(LogEntry(msg=msg,
+        self.entries.append(LogEntry(msg=str(msg),
                                      severity=severity,
-                                     device=device,
+                                     device=str(device),
                                      value=str(value),
                                      expected_value=str(expected_value),
-                                     device_class=device_class,
-                                     device_property=device_property,
-                                     object_value=object_value,
-                                     expected_object_value=expected_object_value))
+                                     device_class=str(device_class),
+                                     device_property=str(device_property),
+                                     object_value=str(object_value),
+                                     expected_object_value=str(expected_object_value)))
 
     def to_dict(self) -> Union[Dict[str, Dict[str, List[Tuple[str, str, str, str]]]], Dict[str, Dict[str, List[List[str]]]]]:
         """
         Get the logs sorted by severity and message
         :return: Dictionary[Dictionary[List[time, device, value, expected value]]]
         """
         by_severity = dict()
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/api.py` & `GridCalEngine-5.1.5/GridCalEngine/api.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/objects_filtering.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/objects_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/timeseries_filtering.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/timeseries_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/filtering.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/filtering.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,27 +14,35 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from typing import List, Union
 from enum import Enum
 import re
 import numpy as np
-from GridCalEngine.Simulations.results_table import ResultsTable
-from GridCalEngine.basic_structures import BoolVec, Mat
 
 
 def is_odd(number: int):
     """
     Check if number is odd
     :param number:
     :return:
     """
     return number % 2 != 0
 
 
+def is_numeric(obj: np.ndarray) -> bool:
+    """
+    Checks if the numpy array is numeric
+    :param obj:
+    :return:
+    """
+    attrs = ['__add__', '__sub__', '__mul__', '__truediv__', '__pow__']
+    return all(hasattr(obj, attr) for attr in attrs)
+
+
 class CompOps(Enum):
     """
     Enumeration of filter oprations
     """
     GT = ">"
     LT = "<"
     GEQ = ">="
@@ -84,21 +92,30 @@
         return str(self.value)
 
     def __repr__(self):
         return str(self)
 
     @staticmethod
     def argparse(s):
+        """
+
+        :param s:
+        :return:
+        """
         try:
             return FilterOps[s]
         except KeyError:
             return s
 
     @classmethod
     def list(cls):
+        """
+
+        :return:
+        """
         return list(map(lambda c: c.value, cls))
 
 
 class FilterSubject(Enum):
     """
     Enumeration of filter oprations
     """
@@ -112,21 +129,30 @@
         return str(self.value)
 
     def __repr__(self):
         return str(self)
 
     @staticmethod
     def argparse(s):
+        """
+
+        :param s:
+        :return:
+        """
         try:
             return FilterSubject[s]
         except KeyError:
             return s
 
     @classmethod
     def list(cls):
+        """
+
+        :return:
+        """
         return list(map(lambda c: c.value, cls))
 
 
 PRIMARY_TYPES = Union[float, bool, int, str]
 
 
 class Filter:
@@ -306,28 +332,27 @@
     MasterFilter
     """
 
     def __init__(self) -> None:
         """
 
         """
-        self.stack: List[Union[Filter, FilterOps]] = []
+        self.stack: List[Union[Filter, FilterOps]] = list()
 
     def add(self, elm: Union[Filter, FilterOps]) -> None:
         """
-
-        :param elm:
-        :return:
+        Add filter or filter operation to the stack
+        :param elm: filter or filter operation
         """
         self.stack.append(elm)
 
-    def size(self):
+    def size(self) -> int:
         """
-
-        :return:
+        Get size of the stack
+        :return: int
         """
         return len(self.stack)
 
     def correct_size(self) -> bool:
         """
         Returs if the stack has the right size: an odd number
         :return:
@@ -366,15 +391,15 @@
 def parse_expression(expression: str) -> MasterFilter:
     """
     Parses the query expression
     :param expression:
     :return: MasterFilter
     """
     mst_flt = MasterFilter()
-    master_tokens = re.split(r'(and|or)', expression)
+    master_tokens = re.split(r'(?<=\s)(and|or)(?=\s)', expression)
 
     for token in master_tokens:
 
         if "and" not in token and "or" not in token:
 
             flt = parse_single(token=token)
 
@@ -382,17 +407,7 @@
                 mst_flt.add(elm=flt)
 
         else:
             elm = FilterOps(token.strip())
             mst_flt.add(elm=elm)
 
     return mst_flt
-
-
-def is_numeric(obj):
-    """
-    Checks if the numpy array is numeric
-    :param obj:
-    :return:
-    """
-    attrs = ['__add__', '__sub__', '__mul__', '__truediv__', '__pow__']
-    return all(hasattr(obj, attr) for attr in attrs)
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Filtering/results_table_filtering.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/results_table_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/common.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/common.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/ips.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/ips.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/powell.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/powell.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/autodiff.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/autodiff.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/NumericalMethods/sparse_solve.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/sparse_solve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/csc_numba.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc_numba.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/csc.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/Sparse/utils.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/utils.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/selected_interface.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/selected_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/ortools_interface.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/ortools_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/pulp_interface.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/pulp_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Utils/MIP/SimpleMip/highs.py` & `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/highs.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Topology/topology.py` & `GridCalEngine-5.1.5/GridCalEngine/Topology/topology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Topology/simulation_indices.py` & `GridCalEngine-5.1.5/GridCalEngine/Topology/simulation_indices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Topology/topology_substation_reduction.py` & `GridCalEngine-5.1.5/GridCalEngine/Topology/topology_substation_reduction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,32 @@
-from GridCalEngine.api import *
+# GridCal
+# Copyright (C) 2015 - 2024 Santiago Peñate Vera
+#
+# This program is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3 of the License, or (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with this program; if not, write to the Free Software Foundation,
+# Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+
+from typing import List, Union
+import numpy as np
 import GridCalEngine.Devices as dev
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCalEngine.Topology.topology import find_islands, get_adjacency_matrix
 from GridCalEngine.Devices.types import BRANCH_TYPES
+from GridCalEngine.basic_structures import IntVec, Logger
+from GridCalEngine.enumerations import DeviceType
 from scipy.sparse import lil_matrix
 
 
 class TopologyProcessorInfo:
     """
     CandidatesInfo
     """
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Topology/admittance_matrices.py` & `GridCalEngine-5.1.5/GridCalEngine/Topology/admittance_matrices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/file_handler.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/file_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 import os
 import json
 
 from collections.abc import Callable
 from typing import Union, List, Any, Dict
 
-from GridCalEngine.IO.cim.cgmes.gridcal_to_cgmes import gridcal_to_cgmes
+from GridCalEngine.IO.cim.cgmes.gridcal_to_cgmes import gridcal_to_cgmes, create_cgmes_headers
 from GridCalEngine.IO.cim.cgmes.cgmes_export import CimExporter
 from GridCalEngine.Simulations.driver_template import DriverTemplate
 from GridCalEngine.IO.cim.cgmes.cgmes_data_parser import CgmesDataParser
 from GridCalEngine.basic_structures import Logger
 from GridCalEngine.data_logger import DataLogger
 
 from GridCalEngine.IO.gridcal.json_parser import save_json_file_v3
@@ -122,24 +122,20 @@
         if isinstance(self.file_name, list):
 
             for f in self.file_name:
                 _, file_extension = os.path.splitext(f)
                 if file_extension.lower() not in ['.xml', '.zip']:
                     raise Exception('Loading multiple files that are not XML/Zip (xml or zip is for CIM or CGMES)')
             import time
-            start = time.time()
             data_parser = CgmesDataParser(text_func=text_func, progress_func=progress_func, logger=self.cgmes_logger)
             data_parser.load_files(files=self.file_name)
             self.cgmes_circuit = CgmesCircuit(cgmes_version=data_parser.cgmes_version, text_func=text_func,
                                               progress_func=progress_func, logger=self.cgmes_logger)
             self.cgmes_circuit.parse_files(data_parser=data_parser)
-            endt = time.time()
-            print("CGMES model load time: ", endt - start, "sec")
             self.circuit = cgmes_to_gridcal(cgmes_model=self.cgmes_circuit, logger=self.cgmes_logger)
-
         else:
 
             if os.path.exists(self.file_name):
                 name, file_extension = os.path.splitext(self.file_name)
                 # print(name, file_extension)
                 if file_extension.lower() in ['.xls', '.xlsx']:
 
@@ -349,15 +345,15 @@
         elif self.file_name.endswith('.sqlite'):
             logger = self.save_sqlite()
 
         elif self.file_name.endswith('.ejson3'):
             logger = self.save_json_v3()
 
         elif self.file_name.endswith('.xml'):
-            logger = self.save_cim()
+            logger = self.save_cgmes()
 
         elif self.file_name.endswith('.gch5'):
             logger = self.save_h5()
 
         elif self.file_name.endswith('.rawx'):
             logger = self.save_rawx()
 
@@ -435,30 +431,31 @@
         """
 
         logger = save_json_file_v3(self.file_name,
                                    self.circuit,
                                    self.options.simulation_drivers)
         return logger
 
-    def save_cim(self):
+    def save_cgmes(self):
         """
         Save the circuit information in CIM format
         :return: logger with information
         """
         logger = Logger()
         # CGMES version should be given in the settings
-        cgmes_circuit = CgmesCircuit(cgmes_version="", text_func=self.text_func,
+        cgmes_circuit = CgmesCircuit(cgmes_version="2.4.15", text_func=self.text_func,
                                      progress_func=self.progress_func, logger=logger)
         if self.options.cgmes_boundary_set != "":
             data_parser = CgmesDataParser(text_func=self.text_func, progress_func=self.progress_func,
                                           logger=logger)
             data_parser.load_files(files=[self.options.cgmes_boundary_set])
             cgmes_circuit.parse_files(data_parser=data_parser)
 
         cgmes_circuit = gridcal_to_cgmes(self.circuit, cgmes_circuit, logger)
+        cgmes_circuit = create_cgmes_headers(cgmes_circuit, version="1")
         cim_exporter = CimExporter(cgmes_circuit=cgmes_circuit)
         cim_exporter.export(self.file_name)
 
         return logger
 
     def save_h5(self):
         """
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/base/units.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/base/units.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/base/base_property.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/base/base_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/dgs/dgs_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/dgs/dgs_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_parser_legacy.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_functions.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/rawx_parser_writer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_parser_writer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/raw_to_gridcal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_to_gridcal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/rawx_parser_legacy.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/gne_device.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/gne_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/switched_shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/switched_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/system_switching_device.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/system_switching_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/psse_object.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/transformer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/facts.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/facts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/owner.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/owner.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/inter_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/inter_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/psse_property.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/generator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/psse_circuit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/bus.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/vsc_dc_line.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/vsc_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/induction_machine.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/induction_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/fixed_shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/fixed_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/load.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/zone.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/zone.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/branch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/raw/devices/substation.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_storage_definitions.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_storage_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_gen_definitions.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_gen_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_bus_definitions.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_bus_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/matpower/matpower_branch_definitions.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_branch_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/pack_unpack.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/pack_unpack.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,99 +35,99 @@
     :return: Dictionary instance
     """
 
     # this list must be sorted in dependency order so that the
     # loading algorithm is able to find the object substitutions
 
     object_types = {
-                    'modelling_authority': dev.ModellingAuthority(),
+        'modelling_authority': dev.ModellingAuthority(),
 
-                    'area': dev.Area(),
-                    'zone': dev.Zone(),
+        'area': dev.Area(),
+        'zone': dev.Zone(),
 
-                    'substation': dev.Substation(),
+        'substation': dev.Substation(),
 
-                    'voltage_level': dev.VoltageLevel(),
+        'voltage_level': dev.VoltageLevel(),
 
-                    'country': dev.Country(),
-                    'community': dev.Community(),
-                    'region': dev.Region(),
-                    'municipality': dev.Municipality(),
+        'country': dev.Country(),
+        'community': dev.Community(),
+        'region': dev.Region(),
+        'municipality': dev.Municipality(),
 
-                    'technology': dev.Technology(),
+        'technology': dev.Technology(),
 
-                    'fuel': dev.Fuel(),
+        'fuel': dev.Fuel(),
 
-                    'emission': dev.EmissionGas(),
+        'emission': dev.EmissionGas(),
 
-                    'bus': dev.Bus(),
+        'bus': dev.Bus(),
 
-                    'bus_bar': dev.BusBar(),
+        'bus_bar': dev.BusBar(),
 
-                    'connectivity node': dev.ConnectivityNode(),
+        'connectivity node': dev.ConnectivityNode(),
 
-                    'load': dev.Load(),
+        'load': dev.Load(),
 
-                    'static_generator': dev.StaticGenerator(),
+        'static_generator': dev.StaticGenerator(),
 
-                    'battery': dev.Battery(),
+        'battery': dev.Battery(),
 
-                    'generator': dev.Generator(),
+        'generator': dev.Generator(),
 
-                    'shunt': dev.Shunt(),
+        'shunt': dev.Shunt(),
 
-                    'linear_shunt': dev.ControllableShunt(),
+        'linear_shunt': dev.ControllableShunt(),
 
-                    'external_grid': dev.ExternalGrid(),
+        'external_grid': dev.ExternalGrid(),
 
-                    'current_injection': dev.CurrentInjection(),
+        'current_injection': dev.CurrentInjection(),
 
-                    'wires': dev.Wire(),
-                    'overhead_line_types': dev.OverheadLineType(),
-                    'underground_cable_types': dev.UndergroundLineType(),
-                    'sequence_line_types': dev.SequenceLineType(),
-                    'transformer_types': dev.TransformerType(),
+        'wires': dev.Wire(),
+        'overhead_line_types': dev.OverheadLineType(),
+        'underground_cable_types': dev.UndergroundLineType(),
+        'sequence_line_types': dev.SequenceLineType(),
+        'transformer_types': dev.TransformerType(),
 
-                    'branch_group': dev.BranchGroup(),
+        'branch_group': dev.BranchGroup(),
 
-                    'branch': dev.Branch(),
-                    'transformer2w': dev.Transformer2W(),
+        'branch': dev.Branch(),
+        'transformer2w': dev.Transformer2W(),
 
-                    'windings': dev.Winding(),
-                    'transformer3w': dev.Transformer3W(),
+        'windings': dev.Winding(),
+        'transformer3w': dev.Transformer3W(),
 
-                    'line': dev.Line(),
-                    'dc_line': dev.DcLine(None, None),
+        'line': dev.Line(),
+        'dc_line': dev.DcLine(None, None),
 
-                    'hvdc': dev.HvdcLine(),
+        'hvdc': dev.HvdcLine(),
 
-                    'vsc': dev.VSC(None, None),
-                    'upfc': dev.UPFC(None, None),
+        'vsc': dev.VSC(None, None),
+        'upfc': dev.UPFC(None, None),
 
-                    'series_reactance': dev.SeriesReactance(),
+        'series_reactance': dev.SeriesReactance(),
 
-                    'switch': dev.Switch(),
+        'switch': dev.Switch(),
 
-                    'contingency_group': dev.ContingencyGroup(),
-                    'contingency': dev.Contingency(),
+        'contingency_group': dev.ContingencyGroup(),
+        'contingency': dev.Contingency(),
 
-                    'investments_group': dev.InvestmentsGroup(),
-                    'investment': dev.Investment(),
+        'investments_group': dev.InvestmentsGroup(),
+        'investment': dev.Investment(),
 
-                    'generator_technology': dev.GeneratorTechnology(),
-                    'generator_fuel': dev.GeneratorFuel(),
-                    'generator_emission': dev.GeneratorEmission(),
+        'generator_technology': dev.GeneratorTechnology(),
+        'generator_fuel': dev.GeneratorFuel(),
+        'generator_emission': dev.GeneratorEmission(),
 
-                    'fluid_node': dev.FluidNode(),
-                    'fluid_path': dev.FluidPath(),
-                    'fluid_turbine': dev.FluidTurbine(),
-                    'fluid_pump': dev.FluidPump(),
-                    'fluid_p2x': dev.FluidP2x(),
+        'fluid_node': dev.FluidNode(),
+        'fluid_path': dev.FluidPath(),
+        'fluid_turbine': dev.FluidTurbine(),
+        'fluid_pump': dev.FluidPump(),
+        'fluid_p2x': dev.FluidP2x(),
 
-                    }
+    }
     return object_types
 
 
 def gather_model_as_data_frames(circuit: MultiCircuit, legacy: bool = False) -> Dict[str, pd.DataFrame]:
     """
     Pack the circuit information into tables (DataFrames)
     :param circuit: MultiCircuit instance
@@ -372,15 +372,14 @@
             arr = data['dense_data']
         else:
             arr = [collection.get(i, default_value) for i in data['dense_data']]
         profile.set(np.array(arr))
     profile.set_initialized()
 
 
-
 def gridcal_object_to_json(elm: ALL_DEV_TYPES) -> Dict[str, str]:
     """
 
     :param elm:
     :return:
     """
 
@@ -448,15 +447,16 @@
                 object_json.append(obj_data)
 
         data[object_type_name] = object_json
 
     # time
     unix_time = circuit.get_unix_time()
     data['time'] = {'unix': unix_time.tolist(),
-                    'prob': list(np.ones(len(unix_time)))}
+                    'prob': list(np.ones(len(unix_time))),
+                    'snapshot_unix': circuit.get_snapshot_time_unix()}
 
     return data
 
 
 def search_property(template_elm: ALL_DEV_TYPES,
                     old_props_dict: Dict[str, str],
                     property_to_search: str,
@@ -1240,14 +1240,19 @@
     if model_data is not None:
 
         if len(model_data) > 0:
 
             tdata = model_data.get('time', None)
             if tdata is not None:
                 circuit.set_unix_time(arr=tdata['unix'])
+
+                snapshot_unix_time = tdata.get('snapshot_unix', None)
+                if snapshot_unix_time is not None:
+                    circuit.set_snapshot_time_unix(val=snapshot_unix_time)
+
             else:
                 logger.add_error(msg=f'The file must have time data regardless of the profiles existance')
                 circuit.time_profile = None
 
             # for each element type...
             item_count = 0
             n_data_types = len(data_model_object_types)
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/zip_interface.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/zip_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/json_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/json_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/generic_io_functions.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/generic_io_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/h5_interface.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/h5_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/excel_interface.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/excel_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/sqlite_interface.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/sqlite_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/gridcal/contingency_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/contingency_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/epc/epc_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/epc/epc_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/others/dpx_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/others/dpx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/others/ipa_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/others/ipa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/others/pypsa_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/others/pypsa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/others/plx_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/others/plx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_enums.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,15 @@
                               voltage_level=volt_lev,  # TODO
                               country=None,  # TODO
                               # latitude=0.0,
                               # longitude=0.0,
                               Vm0=vm,
                               Va0=va)
 
+
         gc_model.add_bus(gcdev_elm)
         calc_node_dict[gcdev_elm.idtag] = gcdev_elm
 
     return calc_node_dict
 
 
 def get_gcdev_connectivity_nodes(cgmes_model: CgmesCircuit,
@@ -804,15 +805,15 @@
     :param gcdev_model: gcdevCircuit
     :param calc_node_dict: Dict[str, gcdev.Bus]
     :param cn_dict: Dict[str, gcdev.ConnectivityNode]
     :param device_to_terminal_dict: Dict[str, Terminal]
     :param logger:
     """
     # convert shunts
-    for device_list in [cgmes_model.LinearShuntCompensator_list, cgmes_model.NonlinearShuntCompensator_list]:
+    for device_list in [cgmes_model.LinearShuntCompensator_list]:
 
         for cgmes_elm in device_list:
 
             calc_nodes, cns = find_connections(cgmes_elm=cgmes_elm,
                                                device_to_terminal_dict=device_to_terminal_dict,
                                                calc_node_dict=calc_node_dict,
                                                cn_dict=cn_dict,
@@ -822,46 +823,66 @@
                 calc_node = calc_nodes[0]
                 cn = cns[0]
 
                 # conversion
                 G, B, G0, B0 = get_values_shunt(shunt=cgmes_elm,
                                                 logger=logger,
                                                 Sbase=Sbase)
-                v_set, is_controlled = get_regulating_control(
-                    cgmes_elm=cgmes_elm,
-                    cgmes_enums=cgmes_enums,
-                    logger=logger)
 
                 gcdev_elm = gcdev.Shunt(
                     idtag=cgmes_elm.uuid,
                     name=cgmes_elm.name,
                     code=cgmes_elm.description,
                     G=G * cgmes_elm.sections,
                     B=B * cgmes_elm.sections,
                     G0=G0 * cgmes_elm.sections,
                     B0=B0 * cgmes_elm.sections,
                     # Bmax=B * cgmes_elm.maximumSections,
                     # Bmin=B,
-                    active=True,  # TODO what is this?
-                    # controlled=is_controlled,
-                    # vset=v_set,
-                    # bus=calc_node,  # ?
-                    # cn=cn,  # ?
+                    active=True,
                 )
                 gcdev_model.add_shunt(calc_node, gcdev_elm)
 
             else:
                 logger.add_error(msg='Not exactly one terminal',
                                  device=cgmes_elm.rdfid,
                                  device_class=cgmes_elm.tpe,
                                  device_property="number of associated terminals",
                                  value=len(calc_nodes),
                                  expected_value=1)
 
 
+def get_gcdev_controllable_shunts(
+        cgmes_model: CgmesCircuit,
+        gcdev_model: MultiCircuit,
+        calc_node_dict: Dict[str, gcdev.Bus],
+        cn_dict: Dict[str, gcdev.ConnectivityNode],
+        device_to_terminal_dict: Dict[str, List[Terminal]],
+        logger: DataLogger,
+        Sbase: float) -> None:
+    """
+    Convert the CGMES non-linear shunt compensators to gcdev Controllable shunts.
+
+    :param cgmes_model: CgmesCircuit
+    :param gcdev_model: gcdevCircuit
+    :param calc_node_dict: Dict[str, gcdev.Bus]
+    :param cn_dict: Dict[str, gcdev.ConnectivityNode]
+    :param device_to_terminal_dict: Dict[str, Terminal]
+    :param logger:
+    """
+    # comes later
+    for device_list in [cgmes_model.NonlinearShuntCompensator_list]:
+        # ...
+        # v_set, is_controlled = get_regulating_control(
+        #     cgmes_elm=cgmes_elm,
+        #     cgmes_enums=cgmes_enums,
+        #     logger=logger)
+        pass
+
+
 def get_gcdev_switches(cgmes_model: CgmesCircuit,
                        gcdev_model: MultiCircuit,
                        calc_node_dict: Dict[str, gcdev.Bus],
                        cn_dict: Dict[str, gcdev.ConnectivityNode],
                        device_to_terminal_dict: Dict[str, List[Terminal]],
                        logger: DataLogger,
                        Sbase: float) -> None:
@@ -1092,25 +1113,26 @@
     get_gcdev_external_grids(cgmes_model, gc_model, calc_node_dict, cn_dict, device_to_terminal_dict, logger)
     get_gcdev_generators(cgmes_model, gc_model, calc_node_dict, cn_dict, device_to_terminal_dict, logger)
 
     get_gcdev_ac_lines(cgmes_model, gc_model, calc_node_dict, cn_dict, device_to_terminal_dict, logger, Sbase)
     get_gcdev_ac_transformers(cgmes_model, gc_model, calc_node_dict, cn_dict, device_to_terminal_dict, logger, Sbase)
 
     get_gcdev_shunts(cgmes_model, gc_model, calc_node_dict, cn_dict, device_to_terminal_dict, logger, Sbase)
+    # get_gcdev_controllable_shunts()  TODO controllable shunts
     get_gcdev_switches(cgmes_model, gc_model, calc_node_dict, cn_dict, device_to_terminal_dict, logger, Sbase)
 
     print('debug')
 
-    # Gridcal to cgmes
-    cgmes_circuit = CgmesCircuit()
-    cgmes_model_export = gridcal_to_cgmes(gc_model, cgmes_circuit, logger)
+    # # Gridcal to cgmes
+    # cgmes_model_export = CgmesCircuit()
+    # cgmes_model_export = gridcal_to_cgmes(gc_model, cgmes_model_export, logger)
 
     # Export test for the imported data
-    start = time.time()
-    serializer = CimExporter(cgmes_model)
-    serializer.export_test()
-    end = time.time()
-    print("ET export time: ", end - start, "sec")
+    # start = time.time()
+    # serializer = CimExporter(cgmes_model)
+    # serializer.export_test()
+    # end = time.time()
+    # print("ET export time: ", end - start, "sec")
 
     # Export data converted from gridcal
 
     return gc_model
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_writer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 import zipfile
 from typing import List, Union, Callable
-from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15 import cgmesProfile
-from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15 import CgmesCircuit
+from GridCalEngine.IO.cim.cgmes.cgmes_enums import cgmesProfile
+from GridCalEngine.IO.cim.cgmes.cgmes_circuit import CgmesCircuit
 
 
 def write_cgmes(filename_zip: str, model: CgmesCircuit, profiles: List[cgmesProfile],
                 text_func: Union[Callable, None] = None,
                 progress_func: Union[Callable, None] = None):
     """
     Write a CGMES model to a zip file
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from GridCalEngine.Devices import MultiCircuit
 from GridCalEngine.Devices.Substation.bus import Bus
 from GridCalEngine.IO.cim.cgmes.base import get_new_rdfid, form_rdfid
 from GridCalEngine.IO.cim.cgmes.cgmes_circuit import CgmesCircuit
+from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.full_model import FullModel
+from GridCalEngine.IO.cim.cgmes.base import Base
 import GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices as cgmes
 import GridCalEngine.Devices as gcdev
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices import GeneratingUnit, \
     ThermalGeneratingUnit, HydroGeneratingUnit, SolarGeneratingUnit, \
     WindGeneratingUnit, NuclearGeneratingUnit
 
 # if cgmes_version == '2.4.15.':
@@ -13,14 +15,29 @@
 #         Terminal
 
 from GridCalEngine.data_logger import DataLogger
 from typing import Dict, List, Tuple, Union
 
 
 # region UTILS
+
+class ReferenceManager:
+    # use it after an element object added
+    def __init__(self):
+        self.data = dict()
+
+    def add(self, cgmes_obj: Base):
+
+        tpe_dict = self.data.get(cgmes_obj.tpe, None)
+        if tpe_dict is None:
+            self.data[cgmes_obj.tpe] = {cgmes_obj.rdfid: cgmes_obj}
+        else:
+            tpe_dict[cgmes_obj.rdfid] = cgmes_obj
+
+
 # def find_terms_connections():
 #     pass   # TODO
 
 
 def find_object_by_uuid(object_list, target_uuid):  # TODO move to CGMES utils
     """
     Finds an object with the specified uuid
@@ -91,14 +108,91 @@
     return R, X, G, B, R0, X0, G0, B0
 
 
 # endregion
 
 # region create new classes for CC
 
+def create_cgmes_headers(cgmes_model: CgmesCircuit, desc: str = "", scenariotime: str = "",
+                         modelingauthorityset: str = "", version: str = ""):
+    from datetime import datetime
+
+    fm_list = [FullModel(rdfid=get_new_rdfid(), tpe="FullModel"), FullModel(rdfid=get_new_rdfid(), tpe="FullModel"),
+               FullModel(rdfid=get_new_rdfid(), tpe="FullModel"), FullModel(rdfid=get_new_rdfid(), tpe="FullModel")]
+    for fm in fm_list:
+        fm.scenarioTime = scenariotime
+        if modelingauthorityset != "":
+            fm.modelingAuthoritySet = modelingauthorityset
+        current_time = datetime.utcnow()
+        formatted_time = current_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+        fm.created = formatted_time
+        fm.version = version
+        fm.description = desc
+
+    if cgmes_model.cgmes_version == "2.4.15":
+        profile_uris = {
+            "EQ": ["http://entsoe.eu/CIM/EquipmentCore/3/1",
+                   "http://entsoe.eu/CIM/EquipmentShortCircuit/3/1",
+                   "http://entsoe.eu/CIM/EquipmentOperation/3/1"],
+            "SSH": ["http://entsoe.eu/CIM/SteadyStateHypothesis/1/1"],
+            "TP": ["http://entsoe.eu/CIM/Topology/4/1"],
+            "SV": ["http://entsoe.eu/CIM/StateVariables/4/1"]
+        }
+    elif cgmes_model.cgmes_version == "3.0.0":
+        profile_uris = {
+            "EQ": ["http://iec.ch/TC57/ns/CIM/CoreEquipment-EU/3.0",
+                   "http://iec.ch/TC57/ns/CIM/Operation-EU/3.0",
+                   "http://iec.ch/TC57/ns/CIM/ShortCircuit-EU/3.0"],
+            "SSH": ["http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU/3.0"],
+            "TP": ["http://iec.ch/TC57/ns/CIM/Topology-EU/3.0"],
+            "SV": ["http://iec.ch/TC57/ns/CIM/StateVariables-EU/3.0"]
+        }
+    else:
+        return
+
+    # EQ profiles
+    prof = profile_uris.get("EQ")
+    fm_list[0].profile = [prof[0]]
+    if True:  # TODO How to decide if it contains Operation?
+        fm_list[0].profile.append(prof[1])
+    if True:  # TODO How to decide if it contains ShortCircuit?
+        fm_list[0].profile.append(prof[2])
+
+    fm_list[1].profile = profile_uris.get("SSH")
+    fm_list[2].profile = profile_uris.get("TP")
+    fm_list[3].profile = profile_uris.get("SV")
+
+    # DependentOn
+    eqbd_id = ""
+    tpbd_id = ""
+    try:
+        for bd in cgmes_model.elements_by_type_boundary.get("FullModel"):
+            if ("http://entsoe.eu/CIM/EquipmentBoundary/3/1" in bd.profile or
+                    "http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU" in bd.profile):
+                eqbd_id = bd.rdfid
+            if "http://entsoe.eu/CIM/TopologyBoundary/3/1" in bd.profile:  # no TPBD in 3.0
+                tpbd_id = bd.rdfid
+
+        fm_list[0].DependentOn = [eqbd_id]
+        fm_list[1].DependentOn = [fm_list[0].rdfid]
+        if tpbd_id != "":
+            fm_list[2].DependentOn = [eqbd_id, tpbd_id, fm_list[0].rdfid]
+            fm_list[3].DependentOn = [tpbd_id, fm_list[0].rdfid, fm_list[1].rdfid, fm_list[2].rdfid]
+        else:
+            fm_list[2].DependentOn = [eqbd_id, fm_list[0].rdfid]
+            fm_list[3].DependentOn = [fm_list[0].rdfid, fm_list[1].rdfid, fm_list[2].rdfid]
+    except TypeError:
+        print("Missing default boundary files")
+        fm_list[1].DependentOn = [fm_list[0].rdfid]
+        fm_list[2].DependentOn = [fm_list[0].rdfid]
+        fm_list[3].DependentOn = [fm_list[0].rdfid, fm_list[1].rdfid, fm_list[2].rdfid]
+
+    cgmes_model.FullModel_list = fm_list
+    return cgmes_model
+
 
 def create_cgmes_terminal(bus: Bus,
                           cgmes_model: CgmesCircuit,
                           logger: DataLogger) -> cgmes.Terminal:
     """ Creates a new Terminal in CGMES model,
     and connects it the relating Topologinal Node """
 
@@ -108,22 +202,23 @@
     # term.phases =
     # term.ConductingEquipment = BusBarSection
     term.connected = True
     tn = find_object_by_uuid(
         object_list=cgmes_model.TopologicalNode_list,
         target_uuid=bus.idtag
     )
+
     if isinstance(tn, cgmes.TopologicalNode):
         term.TopologicalNode = tn
     else:
         logger.add_error(msg='No found TopologinalNode',
                          device=bus,
                          device_class=gcdev.Bus)
 
-    cgmes_model.Terminal_list.append(term)
+    cgmes_model.add(term)
 
     return term
 
 
 def create_cgmes_load_response_char(
         load: gcdev.Load,
         logger: DataLogger) -> cgmes.LoadResponseCharacteristic:
@@ -153,40 +248,40 @@
     Creates the appropriate CGMES GeneratingUnit object
     from a MultiCircuit Generator.
     """
 
     new_rdf_id = get_new_rdfid()
     if gen.technology.name == 'General':
         sm = cgmes.GeneratingUnit(new_rdf_id)
-        cgmes_model.GeneratingUnit_list.append(sm)
+        cgmes_model.add(sm)
         return sm
 
     if gen.technology.name == 'Thermal':
         tgu = cgmes.ThermalGeneratingUnit(new_rdf_id)
-        cgmes_model.ThermalGeneratingUnit_list.append(tgu)
+        cgmes_model.add(tgu)
         return tgu
 
     if gen.technology.name == 'Hydro':
         hgu = cgmes.HydroGeneratingUnit(new_rdf_id)
-        cgmes_model.HydroGeneratingUnit_list.append(hgu)
+        cgmes_model.add(hgu)
         return hgu
 
     if gen.technology.name == 'Solar':
         sgu = cgmes.SolarGeneratingUnit(new_rdf_id)
-        cgmes_model.SolarGeneratingUnit_list.append(sgu)
+        cgmes_model.add(sgu)
         return sgu
 
     if gen.technology.name == 'Wind':
         wgu = cgmes.WindGeneratingUnit(new_rdf_id)
-        cgmes_model.WindGeneratingUnit_list.append(wgu)
+        cgmes_model.add(wgu)
         return wgu
 
     if gen.technology.name == 'Nuclear':
         ngu = cgmes.NuclearGeneratingUnit(new_rdf_id)
-        cgmes_model.NuclearGeneratingUnit_list.append(ngu)
+        cgmes_model.add(ngu)
         return ngu
 
     return None
 
 
 def create_cgmes_regulating_control(
         gen: gcdev.Generator,
@@ -195,24 +290,26 @@
 
     :param gen: MultiCircuit Generator
     :param cgmes_model: CgmesCircuit
     :return:
     """
     new_rdf_id = get_new_rdfid()
     rc = cgmes.RegulatingControl(rdfid=new_rdf_id)
+
     rc.name = f'_RC_{gen.name}'
+    rc.RegulatingCondEq = gen
     # rc.mode: RegulatingControlModeKind
     # rc.Terminal
     # rc.discrete
     # rc.enabled
     # rc.targetDeadband
     # rc.targetValue = gen.Vset
     # rc.targetValueUnitMultiplier = 'k'
 
-    cgmes_model.RegulatingControl_list.append(rc)
+    cgmes_model.add(rc)
 
     return rc
 
 
 # endregion
 
 # region Convert functions from MC to CC
@@ -240,30 +337,30 @@
             base_volt_set.add(bus.Vnom)
 
             new_rdf_id = get_new_rdfid()
             base_volt = cgmes.BaseVoltage(rdfid=new_rdf_id)
             base_volt.name = f'_BV_{int(bus.Vnom)}'
             base_volt.nominalVoltage = bus.Vnom
 
-            cgmes_model.BaseVoltage_list.append(base_volt)
+            cgmes_model.add(base_volt)
     return
 
 
 def get_cgmes_substations(multi_circuit_model: MultiCircuit,
                           cgmes_model: CgmesCircuit,
                           logger: DataLogger) -> None:
     for mc_elm in multi_circuit_model.substations:
         substation = cgmes.Substation(rdfid=form_rdfid(mc_elm.idtag))
         substation.name = mc_elm.name
         substation.Region = find_object_by_uuid(
             object_list=cgmes_model.SubGeographicalRegion_list,
             target_uuid=mc_elm.idtag  # TODO Community.idtag!
         )
 
-        cgmes_model.Substation_list.append(substation)
+        cgmes_model.add(substation)
 
 
 def get_cgmes_voltage_levels(multi_circuit_model: MultiCircuit,
                              cgmes_model: CgmesCircuit,
                              logger: DataLogger) -> None:
     for mc_elm in multi_circuit_model.voltage_levels:
 
@@ -285,15 +382,15 @@
                 vl.Substation = substation
 
                 # link back
                 if substation.VoltageLevels is None:
                     substation.VoltageLevels = list()
                 substation.VoltageLevels.append(vl)
 
-        cgmes_model.VoltageLevel_list.append(vl)
+        cgmes_model.add(vl)
 
 
 def get_cgmes_tn_nodes(multi_circuit_model: MultiCircuit,
                        cgmes_model: CgmesCircuit,
                        logger: DataLogger) -> None:
     for bus in multi_circuit_model.buses:
 
@@ -313,15 +410,15 @@
             # link back
             vl.TopologicalNode = tn
         else:
             print(f'Bus.voltage_level.idtag is None for {bus.name}')
         # TODO bus should have association for VoltageLevel first
         # and the voltagelevel to the substation
 
-        cgmes_model.TopologicalNode_list.append(tn)
+        cgmes_model.add(tn)
 
     return
 
 
 def get_cgmes_cn_nodes(multi_circuit_model: MultiCircuit,
                        cgmes_model: CgmesCircuit,
                        logger: DataLogger) -> None:
@@ -345,15 +442,15 @@
                                  device_class=cn.tpe)
         else:
             logger.add_error(msg='Connectivity Node has no default bus',
                              device=mc_elm,
                              device_class=gcdev.ConnectivityNode)
             # print(f'Topological node not found for cn: {cn.name}')
 
-        cgmes_model.ConnectivityNode_list.append(cn)
+        cgmes_model.add(cn)
 
     return
 
 
 def get_cgmes_svvoltages(v_dict: Dict[str, Tuple[float, float]],
                          cgmes_model: CgmesCircuit,
                          logger: DataLogger) -> CgmesCircuit:
@@ -373,15 +470,15 @@
         sv_voltage = cgmes.SvVoltage(
             rdfid=uuid, tpe='SvVoltage'
         )
         sv_voltage.v = v
         sv_voltage.angle = angle
 
         # Add the SvVoltage instance to the SvVoltage_list
-        cgmes_model.SvVoltage_list.append(sv_voltage)
+        cgmes_model.add(sv_voltage)
 
     return cgmes_model
 
 
 def get_cgmes_loads(multicircuit_model: MultiCircuit,
                     cgmes_model: CgmesCircuit,
                     logger: DataLogger):
@@ -412,15 +509,15 @@
         cl.LoadResponse = create_cgmes_load_response_char(load=mc_elm, logger=logger)
         # cl.LoadGroup = ConformLoadGroup ..?
         cl.p = mc_elm.P / cl.LoadResponse.pConstantPower
         cl.q = mc_elm.Q / cl.LoadResponse.qConstantPower
 
         cl.description = mc_elm.code
 
-        cgmes_model.ConformLoad_list.append(cl)
+        cgmes_model.add(cl)
 
 
 def get_cgmes_equivalent_injections(multicircuit_model: MultiCircuit,
                                     cgmes_model: CgmesCircuit,
                                     logger: DataLogger):
     """
     Converts every Multi Circuit external grid
@@ -437,15 +534,15 @@
         ei.description = mc_elm.code
         ei.name = mc_elm.name
         ei.p = mc_elm.P
         ei.q = mc_elm.Q
         ei.BaseVoltage = find_object_by_attribute(cgmes_model.BaseVoltage_list, "nominalVoltage",
                                                   mc_elm.bus.Vnom)
 
-        cgmes_model.EquivalentInjection_list.append(ei)
+        cgmes_model.add(ei)
 
 
 def get_cgmes_ac_line_segments(multicircuit_model: MultiCircuit,
                                cgmes_model: CgmesCircuit,
                                logger: DataLogger):
     """
     Converts every Multi Circuit line
@@ -478,15 +575,15 @@
             # line.gch = mc_elm.G * Ybase
             line.bch = mc_elm.B * ybase
             line.r0 = mc_elm.R0 * zbase
             line.x0 = mc_elm.X0 * zbase
             # line.g0ch = mc_elm.G0 * Ybase
             line.b0ch = mc_elm.B0 * ybase
 
-        cgmes_model.ACLineSegment_list.append(line)
+        cgmes_model.add(line)
 
 
 def get_cgmes_operational_limits(multicircuit_model: MultiCircuit,
                                  cgmes_model: CgmesCircuit,
                                  logger: DataLogger):
     # OperationalLimitSet and OperationalLimitType
 
@@ -544,15 +641,15 @@
         cgmes_syn.GeneratingUnit = cgmes_gen  # linking them together
         cgmes_gen.RotatingMachine = cgmes_syn  # linking them together
         cgmes_syn.maxQ = mc_elm.Qmax
         cgmes_syn.minQ = mc_elm.Qmin
         # ...
         cgmes_syn.referencePriority = '0'  # ?
 
-        cgmes_model.SynchronousMachine_list.append(cgmes_syn)
+        cgmes_model.add(cgmes_syn)
 
 
 def get_cgmes_power_transformers(multicircuit_model: MultiCircuit,
                                  cgmes_model: CgmesCircuit,
                                  logger: DataLogger):
     for mc_elm in multicircuit_model.transformers2w:
         cm_transformer = cgmes.PowerTransformer(rdfid=form_rdfid(mc_elm.idtag))
@@ -591,19 +688,19 @@
         pte2.g0 = 0
         pte2.b0 = 0
         pte2.ratedU = mc_elm.LV
         pte2.ratedS = mc_elm.Sn
         pte2.endNumber = 2
 
         cm_transformer.PowerTransformerEnd.append(pte1)
-        cgmes_model.PowerTransformerEnd_list.append(pte1)
+        cgmes_model.add(pte1)
         cm_transformer.PowerTransformerEnd.append(pte2)
-        cgmes_model.PowerTransformerEnd_list.append(pte2)
+        cgmes_model.add(pte2)
 
-        cgmes_model.PowerTransformer_list.append(cm_transformer)
+        cgmes_model.add(cm_transformer)
 
     for mc_elm in multicircuit_model.transformers3w:
         cm_transformer = cgmes.PowerTransformer(rdfid=form_rdfid(mc_elm.idtag))
         cm_transformer.uuid = mc_elm.idtag
         cm_transformer.description = mc_elm.code
         cm_transformer.name = mc_elm.name
         cm_transformer.Terminals = [create_cgmes_terminal(mc_elm.bus1, cgmes_model, logger),
@@ -612,17 +709,19 @@
         cm_transformer.PowerTransformerEnd = []
 
         pte1 = cgmes.PowerTransformerEnd()
         pte1.PowerTransformer = cm_transformer
         pte1.ratedU = mc_elm.V1
         pte1.ratedS = mc_elm.rate12
         pte1.endNumber = 1
-        R, X, G, B, R0, X0, G0, B0 = (mc_elm.winding1.R, mc_elm.winding1.X, mc_elm.winding1.G, mc_elm.winding1.B, mc_elm.winding1.R0,
-                                      mc_elm.winding1.X0, mc_elm.winding1.G0, mc_elm.winding1.B0)
-        r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.winding1.rate, mc_elm.winding1.HV)
+        R, X, G, B, R0, X0, G0, B0 = (
+            mc_elm.winding1.R, mc_elm.winding1.X, mc_elm.winding1.G, mc_elm.winding1.B, mc_elm.winding1.R0,
+            mc_elm.winding1.X0, mc_elm.winding1.G0, mc_elm.winding1.B0)
+        r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.winding1.rate,
+                                                                      mc_elm.winding1.HV)
         pte1.r = r
         pte1.x = x
         pte1.g = g
         pte1.b = b
         pte1.r0 = r0
         pte1.x0 = x0
         pte1.g0 = g0
@@ -630,16 +729,16 @@
 
         pte2 = cgmes.PowerTransformerEnd()
         pte2.PowerTransformer = cm_transformer
         pte2.ratedU = mc_elm.V2
         pte2.ratedS = mc_elm.rate23
         pte2.endNumber = 2
         R, X, G, B, R0, X0, G0, B0 = (
-        mc_elm.winding2.R, mc_elm.winding2.X, mc_elm.winding2.G, mc_elm.winding2.B, mc_elm.winding2.R0,
-        mc_elm.winding2.X0, mc_elm.winding2.G0, mc_elm.winding2.B0)
+            mc_elm.winding2.R, mc_elm.winding2.X, mc_elm.winding2.G, mc_elm.winding2.B, mc_elm.winding2.R0,
+            mc_elm.winding2.X0, mc_elm.winding2.G0, mc_elm.winding2.B0)
         r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.winding2.rate,
                                                                       mc_elm.winding2.HV)
         pte2.r = r
         pte2.x = x
         pte2.g = g
         pte2.b = b
         pte2.r0 = r0
@@ -649,35 +748,67 @@
 
         pte3 = cgmes.PowerTransformerEnd()
         pte3.PowerTransformer = cm_transformer
         pte3.ratedU = mc_elm.V3
         pte3.ratedS = mc_elm.rate31
         pte3.endNumber = 3
         R, X, G, B, R0, X0, G0, B0 = (
-        mc_elm.winding3.R, mc_elm.winding3.X, mc_elm.winding3.G, mc_elm.winding3.B, mc_elm.winding3.R0,
-        mc_elm.winding3.X0, mc_elm.winding3.G0, mc_elm.winding3.B0)
+            mc_elm.winding3.R, mc_elm.winding3.X, mc_elm.winding3.G, mc_elm.winding3.B, mc_elm.winding3.R0,
+            mc_elm.winding3.X0, mc_elm.winding3.G0, mc_elm.winding3.B0)
         r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.winding3.rate,
                                                                       mc_elm.winding3.HV)
         pte3.r = r
         pte3.x = x
         pte3.g = g
         pte3.b = b
         pte3.r0 = r0
         pte3.x0 = x0
         pte3.g0 = g0
         pte3.b0 = b0
 
         cm_transformer.PowerTransformerEnd.append(pte1)
-        cgmes_model.PowerTransformerEnd_list.append(pte1)
+        cgmes_model.add(pte1)
         cm_transformer.PowerTransformerEnd.append(pte2)
-        cgmes_model.PowerTransformerEnd_list.append(pte2)
+        cgmes_model.add(pte2)
         cm_transformer.PowerTransformerEnd.append(pte3)
-        cgmes_model.PowerTransformerEnd_list.append(pte3)
+        cgmes_model.add(pte3)
 
-        cgmes_model.PowerTransformer_list.append(cm_transformer)
+        cgmes_model.add(cm_transformer)
+
+
+def get_cgmes_linear_shunts(multicircuit_model: MultiCircuit,
+                            cgmes_model: CgmesCircuit,
+                            logger: DataLogger):
+    """
+    Converts Multi Circuit shunts
+    into CGMES Linear shunt compensator
+
+    :param multicircuit_model:
+    :param cgmes_model:
+    :param logger:
+    :return:
+    """
+
+    for mc_elm in multicircuit_model.shunts:
+        lsc = cgmes.LinearShuntCompensator(rdfid=form_rdfid(mc_elm.idtag))
+        lsc.name = mc_elm.name
+        lsc.description = mc_elm.code
+        # lsc.EquipmentContainer: VoltageLevel .. like at tn_nodes line 284
+        lsc.RegulatingControl = False
+        lsc.controlEnabled = False
+        lsc.maximumSections = 1
+        # lsc.nomU = lsc.EquipmentContainer.BaseVoltage.nominalVoltage
+        # lsc.bPerSection = mc_elm.B / (lsc.nomU ** 2)
+        # lsc.gPerSection = mc_elm.G / (lsc.nomU ** 2)
+        # lsc.sections = ?
+        # lsc.normalSections = ?
+
+        lsc.Terminals = create_cgmes_terminal(mc_elm.bus, cgmes_model, logger)
+
+        cgmes_model.LinearShuntCompensator_list.append(lsc)
 
 
 # endregion
 
 
 def gridcal_to_cgmes(gc_model: MultiCircuit, cgmes_model: CgmesCircuit, logger: DataLogger) -> CgmesCircuit:
     """
@@ -703,10 +834,12 @@
     get_cgmes_loads(gc_model, cgmes_model, logger)
     get_cgmes_equivalent_injections(gc_model, cgmes_model, logger)
     get_cgmes_generators(gc_model, cgmes_model, logger)
 
     get_cgmes_ac_line_segments(gc_model, cgmes_model, logger)
     # transformers, windings
     get_cgmes_power_transformers(gc_model, cgmes_model, logger)
+
     # shunts
+    get_cgmes_linear_shunts(gc_model, cgmes_model, logger)
 
     return cgmes_model
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/base.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/base.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_export.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_export.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_utils.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,20 +286,24 @@
                 return get_voltage_terminal(tp, logger=logger)
             else:
                 return None
         else:
             return None
 
 
-def get_values_shunt(shunt: LinearShuntCompensator, logger: DataLogger, Sbase: float = 100.0):
+def get_values_shunt(shunt: LinearShuntCompensator,
+                     logger: DataLogger,
+                     Sbase: float = 100.0):
     """
     Get the per-unit values of the Shunt (per Section)
 
+    :param shunt: CGMES Linear shunt compensator
+    :param logger: Datalogger
     :param Sbase: Sbase in MVA
-    :return: G, B
+    :return: G, B, G0, B0
     """
     if shunt.BaseVoltage is not None:
         Vnom = get_voltage_shunt(shunt, logger=logger)
 
         if Vnom is not None:
 
             # Zbase = (Vnom * Vnom) / Sbase
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
             # check the declared properties
             for property_name, cim_prop in element.declared_properties.items():
 
                 # try to get the property value, else, fill with None
                 # at this point val is always the string that came in the XML
                 value = getattr(element, property_name)
                 if value is not None and isinstance(value, IdentifiedObject):
-                    value = value.rdfid
+                    continue
 
                 if value is not None:  # if the value is something...
 
                     if cim_prop.class_type in [str, float, int, bool]:
                         # set the referenced object in the property
                         try:
                             if isinstance(value, list):
@@ -325,15 +325,15 @@
                                                      device_property=property_name,
                                                      value='Not found',
                                                      expected_value=value)
                         else:
                             referenced_object_list = set()
                             for v in value:
                                 if isinstance(v, IdentifiedObject):
-                                    v = v.rdfid
+                                    continue
 
                                 referenced_object = all_objects_dict.get(v, None)
 
                                 if referenced_object is None and all_objects_dict_boundary:
                                     # search for the reference in the boundary set
                                     referenced_object = all_objects_dict_boundary.get(v, None)
 
@@ -448,14 +448,16 @@
     :param all_objects_dict_boundary: dictionary of all boundary set objects to
                                       add Parsed objects used to find references
     :param elements_by_type: Dictionary of elements by type to fill in (same as all_objects_dict but by categories)
     :param class_dict: CgmesCircuit or None
     :param logger:DataLogger
     :return: None
     """
+    import time
+    start = time.time()
     for class_name, objects_dict in data.items():
 
         objects_list = list()
         for rdfid, object_data in objects_dict.items():
 
             object_template = class_dict.get(class_name, None)
 
@@ -474,22 +476,26 @@
 
                 objects_list.append(parsed_object)
 
             else:
                 logger.add_error("Class not recognized", device_class=class_name)
 
         elements_by_type[class_name] = objects_list
-
+    endt = time.time()
+    print("data to object: ", endt - start, "sec")
+    start = time.time()
     # replace refferences by actual objects
     find_references(elements_by_type=elements_by_type,
                     all_objects_dict=all_objects_dict,
                     all_objects_dict_boundary=all_objects_dict_boundary,
                     association_inverse_dict=association_inverse_dict,
                     logger=logger,
                     mark_used=True)
+    endt = time.time()
+    print("find references: ", endt - start, "sec")
 
 
 class CgmesCircuit(BaseCircuit):
     """
     CgmesCircuit
     """
 
@@ -1004,40 +1010,41 @@
         """
 
         # read the CGMES data as dictionaries
         # data_parser = CgmesDataParser(text_func=self.text_func,
         #                               progress_func=self.progress_func,
         #                               logger=self.logger)
         # data_parser.load_files(files=files)
-
+        import time
         # set the data
         self.set_data(data=data_parser.data,
                       boundary_set=data_parser.boudary_set)
 
         # convert the dictionaries to the internal class model for the boundary set
         # do not mark the boundary set objects as used
         convert_data_to_objects(data=self.boundary_set,
                                 all_objects_dict=self.all_objects_dict_boundary,
                                 all_objects_dict_boundary=None,
                                 elements_by_type=self.elements_by_type_boundary,
                                 class_dict=self.class_dict,
                                 association_inverse_dict=self.association_inverse_dict,
                                 logger=self.logger)
-
+        start = time.time()
         # convert the dictionaries to the internal class model,
         # this marks as used only the boundary set objects that are referenced,
         # this allows to delete the excess of boundary set objects later
         convert_data_to_objects(data=self.data,
                                 all_objects_dict=self.all_objects_dict,
                                 all_objects_dict_boundary=self.all_objects_dict_boundary,
                                 elements_by_type=self.elements_by_type,
                                 class_dict=self.class_dict,
                                 association_inverse_dict=self.association_inverse_dict,
                                 logger=self.logger)
-
+        endt = time.time()
+        print("Data to objects time: ", endt - start, "sec")
         # Assign the data from all_objects_dict to the appropriate lists in the circuit
         self.assign_data_to_lists()
 
         if delete_unused:
             # delete the unused objects from the boundary set
             self.delete_unused()
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.identified_object import IdentifiedObject
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.geographical_region import GeographicalRegion
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.base_voltage import BaseVoltage
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.substation import Substation
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.voltage_level import VoltageLevel
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.connectivity_node import ConnectivityNode
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.topological_node import TopologicalNode
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.sv_voltage import SvVoltage
@@ -17,7 +18,8 @@
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.nuclear_generating_unit import NuclearGeneratingUnit
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.synchronous_machine import SynchronousMachine
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.ac_line_segment import ACLineSegment
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.regulating_cond_eq import RegulatingCondEq
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.regulating_control import RegulatingControl
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.power_transformer import PowerTransformer
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.power_transformer_end import PowerTransformerEnd
+from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.linear_shunt_compensator import LinearShuntCompensator
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
     def __init__(self, rdfid, tpe):
         IdentifiedObject.__init__(self, rdfid, tpe)
 
         self.scenarioTime: str = None
         self.created: str = None
         self.version: str = None
-        self.profile: str = None
+        self.profile: str | list = None
         self.modelingAuthoritySet: str = None
-        self.DependentOn: str = None
+        self.DependentOn: str | list = None
         self.longDependentOnPF: str = None
         self.Supersedes: str = None
 
         self.register_property(
             name='scenarioTime',
             class_type=str,
             description="scenarioTime.",
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_circuit.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_devices.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_devices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_enums.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/cim16/cim_data_parser.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_data_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/base_db.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/base_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/cgmes_lookup_db.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/cgmes_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/file_system.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/file_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/psse_lookup_db.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/psse_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/IO/cim/db/db_handler.py` & `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/db_handler.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/types.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/types.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/sparse_array.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/sparse_array.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/multi_circuit.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/multi_circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import cmath
 import warnings
 import copy
 import numpy as np
 import pandas as pd
 from typing import List, Dict, Tuple, Union, Any, Callable, Set
 from uuid import getnode as get_mac, uuid4
-from datetime import timedelta, datetime
+import datetime as dateslib
 import networkx as nx
 from matplotlib import pyplot as plt
 from scipy.sparse import csc_matrix, lil_matrix
 
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice
 from GridCalEngine.basic_structures import IntVec, StrVec, Vec, Mat, CxVec, IntMat, CxMat
 from GridCalEngine.data_logger import DataLogger
@@ -188,16 +188,16 @@
 
         # Base power (MVA)
         self.Sbase: float = Sbase
 
         # Base frequency in Hz
         self.fBase: float = fbase
 
-        # Should be able to accept Branches, Lines and Transformers alike
-        # self.Branches = list()
+        # snapshot time
+        self._snapshot_time: dateslib.datetime = dateslib.datetime.now()  # dateslib.datetime(year=2000, month=1, day=1)
 
         self.lines: List[dev.Line] = list()
 
         self.dc_lines: List[dev.DcLine] = list()
 
         self.transformers2w: List[dev.Transformer2W] = list()
 
@@ -438,14 +438,43 @@
         # list of declared diagrams
         self.diagrams: List[Union[dev.MapDiagram, dev.SchematicDiagram]] = list()
 
     def __str__(self):
         return str(self.name)
 
     @property
+    def snapshot_time(self) -> dateslib.datetime:
+        """
+        Returns the current snapshot time
+        :return: Datetime
+        """
+        return self._snapshot_time
+
+    @snapshot_time.setter
+    def snapshot_time(self, val: dateslib.datetime):
+        if type(val) is dateslib.datetime:  # isinstance doesn't work for this
+            self._snapshot_time = dateslib.datetime(year=val.year,
+                                                    month=val.month,
+                                                    day=val.day,
+                                                    hour=val.hour,
+                                                    minute=val.minute,
+                                                    second=val.second,
+                                                    microsecond=val.microsecond)
+        elif type(val) is pd.Timestamp:  # isinstance doesn't work for this
+            self._snapshot_time = dateslib.datetime(year=val.year,
+                                                    month=val.month,
+                                                    day=val.day,
+                                                    hour=val.hour,
+                                                    minute=val.minute,
+                                                    second=val.second,
+                                                    microsecond=val.microsecond)
+        else:
+            raise Exception(f'unsupported value set {val} for snapshot_time')
+
+    @property
     def has_time_series(self) -> bool:
         """
         Area there time series?
         :return: True / False
         """
         # sanity check
         if len(self.buses) > 0:
@@ -468,14 +497,28 @@
     def set_unix_time(self, arr: IntVec):
         """
         Set the time with a unix time
         :param arr: UNIX time iterable
         """
         self.time_profile = pd.to_datetime(arr, unit='s')
 
+    def get_snapshot_time_unix(self) -> int:
+        """
+        Get the unix representation of the snapshot time
+        :return: int
+        """
+        return int(self.snapshot_time.timestamp())
+
+    def set_snapshot_time_unix(self, val: int) -> None:
+        """
+        Convert unix datetime to python datetime
+        :param val: seconds since 1970-01-01T00:00:00
+        """
+        self.snapshot_time = pd.to_datetime(val * 1e9)
+
     def get_objects_with_profiles_list(self) -> List[ALL_DEV_TYPES]:
         """
         get objects_with_profiles in the form of list
         :return: List[dev.EditableDevice]
         """
         lst = list()
         for key, elm_list in self.objects_with_profiles.items():
@@ -2643,31 +2686,31 @@
                 if direction:
                     graph_real_power_flow.add_edge(f, t)
                 else:
                     graph_real_power_flow.add_edge(t, f)
 
         return graph_real_power_flow
 
-    def create_profiles(self, steps, step_length, step_unit, time_base: datetime = datetime.now()):
+    def create_profiles(self, steps, step_length, step_unit, time_base: dateslib.datetime = dateslib.datetime.now()):
         """
         Set the default profiles in all the objects enabled to have profiles.
         :param steps: Number of time steps
         :param step_length: Time length (1, 2, 15, ...)
         :param step_unit: Unit of the time step ("h", "m" or "s")
         :param time_base: Date to start from
         """
 
         index = np.empty(steps, dtype=object)
         for i in range(steps):
             if step_unit == 'h':
-                index[i] = time_base + timedelta(hours=i * step_length)
+                index[i] = time_base + dateslib.timedelta(hours=i * step_length)
             elif step_unit == 'm':
-                index[i] = time_base + timedelta(minutes=i * step_length)
+                index[i] = time_base + dateslib.timedelta(minutes=i * step_length)
             elif step_unit == 's':
-                index[i] = time_base + timedelta(seconds=i * step_length)
+                index[i] = time_base + dateslib.timedelta(seconds=i * step_length)
 
         index = pd.DatetimeIndex(index)
 
         self.format_profiles(index)
 
     def format_profiles(self, index: pd.DatetimeIndex):
         """
@@ -4432,15 +4475,15 @@
                 V_gen.to_excel(writer, 'V generators')
 
                 E_batt.to_excel(writer, 'Energy batteries')
 
         else:
             raise Exception('There are no time series!')
 
-    def set_state(self, t):
+    def set_state(self, t: int):
         """
         Set the profiles state at the index t as the default values.
         """
         for bus in self.buses:
             bus.set_profile_values(t)
 
         for elm in self.get_injection_devices():
@@ -4448,14 +4491,16 @@
 
         for elm in self.get_fluid_devices():
             elm.set_profile_values(t)
 
         for branch in self.get_branches():
             branch.set_profile_values(t)
 
+        self.snapshot_time = self.time_profile[t]
+
     def get_bus_branch_connectivity_matrix(self) -> Tuple[csc_matrix, csc_matrix, csc_matrix]:
         """
         Get the branch-bus connectivity
         :return: Cf, Ct, C
         """
         n = self.get_bus_number()
         m = self.get_branch_number()
@@ -5122,35 +5167,35 @@
     def re_index_time(self, year=None, hours_per_step=1.0):
         """
         Generate sequential time steps to correct the time_profile
         :param year: base year, if None, this year is taken
         :param hours_per_step: number of hours per step, by default 1 hour by step
         """
         if year is None:
-            t0 = datetime.now()
+            t0 = dateslib.datetime.now()
             year = t0.year
 
-        t0 = datetime(year=year, month=1, day=1)
+        t0 = dateslib.datetime(year=year, month=1, day=1)
         self.re_index_time2(t0=t0, step_size=hours_per_step, step_unit='h')
 
     def re_index_time2(self, t0, step_size, step_unit):
         """
         Generate sequential time steps to correct the time_profile
         :param t0: base time
         :param step_size: number of hours per step, by default 1 hour by step
         :param step_unit: 'h', 'm', 's'
         """
         nt = self.get_time_number()
 
         if step_unit == 'h':
-            tm = [t0 + timedelta(hours=t * step_size) for t in range(nt)]
+            tm = [t0 + dateslib.timedelta(hours=t * step_size) for t in range(nt)]
         elif step_unit == 'm':
-            tm = [t0 + timedelta(minutes=t * step_size) for t in range(nt)]
+            tm = [t0 + dateslib.timedelta(minutes=t * step_size) for t in range(nt)]
         elif step_unit == 's':
-            tm = [t0 + timedelta(seconds=t * step_size) for t in range(nt)]
+            tm = [t0 + dateslib.timedelta(seconds=t * step_size) for t in range(nt)]
         else:
             raise Exception("Unsupported time unit")
 
         self.time_profile = pd.to_datetime(tm)
 
     def set_generators_active_profile_from_their_active_power(self):
         """
@@ -5503,14 +5548,20 @@
             logger.add_error(msg="Different number of time steps",
                              device_class="time",
                              value=grid2.get_time_number(),
                              expected_value=self.get_time_number())
         else:
             nt = self.get_time_number()
 
+        if self.snapshot_time != grid2.snapshot_time:
+            logger.add_error(msg="Different snapshot times",
+                             device_class="snapshot time",
+                             value=str(grid2.get_snapshot_time_unix),
+                             expected_value=self.get_snapshot_time_unix)
+
         # for each category
         for key, template_elms_list in self.objects_with_profiles.items():
 
             # for each object type
             for template_elm in template_elms_list:
 
                 # get all objects of the type
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/measurement.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/profile.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/profile.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/municipality.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/municipality.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/contingency_group.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/fuel.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/fuel.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,24 +63,7 @@
     def cost_prof(self, val: Union[Profile, np.ndarray]):
         if isinstance(val, Profile):
             self._cost_prof = val
         elif isinstance(val, np.ndarray):
             self._cost_prof.set(arr=val)
         else:
             raise Exception(str(type(val)) + 'not supported to be set into a cost_prof')
-
-    def get_properties_dict(self, version=3):
-        data = {'id': self.idtag,
-                'name': self.name,
-                'code': self.code,
-                'cost': self.cost,
-                }
-        return data
-
-    def get_profiles_dict(self, version=3):
-        data = {'id': self.idtag,
-                'cost': self.cost_prof}
-        return data
-
-    def get_units_dict(self, version=3):
-        data = {}
-        return data
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/contingency.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency.py`

 * *Files 19% similar despite different names*

```diff
@@ -114,23 +114,7 @@
         """
         return self.group.category
 
     @category.setter
     def category(self, val):
         # self.group.category = val
         pass
-
-    def get_properties_dict(self, version=3):
-        """
-        Get json dictionary
-        :return:
-        """
-
-        return {
-            'id': self.idtag,
-            'name': self.name,
-            'name_code': self.code,
-            'group': self._group.idtag,
-            'device_uuid': self.device_idtag,
-            'prop': self.prop,
-            'value': self.value,
-        }
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/emission_gas.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investment.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,79 +11,81 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-
 from typing import Union
-import numpy as np
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice, DeviceType
-from GridCalEngine.Devices.profile import Profile
+from GridCalEngine.Devices.Aggregation.investments_group import InvestmentsGroup
 
 
-class EmissionGas(EditableDevice):
+class Investment(EditableDevice):
+    """
+    Investment
+    """
 
     def __init__(self,
-                 name: str = '',
-                 code: str = '',
                  idtag: Union[str, None] = None,
-                 cost: float = 0.0,
-                 color: Union[str, None] = None):
+                 device_idtag: Union[str, None] = None,
+                 name="Investment",
+                 code='',
+                 CAPEX=0.0,
+                 OPEX=0.0,
+                 group: InvestmentsGroup = None,
+                 comment: str = ""):
         """
-        Emission gas object
-        :param name: name of the gas (CO2, NOx, etc.)
-        :param code: secondary id
-        :param idtag: UUID code
-        :param cost: cost per tonn (e/t)
-        :param color: hexadecimal color string (i.e. #AA00FF)
+        Contingency
+        :param idtag: String. Element unique identifier
+        :param name: String. Contingency name
+        :param code: String. Contingency code name
+        :param CAPEX: Float. Capital expenditures
+        :param OPEX: Float. Operating expenditures
+        :param group: ContingencyGroup. Contingency group
+        :param comment: Comment
         """
+
         EditableDevice.__init__(self,
-                                name=name,
-                                code=code,
                                 idtag=idtag,
-                                device_type=DeviceType.EmissionGasDevice)
-
-        self.cost = cost
+                                code=code,
+                                name=name,
+                                device_type=DeviceType.InvestmentDevice,
+                                comment=comment)
 
-        self._cost_prof = Profile(default_value=cost, data_type=float)
+        # Contingency type
+        self.device_idtag = device_idtag
+        self.CAPEX = CAPEX
+        self.OPEX = OPEX
+        self._group: InvestmentsGroup = group
+
+        self.register(key='device_idtag', units='', tpe=str, definition='Unique ID')
+        self.register(key='CAPEX', units='Me', tpe=float,
+                      definition='Capital expenditures. This is the initial investment.')
+        self.register(key='OPEX', units='Me', tpe=float,
+                      definition='Operation expenditures. Maintenance costs among other recurrent costs.')
+        self.register(key='group', units='', tpe=DeviceType.InvestmentsGroupDevice, definition='Investment group')
 
-        self.color = color if color is not None else self.rnd_color()
+    @property
+    def group(self) -> InvestmentsGroup:
+        """
+        Group of investments
+        :return:
+        """
+        return self._group
 
-        self.register(key='cost', units='e/t', tpe=float, definition='Cost of emissions (e / ton)',
-                      profile_name='cost_prof')
-        self.register(key='color', units='', tpe=str, definition='Color to paint')
+    @group.setter
+    def group(self, val: InvestmentsGroup):
+        self._group = val
 
     @property
-    def cost_prof(self) -> Profile:
+    def category(self):
         """
-        Cost profile
-        :return: Profile
+        Display the group category
+        :return:
         """
-        return self._cost_prof
+        return self.group.category
 
-    @cost_prof.setter
-    def cost_prof(self, val: Union[Profile, np.ndarray]):
-        if isinstance(val, Profile):
-            self._cost_prof = val
-        elif isinstance(val, np.ndarray):
-            self._cost_prof.set(arr=val)
-        else:
-            raise Exception(str(type(val)) + 'not supported to be set into a cost_prof')
-
-    def get_properties_dict(self, version=3):
-
-        data = {'id': self.idtag,
-                'name': self.name,
-                'code': self.code,
-                'cost': self.cost,
-                }
-        return data
-
-    def get_profiles_dict(self, version=3):
-        data = {'id': self.idtag}
-        return data
-
-    def get_units_dict(self, version=3):
-        data = {}
-        return data
+    @category.setter
+    def category(self, val):
+        # self.group.category = val
+        pass
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/country.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/country.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/modelling_authority.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/modelling_authority.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/region.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/area.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/area.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,17 @@
                                 code=code,
                                 idtag=idtag,
                                 device_type=device_type)
 
         self.latitude = latitude
         self.longitude = longitude
 
-        self.register(key='longitude', units='deg', tpe=float, definition='longitude of the bus.', profile_name='',
+        self.register(key='longitude', units='deg', tpe=float, definition='longitude.', profile_name='',
                       editable=False)
-        self.register(key='latitude', units='deg', tpe=float, definition='latitude of the bus.', profile_name='',
+        self.register(key='latitude', units='deg', tpe=float, definition='latitude.', profile_name='',
                       editable=False)
 
 
 class Area(GenericAreaGroup):
 
     def __init__(self, name: str = 'Area', idtag: Union[str, None] = None, code: str = '', latitude=0.0, longitude=0.0):
         """
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/technology.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/technology.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,25 +44,7 @@
 
         self.color = color if color is not None else self.rnd_color()
 
         self.register(key='name2', units='', tpe=str, definition='Name 2 of the technology')
         self.register(key='name3', units='', tpe=str, definition='Name 3 of the technology')
         self.register(key='name4', units='', tpe=str, definition='Name 4 of the technology')
         self.register(key='color', units='', tpe=str, definition='Color to paint')
-
-    def get_properties_dict(self, version=3):
-        data = {'id': self.idtag,
-                'name': self.name,
-                'name2': self.name2,
-                'name3': self.name3,
-                'name4': self.name4,
-                'code': self.code
-                }
-        return data
-
-    def get_profiles_dict(self, version=3):
-        data = {'id': self.idtag}
-        return data
-
-    def get_units_dict(self, version=3):
-        data = {}
-        return data
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/zone.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/zone.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,9 +42,8 @@
                                   code=code,
                                   device_type=DeviceType.ZoneDevice,
                                   latitude=latitude,
                                   longitude=longitude)
 
         self.area: Union[Area, None] = area
 
-        self.register(key="area", units="", tpe=DeviceType.AreaDevice,
-                      definition="Substation area, altenativelly this can be obtained from the zone")
+        self.register(key="area", units="", tpe=DeviceType.AreaDevice, definition="Area of this zone.")
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/investments_group.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investments_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,28 +37,14 @@
         :param comment: comment
         """
 
         EditableDevice.__init__(self,
                                 name=name,
                                 idtag=idtag,
                                 code='',
-                                device_type=DeviceType.InvestmentsGroupDevice)
+                                device_type=DeviceType.InvestmentsGroupDevice,
+                                comment=comment)
 
         # Contingency type
         self.category = category
-        self.comment = comment
 
         self.register(key='category', units='', tpe=str, definition='Some tag to category the contingency group')
-
-        self.register(key='comment', units='', tpe=str, definition='Some comment')
-
-    def get_properties_dict(self, version=3):
-        """
-        Get json dictionary
-        :return:
-        """
-
-        return {
-            'id': self.idtag,
-            'name': self.name,
-            'category': self.category,
-        }
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/investment.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/underground_line_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,99 +11,104 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-from typing import Union
+import numpy as np
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice, DeviceType
-from GridCalEngine.Devices.Aggregation.investments_group import InvestmentsGroup
 
 
-class Investment(EditableDevice):
-    """
-    Investment
-    """
-
-    def __init__(self,
-                 idtag: Union[str, None] = None,
-                 device_idtag: Union[str, None] = None,
-                 name="Investment",
-                 code='',
-                 CAPEX=0.0,
-                 OPEX=0.0,
-                 group: InvestmentsGroup = None,
-                 comment: str = ""):
-        """
-        Contingency
-        :param idtag: String. Element unique identifier
-        :param name: String. Contingency name
-        :param code: String. Contingency code name
-        :param CAPEX: Float. Capital expenditures
-        :param OPEX: Float. Operating expenditures
-        :param group: ContingencyGroup. Contingency group
-        :param comment: Comment
-        """
+class UndergroundLineType(EditableDevice):
 
+    def __init__(self, name='UndergroundLine', idtag=None, Imax=1, Vnom=1, R=0, X=0, B=0, R0=0, X0=0, B0=0):
+        """
+        Constructor
+        :param name: name of the device
+        :param Imax: rating in kA
+        :param R: Resistance of positive sequence in Ohm/km
+        :param X: Reactance of positive sequence in Ohm/km
+        :param B: Susceptance of positive sequence in uS/km
+        :param R0: Resistance of zero sequence in Ohm/km
+        :param X0: Reactance of zero sequence in Ohm/km
+        :param B0: Susceptance of zero sequence in uS/km
+        """
         EditableDevice.__init__(self,
-                                idtag=idtag,
-                                code=code,
                                 name=name,
-                                device_type=DeviceType.InvestmentDevice)
+                                idtag=idtag,
+                                code='',
+                                device_type=DeviceType.UnderGroundLineDevice)
+
+        self.Imax = Imax
+        self.Vnom = Vnom
+
+        # impudence and admittance per unit of length
+        self.R = R
+        self.X = X
+        self.B = B
+
+        self.R0 = R0
+        self.X0 = X0
+        self.B0 = B0
+
+        self.register(key='Imax', units='kA', tpe=float, definition='Current rating of the line', old_names=['rating'])
+        self.register(key='Vnom', units='kV', tpe=float, definition='Voltage rating of the line')
+        self.register(key='R', units='Ohm/km', tpe=float, definition='Positive-sequence resistance per km')
+        self.register(key='X', units='Ohm/km', tpe=float, definition='Positive-sequence reactance per km')
+        self.register(key='B', units='uS/km', tpe=float, definition='Positive-sequence shunt susceptance per km')
+        self.register(key='R0', units='Ohm/km', tpe=float, definition='Zero-sequence resistance per km')
+        self.register(key='X0', units='Ohm/km', tpe=float, definition='Zero-sequence reactance per km')
+        self.register(key='B0', units='uS/km', tpe=float, definition='Zero-sequence shunt susceptance per km')
+
+    def get_values(self, Sbase, length):
+        """
+        Get the per-unit values
+        :param Sbase: Base power (MVA, always use 100MVA)
+        :param length: length in km
+        :return: R (p.u.), x(p.u.), B(p.u.), Rate (MVA)
+        """
+        Vn = self.Vnom
+        Zbase = (Vn * Vn) / Sbase
+        Ybase = 1.0 / Zbase
+
+        R = np.round(self.R * length / Zbase, 6)
+        X = np.round(self.X * length / Zbase, 6)
+        B = np.round(self.B * 1e6 * length / Ybase, 6)
+
+        R0 = np.round(self.R0 * length / Zbase, 6)
+        X0 = np.round(self.X0 * length / Zbase, 6)
+        B0 = np.round(self.B0 * 1e6 * length / Ybase, 6)
+
+        # get the rating in MVA = kA * kV
+        rate = self.Imax * Vn * np.sqrt(3)
+
+        return R, X, B, R0, X0, B0, rate
+
+    def z_series(self):
+        """
+        positive sequence series impedance in Ohm per unit of length
+        """
+        return self.R + 1j * self.X
+
+    def y_shunt(self):
+        """
+        positive sequence shunt admittance in S per unit of length
+        """
+        return 1j * self.B
+
+    def change_base(self, Sbase_old, Sbase_new):
+        """
+        change the per unit base
+        :param Sbase_old: old base in MVA
+        :param Sbase_new: new base in MVA
+        """
+        b = Sbase_new / Sbase_old
+
+        self.R *= b
+        self.X *= b
+        self.B *= b
+
+        self.R0 *= b
+        self.X0 *= b
+        self.B0 *= b
 
-        # Contingency type
-        self.device_idtag = device_idtag
-        self.CAPEX = CAPEX
-        self.OPEX = OPEX
-        self._group: InvestmentsGroup = group
-        self.comment = comment
-
-        self.register(key='device_idtag', units='', tpe=str, definition='Unique ID')
-        self.register(key='CAPEX', units='Me', tpe=float,
-                      definition='Capital expenditures. This is the initial investment.')
-        self.register(key='OPEX', units='Me', tpe=float,
-                      definition='Operation expenditures. Maintenance costs among other recurrent costs.')
-        self.register(key='group', units='', tpe=DeviceType.InvestmentsGroupDevice, definition='Investment group')
-        self.register(key='comment', units='', tpe=str, definition='Comments')
-
-    @property
-    def group(self) -> InvestmentsGroup:
-        """
-        Group of investments
-        :return:
-        """
-        return self._group
-
-    @group.setter
-    def group(self, val: InvestmentsGroup):
-        self._group = val
-
-    @property
-    def category(self):
-        """
-        Display the group category
-        :return:
-        """
-        return self.group.category
-
-    @category.setter
-    def category(self, val):
-        # self.group.category = val
-        pass
-
-    def get_properties_dict(self, version=3):
-        """
-        Get json dictionary
-        :return:
-        """
-
-        return {
-            'id': self.idtag,
-            'name': self.name,
-            'name_code': self.code,
-            'group': self._group,
-            'device_idtag': self.device_idtag,
-            'CAPEX': self.CAPEX,
-            'OPEX': self.OPEX,
-            'comment': self.comment
-        }
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/community.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/community.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Aggregation/branch_group.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/branch_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_path.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_path.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_pump.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_node.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_turbine.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_turbine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_injection_template.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_injection_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Fluid/fluid_p2x.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_p2x.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/dc_line.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/underground_line_type.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/sequence_line_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,33 +15,35 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 import numpy as np
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice, DeviceType
 
 
-class UndergroundLineType(EditableDevice):
+class SequenceLineType(EditableDevice):
 
-    def __init__(self, name='UndergroundLine', idtag=None, Imax=1, Vnom=1, R=0, X=0, B=0, R0=0, X0=0, B0=0):
+    def __init__(self, name='SequenceLine', idtag=None, Imax=1, Vnom=1,
+                 R=0, X=0, B=0, R0=0, X0=0, B0=0):
         """
         Constructor
-        :param name: name of the device
-        :param Imax: rating in kA
+        :param name: name of the model
+        :param Imax: Line rating current in kA
         :param R: Resistance of positive sequence in Ohm/km
         :param X: Reactance of positive sequence in Ohm/km
         :param B: Susceptance of positive sequence in uS/km
         :param R0: Resistance of zero sequence in Ohm/km
         :param X0: Reactance of zero sequence in Ohm/km
         :param B0: Susceptance of zero sequence in uS/km
         """
+
         EditableDevice.__init__(self,
                                 name=name,
                                 idtag=idtag,
-                                code='',
-                                device_type=DeviceType.UnderGroundLineDevice)
+                                code="",
+                                device_type=DeviceType.SequenceLineDevice)
 
         self.Imax = Imax
         self.Vnom = Vnom
 
         # impudence and admittance per unit of length
         self.R = R
         self.X = X
@@ -79,36 +81,7 @@
         X0 = np.round(self.X0 * length / Zbase, 6)
         B0 = np.round(self.B0 * 1e6 * length / Ybase, 6)
 
         # get the rating in MVA = kA * kV
         rate = self.Imax * Vn * np.sqrt(3)
 
         return R, X, B, R0, X0, B0, rate
-
-    def z_series(self):
-        """
-        positive sequence series impedance in Ohm per unit of length
-        """
-        return self.R + 1j * self.X
-
-    def y_shunt(self):
-        """
-        positive sequence shunt admittance in S per unit of length
-        """
-        return 1j * self.B
-
-    def change_base(self, Sbase_old, Sbase_new):
-        """
-        change the per unit base
-        :param Sbase_old: old base in MVA
-        :param Sbase_new: new base in MVA
-        """
-        b = Sbase_new / Sbase_old
-
-        self.R *= b
-        self.X *= b
-        self.B *= b
-
-        self.R0 *= b
-        self.X0 *= b
-        self.B0 *= b
-
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/series_reactance.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/series_reactance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/wire.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/wire.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/line_locations.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line_locations.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/overhead_line_type.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/overhead_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/switch.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/switch.py`

 * *Files 20% similar despite different names*

```diff
@@ -133,78 +133,14 @@
 
             elif properties.tpe not in [str, float, int, bool]:
                 obj = str(obj)
 
             data.append(obj)
         return data
 
-    def get_properties_dict(self, version=3):
-        """
-        Get json dictionary
-        :return:
-        """
-        if version == 2:
-            d = {'id': self.idtag,
-                 'type': 'Switch',
-                 'phases': 'ps',
-                 'name': self.name,
-                 'name_code': self.code,
-                 'bus_from': self.bus_from.idtag,
-                 'bus_to': self.bus_to.idtag,
-                 'active': self.active,
-
-                 'rate': self.rate,
-
-                 'r': self.R,
-                 'x': self.X
-                 }
-        elif version == 3:
-            d = {'id': self.idtag,
-                 'type': 'Switch',
-                 'phases': 'ps',
-                 'name': self.name,
-                 'name_code': self.code,
-                 'bus_from': self.bus_from.idtag,
-                 'bus_to': self.bus_to.idtag,
-                 'active': self.active,
-
-                 'rate': self.rate,
-                 'contingency_factor1': self.contingency_factor,
-                 'contingency_factor2': self.contingency_factor,
-                 'contingency_factor3': self.contingency_factor,
-
-                 'r': self.R,
-                 'x': self.X
-                 }
-        else:
-            d = dict()
-
-        return d
-
-    def get_profiles_dict(self, version=3):
-        """
-
-        :return:
-        """
-        if self.active_prof is not None:
-            active_prof = self.active_prof.tolist()
-        else:
-            active_prof = list()
-
-        return {'id': self.idtag,
-                'active': active_prof}
-
-    def get_units_dict(self, version=3):
-        """
-        Get units of the values
-        """
-        return {'rate': 'MW',
-                'r': 'p.u.',
-                'x': 'p.u.'}
-
     def plot_profiles(self, time_series=None, my_index=0, show_fig=True):
         """
         Plot the time series results of this object
         :param time_series: TimeSeries Instance
         :param my_index: index of this object in the simulation
         :param show_fig: Show the figure?
         """
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/vsc.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/vsc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/upfc.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/upfc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/transformer.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/hvdc_line.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/hvdc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/line.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/tap_changer.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/winding.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/winding.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/branch.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/branch.py`

 * *Files 5% similar despite different names*

```diff
@@ -370,50 +370,14 @@
 
             elif properties.tpe not in [str, float, int, bool]:
                 obj = str(obj)
 
             data.append(obj)
         return data
 
-    def get_properties_dict(self, version=3):
-        """
-        Get json dictionary
-        :return:
-        """
-
-        d = {'id': self.idtag,
-             'type': 'branch',
-             'phases': 'ps',
-             'name': self.name,
-             'from': self.bus_from.idtag,
-             'to': self.bus_to.idtag,
-             'active': self.active,
-             'rate': self.rate,
-             'r': self.R,
-             'x': self.X,
-             'g': self.G,
-             'b': self.B,
-             'length': self.length,
-             'tap_module': self.tap_module,
-             'bus_to_regulated': self.bus_to_regulated,
-             'vset': self.vset,
-             'temp_base': self.temp_base,
-             'temp_oper': self.temp_oper,
-             'alpha': self.alpha,
-             'tap_angle': self.angle,
-             'branch_type': str(self.branch_type),
-             'active_profile': [],
-             'rate_prof': []}
-
-        if self.active_prof is not None:
-            d['active_profile'] = self.active_prof.tolist()
-            d['rate_prof'] = self.rate_prof.tolist()
-
-        return d
-
     def plot_profiles(self, time_series=None, my_index=0, show_fig=True):
         """
         Plot the time series results of this object
         :param time_series: TimeSeries Instance
         :param my_index: index of this object in the simulation
         :param show_fig: Show the figure?
         """
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/transformer_type.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Branches/transformer3w.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer3w.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/static_generator.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/static_generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/external_grid.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/external_grid.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/current_injection.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/current_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/battery.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/battery.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/generator.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/generator_q_curve.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator_q_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/controllable_shunt.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/controllable_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Injections/load.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/graphic_location.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/graphic_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/map_diagram.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/map_location.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/schematic_diagram.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/schematic_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Diagrams/base_diagram.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/base_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/connectivity_node.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/voltage_level.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/bus.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/busbar.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Substation/substation.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/injection_parent.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/injection_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/editable_device.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/editable_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,16 @@
     This is the main device class from which all inherit
     """
 
     def __init__(self,
                  name: str,
                  idtag: Union[str, None],
                  code: str,
-                 device_type: DeviceType):
+                 device_type: DeviceType,
+                 comment: str = ""):
         """
         Class to generalize any editable device
         :param name: Asset's name
         :param device_type: DeviceType instance
         :param idtag: unique ID, if not provided it is generated
         :param code: alternative code to identify this object in other databases (i.e. psse number tec...)
         """
@@ -170,26 +171,32 @@
 
         self._name: str = name
 
         self.code: str = code
 
         self.device_type: DeviceType = device_type
 
+        self.comment: str = comment
+
         # list of registered properties. This is supremelly useful when accessing via the Table and Tree models
         self.property_list: List[GCProp] = list()
 
+        # dictionary of properties
         self.registered_properties: Dict[str, GCProp] = dict()
 
+        # list of properties that cannot be edited
         self.non_editable_properties: List[str] = list()
 
+
         self.properties_with_profile: Dict[str, Optional[Any]] = dict()
 
         self.register(key='idtag', units='', tpe=str, definition='Unique ID', editable=False)
-        self.register(key='name', units='', tpe=str, definition='Name of the branch.')
+        self.register(key='name', units='', tpe=str, definition='Name of the device.')
         self.register(key='code', units='', tpe=str, definition='Secondary ID')
+        self.register(key='comment', units='', tpe=str, definition='User comment')
 
     def __str__(self) -> str:
         """
         Name of the object
         :return: string
         """
         return self.name
@@ -642,48 +649,14 @@
         """
         Get the profile of a property name
         :param prop: GCProp
         :return: Profile object
         """
         return getattr(self, prop.profile_name)
 
-    def get_properties_dict(self, version=3):
-        """
-
-        :param version:
-        :return:
-        """
-        return dict()
-
-    def get_units_dict(self, version=3):
-        """
-
-        :param version:
-        :return:
-        """
-        return dict()
-
-    def get_profiles_dict(self, version=3):
-        """
-
-        :param version:
-        :return:
-        """
-
-        """
-        {'id': self.idtag,
-        'active': active_prof,
-        'rate': rate_prof}
-        """
-        data = {'id': self.idtag}
-        for property_name, profile_name in self.properties_with_profile.items():
-            data[property_name] = profile_name
-
-        return data
-
     def copy(self):
         """
         Create a deep copy of this object
         """
         tpe = type(self)
 
         try:
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/generator_parent.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/shunt_parent.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,64 +13,63 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from typing import Union
 import numpy as np
+import pandas as pd
+from matplotlib import pyplot as plt
 from GridCalEngine.Devices.Substation.bus import Bus
 from GridCalEngine.Devices.Substation.connectivity_node import ConnectivityNode
 from GridCalEngine.enumerations import BuildStatus, DeviceType
-from GridCalEngine.basic_structures import CxVec
 from GridCalEngine.Devices.profile import Profile
 from GridCalEngine.Devices.Parents.injection_parent import InjectionParent
 
 
-class GeneratorParent(InjectionParent):
+class ShuntParent(InjectionParent):
     """
-    Template for objects that behave like generators
+    Template for objects that behave like shunts
     """
 
     def __init__(self,
                  name: str,
                  idtag: Union[str, None],
                  code: str,
                  bus: Union[Bus, None],
                  cn: Union[ConnectivityNode, None],
-                 control_bus: Union[Bus, None],
-                 control_cn: Union[ConnectivityNode, None],
                  active: bool,
-                 P: float,
-                 Pmin: float,
-                 Pmax: float,
+                 G: float,
+                 B: float,
+                 G0: float,
+                 B0: float,
                  Cost: float,
                  mttf: float,
                  mttr: float,
                  capex: float,
                  opex: float,
-                 srap_enabled: bool,
                  build_status: BuildStatus,
                  device_type: DeviceType):
         """
-
+        ShuntLikeTemplate
         :param name: Name of the device
         :param idtag: unique id of the device (if None or "" a new one is generated)
         :param code: secondary code for compatibility
         :param bus: snapshot bus object
         :param cn: connectivity node
         :param active:active state
-        :param P: active power (MW)
-        :param Pmin: minimum active power (MW)
-        :param Pmax: maximum active power (MW)
+        :param G: positive conductance (MW @ v=1 p.u.)
+        :param B: positive conductance (MVAr @ v=1 p.u.)
+        :param G0: zero-sequence conductance (MW @ v=1 p.u.)
+        :param B0: zero-sequence conductance (MVAr @ v=1 p.u.)
         :param Cost: cost associated with various actions (dispatch or shedding)
         :param mttf: mean time to failure (h)
         :param mttr: mean time to recovery (h)
         :param capex: capital expenditures (investment cost)
         :param opex: operational expenditures (maintainance cost)
-        :param srap_enabled: Is the unit available for SRAP participation?
         :param build_status: BuildStatus
         :param device_type: DeviceType
         """
 
         InjectionParent.__init__(self,
                                  name=name,
                                  idtag=idtag,
@@ -82,138 +81,128 @@
                                  mttf=mttf,
                                  mttr=mttr,
                                  capex=capex,
                                  opex=opex,
                                  build_status=build_status,
                                  device_type=device_type)
 
-        self.control_bus = control_bus
-        self._control_bus_prof = Profile(default_value=control_bus, data_type=DeviceType.BusDevice)
-
-        self.control_cn = control_cn
-
-        self.P = P
-        self._P_prof = Profile(default_value=P, data_type=float)
-
-        self.srap_enabled = srap_enabled
-        self._srap_enabled_prof = Profile(default_value=srap_enabled, data_type=bool)
-
-        # Minimum dispatched power in MW
-        self.Pmin = Pmin
-
-        # Maximum dispatched power in MW
-        self.Pmax = Pmax
+        self.G = G
+        self._G_prof = Profile(default_value=G, data_type=float)
 
-        self.register(key='control_bus', units='', tpe=DeviceType.BusDevice, definition='Control bus',
-                      editable=False, profile_name="control_bus_prof")
+        self.B = B
+        self._B_prof = Profile(default_value=B, data_type=float)
 
-        self.register(key='control_cn', units='', tpe=DeviceType.ConnectivityNodeDevice,
-                      definition='Control connectivity node', editable=False)
-        self.register(key='P', units='MW', tpe=float, definition='Active power', profile_name='P_prof')
-        self.register(key='Pmin', units='MW', tpe=float, definition='Minimum active power. Used in OPF.')
-        self.register(key='Pmax', units='MW', tpe=float, definition='Maximum active power. Used in OPF.')
+        self.G0 = G0
+        self._G0_prof = Profile(default_value=G0, data_type=float)
 
-        self.register(key='srap_enabled', units='', tpe=bool,
-                      definition='Is the unit available for SRAP participation?',
-                      editable=True, profile_name="srap_enabled_prof")
+        self.B0 = B0
+        self._B0_prof = Profile(default_value=B0, data_type=float)
+
+        self.register(key='G', units='MW', tpe=float, definition='Active power', profile_name='G_prof')
+        self.register(key='B', units='MVAr', tpe=float, definition='Reactive power', profile_name='B_prof')
+        self.register(key='G0', units='MW', tpe=float,
+                      definition='Zero sequence active power of the impedance component at V=1.0 p.u.',
+                      profile_name='G0_prof')
+        self.register(key='B0', units='MVAr', tpe=float,
+                      definition='Zero sequence reactive power of the impedance component at V=1.0 p.u.',
+                      profile_name='B0_prof')
 
     @property
-    def control_bus_prof(self) -> Profile:
+    def G_prof(self) -> Profile:
         """
-        Control bus profile
+        Cost profile
         :return: Profile
         """
-        return self._control_bus_prof
+        return self._G_prof
 
-    @control_bus_prof.setter
-    def control_bus_prof(self, val: Union[Profile, np.ndarray]):
+    @G_prof.setter
+    def G_prof(self, val: Union[Profile, np.ndarray]):
         if isinstance(val, Profile):
-            self._control_bus_prof = val
+            self._G_prof = val
         elif isinstance(val, np.ndarray):
-            self._control_bus_prof.set(arr=val)
+            self._G_prof.set(arr=val)
         else:
-            raise Exception(str(type(val)) + 'not supported to be set into control_bus_prof')
+            raise Exception(str(type(val)) + 'not supported to be set into a G_prof')
 
     @property
-    def P_prof(self) -> Profile:
+    def B_prof(self) -> Profile:
         """
         Cost profile
         :return: Profile
         """
-        return self._P_prof
+        return self._B_prof
 
-    @P_prof.setter
-    def P_prof(self, val: Union[Profile, np.ndarray]):
+    @B_prof.setter
+    def B_prof(self, val: Union[Profile, np.ndarray]):
         if isinstance(val, Profile):
-            self._P_prof = val
+            self._B_prof = val
         elif isinstance(val, np.ndarray):
-            self._P_prof.set(arr=val)
+            self._B_prof.set(arr=val)
         else:
-            raise Exception(str(type(val)) + 'not supported to be set into a P_prof')
+            raise Exception(str(type(val)) + 'not supported to be set into a B_prof')
 
     @property
-    def srap_enabled_prof(self) -> Profile:
+    def G0_prof(self) -> Profile:
         """
-        Control bus profile
+        Cost profile
         :return: Profile
         """
-        return self._srap_enabled_prof
+        return self._G0_prof
 
-    @srap_enabled_prof.setter
-    def srap_enabled_prof(self, val: Union[Profile, np.ndarray]):
+    @G0_prof.setter
+    def G0_prof(self, val: Union[Profile, np.ndarray]):
         if isinstance(val, Profile):
-            self._srap_enabled_prof = val
+            self._G0_prof = val
         elif isinstance(val, np.ndarray):
-            self._srap_enabled_prof.set(arr=val)
+            self._G0_prof.set(arr=val)
         else:
-            raise Exception(str(type(val)) + 'not supported to be set into srap_enabled_prof')
+            raise Exception(str(type(val)) + 'not supported to be set into a G_prof')
 
-    def get_properties_dict(self, version=3):
+    @property
+    def B0_prof(self) -> Profile:
         """
-        Get json dictionary
-        :return:
+        Cost profile
+        :return: Profile
         """
-        if version in [2, 3]:
-            return {'id': self.idtag,
-                    'type': 'load',
-                    'phases': 'ps',
-                    'name': self.name,
-                    'name_code': self.code,
-                    'bus': self.bus.idtag,
-                    'active': bool(self.active),
-                    'p': self.P,
-                    'shedding_cost': self.Cost
-                    }
+        return self._B0_prof
+
+    @B0_prof.setter
+    def B0_prof(self, val: Union[Profile, np.ndarray]):
+        if isinstance(val, Profile):
+            self._B0_prof = val
+        elif isinstance(val, np.ndarray):
+            self._B0_prof.set(arr=val)
         else:
-            return dict()
+            raise Exception(str(type(val)) + 'not supported to be set into a B_prof')
 
-    def get_profiles_dict(self, version=3):
+    def plot_profiles(self, time=None, show_fig=True):
         """
-
-        :return:
+        Plot the time series results of this object
+        :param time: array of time values
+        :param show_fig: Show the figure?
         """
 
-        if self.active_prof is not None:
-            active_profile = self.active_prof.tolist()
-            P_prof = self.P_prof.tolist()
-
-        else:
-            active_profile = list()
-            P_prof = list()
+        if time is not None:
+            fig = plt.figure(figsize=(12, 8))
 
-        return {'id': self.idtag,
-                'active': active_profile,
-                'p': P_prof}
+            ax_1 = fig.add_subplot(211)
+            ax_2 = fig.add_subplot(212, sharex=ax_1)
 
-    def get_S(self) -> complex:
-        """
+            # G
+            y = self.G_prof.toarray()
+            df = pd.DataFrame(data=y, index=time, columns=[self.name])
+            ax_1.set_title('Conductance power', fontsize=14)
+            ax_1.set_ylabel('MW', fontsize=11)
+            df.plot(ax=ax_1)
 
-        :return:
-        """
-        return complex(self.P, 0.0)
+            # B
+            y = self.B_prof.toarray()
+            df = pd.DataFrame(data=y, index=time, columns=[self.name])
+            ax_2.set_title('Susceptance power', fontsize=14)
+            ax_2.set_ylabel('MVAr', fontsize=11)
+            df.plot(ax=ax_2)
 
-    def get_Sprof(self) -> CxVec:
-        """
+            plt.legend()
+            fig.suptitle(self.name, fontsize=20)
 
-        :return:
-        """
-        return self.P_prof.toarray().astype(complex)
+            if show_fig:
+                plt.show()
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/controllable_branch_parent.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/controllable_branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/load_parent.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/load_parent.py`

 * *Files 20% similar despite different names*

```diff
@@ -135,55 +135,14 @@
     def get_Sprof(self) -> CxVec:
         """
 
         :return:
         """
         return self.P_prof.toarray() + 1j * self.Q_prof.toarray()
 
-    def get_properties_dict(self, version=3):
-        """
-        Get json dictionary
-        :return:
-        """
-        if version in [2, 3]:
-            return {'id': self.idtag,
-                    'type': 'load',
-                    'phases': 'ps',
-                    'name': self.name,
-                    'name_code': self.code,
-                    'bus': self.bus.idtag,
-                    'active': bool(self.active),
-                    'p': self.P,
-                    'q': self.Q,
-                    'shedding_cost': self.Cost
-                    }
-        else:
-            return dict()
-
-    def get_profiles_dict(self, version=3):
-        """
-
-        :return:
-        """
-
-        if self.active_prof is not None:
-            active_profile = self.active_prof.tolist()
-            P_prof = self.P_prof.tolist()
-            Q_prof = self.Q_prof.tolist()
-
-        else:
-            active_profile = list()
-            P_prof = list()
-            Q_prof = list()
-
-        return {'id': self.idtag,
-                'active': active_profile,
-                'p': P_prof,
-                'q': Q_prof}
-
     def plot_profiles(self, time=None, show_fig=True):
         """
         Plot the time series results of this object
         :param time: array of time values
         :param show_fig: Show the figure?
         """
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Parents/branch_parent.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/generator_emission.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_emission.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,25 +50,7 @@
 
         self.rate = rate
 
         self.register(key='generator', units='', tpe=DeviceType.GeneratorDevice, definition='Generator')
         self.register(key='emission', units='', tpe=DeviceType.EmissionGasDevice, definition='Emission')
         self.register(key='rate', units='t/MWh', tpe=float,
                       definition='Emissions rate of the gas in the generator (t/MWh)')
-
-    def get_properties_dict(self, version=3):
-        data = {'id': self.idtag,
-                'name': self.name,
-                'code': self.code,
-                'generator': self.generator,
-                'emission': self.emission,
-                'rate': self.rate
-                }
-        return data
-
-    def get_profiles_dict(self, version=3):
-        data = {'id': self.idtag}
-        return data
-
-    def get_units_dict(self, version=3):
-        data = {}
-        return data
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/generator_technology.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_technology.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,25 +50,7 @@
 
         self.proportion = proportion
 
         self.register(key='generator', units='', tpe=DeviceType.GeneratorDevice, definition='Generator object')
         self.register(key='technology', units='', tpe=DeviceType.Technology, definition='Technology object')
         self.register(key='proportion', units='p.u.', tpe=float,
                       definition='Share of the generator associated to the technology')
-
-    def get_properties_dict(self, version=3):
-        data = {'id': self.idtag,
-                'name': self.name,
-                'code': self.code,
-                'generator': self.generator,
-                'technology': self.technology,
-                'proportion': self.proportion
-                }
-        return data
-
-    def get_profiles_dict(self, version=3):
-        data = {'id': self.idtag}
-        return data
-
-    def get_units_dict(self, version=3):
-        data = {}
-        return data
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Devices/Associations/generator_fuel.py` & `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_fuel.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,24 +51,7 @@
         self.rate = rate
 
         self.register(key='generator', units='', tpe=DeviceType.GeneratorDevice, definition='Generator')
         self.register(key='fuel', units='', tpe=DeviceType.FuelDevice, definition='Fuel')
         self.register(key='rate', units='t/MWh', tpe=float,
                       definition='Fuel consumption rate in the generator')
 
-    def get_properties_dict(self, version=3):
-        data = {'id': self.idtag,
-                'name': self.name,
-                'code': self.code,
-                'generator': self.generator,
-                'fuel': self.fuel,
-                'rate': self.rate
-                }
-        return data
-
-    def get_profiles_dict(self, version=3):
-        data = {'id': self.idtag}
-        return data
-
-    def get_units_dict(self, version=3):
-        data = {}
-        return data
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/load_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/load_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/bus_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/bus_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/branch_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/branch_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_turbine_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_turbine_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_p2x_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_p2x_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/numerical_circuit.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/numerical_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/generator_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/generator_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_pump_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_pump_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/battery_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/battery_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_path_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_path_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/hvdc_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/hvdc_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/shunt_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/shunt_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/DataStructures/fluid_node_data.py` & `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_node_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_newton_pa.py` & `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_newton_pa.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_bentayga.py` & `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_bentayga.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Compilers/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_data.py` & `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_optimods.py` & `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_optimods.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Compilers/circuit_to_pgm.py` & `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_pgm.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/results_template.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/results_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/results_table.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/results_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/driver_types.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_types.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/driver_template.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/topology_reduction_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_reduction_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/topology_processor_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_processor_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Topology/node_groups_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/node_groups_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/reliability_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/reliability_iterable.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_iterable.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/blackout_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/blackout_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/grid_analysis.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/grid_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Dynamics/dynamic_modules.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/dynamic_modules.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_ts_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_ts_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_opf.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_opf.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/NTC/ntc_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/Clustering/clustering_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/StateEstimation/state_estimation.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_estimation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_ts_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_ts_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/linear_opf_ts.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/linear_opf_ts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/opf_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from typing import List, Union
-from GridCalEngine.enumerations import SolverType, MIPSolvers, ZonalGrouping, TimeGrouping
+from GridCalEngine.enumerations import SolverType, MIPSolvers, ZonalGrouping, TimeGrouping, AcOpfMode
 from GridCalEngine.Simulations.PowerFlow.power_flow_results import PowerFlowResults
 
 
 class OptimalPowerFlowOptions:
     """
     OptimalPowerFlowOptions
     """
@@ -46,14 +46,15 @@
                  export_model_fname: Union[None, str] = None,
                  generate_report=False,
                  ips_method: SolverType = SolverType.NR,
                  ips_tolerance: float = 1e-4,
                  ips_iterations: int = 100,
                  ips_trust_radius: float = 1.0,
                  ips_init_with_pf: bool = False,
+                 acopf_mode: AcOpfMode = AcOpfMode.ACOPFstd,
                  pf_results: PowerFlowResults = None):
         """
         Optimal power flow options
         :param verbose:
         :param solver:
         :param time_grouping:
         :param zonal_grouping:
@@ -110,14 +111,16 @@
 
         self.max_vm = 1.0
 
         self.export_model_fname: Union[None, str] = export_model_fname
 
         self.generate_report = generate_report
 
+        self.acopf_mode = acopf_mode
+
         # IPS settings
         self.ips_method: SolverType = ips_method
         self.ips_tolerance = ips_tolerance
         self.ips_iterations = ips_iterations
         self.ips_trust_radius = ips_trust_radius
         self.ips_init_with_pf = ips_init_with_pf
         self.pf_results = pf_results
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 from GridCalEngine.Utils.NumericalMethods.ips import interior_point_solver, IpsFunctionReturn
 import GridCalEngine.Utils.NumericalMethods.autodiff as ad
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCalEngine.DataStructures.numerical_circuit import compile_numerical_circuit_at, NumericalCircuit
 from GridCalEngine.Simulations.PowerFlow.power_flow_worker import multi_island_pf_nc
 from GridCalEngine.Simulations.PowerFlow.power_flow_options import PowerFlowOptions
 from GridCalEngine.Simulations.OPF.opf_options import OptimalPowerFlowOptions
-from GridCalEngine.enumerations import ReactivePowerControlMode
+from GridCalEngine.enumerations import ReactivePowerControlMode, AcOpfMode
 from typing import Union
 from GridCalEngine.basic_structures import Vec, CxVec, IntVec, Logger
 from GridCalEngine.Simulations.OPF.NumericalMethods.ac_opf_derivatives import (x2var, var2x, eval_f,
                                                                                eval_g, eval_h,
                                                                                jacobians_and_hessians)
 
 
 def compute_autodiff_structures(x, mu, lmbda, compute_jac, compute_hess, admittances, Cg, R, X, Sd, slack, from_idx,
                                 to_idx, fdc, tdc, ndc, pq, pv, Pdcmax, V_U, V_L, P_U, P_L, tanmax, Q_U, Q_L, tapm_max,
                                 tapm_min, tapt_max, tapt_min, alltapm, alltapt, k_m, k_tau, c0, c1, c2, c_s, c_v, Sbase,
-                                rates, il, nll, ig, nig, Sg_undis, ctQ, h=1e-5) -> IpsFunctionReturn:
+                                rates, il, nll, ig, nig, Sg_undis, ctQ, acopf_mode, h=1e-5) -> IpsFunctionReturn:
     """
 
     :param x:
     :param mu:
     :param lmbda:
     :param compute_jac:
     :param compute_hess:
@@ -94,15 +94,15 @@
     ntapt = len(k_tau)
     npq = len(pq)
 
     alltapm0 = alltapm.copy()
     alltapt0 = alltapt.copy()
 
     _, _, _, _, _, _, _, _, tapm, tapt, _ = x2var(x, nVa=N, nVm=N, nPg=Ng, nQg=Ng, npq=npq,
-                                                  M=nll, ntapm=ntapm, ntapt=ntapt, ndc=ndc)
+                                                  M=nll, ntapm=ntapm, ntapt=ntapt, ndc=ndc, acopf_mode=acopf_mode)
 
     alltapm[k_m] = tapm
     alltapt[k_tau] = tapt
 
     admittances.modify_taps(alltapm0, alltapm, alltapt0, alltapt)
 
     Ybus = admittances.Ybus
@@ -159,15 +159,15 @@
                              S=Scalc, St=St, Sf=Sf)
 
 
 def compute_analytic_structures(x, mu, lmbda, compute_jac: bool, compute_hess: bool, admittances, Cg, R, X, Sd, slack,
                                 from_idx, to_idx, f_nd_dc, t_nd_dc, fdc, tdc, ndc, pq, pv, Pf_nondisp, Pdcmax, V_U, V_L,
                                 P_U, P_L, tanmax, Q_U, Q_L, tapm_max, tapm_min, tapt_max, tapt_min, alltapm, alltapt,
                                 k_m, k_tau, c0, c1, c2, c_s, c_v, Sbase, rates, il, nll, ig, nig, Sg_undis, ctQ,
-                                use_bound_slacks) -> IpsFunctionReturn:
+                                acopf_mode) -> IpsFunctionReturn:
     """
     A function that computes the optimization model for a NumericalCircuit object and returns the values of the
     equations and their derivatives computed analyitically
     :param x: State vector
     :param mu: Vector of mu multipliers
     :param lmbda: Vector of lambda multipliers
     :param compute_jac: Boolean that indicates if the Jacobians have to be calculated
@@ -224,54 +224,54 @@
     npq = len(pq)
 
     alltapm0 = alltapm.copy()
     alltapt0 = alltapt.copy()
 
     _, _, _, _, _, _, _, _, tapm, tapt, _ = x2var(x, nVa=N, nVm=N, nPg=Ng, nQg=Ng, npq=npq,
                                                   M=nll, ntapm=ntapm, ntapt=ntapt, ndc=ndc,
-                                                  use_bound_slacks=use_bound_slacks)
+                                                  acopf_mode=acopf_mode)
 
     alltapm[k_m] = tapm
     alltapt[k_tau] = tapt
 
     admittances.modify_taps(alltapm0, alltapm, alltapt0, alltapt)
 
     Ybus = admittances.Ybus
     Yf = admittances.Yf
     Yt = admittances.Yt
     Cf = admittances.Cf
     Ct = admittances.Ct
 
     f = eval_f(x=x, Cg=Cg, k_m=k_m, k_tau=k_tau, nll=nll, c0=c0, c1=c1, c2=c2, c_s=c_s, c_v=c_v,
-               ig=ig, npq=npq, ndc=ndc, Sbase=Sbase, use_bound_slacks=use_bound_slacks)
+               ig=ig, npq=npq, ndc=ndc, Sbase=Sbase, acopf_mode=acopf_mode)
     G, Scalc = eval_g(x=x, Ybus=Ybus, Yf=Yf, Cg=Cg, Sd=Sd, ig=ig, nig=nig, nll=nll, npq=npq, pv=pv, f_nd_dc=f_nd_dc,
                       t_nd_dc=t_nd_dc, fdc=fdc, tdc=tdc, Pf_nondisp=Pf_nondisp, k_m=k_m, k_tau=k_tau, Vm_max=V_U,
-                      Sg_undis=Sg_undis, slack=slack, use_bound_slacks=use_bound_slacks)
+                      Sg_undis=Sg_undis, slack=slack, acopf_mode=acopf_mode)
     H, Sf, St = eval_h(x=x, Yf=Yf, Yt=Yt, from_idx=from_idx, to_idx=to_idx, pq=pq, k_m=k_m, k_tau=k_tau, Vm_max=V_U,
                        Vm_min=V_L, Pg_max=P_U, Pg_min=P_L, Qg_max=Q_U, Qg_min=Q_L, tapm_max=tapm_max, tapm_min=tapm_min,
                        tapt_max=tapt_max, tapt_min=tapt_min, Pdcmax=Pdcmax,
-                       rates=rates, il=il, ig=ig, tanmax=tanmax, ctQ=ctQ, use_bound_slacks=use_bound_slacks)
+                       rates=rates, il=il, ig=ig, tanmax=tanmax, ctQ=ctQ, acopf_mode=acopf_mode)
 
     fx, Gx, Hx, fxx, Gxx, Hxx = jacobians_and_hessians(x=x, c1=c1, c2=c2, c_s=c_s, c_v=c_v, Cg=Cg, Cf=Cf, Ct=Ct, Yf=Yf,
                                                        Yt=Yt, Ybus=Ybus, Sbase=Sbase, il=il, ig=ig, slack=slack, pq=pq,
                                                        pv=pv, tanmax=tanmax, alltapm=alltapm, alltapt=alltapt, fdc=fdc,
                                                        tdc=tdc, k_m=k_m, k_tau=k_tau, mu=mu, lmbda=lmbda, R=R, X=X,
-                                                       F=from_idx, T=to_idx, ctQ=ctQ, use_bound_slacks=use_bound_slacks,
+                                                       F=from_idx, T=to_idx, ctQ=ctQ, acopf_mode=acopf_mode,
                                                        compute_jac=compute_jac, compute_hess=compute_hess)
 
     return IpsFunctionReturn(f=f, G=G, H=H,
                              fx=fx, Gx=Gx, Hx=Hx,
                              fxx=fxx, Gxx=Gxx, Hxx=Hxx,
                              S=Scalc, St=St, Sf=Sf)
 
 
 def evaluate_power_flow_debug(x, mu, lmbda, compute_jac, compute_hess, admittances, Cg, R, X, Sd, slack, from_idx,
                               to_idx, fdc, tdc, ndc, pq, pv, Pdcmax, V_U, V_L, P_U, P_L, tanmax, Q_U, Q_L, tapm_max,
                               tapm_min, tapt_max, tapt_min, alltapm, alltapt, k_m, k_tau, c0, c1, c2, c_s, c_v, Sbase,
-                              rates, il, nll, ig, nig, Sg_undis, ctQ, use_bound_slacks, h=1e-5) -> IpsFunctionReturn:
+                              rates, il, nll, ig, nig, Sg_undis, ctQ, acopf_mode, h=1e-5) -> IpsFunctionReturn:
     """
 
     :param x: State vector
     :param mu: Vector of mu multipliers
     :param lmbda: Vector of lambda multipliers
     :param compute_jac: Boolean that indicates if the Jacobians have to be calculated
     :param compute_hess: Boolean that indicates if the Hessians have to be calculated
@@ -322,15 +322,15 @@
     :return: return the resulting error between the autodif and the analytic derivation
     """
 
     mats_analytic = compute_analytic_structures(x, mu, lmbda, compute_jac, compute_hess, admittances, Cg, R, X, Sd,
                                                 slack, from_idx, to_idx, fdc, tdc, ndc, pq, pv, Pdcmax, V_U, V_L, P_U,
                                                 P_L, tanmax, Q_U, Q_L, tapm_max, tapm_min, tapt_max, tapt_min, alltapm,
                                                 alltapt, k_m, k_tau, c0, c1, c2, c_s, c_v, Sbase, rates, il, nll, ig,
-                                                nig, Sg_undis, ctQ, use_bound_slacks=use_bound_slacks)
+                                                nig, Sg_undis, ctQ, acopf_mode=acopf_mode)
 
     mats_finite = compute_autodiff_structures(x, mu, lmbda, compute_jac, compute_hess, admittances, Cg, R, X, Sd,
                                               slack, from_idx, to_idx, fdc, tdc, ndc, pq, pv, Pdcmax, V_U, V_L, P_U,
                                               P_L, tanmax, Q_U, Q_L, tapm_max, tapm_min, tapt_max, tapt_min, alltapm,
                                               alltapt, k_m, k_tau, c0, c1, c2, c_s, c_v, Sbase, rates, il, nll, ig,
                                               nig, Sg_undis, ctQ, h=h)
 
@@ -402,15 +402,15 @@
         self.sl_vmin: Vec = np.zeros(nbus)
         self.error: float = 0.0
         self.converged: bool = False
         self.iterations: int = 0
 
     def merge(self, other: "NonlinearOPFResults",
               bus_idx: IntVec, br_idx: IntVec, il_idx: IntVec, gen_idx: IntVec, hvdc_idx: IntVec,
-              use_bound_slacks):
+              acopf_mode):
         """
 
         :param other:
         :param bus_idx:
         :param br_idx:
         :param gen_idx:
         :param hvdc_idx:
@@ -426,15 +426,15 @@
         self.Pcost[gen_idx] = other.Pcost
         self.tap_module[br_idx] = other.tap_module
         self.tap_phase[br_idx] = other.tap_phase
         self.hvdc_Pf[hvdc_idx] = other.hvdc_Pf
         self.hvdc_loading[hvdc_idx] = other.hvdc_loading
         self.lam_p[bus_idx] = other.lam_p
         self.lam_q[bus_idx] = other.lam_q
-        if use_bound_slacks:
+        if acopf_mode == AcOpfMode.ACOPFslacks:
             self.sl_sf[il_idx] = other.sl_sf
             self.sl_st[il_idx] = other.sl_st
             self.sl_vmax[bus_idx] = other.sl_vmax
             self.sl_vmin[bus_idx] = other.sl_vmin
         self.error: float = 0.0
         self.converged: bool = False
         self.iterations: int = 0
@@ -453,15 +453,14 @@
                           opf_options: OptimalPowerFlowOptions,
                           debug: bool = False,
                           use_autodiff: bool = False,
                           pf_init: bool = False,
                           Sbus_pf: Union[CxVec, None] = None,
                           voltage_pf: Union[CxVec, None] = None,
                           plot_error: bool = False,
-                          use_bound_slacks: bool = True,
                           logger: Logger = Logger()) -> NonlinearOPFResults:
     """
 
     :param nc: NumericalCircuit
     :param pf_options: PowerFlowOptions
     :param opf_options: OptimalPowerFlowOptions
     :param debug: if true, the jacobians, hessians, etc are checked against finite difeerence versions of them
@@ -549,15 +548,15 @@
     Pf_nondisp = nc.hvdc_data.Pset[hvdc_nondisp_idx]
 
     n_disp_hvdc = len(hvdc_disp_idx)
     f_disp_hvdc = nc.hvdc_data.F[hvdc_disp_idx]
     t_disp_hvdc = nc.hvdc_data.T[hvdc_disp_idx]
     P_hvdc_max = nc.hvdc_data.rate[hvdc_disp_idx]
 
-    if use_bound_slacks:
+    if opf_options.acopf_mode == AcOpfMode.ACOPFslacks:
         nsl = 2 * npq + 2 * n_br_mon
         # Slack relaxations for constraints
         c_s = 1 * np.power(nc.branch_data.overload_cost[br_mon_idx] + 1e-9, 1.0)  # Cost squared since the slack is also squared
         c_v = 1 * nc.bus_data.cost_v[pq] + 1e-9
         sl_sf0 = np.ones(n_br_mon)
         sl_st0 = np.ones(n_br_mon)
         sl_vmax0 = np.ones(npq)
@@ -568,14 +567,15 @@
         c_s = np.array([])
         c_v = np.array([])
         sl_sf0 = np.array([])
         sl_st0 = np.array([])
         sl_vmax0 = np.array([])
         sl_vmin0 = np.array([])
 
+
     # Number of equalities: Nodal power balances, the voltage module of slack and pv buses and the slack reference
     NE = 2 * nbus + n_slack + npv
 
     # Number of inequalities: Line ratings, max and min angle of buses, voltage module range and
 
     if pf_options.control_Q == ReactivePowerControlMode.NoControl:
         NI = 2 * n_br_mon + 2 * npq + 4 * n_gen_disp + 2 * ntapm + 2 * ntapt + 2 * n_disp_hvdc + nsl  # No Reactive constraint (power curve)
@@ -625,54 +625,54 @@
         # run the solver with the function that checks the derivatives
         # against their finite differences equivalent
         result = interior_point_solver(x0=x0, n_x=NV, n_eq=NE, n_ineq=NI,
                                        func=evaluate_power_flow_debug,
                                        arg=(admittances, Cg, Sd, slack, from_idx, to_idx,
                                             pq, pv, Va_max, Va_min, Vm_max, Vm_min, Pg_max, Pg_min,
                                             Qg_max, Qg_min, tapm_max, tapm_min, tapt_max, tapt_min, alltapm, alltapt,
-                                            k_m, k_tau, k_mtau, c0, c1, c2, Sbase, rates, br_mon_idx, gen_disp_idx, nig, Sg_undis,
-                                            pf_options.control_Q, use_bound_slacks),
+                                            k_m, k_tau, k_mtau, c0, c1, c2, Sbase, rates, br_mon_idx, gen_disp_idx, nig,
+                                            Sg_undis, pf_options.control_Q, opf_options.acopf_mode),
                                        verbose=opf_options.verbose,
                                        max_iter=opf_options.ips_iterations,
                                        tol=opf_options.ips_tolerance,
                                        trust=opf_options.ips_trust_radius)
 
     else:
         if use_autodiff:
             # run the solver with the autodiff derivatives
             result = interior_point_solver(x0=x0, n_x=NV, n_eq=NE, n_ineq=NI,
                                            func=compute_autodiff_structures,
                                            arg=(admittances, Cg, Sd, slack, from_idx, to_idx, pq, pv,
                                                 Va_max, Va_min, Vm_max, Vm_min, Pg_max, Pg_min, Qg_max, Qg_min,
                                                 tapm_max, tapm_min, tapt_max, tapt_min, k_m, k_tau, k_mtau,
                                                 c0, c1, c2, Sbase, rates, br_mon_idx, gen_disp_idx, nig, Sg_undis,
-                                                use_bound_slacks, 1e-5),
+                                                opf_options.acopf_mode, 1e-5),
                                            verbose=opf_options.verbose,
                                            max_iter=opf_options.ips_iterations,
                                            tol=opf_options.ips_tolerance,
                                            trust=opf_options.ips_trust_radius)
         else:
             # run the solver with the analytic derivatives
             result = interior_point_solver(x0=x0, n_x=NV, n_eq=NE, n_ineq=NI,
                                            func=compute_analytic_structures,
                                            arg=(admittances, Cg, R, X, Sd, slack, from_idx, to_idx, f_nd_hvdc, t_nd_hvdc,
                                                 f_disp_hvdc, t_disp_hvdc, n_disp_hvdc, pq, pv, Pf_nondisp, P_hvdc_max, Vm_max, Vm_min, Pg_max,
                                                 Pg_min, tanmax, Qg_max, Qg_min, tapm_max, tapm_min, tapt_max, tapt_min,
                                                 alltapm, alltapt, k_m, k_tau, c0, c1, c2, c_s, c_v, Sbase, rates, br_mon_idx,
-                                                n_br_mon, gen_disp_idx, nig, Sg_undis, pf_options.control_Q, use_bound_slacks),
+                                                n_br_mon, gen_disp_idx, nig, Sg_undis, pf_options.control_Q, opf_options.acopf_mode),
                                            verbose=opf_options.verbose,
                                            max_iter=opf_options.ips_iterations,
                                            tol=opf_options.ips_tolerance,
                                            trust=opf_options.ips_trust_radius)
 
     # convert the solution to the problem variables
     (Va, Vm, Pg_dis, Qg_dis, sl_sf, sl_st,
      sl_vmax, sl_vmin, tapm, tapt, Pfdc) = x2var(result.x, nVa=nbus, nVm=nbus, nPg=n_gen_disp, nQg=n_gen_disp,
                                                  M=n_br_mon, npq=npq, ntapm=ntapm, ntapt=ntapt, ndc=n_disp_hvdc,
-                                                 use_bound_slacks=use_bound_slacks)
+                                                 acopf_mode=opf_options.acopf_mode)
 
     # Save Results DataFrame for tests
     # pd.DataFrame(Va).transpose().to_csv('pegase89resth.csv')
     # pd.DataFrame(Vm).transpose().to_csv('pegase89resV.csv')
     # pd.DataFrame(Pg_dis).transpose().to_csv('pegase89resP.csv')
     # pd.DataFrame(Qg_dis).transpose().to_csv('pegase89resQ.csv')
 
@@ -783,15 +783,15 @@
             if muz_t >= 1e-3:
                 logger.add_warning('HVDC rating "to" multipliers did not reach the tolerance',
                                    device_property="mu · z",
                                    device=str(link),
                                    value=str(muz_t),
                                    expected_value='< 1e-3')
 
-        if use_bound_slacks:
+        if opf_options.acopf_mode == AcOpfMode.ACOPFslacks:
             for k in range(n_br_mon):
                 if sl_sf[k] > opf_options.ips_tolerance:
                     logger.add_warning('Branch overload in the from sense',
                                        device=str(br_mon_idx[k]),
                                        device_property="Slack",
                                        value=str(sl_sf[k]),
                                        expected_value=f'< {opf_options.ips_tolerance}')
@@ -839,15 +839,14 @@
                       t_idx: Union[None, int] = None,
                       debug: bool = False,
                       use_autodiff: bool = False,
                       pf_init=False,
                       Sbus_pf0: Union[CxVec, None] = None,
                       voltage_pf0: Union[CxVec, None] = None,
                       plot_error: bool = False,
-                      use_bound_slacks: bool = True,
                       logger: Logger = Logger()) -> NonlinearOPFResults:
     """
     Run optimal power flow for a MultiCircuit
     :param grid: MultiCircuit
     :param opf_options: OptimalPowerFlowOptions
     :param pf_options: PowerFlowOptions
     :param t_idx: Time index
@@ -894,15 +893,14 @@
                                            pf_options=pf_options,
                                            debug=debug,
                                            use_autodiff=use_autodiff,
                                            pf_init=pf_init,
                                            Sbus_pf=Sbus_pf[island.original_bus_idx],
                                            voltage_pf=voltage_pf[island.original_bus_idx],
                                            plot_error=plot_error,
-                                           use_bound_slacks=use_bound_slacks,
                                            logger=logger)
 
         if pf_init and not island_res.converged:
             # if we were initializing with the power flow results and it failed, try without power flow initialization
 
             logger.add_warning(msg="Trying flat start because power flow initialization did not converge")
 
@@ -911,24 +909,23 @@
                                                pf_options=pf_options,
                                                debug=debug,
                                                use_autodiff=use_autodiff,
                                                pf_init=False,
                                                Sbus_pf=Sbus_pf[island.original_bus_idx],
                                                voltage_pf=voltage_pf[island.original_bus_idx],
                                                plot_error=plot_error,
-                                               use_bound_slacks=use_bound_slacks,
                                                logger=logger)
 
         results.merge(other=island_res,
                       bus_idx=island.bus_data.original_idx,
                       br_idx=island.branch_data.original_idx,
                       il_idx=island.branch_data.get_monitor_enabled_indices(),
                       gen_idx=island.generator_data.original_idx,
                       hvdc_idx=island.hvdc_data.original_idx,
-                      use_bound_slacks=use_bound_slacks)
+                      acopf_mode=opf_options.acopf_mode)
         if i > 0:
             results.error = max(results.error, island_res.error)
             results.iterations = max(results.iterations, island_res.iterations)
             results.converged = results.converged and island_res.converged if i > 0 else island_res.converged
         else:
             results.error = island_res.error
             results.iterations = island_res.iterations
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 from scipy import sparse as sp
 from scipy.sparse import csc_matrix as csc
 from scipy.sparse import lil_matrix
 
 from GridCalEngine.Utils.Sparse.csc import diags
 from typing import Tuple, Union
 from GridCalEngine.basic_structures import Vec, CxVec, IntVec, csr_matrix, csc_matrix
-from GridCalEngine.enumerations import ReactivePowerControlMode
+from GridCalEngine.enumerations import ReactivePowerControlMode, AcOpfMode
 
 
 def x2var(x: Vec,
           nVa: int,
           nVm: int,
           nPg: int,
           nQg: int,
           npq: int,
           M: int,
           ntapm: int,
           ntapt: int,
           ndc: int,
-          use_bound_slacks: bool) -> Tuple[Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec]:
+          acopf_mode: AcOpfMode) -> Tuple[Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec, Vec]:
     """
     Convert the x solution vector to its composing variables
     :param x: solution vector
     :param nVa: number of voltage angle vars
     :param nVm: number of voltage module vars
     :param nPg: number of generator active power vars
     :param nQg: number of generator reactive power vars
@@ -64,15 +64,15 @@
     Pg = x[a: b]
     a = b
     b += nQg
 
     Qg = x[a: b]
     a = b
 
-    if use_bound_slacks:
+    if acopf_mode == AcOpfMode.ACOPFslacks:
         b += M
 
         sl_sf = x[a: b]
         a = b
         b += M
 
         sl_st = x[a: b]
@@ -406,19 +406,20 @@
             dSbusdmdva, dSfdmdva, dStdmdva,
             dSbusdmdt, dSfdmdt, dStdmdt,
             dSbusdtdt, dSfdtdt, dStdtdt,
             dSbusdtdvm, dSfdtdvm, dStdtdvm,
             dSbusdtdva, dSfdtdva, dStdtdva)
 
 
-def eval_f(x: Vec, Cg: csr_matrix, k_m: Vec, k_tau: Vec, nll: int, c0: Vec, c1: Vec, c2: Vec, c_s: Vec,
-           c_v: Vec, ig: Vec, npq: int, ndc: int, Sbase: float, use_bound_slacks: bool) -> float:
+def eval_f(x: Vec, Cg: csc_matrix, k_m: Vec, k_tau: Vec, nll: int, c0: Vec, c1: Vec, c2: Vec, c_s: Vec,
+           c_v: Vec, ig: Vec, npq: int, ndc: int, Sbase: float, acopf_mode: AcOpfMode) -> float:
     """
     Calculates the value of the objective function at the current state (given by x)
     :param x: State vector
+
     :param Cg: Generation connectivity matrix
     :param k_m: List with the index of the module controlled transformers
     :param k_tau: List with the index of the phase controlled transformers
     :param nll: Number of monitored lines
     :param c0: Base cost of generators
     :param c1: Linear cost of generators
     :param c2: Quadratic cost of generators
@@ -433,25 +434,25 @@
     N, _ = Cg.shape  # Check
     Ng = len(ig)
     ntapm = len(k_m)
     ntapt = len(k_tau)
 
     _, _, Pg, Qg, sl_sf, sl_st, sl_vmax, sl_vmin, _, _, _ = x2var(x, nVa=N, nVm=N, nPg=Ng, nQg=Ng, npq=npq,
                                                                   M=nll, ntapm=ntapm, ntapt=ntapt, ndc=ndc,
-                                                                  use_bound_slacks=use_bound_slacks)
+                                                                  acopf_mode=acopf_mode)
     # Obj. function:  Active power generation costs plus overloads and voltage deviation penalties
     fval = 1e-4 * (np.sum((c0 + c1 * Pg * Sbase + c2 * np.power(Pg * Sbase, 2)))
                    + np.sum(c_s * (sl_sf + sl_st)) + np.sum(c_v * (sl_vmax + sl_vmin)))
 
     return fval
 
 
-def eval_g(x: Vec, Ybus: csr_matrix, Yf: csr_matrix, Cg: csr_matrix, Sd: CxVec, ig: Vec, nig: Vec, nll: int, npq: int,
+def eval_g(x: Vec, Ybus: csc_matrix, Yf: csc_matrix, Cg: csc_matrix, Sd: CxVec, ig: Vec, nig: Vec, nll: int, npq: int,
            pv: Vec, f_nd_dc: Vec, t_nd_dc: Vec, fdc: Vec, tdc: Vec, Pf_nondisp: Vec, k_m: Vec, k_tau: Vec, Vm_max: Vec,
-           Sg_undis: CxVec, slack: Vec, use_bound_slacks: bool) -> Tuple[Vec, Vec]:
+           Sg_undis: CxVec, slack: Vec, acopf_mode: AcOpfMode) -> Tuple[Vec, Vec]:
     """
     Calculates the equality constraints at the current state (given by x)
     :param x: State vector
     :param Ybus: Bus admittance matrix
     :param Yf: From admittance matrix
     :param Cg: Generators connectivity matrix
     :param Sd: Loads vector
@@ -477,15 +478,15 @@
     Ng = len(ig)
     ntapm = len(k_m)
     ntapt = len(k_tau)
     ndc = len(fdc)
 
     va, vm, Pg_dis, Qg_dis, sl_sf, sl_st, sl_vmax, sl_vmin, _, _, Pfdc = x2var(x, nVa=N, nVm=N, nPg=Ng, nQg=Ng, npq=npq,
                                                                                M=nll, ntapm=ntapm, ntapt=ntapt, ndc=ndc,
-                                                                               use_bound_slacks=use_bound_slacks)
+                                                                               acopf_mode=acopf_mode)
 
     V = vm * np.exp(1j * va)
     S = V * np.conj(Ybus @ V)
     S_dispatch = Cg[:, ig] @ (Pg_dis + 1j * Qg_dis)  # Variable generation
     S_undispatch = Cg[:, nig] @ Sg_undis  # Fixed generation
     dS = S + Sd - S_dispatch - S_undispatch  # Nodal power balance
 
@@ -497,18 +498,18 @@
         dS[t_nd_dc[nd_link]] -= Pf_nondisp[nd_link]
 
     gval = np.r_[dS.real, dS.imag, va[slack], vm[pv] - Vm_max[pv]]
 
     return gval, S
 
 
-def eval_h(x: Vec, Yf: csr_matrix, Yt: csr_matrix, from_idx: Vec, to_idx: Vec, pq: Vec, k_m: Vec, k_tau: Vec,
+def eval_h(x: Vec, Yf: csc_matrix, Yt: csc_matrix, from_idx: Vec, to_idx: Vec, pq: Vec, k_m: Vec, k_tau: Vec,
            Vm_max: Vec, Vm_min: Vec, Pg_max: Vec, Pg_min: Vec, Qg_max: Vec, Qg_min: Vec, tapm_max: Vec,
            tapm_min: Vec, tapt_max: Vec, tapt_min: Vec, Pdcmax: Vec, rates: Vec, il: Vec, ig: Vec,
-           tanmax: Vec, ctQ: ReactivePowerControlMode, use_bound_slacks: bool) -> Tuple[Vec, CxVec, CxVec]:
+           tanmax: Vec, ctQ: ReactivePowerControlMode, acopf_mode: AcOpfMode) -> Tuple[Vec, CxVec, CxVec]:
     """
     Calculates the inequality constraints at the current state (given by x)
     :param x: State vector
     :param Yf: From admittance matrix
     :param Yt: To admittance matrix
     :param from_idx: Vector with the indices of the 'from' buses for each line
     :param to_idx: Vector with the indices of the 'from' buses for each line
@@ -541,28 +542,28 @@
     ntapt = len(k_tau)
     ndc = len(Pdcmax)
     npq = len(pq)
     nll = len(il)
 
     va, vm, Pg, Qg, sl_sf, sl_st, sl_vmax, sl_vmin, tapm, tapt, Pfdc = x2var(x, nVa=N, nVm=N, nPg=Ng, nQg=Ng, npq=npq,
                                                                              M=nll, ntapm=ntapm, ntapt=ntapt, ndc=ndc,
-                                                                             use_bound_slacks=use_bound_slacks)
+                                                                             acopf_mode=acopf_mode)
 
     V = vm * np.exp(1j * va)
     Sf = V[from_idx[il]] * np.conj(Yf[il, :] @ V)
     St = V[to_idx[il]] * np.conj(Yt[il, :] @ V)
 
     Sftot = V[from_idx] * np.conj(Yf @ V)
     Sttot = V[to_idx] * np.conj(Yt @ V)
 
     Sf2 = np.conj(Sf) * Sf
     St2 = np.conj(St) * St
     rates2 = np.power(rates[il], 2.0)
 
-    if use_bound_slacks:
+    if acopf_mode == AcOpfMode.ACOPFslacks:
         hval = np.r_[
             Sf2.real - rates2 - sl_sf,  # rates "lower limit"
             St2.real - rates2 - sl_st,  # rates "upper limit"
             vm[pq] - Vm_max[pq] - sl_vmax,  # voltage module upper limit
             Pg - Pg_max[ig],  # generator P upper limits
             Qg - Qg_max[ig],  # generator Q upper limits
             Vm_min[pq] - vm[pq] - sl_vmin,  # voltage module lower limit
@@ -598,19 +599,19 @@
 
     if ndc != 0:
         hval = np.r_[hval, Pfdc - Pdcmax, - Pdcmax - Pfdc]
 
     return hval, Sftot, Sttot
 
 
-def jacobians_and_hessians(x: Vec, c1: Vec, c2: Vec, c_s: Vec, c_v: Vec, Cg: csr_matrix, Cf: csc, Ct: csc,
-                           Yf: csr_matrix, Yt: csr_matrix, Ybus: csr_matrix, Sbase: float, il: Vec, ig: Vec,
+def jacobians_and_hessians(x: Vec, c1: Vec, c2: Vec, c_s: Vec, c_v: Vec, Cg: csc_matrix, Cf: csc, Ct: csc,
+                           Yf: csc_matrix, Yt: csc_matrix, Ybus: csc_matrix, Sbase: float, il: Vec, ig: Vec,
                            slack: Vec, pq: Vec, pv: Vec, tanmax: Vec, alltapm: Vec, alltapt: Vec, fdc: Vec, tdc: Vec,
                            k_m: Vec, k_tau: Vec, mu, lmbda, R: Vec, X: Vec, F: Vec, T: Vec,
-                           ctQ: ReactivePowerControlMode, use_bound_slacks: bool, compute_jac: bool,
+                           ctQ: ReactivePowerControlMode, acopf_mode: AcOpfMode, compute_jac: bool,
                            compute_hess: bool) -> Tuple[Vec, csc, csc, csc, csc, csc]:
 
     """
     Calculates the jacobians and hessians of the objective function and the equality and inequality constraints
     at the current state given by x
     :param x: State vector
     :param c1: Linear cost of each generator
@@ -659,17 +660,17 @@
     if ctQ != ReactivePowerControlMode.NoControl:
         nqct = Ng
     else:
         nqct = 0
 
     va, vm, Pg, Qg, sl_sf, sl_st, sl_vmax, sl_vmin, tapm, tapt, Pfdc = x2var(x, nVa=N, nVm=N, nPg=Ng, nQg=Ng, npq=npq,
                                                                              M=M, ntapm=ntapm, ntapt=ntapt, ndc=ndc,
-                                                                             use_bound_slacks=use_bound_slacks)
+                                                                             acopf_mode=acopf_mode)
 
-    if use_bound_slacks:
+    if acopf_mode == AcOpfMode.ACOPFslacks:
         nsl = 2 * npq + 2 * M  # Number of slacks
     else:
         nsl = 0
 
     npfvar = 2 * N + 2 * Ng  # Number of variables of the typical power flow (V, th, P, Q). Used to ease readability
 
     V = vm * np.exp(1j * va)
@@ -685,15 +686,15 @@
 
         # OBJECTIVE FUNCTION GRAD --------------------------------------------------------------------------------------
 
         fx = np.zeros(NV)
 
         fx[2 * N: 2 * N + Ng] = (2 * c2 * Pg * (Sbase * Sbase) + c1 * Sbase) * 1e-4
 
-        if use_bound_slacks:
+        if acopf_mode == AcOpfMode.ACOPFslacks:
             fx[npfvar: npfvar + M] = c_s
             fx[npfvar + M: npfvar + 2 * M] = c_s
             fx[npfvar + 2 * M: npfvar + 2 * M + npq] = c_v
             fx[npfvar + 2 * M + npq: npfvar + 2 * M + 2 * npq] = c_v
 
         # EQUALITY CONSTRAINTS GRAD ------------------------------------------------------------------------------------
         """
@@ -843,15 +844,15 @@
         Stva = (1j * (ItCJmat @ Ct[il, :] @ Vmat - Vtmat @ np.conj(Yt[il, :]) @ np.conj(Vmat)))
 
         Hpu = sp.hstack([lil_matrix((Ng, 2 * N)), diags(np.ones(Ng)), lil_matrix((Ng, NV - 2 * N - Ng))])
         Hpl = sp.hstack([lil_matrix((Ng, 2 * N)), diags(- np.ones(Ng)), lil_matrix((Ng, NV - 2 * N - Ng))])
         Hqu = sp.hstack([lil_matrix((Ng, 2 * N + Ng)), diags(np.ones(Ng)), lil_matrix((Ng, NV - 2 * N - 2 * Ng))])
         Hql = sp.hstack([lil_matrix((Ng, 2 * N + Ng)), diags(- np.ones(Ng)), lil_matrix((Ng, NV - 2 * N - 2 * Ng))])
 
-        if use_bound_slacks:
+        if acopf_mode == AcOpfMode.ACOPFslacks:
             Hvu = sp.hstack([lil_matrix((npq, N)), diags(np.ones(npq)), lil_matrix((npq, 2 * Ng + 2 * M)),
                              diags(- np.ones(npq)), lil_matrix((npq, npq + ntapm + ntapt + ndc))])
 
             Hvl = sp.hstack([lil_matrix((npq, N)), diags(- np.ones(npq)), lil_matrix((npq, 2 * Ng + 2 * M + npq)),
                              diags(- np.ones(npq)), lil_matrix((npq, ntapm + ntapt + ndc))])
 
             Hslsf = sp.hstack([lil_matrix((M, npfvar)), diags(- np.ones(M)),
@@ -880,15 +881,15 @@
             Sftapt = dSfdt[il, :].copy()
             Sttapm = dStdm[il, :].copy()
             Sttapt = dStdt[il, :].copy()
 
             SfX = sp.hstack([Sfva, Sfvm, lil_matrix((M, 2 * Ng + nsl)), Sftapm, Sftapt, lil_matrix((M, ndc))])
             StX = sp.hstack([Stva, Stvm, lil_matrix((M, 2 * Ng + nsl)), Sttapm, Sttapt, lil_matrix((M, ndc))])
 
-            if use_bound_slacks:
+            if acopf_mode == AcOpfMode.ACOPFslacks:
                 HSf = 2 * (Sfmat.real @ SfX.real + Sfmat.imag @ SfX.imag) + Hslsf
                 HSt = 2 * (Stmat.real @ StX.real + Stmat.imag @ StX.imag) + Hslst
             else:
                 HSf = 2 * (Sfmat.real @ SfX.real + Sfmat.imag @ SfX.imag)
                 HSt = 2 * (Stmat.real @ StX.real + Stmat.imag @ StX.imag)
 
             if ntapm != 0:
@@ -921,15 +922,15 @@
             Htapml = lil_matrix((ntapm, NV))
             Htaptu = lil_matrix((ntapt, NV))
             Htaptl = lil_matrix((ntapt, NV))
 
             SfX = sp.hstack([Sfva, Sfvm, lil_matrix((M, 2 * Ng + nsl + ndc))])
             StX = sp.hstack([Stva, Stvm, lil_matrix((M, 2 * Ng + nsl + ndc))])
 
-            if use_bound_slacks:
+            if acopf_mode == AcOpfMode.ACOPFslacks:
                 HSf = 2 * (Sfmat.real @ SfX.real + Sfmat.imag @ SfX.imag) + Hslsf
                 HSt = 2 * (Stmat.real @ StX.real + Stmat.imag @ StX.imag) + Hslst
             else:
                 HSf = 2 * (Sfmat.real @ SfX.real + Sfmat.imag @ SfX.imag)
                 HSt = 2 * (Stmat.real @ StX.real + Stmat.imag @ StX.imag)
 
         if ctQ != ReactivePowerControlMode.NoControl:
```

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ATC/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/__init__.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py` & `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/setup.py` & `GridCalEngine-5.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.4/PKG-INFO` & `GridCalEngine-5.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCalEngine
-Version: 5.1.4
+Version: 5.1.5
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```

