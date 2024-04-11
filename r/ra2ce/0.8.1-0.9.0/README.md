# Comparing `tmp/ra2ce-0.8.1.tar.gz` & `tmp/ra2ce-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ra2ce-0.8.1.tar", max compression
+gzip compressed data, was "ra2ce-0.9.0.tar", max compression
```

## Comparing `ra2ce-0.8.1.tar` & `ra2ce-0.9.0.tar`

### file list

```diff
@@ -1,153 +1,155 @@
--rw-r--r--   0        0        0      877 2024-03-20 13:58:22.944678 ra2ce-0.8.1/LICENSE
--rw-r--r--   0        0        0     3677 2024-03-20 13:58:23.835281 ra2ce-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       23 2024-03-20 13:58:23.835281 ra2ce-0.8.1/ra2ce/__init__.py
--rw-r--r--   0        0        0     2098 2024-03-20 13:58:23.835281 ra2ce-0.8.1/ra2ce/__main__.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.835281 ra2ce-0.8.1/ra2ce/analysis/__init__.py
--rw-r--r--   0        0        0     2312 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_collection.py
--rw-r--r--   0        0        0        2 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/__init__.py
--rw-r--r--   0        0        0     7114 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/analysis_config_data.py
--rw-r--r--   0        0        0    12833 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/analysis_config_data_reader.py
--rw-r--r--   0        0        0     4551 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/analysis_config_data_validator.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/__init__.py
--rw-r--r--   0        0        0      175 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/analysis_direct_enum.py
--rw-r--r--   0        0        0      481 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/analysis_indirect_enum.py
--rw-r--r--   0        0        0      537 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/damage_curve_enum.py
--rw-r--r--   0        0        0      160 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/event_type_enum.py
--rw-r--r--   0        0        0      173 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/loss_type_enum.py
--rw-r--r--   0        0        0      217 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/risk_calculation_mode_enum.py
--rw-r--r--   0        0        0      165 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/weighing_enum.py
--rw-r--r--   0        0        0      687 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/README.md
--rw-r--r--   0        0        0     3990 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_config_wrapper.py
--rw-r--r--   0        0        0     8697 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_factory.py
--rw-r--r--   0        0        0     1874 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_input_wrapper.py
--rw-r--r--   0        0        0     1794 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_protocol.py
--rw-r--r--   0        0        0     1485 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_result_wrapper.py
--rw-r--r--   0        0        0     3351 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/analysis_result_wrapper_exporter.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/__init__.py
--rw-r--r--   0        0        0     1349 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/analysis_direct_protocol.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage/__init__.py
--rw-r--r--   0        0        0     5652 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage/damage_fraction_uniform.py
--rw-r--r--   0        0        0     6461 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage/damage_function_road_type_lane.py
--rw-r--r--   0        0        0     2806 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage/manual_damage_functions.py
--rw-r--r--   0        0        0     4611 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage/max_damage.py
--rw-r--r--   0        0        0      229 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/__init__.py
--rw-r--r--   0        0        0    17670 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/damage_network_base.py
--rw-r--r--   0        0        0     2895 2024-03-20 13:58:23.850909 ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/damage_network_events.py
--rw-r--r--   0        0        0    13051 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/damage_network_return_periods.py
--rw-r--r--   0        0        0      889 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/risk_utils.py
--rw-r--r--   0        0        0     4720 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/direct/direct_damage.py
--rw-r--r--   0        0        0    39764 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/direct/direct_lookup.py
--rw-r--r--   0        0        0     5771 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/direct/direct_utils.py
--rw-r--r--   0        0        0    19706 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/direct/effectiveness_measures.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/direct/readme.txt
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/__init__.py
--rw-r--r--   0        0        0     1509 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/analysis_indirect_protocol.py
--rw-r--r--   0        0        0    12883 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/losses.py
--rw-r--r--   0        0        0    11986 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_isolated_locations.py
--rw-r--r--   0        0        0     8541 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_losses.py
--rw-r--r--   0        0        0     6773 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_origin_closest_destination.py
--rw-r--r--   0        0        0    17649 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_origin_destination.py
--rw-r--r--   0        0        0     5869 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_redundancy.py
--rw-r--r--   0        0        0     4607 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/optimal_route_origin_closest_destination.py
--rw-r--r--   0        0        0     9406 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/optimal_route_origin_destination.py
--rw-r--r--   0        0        0    43460 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/origin_closest_destination.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/readme.txt
--rw-r--r--   0        0        0     8086 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/single_link_losses.py
--rw-r--r--   0        0        0     4707 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/single_link_redundancy.py
--rw-r--r--   0        0        0      220 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/__init__.py
--rw-r--r--   0        0        0     3389 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/accumulated_traffic_dataclass.py
--rw-r--r--   0        0        0     4072 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/equity_analysis.py
--rw-r--r--   0        0        0     1227 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/README.md
--rw-r--r--   0        0        0     2983 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis.py
--rw-r--r--   0        0        0     4123 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_base.py
--rw-r--r--   0        0        0     3025 2024-03-20 13:58:23.866522 ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_factory.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/__init__.py
--rw-r--r--   0        0        0      511 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/length_weighing_analysis.py
--rw-r--r--   0        0        0      401 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/README.md
--rw-r--r--   0        0        0     1257 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/time_weighing_analysis.py
--rw-r--r--   0        0        0      869 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_factory.py
--rw-r--r--   0        0        0      880 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_protocol.py
--rw-r--r--   0        0        0      777 2024-03-20 13:58:23.835281 ra2ce-0.8.1/ra2ce/analysis/README.md
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/configuration/__init__.py
--rw-r--r--   0        0        0     1391 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/configuration/config_data_protocol.py
--rw-r--r--   0        0        0     2060 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/configuration/config_wrapper_protocol.py
--rw-r--r--   0        0        0     1663 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/configuration/ini_configuration_reader_protocol.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/io/__init__.py
--rw-r--r--   0        0        0       75 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/io/readers/__init__.py
--rw-r--r--   0        0        0     1321 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/io/readers/file_reader_protocol.py
--rw-r--r--   0        0        0     1579 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/io/readers/graph_pickle_reader.py
--rw-r--r--   0        0        0      529 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/io/README.md
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/io/writers/__init__.py
--rw-r--r--   0        0        0     1361 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/io/writers/ra2ce_exporter_protocol.py
--rw-r--r--   0        0        0      718 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/README.md
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/validation/__init__.py
--rw-r--r--   0        0        0     1318 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/validation/ra2ce_validator_protocol.py
--rw-r--r--   0        0        0      466 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/validation/README.md
--rw-r--r--   0        0        0     1731 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/common/validation/validation_report.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/configuration/__init__.py
--rw-r--r--   0        0        0     5500 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/configuration/config_factory.py
--rw-r--r--   0        0        0     2659 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/configuration/config_wrapper.py
--rw-r--r--   0        0        0     2106 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/configuration/ra2ce_enum_base.py
--rw-r--r--   0        0        0      245 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/configuration/README.md
--rw-r--r--   0        0        0       44 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/network/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/network/exporters/__init__.py
--rw-r--r--   0        0        0     1812 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/network/exporters/geodataframe_network_exporter.py
--rw-r--r--   0        0        0     1778 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/network/exporters/json_exporter.py
--rw-r--r--   0        0        0     2169 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/network/exporters/multi_graph_network_exporter.py
--rw-r--r--   0        0        0     2918 2024-03-20 13:58:23.882146 ra2ce-0.8.1/ra2ce/network/exporters/network_exporter_base.py
--rw-r--r--   0        0        0     2186 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/exporters/network_exporter_factory.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/graph_files/__init__.py
--rw-r--r--   0        0        0     1077 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/graph_files/graph_file.py
--rw-r--r--   0        0        0     5753 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/graph_files/graph_files_collection.py
--rw-r--r--   0        0        0      951 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/graph_files/graph_files_protocol.py
--rw-r--r--   0        0        0      966 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/graph_files/network_file.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/__init__.py
--rw-r--r--   0        0        0     2277 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_common_functions.py
--rw-r--r--   0        0        0     1851 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_files.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/__init__.py
--rw-r--r--   0        0        0     2006 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_base.py
--rw-r--r--   0        0        0     6319 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_gpkg.py
--rw-r--r--   0        0        0     2855 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_table.py
--rw-r--r--   0        0        0    10002 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_tif.py
--rw-r--r--   0        0        0     1460 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_protocol.py
--rw-r--r--   0        0        0     1618 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_parallel_run.py
--rw-r--r--   0        0        0     3079 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_names.py
--rw-r--r--   0        0        0    32496 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/hazard/hazard_overlay.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/network_config_data/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/network_config_data/enums/__init__.py
--rw-r--r--   0        0        0      178 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/network_config_data/enums/aggregate_wl_enum.py
--rw-r--r--   0        0        0      217 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/network_config_data/enums/network_type_enum.py
--rw-r--r--   0        0        0      134 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_config_data/enums/part_of_day_enum.py
--rw-r--r--   0        0        0      447 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_config_data/enums/road_type_enum.py
--rw-r--r--   0        0        0      638 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_config_data/enums/source_enum.py
--rw-r--r--   0        0        0     4909 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_config_data/network_config_data.py
--rw-r--r--   0        0        0     9975 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_config_data/network_config_data_reader.py
--rw-r--r--   0        0        0     6039 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_config_data/network_config_data_validator.py
--rw-r--r--   0        0        0      577 2024-03-20 13:58:23.897771 ra2ce-0.8.1/ra2ce/network/network_config_data/README.md
--rw-r--r--   0        0        0     4243 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_config_wrapper.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/__init__.py
--rw-r--r--   0        0        0     3327 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/network_wrapper_factory.py
--rw-r--r--   0        0        0     1495 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/network_wrapper_protocol.py
--rw-r--r--   0        0        0        0 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/osm_network_wrapper/__init__.py
--rw-r--r--   0        0        0     4867 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/osm_network_wrapper/extremities_data.py
--rw-r--r--   0        0        0    17213 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/osm_network_wrapper/osm_network_wrapper.py
--rw-r--r--   0        0        0     3683 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/osm_network_wrapper/osm_utils.py
--rw-r--r--   0        0        0      599 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/README.md
--rw-r--r--   0        0        0     8407 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/shp_network_wrapper.py
--rw-r--r--   0        0        0     4701 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/trails_network_wrapper.py
--rw-r--r--   0        0        0     8406 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/network_wrappers/vector_network_wrapper.py
--rw-r--r--   0        0        0     9585 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/networks.py
--rw-r--r--   0        0        0    75922 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/networks_utils.py
--rw-r--r--   0        0        0    26000 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/origins_destinations.py
--rw-r--r--   0        0        0     7495 2024-03-20 13:58:23.913399 ra2ce-0.8.1/ra2ce/network/segmentation.py
--rw-r--r--   0        0        0     3431 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/ra2ce_handler.py
--rw-r--r--   0        0        0     2840 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/ra2ce_logging.py
--rw-r--r--   0        0        0      140 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/runners/__init__.py
--rw-r--r--   0        0        0     2349 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/runners/analysis_runner_factory.py
--rw-r--r--   0        0        0     2045 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/runners/analysis_runner_protocol.py
--rw-r--r--   0        0        0     3271 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/runners/direct_analysis_runner.py
--rw-r--r--   0        0        0     2897 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/runners/indirect_analysis_runner.py
--rw-r--r--   0        0        0      751 2024-03-20 13:58:23.929019 ra2ce-0.8.1/ra2ce/runners/README.md
--rw-r--r--   0        0        0     3305 2024-03-20 13:58:22.944678 ra2ce-0.8.1/README.md
--rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 ra2ce-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      877 2024-04-11 13:42:51.334331 ra2ce-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3661 2024-04-11 13:42:53.287450 ra2ce-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-11 13:42:53.287450 ra2ce-0.9.0/ra2ce/__init__.py
+-rw-r--r--   0        0        0     2098 2024-04-11 13:42:53.287450 ra2ce-0.9.0/ra2ce/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.287450 ra2ce-0.9.0/ra2ce/analysis/__init__.py
+-rw-r--r--   0        0        0     2312 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_collection.py
+-rw-r--r--   0        0        0        2 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/__init__.py
+-rw-r--r--   0        0        0     7298 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/analysis_config_data.py
+-rw-r--r--   0        0        0    12568 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/analysis_config_data_reader.py
+-rw-r--r--   0        0        0     4551 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/analysis_config_data_validator.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/analysis_direct_enum.py
+-rw-r--r--   0        0        0      464 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/analysis_indirect_enum.py
+-rw-r--r--   0        0        0      537 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/damage_curve_enum.py
+-rw-r--r--   0        0        0      160 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/event_type_enum.py
+-rw-r--r--   0        0        0      173 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/loss_type_enum.py
+-rw-r--r--   0        0        0      217 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/risk_calculation_mode_enum.py
+-rw-r--r--   0        0        0      203 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/trip_purposes.py
+-rw-r--r--   0        0        0      165 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/weighing_enum.py
+-rw-r--r--   0        0        0      687 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/README.md
+-rw-r--r--   0        0        0     3837 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_config_wrapper.py
+-rw-r--r--   0        0        0     8255 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_factory.py
+-rw-r--r--   0        0        0     1874 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_input_wrapper.py
+-rw-r--r--   0        0        0     1794 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_protocol.py
+-rw-r--r--   0        0        0     1489 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_result_wrapper.py
+-rw-r--r--   0        0        0     3353 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/analysis_result_wrapper_exporter.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/direct/__init__.py
+-rw-r--r--   0        0        0     1349 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/direct/analysis_direct_protocol.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.303077 ra2ce-0.9.0/ra2ce/analysis/direct/damage/__init__.py
+-rw-r--r--   0        0        0     5652 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage/damage_fraction_uniform.py
+-rw-r--r--   0        0        0     6461 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage/damage_function_road_type_lane.py
+-rw-r--r--   0        0        0     2806 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage/manual_damage_functions.py
+-rw-r--r--   0        0        0     4611 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage/max_damage.py
+-rw-r--r--   0        0        0      229 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/__init__.py
+-rw-r--r--   0        0        0    17670 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/damage_network_base.py
+-rw-r--r--   0        0        0     2895 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/damage_network_events.py
+-rw-r--r--   0        0        0    13051 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/damage_network_return_periods.py
+-rw-r--r--   0        0        0      889 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/risk_utils.py
+-rw-r--r--   0        0        0     4718 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/direct_damage.py
+-rw-r--r--   0        0        0    39766 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/direct_lookup.py
+-rw-r--r--   0        0        0     5787 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/direct_utils.py
+-rw-r--r--   0        0        0    19695 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/effectiveness_measures.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/direct/readme.txt
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/__init__.py
+-rw-r--r--   0        0        0     1509 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/analysis_indirect_protocol.py
+-rw-r--r--   0        0        0    27260 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/losses.py
+-rw-r--r--   0        0        0    12404 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_isolated_locations.py
+-rw-r--r--   0        0        0     8541 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_losses.py
+-rw-r--r--   0        0        0     6770 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_origin_closest_destination.py
+-rw-r--r--   0        0        0    17649 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_origin_destination.py
+-rw-r--r--   0        0        0     7725 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_redundancy.py
+-rw-r--r--   0        0        0     4605 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/optimal_route_origin_closest_destination.py
+-rw-r--r--   0        0        0     9406 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/optimal_route_origin_destination.py
+-rw-r--r--   0        0        0    43708 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/origin_closest_destination.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/readme.txt
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/single_link_losses.py
+-rw-r--r--   0        0        0     4707 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/single_link_redundancy.py
+-rw-r--r--   0        0        0      220 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/__init__.py
+-rw-r--r--   0        0        0     3389 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/accumulated_traffic_dataclass.py
+-rw-r--r--   0        0        0     4072 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/equity_analysis.py
+-rw-r--r--   0        0        0     1227 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/README.md
+-rw-r--r--   0        0        0     2983 2024-04-11 13:42:53.318702 ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis.py
+-rw-r--r--   0        0        0     4123 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_base.py
+-rw-r--r--   0        0        0     3025 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_factory.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/__init__.py
+-rw-r--r--   0        0        0      511 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/length_weighing_analysis.py
+-rw-r--r--   0        0        0      401 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/README.md
+-rw-r--r--   0        0        0     1766 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/time_weighing_analysis.py
+-rw-r--r--   0        0        0      867 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_factory.py
+-rw-r--r--   0        0        0      882 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_protocol.py
+-rw-r--r--   0        0        0     1525 2024-04-11 13:42:53.287450 ra2ce-0.9.0/ra2ce/analysis/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/configuration/__init__.py
+-rw-r--r--   0        0        0     1391 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/configuration/config_data_protocol.py
+-rw-r--r--   0        0        0     2060 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/configuration/config_wrapper_protocol.py
+-rw-r--r--   0        0        0     1663 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/configuration/ini_configuration_reader_protocol.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/io/__init__.py
+-rw-r--r--   0        0        0       75 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/io/readers/__init__.py
+-rw-r--r--   0        0        0     1321 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/io/readers/file_reader_protocol.py
+-rw-r--r--   0        0        0     1579 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/io/readers/graph_pickle_reader.py
+-rw-r--r--   0        0        0      529 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/io/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/io/writers/__init__.py
+-rw-r--r--   0        0        0     1361 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/io/writers/ra2ce_exporter_protocol.py
+-rw-r--r--   0        0        0      718 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/validation/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/validation/ra2ce_validator_protocol.py
+-rw-r--r--   0        0        0      466 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/validation/README.md
+-rw-r--r--   0        0        0     1731 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/common/validation/validation_report.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/configuration/__init__.py
+-rw-r--r--   0        0        0     5489 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/configuration/config_factory.py
+-rw-r--r--   0        0        0     2648 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/configuration/config_wrapper.py
+-rw-r--r--   0        0        0     2106 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/configuration/ra2ce_enum_base.py
+-rw-r--r--   0        0        0      245 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/configuration/README.md
+-rw-r--r--   0        0        0       44 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/network/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/network/exporters/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/network/exporters/geodataframe_network_exporter.py
+-rw-r--r--   0        0        0     1778 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/exporters/json_exporter.py
+-rw-r--r--   0        0        0     2169 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/exporters/multi_graph_network_exporter.py
+-rw-r--r--   0        0        0     2918 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/exporters/network_exporter_base.py
+-rw-r--r--   0        0        0     2186 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/exporters/network_exporter_factory.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/graph_files/__init__.py
+-rw-r--r--   0        0        0     1077 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/graph_files/graph_file.py
+-rw-r--r--   0        0        0     5753 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/graph_files/graph_files_collection.py
+-rw-r--r--   0        0        0      951 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/graph_files/graph_files_protocol.py
+-rw-r--r--   0        0        0      966 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/graph_files/network_file.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/__init__.py
+-rw-r--r--   0        0        0     2277 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_common_functions.py
+-rw-r--r--   0        0        0     1851 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_files.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/__init__.py
+-rw-r--r--   0        0        0     2006 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_base.py
+-rw-r--r--   0        0        0     5630 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_gpkg.py
+-rw-r--r--   0        0        0     2839 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_table.py
+-rw-r--r--   0        0        0     9624 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_tif.py
+-rw-r--r--   0        0        0     1462 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_protocol.py
+-rw-r--r--   0        0        0     3079 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_names.py
+-rw-r--r--   0        0        0    32453 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/hazard/hazard_overlay.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/enums/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/enums/aggregate_wl_enum.py
+-rw-r--r--   0        0        0      217 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/enums/network_type_enum.py
+-rw-r--r--   0        0        0      134 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/enums/part_of_day_enum.py
+-rw-r--r--   0        0        0      447 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/enums/road_type_enum.py
+-rw-r--r--   0        0        0      638 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/enums/source_enum.py
+-rw-r--r--   0        0        0     5045 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_config_data/network_config_data.py
+-rw-r--r--   0        0        0    10573 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_config_data/network_config_data_reader.py
+-rw-r--r--   0        0        0     6039 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_config_data/network_config_data_validator.py
+-rw-r--r--   0        0        0      570 2024-04-11 13:42:53.349953 ra2ce-0.9.0/ra2ce/network/network_config_data/README.md
+-rw-r--r--   0        0        0     4090 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_config_wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/__init__.py
+-rw-r--r--   0        0        0     3327 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/network_wrapper_factory.py
+-rw-r--r--   0        0        0     1495 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/network_wrapper_protocol.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/osm_network_wrapper/__init__.py
+-rw-r--r--   0        0        0     4867 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/osm_network_wrapper/extremities_data.py
+-rw-r--r--   0        0        0    18179 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/osm_network_wrapper/osm_network_wrapper.py
+-rw-r--r--   0        0        0    15457 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/osm_network_wrapper/osm_utils.py
+-rw-r--r--   0        0        0      945 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/README.md
+-rw-r--r--   0        0        0     8407 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/shp_network_wrapper.py
+-rw-r--r--   0        0        0     4701 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/trails_network_wrapper.py
+-rw-r--r--   0        0        0    16566 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/network_wrappers/vector_network_wrapper.py
+-rw-r--r--   0        0        0    12507 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/networks.py
+-rw-r--r--   0        0        0    82723 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/networks_utils.py
+-rw-r--r--   0        0        0    27989 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/origins_destinations.py
+-rw-r--r--   0        0        0      817 2024-04-11 13:42:53.334326 ra2ce-0.9.0/ra2ce/network/README.md
+-rw-r--r--   0        0        0     7495 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/network/segmentation.py
+-rw-r--r--   0        0        0     7123 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/ra2ce_handler.py
+-rw-r--r--   0        0        0     3929 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/ra2ce_logger.py
+-rw-r--r--   0        0        0     1734 2024-04-11 13:42:53.287450 ra2ce-0.9.0/ra2ce/README.md
+-rw-r--r--   0        0        0      140 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/runners/__init__.py
+-rw-r--r--   0        0        0     2349 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/runners/analysis_runner_factory.py
+-rw-r--r--   0        0        0     2034 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/runners/analysis_runner_protocol.py
+-rw-r--r--   0        0        0     3271 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/runners/direct_analysis_runner.py
+-rw-r--r--   0        0        0     2886 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/runners/indirect_analysis_runner.py
+-rw-r--r--   0        0        0      751 2024-04-11 13:42:53.365577 ra2ce-0.9.0/ra2ce/runners/README.md
+-rw-r--r--   0        0        0     3305 2024-04-11 13:42:51.334331 ra2ce-0.9.0/README.md
+-rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 ra2ce-0.9.0/PKG-INFO
```

### Comparing `ra2ce-0.8.1/LICENSE` & `ra2ce-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/pyproject.toml` & `ra2ce-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ra2ce"
-version = "0.8.1"
+version = "0.9.0"
 description = "Risk Assessment and Adaptation for Critical infrastructurE (RA2CE)."
 authors = [
   "Margreet van Marle <Margreet.vanMarle@deltares.nl>", 
   "Kees van Ginkel <kees.vanginkel@deltares.nl>",
 ]
 maintainers = [
   "Carles Salvador Soriano Perez <carles.sorianoperez@deltares.nl>",
@@ -94,15 +94,15 @@
 testbook = "^0.4.2"
 pytest-xdist = "^3.3.1"
 pytest-profiling = "^1.7.0"
 pytest-notebook = "^0.9.0"
 
 [tool.black]
 line-length = 88
-target-version = ['py38', 'py39']
+target-version = ['py310', 'py311']
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
     | \.mypy_cache
@@ -116,21 +116,20 @@
   )/
 )
 '''
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
-line_length = 88
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 changelog_file = "docs/changelog.md"
 update_changelog_on_bump = true
-version = "0.8.1"
+version = "0.9.0"
 tag_format = "v$major.$minor.$patch"
 version_files= [
     "ra2ce/__init__.py",
     "pyproject.toml:version",]
 
 [tool.pytest]
 markers = [
```

### Comparing `ra2ce-0.8.1/ra2ce/__main__.py` & `ra2ce-0.9.0/ra2ce/__main__.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_collection.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_collection.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/analysis_config_data.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/analysis_config_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 from __future__ import annotations
 
 import math
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Optional
 
-from ra2ce.analysis.analysis_config_data.enums import damage_curve_enum
 from ra2ce.analysis.analysis_config_data.enums.analysis_direct_enum import (
     AnalysisDirectEnum,
 )
 from ra2ce.analysis.analysis_config_data.enums.analysis_indirect_enum import (
     AnalysisIndirectEnum,
 )
+from ra2ce.analysis.analysis_config_data.enums.trip_purposes import TripPurposeEnum
+from ra2ce.analysis.analysis_config_data.enums.damage_curve_enum import DamageCurveEnum
 from ra2ce.analysis.analysis_config_data.enums.event_type_enum import EventTypeEnum
 from ra2ce.analysis.analysis_config_data.enums.loss_type_enum import LossTypeEnum
 from ra2ce.analysis.analysis_config_data.enums.risk_calculation_mode_enum import (
     RiskCalculationModeEnum,
 )
 from ra2ce.analysis.analysis_config_data.enums.weighing_enum import WeighingEnum
 from ra2ce.common.configuration.config_data_protocol import ConfigDataProtocol
@@ -85,27 +86,32 @@
         default_factory=lambda: AnalysisIndirectEnum.INVALID
     )
     # general
     weighing: WeighingEnum = field(default_factory=lambda: WeighingEnum.NONE)
     loss_per_distance: str = ""
     loss_type: LossTypeEnum = field(default_factory=lambda: LossTypeEnum.NONE)
     disruption_per_category: str = ""
-    traffic_cols: list[str] = field(default_factory=list)
     # losses
-    duration_event: float = math.nan # TODO remove the deprecated attribute that have been replaced by csv
-    duration_disruption: float = math.nan
-    fraction_detour: float = math.nan
-    fraction_drivethrough: float = 0.0
-    rest_capacity: float = math.nan
-    maximum_jam: float = math.nan
+    traffic_cols: list[str] = field(default_factory=list)
+    duration_event: float = (
+        math.nan
+    )  # TODO remove the deprecated attribute that have been replaced by csv
+    production_loss_per_capita_per_day: float = math.nan
     part_of_day: PartOfDayEnum = field(default_factory=lambda: PartOfDayEnum.DAY)
-    performance: str = "diff_time"  # "diff_time" or "diff_length" relates to the used criticality metric
+    performance: str = (
+        "diff_time"  # "diff_time" or "diff_length" relates to the used criticality metric
+    )
+    hours_per_day: float = 24
+    trip_purposes: list[TripPurposeEnum] = field(
+        default_factory=lambda: [TripPurposeEnum.NONE]
+    )
     resilience_curve_file: Optional[Path] = None
     traffic_intensities_file: Optional[Path] = None
     values_of_time_file: Optional[Path] = None
+    # the redundancy analysis) and the intensities
     # accessibility analyses
     aggregate_wl: AggregateWlEnum = field(default_factory=lambda: AggregateWlEnum.NONE)
     threshold: float = math.nan
     threshold_destinations: float = math.nan
     uniform_duration: float = math.nan
     gdp_percapita: float = math.nan
     equity_weight: str = ""
@@ -130,30 +136,30 @@
     repair_costs: float = math.nan
     evaluation_period: float = math.nan
     interest_rate: float = math.nan
     climate_factor: float = math.nan
     climate_period: float = math.nan
     # road damage
     event_type: EventTypeEnum = field(default_factory=lambda: EventTypeEnum.INVALID)
-    damage_curve: damage_curve_enum.DamageCurveEnum = field(
-        default_factory=lambda: EventTypeEnum.INVALID
+    damage_curve: DamageCurveEnum = field(
+        default_factory=lambda: DamageCurveEnum.INVALID
     )
     risk_calculation_mode: RiskCalculationModeEnum = field(
         default_factory=lambda: RiskCalculationModeEnum.NONE
     )
     risk_calculation_year: int = 0
     create_table: bool = False
     file_name: Optional[Path] = None
 
 
 @dataclass
 class AnalysisConfigData(ConfigDataProtocol):
     """
     Reflects all config data from analysis.ini with defaults set.
-    Additionally some attributes from the network config are added for completeness (files, origins_destinations, network, hazard_names)
+    Additionally, some attributes from the network config are added for completeness (files, origins_destinations, network, hazard_names)
     """
 
     root_path: Optional[Path] = None
     input_path: Optional[Path] = None
     output_path: Optional[Path] = None
     static_path: Optional[Path] = None
     project: ProjectSection = field(default_factory=ProjectSection)
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/analysis_config_data_reader.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/analysis_config_data_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from ra2ce.analysis.analysis_config_data.enums.damage_curve_enum import DamageCurveEnum
 from ra2ce.analysis.analysis_config_data.enums.event_type_enum import EventTypeEnum
 from ra2ce.analysis.analysis_config_data.enums.loss_type_enum import LossTypeEnum
 from ra2ce.analysis.analysis_config_data.enums.risk_calculation_mode_enum import (
     RiskCalculationModeEnum,
 )
 from ra2ce.analysis.analysis_config_data.enums.weighing_enum import WeighingEnum
+from ra2ce.analysis.analysis_config_data.enums.trip_purposes import TripPurposeEnum
 from ra2ce.common.configuration.ini_configuration_reader_protocol import (
     ConfigDataReaderProtocol,
 )
 
 
 class AnalysisConfigDataReader(ConfigDataReaderProtocol):
     """
@@ -126,45 +127,37 @@
         _section.loss_type = LossTypeEnum.get_enum(
             self._parser.get(section_name, "loss_type", fallback=None)
         )
         # losses
         _section.traffic_cols = self._parser.getlist(
             section_name, "traffic_cols", fallback=_section.traffic_cols
         )
-        _section.duration_event = self._parser.getfloat(
-            section_name,
-            "duration_event",
-            fallback=_section.duration_event,
-        )  # TODO remove the deprecated attribute that have been replaced by csv
-        _section.duration_disruption = self._parser.getfloat(
-            section_name,
-            "duration_disruption",
-            fallback=_section.duration_disruption,
+        _section.trip_purposes = list(
+            map(
+                TripPurposeEnum.get_enum,
+                self._parser.getlist(section_name, "trip_purposes", fallback=[]),
+            )
         )
-        _section.fraction_detour = self._parser.getfloat(
+        _section.production_loss_per_capita_per_day = self._parser.getfloat(
             section_name,
-            "fraction_detour",
-            fallback=_section.fraction_detour,
+            "production_loss_per_capita_per_day",
+            fallback=_section.production_loss_per_capita_per_day,
         )
-        _section.fraction_drivethrough = self._parser.getfloat(
-            section_name,
-            "fraction_drivethrough",
-            fallback=_section.fraction_drivethrough,
-        )
-        _section.rest_capacity = self._parser.getfloat(
+        _section.duration_event = self._parser.getfloat(
             section_name,
-            "rest_capacity",
-            fallback=_section.rest_capacity,
+            "duration_event",
+            fallback=_section.duration_event,
         )
-        _section.maximum_jam = self._parser.getfloat(
+        _section.hours_per_day = self._parser.getfloat(
             section_name,
-            "maximum_jam",
-            fallback=_section.maximum_jam,
+            "hours_per_day",
+            fallback=_section.hours_per_day,
         )
-        # accessiblity analyses
+
+        # accessibility analyses
         _section.threshold = self._parser.getfloat(
             section_name,
             "threshold",
             fallback=_section.threshold,
         )
         _section.threshold_destinations = self._parser.getfloat(
             section_name,
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/analysis_config_data_validator.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/analysis_config_data_validator.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/enums/damage_curve_enum.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/enums/damage_curve_enum.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_config_data/README.md` & `ra2ce-0.9.0/ra2ce/analysis/analysis_config_data/README.md`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_config_wrapper.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_config_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,10 +90,8 @@
 
         return _new_analysis
 
     def configure(self) -> None:
         self.initialize_output_dirs()
 
     def is_valid(self) -> bool:
-        _file_is_valid = self.ini_file.is_file() and self.ini_file.suffix == ".ini"
-        _validation_report = AnalysisConfigDataValidator(self.config_data).validate()
-        return _file_is_valid and _validation_report.is_valid()
+        return AnalysisConfigDataValidator(self.config_data).validate().is_valid()
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_factory.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,39 +31,35 @@
 )
 from ra2ce.analysis.analysis_config_wrapper import AnalysisConfigWrapper
 from ra2ce.analysis.analysis_input_wrapper import AnalysisInputWrapper
 from ra2ce.analysis.direct.analysis_direct_protocol import AnalysisDirectProtocol
 from ra2ce.analysis.direct.direct_damage import DirectDamage
 from ra2ce.analysis.direct.effectiveness_measures import EffectivenessMeasures
 from ra2ce.analysis.indirect.analysis_indirect_protocol import AnalysisIndirectProtocol
-from ra2ce.analysis.indirect.losses import Losses
 from ra2ce.analysis.indirect.multi_link_isolated_locations import (
     MultiLinkIsolatedLocations,
 )
-from ra2ce.analysis.indirect.multi_link_losses import MultiLinkLosses
 from ra2ce.analysis.indirect.multi_link_origin_closest_destination import (
     MultiLinkOriginClosestDestination,
 )
 from ra2ce.analysis.indirect.multi_link_origin_destination import (
     MultiLinkOriginDestination,
 )
 from ra2ce.analysis.indirect.multi_link_redundancy import MultiLinkRedundancy
 from ra2ce.analysis.indirect.optimal_route_origin_closest_destination import (
     OptimalRouteOriginClosestDestination,
 )
 from ra2ce.analysis.indirect.optimal_route_origin_destination import (
     OptimalRouteOriginDestination,
 )
-from ra2ce.analysis.indirect.single_link_losses import SingleLinkLosses
+from ra2ce.analysis.indirect.losses import Losses
 from ra2ce.analysis.indirect.single_link_redundancy import SingleLinkRedundancy
-from ra2ce.network.hazard.hazard_names import HazardNames
 
 
 class AnalysisFactory:
-
     @staticmethod
     def get_direct_analysis(
         analysis: AnalysisSectionDirect,
         analysis_config: AnalysisConfigWrapper,
     ) -> AnalysisDirectProtocol:
         """
         Create an analysis based on the given analysis configuration.
@@ -87,16 +83,16 @@
             return DirectDamage(_analysis_input)
         if analysis.analysis == AnalysisDirectEnum.EFFECTIVENESS_MEASURES:
             return EffectivenessMeasures(_analysis_input)
         raise NotImplementedError(f"Analysis {analysis.analysis} not implemented")
 
     @staticmethod
     def get_indirect_analysis(
-        analysis: AnalysisSectionIndirect,
-        analysis_config: AnalysisConfigWrapper,
+            analysis: AnalysisSectionIndirect,
+            analysis_config: AnalysisConfigWrapper,
     ) -> AnalysisIndirectProtocol:
         """
         Create an analysis based on the given analysis configuration.
 
         Args:
             analysis (AnalysisSectionIndirect): Analysis section.
             analysis_config (AnalysisConfigWrapper): Analysis configuration.
@@ -132,55 +128,50 @@
             _analysis_input = AnalysisInputWrapper.from_input(
                 analysis=analysis,
                 analysis_config=analysis_config,
                 graph_file_hazard=analysis_config.graph_files.origins_destinations_graph_hazard,
             )
             return MultiLinkOriginDestination(_analysis_input)
         if (
-            analysis.analysis
-            == AnalysisIndirectEnum.OPTIMAL_ROUTE_ORIGIN_CLOSEST_DESTINATION
+                analysis.analysis
+                == AnalysisIndirectEnum.OPTIMAL_ROUTE_ORIGIN_CLOSEST_DESTINATION
         ):
             _analysis_input = AnalysisInputWrapper.from_input(
                 analysis=analysis,
                 analysis_config=analysis_config,
                 graph_file_hazard=analysis_config.graph_files.origins_destinations_graph_hazard,
             )
             return OptimalRouteOriginClosestDestination(analysis_input=_analysis_input)
         if (
-            analysis.analysis
-            == AnalysisIndirectEnum.MULTI_LINK_ORIGIN_CLOSEST_DESTINATION
+                analysis.analysis
+                == AnalysisIndirectEnum.MULTI_LINK_ORIGIN_CLOSEST_DESTINATION
         ):
             _analysis_input = AnalysisInputWrapper.from_input(
                 analysis=analysis,
                 analysis_config=analysis_config,
                 graph_file=analysis_config.graph_files.origins_destinations_graph,
                 graph_file_hazard=analysis_config.graph_files.origins_destinations_graph_hazard,
             )
             return MultiLinkOriginClosestDestination(_analysis_input)
-        if analysis.analysis == AnalysisIndirectEnum.LOSSES:
-            _analysis_input = AnalysisInputWrapper.from_input(
-                analysis=analysis,
-                analysis_config=analysis_config,
-                graph_file_hazard=analysis_config.graph_files.base_graph_hazard,
-            )
-            return Losses(_analysis_input)
         if analysis.analysis == AnalysisIndirectEnum.SINGLE_LINK_LOSSES:
             _analysis_input = AnalysisInputWrapper.from_input(
                 analysis=analysis,
                 analysis_config=analysis_config,
+                graph_file=analysis_config.graph_files.base_graph_hazard,
                 graph_file_hazard=analysis_config.graph_files.base_graph_hazard,
             )
-            return SingleLinkLosses(_analysis_input)
+            return Losses(_analysis_input, analysis_config)
         if analysis.analysis == AnalysisIndirectEnum.MULTI_LINK_LOSSES:
             _analysis_input = AnalysisInputWrapper.from_input(
                 analysis=analysis,
                 analysis_config=analysis_config,
                 graph_file_hazard=analysis_config.graph_files.base_graph_hazard,
             )
-            return MultiLinkLosses(_analysis_input)
+
+            return Losses(_analysis_input, analysis_config)
         if analysis.analysis == AnalysisIndirectEnum.MULTI_LINK_ISOLATED_LOCATIONS:
             _analysis_input = AnalysisInputWrapper.from_input(
                 analysis=analysis,
                 analysis_config=analysis_config,
                 graph_file_hazard=analysis_config.graph_files.base_graph_hazard,
             )
             return MultiLinkIsolatedLocations(_analysis_input)
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_input_wrapper.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_input_wrapper.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_protocol.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_result_wrapper.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_result_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from dataclasses import dataclass
+
 import geopandas as gpd
+
 from ra2ce.analysis.analysis_protocol import AnalysisProtocol
 
 
 @dataclass
 class AnalysisResultWrapper:
     analysis_result: gpd.GeoDataFrame
     analysis: AnalysisProtocol
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/analysis_result_wrapper_exporter.py` & `ra2ce-0.9.0/ra2ce/analysis/analysis_result_wrapper_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-from copy import deepcopy
 import logging
+from copy import deepcopy
 from pathlib import Path
+
 from geopandas import GeoDataFrame
+
 from ra2ce.analysis.analysis_result_wrapper import AnalysisResultWrapper
 
 
 class AnalysisResultWrapperExporter:
-
     def export_result(
         self,
         result_wrapper: AnalysisResultWrapper,
     ):
         """
         Exports the given result into the analysis requested formats ( `.gpkg` and / or `.csv`).
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/analysis_direct_protocol.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/analysis_direct_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage/damage_fraction_uniform.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage/damage_fraction_uniform.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage/damage_function_road_type_lane.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage/damage_function_road_type_lane.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage/manual_damage_functions.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage/manual_damage_functions.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage/max_damage.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage/max_damage.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/damage_network_base.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/damage_network_base.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/damage_network_events.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/damage_network_events.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/damage_network_return_periods.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/damage_network_return_periods.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/damage_calculation/risk_utils.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/damage_calculation/risk_utils.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/direct_damage.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/direct_damage.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         self.analysis = analysis_input.analysis
         self.graph_file = None
         self.graph_file_hazard = analysis_input.graph_file_hazard
         self.input_path = analysis_input.input_path
         self.output_path = analysis_input.output_path
 
     def execute(self) -> GeoDataFrame:
-
         def _rename_road_gdf_to_conventions(road_gdf_columns: list[str]) -> list[str]:
             """
             Rename the columns in the road_gdf to the conventions of the ra2ce documentation
 
             'eg' RP100_fr -> F_RP100_me
                         -> F_EV1_mi
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/direct_lookup.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/direct_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from scipy.interpolate import interp1d
 
 
 def dataframe_lookup(row: pd.Series, lookup_df: DataFrame, columns: list) -> Any:
     row_values = [row[column] for column in columns]
     return lookup_df.loc[tuple(row_values)]
 
+
 class LookUp:
     """ " This namespace contains several lookup tables, used e.g. for road damage calculation."""
 
     @staticmethod
     def road_mapping():
         """Mapping of OSM road infrastructure types"""
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/direct_utils.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/direct_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,17 @@
     """
     # Todo: in the future we can make it more generic, so that we can easily get the mode/mean/whatever
 
     dictionary = dict(gdf.groupby("road_type")["lanes"].agg(pd.Series.mode))
 
     # get a default value if any key of the dictionary became empty (because the mode operation on the 'lanes' column
     # for a road type results in an empty array
-    non_empty_modes = [value for value in dictionary.values() if isinstance(value, float) and value > 0]
+    non_empty_modes = [
+        value for value in dictionary.values() if isinstance(value, float) and value > 0
+    ]
     default_value = np.mean(non_empty_modes)
 
     # Replace empty arrays with the calculated average
     for key, value in dictionary.items():
         if isinstance(value, np.ndarray) and len(value) == 0:
             dictionary[key] = default_value
     return dictionary
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/direct/effectiveness_measures.py` & `ra2ce-0.9.0/ra2ce/analysis/direct/effectiveness_measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import numpy as np
 import pandas as pd
 
 from ra2ce.analysis.analysis_config_data.analysis_config_data import (
     AnalysisSectionDirect,
 )
 from ra2ce.analysis.analysis_input_wrapper import AnalysisInputWrapper
-from ra2ce.analysis.direct.analysis_direct_protocol import (
-    AnalysisDirectProtocol,
-)
+from ra2ce.analysis.direct.analysis_direct_protocol import AnalysisDirectProtocol
 from ra2ce.network.graph_files.network_file import NetworkFile
 
 
 class EffectivenessMeasures(AnalysisDirectProtocol):
     analysis: AnalysisSectionDirect
     graph_file: NetworkFile
     graph_file_hazard: NetworkFile
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/analysis_indirect_protocol.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/analysis_indirect_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_isolated_locations.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_isolated_locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,22 @@
             crs (int, optional): The coordinate reference system used for geographical data. Defaults to 4326 (WGS84).
 
         Returns:
             tuple (gpd.GeoDataFrame, pd.DataFrame): A tuple containing the location GeoDataFrame updated with hazard impacts,
                 and a DataFrame summarizing the impacts per location category.
         """
 
+        def _is_not_none(value):
+            return (
+                value is not None
+                and value is not pd.NA
+                and not pd.isna(value)
+                and not np.isnan(value)
+            )
+
         # Load the point shapefile with the locations of which the isolated locations should be identified.
         locations = read_feather(
             self.static_path.joinpath("output_graph", "locations_hazard.feather")
         )
         # TODO PUT CRS IN DOCUMENTATION OR MAKE CHANGABLE
         # reproject the datasets to be able to make a buffer in meters
         nearest_utm = self.utm_crs(locations.total_bounds)
@@ -169,18 +177,22 @@
             graph_hz_indirect = copy.deepcopy(graph)
 
             # filter graph edges that are directly disrupted by the hazard(s), i.e. flooded
             edges = [e for e in graph.edges.data(keys=True) if hazard_name in e[-1]]
             edges_hz_direct = [
                 e
                 for e in edges
-                if e[-1][hazard_name]
+                if (hazard_name in e[-1])
                 and (
-                    (e[-1][hazard_name] > float(analysis.threshold))
-                    & ("bridge" not in e[-1])
+                    _is_not_none(e[-1][hazard_name])
+                    and (e[-1][hazard_name] > float(analysis.threshold))
+                    & (
+                        ("bridge" not in e[-1])
+                        or ("bridge" in e[-1] and e[-1]["bridge"] != "yes")
+                    )
                 )
             ]
             edges_hz_indirect = [e for e in edges if e not in edges_hz_direct]
 
             # get indirect graph - remove the edges that are impacted by hazard directly
             graph_hz_indirect.remove_edges_from(edges_hz_direct)
             # get indirect graph without the largest component, i.e. isolated graph
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_losses.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_losses.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_origin_closest_destination.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_origin_closest_destination.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ra2ce.analysis.indirect.origin_closest_destination import OriginClosestDestination
 from ra2ce.network.graph_files.graph_file import GraphFile
 from ra2ce.network.hazard.hazard_names import HazardNames
 from ra2ce.network.network_config_data.network_config_data import (
     OriginsDestinationsSection,
 )
 from ra2ce.network.networks_utils import graph_to_gpkg
-from ra2ce.ra2ce_logging import logging
+from ra2ce.ra2ce_logger import logging
 
 
 class MultiLinkOriginClosestDestination(AnalysisIndirectProtocol):
     analysis: AnalysisSectionIndirect
     graph_file: GraphFile
     graph_file_hazard: GraphFile
     input_path: Path
@@ -62,15 +62,14 @@
 
         if save_path.exists():
             save_path.unlink()
         gdf.to_file(save_path, driver="GPKG")
         logging.info("Results saved to: {}".format(save_path))
 
     def execute(self) -> GeoDataFrame:
-
         def _save_gpkg_analysis(
             base_graph,
             to_save_gdf: list[GeoDataFrame],
             to_save_gdf_names: list[str],
         ):
             for to_save, save_name in zip(to_save_gdf, to_save_gdf_names):
                 if not to_save.empty:
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_origin_destination.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_origin_destination.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/multi_link_redundancy.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/single_link_redundancy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import copy
 from pathlib import Path
 
 import networkx as nx
 import numpy as np
 import osmnx
-import pandas as pd
 from geopandas import GeoDataFrame
 
 from ra2ce.analysis.analysis_config_data.analysis_config_data import (
     AnalysisSectionIndirect,
 )
 from ra2ce.analysis.analysis_config_data.enums.weighing_enum import WeighingEnum
 from ra2ce.analysis.analysis_input_wrapper import AnalysisInputWrapper
@@ -16,134 +14,98 @@
 from ra2ce.analysis.indirect.weighing_analysis.weighing_analysis_factory import (
     WeighingAnalysisFactory,
 )
 from ra2ce.network.graph_files.graph_file import GraphFile
 from ra2ce.network.hazard.hazard_names import HazardNames
 
 
-class MultiLinkRedundancy(AnalysisIndirectProtocol):
+class SingleLinkRedundancy(AnalysisIndirectProtocol):
     analysis: AnalysisSectionIndirect
-    graph_file_hazard: GraphFile
+    graph_file: GraphFile
     input_path: Path
     static_path: Path
     output_path: Path
     hazard_names: HazardNames
 
-    def __init__(
-        self,
-        analysis_input: AnalysisInputWrapper,
-    ) -> None:
+    def __init__(self, analysis_input: AnalysisInputWrapper) -> None:
         self.analysis = analysis_input.analysis
-        self.graph_file_hazard = analysis_input.graph_file_hazard
+        self.graph_file = analysis_input.graph_file
         self.input_path = analysis_input.input_path
         self.static_path = analysis_input.static_path
         self.output_path = analysis_input.output_path
         self.hazard_names = analysis_input.hazard_names
+        self.result = None
 
     def execute(self) -> GeoDataFrame:
-        """Calculates the multi-link redundancy of a NetworkX graph.
-
-        The function removes all links of a variable that have a minimum value
-        of min_threshold. For each link it calculates the alternative path, if
-        any available. This function only removes one group at the time and saves the data from removing that group.
-
-        Returns:
-            aggregated_results (GeoDataFrame): The results of the analysis aggregated into a table.
-        """
-        results = []
-        master_graph = copy.deepcopy(self.graph_file_hazard.get_graph())
-        for hazard in self.hazard_names.names:
-            hazard_name = self.hazard_names.get_name(hazard)
-
-            _graph = copy.deepcopy(master_graph)
-            # Create a geodataframe from the full graph
-            gdf = osmnx.graph_to_gdfs(master_graph, nodes=False)
-            if "rfid" in gdf:
-                gdf["rfid"] = gdf["rfid"].astype(str)
-
-            # Create the edgelist that consist of edges that should be removed
-            edges_remove = [
-                e for e in _graph.edges.data(keys=True) if hazard_name in e[-1]
-            ]
-            edges_remove = [e for e in edges_remove if (e[-1][hazard_name] is not None)]
-            edges_remove = [
-                e
-                for e in edges_remove
-                if (e[-1][hazard_name] > float(self.analysis.threshold))
-                & ("bridge" not in e[-1])
-            ]
-
-            _graph.remove_edges_from(edges_remove)
-
-            columns = [
-                "u",
-                "v",
-                f"alt_{self.analysis.weighing.config_value}",
-                "alt_nodes",
-                "connected",
-            ]
-
-            if "rfid" in gdf:
-                columns.insert(2, "rfid")
-
-            df_calculated = pd.DataFrame(columns=columns)
-            _weighing_analyser = WeighingAnalysisFactory.get_analysis(
-                self.analysis.weighing
-            )
-
-            for edges in edges_remove:
-                u, v, k, _weighing_analyser.weighing_data = edges
-
-                if nx.has_path(_graph, u, v):
-                    alt_dist = nx.dijkstra_path_length(
-                        _graph, u, v, weight=WeighingEnum.LENGTH.config_value
-                    )
-                    alt_nodes = nx.dijkstra_path(_graph, u, v)
-                    connected = 1
-                    alt_value = _weighing_analyser.calculate_alternative_distance(
-                        alt_dist
-                    )
-                else:
-                    alt_value = _weighing_analyser.calculate_distance()
-                    alt_nodes, connected = np.NaN, 0
-
-                data = {
-                    "u": [u],
-                    "v": [v],
-                    f"alt_{self.analysis.weighing.config_value}": [alt_value],
-                    "alt_nodes": [alt_nodes],
-                    "connected": [connected],
-                }
-                _weighing_analyser.extend_graph(data)
-
-                if "rfid" in gdf:
-                    data["rfid"] = [str(_weighing_analyser.weighing_data["rfid"])]
-
-                df_calculated = pd.concat(
-                    [df_calculated, pd.DataFrame(data)], ignore_index=True
+        """This is the function to analyse roads with a single link disruption and an alternative route."""
+        # TODO adjust to the right names of the RA2CE tool
+        # if 'road_usage_data_path' in InputDict:
+        #     road_usage_data = pd.read_excel(InputDict.road_usage_data_path)
+        #     road_usage_data.dropna(axis=0, how='all', subset=['vehicle_type'], inplace=True)
+        #     aadt_names = [aadt_name for aadt_name in road_usage_data['attribute_name'] if aadt_name == aadt_name]
+        # else:
+        #     aadt_names = None
+        #     road_usage_data = pd.DataFrame()
+
+        # create a geodataframe from the graph
+        _gdf_graph = osmnx.graph_to_gdfs(self.graph_file.get_graph(), nodes=False)
+
+        # list for the length of the alternative routes
+        _alt_value_list = []
+        _alt_nodes_list = []
+        _diff_value_list = []
+        _detour_exist_list = []
+
+        _weighing_analyser = WeighingAnalysisFactory.get_analysis(
+            self.analysis.weighing
+        )
+        for e_remove in list(self.graph_file.graph.edges.data(keys=True)):
+            u, v, k, _weighing_analyser.weighing_data = e_remove
+
+            # if data['highway'] in attr_list:
+            # remove the edge
+            self.graph_file.graph.remove_edge(u, v, k)
+
+            if nx.has_path(self.graph_file.graph, u, v):
+                # calculate the alternative distance if that edge is unavailable
+                alt_dist = nx.dijkstra_path_length(
+                    self.graph_file.graph, u, v, weight=WeighingEnum.LENGTH.config_value
                 )
-            df_calculated[f"alt_{self.analysis.weighing.config_value}"] = pd.to_numeric(
-                df_calculated[f"alt_{self.analysis.weighing.config_value}"],
-                errors="coerce",
-            )
-
-            # Merge the dataframes
-            if "rfid" in gdf:
-                gdf = gdf.merge(df_calculated, how="left", on=["u", "v", "rfid"])
-            else:
-                gdf = gdf.merge(df_calculated, how="left", on=["u", "v"])
+                alt_nodes = nx.dijkstra_path(self.graph_file.graph, u, v)
+                alt_value = _weighing_analyser.calculate_alternative_distance(alt_dist)
 
-            # calculate the differences in distance and time
-            # previously here you find if dist==dist which is a critical bug. Replaced by verifying dist is a value.
-            gdf[f"diff_{self.analysis.weighing.config_value}"] = [
-                round(alt - base, 2) if alt else np.NaN
-                for (alt, base) in zip(
-                    gdf[f"alt_{self.analysis.weighing.config_value}"],
-                    gdf[f"{self.analysis.weighing.config_value}"],
+                # append alternative route nodes
+                _alt_value_list.append(alt_value)
+                _alt_nodes_list.append(alt_nodes)
+
+                # calculate the difference in distance
+                _diff_value_list.append(
+                    round(
+                        alt_value
+                        - _weighing_analyser.weighing_data[
+                            self.analysis.weighing.config_value
+                        ],
+                        2,
+                    )
                 )
-            ]
 
-            gdf["hazard"] = hazard_name
+                _detour_exist_list.append(1)
+            else:
+                _alt_value_list.append(_weighing_analyser.calculate_distance())
+                _alt_nodes_list.append(np.NaN)
+                _diff_value_list.append(np.NaN)
+                _detour_exist_list.append(0)
+
+            # add edge again to the graph
+            self.graph_file.graph.add_edge(u, v, k, **_weighing_analyser.weighing_data)
+
+        # Add the new columns to the geodataframe
+        _weighing_analyser.extend_graph(_gdf_graph)
+        _gdf_graph[f"alt_{self.analysis.weighing.config_value}"] = _alt_value_list
+        _gdf_graph["alt_nodes"] = _alt_nodes_list
+        _gdf_graph[f"diff_{self.analysis.weighing.config_value}"] = _diff_value_list
+        _gdf_graph["detour"] = _detour_exist_list
 
-            results.append(gdf)
+        # Extra calculation possible (like multiplying the disruption time with the cost for disruption)
+        # todo: input here this option
 
-        return pd.concat(results, ignore_index=True)
+        return _gdf_graph
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/optimal_route_origin_closest_destination.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/optimal_route_origin_closest_destination.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 
         if save_path.exists():
             save_path.unlink()
         gdf.to_file(save_path, driver="GPKG")
         logging.info("Results saved to: {}".format(save_path))
 
     def execute(self) -> GeoDataFrame:
-
         def _save_gpkg_analysis(
             base_graph,
             to_save_gdf: list[GeoDataFrame],
             to_save_gdf_names: list[str],
         ):
             for to_save, save_name in zip(to_save_gdf, to_save_gdf_names):
                 if not to_save.empty:
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/optimal_route_origin_destination.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/optimal_route_origin_destination.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/origin_closest_destination.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/origin_closest_destination.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,24 +180,26 @@
                 for i, dn in self.destination_names_short.items():
                     destinations[hazard_name + "_P" + dn] = 0
             else:
                 destinations[hazard_name + "_P"] = 0
 
             # Check if the o/d pairs are still connected while some links are disrupted by the hazard(s)
             h = copy.deepcopy(graph)
-
-            edges_remove = [
-                e for e in graph.edges.data(keys=True) if hazard_name in e[-1]
-            ]
+            edges_remove = []
+            for e in graph.edges.data(keys=True):
+                if (hazard_name in e[-1]) and (
+                    ("bridge" not in e[-1])
+                    or ("bridge" in e[-1] and e[-1]["bridge"] != "yes")
+                ):
+                    edges_remove.append(e)
             edges_remove = [e for e in edges_remove if (e[-1][hazard_name] is not None)]
             edges_remove = [
                 e
                 for e in edges_remove
                 if (e[-1][hazard_name] > float(self.network_threshold))
-                & ("bridge" not in e[-1])
             ]
             h.remove_edges_from(edges_remove)
 
             if self.destination_key:
                 (
                     base_graph,
                     origins,
@@ -403,18 +405,20 @@
         )
         return destinations
 
     def update_origins(self, origins, other, col_name):
         # Attribute to the origins that don't have access that they do not have any access
         if len(other) > 0:
             for oth in other:
-                origins.loc[
-                    origins[self.od_id] == int(oth[-1].split("_")[-1]),
-                    col_name,
-                ] = "no access"
+                od_id_list = oth[-1].split(",")
+                for od_id in od_id_list:
+                    origins.loc[
+                        origins[self.od_id] == int(od_id.split("_")[-1]),
+                        col_name,
+                    ] = "no access"
         return origins
 
     def get_nr_without_access(
         self,
         origins: gpd.GeoDataFrame,
         origins_without_access: list,
         add_key_name: str = None,
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/single_link_losses.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/multi_link_redundancy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,183 +1,201 @@
+import copy
 from pathlib import Path
 
+import geopandas as gpd
+import networkx as nx
 import numpy as np
+import osmnx
 import pandas as pd
 from geopandas import GeoDataFrame
 
 from ra2ce.analysis.analysis_config_data.analysis_config_data import (
     AnalysisSectionIndirect,
 )
-from ra2ce.analysis.analysis_config_data.enums.loss_type_enum import LossTypeEnum
+from ra2ce.analysis.analysis_config_data.enums.weighing_enum import WeighingEnum
 from ra2ce.analysis.analysis_input_wrapper import AnalysisInputWrapper
 from ra2ce.analysis.indirect.analysis_indirect_protocol import AnalysisIndirectProtocol
-from ra2ce.analysis.indirect.single_link_redundancy import SingleLinkRedundancy
+from ra2ce.analysis.indirect.weighing_analysis.weighing_analysis_factory import (
+    WeighingAnalysisFactory,
+)
 from ra2ce.network.graph_files.graph_file import GraphFile
 from ra2ce.network.hazard.hazard_names import HazardNames
 
 
-class SingleLinkLosses(AnalysisIndirectProtocol):
+class MultiLinkRedundancy(AnalysisIndirectProtocol):
     analysis: AnalysisSectionIndirect
     graph_file_hazard: GraphFile
     input_path: Path
     static_path: Path
     output_path: Path
     hazard_names: HazardNames
-    _analysis_input: AnalysisInputWrapper
 
     def __init__(
         self,
         analysis_input: AnalysisInputWrapper,
     ) -> None:
         self.analysis = analysis_input.analysis
         self.graph_file_hazard = analysis_input.graph_file_hazard
         self.input_path = analysis_input.input_path
         self.static_path = analysis_input.static_path
         self.output_path = analysis_input.output_path
         self.hazard_names = analysis_input.hazard_names
-        self._analysis_input = analysis_input
 
-    def _single_link_losses_uniform(
-        self,
-        gdf: GeoDataFrame,
-        analysis: AnalysisSectionIndirect,
-        losses_df: pd.DataFrame,
-    ):
-        for hz in self.hazard_names.names:
-            for col in analysis.traffic_cols:
-                try:
-                    assert gdf[col + "_detour_losses"]
-                    assert gdf[col + "_nodetour_losses"]
-                except Exception:
-                    gdf[col + "_detour_losses"] = 0
-                    gdf[col + "_nodetour_losses"] = 0
-                # detour_losses = traffic_per_day[veh/day] * detour_distance[meter] * cost_per_meter[USD/meter/vehicle]  * duration_disruption[hour] / 24[hour/day]
-                gdf.loc[
-                    (gdf["detour"] == 1)
-                    & (
-                        gdf[hz + "_" + analysis.aggregate_wl.config_value]
-                        > analysis.threshold
-                    ),
-                    col + "_detour_losses",
-                ] += (
-                    gdf[col]
-                    * gdf["diff_dist"]
-                    * losses_df.loc[losses_df["traffic_class"] == col, "cost"].values[0]
-                    * analysis.uniform_duration
-                    / 24
-                )
-                # no_detour_losses = traffic_per_day[veh/day] * occupancy[person/veh] * gdp_percapita_per_day[USD/person] * duration_disruption[hour] / 24[hour/day]
-                gdf.loc[
-                    (gdf["detour"] == 0)
-                    & (
-                        gdf[hz + "_" + analysis.aggregate_wl.config_value]
-                        > analysis.threshold
-                    ),
-                    col + "_nodetour_losses",
-                ] += (
-                    gdf[col]
-                    * losses_df.loc[
-                        losses_df["traffic_class"] == col, "occupancy"
-                    ].values[0]
-                    * analysis.gdp_percapita
-                    * analysis.uniform_duration
-                    / 24
-                )
-            gdf["total_losses_" + hz] = np.nansum(
-                gdf[[x for x in gdf.columns if ("losses" in x) and ("total" not in x)]],
-                axis=1,
-            )
-
-    def _single_link_losses_categorized(
-        self,
-        gdf: GeoDataFrame,
-        analysis: AnalysisSectionIndirect,
-        losses_df: pd.DataFrame,
-        disruption_df: pd.DataFrame,
-    ):
-        _road_classes = [x for x in disruption_df.columns if "class" in x]
-        for hz in self.hazard_names.names:
-            disruption_df["class_identifier"] = ""
-            gdf["class_identifier"] = ""
-            for i, road_class in enumerate(_road_classes):
-                disruption_df["class_identifier"] += disruption_df[road_class]
-                gdf["class_identifier"] += gdf[road_class[6:]]
-                if i < len(_road_classes) - 1:
-                    disruption_df["class_identifier"] += "_nextclass_"
-                    gdf["class_identifier"] += "_nextclass_"
-
-            _all_road_categories = np.unique(gdf["class_identifier"])
-            gdf["duration_disruption"] = 0
-
-            for lb in np.unique(disruption_df["lower_bound"]):
-                disruption_df_ = disruption_df.loc[disruption_df["lower_bound"] == lb]
-                ub = disruption_df_["upper_bound"].values[0]
-                if ub <= 0:
-                    ub = 1e10
-                for road_cat in _all_road_categories:
-                    gdf.loc[
-                        (gdf[hz + "_" + analysis.aggregate_wl.config_value] > lb)
-                        & (gdf[hz + "_" + analysis.aggregate_wl.config_value] <= ub)
-                        & (gdf["class_identifier"] == road_cat),
-                        "duration_disruption",
-                    ] = disruption_df_.loc[
-                        disruption_df_["class_identifier"] == road_cat,
-                        "duration_disruption",
-                    ].values[
-                        0
-                    ]
-
-            for col in analysis.traffic_cols:
-                try:
-                    assert gdf[col + "_detour_losses"]
-                    assert gdf[col + "_nodetour_losses"]
-                except Exception:
-                    gdf[col + "_detour_losses"] = 0
-                    gdf[col + "_nodetour_losses"] = 0
-                # detour_losses = traffic_per_day[veh/day] * detour_distance[meter] * cost_per_meter[USD/meter/vehicle] * duration_disruption[hour] / 24[hour/day]
-                gdf.loc[gdf["detour"] == 1, col + "_detour_losses"] += (
-                    gdf[col]
-                    * gdf["diff_dist"]
-                    * losses_df.loc[losses_df["traffic_class"] == col, "cost"].values[0]
-                    * gdf["duration_disruption"]
-                    / 24
+    def _update_time(self, gdf_calculated: pd.DataFrame, gdf_graph: gpd.GeoDataFrame):
+        """
+        updates the time column with the calculated dataframe and updates the rest of the gdf_graph if time is None.
+        """
+        if (
+            WeighingEnum.TIME.config_value not in gdf_graph.columns
+            or WeighingEnum.TIME.config_value not in gdf_calculated.columns
+        ):
+            return gdf_graph
+        gdf_graph[WeighingEnum.TIME.config_value] = gdf_calculated[
+            WeighingEnum.TIME.config_value
+        ]
+        for i, row in gdf_graph.iterrows():
+            row_avgspeed = row.get("avgspeed", None)
+            row_length = row.get("length", None)
+            if (
+                pd.isna(row[WeighingEnum.TIME.config_value])
+                and row_avgspeed
+                and row_length
+            ):
+                gdf_graph.at[i, WeighingEnum.TIME.config_value] = (
+                    row_length * 1e-3 / row_avgspeed
                 )
-                # no_detour_losses = traffic_per_day[veh/day] * occupancy[person/veh] * gdp_percapita[USD/person] * duration_disruption[hour] / 24[hour/day]
-                gdf.loc[gdf["detour"] == 0, col + "_nodetour_losses"] += (
-                    gdf[col]
-                    * losses_df.loc[
-                        losses_df["traffic_class"] == col, "occupancy"
-                    ].values[0]
-                    * analysis.gdp_percapita
-                    * gdf["duration_disruption"]
-                    / 24
+            else:
+                gdf_graph.at[i, WeighingEnum.TIME.config_value] = row.get(
+                    WeighingEnum.TIME.config_value, None
                 )
-            gdf["total_losses_" + hz] = np.nansum(
-                gdf[[x for x in gdf.columns if ("losses" in x) and ("total" not in x)]],
-                axis=1,
-            )
+        return gdf_graph
 
     def execute(self) -> GeoDataFrame:
-        """Calculates single link disruption losses.
+        """Calculates the multi-link redundancy of a NetworkX graph.
+
+        The function removes all links of a variable that have a minimum value
+        of min_threshold. For each link it calculates the alternative path, if
+        any available. This function only removes one group at the time and saves the data from removing that group.
 
         Returns:
-            GeoDataFrame: The results of the analysis aggregated into a table.
+            aggregated_results (GeoDataFrame): The results of the analysis aggregated into a table.
         """
-        gdf = SingleLinkRedundancy(self._analysis_input).execute()
 
-        losses_fn = self.static_path.joinpath("hazard", self.analysis.loss_per_distance)
-        losses_df = pd.read_excel(losses_fn, sheet_name="Sheet1")
+        def _is_not_none(value):
+            return (
+                value is not None
+                and value is not pd.NA
+                and not pd.isna(value)
+                and not np.isnan(value)
+            )
+
+        results = []
+        master_graph = copy.deepcopy(self.graph_file_hazard.get_graph())
+        for hazard in self.hazard_names.names:
+            hazard_name = self.hazard_names.get_name(hazard)
+
+            _graph = copy.deepcopy(master_graph)
+            # Create a geodataframe from the full graph
+            gdf = osmnx.graph_to_gdfs(master_graph, nodes=False)
+            if "rfid" in gdf:
+                gdf["rfid"] = gdf["rfid"].astype(str)
+
+            # Create the edgelist that consist of edges that should be removed
+            edges_remove = []
+            for e in _graph.edges.data(keys=True):
+                if (hazard_name in e[-1]) and (
+                    ("bridge" not in e[-1])
+                    or ("bridge" in e[-1] and e[-1]["bridge"] != "yes")
+                ):
+                    edges_remove.append(e)
+            edges_remove = [e for e in edges_remove if (e[-1][hazard_name] is not None)]
+            edges_remove = [
+                e
+                for e in edges_remove
+                if (hazard_name in e[-1])
+                and (
+                    _is_not_none(e[-1][hazard_name])
+                    and (e[-1][hazard_name] > float(self.analysis.threshold))
+                    and (
+                        ("bridge" not in e[-1])
+                        or ("bridge" in e[-1] and e[-1]["bridge"] != "yes")
+                    )
+                )
+            ]
+
+            _graph.remove_edges_from(edges_remove)
 
-        if self.analysis.loss_type == LossTypeEnum.UNIFORM:
-            # assume uniform threshold for disruption
-            self._single_link_losses_uniform(gdf, self.analysis, losses_df)
-
-        if self.analysis.loss_type == LossTypeEnum.CATEGORIZED:
-            _disruption_file = self.static_path.joinpath(
-                "hazard", self.analysis.disruption_per_category
+            columns = [
+                "u",
+                "v",
+                f"alt_{self.analysis.weighing.config_value}",
+                "alt_nodes",
+                f"diff_{self.analysis.weighing.config_value}",
+                "connected",
+            ]
+
+            if "rfid" in gdf:
+                columns.insert(2, "rfid")
+
+            df_calculated = pd.DataFrame(columns=columns)
+            _weighing_analyser = WeighingAnalysisFactory.get_analysis(
+                self.analysis.weighing
             )
-            _disruption_df = pd.read_excel(_disruption_file, sheet_name="Sheet1")
-            self._single_link_losses_categorized(
-                gdf, self.analysis, losses_df, _disruption_df
+
+            for edges in edges_remove:
+                u, v, k, _weighing_analyser.weighing_data = edges
+
+                if nx.has_path(_graph, u, v):
+                    alt_dist = nx.dijkstra_path_length(
+                        _graph, u, v, weight=WeighingEnum.LENGTH.config_value
+                    )
+                    alt_nodes = nx.dijkstra_path(_graph, u, v)
+                    connected = 1
+                    alt_value = _weighing_analyser.calculate_alternative_distance(
+                        alt_dist
+                    )
+                else:
+                    alt_value = _weighing_analyser.calculate_distance()
+                    alt_nodes, connected = np.NaN, 0
+
+                diff = round(
+                    alt_value
+                    - _weighing_analyser.weighing_data[
+                        self.analysis.weighing.config_value
+                    ],
+                    3,
+                )
+
+                data = {
+                    "u": [u],
+                    "v": [v],
+                    f"alt_{self.analysis.weighing.config_value}": [alt_value],
+                    "alt_nodes": [alt_nodes],
+                    f"diff_{self.analysis.weighing.config_value}": diff,
+                    "connected": [connected],
+                }
+                _weighing_analyser.extend_graph(data)
+
+                if "rfid" in gdf:
+                    data["rfid"] = [str(_weighing_analyser.weighing_data["rfid"])]
+
+                df_calculated = pd.concat(
+                    [df_calculated, pd.DataFrame(data)], ignore_index=True
+                )
+            df_calculated[f"alt_{self.analysis.weighing.config_value}"] = pd.to_numeric(
+                df_calculated[f"alt_{self.analysis.weighing.config_value}"],
+                errors="coerce",
             )
 
-        return gdf
+            # Merge the dataframes
+            if "rfid" in gdf:
+                gdf = gdf.merge(df_calculated, how="left", on=["u", "v", "rfid"])
+            else:
+                gdf = gdf.merge(df_calculated, how="left", on=["u", "v"])
+
+            gdf = self._update_time(df_calculated, gdf)
+
+            gdf["hazard"] = hazard_name
+
+            results.append(gdf)
+
+        return pd.concat(results, ignore_index=True)
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/accumulated_traffic_dataclass.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/accumulated_traffic_dataclass.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/equity_analysis.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/equity_analysis.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/README.md` & `ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/README.md`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_base.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import ast
-from collections import defaultdict
 import itertools
 import logging
 from abc import ABC, abstractmethod
+from collections import defaultdict
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
 from ra2ce.analysis.indirect.traffic_analysis.accumulated_traffic_dataclass import (
     AccumulatedTraffic,
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_factory.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/traffic_analysis/traffic_analysis_factory.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/time_weighing_analysis.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/time_weighing_analysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 import geopandas as gpd
+import numpy as np
+import pandas as pd
+
 from ra2ce.analysis.analysis_config_data.enums.weighing_enum import WeighingEnum
 from ra2ce.analysis.indirect.weighing_analysis.weighing_analysis_protocol import (
     WeighingAnalysisProtocol,
 )
 
 
 class TimeWeighingAnalysis(WeighingAnalysisProtocol):
     time_list: list
     weighing_data: dict
 
     def __init__(self) -> None:
         self.time_list = []
 
     def _calculate_time(self) -> float:
-        _calculated_time = round(
-            (self.weighing_data["length"] * 1e-3) / self.weighing_data["avgspeed"],
-            2,
-        )  # in hours and avg speed in km/h
-        self.weighing_data[WeighingEnum.TIME.config_value] = _calculated_time
-        return round(_calculated_time, 2)
+        length = self.weighing_data.get("length", None)
+        avgspeed = self.weighing_data.get("avgspeed", None)
+        if length and avgspeed:
+            _calculated_time = round(
+                (length * 1e-3) / avgspeed,
+                3,
+            )  # in hours and avg speed in km/h
+            self.weighing_data[WeighingEnum.TIME.config_value] = _calculated_time
+            return round(_calculated_time, 3)
+        else:
+            return np.nan
 
     def calculate_distance(self) -> float:
         self.time_list.append(self._calculate_time())
         return self.time_list[-1]
 
     def calculate_alternative_distance(self, alt_dist: float) -> float:
-        alt_time = (alt_dist * 1e-3) / self.weighing_data["avgspeed"]  # in hours
-        self.time_list.append(self._calculate_time())
-        return alt_time
+        avgspeed = self.weighing_data.get("avgspeed", None)
+        if avgspeed:
+            alt_time = (alt_dist * 1e-3) / avgspeed  # in hours
+            self.time_list.append(self._calculate_time())
+            return alt_time
+        else:
+            return np.nan
 
     def extend_graph(self, gdf_graph: gpd.GeoDataFrame | dict) -> None:
-        gdf_graph[WeighingEnum.TIME.config_value] = self.time_list
+        if isinstance(gdf_graph, gpd.GeoDataFrame):
+            gdf_graph[WeighingEnum.TIME.config_value] = self.time_list
+        elif isinstance(gdf_graph, dict):
+            gdf_graph[WeighingEnum.TIME.config_value] = [self.time_list[-1]]
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_factory.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 )
 from ra2ce.analysis.indirect.weighing_analysis.weighing_analysis_protocol import (
     WeighingAnalysisProtocol,
 )
 
 
 class WeighingAnalysisFactory:
-
     @staticmethod
     def get_analysis(weighing_type: WeighingEnum) -> WeighingAnalysisProtocol:
         if weighing_type == WeighingEnum.TIME:
             return TimeWeighingAnalysis()
         if weighing_type == WeighingEnum.LENGTH:
             return LengthWeighingAnalysis()
```

### Comparing `ra2ce-0.8.1/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_protocol.py` & `ra2ce-0.9.0/ra2ce/analysis/indirect/weighing_analysis/weighing_analysis_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Protocol, runtime_checkable
+
 import geopandas as gpd
 
 
 @runtime_checkable
 class WeighingAnalysisProtocol(Protocol):
     weighing_data: dict
```

### Comparing `ra2ce-0.8.1/ra2ce/common/configuration/config_data_protocol.py` & `ra2ce-0.9.0/ra2ce/common/configuration/config_data_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/configuration/config_wrapper_protocol.py` & `ra2ce-0.9.0/ra2ce/common/configuration/config_wrapper_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/configuration/ini_configuration_reader_protocol.py` & `ra2ce-0.9.0/ra2ce/common/configuration/ini_configuration_reader_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/io/readers/file_reader_protocol.py` & `ra2ce-0.9.0/ra2ce/common/io/readers/file_reader_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/io/readers/graph_pickle_reader.py` & `ra2ce-0.9.0/ra2ce/common/io/readers/graph_pickle_reader.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/io/README.md` & `ra2ce-0.9.0/ra2ce/common/io/README.md`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/io/writers/ra2ce_exporter_protocol.py` & `ra2ce-0.9.0/ra2ce/common/io/writers/ra2ce_exporter_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/README.md` & `ra2ce-0.9.0/ra2ce/common/README.md`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/validation/ra2ce_validator_protocol.py` & `ra2ce-0.9.0/ra2ce/common/validation/ra2ce_validator_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/common/validation/validation_report.py` & `ra2ce-0.9.0/ra2ce/common/validation/validation_report.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/configuration/config_factory.py` & `ra2ce-0.9.0/ra2ce/configuration/config_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 from pathlib import Path
 from typing import Optional
 
 from ra2ce.analysis.analysis_config_data.analysis_config_data import AnalysisConfigData
 from ra2ce.analysis.analysis_config_data.analysis_config_data_reader import (
     AnalysisConfigDataReader,
 )
-from ra2ce.analysis.analysis_config_wrapper import (
-    AnalysisConfigWrapper,
-)
+from ra2ce.analysis.analysis_config_wrapper import AnalysisConfigWrapper
 from ra2ce.configuration.config_wrapper import ConfigWrapper
 from ra2ce.network.network_config_data.network_config_data_reader import (
     NetworkConfigDataReader,
 )
 from ra2ce.network.network_config_wrapper import NetworkConfigWrapper
```

### Comparing `ra2ce-0.8.1/ra2ce/configuration/config_wrapper.py` & `ra2ce-0.9.0/ra2ce/configuration/config_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from __future__ import annotations
 
 import logging
 
-from ra2ce.analysis.analysis_config_wrapper import (
-    AnalysisConfigWrapper,
-)
+from ra2ce.analysis.analysis_config_wrapper import AnalysisConfigWrapper
 from ra2ce.network.network_config_wrapper import NetworkConfigWrapper
 
 
 class ConfigWrapper:
     network_config: NetworkConfigWrapper
     analysis_config: AnalysisConfigWrapper
```

### Comparing `ra2ce-0.8.1/ra2ce/configuration/ra2ce_enum_base.py` & `ra2ce-0.9.0/ra2ce/configuration/ra2ce_enum_base.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/exporters/geodataframe_network_exporter.py` & `ra2ce-0.9.0/ra2ce/network/exporters/geodataframe_network_exporter.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/exporters/json_exporter.py` & `ra2ce-0.9.0/ra2ce/network/exporters/json_exporter.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/exporters/multi_graph_network_exporter.py` & `ra2ce-0.9.0/ra2ce/network/exporters/multi_graph_network_exporter.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/exporters/network_exporter_base.py` & `ra2ce-0.9.0/ra2ce/network/exporters/network_exporter_base.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/exporters/network_exporter_factory.py` & `ra2ce-0.9.0/ra2ce/network/exporters/network_exporter_factory.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/graph_files/graph_file.py` & `ra2ce-0.9.0/ra2ce/network/graph_files/graph_file.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/graph_files/graph_files_collection.py` & `ra2ce-0.9.0/ra2ce/network/graph_files/graph_files_collection.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/graph_files/graph_files_protocol.py` & `ra2ce-0.9.0/ra2ce/network/graph_files/graph_files_protocol.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/graph_files/network_file.py` & `ra2ce-0.9.0/ra2ce/network/graph_files/network_file.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_common_functions.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_common_functions.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_files.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_files.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_base.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_base.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_gpkg.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_gpkg.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,26 +26,22 @@
 from geopandas import GeoDataFrame, read_file, sjoin
 from networkx import Graph
 from numpy import nanmean
 
 from ra2ce.network.hazard.hazard_intersect.hazard_intersect_builder_base import (
     HazardIntersectBuilderBase,
 )
-from ra2ce.network.hazard.hazard_intersect.hazard_intersect_parallel_run import (
-    get_hazard_parallel_process,
-)
 
 
 @dataclass
 class HazardIntersectBuilderForGpkg(HazardIntersectBuilderBase):
     hazard_field_name: str = ""
     hazard_aggregate_wl: str = ""
-    hazard_names: list[str] = field(default_factory=list)
     ra2ce_names: list[str] = field(default_factory=list)
-    hazard_gpkg_files: list[str] = field(default_factory=list)
+    hazard_gpkg_files: list[Path] = field(default_factory=list)
 
     def _from_networkx(self, hazard_overlay: Graph) -> Graph:
         """Overlays the hazard `gpkg` file over the road segments NetworkX graph.
 
         Args:
             hazard_overlay (NetworkX graph): The graph that should be overlayed with the hazard `gpkg` file(s).
 
@@ -86,18 +82,16 @@
                             race_name + "_" + self.hazard_aggregate_wl[:2]
                         ] = 0
                 else:
                     hazard_overlay[u][v][k][
                         race_name + "_" + self.hazard_aggregate_wl[:2]
                     ] = 0
 
-        # Run in parallel to boost performance.
-        self._overlay_in_parallel(networkx_overlay)
-        # for i, _ra2ce_name in self.ra2ce_names:
-        #     networkx_overlay(self.hazard_shp_files[i], _ra2ce_name)
+        self._overlay_hazard_files(networkx_overlay)
+
         return hazard_overlay
 
     def _from_geodataframe(self, hazard_overlay: GeoDataFrame) -> GeoDataFrame:
         """Overlays the hazard shapefile over the road segments GeoDataFrame. The gdf is reprojected to the hazard shapefile if necessary.
 
         Args:
             hazard_overlay (GeoDataFrame): the network geodataframe that should be overlayed with the hazard shapefile(s)
@@ -123,26 +117,17 @@
                     self.hazard_field_name: ra2ce_name
                     + "_"
                     + self.hazard_aggregate_wl[:2]
                 },
                 inplace=True,
             )
 
-        # Run in parallel to boost performance.
-        self._overlay_in_parallel(geodataframe_overlay)
-        # for i, _ra2ce_name in self.ra2ce_names:
-        #     geodataframe_overlay(self.hazard_shp_files[i], _ra2ce_name)
+        self._overlay_hazard_files(geodataframe_overlay)
 
         if hazard_overlay.crs != gdf_crs_original:
             hazard_overlay = hazard_overlay.to_crs(gdf_crs_original)
 
         return hazard_overlay
 
-    def _overlay_in_parallel(self, overlay_func: Callable):
-        # Run in parallel to boost performance.
-        get_hazard_parallel_process(
-            overlay_func,
-            lambda delayed_func: (
-                delayed_func(self.hazard_gpkg_files[i], _ra2ce_name)
-                for i, _ra2ce_name in enumerate(self.ra2ce_names)
-            ),
-        )
+    def _overlay_hazard_files(self, overlay_func: Callable[[str, str], None]):
+        for i, _ra2ce_name in enumerate(self.ra2ce_names):
+            overlay_func(self.hazard_gpkg_files[i], _ra2ce_name)
```

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_table.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,15 @@
 from geopandas import GeoDataFrame
 from networkx import Graph
 from pandas import read_csv
 
 from ra2ce.network.hazard.hazard_intersect.hazard_intersect_builder_base import (
     HazardIntersectBuilderBase,
 )
-from ra2ce.network.networks_utils import (
-    graph_from_gdf,
-    graph_to_gdf,
-)
+from ra2ce.network.networks_utils import graph_from_gdf, graph_to_gdf
 
 
 @dataclass
 class HazardIntersectBuilderForTable(HazardIntersectBuilderBase):
     hazard_field_name: str = ""
     network_file_id: str = ""
     hazard_id: str = ""
```

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_tif.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_for_tif.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,15 @@
 from ra2ce.network.hazard.hazard_common_functions import (
     get_edges_geoms,
     validate_extent_graph,
 )
 from ra2ce.network.hazard.hazard_intersect.hazard_intersect_builder_base import (
     HazardIntersectBuilderBase,
 )
-from ra2ce.network.hazard.hazard_intersect.hazard_intersect_parallel_run import (
-    get_hazard_parallel_process,
-)
+
 from ra2ce.network.networks_utils import (
     fraction_flooded,
     get_graph_edges_extent,
     get_valid_mean,
 )
 
 
@@ -158,16 +156,15 @@
                 hazard_overlay,
                 {
                     (edges[0], edges[1], edges[2]): {ra2ce_name + "_fr": x}
                     for x, edges in zip(graph_fraction_flooded, edges_geoms)
                 },
             )
 
-        # Run in parallel to boost performance.
-        self._overlay_in_parallel(overlay_network_x)
+        self._overlay_hazard_files(overlay_network_x)
         return hazard_overlay
 
     def _from_geodataframe(self, hazard_overlay: GeoDataFrame):
         """Overlays the hazard raster over the road segments GeoDataFrame.
 
         Args:
             *graph* (GeoDataFrame) : GeoDataFrame that will be intersected with the hazard map raster.
@@ -227,20 +224,13 @@
             ) = list(zip(*map(_get_attributes, flood_stats)))
 
             tqdm.pandas(desc="Network fraction with hazard overlay with " + hazard_name)
             hazard_overlay[ra2ce_name + "_fr"] = hazard_overlay.geometry.progress_apply(
                 lambda x, _hz_str=_hazard_files_str: fraction_flooded(x, _hz_str)
             )
 
-        # Run in parallel to boost performance.
-        self._overlay_in_parallel(overlay_geodataframe)
+        self._overlay_hazard_files(overlay_geodataframe)
         return hazard_overlay
 
-    def _overlay_in_parallel(self, overlay_func: Callable):
-        # Run in parallel to boost performance.
-        get_hazard_parallel_process(
-            overlay_func,
-            lambda delayed_func: (
-                delayed_func(self.hazard_tif_files[i], hn, rn)
-                for i, (hn, rn) in enumerate(self._combined_names)
-            ),
-        )
+    def _overlay_hazard_files(self, overlay_func: Callable[[str, str, str], None]):
+        for i, (hn, rn) in enumerate(self._combined_names):
+            overlay_func(self.hazard_tif_files[i], hn, rn)
```

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_protocol.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_intersect/hazard_intersect_builder_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from typing import Protocol
+
 from geopandas import GeoDataFrame
 from networkx import Graph
 
 
 class HazardIntersectBuilderProtocol(Protocol):
     def get_intersection(
         self, hazard_overlay: GeoDataFrame | Graph
```

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_intersect/hazard_intersect_parallel_run.py` & `ra2ce-0.9.0/ra2ce/network/network_wrappers/network_wrapper_protocol.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,27 +14,23 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
+from typing import Protocol, runtime_checkable
 
-# This file contains the common utils to run a method in parallel
-from joblib import Parallel, delayed
-from typing import Callable
+from geopandas import GeoDataFrame
+from networkx import MultiGraph
 
 
-def get_hazard_parallel_process(
-    delegated_func: Callable, func_iterable: Callable
-) -> None:
-    """
-    Runs in parallel a delegated process which will consume using the `delayed` method together
-    with its associated parameters to retrieve from `func_iterable`.
+@runtime_checkable
+class NetworkWrapperProtocol(Protocol):
+    def get_network(self) -> tuple[MultiGraph, GeoDataFrame]:
+        """
+        Gets a network built within this wrapper instance. No arguments are accepted, the `__init__` method is meant to assign all required attributes for a wrapper.
 
-    Args:
-        delegated_func (Callable): Method signature which will be run in parallel.
-        func_iterable (Callable): Method generating the arguments required for `delegated_func`.
-    """
-    return Parallel(n_jobs=2, require="sharedmem")(
-        func_iterable(delayed(delegated_func))
-    )
+        Returns:
+            tuple[MultiGraph, GeoDataFrame]: Tuple of MultiGraph representing the graph and GeoDataFrame representing the network.
+        """
+        pass
```

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_names.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_names.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/hazard/hazard_overlay.py` & `ra2ce-0.9.0/ra2ce/network/hazard/hazard_overlay.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,19 +433,18 @@
                 ra2ce_names=self.ra2ce_names,
                 hazard_tif_files=self.hazard_files.tif,
             ).get_intersection(to_overlay)
         elif self.hazard_files.gpkg:
             return HazardIntersectBuilderForGpkg(
                 hazard_field_name=self._hazard_field_name,
                 hazard_aggregate_wl=self._hazard_aggregate_wl,
-                hazard_names=self.hazard_names,
                 ra2ce_names=self.ra2ce_names,
                 hazard_gpkg_files=self.hazard_files.gpkg,
             ).get_intersection(to_overlay)
-        elif self.hazard["table"]:
+        elif self.hazard_files["table"]:
             return HazardIntersectBuilderForTable(
                 hazard_field_name=self._hazard_field_name,
                 network_file_id=self._network_file_id,
                 hazard_id=self._hazard_id,
                 ra2ce_name_key=self._ra2ce_name_key,
             ).get_intersection(to_overlay)
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_config_data/enums/source_enum.py` & `ra2ce-0.9.0/ra2ce/network/network_config_data/enums/source_enum.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/network_config_data/network_config_data.py` & `ra2ce-0.9.0/ra2ce/network/network_config_data/network_config_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 @dataclass
 class NetworkSection:
     directed: bool = False
     source: SourceEnum = field(default_factory=lambda: SourceEnum.INVALID)
     primary_file: list[Path] = field(default_factory=list)
     diversion_file: list[Path] = field(default_factory=list)
     file_id: str = ""
+    link_type_column: str = ""
     polygon: Optional[Path] = None
     network_type: NetworkTypeEnum = field(default_factory=lambda: NetworkTypeEnum.NONE)
     road_types: list[RoadTypeEnum] = field(default_factory=list)
     save_gpkg: bool = False
 
 
 @dataclass
@@ -76,23 +77,25 @@
 @dataclass
 class HazardSection:
     hazard_map: list[Path] = field(default_factory=list)
     hazard_id: str = ""
     hazard_field_name: list[str] = field(default_factory=list)
     aggregate_wl: AggregateWlEnum = field(default_factory=lambda: AggregateWlEnum.NONE)
     hazard_crs: str = ""
+    scenario_cost: list[float] = field(default_factory=list)
 
 
 @dataclass
 class CleanupSection:
     snapping_threshold: bool = False
     pruning_threshold: bool = False
     segmentation_length: float = float("nan")
     merge_lines: bool = False
     cut_at_intersections: bool = False
+    delete_duplicate_nodes: bool = False
 
 
 @dataclass
 class NetworkConfigData(ConfigDataProtocol):
     root_path: Optional[Path] = None
     input_path: Optional[Path] = None
     output_path: Optional[Path] = None
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_config_data/network_config_data_reader.py` & `ra2ce-0.9.0/ra2ce/network/network_config_data/network_config_data_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Any, Union
 
 from ra2ce.common.configuration.ini_configuration_reader_protocol import (
     ConfigDataReaderProtocol,
 )
@@ -22,15 +23,15 @@
 
 class NetworkConfigDataReader(ConfigDataReaderProtocol):
     _parser: ConfigParser
 
     def __init__(self) -> None:
         self._parser = ConfigParser(
             inline_comment_prefixes="#",
-            converters={"list": lambda x: [x.strip() for x in x.split(",")]},
+            converters={"list": lambda x: [x.strip() for x in re.split("[,|;]", x)]},
         )
 
     def read(self, ini_file: Path) -> NetworkConfigData:
         self._parser.read(ini_file)
         self._remove_none_values()
 
         _parent_dir = ini_file.parent
@@ -170,33 +171,38 @@
             )
         )
         _network_section.polygon = self._get_str_as_path(_network_section.polygon)
         return _network_section
 
     def get_origins_destinations_section(self) -> OriginsDestinationsSection:
         _section = "origins_destinations"
+        if _section not in self._parser:
+            return OriginsDestinationsSection()
+
         _od_section = OriginsDestinationsSection(**self._parser[_section])
         _od_section.origin_out_fraction = self._parser.getint(
             _section, "origin_out_fraction", fallback=_od_section.origin_out_fraction
         )
         _od_section.origins = self._get_str_as_path(_od_section.origins)
         _od_section.destinations = self._get_str_as_path(_od_section.destinations)
         _od_section.region = self._get_str_as_path(_od_section.region)
         return _od_section
 
     def get_isolation_section(self) -> IsolationSection:
         _section = "isolation"
         if _section not in self._parser:
             return IsolationSection()
+
         return IsolationSection(**self._parser[_section])
 
     def get_hazard_section(self) -> HazardSection:
         _section = "hazard"
         if _section not in self._parser:
             return HazardSection()
+
         _hazard_section = HazardSection(**self._parser[_section])
         _hazard_section.hazard_map = list(
             map(
                 self._get_str_as_path,
                 self._parser.getlist(
                     _section, "hazard_map", fallback=_hazard_section.hazard_map
                 ),
@@ -204,18 +210,25 @@
         )
         _hazard_section.hazard_field_name = self._parser.getlist(
             _section, "hazard_field_name", fallback=_hazard_section.hazard_field_name
         )
         _hazard_section.aggregate_wl = AggregateWlEnum.get_enum(
             self._parser.get(_section, "aggregate_wl", fallback=None)
         )
+        _hazard_section.scenario_cost = list(
+            self._parser.getlist(
+                _section, "scenario_cost", fallback=_hazard_section.scenario_cost
+            )
+        )
         return _hazard_section
 
     def get_cleanup_section(self) -> CleanupSection:
         _section = "cleanup"
+        if _section not in self._parser:
+            return CleanupSection()
 
         _cleanup_section = CleanupSection()
         _cleanup_section.snapping_threshold = self._parser.getboolean(
             _section,
             "snapping_threshold",
             fallback=_cleanup_section.snapping_threshold,
         )
@@ -233,8 +246,13 @@
             _section, "merge_lines", fallback=_cleanup_section.merge_lines
         )
         _cleanup_section.cut_at_intersections = self._parser.getboolean(
             _section,
             "cut_at_intersections",
             fallback=_cleanup_section.cut_at_intersections,
         )
+        _cleanup_section.delete_duplicate_nodes = self._parser.getboolean(
+            _section,
+            "delete_duplicate_nodes",
+            fallback=_cleanup_section.delete_duplicate_nodes,
+        )
         return _cleanup_section
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_config_data/network_config_data_validator.py` & `ra2ce-0.9.0/ra2ce/network/network_config_data/network_config_data_validator.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/network_config_data/README.md` & `ra2ce-0.9.0/ra2ce/network/network_config_data/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-# Network config data module.
+# Network config data
 
-In this module we contain the representation of a network configuration file, its readers and validators.
+In this package we contain the representation of a network configuration file, its readers and validators.
 
 - `network_config_data.py` contains the main `dataclass` `NetworkConfigData` which has the properties representing each of the different INI sections as `dataclasses`.
 - `network_config_data_validator.py` contains the logic to validate all properties of a `NetworkConfigData`.
 - `network_config_data.py` contains the `NetworkConfigDataReader`, an `*.ini` file reader that parses its content into an instance of a `NetworkConfigData`.
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_config_wrapper.py` & `ra2ce-0.9.0/ra2ce/network/network_config_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,10 +99,8 @@
             return
 
         # There is a hazard map or multiple hazard maps that should be intersected with the graph.
         hazard = HazardOverlay(self.config_data, self.graph_files)
         self.graph_files = hazard.create()
 
     def is_valid(self) -> bool:
-        _file_is_valid = self.ini_file.is_file() and self.ini_file.suffix == ".ini"
-        _validation_report = NetworkConfigDataValidator(self.config_data).validate()
-        return _file_is_valid and _validation_report.is_valid()
+        return NetworkConfigDataValidator(self.config_data).validate().is_valid()
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_wrappers/network_wrapper_factory.py` & `ra2ce-0.9.0/ra2ce/network/network_wrappers/network_wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/network_wrappers/network_wrapper_protocol.py` & `ra2ce-0.9.0/ra2ce/runners/analysis_runner_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,23 +14,42 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
-from typing import Protocol, runtime_checkable
 
-from geopandas import GeoDataFrame
-from networkx import MultiGraph
+import logging
 
+from ra2ce.configuration.config_wrapper import ConfigWrapper
+from ra2ce.runners.analysis_runner_protocol import AnalysisRunner
+from ra2ce.runners.direct_analysis_runner import DirectAnalysisRunner
+from ra2ce.runners.indirect_analysis_runner import IndirectAnalysisRunner
 
-@runtime_checkable
-class NetworkWrapperProtocol(Protocol):
-    def get_network(self) -> tuple[MultiGraph, GeoDataFrame]:
+
+class AnalysisRunnerFactory:
+    @staticmethod
+    def get_runner(ra2ce_input: ConfigWrapper) -> AnalysisRunner:
         """
-        Gets a network built within this wrapper instance. No arguments are accepted, the `__init__` method is meant to assign all required attributes for a wrapper.
+        Gets the supported first analysis runner for the given input. The runner is initialized within this method.
+
+        Args:
+            ra2ce_input (Ra2ceInput): Input representing a set of network and analysis ini configurations.
 
         Returns:
-            tuple[MultiGraph, GeoDataFrame]: Tuple of MultiGraph representing the graph and GeoDataFrame representing the network.
+            AnalysisRunner: Initialized Ra2ce analysis runner.
         """
-        pass
+        _available_runners = [DirectAnalysisRunner, IndirectAnalysisRunner]
+        _supported_runners = [
+            _runner for _runner in _available_runners if _runner.can_run(ra2ce_input)
+        ]
+        if not _supported_runners:
+            _err_mssg = "No analysis runner found for the given configuration."
+            logging.error(_err_mssg)
+            raise ValueError(_err_mssg)
+
+        # Initialized selected supported runner (First one available).
+        _selected_runner = _supported_runners[0]()
+        if len(_supported_runners) > 1:
+            logging.warning(f"More than one runner available, using {_selected_runner}")
+        return _selected_runner
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_wrappers/osm_network_wrapper/extremities_data.py` & `ra2ce-0.9.0/ra2ce/network/network_wrappers/osm_network_wrapper/extremities_data.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/network_wrappers/osm_network_wrapper/osm_network_wrapper.py` & `ra2ce-0.9.0/ra2ce/network/network_wrappers/osm_network_wrapper/osm_network_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,34 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from __future__ import annotations
+
 import logging
 from pathlib import Path
 from typing import Any
 
 import networkx as nx
 import osmnx
 import pandas as pd
 from geopandas import GeoDataFrame
 from networkx import MultiDiGraph, MultiGraph
 from shapely.geometry.base import BaseGeometry
-from ra2ce.network.network_config_data.enums.network_type_enum import NetworkTypeEnum
-from ra2ce.network.network_config_data.enums.road_type_enum import RoadTypeEnum
+import pyproj
+from ra2ce.network.network_wrappers.osm_network_wrapper.osm_utils import (
+    get_node_nearest_edge, is_endnode_check, modify_graph, remove_key
+)
 
 import ra2ce.network.networks_utils as nut
 from ra2ce.network.exporters.json_exporter import JsonExporter
+from ra2ce.network.network_config_data.enums.network_type_enum import NetworkTypeEnum
+from ra2ce.network.network_config_data.enums.road_type_enum import RoadTypeEnum
 from ra2ce.network.network_config_data.network_config_data import NetworkConfigData
 from ra2ce.network.network_wrappers.network_wrapper_protocol import (
     NetworkWrapperProtocol,
 )
 from ra2ce.network.network_wrappers.osm_network_wrapper.extremities_data import (
     ExtremitiesData,
 )
@@ -408,9 +413,23 @@
     @staticmethod
     def snap_nodes_to_nodes(graph: MultiDiGraph, threshold: float) -> MultiDiGraph:
         return osmnx.consolidate_intersections(
             G=graph, rebuild_graph=True, tolerance=threshold, dead_ends=False
         )
 
     @staticmethod
-    def snap_nodes_to_edges(graph: MultiDiGraph, threshold: float):
-        raise NotImplementedError("Next thing to do!")
+    def snap_nodes_to_edges(graph: MultiDiGraph, threshold: float) -> MultiDiGraph:
+        def threshold_check(node_nearest_ed: dict):
+            distance = node_nearest_ed['nearest_edge'][-1]
+            return distance <= threshold
+
+        end_nodes = [node for node in graph.nodes(data=True) if is_endnode_check(graph, node[0])]
+
+        if not graph.graph or not graph.graph['crs'] or isinstance(graph.graph['crs'], str):
+            graph.graph['crs'] = pyproj.CRS("epsg:4326")
+        nut.add_missing_geoms_graph(graph=graph, geom_name='geometry').to_directed()
+
+        for node_nearest_edge_data in filter(threshold_check,
+                                             map(lambda end_node:
+                                                 get_node_nearest_edge(graph, end_node), end_nodes)):
+            modify_graph(graph=graph, node_nearest_edge_data=node_nearest_edge_data)
+        return graph
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_wrappers/shp_network_wrapper.py` & `ra2ce-0.9.0/ra2ce/network/network_wrappers/shp_network_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             edges, nodes, id_name, tolerance=0.00001, crs_=self.crs
         )  ## PAY ATTENTION TO THE TOLERANCE, THE UNIT IS DEGREES
         logging.info("Function [cut_lines]: executed")
 
         if not edges.crs:
             edges.crs = self.crs
 
-        # create tuples from the adjecent nodes and add as column in geodataframe
+        # create tuples from the adjacent nodes and add as column in geodataframe
         edges_complex = nut.join_nodes_edges(nodes, edges, id_name)
         edges_complex.crs = self.crs  # set the right CRS
         edges_complex.dropna(subset=["node_A", "node_B"], inplace=True)
 
         assert (
             edges_complex["node_A"].isnull().sum() == 0
         ), "Some edges cannot be assigned nodes, please check your input shapefile."
```

### Comparing `ra2ce-0.8.1/ra2ce/network/network_wrappers/trails_network_wrapper.py` & `ra2ce-0.9.0/ra2ce/network/network_wrappers/trails_network_wrapper.py`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/ra2ce/network/network_wrappers/vector_network_wrapper.py` & `ra2ce-0.9.0/ra2ce/network/segmentation.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,220 +16,175 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import logging
-from pathlib import Path
+from decimal import Decimal
 
 import geopandas as gpd
-import momepy
-import networkx as nx
-import pandas as pd
-from shapely.geometry import Point
-
-import ra2ce.network.networks_utils as nut
-from ra2ce.network.network_config_data.network_config_data import NetworkConfigData
-from ra2ce.network.network_wrappers.network_wrapper_protocol import (
-    NetworkWrapperProtocol,
-)
+from shapely.geometry import LineString, MultiLineString, Point
 
+from ra2ce.network.networks_utils import cut as network_cut
 
-class VectorNetworkWrapper(NetworkWrapperProtocol):
-    """A class for handling and manipulating vector files.
 
-    Provides methods for reading vector data, cleaning it, and setting up graph and
-    network.
-    """
-
-    def __init__(
-        self,
-        config_data: NetworkConfigData,
-    ) -> None:
-        self.crs = config_data.crs
-
-        # Network options
-        self.primary_files = config_data.network.primary_file
-        self.directed = config_data.network.directed
-
-        # Origins Destinations
-        self.region_path = config_data.origins_destinations.region
-
-    def get_network(
-        self,
-    ) -> tuple[nx.MultiGraph, gpd.GeoDataFrame]:
-        """Gets a network built from vector files.
+class Segmentation:  # Todo: more naturally, this would be METHOD of the network class.
+    """cut the edges in the complex geodataframe to segments of equal lengths or smaller
+    # output will be the cut edges_complex
 
-        Returns:
-            nx.MultiGraph: MultiGraph representing the graph.
-            gpd.GeoDataFrame: GeoDataFrame representing the network.
-        """
-        gdf = self._read_vector_to_project_region_and_crs()
-        gdf = self.clean_vector(gdf)
-        if self.directed:
-            graph = self.get_direct_graph_from_vector(gdf)
-        else:
-            graph = self.get_indirect_graph_from_vector(gdf)
-        edges, nodes = self.get_network_edges_and_nodes_from_graph(graph)
-        graph_complex = nut.graph_from_gdf(edges, nodes, node_id="node_fid")
-        return graph_complex, edges
-
-    def _read_vector_to_project_region_and_crs(self) -> gpd.GeoDataFrame:
-        gdf = self._read_files(self.primary_files)
-        if gdf is None:
-            logging.info("no file is read.")
-            return None
-
-        # set crs and reproject if needed
-        if not gdf.crs and self.crs:
-            gdf = gdf.set_crs(self.crs)
-            logging.info("setting crs as default EPSG:4326. specify crs if incorrect")
-
-        if self.crs:
-            gdf = gdf.to_crs(self.crs)
-            logging.info("reproject vector file to project crs")
-
-        # clip for region
-        if self.region_path:
-            _region_gpd = self._read_files([self.region_path])
-            gdf = gpd.overlay(gdf, _region_gpd, how="intersection", keep_geom_type=True)
-            logging.info("clip vector file to project region")
-
-        # validate
-        if not any(gdf):
-            logging.warning("No vector features found within project region")
-            return None
+    Variables:
+        *self.edges_input* (Geopandas DataFrame) : the edges that are to be segmented
+        *self.segmentation_length* (float) : segmentation lenght in degrees #Todo also in meters?
+        *self.save_files* (Boolean) : save segmented graph?
 
-        return gdf
+    Result:
+        *self.edges_segmented* (Geopandas DataFrame) : the segmented edges dataframe
 
-    def _read_files(self, file_list: list[Path]) -> gpd.GeoDataFrame:
-        """Reads a list of files into a GeoDataFrame.
 
-        Args:
-            file_list (list[Path]): List of file paths.
+    """
 
-        Returns:
-            gpd.GeoDataFrame: GeoDataFrame representing the data.
-        """
-        # read file
-        gdf = gpd.GeoDataFrame(
-            pd.concat([gpd.read_file(_fl, engine="pyogrio") for _fl in file_list])
+    def __init__(self, edges_input, segmentation_length, save_files: bool = False):
+        # General
+        self.edges_input = edges_input  # Edges GeoDataFrame
+        self.edges_segmented = (
+            None  # This is where the result will be saved Edges GeoDataframe
         )
+        self.segmentation_length = segmentation_length
+        self.save_files = save_files  # Todo not implemented yet
+
+    def apply_segmentation(self):
+        self.cut_gdf()
         logging.info(
-            "Read files {} into a 'GeoDataFrame'.".format(
-                ", ".join(map(str, file_list))
+            "Finished segmenting the geodataframe with split length: {} degree".format(
+                self.segmentation_length
             )
         )
-        return gdf
+        return self.edges_segmented
 
-    @staticmethod
-    def get_direct_graph_from_vector(gdf: gpd.GeoDataFrame) -> nx.DiGraph:
-        """Creates a simple directed graph with node and edge geometries based on a given GeoDataFrame.
+    def cut(self, line: LineString, distance: float) -> list:
+        """Cuts a line in two at a distance from its starting point
 
         Args:
-            gdf (gpd.GeoDataFrame): Input GeoDataFrame containing line geometries.
-                Allow both LineString and MultiLineString.
+            line (LineString): Single linestring.
+            distance (float): Distance from starting point of linestring
 
         Returns:
-            nx.DiGraph: NetworkX graph object with "crs", "approach" as graph properties.
+            (list): A list containing two shapely linestring objects.
         """
 
-        # simple geometry handeling
-        gdf = VectorNetworkWrapper.explode_and_deduplicate_geometries(gdf)
-
-        # to graph
-        digraph = nx.DiGraph(crs=gdf.crs, approach="primal")
-        for _, row in gdf.iterrows():
-            link_id = row.get("link_id", None)
-
-            from_node = row.geometry.coords[0]
-            to_node = row.geometry.coords[-1]
-            digraph.add_node(from_node, geometry=Point(from_node))
-            digraph.add_node(to_node, geometry=Point(to_node))
-            digraph.add_edge(
-                from_node,
-                to_node,
-                link_id=link_id,
-                avgspeed=row.pop("avgspeed") if "avgspeed" in row else None,
-                geometry=row.pop(
-                    "geometry"
-                ),  # **row TODO: check if we do need all columns
-            )
-
-        return digraph
+        if distance <= 0.0 or distance >= line.length:
+            return [LineString(line)]
+        coords = list(line.coords)
+        for i, p in enumerate(coords):
+            pd = line.project(Point(p))
+            if pd == distance:
+                return [LineString(coords[: i + 1]), LineString(coords[i:])]
+            if pd > distance:
+                cp = line.interpolate(distance)
+                return [
+                    LineString(coords[:i] + [(cp.x, cp.y)]),
+                    LineString([(cp.x, cp.y)] + coords[i:]),
+                ]
 
-    @staticmethod
-    def get_indirect_graph_from_vector(gdf: gpd.GeoDataFrame) -> nx.Graph:
-        """Creates a simple undirected graph with node and edge geometries based on a given GeoDataFrame.
+    def check_divisibility(self, dividend, divisor):
+        """Checks if the dividend is a multiple of the divisor and outputs a boolean value
 
         Args:
-            gdf (gpd.GeoDataFrame): Input GeoDataFrame containing line geometries.
-                Allow both LineString and MultiLineString.
+            dividend (float): The number which is divided
+            divisor (float): The number which divides
 
         Returns:
-            nx.Graph: NetworkX graph object with "crs", "approach" as graph properties.
+            is_multiple (bool): True if the dividend is a multiple of the divisor, False if not
         """
-        digraph = VectorNetworkWrapper.get_direct_graph_from_vector(gdf)
-        return digraph.to_undirected()
 
-    @staticmethod
-    def get_network_edges_and_nodes_from_graph(
-        graph: nx.Graph,
-    ) -> tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]:
-        """Sets up network nodes and edges from a given graph.
+        dividend = Decimal(str(dividend))
+        divisor = Decimal(str(divisor))
+        remainder = dividend % divisor
+
+        return remainder == Decimal("0")
+
+    def number_of_segments(self, linestring: LineString, split_length: float) -> int:
+        """Returns the integer number of segments which will result from chopping up a linestring with split_length
 
         Args:
-            graph (nx.Graph): Input graph with geometry for nodes and edges.
-                Must contain "crs" as graph property.
+            linestring (LineString): Single linestring.
+            split_length (float): The length by which to divide the linestring object.
 
         Returns:
-            gpd.GeoDataFrame: GeoDataFrame representing the network edges with "edge_fid", "node_A", and "node_B".
-            gpd.GeoDataFrame: GeoDataFrame representing the network nodes with "node_fid".
+            n (int): Integer number of segments which will result from splitting linestring with split_length.
         """
 
-        # TODO ths function use conventions. Good to make consistant convention with osm
-        nodes, edges = momepy.nx_to_gdf(graph, nodeID="node_fid")
-        edges["edge_fid"] = (
-            edges["node_start"].astype(str) + "_" + edges["node_end"].astype(str)
-        )
-        edges.rename(
-            {"node_start": "node_A", "node_end": "node_B"}, axis=1, inplace=True
-        )
-        if not nodes.crs:
-            nodes.crs = graph.graph["crs"]
-        if not edges.crs:
-            edges.crs = graph.graph["crs"]
-        return edges, nodes
-
-    @staticmethod
-    def clean_vector(gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
-        """Cleans a GeoDataFrame.
+        divisible = self.check_divisibility(linestring.length, split_length)
+        if divisible:
+            return int(linestring.length / split_length)
+        return int(linestring.length / split_length) + 1
+
+    def split_linestring(self, linestring: LineString, split_length: float):
+        """Cuts a linestring in equivalent segments of length split_length
 
         Args:
-            gdf (gpd.GeoDataFrame): Input GeoDataFrame.
+            linestring (LineString): Single linestring.
+            split_length (float): Length by which to split the linestring into equal segments.
 
         Returns:
-            gpd.GeoDataFrame: Cleaned GeoDataFrame.
+            result_list (list): List of LineString objects that all have the same length split_lenght.
         """
 
-        gdf = VectorNetworkWrapper.explode_and_deduplicate_geometries(gdf)
+        n_segments = self.number_of_segments(linestring, split_length)
+        if n_segments != 1:
+            result_list = [None] * n_segments
+            current_right_linestring = linestring
+
+            for i in range(0, n_segments - 1):
+                r = network_cut(current_right_linestring, split_length)
+                # Can accidently return Nonetypes
+                if r is not None:
+                    current_left_linestring = r[0]
+                    current_right_linestring = r[1]
+                    result_list[i] = current_left_linestring
+                    result_list[i + 1] = current_right_linestring
+                # Sometimes the remainder is so small that it is only one point, which cannot be cut, in that case
+                # just pass #Todo: maybe we can do something here to avoid this error
 
-        return gdf
+        else:
+            result_list = [linestring]
 
-    @staticmethod
-    def explode_and_deduplicate_geometries(gpd: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
-        """Explodes and deduplicates geometries a GeoDataFrame.
+        # Make sure this  function does not return any None objects, because these will cause problems later
+        result_list = [
+            x
+            for x in result_list
+            if (type(x) == LineString or type(x) == MultiLineString)
+        ]
 
-        Args:
-            gpd (gpd.GeoDataFrame): Input GeoDataFrame.
+        return result_list
 
-        Returns:
-            gpd.GeoDataFrame: GeoDataFrame with exploded and deduplicated geometries.
+    def cut_gdf(self):
         """
-        gpd = gpd.explode()
-        gpd = gpd[
-            gpd.index.isin(
-                gpd.geometry.apply(lambda geom: geom.wkb).drop_duplicates().index
-            )
-        ]
-        return gpd
+        Cuts every linestring or multilinestring feature in a gdf to equal length segments. Assumes only linestrings for now.
+
+            *gdf* (GeoDataFrame) : GeoDataFrame to split
+            *length* (units of the projection) : Typically in degrees, 0.001 degrees ~ 111 m in Europe
+        """
+        gdf = self.edges_input.copy()
+        columns = gdf.columns
+
+        data = {"splt_id": []}
+
+        for column in columns:
+            data[column] = []
+
+        count = 0
+        for _, row in gdf.iterrows():
+            geom = row["geometry"]
+            assert type(geom) == LineString or type(geom) == MultiLineString
+            linestrings = self.split_linestring(geom, self.segmentation_length)
+
+            for _, linestring in enumerate(linestrings):
+                for key, value in row.items():
+                    if key == "geometry":
+                        data[key].append(linestring)
+                    else:
+                        data[key].append(value)
+                data["splt_id"].append(count)
+                count += 1
+        self.edges_segmented = gpd.GeoDataFrame(data)
```

### Comparing `ra2ce-0.8.1/ra2ce/network/networks.py` & `ra2ce-0.9.0/ra2ce/network/networks.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,20 +15,24 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+import copy
 import logging
+import warnings
 from pathlib import Path
 
+import geopandas as gpd
 import networkx as nx
+import osmnx
+import pandas as pd
 import pyproj
-from geopandas import GeoDataFrame
 
 from ra2ce.network import networks_utils as nut
 from ra2ce.network.exporters.network_exporter_factory import NetworkExporterFactory
 from ra2ce.network.graph_files.graph_files_collection import GraphFilesCollection
 from ra2ce.network.network_config_data.network_config_data import NetworkConfigData
 from ra2ce.network.network_wrappers.network_wrapper_factory import NetworkWrapperFactory
 
@@ -135,30 +139,87 @@
             self.origins,
         )
 
         return out_fn
 
     def _export_network_files(
         self,
-        network: nx.MultiGraph | GeoDataFrame,
+        network: nx.MultiGraph | gpd.GeoDataFrame,
         graph_type: str,
         types_to_export: list[str],
     ):
         _exporter = NetworkExporterFactory()
         _exporter.export(
             network=network,
             basename=graph_type,
             output_dir=self.output_graph_dir,
             export_types=types_to_export,
         )
         self.graph_files.set_file(_exporter.get_pickle_path())
         self.graph_files.set_graph(graph_type, network)
 
-    def _get_new_network_and_graph(self, export_types: list[str]) -> None:
-        (_base_graph, _network_gdf) = NetworkWrapperFactory(
+    def _include_attributes(self, attributes: list, graph: nx.Graph) -> nx.Graph:
+        def _add_x_y_to_nodes(graph: nx.Graph) -> nx.Graph:
+            for node, data in graph.nodes(data=True):
+                if "x" not in data or "y" not in data:
+                    # Use 'geometry' or provide default values if it's not present
+                    geometry = data.get("geometry", (0.0, 0.0))
+                    data.setdefault("x", round(geometry.x, 7))
+                    data.setdefault("y", round(geometry.y, 7))
+            return graph
+
+        # If required_attributes are provided, check if all edges already have them
+        if attributes and all(
+            all(attr in edge_data for attr in attributes)
+            for _, _, edge_data in graph.edges(data=True)
+        ):
+            # If all required attributes are present, return the original graph
+            return graph
+        graph = _add_x_y_to_nodes(graph)
+        gdf_nodes, gdf_edges = osmnx.graph_to_gdfs(graph)
+        updated_graph = copy.deepcopy(graph)
+        for attribute in attributes:
+            if attribute in gdf_edges.columns:
+                attribute_values_gdf = gdf_edges[attribute]
+                for (u, v, key), attribute_values in attribute_values_gdf.items():
+                    updated_graph[u][v][key][attribute] = attribute_values
+        return updated_graph
+
+    def _get_edges_time_hours(self, _graph: nx.MultiGraph) -> dict:
+        result = {}
+
+        for e in _graph.edges.data(keys=True):
+            if not e[-1].get("avgspeed"):
+                warnings.warn(
+                    "Some edges have missing 'avgspeed' attribute. Time values set to None.",
+                    UserWarning,
+                )
+                time_value = None
+            else:
+                time_value = (e[-1]["length"] / 1000) / e[-1]["avgspeed"]
+            result[(e[0], e[1], e[2])] = {"time": time_value}
+
+        return result
+
+    def _get_edges_time_hours_row_wise(self, _row: pd.Series) -> pd.Series | None:
+        row_avgspeed = _row.get("avgspeed", None)
+        if row_avgspeed:
+            return _row["length"] * 1e-3 / _row["avgspeed"]
+        else:
+            warnings.warn(
+                "Some edges have missing 'avgspeed' attribute. Time values set to None.",
+                UserWarning,
+            )
+            return None
+
+    def _get_new_network_and_graph(
+        self, export_types: list[str]
+    ) -> tuple[nx.classes.graph.Graph, gpd.GeoDataFrame]:
+
+        _base_graph, _network_gdf = NetworkWrapperFactory(
             self._config_data
         ).get_network()
 
         self.base_graph_crs = _network_gdf.crs
         self.base_network_crs = _network_gdf.crs
 
         # Set the road lengths to meters for both the base_graph and network_gdf
@@ -167,17 +228,27 @@
             (e[0], e[1], e[2]): {
                 "length": nut.line_length(e[-1]["geometry"], _network_gdf.crs)
             }
             for e in _base_graph.edges.data(keys=True)
         }
         nx.set_edge_attributes(_base_graph, edges_lengths_meters)
 
+        edges_time_hours = self._get_edges_time_hours(_base_graph)
+        nx.set_edge_attributes(_base_graph, edges_time_hours)
+
         _network_gdf["length"] = _network_gdf["geometry"].apply(
             lambda x: nut.line_length(x, _network_gdf.crs)
         )
+        _network_gdf["time"] = _network_gdf.apply(
+            self._get_edges_time_hours_row_wise, axis=1
+        )
+
+        _base_graph = self._include_attributes(
+            attributes=["avgspeed", "bridge", "tunnel"], graph=_base_graph
+        )
 
         # Save the graph and geodataframe
         self._export_network_files(_base_graph, "base_graph", export_types)
         self._export_network_files(_network_gdf, "base_network", export_types)
 
     def _get_stored_network_and_graph(self) -> None:
         base_graph_filepath = self.graph_files.base_graph.file
@@ -186,15 +257,15 @@
         logging.info(
             "Apparently, you already did create a network with ra2ce earlier. "
             + "Ra2ce will use this: {}".format(base_graph_filepath)
         )
 
         def get_graph(
             file_type: str, file_path: Path | None
-        ) -> nx.MultiGraph | GeoDataFrame:
+        ) -> nx.MultiGraph | gpd.GeoDataFrame:
             graph = self.graph_files.get_graph(file_type)
             if graph is None:
                 raise FileNotFoundError(
                     "No base {} file found at {}.".format(file_type, file_path)
                 )
             return graph
```

### Comparing `ra2ce-0.8.1/ra2ce/network/networks_utils.py` & `ra2ce-0.9.0/ra2ce/network/networks_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,28 +22,29 @@
 import itertools
 import logging
 import os
 import sys
 import warnings
 from pathlib import Path
 from statistics import mean
-from typing import Optional, Union
+from typing import Optional
 
 import geopandas as gpd
 import networkx as nx
 import numpy as np
 import pandas as pd
 import pyproj
 import rasterio
 import rtree
 from geopy import distance
-from networkx import Graph, set_edge_attributes
 from numpy.ma import MaskedArray
 from osgeo import gdal
-from osmnx import graph_to_gdfs, simplify_graph
+from osmnx import graph_to_gdfs
+from osmnx._errors import GraphSimplificationError
+from osmnx.simplification import _get_paths_to_simplify, _remove_rings, utils
 from rasterio.features import shapes
 from rasterio.mask import mask
 from shapely.geometry import LineString, MultiLineString, Point, box, shape
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 from shapely.ops import linemerge, unary_union
 from tqdm import tqdm
 
@@ -696,15 +697,14 @@
         if seg:
             segments.append(seg)
 
     segments.append(current_line)
     return segments
 
 
-
 def cut(line: BaseMultipartGeometry, distance: float) -> tuple[LineString, LineString]:
     # Cuts a line in two at a distance from its starting point
     # This is taken from shapely manual
     if (distance <= 0.0) | (distance >= line.length):
         return [None, LineString(line)]
 
     if isinstance(line, LineString):
@@ -737,20 +737,20 @@
                         LineString([(cp.x, cp.y)] + [xy[0:2] for xy in coords[i:]]),
                     ]
 
 
 def join_nodes_edges(
     gdf_nodes: gpd.GeoDataFrame, gdf_edges: gpd.GeoDataFrame, id_name: str
 ) -> gpd.GeoDataFrame:
-    """Creates tuples from the adjecent nodes and add as column in geodataframe.
+    """Creates tuples from the adjacent nodes and add as column in geodataframe.
     Args:
         gdf_nodes [geodataframe]: geodataframe of the nodes of a graph
         gdf_edges [geodataframe]: geodataframe of the edges of a graph
     Returns:
-        result [geodataframe]: geodataframe of adjecent nodes from edges
+        result [geodataframe]: geodataframe of adjacent nodes from edges
     """
     logging.info("Started joining edges and nodes...")
     # list of the edges that are not topographically correct
     incorrect_edges = []
 
     # add node attributes to edges
     gdf = gpd.sjoin(gdf_edges, gdf_nodes, how="left", op="intersects")
@@ -1039,16 +1039,16 @@
         "For further network processing, change the 'file_id' parameter in the network.ini file"
         "to '{}".format(new_id_name, id_name, new_id_name)
     )
     return gdf, new_id_name
 
 
 def graph_check_create_unique_ids(
-    graph: Graph, id_name: str, new_id_name: str = "rfid"
-) -> tuple[Graph, str]:
+    graph: nx.Graph, id_name: str, new_id_name: str = "rfid"
+) -> tuple[nx.Graph, str]:
     """
     TODO: This is not really being used. It could be removed.
     Check if the ID's are unique per edge: if not, add an own ID called 'fid'
 
     Args:
         graph (Graph): Graph to prune from repeated ids.
         id_name (str): ID to search.
@@ -1101,40 +1101,197 @@
     for nd in nodes_without_geom:
         graph.nodes[nd][geom_name] = Point(graph.nodes[nd]["x"], graph.nodes[nd]["y"])
 
     edges_without_geom = [
         e for e in graph.edges.data(keys=True, data=True) if geom_name not in e[-1]
     ]
     for ed in edges_without_geom:
-        if graph.nodes[ed[0]].get(geom_name, None) and graph.nodes[ed[1]].get(geom_name, None):
+        if graph.nodes[ed[0]].get(geom_name, None) and graph.nodes[ed[1]].get(
+            geom_name, None
+        ):
             graph[ed[0]][ed[1]][ed[2]][geom_name] = LineString(
                 [graph.nodes[ed[0]][geom_name], graph.nodes[ed[1]][geom_name]]
             )
     return graph
 
 
 def simplify_graph_count(complex_graph: nx.Graph) -> nx.Graph:
+    """
+    _summary_
+
+    Args:
+        complex_graph (nx.Graph): _description_
+
+    Returns:
+        nx.Graph: _description_
+    """
     # Simplify the graph topology and log the change in nr of nodes and edges.
     old_len_nodes = complex_graph.number_of_nodes()
     old_len_edges = complex_graph.number_of_edges()
 
-    simple_graph = simplify_graph(complex_graph)
+    simple_graph = simplify_graph(
+        graph=complex_graph, strict=True, remove_rings=True, track_merged=False
+    )
 
     new_len_nodes = simple_graph.number_of_nodes()
     new_len_edges = simple_graph.number_of_edges()
 
     logging.info(
         "Graph simplified from {:,} to {:,} nodes and {:,} to {:,} edges.".format(
             old_len_nodes, new_len_nodes, old_len_edges, new_len_edges
         )
     )
 
     return simple_graph
 
 
+def simplify_graph(
+    graph: nx.Graph, strict: bool, remove_rings: bool, track_merged: bool
+):
+    """
+    This is an OSMNX function with the same name, modified to check if geometry attribute exists in the nodes of each
+    path to simplify.
+
+    !IMPORTANT! This whole method makes us bound to `OSMNX==1.7.1`.
+
+    Check the official OSMNX documentation for more details.
+
+    Args:
+        graph (networkx.MultiDiGraph): input graph
+        strict (bool): if False, allow nodes to be end points even if they fail all other
+            rules but have incident edges with different OSM IDs. Lets you keep
+            nodes at elbow two-way intersections, but sometimes individual blocks
+            have multiple OSM IDs within them too.
+        remove_rings(bool): if True, remove isolated self-contained rings that have no endpoints
+        track_merged (bool): if True, add `merged_edges` attribute on simplified edges, containing
+            a list of all the (u, v) node pairs that were merged together
+
+    Returns
+         networkx.MultiDiGraph: topologically simplified graph, with a new `geometry` attribute on
+            each simplified edge
+    """
+    if "simplified" in graph.graph and graph.graph["simplified"]:  # pragma: no cover
+        msg = "This graph has already been simplified, cannot simplify it again."
+        raise GraphSimplificationError(msg)
+
+    logging.info("Begin topologically simplifying the graph...")
+
+    # define edge segment attributes to sum upon edge simplification
+    attrs_to_sum = {"length", "travel_time"}
+
+    # make a copy to not mutate original graph object caller passed in
+    graph = graph.copy()
+    initial_node_count = len(graph)
+    initial_edge_count = len(graph.edges)
+    all_nodes_to_remove = []
+    all_edges_to_add = []
+
+    # generate each path that needs to be simplified
+    for path in _get_paths_to_simplify(graph, strict):
+        # add the interstitial edges we're removing to a list so we can retain
+        # their spatial geometry
+        merged_edges = []
+        path_attributes = {}
+        for u, v in zip(path[:-1], path[1:]):
+            if track_merged:
+                # keep track of the edges that were merged
+                merged_edges.append((u, v))
+
+            # there should rarely be multiple edges between interstitial nodes
+            # usually happens if OSM has duplicate ways digitized for just one
+            # street... we will keep only one of the edges (see below)
+            edge_count = graph.number_of_edges(u, v)
+            if edge_count != 1:
+                utils.log(
+                    f"Found {edge_count} edges between {u} and {v} when simplifying"
+                )
+
+            # get edge between these nodes: if multiple edges exist between
+            # them (see above), we retain only one in the simplified graph
+            # We can't assume that there exists an edge from u to v
+            # with key=0, so we get a list of all edges from u to v
+            # and just take the first one.
+            edge_data = list(graph.get_edge_data(u, v).values())[0]
+            for attr in edge_data:
+                if attr in path_attributes:
+                    # if this key already exists in the dict, append it to the
+                    # value list
+                    path_attributes[attr].append(edge_data[attr])
+                else:
+                    # if this key doesn't already exist, set the value to a list
+                    # containing the one value
+                    path_attributes[attr] = [edge_data[attr]]
+
+        # consolidate the path's edge segments' attribute values
+        for attr in path_attributes:
+            if attr in attrs_to_sum:
+                # if this attribute must be summed, sum it now
+                path_attributes[attr] = sum(path_attributes[attr])
+            elif attr != "geometry" and len(set(path_attributes[attr])) == 1:
+                # if there's only 1 unique value in this attribute list,
+                # consolidate it to the single value (the zero-th):
+                path_attributes[attr] = path_attributes[attr][0]
+            elif attr != "geometry":
+                # otherwise, if there are multiple values, keep one of each
+                path_attributes[attr] = list(set(path_attributes[attr]))
+
+        # construct the new consolidated edge's geometry for this path
+        if all("geometry" in graph.nodes[node] for node in path):
+            # Check if all nodes in the path have "geometry" attribute
+            # Use existing geometries to create LineString
+            path_attributes["geometry"] = LineString(
+                [graph.nodes[node]["geometry"] for node in path]
+            )
+        elif all(
+            "x" in graph.nodes[node] and "y" in graph.nodes[node] for node in path
+        ):
+            # Create LineString using x and y coordinates
+            path_attributes["geometry"] = LineString(
+                [
+                    Point((graph.nodes[node]["x"], graph.nodes[node]["y"]))
+                    for node in path
+                ]
+            )
+        else:
+            raise ValueError(
+                "All nodes in the path must have 'geometry' or 'x' and 'y' attributes."
+            )
+
+        if track_merged:
+            # add the merged edges as a new attribute of the simplified edge
+            path_attributes["merged_edges"] = merged_edges
+
+        # add the nodes and edge to their lists for processing at the end
+        all_nodes_to_remove.extend(path[1:-1])
+        all_edges_to_add.append(
+            {"origin": path[0], "destination": path[-1], "attr_dict": path_attributes}
+        )
+
+    # for each edge to add in the list we assembled, create a new edge between
+    # the origin and destination
+    for edge in all_edges_to_add:
+        graph.add_edge(edge["origin"], edge["destination"], **edge["attr_dict"])
+
+    # finally remove all the interstitial nodes between the new edges
+    graph.remove_nodes_from(set(all_nodes_to_remove))
+
+    if remove_rings:
+        graph = _remove_rings(graph)
+
+    # mark the graph as having been simplified
+    graph.graph["simplified"] = True
+
+    msg = (
+        f"Simplified graph: {initial_node_count:,} to {len(graph):,} nodes, "
+        f"{initial_edge_count:,} to {len(graph.edges):,} edges"
+    )
+    logging.info(msg)
+    return graph
+
+
 def graph_from_gdf(
     gdf: gpd.GeoDataFrame, gdf_nodes, name: str = "network", node_id: str = "ID"
 ) -> nx.MultiGraph:
     # create a Graph object
     _created_graph = nx.MultiGraph(crs=gdf.crs)
 
     # create nodes on the Graph
@@ -1187,15 +1344,17 @@
         edges = graph_to_gdfs(graph_to_convert, nodes=save_nodes, edges=save_edges)
     elif save_nodes and not save_edges:
         nodes = graph_to_gdfs(graph_to_convert, nodes=save_nodes, edges=save_edges)
 
     return edges, nodes
 
 
-def graph_to_gpkg(origin_graph: nx.classes.graph.Graph, edge_gpkg: str, node_gpkg: str) -> None:
+def graph_to_gpkg(
+    origin_graph: nx.classes.graph.Graph, edge_gpkg: str, node_gpkg: str
+) -> None:
     """Takes in a networkx graph object and outputs shapefiles at the paths indicated by edge_gpkg and node_gpkg
 
     Arguments:
         origin_graph [nx.classes.graph.Graph]: networkx graph object to be converted
         edge_gpkg [str]: output path including extension for edges geopackage
         node_gpkg [str]: output path including extension for nodes geopackage
 
@@ -1220,17 +1379,17 @@
         nodes.crs = edges.crs
 
     logging.info("Saving nodes as shapefile: {}".format(node_gpkg))
     logging.info("Saving edges as shapefile: {}".format(edge_gpkg))
 
     # The encoding utf-8 might result in an empty shapefile if the wrong encoding is used.
     for entity in [nodes, edges]:
-        if 'osmid' in entity:
+        if "osmid" in entity:
             # Otherwise it gives this error: cannot insert osmid, already exist
-            entity['osmid_original'] = entity.pop('osmid')
+            entity["osmid_original"] = entity.pop("osmid")
     for _path in [node_gpkg, edge_gpkg]:
         if _path.exists():
             _path.unlink()
     nodes.to_file(node_gpkg, driver="GPKG", encoding="utf-8")
     edges.to_file(edge_gpkg, driver="GPKG", encoding="utf-8")
 
 
@@ -1566,15 +1725,15 @@
                 "Could not find the simple ID belonging to complex ID {}; value set to None. Full error: {}".format(
                     key, e
                 )
             )
             simple_ids_per_complex_id[key] = None
 
     # Now the format of simple_ids_per_complex_id is: {(u,v,k) : 'rfid}
-    set_edge_attributes(complex_graph, simple_ids_per_complex_id, new_id)
+    nx.set_edge_attributes(complex_graph, simple_ids_per_complex_id, new_id)
 
     return complex_graph
 
 
 def calc_avg_speed(graph, road_type_col_name, save_csv=False, save_path=None):
     """Calculates the average speed from OSM roads, per road type
```

### Comparing `ra2ce-0.8.1/ra2ce/network/origins_destinations.py` & `ra2ce-0.9.0/ra2ce/network/origins_destinations.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import logging
 import os
+from collections import defaultdict
 from pathlib import Path
 from typing import Optional, Union
 
 import geopandas as gpd
 import networkx
 import networkx as nx
 import numpy as np
@@ -136,15 +137,21 @@
 
     return od
 
 
 def closest_node(node: np.ndarray, nodes: np.ndarray) -> np.ndarray:
     deltas = nodes - node
     dist_2 = np.einsum("ij,ij->i", deltas, deltas)
-    return nodes[np.argmin(dist_2)]
+    # Find indices of all minimum distances
+    min_dist_indices = np.where(dist_2 == dist_2.min())[0]
+
+    # CROSSCADE: The previous return value `nodes[np.argmin(dist_2)]`
+    # returned a np.ndarray of 1 dimension (`[result]`), whilst the new value
+    # will return a 2 dimensional np.ndarray ( `[[result]]`)
+    return np.round(nodes[min_dist_indices], decimals=7)[0]
 
 
 def get_od(o_id: str, d_id: str) -> str:
     """
     Gets a valid origin id node from the given pair.
 
     Args:
@@ -163,15 +170,16 @@
         return d_id
     return np.nan
 
 
 def add_data_to_existing_node(graph, node, match_name):
     if "od_id" in graph.nodes[node]:
         # the node already has a origin/destination attribute
-        graph.nodes[node]["od_id"] = graph.nodes[node]["od_id"] + "," + match_name
+        if match_name not in set(graph.nodes[node]["od_id"].split(",")):
+            graph.nodes[node]["od_id"] = graph.nodes[node]["od_id"] + "," + match_name
     else:
         graph.nodes[node]["od_id"] = match_name
     return graph
 
 
 def update_edges_with_new_node(
     graph: networkx.MultiGraph,
@@ -195,15 +203,21 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_b != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_b, graph_crs), geometry=line_b)
+        edge_data.update(
+            length=line_length(line_b, graph_crs),
+            geometry=line_b,
+            node_A=node_a,
+            node_B=new_node_id,
+            edge_fid=f"{node_a}_{new_node_id}",
+        )
         graph.add_edge(node_a, new_node_id, k_new, **edge_data)
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_a, new_node_id, k_new) for p in set(list(line_b.coords[1:-1]))}
         )
 
@@ -215,16 +229,24 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_b != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_b, graph_crs), geometry=line_b)
-        graph.add_edge(node_b, new_node_id, k_new, **edge_data)
+        edge_data.update(
+            length=line_length(line_b, graph_crs),
+            geometry=line_b,
+            node_A=new_node_id,
+            node_B=node_b,
+            edge_fid=f"{new_node_id}_{node_b}",
+        )
+        graph.add_edge(
+            new_node_id, node_b, k_new, **edge_data
+        )  # changed the u, v order
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_b, new_node_id, k_new) for p in set(list(line_b.coords[1:-1]))}
         )
 
         cnt += 1
@@ -235,15 +257,21 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_b != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_b, graph_crs), geometry=line_b)
+        edge_data.update(
+            length=line_length(line_b, graph_crs),
+            geometry=line_b,
+            node_A=node_a,
+            node_B=new_node_id,
+            edge_fid=f"{node_b}_{new_node_id}",
+        )
         graph.add_edge(node_a, new_node_id, k_new, **edge_data)
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_a, new_node_id, k_new) for p in set(list(line_b.coords[1:-1]))}
         )
 
@@ -255,16 +283,24 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_b != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_b, graph_crs), geometry=line_b)
-        graph.add_edge(node_b, new_node_id, k_new, **edge_data)
+        edge_data.update(
+            length=line_length(line_b, graph_crs),
+            geometry=line_b,
+            node_A=new_node_id,
+            node_B=node_b,
+            edge_fid=f"{new_node_id}_{node_b}",
+        )
+        graph.add_edge(
+            new_node_id, node_b, k_new, **edge_data
+        )  # changed the u, v order
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_b, new_node_id, k_new) for p in set(list(line_b.coords[1:-1]))}
         )
 
         cnt += 1
@@ -275,16 +311,24 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_a != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_a, graph_crs), geometry=line_a)
-        graph.add_edge(node_b, new_node_id, k_new, **edge_data)
+        edge_data.update(
+            length=line_length(line_a, graph_crs),
+            geometry=line_a,
+            node_A=new_node_id,
+            node_B=node_b,
+            edge_fid=f"{new_node_id}_{node_b}",
+        )
+        graph.add_edge(
+            new_node_id, node_b, k_new, **edge_data
+        )  # changed the u, v order
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_b, new_node_id, k_new) for p in set(list(line_a.coords[1:-1]))}
         )
 
         cnt += 1
@@ -295,15 +339,21 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_a != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_a, graph_crs), geometry=line_a)
+        edge_data.update(
+            length=line_length(line_a, graph_crs),
+            geometry=line_a,
+            node_A=node_a,
+            node_B=new_node_id,
+            edge_fid=f"{node_a}_{new_node_id}",
+        )
         graph.add_edge(node_a, new_node_id, k_new, **edge_data)
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_a, new_node_id, k_new) for p in set(list(line_a.coords[1:-1]))}
         )
 
@@ -315,16 +365,24 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_a != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_a, graph_crs), geometry=line_a)
-        graph.add_edge(node_b, new_node_id, k_new, **edge_data)
+        edge_data.update(
+            length=line_length(line_a, graph_crs),
+            geometry=line_a,
+            node_A=new_node_id,
+            node_B=node_b,
+            edge_fid=f"{new_node_id}_{node_b}",
+        )
+        graph.add_edge(
+            new_node_id, node_b, k_new, **edge_data
+        )  # changed the u, v order
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_b, new_node_id, k_new) for p in set(list(line_a.coords[1:-1]))}
         )
 
         cnt += 1
@@ -335,15 +393,21 @@
         if node_a == node_b and graph.has_edge(*(node_a, new_node_id, 0)):
             if line_a != graph.edges[(node_a, new_node_id, 0)]["geometry"]:
                 k_new = 1
             else:
                 k_new = 0
         else:
             k_new = 0
-        edge_data.update(length=line_length(line_a, graph_crs), geometry=line_a)
+        edge_data.update(
+            length=line_length(line_a, graph_crs),
+            geometry=line_a,
+            node_A=node_a,
+            node_B=new_node_id,
+            edge_fid=f"{node_a}_{new_node_id}",
+        )
         graph.add_edge(node_a, new_node_id, k_new, **edge_data)
 
         # Update the inverse vertices dict
         inverse_vertices_dict.update(
             {p: (node_a, new_node_id, k_new) for p in set(list(line_a.coords[1:-1]))}
         )
 
@@ -352,16 +416,17 @@
     try:
         assert cnt == 2
     except AssertionError:
         logging.warning(
             "No combination of nodes/road segments found for the OD assignment."
         )
 
-    # remove the edge that is split in two from the graph
-    graph.remove_edge(node_a, node_b, k)
+    if graph.has_edge(node_a, node_b, k):
+        # remove the edge that is split in two from the graph
+        graph.remove_edge(node_a, node_b, k)
 
     return graph, inverse_vertices_dict
 
 
 def add_od_nodes(
     od: gpd.GeoDataFrame,
     graph: Union[nx.classes.Graph, nx.classes.MultiGraph],
@@ -388,31 +453,33 @@
                         [closest_v_data["x"], closest_v_data["y"]],
                     ]
                 ),
             )
             closest_node_on_extremities_id = get_node_id_from_position(
                 graph, *closest_node_on_extremities
             )
-            inverse_nodes_dict[(closest_node_on_road[0], closest_node_on_road[1])] = (
-                closest_node_on_extremities_id
-            )
+            inverse_nodes_dict[
+                (closest_node_on_road[0], closest_node_on_road[1])
+            ] = closest_node_on_extremities_id
 
         return inverse_nodes_dict
 
     def get_node_id_from_position(
         g: Union[nx.classes.Graph], x: float, y: float
     ) -> Union[float, None]:
         nodes = [
             (node, data)
             for node, data in g.nodes(data=True)
-            if data.get("x") == x and data.get("y") == y
+            if "geometry" in data
+            and round(data["geometry"].x, 7) == round(x, 7)
+            and round(data["geometry"].y, 7) == round(y, 7)
         ]
         return nodes[0][0] if nodes else None
 
-    """Gets from each origin and destination the closest vertice on the graph edge.
+    """Gets from each origin and destination the closest vertex on the graph edge.
     Args:
         od [Geodataframe]: The GeoDataFrame with the origins and destinations
         graph [networkX graph]: networkX graph
         crs [string or pyproj crs]:
     Returns:
         od [Geodataframe]: The GeoDataFrame with the locations of the origins and destinations on the road vertices
         graph [networkX graph]: The networkX graph updated with origins and destinations
```

### Comparing `ra2ce-0.8.1/ra2ce/ra2ce_logging.py` & `ra2ce-0.9.0/ra2ce/ra2ce_logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,46 +15,81 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+from __future__ import annotations
 
 import logging
 from pathlib import Path
 from typing import Optional
 
 
 class Ra2ceLogger:
-    log_file: Optional[Path] = None
+    """
+    Class to handle the logging configuration for the RA2CE application.
+    """
 
-    def __init__(self, logging_dir: Path, logger_name: str) -> None:
-        if not logging_dir.is_dir():
-            logging_dir.mkdir(parents=True)
-        self.log_file = logging_dir.joinpath(f"{logger_name}.log")
-        if not self.log_file.is_file():
-            self.log_file.touch()
+    log_file: Optional[Path] = None
+    _file_handler: Optional[logging.FileHandler] = None
 
+    def __init__(self, log_file: Optional[Path], logger_name: str) -> None:
+        self.log_file = log_file
         self._set_file_handler()
         self._set_console_handler()
         self._set_formatter()
         logging.info(f"{logger_name} logger initialized.")
 
+    @classmethod
+    def initialize_file_logger(cls, logging_dir: Path, logger_name: str) -> Ra2ceLogger:
+        """
+        Initializes a logger that writes to a file and to console.
+
+        Args:
+            logging_dir (Path): Path to the logging directory
+            logger_name (str): Name of the logger
+
+        Returns:
+            Ra2ceLogger: The logger object
+        """
+        if not logging_dir.is_dir():
+            logging_dir.mkdir(parents=True)
+        _log_file = logging_dir.joinpath(f"{logger_name}.log")
+        if not _log_file.is_file():
+            _log_file.touch()
+        return cls(_log_file, logger_name)
+
+    @classmethod
+    def initialize_console_logger(cls, logger_name: str) -> Ra2ceLogger:
+        """
+        Initializes a logger that writes to console only.
+
+        Args:
+            logger_name (str): Name of the logger
+
+        Returns:
+            Ra2ceLogger: The logger object
+        """
+        return cls(None, logger_name)
+
     def _get_logger(self) -> logging.Logger:
         """
         Gets the ra2ce logger which by default is the root logging.Logger.
 
         Returns:
             logging.Logger: Logger instance.
         """
         return logging.getLogger("")
 
     def _set_file_handler(self) -> None:
         # Create a root logger and set the minimum logging level.
+        if not self.log_file:
+            return
         self._get_logger().setLevel(logging.INFO)
         self._file_handler = logging.FileHandler(filename=self.log_file, mode="a")
         self._file_handler.setLevel(logging.INFO)
         self._get_logger().addHandler(self._file_handler)
 
     def _set_console_handler(self) -> None:
         # Create a console handler and set the required logging level.
@@ -64,9 +99,10 @@
 
     def _set_formatter(self) -> None:
         # Create a formatter and add to the file and console handlers.
         _formatter = logging.Formatter(
             fmt="%(asctime)s - [%(filename)s:%(lineno)d] - %(name)s - %(levelname)s - %(message)s",
             datefmt="%Y-%m-%d %I:%M:%S %p",
         )
-        self._file_handler.setFormatter(_formatter)
+        if self.log_file:
+            self._file_handler.setFormatter(_formatter)
         self._console_handler.setFormatter(_formatter)
```

### Comparing `ra2ce-0.8.1/ra2ce/runners/analysis_runner_protocol.py` & `ra2ce-0.9.0/ra2ce/runners/analysis_runner_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from typing import Protocol, runtime_checkable
 
-from ra2ce.analysis.analysis_config_wrapper import (
-    AnalysisConfigWrapper,
-)
+from ra2ce.analysis.analysis_config_wrapper import AnalysisConfigWrapper
 from ra2ce.analysis.analysis_result_wrapper import AnalysisResultWrapper
 from ra2ce.configuration.config_wrapper import ConfigWrapper
 
 
 @runtime_checkable
 class AnalysisRunner(Protocol):
     @staticmethod
```

### Comparing `ra2ce-0.8.1/ra2ce/runners/direct_analysis_runner.py` & `ra2ce-0.9.0/ra2ce/runners/direct_analysis_runner.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 
 import logging
 import time
 
 from ra2ce.analysis.analysis_collection import AnalysisCollection
 from ra2ce.analysis.analysis_config_wrapper import AnalysisConfigWrapper
 from ra2ce.analysis.analysis_result_wrapper import AnalysisResultWrapper
-from ra2ce.configuration.config_wrapper import ConfigWrapper
 from ra2ce.analysis.analysis_result_wrapper_exporter import (
     AnalysisResultWrapperExporter,
 )
+from ra2ce.configuration.config_wrapper import ConfigWrapper
 from ra2ce.runners.analysis_runner_protocol import AnalysisRunner
 
 
 class DirectAnalysisRunner(AnalysisRunner):
     def __str__(self) -> str:
         return "Direct Analysis Runner"
```

### Comparing `ra2ce-0.8.1/ra2ce/runners/indirect_analysis_runner.py` & `ra2ce-0.9.0/ra2ce/runners/indirect_analysis_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,20 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import logging
 import time
 
 from ra2ce.analysis.analysis_collection import AnalysisCollection
-from ra2ce.analysis.analysis_config_wrapper import (
-    AnalysisConfigWrapper,
-)
+from ra2ce.analysis.analysis_config_wrapper import AnalysisConfigWrapper
 from ra2ce.analysis.analysis_result_wrapper import AnalysisResultWrapper
-from ra2ce.configuration.config_wrapper import ConfigWrapper
 from ra2ce.analysis.analysis_result_wrapper_exporter import (
     AnalysisResultWrapperExporter,
 )
+from ra2ce.configuration.config_wrapper import ConfigWrapper
 from ra2ce.runners.analysis_runner_protocol import AnalysisRunner
 
 
 class IndirectAnalysisRunner(AnalysisRunner):
     def __str__(self) -> str:
         return "Indirect Analysis Runner"
```

### Comparing `ra2ce-0.8.1/ra2ce/runners/README.md` & `ra2ce-0.9.0/ra2ce/runners/README.md`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/README.md` & `ra2ce-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ra2ce-0.8.1/PKG-INFO` & `ra2ce-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra2ce
-Version: 0.8.1
+Version: 0.9.0
 Summary: Risk Assessment and Adaptation for Critical infrastructurE (RA2CE).
 Home-page: https://github.com/Deltares/ra2ce
 License: GPL-3.0-or-later
 Author: Margreet van Marle
 Author-email: Margreet.vanMarle@deltares.nl
 Maintainer: Carles Salvador Soriano Perez
 Maintainer-email: carles.sorianoperez@deltares.nl
```

