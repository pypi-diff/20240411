# Comparing `tmp/one_interfaces-6.7.0.tar.gz` & `tmp/one_interfaces-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\one_interfaces-6.7.0.tar", last modified: Wed Apr  3 13:42:35 2024, max compression
+gzip compressed data, was "dist\one_interfaces-6.8.0.tar", last modified: Thu Apr 11 15:54:23 2024, max compression
```

## Comparing `one_interfaces-6.7.0.tar` & `one_interfaces-6.8.0.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:42:35.730317 one_interfaces-6.7.0/
--rw-rw-rw-   0        0        0      580 2022-07-05 14:29:22.000000 one_interfaces-6.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0       62 2022-07-05 14:29:22.000000 one_interfaces-6.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1217 2024-04-03 13:42:35.730317 one_interfaces-6.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      394 2022-11-11 17:33:49.000000 one_interfaces-6.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 13:42:35.716018 one_interfaces-6.7.0/one_interfaces/
--rw-rw-rw-   0        0        0       23 2024-04-02 22:03:12.000000 one_interfaces-6.7.0/one_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/account_status_pb2.py
--rw-rw-rw-   0        0        0     2440 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/activity_pb2.py
--rw-rw-rw-   0        0        0     1899 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/activity_type_pb2.py
--rw-rw-rw-   0        0        0     2231 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/address_pb2.py
--rw-rw-rw-   0        0        0     1681 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/agency_pb2.py
--rw-rw-rw-   0        0        0     1874 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_pb2.py
--rw-rw-rw-   0        0        0     2811 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_result_pb2.py
--rw-rw-rw-   0        0        0     1769 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_results_import_profile_pb2.py
--rw-rw-rw-   0        0        0     1758 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_results_import_telemetry_pb2.py
--rw-rw-rw-   0        0        0     1223 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/apierror_pb2.py
--rw-rw-rw-   0        0        0     1393 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/apiresponse_pb2.py
--rw-rw-rw-   0        0        0     1941 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/auditevent_pb2.py
--rw-rw-rw-   0        0        0     1474 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cell_monitor_backup_pb2.py
--rw-rw-rw-   0        0        0     1519 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cell_pb2.py
--rw-rw-rw-   0        0        0     1541 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/celldata_binding_pb2.py
--rw-rw-rw-   0        0        0     1988 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/celldata_pb2.py
--rw-rw-rw-   0        0        0     1534 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cells_pb2.py
--rw-rw-rw-   0        0        0     1871 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cellvalue_backup_pb2.py
--rw-rw-rw-   0        0        0     4778 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/client_pb2.py
--rw-rw-rw-   0        0        0     2054 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/coagmeasurement_pb2.py
--rw-rw-rw-   0        0        0     2429 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/column_pb2.py
--rw-rw-rw-   0        0        0     2097 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/computation_binding_pb2.py
--rw-rw-rw-   0        0        0     2564 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/computation_pb2.py
--rw-rw-rw-   0        0        0     1893 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/computation_variable_binding_pb2.py
--rw-rw-rw-   0        0        0     2027 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/configuration_note_pb2.py
--rw-rw-rw-   0        0        0     2970 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/configuration_pb2.py
--rw-rw-rw-   0        0        0     1499 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/configuration_tag_pb2.py
--rw-rw-rw-   0        0        0    13410 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/content_pb2.py
--rw-rw-rw-   0        0        0     1951 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/csv_configuration_file_pb2.py
--rw-rw-rw-   0        0        0     1743 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/data_source_binding_pb2.py
--rw-rw-rw-   0        0        0     2052 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/data_source_configuration_pb2.py
--rw-rw-rw-   0        0        0     1536 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py
--rw-rw-rw-   0        0        0     2041 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py
--rw-rw-rw-   0        0        0     1523 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py
--rw-rw-rw-   0        0        0     3269 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_pb2.py
--rw-rw-rw-   0        0        0     2247 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_pb2.py
--rw-rw-rw-   0        0        0     3800 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py
--rw-rw-rw-   0        0        0     2063 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_type_pb2.py
--rw-rw-rw-   0        0        0     2020 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_user_right_pb2.py
--rw-rw-rw-   0        0        0     1342 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/display_options_pb2.py
--rw-rw-rw-   0        0        0     1820 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_source_definition_pb2.py
--rw-rw-rw-   0        0        0     1669 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_definition_pb2.py
--rw-rw-rw-   0        0        0     1376 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_field_pb2.py
--rw-rw-rw-   0        0        0     1605 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py
--rw-rw-rw-   0        0        0     1508 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_pb2.py
--rw-rw-rw-   0        0        0     2309 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_dataset_definition_pb2.py
--rw-rw-rw-   0        0        0     1303 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_aggregate_pb2.py
--rw-rw-rw-   0        0        0     1408 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_auditevent_pb2.py
--rw-rw-rw-   0        0        0     1385 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_azure_notification_hubtype_pb2.py
--rw-rw-rw-   0        0        0     1642 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_cell_range_action_pb2.py
--rw-rw-rw-   0        0        0     1730 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_datasource_pb2.py
--rw-rw-rw-   0        0        0     1392 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_day_pb2.py
--rw-rw-rw-   0        0        0     1515 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py
--rw-rw-rw-   0        0        0     1381 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_digital_twin_restriction_pb2.py
--rw-rw-rw-   0        0        0     1422 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_digital_twin_user_right_pb2.py
--rw-rw-rw-   0        0        0     1339 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_domain_source_pb2.py
--rw-rw-rw-   0        0        0     1373 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_entity_pb2.py
--rw-rw-rw-   0        0        0     1433 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_identity_provider_pb2.py
--rw-rw-rw-   0        0        0     1552 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_import_status_pb2.py
--rw-rw-rw-   0        0        0     1416 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_limit_operation_pb2.py
--rw-rw-rw-   0        0        0     1394 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_limit_pb2.py
--rw-rw-rw-   0        0        0     1545 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_month_pb2.py
--rw-rw-rw-   0        0        0     1606 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_category_pb2.py
--rw-rw-rw-   0        0        0     1557 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_delivery_method_pb2.py
--rw-rw-rw-   0        0        0     1427 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_message_type_pb2.py
--rw-rw-rw-   0        0        0     1346 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_platform_pb2.py
--rw-rw-rw-   0        0        0     1452 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_one_log_level_pb2.py
--rw-rw-rw-   0        0        0     1374 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_output_placement_pb2.py
--rw-rw-rw-   0        0        0     1269 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_rendering_engine_pb2.py
--rw-rw-rw-   0        0        0     1681 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py
--rw-rw-rw-   0        0        0     1663 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_pb2.py
--rw-rw-rw-   0        0        0     3080 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_sampling_statistic_pb2.py
--rw-rw-rw-   0        0        0     1483 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_time_context_pb2.py
--rw-rw-rw-   0        0        0     1388 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_time_unit_pb2.py
--rw-rw-rw-   0        0        0    27482 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_timezone_pb2.py
--rw-rw-rw-   0        0        0     1415 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_valid_value_restriction_pb2.py
--rw-rw-rw-   0        0        0     1376 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_variable_type_pb2.py
--rw-rw-rw-   0        0        0     2357 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_wims_week_definition_pb2.py
--rw-rw-rw-   0        0        0     1341 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_worksheet_pb2.py
--rw-rw-rw-   0        0        0     1768 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/execution_details_pb2.py
--rw-rw-rw-   0        0        0     2010 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/execution_parameter_pb2.py
--rw-rw-rw-   0        0        0     1211 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/expression_line_pb2.py
--rw-rw-rw-   0        0        0     2205 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/feature_pb2.py
--rw-rw-rw-   0        0        0     1589 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/feature_state_type_pb2.py
--rw-rw-rw-   0        0        0     1793 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/file_configuration_pb2.py
--rw-rw-rw-   0        0        0     1563 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/gauge_data_point_pb2.py
--rw-rw-rw-   0        0        0     1560 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/gis_pb2.py
--rw-rw-rw-   0        0        0     1231 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/historian_binding_pb2.py
--rw-rw-rw-   0        0        0     1981 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/historian_data_pb2.py
--rw-rw-rw-   0        0        0     1536 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/i18nkey_text_reference_pb2.py
--rw-rw-rw-   0        0        0     1855 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/ingest_client_pb2.py
--rw-rw-rw-   0        0        0     1698 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/jsonTicksDateTime_pb2.py
--rw-rw-rw-   0        0        0     1325 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/key_value_pb2.py
--rw-rw-rw-   0        0        0     1668 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/limit_configuration_pb2.py
--rw-rw-rw-   0        0        0     2385 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/limit_pb2.py
--rw-rw-rw-   0        0        0     1948 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/measurement_pb2.py
--rw-rw-rw-   0        0        0     1768 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/model_execution_pb2.py
--rw-rw-rw-   0        0        0     1424 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/model_location_pb2.py
--rw-rw-rw-   0        0        0     2391 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/model_template_pb2.py
--rw-rw-rw-   0        0        0     1233 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/multi_point2d_pb2.py
--rw-rw-rw-   0        0        0     1233 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/multi_point3d_pb2.py
--rw-rw-rw-   0        0        0     1472 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/note_pb2.py
--rw-rw-rw-   0        0        0     1695 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_broadcast_pb2.py
--rw-rw-rw-   0        0        0     1448 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_contact_pb2.py
--rw-rw-rw-   0        0        0     1859 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_device_pb2.py
--rw-rw-rw-   0        0        0     2430 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_direct_preference_pb2.py
--rw-rw-rw-   0        0        0     2254 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_event_pb2.py
--rw-rw-rw-   0        0        0     2267 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_in_app_notification_message_pb2.py
--rw-rw-rw-   0        0        0     1743 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_preference_pb2.py
--rw-rw-rw-   0        0        0     2174 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_template_pb2.py
--rw-rw-rw-   0        0        0     2201 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_topic_pb2.py
--rw-rw-rw-   0        0        0     1828 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/notification_topic_variable_pb2.py
--rw-rw-rw-   0        0        0     2450 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/notification_user_preference_pb2.py
--rw-rw-rw-   0        0        0     2455 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/operation_export_pb2.py
--rw-rw-rw-   0        0        0     2111 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/outputcell_backup_pb2.py
--rw-rw-rw-   0        0        0     1552 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/pagination_pb2.py
--rw-rw-rw-   0        0        0     2177 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_agency_code_pb2.py
--rw-rw-rw-   0        0        0     1674 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_agency_code_type_pb2.py
--rw-rw-rw-   0        0        0     1819 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_definition_pb2.py
--rw-rw-rw-   0        0        0     2356 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_pb2.py
--rw-rw-rw-   0        0        0     2569 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/plant_status_pb2.py
--rw-rw-rw-   0        0        0     1158 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/point2d_pb2.py
--rw-rw-rw-   0        0        0     1186 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/point3d_pb2.py
--rw-rw-rw-   0        0        0     1637 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/post_filtering_column_definition_pb2.py
--rw-rw-rw-   0        0        0     1878 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/post_filtering_pb2.py
--rw-rw-rw-   0        0        0     1585 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/privileges_pb2.py
--rw-rw-rw-   0        0        0     2503 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/product_offering_pb2.py
--rw-rw-rw-   0        0        0     2064 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/quantity_type_pb2.py
--rw-rw-rw-   0        0        0     1448 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/record_auditinfo_pb2.py
--rw-rw-rw-   0        0        0     2076 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_definition_json_v2_pb2.py
--rw-rw-rw-   0        0        0     2780 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/report_definition_pb2.py
--rw-rw-rw-   0        0        0     2178 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_definition_runs_pb2.py
--rw-rw-rw-   0        0        0     1842 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_definition_tags_pb2.py
--rw-rw-rw-   0        0        0     1677 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_parameter_pb2.py
--rw-rw-rw-   0        0        0     2382 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_run_pb2.py
--rw-rw-rw-   0        0        0     1971 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/reportable_qualifier_definition_pb2.py
--rw-rw-rw-   0        0        0     1417 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/reportable_qualifier_pb2.py
--rw-rw-rw-   0        0        0     1252 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/rights_pb2.py
--rw-rw-rw-   0        0        0     2008 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/role_pb2.py
--rw-rw-rw-   0        0        0     1972 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/row_index_pb2.py
--rw-rw-rw-   0        0        0     1346 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/row_merge_result_pb2.py
--rw-rw-rw-   0        0        0     1692 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/row_pb2.py
--rw-rw-rw-   0        0        0     1403 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_occurrence_pb2.py
--rw-rw-rw-   0        0        0     2186 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_pb2.py
--rw-rw-rw-   0        0        0     1472 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_recurrence_pattern_pb2.py
--rw-rw-rw-   0        0        0     1887 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_type_pb2.py
--rw-rw-rw-   0        0        0     2533 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/scope_pb2.py
--rw-rw-rw-   0        0        0     1931 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/search_option_pb2.py
--rw-rw-rw-   0        0        0     2186 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/series_pb2.py
--rw-rw-rw-   0        0        0     2279 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/service_tech_tenant_request_pb2.py
--rw-rw-rw-   0        0        0     1649 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_connection_info_pb2.py
--rw-rw-rw-   0        0        0     1261 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py
--rw-rw-rw-   0        0        0     1567 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_payload_pb2.py
--rw-rw-rw-   0        0        0     1598 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_pb2.py
--rw-rw-rw-   0        0        0     1624 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_message_pb2.py
--rw-rw-rw-   0        0        0     1197 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_binding_pb2.py
--rw-rw-rw-   0        0        0     1699 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_computation_pb2.py
--rw-rw-rw-   0        0        0     1753 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_definition_pb2.py
--rw-rw-rw-   0        0        0     1500 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_pb2.py
--rw-rw-rw-   0        0        0     1820 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/template_parameter_pb2.py
--rw-rw-rw-   0        0        0     2465 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/tenant_pb2.py
--rw-rw-rw-   0        0        0     1680 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/tenant_product_offering_pb2.py
--rw-rw-rw-   0        0        0     2113 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/test_analyte_group_pb2.py
--rw-rw-rw-   0        0        0     1415 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/time_context_pb2.py
--rw-rw-rw-   0        0        0     2106 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/timeseriesdata_pb2.py
--rw-rw-rw-   0        0        0     1372 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/timewindow_pb2.py
--rw-rw-rw-   0        0        0     1499 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/timezones_pb2.py
--rw-rw-rw-   0        0        0     1835 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/unit_agency_code_pb2.py
--rw-rw-rw-   0        0        0     1627 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/unit_agency_code_type_pb2.py
--rw-rw-rw-   0        0        0     1701 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/unit_pb2.py
--rw-rw-rw-   0        0        0     1308 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_password_management_pb2.py
--rw-rw-rw-   0        0        0     4289 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_pb2.py
--rw-rw-rw-   0        0        0     1812 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_preference_pb2.py
--rw-rw-rw-   0        0        0     1969 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_profile_pb2.py
--rw-rw-rw-   0        0        0     1784 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/valid_value_pb2.py
--rw-rw-rw-   0        0        0     1966 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/variable_pb2.py
--rw-rw-rw-   0        0        0     1799 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/worksheet_definition_pb2.py
--rw-rw-rw-   0        0        0     1511 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/worksheet_pb2.py
--rw-rw-rw-   0        0        0     1789 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/worksheet_view_pb2.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:42:35.728315 one_interfaces-6.7.0/one_interfaces.egg-info/
--rw-rw-rw-   0        0        0     1217 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7545 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        4 2022-07-05 14:29:22.000000 one_interfaces-6.7.0/requirements.txt
--rw-rw-rw-   0        0        0      159 2024-04-03 13:42:35.732314 one_interfaces-6.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1714 2022-11-11 17:30:03.000000 one_interfaces-6.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:54:23.220019 one_interfaces-6.8.0/
+-rw-rw-rw-   0        0        0      580 2022-07-05 14:29:22.000000 one_interfaces-6.8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       62 2022-07-05 14:29:22.000000 one_interfaces-6.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1217 2024-04-11 15:54:23.221019 one_interfaces-6.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2022-11-11 17:33:49.000000 one_interfaces-6.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 15:54:23.212019 one_interfaces-6.8.0/one_interfaces/
+-rw-rw-rw-   0        0        0       23 2024-04-11 15:51:44.000000 one_interfaces-6.8.0/one_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/account_status_pb2.py
+-rw-rw-rw-   0        0        0     2440 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/activity_pb2.py
+-rw-rw-rw-   0        0        0     1899 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/activity_type_pb2.py
+-rw-rw-rw-   0        0        0     2231 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/address_pb2.py
+-rw-rw-rw-   0        0        0     1681 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/agency_pb2.py
+-rw-rw-rw-   0        0        0     1874 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_pb2.py
+-rw-rw-rw-   0        0        0     2811 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_result_pb2.py
+-rw-rw-rw-   0        0        0     1769 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_results_import_profile_pb2.py
+-rw-rw-rw-   0        0        0     1758 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_results_import_telemetry_pb2.py
+-rw-rw-rw-   0        0        0     1223 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/apierror_pb2.py
+-rw-rw-rw-   0        0        0     1393 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/apiresponse_pb2.py
+-rw-rw-rw-   0        0        0     1941 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/auditevent_pb2.py
+-rw-rw-rw-   0        0        0     1474 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cell_monitor_backup_pb2.py
+-rw-rw-rw-   0        0        0     1519 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cell_pb2.py
+-rw-rw-rw-   0        0        0     1541 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/celldata_binding_pb2.py
+-rw-rw-rw-   0        0        0     1988 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/celldata_pb2.py
+-rw-rw-rw-   0        0        0     1534 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cells_pb2.py
+-rw-rw-rw-   0        0        0     1871 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cellvalue_backup_pb2.py
+-rw-rw-rw-   0        0        0     4778 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/client_pb2.py
+-rw-rw-rw-   0        0        0     2054 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/coagmeasurement_pb2.py
+-rw-rw-rw-   0        0        0     2429 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/column_pb2.py
+-rw-rw-rw-   0        0        0     2097 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/computation_binding_pb2.py
+-rw-rw-rw-   0        0        0     2564 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/computation_pb2.py
+-rw-rw-rw-   0        0        0     1893 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/computation_variable_binding_pb2.py
+-rw-rw-rw-   0        0        0     2027 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/configuration_note_pb2.py
+-rw-rw-rw-   0        0        0     2970 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/configuration_pb2.py
+-rw-rw-rw-   0        0        0     1499 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/configuration_tag_pb2.py
+-rw-rw-rw-   0        0        0    13410 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/content_pb2.py
+-rw-rw-rw-   0        0        0     1951 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/csv_configuration_file_pb2.py
+-rw-rw-rw-   0        0        0     1743 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/data_source_binding_pb2.py
+-rw-rw-rw-   0        0        0     2052 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/data_source_configuration_pb2.py
+-rw-rw-rw-   0        0        0     1536 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     2041 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py
+-rw-rw-rw-   0        0        0     1523 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     3269 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_pb2.py
+-rw-rw-rw-   0        0        0     2247 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_pb2.py
+-rw-rw-rw-   0        0        0     3800 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     2063 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_type_pb2.py
+-rw-rw-rw-   0        0        0     2020 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_user_right_pb2.py
+-rw-rw-rw-   0        0        0     1342 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/display_options_pb2.py
+-rw-rw-rw-   0        0        0     1820 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_source_definition_pb2.py
+-rw-rw-rw-   0        0        0     1669 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_definition_pb2.py
+-rw-rw-rw-   0        0        0     1376 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_field_pb2.py
+-rw-rw-rw-   0        0        0     1605 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py
+-rw-rw-rw-   0        0        0     1508 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_pb2.py
+-rw-rw-rw-   0        0        0     2309 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_dataset_definition_pb2.py
+-rw-rw-rw-   0        0        0     1303 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_aggregate_pb2.py
+-rw-rw-rw-   0        0        0     1408 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_auditevent_pb2.py
+-rw-rw-rw-   0        0        0     1385 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_azure_notification_hubtype_pb2.py
+-rw-rw-rw-   0        0        0     1642 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_cell_range_action_pb2.py
+-rw-rw-rw-   0        0        0     1782 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_datasource_pb2.py
+-rw-rw-rw-   0        0        0     1392 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_day_pb2.py
+-rw-rw-rw-   0        0        0     1515 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py
+-rw-rw-rw-   0        0        0     1381 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_digital_twin_restriction_pb2.py
+-rw-rw-rw-   0        0        0     1422 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_digital_twin_user_right_pb2.py
+-rw-rw-rw-   0        0        0     1339 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_domain_source_pb2.py
+-rw-rw-rw-   0        0        0     1373 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_entity_pb2.py
+-rw-rw-rw-   0        0        0     1433 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_identity_provider_pb2.py
+-rw-rw-rw-   0        0        0     1552 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_import_status_pb2.py
+-rw-rw-rw-   0        0        0     1416 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_limit_operation_pb2.py
+-rw-rw-rw-   0        0        0     1437 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_limit_pb2.py
+-rw-rw-rw-   0        0        0     1545 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_month_pb2.py
+-rw-rw-rw-   0        0        0     1606 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_category_pb2.py
+-rw-rw-rw-   0        0        0     1557 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_delivery_method_pb2.py
+-rw-rw-rw-   0        0        0     1427 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_message_type_pb2.py
+-rw-rw-rw-   0        0        0     1346 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_platform_pb2.py
+-rw-rw-rw-   0        0        0     1452 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_one_log_level_pb2.py
+-rw-rw-rw-   0        0        0     1374 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_output_placement_pb2.py
+-rw-rw-rw-   0        0        0     1269 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_rendering_engine_pb2.py
+-rw-rw-rw-   0        0        0     1681 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py
+-rw-rw-rw-   0        0        0     1663 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_pb2.py
+-rw-rw-rw-   0        0        0     3080 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_sampling_statistic_pb2.py
+-rw-rw-rw-   0        0        0     1483 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_time_context_pb2.py
+-rw-rw-rw-   0        0        0     1388 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_time_unit_pb2.py
+-rw-rw-rw-   0        0        0    27482 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_timezone_pb2.py
+-rw-rw-rw-   0        0        0     1415 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_valid_value_restriction_pb2.py
+-rw-rw-rw-   0        0        0     1376 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_variable_type_pb2.py
+-rw-rw-rw-   0        0        0     2357 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_wims_week_definition_pb2.py
+-rw-rw-rw-   0        0        0     1341 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_worksheet_pb2.py
+-rw-rw-rw-   0        0        0     1768 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/execution_details_pb2.py
+-rw-rw-rw-   0        0        0     2010 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/execution_parameter_pb2.py
+-rw-rw-rw-   0        0        0     1211 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/expression_line_pb2.py
+-rw-rw-rw-   0        0        0     2205 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/feature_pb2.py
+-rw-rw-rw-   0        0        0     1589 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/feature_state_type_pb2.py
+-rw-rw-rw-   0        0        0     1793 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/file_configuration_pb2.py
+-rw-rw-rw-   0        0        0     1563 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/gauge_data_point_pb2.py
+-rw-rw-rw-   0        0        0     1560 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/gis_pb2.py
+-rw-rw-rw-   0        0        0     1231 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/historian_binding_pb2.py
+-rw-rw-rw-   0        0        0     1981 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/historian_data_pb2.py
+-rw-rw-rw-   0        0        0     1536 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/i18nkey_text_reference_pb2.py
+-rw-rw-rw-   0        0        0     1855 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/ingest_client_pb2.py
+-rw-rw-rw-   0        0        0     1698 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/jsonTicksDateTime_pb2.py
+-rw-rw-rw-   0        0        0     1325 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/key_value_pb2.py
+-rw-rw-rw-   0        0        0     1668 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/limit_configuration_pb2.py
+-rw-rw-rw-   0        0        0     2385 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/limit_pb2.py
+-rw-rw-rw-   0        0        0     1948 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/measurement_pb2.py
+-rw-rw-rw-   0        0        0     1768 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/model_execution_pb2.py
+-rw-rw-rw-   0        0        0     1424 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/model_location_pb2.py
+-rw-rw-rw-   0        0        0     2433 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/model_template_pb2.py
+-rw-rw-rw-   0        0        0     1233 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/multi_point2d_pb2.py
+-rw-rw-rw-   0        0        0     1233 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/multi_point3d_pb2.py
+-rw-rw-rw-   0        0        0     1472 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/note_pb2.py
+-rw-rw-rw-   0        0        0     1695 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_broadcast_pb2.py
+-rw-rw-rw-   0        0        0     1448 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_contact_pb2.py
+-rw-rw-rw-   0        0        0     1859 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_device_pb2.py
+-rw-rw-rw-   0        0        0     2430 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_direct_preference_pb2.py
+-rw-rw-rw-   0        0        0     2254 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_event_pb2.py
+-rw-rw-rw-   0        0        0     2267 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_in_app_notification_message_pb2.py
+-rw-rw-rw-   0        0        0     1743 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_preference_pb2.py
+-rw-rw-rw-   0        0        0     2174 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_template_pb2.py
+-rw-rw-rw-   0        0        0     2201 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_topic_pb2.py
+-rw-rw-rw-   0        0        0     1828 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_topic_variable_pb2.py
+-rw-rw-rw-   0        0        0     2450 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_user_preference_pb2.py
+-rw-rw-rw-   0        0        0     2455 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/operation_export_pb2.py
+-rw-rw-rw-   0        0        0     2111 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/outputcell_backup_pb2.py
+-rw-rw-rw-   0        0        0     1552 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/pagination_pb2.py
+-rw-rw-rw-   0        0        0     2177 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_agency_code_pb2.py
+-rw-rw-rw-   0        0        0     1674 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_agency_code_type_pb2.py
+-rw-rw-rw-   0        0        0     1819 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_definition_pb2.py
+-rw-rw-rw-   0        0        0     2356 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_pb2.py
+-rw-rw-rw-   0        0        0     2569 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/plant_status_pb2.py
+-rw-rw-rw-   0        0        0     1158 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/point2d_pb2.py
+-rw-rw-rw-   0        0        0     1186 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/point3d_pb2.py
+-rw-rw-rw-   0        0        0     1637 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/post_filtering_column_definition_pb2.py
+-rw-rw-rw-   0        0        0     1878 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/post_filtering_pb2.py
+-rw-rw-rw-   0        0        0     1585 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/privileges_pb2.py
+-rw-rw-rw-   0        0        0     2503 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/product_offering_pb2.py
+-rw-rw-rw-   0        0        0     2064 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/quantity_type_pb2.py
+-rw-rw-rw-   0        0        0     1448 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/record_auditinfo_pb2.py
+-rw-rw-rw-   0        0        0     2076 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_json_v2_pb2.py
+-rw-rw-rw-   0        0        0     2780 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_pb2.py
+-rw-rw-rw-   0        0        0     2178 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_runs_pb2.py
+-rw-rw-rw-   0        0        0     1842 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_tags_pb2.py
+-rw-rw-rw-   0        0        0     1677 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_parameter_pb2.py
+-rw-rw-rw-   0        0        0     2382 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_run_pb2.py
+-rw-rw-rw-   0        0        0     1971 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/reportable_qualifier_definition_pb2.py
+-rw-rw-rw-   0        0        0     1417 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/reportable_qualifier_pb2.py
+-rw-rw-rw-   0        0        0     1252 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/rights_pb2.py
+-rw-rw-rw-   0        0        0     2008 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/role_pb2.py
+-rw-rw-rw-   0        0        0     1972 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/row_index_pb2.py
+-rw-rw-rw-   0        0        0     1346 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/row_merge_result_pb2.py
+-rw-rw-rw-   0        0        0     1692 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/row_pb2.py
+-rw-rw-rw-   0        0        0     1403 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_occurrence_pb2.py
+-rw-rw-rw-   0        0        0     2186 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_pb2.py
+-rw-rw-rw-   0        0        0     1472 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_recurrence_pattern_pb2.py
+-rw-rw-rw-   0        0        0     1887 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_type_pb2.py
+-rw-rw-rw-   0        0        0     2533 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/scope_pb2.py
+-rw-rw-rw-   0        0        0     1931 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/search_option_pb2.py
+-rw-rw-rw-   0        0        0     2186 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/series_pb2.py
+-rw-rw-rw-   0        0        0     2279 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/service_tech_tenant_request_pb2.py
+-rw-rw-rw-   0        0        0     1649 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_connection_info_pb2.py
+-rw-rw-rw-   0        0        0     1261 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py
+-rw-rw-rw-   0        0        0     1567 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_payload_pb2.py
+-rw-rw-rw-   0        0        0     1598 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_pb2.py
+-rw-rw-rw-   0        0        0     1624 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_message_pb2.py
+-rw-rw-rw-   0        0        0     1197 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_binding_pb2.py
+-rw-rw-rw-   0        0        0     1699 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_computation_pb2.py
+-rw-rw-rw-   0        0        0     1753 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_definition_pb2.py
+-rw-rw-rw-   0        0        0     1500 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_pb2.py
+-rw-rw-rw-   0        0        0     1820 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/template_parameter_pb2.py
+-rw-rw-rw-   0        0        0     2465 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/tenant_pb2.py
+-rw-rw-rw-   0        0        0     1680 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/tenant_product_offering_pb2.py
+-rw-rw-rw-   0        0        0     2113 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/test_analyte_group_pb2.py
+-rw-rw-rw-   0        0        0     1415 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/time_context_pb2.py
+-rw-rw-rw-   0        0        0     2106 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/timeseriesdata_pb2.py
+-rw-rw-rw-   0        0        0     1372 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/timewindow_pb2.py
+-rw-rw-rw-   0        0        0     1499 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/timezones_pb2.py
+-rw-rw-rw-   0        0        0     1835 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/unit_agency_code_pb2.py
+-rw-rw-rw-   0        0        0     1627 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/unit_agency_code_type_pb2.py
+-rw-rw-rw-   0        0        0     1701 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/unit_pb2.py
+-rw-rw-rw-   0        0        0     1308 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/user_password_management_pb2.py
+-rw-rw-rw-   0        0        0     4289 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/user_pb2.py
+-rw-rw-rw-   0        0        0     1812 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/user_preference_pb2.py
+-rw-rw-rw-   0        0        0     1969 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/user_profile_pb2.py
+-rw-rw-rw-   0        0        0     1784 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/valid_value_pb2.py
+-rw-rw-rw-   0        0        0     1966 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/variable_pb2.py
+-rw-rw-rw-   0        0        0     1799 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/worksheet_definition_pb2.py
+-rw-rw-rw-   0        0        0     1511 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/worksheet_pb2.py
+-rw-rw-rw-   0        0        0     1789 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/worksheet_view_pb2.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:54:23.219348 one_interfaces-6.8.0/one_interfaces.egg-info/
+-rw-rw-rw-   0        0        0     1217 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7545 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        4 2022-07-05 14:29:22.000000 one_interfaces-6.8.0/requirements.txt
+-rw-rw-rw-   0        0        0      159 2024-04-11 15:54:23.222019 one_interfaces-6.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2022-11-11 17:30:03.000000 one_interfaces-6.8.0/setup.py
```

### Comparing `one_interfaces-6.7.0/LICENSE.txt` & `one_interfaces-6.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/PKG-INFO` & `one_interfaces-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: one_interfaces
-Version: 6.7.0
+Version: 6.8.0
 Summary: Python bindings for ONE.
 Home-page: https://github.com/aquaticinformatics/one_interfaces
 Author: Aquatic Informatics
 Author-email: info@aquaticinformatics.com
 Maintainer: Aquatic Informatics
 License: BSD
 Description: One_Interfaces
```

### Comparing `one_interfaces-6.7.0/one_interfaces/account_status_pb2.py` & `one_interfaces-6.8.0/one_interfaces/account_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/activity_pb2.py` & `one_interfaces-6.8.0/one_interfaces/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/activity_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/activity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/address_pb2.py` & `one_interfaces-6.8.0/one_interfaces/address_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/agency_pb2.py` & `one_interfaces-6.8.0/one_interfaces/agency_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/analyte_pb2.py` & `one_interfaces-6.8.0/one_interfaces/analyte_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/analyte_result_pb2.py` & `one_interfaces-6.8.0/one_interfaces/analyte_result_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/analyte_results_import_profile_pb2.py` & `one_interfaces-6.8.0/one_interfaces/analyte_results_import_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/analyte_results_import_telemetry_pb2.py` & `one_interfaces-6.8.0/one_interfaces/analyte_results_import_telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/apierror_pb2.py` & `one_interfaces-6.8.0/one_interfaces/apierror_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/apiresponse_pb2.py` & `one_interfaces-6.8.0/one_interfaces/apiresponse_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/auditevent_pb2.py` & `one_interfaces-6.8.0/one_interfaces/auditevent_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/cell_monitor_backup_pb2.py` & `one_interfaces-6.8.0/one_interfaces/cell_monitor_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/cell_pb2.py` & `one_interfaces-6.8.0/one_interfaces/cell_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/celldata_binding_pb2.py` & `one_interfaces-6.8.0/one_interfaces/celldata_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/celldata_pb2.py` & `one_interfaces-6.8.0/one_interfaces/celldata_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/cells_pb2.py` & `one_interfaces-6.8.0/one_interfaces/cells_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/cellvalue_backup_pb2.py` & `one_interfaces-6.8.0/one_interfaces/cellvalue_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/client_pb2.py` & `one_interfaces-6.8.0/one_interfaces/client_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/coagmeasurement_pb2.py` & `one_interfaces-6.8.0/one_interfaces/coagmeasurement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/column_pb2.py` & `one_interfaces-6.8.0/one_interfaces/column_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/computation_binding_pb2.py` & `one_interfaces-6.8.0/one_interfaces/computation_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/computation_pb2.py` & `one_interfaces-6.8.0/one_interfaces/computation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/computation_variable_binding_pb2.py` & `one_interfaces-6.8.0/one_interfaces/computation_variable_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/configuration_note_pb2.py` & `one_interfaces-6.8.0/one_interfaces/configuration_note_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/configuration_pb2.py` & `one_interfaces-6.8.0/one_interfaces/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/configuration_tag_pb2.py` & `one_interfaces-6.8.0/one_interfaces/configuration_tag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/content_pb2.py` & `one_interfaces-6.8.0/one_interfaces/content_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/csv_configuration_file_pb2.py` & `one_interfaces-6.8.0/one_interfaces/csv_configuration_file_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/data_source_binding_pb2.py` & `one_interfaces-6.8.0/one_interfaces/data_source_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/data_source_configuration_pb2.py` & `one_interfaces-6.8.0/one_interfaces/data_source_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/digital_twin_user_right_pb2.py` & `one_interfaces-6.8.0/one_interfaces/digital_twin_user_right_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/display_options_pb2.py` & `one_interfaces-6.8.0/one_interfaces/display_options_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enterprise_data_source_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enterprise_data_source_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_field_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_field_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enterprise_dataset_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enterprise_dataset_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_aggregate_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_aggregate_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_auditevent_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_auditevent_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_azure_notification_hubtype_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_azure_notification_hubtype_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_cell_range_action_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_cell_range_action_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_datasource_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_datasource_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x65num_datasource.proto*\xf1\x02\n\x0e\x45numDataSource\x12\x16\n\x12\x44\x41TASOURCE_UNKNOWN\x10\x00\x12\x13\n\x0f\x44\x41TASOURCE_FORM\x10\x01\x12\x1a\n\x16\x44\x41TASOURCE_COMPUTATION\x10\x02\x12\x1a\n\x16\x44\x41TASOURCE_SPREADSHEET\x10\x03\x12$\n DATASOURCE_INSTRUMENTMEASUREMENT\x10\x04\x12\x15\n\x11\x44\x41TASOURCE_IMPORT\x10\x05\x12%\n!DATASOURCE_SPREADSHEET_DEFINITION\x10\x06\x12\x16\n\x12\x44\x41TASOURCE_CONNECT\x10\x07\x12\x1d\n\x19\x44\x41TASOURCE_SAMPLE_MANAGER\x10\x08\x12\x18\n\x14\x44\x41TASOURCE_WIMS_SYNC\x10\t\x12\x1f\n\x1b\x44\x41TASOURCE_WIMS_COMPUTATION\x10\n\x12$\n DATASOURCE_SPREADSHEET_HISTORIAN\x10\x0b\x42\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x65num_datasource.proto*\x8f\x03\n\x0e\x45numDataSource\x12\x16\n\x12\x44\x41TASOURCE_UNKNOWN\x10\x00\x12\x13\n\x0f\x44\x41TASOURCE_FORM\x10\x01\x12\x1a\n\x16\x44\x41TASOURCE_COMPUTATION\x10\x02\x12\x1a\n\x16\x44\x41TASOURCE_SPREADSHEET\x10\x03\x12$\n DATASOURCE_INSTRUMENTMEASUREMENT\x10\x04\x12\x15\n\x11\x44\x41TASOURCE_IMPORT\x10\x05\x12%\n!DATASOURCE_SPREADSHEET_DEFINITION\x10\x06\x12\x16\n\x12\x44\x41TASOURCE_CONNECT\x10\x07\x12\x1d\n\x19\x44\x41TASOURCE_SAMPLE_MANAGER\x10\x08\x12\x18\n\x14\x44\x41TASOURCE_WIMS_SYNC\x10\t\x12\x1f\n\x1b\x44\x41TASOURCE_WIMS_COMPUTATION\x10\n\x12$\n DATASOURCE_SPREADSHEET_HISTORIAN\x10\x0b\x12\x1c\n\x18\x44\x41TASOURCE_PROCESS_MODEL\x10\x0c\x42\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'enum_datasource_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
   _globals['_ENUMDATASOURCE']._serialized_start=26
-  _globals['_ENUMDATASOURCE']._serialized_end=395
+  _globals['_ENUMDATASOURCE']._serialized_end=425
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_day_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_day_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_digital_twin_restriction_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_digital_twin_restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_digital_twin_user_right_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_digital_twin_user_right_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_domain_source_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_domain_source_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_entity_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_identity_provider_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_identity_provider_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_import_status_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_import_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_limit_operation_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_limit_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_limit_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_limit_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x65num_limit.proto*\xa7\x01\n\tEnumLimit\x12\x11\n\rLIMIT_UNKNOWN\x10\x00\x12\x13\n\x0fLIMIT_HIGHALARM\x10\x01\x12\x12\n\x0eLIMIT_HIGHNEAR\x10\x02\x12\x11\n\rLIMIT_LOWNEAR\x10\x03\x12\x12\n\x0eLIMIT_LOWALARM\x10\x04\x12\x14\n\x10LIMIT_REGULATORY\x10\x05\x12\x11\n\rLIMIT_WARNING\x10\x06\x12\x0e\n\nLIMIT_GOAL\x10\x07\x42\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x65num_limit.proto*\xc2\x01\n\tEnumLimit\x12\x11\n\rLIMIT_UNKNOWN\x10\x00\x12\x13\n\x0fLIMIT_HIGHALARM\x10\x01\x12\x12\n\x0eLIMIT_HIGHNEAR\x10\x02\x12\x11\n\rLIMIT_LOWNEAR\x10\x03\x12\x12\n\x0eLIMIT_LOWALARM\x10\x04\x12\x14\n\x10LIMIT_REGULATORY\x10\x05\x12\x11\n\rLIMIT_WARNING\x10\x06\x12\x0e\n\nLIMIT_GOAL\x10\x07\x12\x19\n\x15LIMIT_LEVEL_THRESHOLD\x10\x08\x42\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'enum_limit_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
   _globals['_ENUMLIMIT']._serialized_start=21
-  _globals['_ENUMLIMIT']._serialized_end=188
+  _globals['_ENUMLIMIT']._serialized_end=215
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_month_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_month_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_notification_category_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_notification_category_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_notification_delivery_method_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_notification_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_notification_message_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_notification_message_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_notification_platform_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_notification_platform_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_one_log_level_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_one_log_level_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_output_placement_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_output_placement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_rendering_engine_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_rendering_engine_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_sampling_statistic_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_sampling_statistic_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_time_context_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_time_context_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_time_unit_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_time_unit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_timezone_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_timezone_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_valid_value_restriction_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_valid_value_restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_variable_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_variable_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_wims_week_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_wims_week_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/enum_worksheet_pb2.py` & `one_interfaces-6.8.0/one_interfaces/enum_worksheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/execution_details_pb2.py` & `one_interfaces-6.8.0/one_interfaces/execution_details_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/execution_parameter_pb2.py` & `one_interfaces-6.8.0/one_interfaces/execution_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/expression_line_pb2.py` & `one_interfaces-6.8.0/one_interfaces/expression_line_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/feature_pb2.py` & `one_interfaces-6.8.0/one_interfaces/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/feature_state_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/feature_state_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/file_configuration_pb2.py` & `one_interfaces-6.8.0/one_interfaces/file_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/gauge_data_point_pb2.py` & `one_interfaces-6.8.0/one_interfaces/gauge_data_point_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/gis_pb2.py` & `one_interfaces-6.8.0/one_interfaces/gis_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/historian_binding_pb2.py` & `one_interfaces-6.8.0/one_interfaces/historian_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/historian_data_pb2.py` & `one_interfaces-6.8.0/one_interfaces/historian_data_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/i18nkey_text_reference_pb2.py` & `one_interfaces-6.8.0/one_interfaces/i18nkey_text_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/ingest_client_pb2.py` & `one_interfaces-6.8.0/one_interfaces/ingest_client_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/jsonTicksDateTime_pb2.py` & `one_interfaces-6.8.0/one_interfaces/jsonTicksDateTime_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/key_value_pb2.py` & `one_interfaces-6.8.0/one_interfaces/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/limit_configuration_pb2.py` & `one_interfaces-6.8.0/one_interfaces/limit_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/limit_pb2.py` & `one_interfaces-6.8.0/one_interfaces/limit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/measurement_pb2.py` & `one_interfaces-6.8.0/one_interfaces/measurement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/model_execution_pb2.py` & `one_interfaces-6.8.0/one_interfaces/model_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/model_location_pb2.py` & `one_interfaces-6.8.0/one_interfaces/model_location_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/model_template_pb2.py` & `one_interfaces-6.8.0/one_interfaces/model_template_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 import template_parameter_pb2 as template__parameter__pb2
 import model_location_pb2 as model__location__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14model_template.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x18template_parameter.proto\x1a\x14model_location.proto\"\xde\x03\n\rModelTemplate\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\ttwinRefId\x18\x03 \x01(\t\x12\x17\n\x0f\x65xternalModelId\x18\x04 \x01(\t\x12\x1a\n\x12simulationInterval\x18\x05 \x01(\t\x12\x1d\n\x15\x66orecastDurationHours\x18\x06 \x01(\x01\x12\x1d\n\x15inputDataSourceDriver\x18\x07 \x01(\t\x12\x34\n\x0einputDataSetId\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1e\n\x16outputDataSourceDriver\x18\t \x01(\t\x12\x35\n\x0foutputDataSetId\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12!\n\tlocations\x18\x0b \x03(\x0b\x32\x0e.ModelLocation\x12\"\n\x06inputs\x18\x0c \x03(\x0b\x32\x12.TemplateParameter\x12#\n\x07outputs\x18\r \x03(\x0b\x32\x12.TemplateParameter\x12-\n\x07\x63omment\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\"/\n\x0eModelTemplates\x12\x1d\n\x05items\x18\x01 \x03(\x0b\x32\x0e.ModelTemplateB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14model_template.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x18template_parameter.proto\x1a\x14model_location.proto\"\xef\x03\n\rModelTemplate\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\ttwinRefId\x18\x03 \x01(\t\x12\x17\n\x0f\x65xternalModelId\x18\x04 \x01(\t\x12\x1a\n\x12simulationInterval\x18\x05 \x01(\t\x12\x1d\n\x15\x66orecastDurationHours\x18\x06 \x01(\x01\x12\x1d\n\x15inputDataSourceDriver\x18\x07 \x01(\t\x12\x34\n\x0einputDataSetId\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1e\n\x16outputDataSourceDriver\x18\t \x01(\t\x12\x35\n\x0foutputDataSetId\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12!\n\tlocations\x18\x0b \x03(\x0b\x32\x0e.ModelLocation\x12\"\n\x06inputs\x18\x0c \x03(\x0b\x32\x12.TemplateParameter\x12#\n\x07outputs\x18\r \x03(\x0b\x32\x12.TemplateParameter\x12-\n\x07\x63omment\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x0f\n\x07\x65nabled\x18\x0f \x01(\x08\"/\n\x0eModelTemplates\x12\x1d\n\x05items\x18\x01 \x03(\x0b\x32\x0e.ModelTemplateB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'model_template_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
   _globals['_MODELTEMPLATE']._serialized_start=105
-  _globals['_MODELTEMPLATE']._serialized_end=583
-  _globals['_MODELTEMPLATES']._serialized_start=585
-  _globals['_MODELTEMPLATES']._serialized_end=632
+  _globals['_MODELTEMPLATE']._serialized_end=600
+  _globals['_MODELTEMPLATES']._serialized_start=602
+  _globals['_MODELTEMPLATES']._serialized_end=649
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.7.0/one_interfaces/multi_point2d_pb2.py` & `one_interfaces-6.8.0/one_interfaces/multi_point2d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/multi_point3d_pb2.py` & `one_interfaces-6.8.0/one_interfaces/multi_point3d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/note_pb2.py` & `one_interfaces-6.8.0/one_interfaces/note_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_broadcast_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_broadcast_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_contact_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_contact_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_device_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_device_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_direct_preference_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_direct_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_event_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_in_app_notification_message_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_in_app_notification_message_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_preference_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_template_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_template_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_topic_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_topic_variable_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_topic_variable_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/notification_user_preference_pb2.py` & `one_interfaces-6.8.0/one_interfaces/notification_user_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/operation_export_pb2.py` & `one_interfaces-6.8.0/one_interfaces/operation_export_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/outputcell_backup_pb2.py` & `one_interfaces-6.8.0/one_interfaces/outputcell_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/pagination_pb2.py` & `one_interfaces-6.8.0/one_interfaces/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/parameter_agency_code_pb2.py` & `one_interfaces-6.8.0/one_interfaces/parameter_agency_code_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/parameter_agency_code_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/parameter_agency_code_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/parameter_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/parameter_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/parameter_pb2.py` & `one_interfaces-6.8.0/one_interfaces/parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/plant_status_pb2.py` & `one_interfaces-6.8.0/one_interfaces/plant_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/point2d_pb2.py` & `one_interfaces-6.8.0/one_interfaces/point2d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/point3d_pb2.py` & `one_interfaces-6.8.0/one_interfaces/point3d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/post_filtering_column_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/post_filtering_column_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/post_filtering_pb2.py` & `one_interfaces-6.8.0/one_interfaces/post_filtering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/privileges_pb2.py` & `one_interfaces-6.8.0/one_interfaces/privileges_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/product_offering_pb2.py` & `one_interfaces-6.8.0/one_interfaces/product_offering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/quantity_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/quantity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/record_auditinfo_pb2.py` & `one_interfaces-6.8.0/one_interfaces/record_auditinfo_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/report_definition_json_v2_pb2.py` & `one_interfaces-6.8.0/one_interfaces/report_definition_json_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/report_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/report_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/report_definition_runs_pb2.py` & `one_interfaces-6.8.0/one_interfaces/report_definition_runs_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/report_definition_tags_pb2.py` & `one_interfaces-6.8.0/one_interfaces/report_definition_tags_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/report_parameter_pb2.py` & `one_interfaces-6.8.0/one_interfaces/report_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/report_run_pb2.py` & `one_interfaces-6.8.0/one_interfaces/report_run_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/reportable_qualifier_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/reportable_qualifier_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/reportable_qualifier_pb2.py` & `one_interfaces-6.8.0/one_interfaces/reportable_qualifier_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/rights_pb2.py` & `one_interfaces-6.8.0/one_interfaces/rights_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/role_pb2.py` & `one_interfaces-6.8.0/one_interfaces/role_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/row_index_pb2.py` & `one_interfaces-6.8.0/one_interfaces/row_index_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/row_merge_result_pb2.py` & `one_interfaces-6.8.0/one_interfaces/row_merge_result_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/row_pb2.py` & `one_interfaces-6.8.0/one_interfaces/row_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/schedule_occurrence_pb2.py` & `one_interfaces-6.8.0/one_interfaces/schedule_occurrence_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/schedule_pb2.py` & `one_interfaces-6.8.0/one_interfaces/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/schedule_recurrence_pattern_pb2.py` & `one_interfaces-6.8.0/one_interfaces/schedule_recurrence_pattern_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/schedule_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/schedule_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/scope_pb2.py` & `one_interfaces-6.8.0/one_interfaces/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/search_option_pb2.py` & `one_interfaces-6.8.0/one_interfaces/search_option_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/series_pb2.py` & `one_interfaces-6.8.0/one_interfaces/series_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/service_tech_tenant_request_pb2.py` & `one_interfaces-6.8.0/one_interfaces/service_tech_tenant_request_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_connection_info_pb2.py` & `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py` & `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_payload_pb2.py` & `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_payload_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_pb2.py` & `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_message_pb2.py` & `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_message_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/spreadsheet_binding_pb2.py` & `one_interfaces-6.8.0/one_interfaces/spreadsheet_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/spreadsheet_computation_pb2.py` & `one_interfaces-6.8.0/one_interfaces/spreadsheet_computation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/spreadsheet_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/spreadsheet_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/spreadsheet_pb2.py` & `one_interfaces-6.8.0/one_interfaces/spreadsheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/template_parameter_pb2.py` & `one_interfaces-6.8.0/one_interfaces/template_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/tenant_pb2.py` & `one_interfaces-6.8.0/one_interfaces/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/tenant_product_offering_pb2.py` & `one_interfaces-6.8.0/one_interfaces/tenant_product_offering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/test_analyte_group_pb2.py` & `one_interfaces-6.8.0/one_interfaces/test_analyte_group_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/time_context_pb2.py` & `one_interfaces-6.8.0/one_interfaces/time_context_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/timeseriesdata_pb2.py` & `one_interfaces-6.8.0/one_interfaces/timeseriesdata_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/timewindow_pb2.py` & `one_interfaces-6.8.0/one_interfaces/timewindow_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/timezones_pb2.py` & `one_interfaces-6.8.0/one_interfaces/timezones_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/unit_agency_code_pb2.py` & `one_interfaces-6.8.0/one_interfaces/unit_agency_code_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/unit_agency_code_type_pb2.py` & `one_interfaces-6.8.0/one_interfaces/unit_agency_code_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/unit_pb2.py` & `one_interfaces-6.8.0/one_interfaces/unit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/user_password_management_pb2.py` & `one_interfaces-6.8.0/one_interfaces/user_password_management_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/user_pb2.py` & `one_interfaces-6.8.0/one_interfaces/user_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/user_preference_pb2.py` & `one_interfaces-6.8.0/one_interfaces/user_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/user_profile_pb2.py` & `one_interfaces-6.8.0/one_interfaces/user_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/valid_value_pb2.py` & `one_interfaces-6.8.0/one_interfaces/valid_value_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/variable_pb2.py` & `one_interfaces-6.8.0/one_interfaces/variable_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/worksheet_definition_pb2.py` & `one_interfaces-6.8.0/one_interfaces/worksheet_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/worksheet_pb2.py` & `one_interfaces-6.8.0/one_interfaces/worksheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces/worksheet_view_pb2.py` & `one_interfaces-6.8.0/one_interfaces/worksheet_view_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/one_interfaces.egg-info/PKG-INFO` & `one_interfaces-6.8.0/one_interfaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: one-interfaces
-Version: 6.7.0
+Version: 6.8.0
 Summary: Python bindings for ONE.
 Home-page: https://github.com/aquaticinformatics/one_interfaces
 Author: Aquatic Informatics
 Author-email: info@aquaticinformatics.com
 Maintainer: Aquatic Informatics
 License: BSD
 Description: One_Interfaces
```

### Comparing `one_interfaces-6.7.0/one_interfaces.egg-info/SOURCES.txt` & `one_interfaces-6.8.0/one_interfaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.7.0/setup.py` & `one_interfaces-6.8.0/setup.py`

 * *Files identical despite different names*

