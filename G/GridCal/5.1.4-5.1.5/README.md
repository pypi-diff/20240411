# Comparing `tmp/GridCal-5.1.4.tar.gz` & `tmp/GridCal-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCal-5.1.4.tar", last modified: Tue Apr  9 17:48:33 2024, max compression
+gzip compressed data, was "GridCal-5.1.5.tar", last modified: Thu Apr 11 17:55:34 2024, max compression
```

## Comparing `GridCal-5.1.4.tar` & `GridCal-5.1.5.tar`

### file list

```diff
@@ -1,225 +1,227 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-09 17:48:10.240457 GridCal-5.1.4/GridCal/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.4/GridCal/ExecuteGridCal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.4/GridCal/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.4/GridCal/update.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.4/GridCal/templates.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.4/GridCal/Session/results_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Session/export_results_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Session/session.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Session/synchronization_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Session/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.4/GridCal/Session/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.4/GridCal/data/cables.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.4/GridCal/data/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      388 2024-04-09 17:48:10.240457 GridCal-5.1.4/GridCal/data/sequence_lines.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.4/GridCal/data/transformers.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.4/GridCal/data/wires.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.4/GridCal/Gui/GeneralDialogues.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/update_gui_all.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/messages.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/themes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.4/GridCal/Gui/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    85064 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/GuiFunctions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/plot_config.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/update_gui_common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/Widgets/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/Widgets/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/Widgets/custom_qrangeslider.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.4/GridCal/Gui/CoordinatesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.4/GridCal/Gui/CoordinatesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/CoordinatesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/CoordinatesInput/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.4/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.4/GridCal/Gui/TowerBuilder/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.4/GridCal/Gui/TowerBuilder/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.4/GridCal/Gui/TowerBuilder/table_models.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/TowerBuilder/test_.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Gui/TowerBuilder/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Gui/TowerBuilder/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.4/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/graphics_manager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.4/GridCal/Gui/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/diagrams_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   183547 2024-04-09 17:48:10.232457 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6687 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6203 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16999 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13480 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4212 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12258 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4852 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9421 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9485 2024-04-09 17:48:10.232457 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4683 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32907 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30218 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21562 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30410 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   160152 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/node_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/map_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19136 2024-04-08 13:34:15.959164 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4856 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1854 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.4/GridCal/Gui/AboutDialogue/about_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.4/GridCal/Gui/AboutDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.4/GridCal/Gui/AboutDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.4/GridCal/Gui/AboutDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.4/GridCal/Gui/AboutDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.4/GridCal/Gui/ProfilesInput/excel_dialog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.4/GridCal/Gui/ProfilesInput/profiles_from_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.4/GridCal/Gui/ProfilesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.4/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.4/GridCal/Gui/ProfilesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.4/GridCal/Gui/ProfilesInput/models_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.4/GridCal/Gui/ProfilesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/ProfilesInput/profile_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.4/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/Analysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/Analysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/Analysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.4/GridCal/Gui/Analysis/AnalysisDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/Analysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.4/GridCal/Gui/Analysis/object_plot_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.4/GridCal/Gui/CascadingSteps/cascading_steps.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/CascadingSteps/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/CascadingSteps/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.4/GridCal/Gui/CascadingSteps/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.4/GridCal/Gui/Main/ConsoleLogController.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.4/GridCal/Gui/Main/GridCalMain.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   275391 2024-04-09 17:48:10.232457 GridCal-5.1.4/GridCal/Gui/Main/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.4/GridCal/Gui/Main/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.4/GridCal/Gui/Main/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-09 17:48:10.232457 GridCal-5.1.4/GridCal/Gui/Main/ConsoleLog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   807547 2024-04-09 17:48:10.240457 GridCal-5.1.4/GridCal/Gui/Main/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/Main/object_select_window.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/README.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)   110018 2024-04-08 13:34:15.963164 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/simulations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33842 2024-04-08 13:34:15.963164 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/io.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31266 2024-04-08 13:34:15.963164 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/base_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Settings/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17616 2024-04-08 13:34:15.963164 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Settings/configuration.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45037 2024-04-08 13:34:15.963164 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/objects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20949 2024-03-28 10:16:48.960877 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/time_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    71734 2024-04-09 17:48:10.236457 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/diagrams.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Results/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Results/results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.4/GridCal/Gui/Visualization/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/Visualization/visualization.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/Visualization/palettes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.4/GridCal/Gui/SyncDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.4/GridCal/Gui/SyncDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/SyncDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Gui/SyncDialogue/sync_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/SyncDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/RosetaExplorer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/RosetaExplorer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/RosetaExplorer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.4/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/RosetaExplorer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.4/GridCal/Gui/LoadDesigner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.4/GridCal/Gui/LoadDesigner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.4/GridCal/Gui/LoadDesigner/load_designer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.4/GridCal/Gui/LoadDesigner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.4/GridCal/Gui/LoadDesigner/load_designer_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.4/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/WindPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/WindPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/WindPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/WindPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.4/GridCal/Gui/SystemScaler/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.4/GridCal/Gui/SystemScaler/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.4/GridCal/Gui/SystemScaler/system_scaler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.4/GridCal/Gui/SystemScaler/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.4/GridCal/Gui/SystemScaler/system_scaler_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/TreeModelViewer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.4/GridCal/Gui/TreeModelViewer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/TreeModelViewer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.4/GridCal/Gui/TreeModelViewer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.4/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.4/GridCal/Gui/GridGenerator/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.4/GridCal/Gui/GridGenerator/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.4/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.4/GridCal/Gui/GridGenerator/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.4/GridCal/Gui/GridGenerator/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4902 2024-03-11 19:28:12.175075 GridCal-5.1.4/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-09 17:48:33.600457 GridCal-5.1.4/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-09 17:48:33.600457 GridCal-5.1.4/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-11 15:31:05.578472 GridCal-5.1.5/GridCal/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/ExecuteGridCal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.5/GridCal/update.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/templates.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.5/GridCal/Session/results_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/export_results_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/session.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/synchronization_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.5/GridCal/Session/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.5/GridCal/data/cables.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.5/GridCal/data/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      388 2024-04-11 15:31:05.578472 GridCal-5.1.5/GridCal/data/sequence_lines.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.5/GridCal/data/transformers.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.5/GridCal/data/wires.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.5/GridCal/Gui/GeneralDialogues.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/update_gui_all.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/messages.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/themes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.5/GridCal/Gui/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    85064 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/GuiFunctions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/plot_config.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/update_gui_common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/Widgets/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Widgets/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/Widgets/custom_qrangeslider.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/TowerBuilder/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/TowerBuilder/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/Gui/TowerBuilder/table_models.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/TowerBuilder/test_.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/TowerBuilder/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/TowerBuilder/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.5/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/graphics_manager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.5/GridCal/Gui/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/diagrams_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   186520 2024-04-11 16:03:35.834534 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6687 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6203 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16999 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13480 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4212 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12258 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4852 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9421 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9485 2024-04-11 15:31:05.570472 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4683 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32907 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30218 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21562 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30410 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   160182 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/node_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20956 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4966 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2159 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4975 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1917 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/Gui/AboutDialogue/about_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.5/GridCal/Gui/AboutDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.5/GridCal/Gui/AboutDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.5/GridCal/Gui/AboutDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/Gui/AboutDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_dialog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.5/GridCal/Gui/ProfilesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.5/GridCal/Gui/ProfilesInput/models_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profile_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/Gui/Analysis/AnalysisDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.5/GridCal/Gui/Analysis/object_plot_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/CascadingSteps/cascading_steps.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CascadingSteps/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CascadingSteps/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CascadingSteps/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.5/GridCal/Gui/Main/ConsoleLogController.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.5/GridCal/Gui/Main/GridCalMain.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   277012 2024-04-11 17:39:50.574328 GridCal-5.1.5/GridCal/Gui/Main/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/Main/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-11 17:39:50.802328 GridCal-5.1.5/GridCal/Gui/Main/ConsoleLog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   762396 2024-04-11 17:39:50.342328 GridCal-5.1.5/GridCal/Gui/Main/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Main/object_select_window.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/README.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)   110018 2024-04-08 13:34:15.963164 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/simulations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33887 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/io.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31266 2024-04-08 13:34:15.963164 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/base_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Settings/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17930 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Settings/configuration.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45640 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/objects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21114 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/time_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    71734 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/diagrams.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Results/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Results/results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/Visualization/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Visualization/visualization.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Visualization/palettes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/SyncDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/SyncDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SyncDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/SyncDialogue/sync_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SyncDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.5/GridCal/Gui/LoadDesigner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/GridGenerator/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.5/GridCal/Gui/GridGenerator/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.5/GridCal/Gui/GridGenerator/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.5/GridCal/Gui/GridGenerator/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4923 2024-04-11 17:44:56.522321 GridCal-5.1.5/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-11 17:55:34.142307 GridCal-5.1.5/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-11 17:55:34.142307 GridCal-5.1.5/setup.cfg
```

### Comparing `GridCal-5.1.4/GridCal/__version__.py` & `GridCal-5.1.5/GridCal/__version__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCal_VERSION__ = "5.1.4"
+__GridCal_VERSION__ = "5.1.5"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCal_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCal-5.1.4/GridCal/__init__.py` & `GridCal-5.1.5/GridCal/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/ExecuteGridCal.py` & `GridCal-5.1.5/GridCal/ExecuteGridCal.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/LICENSE.txt` & `GridCal-5.1.5/GridCal/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/update.py` & `GridCal-5.1.5/GridCal/update.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/templates.py` & `GridCal-5.1.5/GridCal/templates.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Session/results_model.py` & `GridCal-5.1.5/GridCal/Session/results_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Session/export_results_driver.py` & `GridCal-5.1.5/GridCal/Session/export_results_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Session/session.py` & `GridCal-5.1.5/GridCal/Session/session.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Session/synchronization_driver.py` & `GridCal-5.1.5/GridCal/Session/synchronization_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Session/file_handler.py` & `GridCal-5.1.5/GridCal/Session/file_handler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/data/cables.csv` & `GridCal-5.1.5/GridCal/data/cables.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/data/transformers.csv` & `GridCal-5.1.5/GridCal/data/transformers.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/data/wires.csv` & `GridCal-5.1.5/GridCal/data/wires.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/GeneralDialogues.py` & `GridCal-5.1.5/GridCal/Gui/GeneralDialogues.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/update_gui_all.py` & `GridCal-5.1.5/GridCal/Gui/update_gui_all.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/messages.py` & `GridCal-5.1.5/GridCal/Gui/messages.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/themes.py` & `GridCal-5.1.5/GridCal/Gui/themes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ConsoleWidget.py` & `GridCal-5.1.5/GridCal/Gui/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/GuiFunctions.py` & `GridCal-5.1.5/GridCal/Gui/GuiFunctions.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/plot_config.py` & `GridCal-5.1.5/GridCal/Gui/plot_config.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/update_gui_common.py` & `GridCal-5.1.5/GridCal/Gui/update_gui_common.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Widgets/matplotlibwidget.py` & `GridCal-5.1.5/GridCal/Gui/Widgets/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Widgets/custom_qrangeslider.py` & `GridCal-5.1.5/GridCal/Gui/Widgets/custom_qrangeslider.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ContingencyPlanner/gui.py` & `GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/CoordinatesInput/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/CoordinatesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/CoordinatesInput/gui.py` & `GridCal-5.1.5/GridCal/Gui/CoordinatesInput/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TowerBuilder/table_models.py` & `GridCal-5.1.5/GridCal/Gui/TowerBuilder/table_models.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TowerBuilder/test_.py` & `GridCal-5.1.5/GridCal/Gui/TowerBuilder/test_.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TowerBuilder/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/TowerBuilder/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TowerBuilder/gui.py` & `GridCal-5.1.5/GridCal/Gui/TowerBuilder/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py` & `GridCal-5.1.5/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/graphics_manager.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/graphics_manager.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/diagrams_model.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/diagrams_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
                                QSplitter, QMessageBox, QAbstractItemView, QGraphicsScene, QGraphicsSceneMouseEvent,
                                QGraphicsItem, QGraphicsTextItem, QMenu, QWidget)
 from PySide6.QtSvg import QSvgGenerator
 
 from GridCalEngine.Devices.types import ALL_DEV_TYPES, INJECTION_DEVICE_TYPES, FLUID_TYPES
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCalEngine.Devices.Substation.bus import Bus
+from GridCalEngine.Devices.Substation.substation import Substation
+from GridCalEngine.Devices.Substation.voltage_level import VoltageLevel
 from GridCalEngine.Devices.Substation.busbar import BusBar
 from GridCalEngine.Devices.Substation.connectivity_node import ConnectivityNode
 from GridCalEngine.Devices.Branches.line import Line
 from GridCalEngine.Devices.Branches.dc_line import DcLine
 from GridCalEngine.Devices.Branches.transformer import Transformer2W
 from GridCalEngine.Devices.Branches.vsc import VSC
 from GridCalEngine.Devices.Branches.upfc import UPFC
@@ -3610,14 +3612,148 @@
 
                 if ok:
                     if api_object.active:
                         api_object.active_prof.fill(True)
                     else:
                         api_object.active_prof.fill(False)
 
+    def split_line_now(self, line_graphics: LineGraphicItem, position: float, extra_km: float):
+        """
+
+        :param line_graphics:
+        :param position:
+        :param extra_km:
+        :return:
+        """
+
+        if 0.0 < position < 1.0:
+
+            # Each of the Branches will have the proportional impedance
+            # Bus_from           Middle_bus            Bus_To
+            # o----------------------o--------------------o
+            #   >-------- x -------->|
+            #   (x: distance measured in per unit (0~1)
+            line = line_graphics.api_object
+            name = line.name + ' split'
+            mid_sub = Substation(name=name,
+                                 area=line.bus_from.area,
+                                 zone=line.bus_from.zone,
+                                 country=line.bus_from.country)
+            mid_vl = VoltageLevel(name=name, substation=mid_sub)
+            mid_bus = Bus(name=name,
+                          vnom=line.bus_from.Vnom,
+                          vmin=line.bus_from.Vmin,
+                          vmax=line.bus_from.Vmax,
+                          voltage_level=mid_vl,
+                          substation=mid_sub,
+                          area=line.bus_from.area,
+                          zone=line.bus_from.zone,
+                          country=line.bus_from.country)
+
+            bus_f_graphics_data = self.diagram.query_point(line.bus_from)
+            bus_t_graphics_data = self.diagram.query_point(line.bus_to)
+            bus_f_graphic_obj = self.graphics_manager.query(line.bus_from)
+            bus_t_graphic_obj = self.graphics_manager.query(line.bus_to)
+
+            if bus_f_graphics_data is None:
+                error_msg(f"{line.bus_from} was not found in the diagram")
+                return None
+            if bus_t_graphics_data is None:
+                error_msg(f"{line.bus_to} was not found in the diagram")
+                return None
+            if bus_f_graphic_obj is None:
+                error_msg(f"{line.bus_from} was not found in the graphics manager")
+                return None
+            if bus_t_graphic_obj is None:
+                error_msg(f"{line.bus_to} was not found in the graphics manager")
+                return None
+
+            # C(x, y) = (x1 + t * (x2 - x1), y1 + t * (y2 - y1))
+            middle_bus_x = int(bus_f_graphics_data.x + (bus_t_graphics_data.x - bus_f_graphics_data.x) * position)
+            middle_bus_y = int(bus_f_graphics_data.y + (bus_t_graphics_data.y - bus_f_graphics_data.y) * position)
+
+            position_a = position + (extra_km / line.length) if line.length > 0.0 else position
+
+            # create first split
+            br1 = Line(name=line.name + ' split 1',
+                       bus_from=line.bus_from,
+                       bus_to=mid_bus,
+                       r=line.R * position_a,
+                       x=line.X * position_a,
+                       b=line.B * position_a,
+                       r0=line.R0 * position_a,
+                       x0=line.X0 * position_a,
+                       b0=line.B0 * position_a,
+                       r2=line.R2 * position_a,
+                       x2=line.X2 * position_a,
+                       b2=line.B2 * position_a,
+                       length=line.length * position_a,
+                       rate=line.rate,
+                       contingency_factor=line.contingency_factor,
+                       protection_rating_factor=line.protection_rating_factor)
+
+            position_c = (1.0 - position) + (extra_km / line.length) if line.length > 0.0 else (1.0 - position)
+            br2 = Line(name=line.name + ' split 2',
+                       bus_from=mid_bus,
+                       bus_to=line.bus_to,
+                       r=line.R * position_c,
+                       x=line.X * position_c,
+                       b=line.B * position_c,
+                       r0=line.R0 * position_c,
+                       x0=line.X0 * position_c,
+                       b0=line.B0 * position_c,
+                       r2=line.R2 * position_c,
+                       x2=line.X2 * position_c,
+                       b2=line.B2 * position_c,
+                       length=line.length * position_c,
+                       rate=line.rate,
+                       contingency_factor=line.contingency_factor,
+                       protection_rating_factor=line.protection_rating_factor)
+
+            # deactivate the original line
+            line_graphics.api_object.active = False
+            line_graphics.api_object.active_prof.fill(False)
+            line_graphics.set_enable(False)
+
+            # add to gridcal the new 2 lines and the bus
+            self.circuit.add_bus(mid_bus)
+            self.circuit.add_line(br1)
+            self.circuit.add_line(br2)
+
+            # add new stuff as new investment
+            inv_group = InvestmentsGroup(name=line.name + ' split', category='Line split')
+            self.circuit.add_investments_group(inv_group)
+            self.circuit.add_investment(
+                Investment(name=mid_bus.name, device_idtag=mid_bus.idtag, group=inv_group))
+            self.circuit.add_investment(Investment(name=br1.name, device_idtag=br1.idtag, group=inv_group))
+            self.circuit.add_investment(Investment(name=br2.name, device_idtag=br2.idtag, group=inv_group))
+
+            # add to the schematic the new 2 lines and the bus
+            middle_bus_graphics = self.add_api_bus(bus=mid_bus,
+                                                   injections_by_tpe=dict(),
+                                                   x0=middle_bus_x,
+                                                   y0=middle_bus_y)
+            br1_graphics = self.add_api_line(branch=br1,
+                                             bus_f_graphic0=bus_f_graphic_obj,
+                                             bus_t_graphic0=middle_bus_graphics)
+            br2_graphics = self.add_api_line(branch=br2,
+                                             bus_f_graphic0=middle_bus_graphics,
+                                             bus_t_graphic0=bus_t_graphic_obj)
+
+            self.add_to_scene(middle_bus_graphics)
+            self.add_to_scene(br1_graphics)
+            self.add_to_scene(br2_graphics)
+
+            # redraw
+            bus_f_graphic_obj.arrange_children()
+            bus_t_graphic_obj.arrange_children()
+            middle_bus_graphics.arrange_children()
+        else:
+            error_msg("Incorrect position", 'Line split')
+
     def split_line(self, line_graphics: LineGraphicItem):
         """
         Split line
         :return:
         """
         dlg = InputNumberDialogue(min_value=1.0,
                                   max_value=99.0,
@@ -3627,139 +3763,30 @@
                                        "line as a percentage of the total length",
                                   suffix=' %',
                                   decimals=2,
                                   default_value=50.0)
         if dlg.exec_():
 
             if dlg.is_accepted:
-
                 position = dlg.value / 100.0
 
-                if 0.0 < position < 1.0:
-
-                    # Each of the Branches will have the proportional impedance
-                    # Bus_from           Middle_bus            Bus_To
-                    # o----------------------o--------------------o
-                    #   >-------- x -------->|
-                    #   (x: distance measured in per unit (0~1)
-                    line = line_graphics.api_object
-
-                    mid_bus = Bus(name=line.name + ' split',
-                                  vnom=line.bus_from.Vnom,
-                                  vmin=line.bus_from.Vmin,
-                                  vmax=line.bus_from.Vmax)
-
-                    bus_f_graphics_data = self.diagram.query_point(line.bus_from)
-                    bus_t_graphics_data = self.diagram.query_point(line.bus_to)
-                    bus_f_graphic_obj = self.graphics_manager.query(line.bus_from)
-                    bus_t_graphic_obj = self.graphics_manager.query(line.bus_to)
-
-                    if bus_f_graphics_data is None:
-                        error_msg(f"{line.bus_from} was not found in the diagram")
-                        return None
-                    if bus_t_graphics_data is None:
-                        error_msg(f"{line.bus_to} was not found in the diagram")
-                        return None
-                    if bus_f_graphic_obj is None:
-                        error_msg(f"{line.bus_from} was not found in the graphics manager")
-                        return None
-                    if bus_t_graphic_obj is None:
-                        error_msg(f"{line.bus_to} was not found in the graphics manager")
-                        return None
-
-                    # C(x, y) = (x1 + t * (x2 - x1), y1 + t * (y2 - y1))
-                    middle_bus_x = bus_f_graphics_data.x + (bus_t_graphics_data.x - bus_f_graphics_data.x) * position
-                    middle_bus_y = bus_f_graphics_data.y + (bus_t_graphics_data.y - bus_f_graphics_data.y) * position
-
-                    # create first split
-                    br1 = Line(name=line.name + ' split 1',
-                               bus_from=line.bus_from,
-                               bus_to=mid_bus,
-                               r=line.R * position,
-                               x=line.X * position,
-                               b=line.B * position,
-                               r0=line.R0 * position,
-                               x0=line.X0 * position,
-                               b0=line.B0 * position,
-                               r2=line.R2 * position,
-                               x2=line.X2 * position,
-                               b2=line.B2 * position,
-                               length=line.length * position,
-                               rate=line.rate,
-                               contingency_factor=line.contingency_factor,
-                               protection_rating_factor=line.protection_rating_factor)
-
-                    position_c = 1.0 - position
-                    br2 = Line(name=line.name + ' split 2',
-                               bus_from=mid_bus,
-                               bus_to=line.bus_to,
-                               r=line.R * position_c,
-                               x=line.X * position_c,
-                               b=line.B * position_c,
-                               r0=line.R0 * position_c,
-                               x0=line.X0 * position_c,
-                               b0=line.B0 * position_c,
-                               r2=line.R2 * position_c,
-                               x2=line.X2 * position_c,
-                               b2=line.B2 * position_c,
-                               length=line.length * position_c,
-                               rate=line.rate,
-                               contingency_factor=line.contingency_factor,
-                               protection_rating_factor=line.protection_rating_factor)
-
-                    # deactivate the original line
-                    line_graphics.api_object.active = False
-                    line_graphics.api_object.active_prof.fill(False)
-                    line_graphics.set_enable(False)
-
-                    # add to gridcal the new 2 lines and the bus
-                    self.circuit.add_bus(mid_bus)
-                    self.circuit.add_line(br1)
-                    self.circuit.add_line(br2)
-
-                    # add new stuff as new investment
-                    inv_group = InvestmentsGroup(name=line.name + ' split', category='Line split')
-                    self.circuit.add_investments_group(inv_group)
-                    self.circuit.add_investment(
-                        Investment(name=mid_bus.name, device_idtag=mid_bus.idtag, group=inv_group))
-                    self.circuit.add_investment(Investment(name=br1.name, device_idtag=br1.idtag, group=inv_group))
-                    self.circuit.add_investment(Investment(name=br2.name, device_idtag=br2.idtag, group=inv_group))
-
-                    # add to the schematic the new 2 lines and the bus
-                    middle_bus_graphics = self.add_api_bus(bus=mid_bus,
-                                                           injections_by_tpe=dict(),
-                                                           x0=middle_bus_x,
-                                                           y0=middle_bus_y)
-                    br1_graphics = self.add_api_line(branch=br1,
-                                                     bus_f_graphic0=bus_f_graphic_obj,
-                                                     bus_t_graphic0=middle_bus_graphics)
-                    br2_graphics = self.add_api_line(branch=br2,
-                                                     bus_f_graphic0=middle_bus_graphics,
-                                                     bus_t_graphic0=bus_t_graphic_obj)
-
-                    self.add_to_scene(middle_bus_graphics)
-                    self.add_to_scene(br1_graphics)
-                    self.add_to_scene(br2_graphics)
-
-                    # redraw
-                    bus_f_graphic_obj.arrange_children()
-                    bus_t_graphic_obj.arrange_children()
-                    middle_bus_graphics.arrange_children()
-                else:
-                    error_msg("Incorrect position", 'Line split')
+                self.split_line_now(line_graphics=line_graphics,
+                                    position=position,
+                                    extra_km=0.0)
 
     def split_line_in_out(self, line_graphics: LineGraphicItem):
         """
         Split line and create extra substations so that an in/out is formed
         :param line_graphics: Original LineGraphicItem to split
         """
+        title = "Split line with input/output"
         dlg = InputNumberDialogue(min_value=1.0,
                                   max_value=99.0,
                                   is_int=False,
-                                  title="Split line with input/output",
+                                  title=title,
                                   text="Enter the distance from the beginning of the \n"
                                        "line as a percentage of the total length",
                                   suffix=' %',
                                   decimals=2,
                                   default_value=50.0)
         if dlg.exec_():
 
@@ -3768,219 +3795,247 @@
                 position = dlg.value / 100.0
 
                 if 0.0 < position < 1.0:
 
                     dlg2 = InputNumberDialogue(min_value=0.01,
                                                max_value=99999999.0,
                                                is_int=False,
-                                               title="Split line with input/output",
-                                               text="Distance from the original line",
+                                               title=title,
+                                               text="Distance from the splitting point",
                                                suffix=' km',
                                                decimals=2,
                                                default_value=1.0)
 
                     if dlg2.exec_():
 
                         if dlg2.is_accepted:
 
-                            # Each of the Branches will have the proportional impedance
-                            # Bus_from           Middle_bus            Bus_To
-                            # o----------------------o--------------------o
-                            #   >-------- x -------->|
-                            #   (x: distance measured in per unit (0~1)
-                            line = line_graphics.api_object
-                            bus_f_graphics_data = self.diagram.query_point(line.bus_from)
-                            bus_t_graphics_data = self.diagram.query_point(line.bus_to)
-                            bus_f_graphic_obj = self.graphics_manager.query(line.bus_from)
-                            bus_t_graphic_obj = self.graphics_manager.query(line.bus_to)
-
-                            if bus_f_graphics_data is None:
-                                error_msg(f"{line.bus_from} was not found in the diagram")
-                                return None
-                            if bus_t_graphics_data is None:
-                                error_msg(f"{line.bus_to} was not found in the diagram")
-                                return None
-                            if bus_f_graphic_obj is None:
-                                error_msg(f"{line.bus_from} was not found in the graphics manager")
-                                return None
-                            if bus_t_graphic_obj is None:
-                                error_msg(f"{line.bus_to} was not found in the graphics manager")
-                                return None
-
-                            # C(x, y) = (x1 + t * (x2 - x1), y1 + t * (y2 - y1))
-                            mid_x = bus_f_graphics_data.x + (bus_t_graphics_data.x - bus_f_graphics_data.x) * position
-                            mid_y = bus_f_graphics_data.y + (bus_t_graphics_data.y - bus_f_graphics_data.y) * position
-
-                            B1 = Bus(name=line.name + ' split bus 1',
-                                     vnom=line.bus_from.Vnom,
-                                     vmin=line.bus_from.Vmin,
-                                     vmax=line.bus_from.Vmax)
-
-                            B2 = Bus(name=line.name + ' split bus 2',
-                                     vnom=line.bus_from.Vnom,
-                                     vmin=line.bus_from.Vmin,
-                                     vmax=line.bus_from.Vmax)
-
-                            B3 = Bus(name=line.name + ' new bus',
-                                     vnom=line.bus_from.Vnom,
-                                     vmin=line.bus_from.Vmin,
-                                     vmax=line.bus_from.Vmax)
-
-                            # create first split
-                            br1 = Line(name=line.name + ' split 1',
-                                       bus_from=line.bus_from,
-                                       bus_to=B1,
-                                       r=line.R * position,
-                                       x=line.X * position,
-                                       b=line.B * position,
-                                       r0=line.R0 * position,
-                                       x0=line.X0 * position,
-                                       b0=line.B0 * position,
-                                       r2=line.R2 * position,
-                                       x2=line.X2 * position,
-                                       b2=line.B2 * position,
-                                       length=line.length * position,
-                                       rate=line.rate,
-                                       contingency_factor=line.contingency_factor,
-                                       protection_rating_factor=line.protection_rating_factor)
-
-                            position_c = 1.0 - position
-                            br2 = Line(name=line.name + ' split 2',
-                                       bus_from=B2,
-                                       bus_to=line.bus_to,
-                                       r=line.R * position_c,
-                                       x=line.X * position_c,
-                                       b=line.B * position_c,
-                                       r0=line.R0 * position_c,
-                                       x0=line.X0 * position_c,
-                                       b0=line.B0 * position_c,
-                                       r2=line.R2 * position_c,
-                                       x2=line.X2 * position_c,
-                                       b2=line.B2 * position_c,
-                                       length=line.length * position_c,
-                                       rate=line.rate,
-                                       contingency_factor=line.contingency_factor,
-                                       protection_rating_factor=line.protection_rating_factor)
-
-                            # kilometers of the in/out appart from the original line
-                            km_io = dlg2.value
-                            proportion_io = km_io / line.length
-
-                            br3 = Line(name=line.name + ' in',
-                                       bus_from=B1,
-                                       bus_to=B3,
-                                       r=line.R * proportion_io,
-                                       x=line.X * proportion_io,
-                                       b=line.B * proportion_io,
-                                       r0=line.R0 * proportion_io,
-                                       x0=line.X0 * proportion_io,
-                                       b0=line.B0 * proportion_io,
-                                       r2=line.R2 * proportion_io,
-                                       x2=line.X2 * proportion_io,
-                                       b2=line.B2 * proportion_io,
-                                       length=line.length * proportion_io,
-                                       rate=line.rate,
-                                       contingency_factor=line.contingency_factor,
-                                       protection_rating_factor=line.protection_rating_factor)
-
-                            br4 = Line(name=line.name + ' out',
-                                       bus_from=B3,
-                                       bus_to=B2,
-                                       r=line.R * proportion_io,
-                                       x=line.X * proportion_io,
-                                       b=line.B * proportion_io,
-                                       r0=line.R0 * proportion_io,
-                                       x0=line.X0 * proportion_io,
-                                       b0=line.B0 * proportion_io,
-                                       r2=line.R2 * proportion_io,
-                                       x2=line.X2 * proportion_io,
-                                       b2=line.B2 * proportion_io,
-                                       length=line.length * proportion_io,
-                                       rate=line.rate,
-                                       contingency_factor=line.contingency_factor,
-                                       protection_rating_factor=line.protection_rating_factor)
-
-                            # deactivate the original line
-                            line_graphics.api_object.active = False
-                            line_graphics.api_object.active_prof.fill(False)
-                            line_graphics.set_enable(False)
-
-                            # add to gridcal the new 2 lines and the bus
-                            self.circuit.add_bus(B1)
-                            self.circuit.add_bus(B2)
-                            self.circuit.add_bus(B3)
-                            self.circuit.add_line(br1)
-                            self.circuit.add_line(br2)
-                            self.circuit.add_line(br3)
-                            self.circuit.add_line(br4)
-
-                            # add new stuff as new investment
-                            inv_group = InvestmentsGroup(name=line.name + ' in/out', category='Line in/out')
-                            self.circuit.add_investments_group(inv_group)
-                            self.circuit.add_investment(
-                                Investment(name=B1.name, device_idtag=B1.idtag, group=inv_group))
-                            self.circuit.add_investment(
-                                Investment(name=B2.name, device_idtag=B2.idtag, group=inv_group))
-                            self.circuit.add_investment(
-                                Investment(name=B3.name, device_idtag=B3.idtag, group=inv_group))
-                            self.circuit.add_investment(
-                                Investment(name=br1.name, device_idtag=br1.idtag, group=inv_group))
-                            self.circuit.add_investment(
-                                Investment(name=br2.name, device_idtag=br2.idtag, group=inv_group))
-                            self.circuit.add_investment(
-                                Investment(name=br3.name, device_idtag=br3.idtag, group=inv_group))
-                            self.circuit.add_investment(
-                                Investment(name=br4.name, device_idtag=br4.idtag, group=inv_group))
-
-                            # add to the schematic the new 2 lines and the bus
-                            B1_graphics = self.add_api_bus(bus=B1,
-                                                           injections_by_tpe=dict(),
-                                                           x0=mid_x,
-                                                           y0=mid_y)
-
-                            B2_graphics = self.add_api_bus(bus=B2,
-                                                           injections_by_tpe=dict(),
-                                                           x0=mid_x,
-                                                           y0=mid_y)
-
-                            B3_graphics = self.add_api_bus(bus=B3,
-                                                           injections_by_tpe=dict(),
-                                                           x0=mid_x,
-                                                           y0=mid_y)
-
-                            br1_graphics = self.add_api_line(branch=br1,
-                                                             bus_f_graphic0=bus_f_graphic_obj,
-                                                             bus_t_graphic0=B1_graphics)
-
-                            br2_graphics = self.add_api_line(branch=br2,
-                                                             bus_f_graphic0=B2_graphics,
-                                                             bus_t_graphic0=bus_t_graphic_obj)
-
-                            br3_graphics = self.add_api_line(branch=br3,
-                                                             bus_f_graphic0=B1_graphics,
-                                                             bus_t_graphic0=B3_graphics)
-
-                            br4_graphics = self.add_api_line(branch=br4,
-                                                             bus_f_graphic0=B3_graphics,
-                                                             bus_t_graphic0=B2_graphics)
-
-                            self.add_to_scene(B1_graphics)
-                            self.add_to_scene(B2_graphics)
-                            self.add_to_scene(B3_graphics)
-                            self.add_to_scene(br1_graphics)
-                            self.add_to_scene(br2_graphics)
-                            self.add_to_scene(br3_graphics)
-                            self.add_to_scene(br4_graphics)
-
-                            # redraw
-                            bus_f_graphic_obj.arrange_children()
-                            bus_t_graphic_obj.arrange_children()
-                            B1_graphics.arrange_children()
-                            B2_graphics.arrange_children()
-                            B3_graphics.arrange_children()
+                            create_extra_nodes = yes_no_question(text="Add extra buses?", title=title)
+
+                            if create_extra_nodes:
+                                # Each of the Branches will have the proportional impedance
+                                # Bus_from           Middle_bus            Bus_To
+                                # o----------------------o--------------------o
+                                #   >-------- x -------->|
+                                #   (x: distance measured in per unit (0~1)
+                                line = line_graphics.api_object
+                                bus_f_graphics_data = self.diagram.query_point(line.bus_from)
+                                bus_t_graphics_data = self.diagram.query_point(line.bus_to)
+                                bus_f_graphic_obj = self.graphics_manager.query(line.bus_from)
+                                bus_t_graphic_obj = self.graphics_manager.query(line.bus_to)
+
+                                if bus_f_graphics_data is None:
+                                    error_msg(f"{line.bus_from} was not found in the diagram")
+                                    return None
+                                if bus_t_graphics_data is None:
+                                    error_msg(f"{line.bus_to} was not found in the diagram")
+                                    return None
+                                if bus_f_graphic_obj is None:
+                                    error_msg(f"{line.bus_from} was not found in the graphics manager")
+                                    return None
+                                if bus_t_graphic_obj is None:
+                                    error_msg(f"{line.bus_to} was not found in the graphics manager")
+                                    return None
+
+                                # C(x, y) = (x1 + t * (x2 - x1), y1 + t * (y2 - y1))
+                                mid_x = bus_f_graphics_data.x + (
+                                            bus_t_graphics_data.x - bus_f_graphics_data.x) * position
+                                mid_y = bus_f_graphics_data.y + (
+                                            bus_t_graphics_data.y - bus_f_graphics_data.y) * position
+
+                                B1 = Bus(name=line.name + ' split bus 1',
+                                         vnom=line.bus_from.Vnom,
+                                         vmin=line.bus_from.Vmin,
+                                         vmax=line.bus_from.Vmax,
+                                         area=line.bus_from.area,
+                                         zone=line.bus_from.zone,
+                                         country=line.bus_from.country)
+
+                                B2 = Bus(name=line.name + ' split bus 2',
+                                         vnom=line.bus_from.Vnom,
+                                         vmin=line.bus_from.Vmin,
+                                         vmax=line.bus_from.Vmax,
+                                         area=line.bus_from.area,
+                                         zone=line.bus_from.zone,
+                                         country=line.bus_from.country)
+
+                                mid_sub = Substation(name=line.name + ' new bus',
+                                                     area=line.bus_from.area,
+                                                     zone=line.bus_from.zone,
+                                                     country=line.bus_from.country)
+                                mid_vl = VoltageLevel(name=line.name + ' new bus',
+                                                      substation=mid_sub)
+                                B3 = Bus(name=line.name + ' new bus',
+                                         vnom=line.bus_from.Vnom,
+                                         vmin=line.bus_from.Vmin,
+                                         vmax=line.bus_from.Vmax,
+                                         voltage_level=mid_vl,
+                                         substation=mid_sub,
+                                         area=line.bus_from.area,
+                                         zone=line.bus_from.zone,
+                                         country=line.bus_from.country)
+
+                                # create first split
+                                br1 = Line(name=line.name + ' split 1',
+                                           bus_from=line.bus_from,
+                                           bus_to=B1,
+                                           r=line.R * position,
+                                           x=line.X * position,
+                                           b=line.B * position,
+                                           r0=line.R0 * position,
+                                           x0=line.X0 * position,
+                                           b0=line.B0 * position,
+                                           r2=line.R2 * position,
+                                           x2=line.X2 * position,
+                                           b2=line.B2 * position,
+                                           length=line.length * position,
+                                           rate=line.rate,
+                                           contingency_factor=line.contingency_factor,
+                                           protection_rating_factor=line.protection_rating_factor)
+
+                                position_c = 1.0 - position
+                                br2 = Line(name=line.name + ' split 2',
+                                           bus_from=B2,
+                                           bus_to=line.bus_to,
+                                           r=line.R * position_c,
+                                           x=line.X * position_c,
+                                           b=line.B * position_c,
+                                           r0=line.R0 * position_c,
+                                           x0=line.X0 * position_c,
+                                           b0=line.B0 * position_c,
+                                           r2=line.R2 * position_c,
+                                           x2=line.X2 * position_c,
+                                           b2=line.B2 * position_c,
+                                           length=line.length * position_c,
+                                           rate=line.rate,
+                                           contingency_factor=line.contingency_factor,
+                                           protection_rating_factor=line.protection_rating_factor)
+
+                                # kilometers of the in/out appart from the original line
+                                km_io = dlg2.value
+                                proportion_io = km_io / line.length
+
+                                br3 = Line(name=line.name + ' in',
+                                           bus_from=B1,
+                                           bus_to=B3,
+                                           r=line.R * proportion_io,
+                                           x=line.X * proportion_io,
+                                           b=line.B * proportion_io,
+                                           r0=line.R0 * proportion_io,
+                                           x0=line.X0 * proportion_io,
+                                           b0=line.B0 * proportion_io,
+                                           r2=line.R2 * proportion_io,
+                                           x2=line.X2 * proportion_io,
+                                           b2=line.B2 * proportion_io,
+                                           length=line.length * proportion_io,
+                                           rate=line.rate,
+                                           contingency_factor=line.contingency_factor,
+                                           protection_rating_factor=line.protection_rating_factor)
+
+                                br4 = Line(name=line.name + ' out',
+                                           bus_from=B3,
+                                           bus_to=B2,
+                                           r=line.R * proportion_io,
+                                           x=line.X * proportion_io,
+                                           b=line.B * proportion_io,
+                                           r0=line.R0 * proportion_io,
+                                           x0=line.X0 * proportion_io,
+                                           b0=line.B0 * proportion_io,
+                                           r2=line.R2 * proportion_io,
+                                           x2=line.X2 * proportion_io,
+                                           b2=line.B2 * proportion_io,
+                                           length=line.length * proportion_io,
+                                           rate=line.rate,
+                                           contingency_factor=line.contingency_factor,
+                                           protection_rating_factor=line.protection_rating_factor)
+
+                                # deactivate the original line
+                                line_graphics.api_object.active = False
+                                line_graphics.api_object.active_prof.fill(False)
+                                line_graphics.set_enable(False)
+
+                                # add to gridcal the new 2 lines and the bus
+                                self.circuit.add_bus(B1)
+                                self.circuit.add_bus(B2)
+                                self.circuit.add_bus(B3)
+                                self.circuit.add_line(br1)
+                                self.circuit.add_line(br2)
+                                self.circuit.add_line(br3)
+                                self.circuit.add_line(br4)
+
+                                # add new stuff as new investment
+                                inv_group = InvestmentsGroup(name=line.name + ' in/out', category='Line in/out')
+                                self.circuit.add_investments_group(inv_group)
+                                self.circuit.add_investment(
+                                    Investment(name=B1.name, device_idtag=B1.idtag, group=inv_group))
+                                self.circuit.add_investment(
+                                    Investment(name=B2.name, device_idtag=B2.idtag, group=inv_group))
+                                self.circuit.add_investment(
+                                    Investment(name=B3.name, device_idtag=B3.idtag, group=inv_group))
+                                self.circuit.add_investment(
+                                    Investment(name=br1.name, device_idtag=br1.idtag, group=inv_group))
+                                self.circuit.add_investment(
+                                    Investment(name=br2.name, device_idtag=br2.idtag, group=inv_group))
+                                self.circuit.add_investment(
+                                    Investment(name=br3.name, device_idtag=br3.idtag, group=inv_group))
+                                self.circuit.add_investment(
+                                    Investment(name=br4.name, device_idtag=br4.idtag, group=inv_group))
+
+                                # add to the schematic the new 2 lines and the bus
+                                B1_graphics = self.add_api_bus(bus=B1,
+                                                               injections_by_tpe=dict(),
+                                                               x0=mid_x,
+                                                               y0=mid_y)
+
+                                B2_graphics = self.add_api_bus(bus=B2,
+                                                               injections_by_tpe=dict(),
+                                                               x0=mid_x,
+                                                               y0=mid_y)
+
+                                B3_graphics = self.add_api_bus(bus=B3,
+                                                               injections_by_tpe=dict(),
+                                                               x0=mid_x,
+                                                               y0=mid_y)
+
+                                br1_graphics = self.add_api_line(branch=br1,
+                                                                 bus_f_graphic0=bus_f_graphic_obj,
+                                                                 bus_t_graphic0=B1_graphics)
+
+                                br2_graphics = self.add_api_line(branch=br2,
+                                                                 bus_f_graphic0=B2_graphics,
+                                                                 bus_t_graphic0=bus_t_graphic_obj)
+
+                                br3_graphics = self.add_api_line(branch=br3,
+                                                                 bus_f_graphic0=B1_graphics,
+                                                                 bus_t_graphic0=B3_graphics)
+
+                                br4_graphics = self.add_api_line(branch=br4,
+                                                                 bus_f_graphic0=B3_graphics,
+                                                                 bus_t_graphic0=B2_graphics)
+
+                                self.add_to_scene(B1_graphics)
+                                self.add_to_scene(B2_graphics)
+                                self.add_to_scene(B3_graphics)
+                                self.add_to_scene(br1_graphics)
+                                self.add_to_scene(br2_graphics)
+                                self.add_to_scene(br3_graphics)
+                                self.add_to_scene(br4_graphics)
+
+                                # redraw
+                                bus_f_graphic_obj.arrange_children()
+                                bus_t_graphic_obj.arrange_children()
+                                B1_graphics.arrange_children()
+                                B2_graphics.arrange_children()
+                                B3_graphics.arrange_children()
+                            else:
+                                self.split_line_now(line_graphics=line_graphics,
+                                                    position=position,
+                                                    extra_km=dlg2.value)
+                        else:
+                            pass
                 else:
                     error_msg("Incorrect position", 'Line split')
 
     def change_bus(self, line_graphics: LineGraphicTemplateItem):
         """
         change the from or to bus of the nbranch with another selected bus
         :param line_graphics
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/map_widget.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,16 +338,16 @@
         self.devYFact = 33.0
         initial_zoom_factor = 0.47
         self.devXFact  = 48.3
         self.devYFact = 61.9
         self.schema_zoom = 1
         self.view.scale(initial_zoom_factor, initial_zoom_factor)
         self.remapSchema()
+        self.schema_Manager = schemaManager(self.scene, self.devXFact, self.devYFact)
         self.selTempDistance = 20
-        self.schema_Manager = schemaManager(self.scene)
 
     def convertToQMouseEvent(self, sceneMouseEvent):
         # Get relevant information from QGraphicsSceneMouseEvent
         pos = sceneMouseEvent.screenPos()
         button = sceneMouseEvent.button()
         buttons = sceneMouseEvent.buttons()
         modifiers = sceneMouseEvent.modifiers()
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/node_widget.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/node_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/map_events.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from typing import Union, List
 import numpy as np
 from PySide6.QtWidgets import QWidget
 from collections.abc import Callable
 
+from GridCal.Gui.Diagrams.MapWidget.Schema.Nodes import NodeGraphicItem
 from GridCalEngine.Devices.Diagrams.map_location import MapLocation
 from GridCalEngine.Devices.Substation import Bus
 from GridCalEngine.Devices.Branches.line import Line
 from GridCalEngine.Devices.Branches.dc_line import DcLine
 from GridCalEngine.Devices.Branches.hvdc_line import HvdcLine
 from GridCalEngine.Devices.Diagrams.map_diagram import MapDiagram
 from GridCalEngine.Devices.types import BRANCH_TYPES
@@ -33,15 +34,15 @@
 from GridCalEngine.Devices.types import ALL_DEV_TYPES
 
 from GridCal.Gui.Diagrams.MapWidget.map_widget import MapWidget, PolylineData, Place
 import GridCal.Gui.Visualization.visualization as viz
 import GridCal.Gui.Visualization.palettes as palettes
 from GridCal.Gui.Diagrams.graphics_manager import GraphicsManager
 from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
-
+from GridCalEngine.enumerations import DeviceType
 
 class GridMapWidget(MapWidget):
 
     def __init__(self,
                  parent: Union[QWidget, None],
                  tile_src: Tiles,
                  start_level: int,
@@ -62,14 +63,17 @@
         # diagram to store the objects locations
         self.diagram: MapDiagram = MapDiagram(name=name,
                                               tile_source=tile_src.TilesetName,
                                               start_level=start_level,
                                               longitude=longitude,
                                               latitude=latitude) if diagram is None else diagram
 
+        if self.diagram:
+            self.draw()
+
         # add empty polylines layer
         self.polyline_layer_id = self.AddPolylineLayer(data=[],
                                                        map_rel=True,
                                                        visible=True,
                                                        show_levels=list(range(20)),
                                                        selectable=True,
                                                        # levels at which to show the polylines
@@ -130,14 +134,36 @@
         :param latitude:
         :return:
         """
         # print('Map lat:', latitude, 'lon:', longitude)
         self.diagram.latitude = latitude
         self.diagram.longitude = longitude
 
+
+    def draw(self) -> None:
+        for category, points_group in self.diagram.data.items():
+            if category == DeviceType.SubstationDevice.value:
+                for idtag, location in points_group.locations.items():
+                    self.schema_Manager.CreateSubstation(location.latitude, location.longitude)
+            elif category == DeviceType.LineDevice.value:
+
+                for idtag, location in points_group.locations.items():
+                    self.schema_Manager.CreateLine()
+                    line: Line = location.api_object
+                    for elm in line.locations.data:
+                        self.schema_Manager.CurrentLine.CreateNode(elm.long, -elm.lat)
+                        nodSiz = len(self.schema_Manager.CurrentLine.Nodes)
+                        if(nodSiz > 1):
+                            i1 = nodSiz - 1
+                            i2 = nodSiz - 2
+                            self.schema_Manager.CurrentLine.CreateConnector(i1, i2)
+            elif category == DeviceType.VoltageLevelDevice.value:
+                for idtag, location in points_group.locations.items():
+                    self.schema_Manager.CreateSubstation(location.latitude, location.longitude)
+
     def colour_results(self,
                        buses: List[Bus],
                        branches: List[BRANCH_TYPES],
                        hvdc_lines: List[HvdcLine],
                        Sbus: CxVec,
                        bus_active: IntVec,
                        Sf: CxVec,
@@ -379,14 +405,26 @@
         if prog_func is not None:
             prog_func((i + 1) / nn * 100.0)
 
         diagram.set_point(device=substation, location=MapLocation())
 
     # --------------------------------------------------------------------------------------------------------------
     if text_func is not None:
+        text_func('Creating schematic buses')
+
+    nn = len(voltage_levels)
+    for i, voltageLevel in enumerate(voltage_levels):
+
+        if prog_func is not None:
+            prog_func((i + 1) / nn * 100.0)
+
+        diagram.set_point(device=voltageLevel, location=MapLocation())
+
+    # --------------------------------------------------------------------------------------------------------------
+    if text_func is not None:
         text_func('Creating schematic fluid nodes devices')
 
     nn = len(fluid_nodes)
     for i, elm in enumerate(fluid_nodes):
 
         if prog_func is not None:
             prog_func((i + 1) / nn * 100.0)
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from PySide6.QtGui import QPen, QCursor, QIcon, QPixmap, QBrush, QColor
 from PySide6.QtWidgets import QMenu, QGraphicsSceneMouseEvent
 import random
 
 from GridCalEngine.IO.matpower.matpower_branch_definitions import QT
 
 
-class NodeGraphicItem(QtWidgets.QGraphicsEllipseItem):
+class SubstationGraphicItem(QtWidgets.QGraphicsEllipseItem):
     """
       Represents a block in the diagram
       Has an x and y and width and height
       width and height can only be adjusted with a tip in the lower right corner.
 
       - in and output ports
       - parameters
@@ -53,16 +53,20 @@
         self.setFlag(QtWidgets.QGraphicsItem.ItemIsMovable)  # Allow moving the node
         self.setFlag(QtWidgets.QGraphicsItem.ItemIsSelectable)  # Allow selecting the node
         parent.Scene.addItem(self)
 
         # Create a pen with reduced line width
         self.change_pen_width(0.5)
 
-        self.colorInner = QColor(100, random.randint(0, 255), random.randint(0, 255), random.randint(0, 255))
-        self.colorBorder = QColor(100, random.randint(0, 255), random.randint(0, 255), random.randint(0, 255))
+        # self.colorInner = QColor(100, random.randint(0, 255), random.randint(0, 255), random.randint(0, 255))
+        # self.colorBorder = QColor(100, random.randint(0, 255), random.randint(0, 255), random.randint(0, 255))
+
+        self.colorInner = QColor(255, 100, 100, 100)
+        self.colorBorder = QColor(255, 100, 100, 100)
+
         # Assign color to the node
         self.setDefaultColor()
 
     def updatePosition(self):
         real_position = self.pos()
         center_point = self.getPos()
         self.x = center_point.x() + real_position.x()
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py` & `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/AboutDialogue/about_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/AboutDialogue/about_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/AboutDialogue/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/AboutDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/AboutDialogue/gui.py` & `GridCal-5.1.5/GridCal/Gui/AboutDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ProfilesInput/excel_dialog.py` & `GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_dialog.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py` & `GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ProfilesInput/models_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/ProfilesInput/models_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ProfilesInput/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/ProfilesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ProfilesInput/profile_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/ProfilesInput/profile_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py` & `GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/ProfilesInput/excel_sheet_selection.py` & `GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_sheet_selection.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Analysis/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/Analysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Analysis/AnalysisDialogue.py` & `GridCal-5.1.5/GridCal/Gui/Analysis/AnalysisDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Analysis/gui.py` & `GridCal-5.1.5/GridCal/Gui/Analysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Analysis/object_plot_analysis.py` & `GridCal-5.1.5/GridCal/Gui/Analysis/object_plot_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/CascadingSteps/cascading_steps.py` & `GridCal-5.1.5/GridCal/Gui/CascadingSteps/cascading_steps.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/CascadingSteps/gui.py` & `GridCal-5.1.5/GridCal/Gui/CascadingSteps/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/ConsoleLogController.py` & `GridCal-5.1.5/GridCal/Gui/Main/ConsoleLogController.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/GridCalMain.py` & `GridCal-5.1.5/GridCal/Gui/Main/GridCalMain.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/MainWindow.py` & `GridCal-5.1.5/GridCal/Gui/Main/MainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'MainWindow.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.1
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
     QCursor, QFont, QFontDatabase, QGradient,
     QIcon, QImage, QKeySequence, QLinearGradient,
     QPainter, QPalette, QPixmap, QRadialGradient,
     QTransform)
 from PySide6.QtWidgets import (QAbstractItemView, QApplication, QCheckBox, QComboBox,
-    QDoubleSpinBox, QFrame, QGridLayout, QGroupBox,
-    QHBoxLayout, QHeaderView, QLabel, QLineEdit,
-    QListView, QMainWindow, QMenu, QMenuBar,
-    QPlainTextEdit, QProgressBar, QPushButton, QRadioButton,
-    QSizePolicy, QSlider, QSpacerItem, QSpinBox,
-    QSplitter, QTabWidget, QTableView, QTextEdit,
-    QToolBar, QTreeView, QVBoxLayout, QWidget)
+    QDateTimeEdit, QDoubleSpinBox, QFrame, QGridLayout,
+    QGroupBox, QHBoxLayout, QHeaderView, QLabel,
+    QLineEdit, QListView, QMainWindow, QMenu,
+    QMenuBar, QPlainTextEdit, QProgressBar, QPushButton,
+    QRadioButton, QSizePolicy, QSlider, QSpacerItem,
+    QSpinBox, QSplitter, QTabWidget, QTableView,
+    QTextEdit, QToolBar, QTreeView, QVBoxLayout,
+    QWidget)
 from .icons_rc import *
 
 class Ui_mainWindow(object):
     def setupUi(self, mainWindow):
         if not mainWindow.objectName():
             mainWindow.setObjectName(u"mainWindow")
         mainWindow.resize(1292, 746)
@@ -435,14 +436,19 @@
         icon64.addFile(u":/Icons/icons/uncheck_all.svg", QSize(), QIcon.Normal, QIcon.Off)
         self.actionDisable_all_results_tags.setIcon(icon64)
         self.actionEnable_all_results_tags = QAction(mainWindow)
         self.actionEnable_all_results_tags.setObjectName(u"actionEnable_all_results_tags")
         icon65 = QIcon()
         icon65.addFile(u":/Icons/icons/check_all.svg", QSize(), QIcon.Normal, QIcon.Off)
         self.actionEnable_all_results_tags.setIcon(icon65)
+        self.actionDetect_substations = QAction(mainWindow)
+        self.actionDetect_substations.setObjectName(u"actionDetect_substations")
+        icon66 = QIcon()
+        icon66.addFile(u":/Icons/icons/chip.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.actionDetect_substations.setIcon(icon66)
         self.centralwidget = QWidget(mainWindow)
         self.centralwidget.setObjectName(u"centralwidget")
         self.gridLayout_3 = QGridLayout(self.centralwidget)
         self.gridLayout_3.setObjectName(u"gridLayout_3")
         self.gridLayout_3.setContentsMargins(0, 0, 0, 0)
         self.tabWidget = QTabWidget(self.centralwidget)
         self.tabWidget.setObjectName(u"tabWidget")
@@ -471,15 +477,15 @@
         self.verticalLayout_5.setObjectName(u"verticalLayout_5")
         self.verticalLayout_5.setContentsMargins(0, 0, 0, 0)
         self.diagram_selection_splitter = QSplitter(self.frame_6)
         self.diagram_selection_splitter.setObjectName(u"diagram_selection_splitter")
         self.diagram_selection_splitter.setOrientation(Qt.Horizontal)
         self.schematic_frame = QFrame(self.diagram_selection_splitter)
         self.schematic_frame.setObjectName(u"schematic_frame")
-        sizePolicy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+        sizePolicy = QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.schematic_frame.sizePolicy().hasHeightForWidth())
         self.schematic_frame.setSizePolicy(sizePolicy)
         self.schematic_frame.setFrameShape(QFrame.NoFrame)
         self.schematic_frame.setFrameShadow(QFrame.Raised)
         self.verticalLayout_3 = QVBoxLayout(self.schematic_frame)
@@ -521,17 +527,17 @@
         self.available_results_to_color_comboBox.setMinimumSize(QSize(164, 0))
 
         self.horizontalLayout_30.addWidget(self.available_results_to_color_comboBox)
 
         self.colour_results_pushButton = QPushButton(self.grid_colouring_frame)
         self.colour_results_pushButton.setObjectName(u"colour_results_pushButton")
         self.colour_results_pushButton.setMaximumSize(QSize(32, 16777215))
-        icon66 = QIcon()
-        icon66.addFile(u":/Icons/icons/color_grid.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.colour_results_pushButton.setIcon(icon66)
+        icon67 = QIcon()
+        icon67.addFile(u":/Icons/icons/color_grid.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.colour_results_pushButton.setIcon(icon67)
 
         self.horizontalLayout_30.addWidget(self.colour_results_pushButton)
 
 
         self.verticalLayout_2.addWidget(self.grid_colouring_frame)
 
         self.schematic_step_label = QLabel(self.diagram_selection_frame)
@@ -610,23 +616,23 @@
 
         self.filter_pushButton = QPushButton(self.frame_54)
         self.filter_pushButton.setObjectName(u"filter_pushButton")
         self.filter_pushButton.setIcon(icon60)
 
         self.horizontalLayout_28.addWidget(self.filter_pushButton)
 
-        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_28.addItem(self.horizontalSpacer_2)
 
         self.structure_analysis_pushButton = QPushButton(self.frame_54)
         self.structure_analysis_pushButton.setObjectName(u"structure_analysis_pushButton")
-        icon67 = QIcon()
-        icon67.addFile(u":/Icons/icons/histogram.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.structure_analysis_pushButton.setIcon(icon67)
+        icon68 = QIcon()
+        icon68.addFile(u":/Icons/icons/histogram.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.structure_analysis_pushButton.setIcon(icon68)
 
         self.horizontalLayout_28.addWidget(self.structure_analysis_pushButton)
 
 
         self.verticalLayout_20.addWidget(self.frame_54)
 
         self.dataStructureTableView = QTableView(self.tab_15)
@@ -639,17 +645,17 @@
         self.frame_9.setFrameShape(QFrame.NoFrame)
         self.frame_9.setFrameShadow(QFrame.Raised)
         self.horizontalLayout_25 = QHBoxLayout(self.frame_9)
         self.horizontalLayout_25.setObjectName(u"horizontalLayout_25")
         self.horizontalLayout_25.setContentsMargins(0, 0, 0, 0)
         self.set_profile_state_button = QPushButton(self.frame_9)
         self.set_profile_state_button.setObjectName(u"set_profile_state_button")
-        icon68 = QIcon()
-        icon68.addFile(u":/Icons/icons/copy2left.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.set_profile_state_button.setIcon(icon68)
+        icon69 = QIcon()
+        icon69.addFile(u":/Icons/icons/copy2left.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.set_profile_state_button.setIcon(icon69)
 
         self.horizontalLayout_25.addWidget(self.set_profile_state_button)
 
         self.db_step_slider = QSlider(self.frame_9)
         self.db_step_slider.setObjectName(u"db_step_slider")
         self.db_step_slider.setOrientation(Qt.Horizontal)
 
@@ -659,31 +665,31 @@
         self.db_step_label.setObjectName(u"db_step_label")
         self.db_step_label.setMinimumSize(QSize(200, 0))
         self.db_step_label.setFont(font)
         self.db_step_label.setAlignment(Qt.AlignLeading|Qt.AlignLeft|Qt.AlignVCenter)
 
         self.horizontalLayout_25.addWidget(self.db_step_label)
 
-        self.horizontalSpacer_9 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_9 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_25.addItem(self.horizontalSpacer_9)
 
         self.add_object_pushButton = QPushButton(self.frame_9)
         self.add_object_pushButton.setObjectName(u"add_object_pushButton")
-        icon69 = QIcon()
-        icon69.addFile(u":/Icons/icons/plus.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.add_object_pushButton.setIcon(icon69)
+        icon70 = QIcon()
+        icon70.addFile(u":/Icons/icons/plus.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.add_object_pushButton.setIcon(icon70)
 
         self.horizontalLayout_25.addWidget(self.add_object_pushButton)
 
         self.delete_selected_objects_pushButton = QPushButton(self.frame_9)
         self.delete_selected_objects_pushButton.setObjectName(u"delete_selected_objects_pushButton")
-        icon70 = QIcon()
-        icon70.addFile(u":/Icons/icons/minus.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.delete_selected_objects_pushButton.setIcon(icon70)
+        icon71 = QIcon()
+        icon71.addFile(u":/Icons/icons/minus.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.delete_selected_objects_pushButton.setIcon(icon71)
 
         self.horizontalLayout_25.addWidget(self.delete_selected_objects_pushButton)
 
 
         self.verticalLayout_20.addWidget(self.frame_9)
 
         self.tabWidget_5.addTab(self.tab_15, icon47, "")
@@ -709,47 +715,47 @@
         self.new_profiles_structure_pushButton.setObjectName(u"new_profiles_structure_pushButton")
         self.new_profiles_structure_pushButton.setIcon(icon21)
 
         self.horizontalLayout.addWidget(self.new_profiles_structure_pushButton)
 
         self.delete_profiles_structure_pushButton = QPushButton(self.frame)
         self.delete_profiles_structure_pushButton.setObjectName(u"delete_profiles_structure_pushButton")
-        icon71 = QIcon()
-        icon71.addFile(u":/Icons/icons/new (delete).svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.delete_profiles_structure_pushButton.setIcon(icon71)
+        icon72 = QIcon()
+        icon72.addFile(u":/Icons/icons/new (delete).svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.delete_profiles_structure_pushButton.setIcon(icon72)
 
         self.horizontalLayout.addWidget(self.delete_profiles_structure_pushButton)
 
         self.edit_profiles_pushButton = QPushButton(self.frame)
         self.edit_profiles_pushButton.setObjectName(u"edit_profiles_pushButton")
-        icon72 = QIcon()
-        icon72.addFile(u":/Icons/icons/import_profiles.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.edit_profiles_pushButton.setIcon(icon72)
+        icon73 = QIcon()
+        icon73.addFile(u":/Icons/icons/import_profiles.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.edit_profiles_pushButton.setIcon(icon73)
         self.edit_profiles_pushButton.setFlat(False)
 
         self.horizontalLayout.addWidget(self.edit_profiles_pushButton)
 
         self.edit_profiles_from_models_pushButton = QPushButton(self.frame)
         self.edit_profiles_from_models_pushButton.setObjectName(u"edit_profiles_from_models_pushButton")
-        icon73 = QIcon()
-        icon73.addFile(u":/Icons/icons/import_models.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.edit_profiles_from_models_pushButton.setIcon(icon73)
+        icon74 = QIcon()
+        icon74.addFile(u":/Icons/icons/import_models.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.edit_profiles_from_models_pushButton.setIcon(icon74)
         self.edit_profiles_from_models_pushButton.setFlat(False)
 
         self.horizontalLayout.addWidget(self.edit_profiles_from_models_pushButton)
 
-        self.horizontalSpacer = QSpacerItem(183, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer = QSpacerItem(183, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout.addItem(self.horizontalSpacer)
 
         self.plot_time_series_pushButton = QPushButton(self.frame)
         self.plot_time_series_pushButton.setObjectName(u"plot_time_series_pushButton")
-        icon74 = QIcon()
-        icon74.addFile(u":/Icons/icons/plot.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.plot_time_series_pushButton.setIcon(icon74)
+        icon75 = QIcon()
+        icon75.addFile(u":/Icons/icons/plot.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.plot_time_series_pushButton.setIcon(icon75)
 
         self.horizontalLayout.addWidget(self.plot_time_series_pushButton)
 
 
         self.verticalLayout_42.addWidget(self.frame)
 
         self.profiles_tableView = QTableView(self.tab_16)
@@ -765,96 +771,96 @@
         self.frame_12.setFrameShape(QFrame.NoFrame)
         self.frame_12.setFrameShadow(QFrame.Raised)
         self.horizontalLayout_4 = QHBoxLayout(self.frame_12)
         self.horizontalLayout_4.setObjectName(u"horizontalLayout_4")
         self.horizontalLayout_4.setContentsMargins(0, 0, 0, 0)
         self.copy_profile_pushButton = QPushButton(self.frame_12)
         self.copy_profile_pushButton.setObjectName(u"copy_profile_pushButton")
-        icon75 = QIcon()
-        icon75.addFile(u":/Icons/icons/copy.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.copy_profile_pushButton.setIcon(icon75)
+        icon76 = QIcon()
+        icon76.addFile(u":/Icons/icons/copy.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.copy_profile_pushButton.setIcon(icon76)
 
         self.horizontalLayout_4.addWidget(self.copy_profile_pushButton)
 
         self.paste_profiles_pushButton = QPushButton(self.frame_12)
         self.paste_profiles_pushButton.setObjectName(u"paste_profiles_pushButton")
-        icon76 = QIcon()
-        icon76.addFile(u":/Icons/icons/paste.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.paste_profiles_pushButton.setIcon(icon76)
+        icon77 = QIcon()
+        icon77.addFile(u":/Icons/icons/paste.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.paste_profiles_pushButton.setIcon(icon77)
 
         self.horizontalLayout_4.addWidget(self.paste_profiles_pushButton)
 
         self.set_linear_combination_profile_pushButton = QPushButton(self.frame_12)
         self.set_linear_combination_profile_pushButton.setObjectName(u"set_linear_combination_profile_pushButton")
-        icon77 = QIcon()
-        icon77.addFile(u":/Icons/icons/copy2right.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.set_linear_combination_profile_pushButton.setIcon(icon77)
+        icon78 = QIcon()
+        icon78.addFile(u":/Icons/icons/copy2right.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.set_linear_combination_profile_pushButton.setIcon(icon78)
 
         self.horizontalLayout_4.addWidget(self.set_linear_combination_profile_pushButton)
 
         self.device_type_magnitude_comboBox_2 = QComboBox(self.frame_12)
         self.device_type_magnitude_comboBox_2.setObjectName(u"device_type_magnitude_comboBox_2")
         self.device_type_magnitude_comboBox_2.setMinimumSize(QSize(200, 0))
 
         self.horizontalLayout_4.addWidget(self.device_type_magnitude_comboBox_2)
 
-        self.horizontalSpacer_13 = QSpacerItem(267, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_13 = QSpacerItem(267, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_4.addItem(self.horizontalSpacer_13)
 
         self.profile_add_pushButton = QPushButton(self.frame_12)
         self.profile_add_pushButton.setObjectName(u"profile_add_pushButton")
-        self.profile_add_pushButton.setIcon(icon69)
+        self.profile_add_pushButton.setIcon(icon70)
 
         self.horizontalLayout_4.addWidget(self.profile_add_pushButton)
 
         self.profile_subtract_pushButton = QPushButton(self.frame_12)
         self.profile_subtract_pushButton.setObjectName(u"profile_subtract_pushButton")
-        self.profile_subtract_pushButton.setIcon(icon70)
+        self.profile_subtract_pushButton.setIcon(icon71)
 
         self.horizontalLayout_4.addWidget(self.profile_subtract_pushButton)
 
         self.profile_multiply_pushButton = QPushButton(self.frame_12)
         self.profile_multiply_pushButton.setObjectName(u"profile_multiply_pushButton")
-        icon78 = QIcon()
-        icon78.addFile(u":/Icons/icons/multiply.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.profile_multiply_pushButton.setIcon(icon78)
+        icon79 = QIcon()
+        icon79.addFile(u":/Icons/icons/multiply.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.profile_multiply_pushButton.setIcon(icon79)
 
         self.horizontalLayout_4.addWidget(self.profile_multiply_pushButton)
 
         self.profile_divide_pushButton = QPushButton(self.frame_12)
         self.profile_divide_pushButton.setObjectName(u"profile_divide_pushButton")
-        icon79 = QIcon()
-        icon79.addFile(u":/Icons/icons/divide.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.profile_divide_pushButton.setIcon(icon79)
+        icon80 = QIcon()
+        icon80.addFile(u":/Icons/icons/divide.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.profile_divide_pushButton.setIcon(icon80)
 
         self.horizontalLayout_4.addWidget(self.profile_divide_pushButton)
 
         self.set_profile_value_pushButton = QPushButton(self.frame_12)
         self.set_profile_value_pushButton.setObjectName(u"set_profile_value_pushButton")
-        icon80 = QIcon()
-        icon80.addFile(u":/Icons/icons/copy2up.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.set_profile_value_pushButton.setIcon(icon80)
+        icon81 = QIcon()
+        icon81.addFile(u":/Icons/icons/copy2up.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.set_profile_value_pushButton.setIcon(icon81)
 
         self.horizontalLayout_4.addWidget(self.set_profile_value_pushButton)
 
         self.profile_factor_doubleSpinBox = QDoubleSpinBox(self.frame_12)
         self.profile_factor_doubleSpinBox.setObjectName(u"profile_factor_doubleSpinBox")
         self.profile_factor_doubleSpinBox.setMinimum(-999999.000000000000000)
         self.profile_factor_doubleSpinBox.setMaximum(9999999.000000000000000)
         self.profile_factor_doubleSpinBox.setValue(1.000000000000000)
 
         self.horizontalLayout_4.addWidget(self.profile_factor_doubleSpinBox)
 
 
         self.verticalLayout_42.addWidget(self.frame_12)
 
-        icon81 = QIcon()
-        icon81.addFile(u":/Icons/icons/time_series.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.tabWidget_5.addTab(self.tab_16, icon81, "")
+        icon82 = QIcon()
+        icon82.addFile(u":/Icons/icons/time_series.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.tabWidget_5.addTab(self.tab_16, icon82, "")
 
         self.verticalLayout_26.addWidget(self.tabWidget_5)
 
         self.dataStructuresSplitter.addWidget(self.frame_38)
 
         self.verticalLayout_8.addWidget(self.dataStructuresSplitter)
 
@@ -878,17 +884,17 @@
         self.simulationDataStructuresListView.setObjectName(u"simulationDataStructuresListView")
 
         self.gridLayout_19.addWidget(self.simulationDataStructuresListView, 1, 0, 1, 4)
 
         self.compute_simulation_data_pushButton = QPushButton(self.frame_28)
         self.compute_simulation_data_pushButton.setObjectName(u"compute_simulation_data_pushButton")
         self.compute_simulation_data_pushButton.setMaximumSize(QSize(32, 16777215))
-        icon82 = QIcon()
-        icon82.addFile(u":/Icons/icons/calculator.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.compute_simulation_data_pushButton.setIcon(icon82)
+        icon83 = QIcon()
+        icon83.addFile(u":/Icons/icons/calculator.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.compute_simulation_data_pushButton.setIcon(icon83)
 
         self.gridLayout_19.addWidget(self.compute_simulation_data_pushButton, 0, 0, 1, 1)
 
         self.exportSimulationDataButton = QPushButton(self.frame_28)
         self.exportSimulationDataButton.setObjectName(u"exportSimulationDataButton")
         self.exportSimulationDataButton.setMaximumSize(QSize(32, 16777215))
         self.exportSimulationDataButton.setIcon(icon3)
@@ -909,64 +915,64 @@
         self.gridLayout_23.setObjectName(u"gridLayout_23")
         self.gridLayout_23.setContentsMargins(0, 8, -1, -1)
         self.arrayModeComboBox = QComboBox(self.frame_29)
         self.arrayModeComboBox.setObjectName(u"arrayModeComboBox")
 
         self.gridLayout_23.addWidget(self.arrayModeComboBox, 0, 3, 1, 1)
 
-        self.horizontalSpacer_23 = QSpacerItem(510, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_23 = QSpacerItem(510, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.gridLayout_23.addItem(self.horizontalSpacer_23, 0, 5, 1, 1)
 
         self.simulationDataStructureTableView = QTableView(self.frame_29)
         self.simulationDataStructureTableView.setObjectName(u"simulationDataStructureTableView")
 
         self.gridLayout_23.addWidget(self.simulationDataStructureTableView, 1, 0, 1, 7)
 
         self.copyArraysToNumpyButton = QPushButton(self.frame_29)
         self.copyArraysToNumpyButton.setObjectName(u"copyArraysToNumpyButton")
-        icon83 = QIcon()
-        icon83.addFile(u":/Icons/icons/array.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.copyArraysToNumpyButton.setIcon(icon83)
+        icon84 = QIcon()
+        icon84.addFile(u":/Icons/icons/array.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.copyArraysToNumpyButton.setIcon(icon84)
 
         self.gridLayout_23.addWidget(self.copyArraysToNumpyButton, 0, 1, 1, 1)
 
         self.plotArraysButton = QPushButton(self.frame_29)
         self.plotArraysButton.setObjectName(u"plotArraysButton")
         self.plotArraysButton.setMinimumSize(QSize(32, 0))
-        self.plotArraysButton.setIcon(icon74)
+        self.plotArraysButton.setIcon(icon75)
 
         self.gridLayout_23.addWidget(self.plotArraysButton, 0, 6, 1, 1)
 
         self.copyArraysButton = QPushButton(self.frame_29)
         self.copyArraysButton.setObjectName(u"copyArraysButton")
         self.copyArraysButton.setMinimumSize(QSize(32, 0))
-        self.copyArraysButton.setIcon(icon75)
+        self.copyArraysButton.setIcon(icon76)
 
         self.gridLayout_23.addWidget(self.copyArraysButton, 0, 2, 1, 1)
 
         self.simulationDataSplitter.addWidget(self.frame_29)
 
         self.horizontalLayout_7.addWidget(self.simulationDataSplitter)
 
-        icon84 = QIcon()
-        icon84.addFile(u":/Icons/icons/spmat.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.tabWidget_3.addTab(self.compiledArraysTab, icon84, "")
+        icon85 = QIcon()
+        icon85.addFile(u":/Icons/icons/spmat.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.tabWidget_3.addTab(self.compiledArraysTab, icon85, "")
         self.commentsTab = QWidget()
         self.commentsTab.setObjectName(u"commentsTab")
         self.verticalLayout_18 = QVBoxLayout(self.commentsTab)
         self.verticalLayout_18.setObjectName(u"verticalLayout_18")
         self.comments_textEdit = QTextEdit(self.commentsTab)
         self.comments_textEdit.setObjectName(u"comments_textEdit")
 
         self.verticalLayout_18.addWidget(self.comments_textEdit)
 
-        icon85 = QIcon()
-        icon85.addFile(u":/Icons/icons/edit.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.tabWidget_3.addTab(self.commentsTab, icon85, "")
+        icon86 = QIcon()
+        icon86.addFile(u":/Icons/icons/edit.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.tabWidget_3.addTab(self.commentsTab, icon86, "")
 
         self.verticalLayout_9.addWidget(self.tabWidget_3)
 
         self.tabWidget.addTab(self.GridTab, icon57, "")
         self.ResultsTab = QWidget()
         self.ResultsTab.setObjectName(u"ResultsTab")
         self.verticalLayout_13 = QVBoxLayout(self.ResultsTab)
@@ -1016,21 +1022,21 @@
         brush1 = QBrush(QColor(190, 190, 190, 255))
         brush1.setStyle(Qt.SolidPattern)
         palette.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.label_16.setPalette(palette)
 
         self.horizontalLayout_34.addWidget(self.label_16)
 
-        self.horizontalSpacer_22 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_22 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_34.addItem(self.horizontalSpacer_22)
 
         self.deleteDriverButton = QPushButton(self.frame_62)
         self.deleteDriverButton.setObjectName(u"deleteDriverButton")
-        self.deleteDriverButton.setIcon(icon70)
+        self.deleteDriverButton.setIcon(icon71)
 
         self.horizontalLayout_34.addWidget(self.deleteDriverButton)
 
 
         self.verticalLayout_10.addWidget(self.frame_62)
 
         self.splitter.addWidget(self.frame_61)
@@ -1060,15 +1066,15 @@
         palette1.setBrush(QPalette.Active, QPalette.WindowText, brush)
         palette1.setBrush(QPalette.Inactive, QPalette.WindowText, brush)
         palette1.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.label_37.setPalette(palette1)
 
         self.horizontalLayout_33.addWidget(self.label_37)
 
-        self.horizontalSpacer_21 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_21 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_33.addItem(self.horizontalSpacer_21)
 
         self.loadResultFromDiskButton = QPushButton(self.frame_60)
         self.loadResultFromDiskButton.setObjectName(u"loadResultFromDiskButton")
         self.loadResultFromDiskButton.setIcon(icon1)
 
@@ -1127,78 +1133,78 @@
 
         self.search_results_Button = QPushButton(self.frame_8)
         self.search_results_Button.setObjectName(u"search_results_Button")
         self.search_results_Button.setIcon(icon60)
 
         self.horizontalLayout_2.addWidget(self.search_results_Button)
 
-        self.horizontalSpacer_20 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_20 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_2.addItem(self.horizontalSpacer_20)
 
         self.units_label = QLabel(self.frame_8)
         self.units_label.setObjectName(u"units_label")
 
         self.horizontalLayout_2.addWidget(self.units_label)
 
         self.results_traspose_checkBox = QCheckBox(self.frame_8)
         self.results_traspose_checkBox.setObjectName(u"results_traspose_checkBox")
-        icon86 = QIcon()
-        icon86.addFile(u":/Icons/icons/transpose.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.results_traspose_checkBox.setIcon(icon86)
+        icon87 = QIcon()
+        icon87.addFile(u":/Icons/icons/transpose.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.results_traspose_checkBox.setIcon(icon87)
 
         self.horizontalLayout_2.addWidget(self.results_traspose_checkBox)
 
         self.results_as_cdf_checkBox = QCheckBox(self.frame_8)
         self.results_as_cdf_checkBox.setObjectName(u"results_as_cdf_checkBox")
-        icon87 = QIcon()
-        icon87.addFile(u":/Icons/icons/cdf.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.results_as_cdf_checkBox.setIcon(icon87)
+        icon88 = QIcon()
+        icon88.addFile(u":/Icons/icons/cdf.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.results_as_cdf_checkBox.setIcon(icon88)
 
         self.horizontalLayout_2.addWidget(self.results_as_cdf_checkBox)
 
         self.results_as_abs_checkBox = QCheckBox(self.frame_8)
         self.results_as_abs_checkBox.setObjectName(u"results_as_abs_checkBox")
-        icon88 = QIcon()
-        icon88.addFile(u":/Icons/icons/abs.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.results_as_abs_checkBox.setIcon(icon88)
+        icon89 = QIcon()
+        icon89.addFile(u":/Icons/icons/abs.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.results_as_abs_checkBox.setIcon(icon89)
 
         self.horizontalLayout_2.addWidget(self.results_as_abs_checkBox)
 
         self.copy_results_pushButton = QPushButton(self.frame_8)
         self.copy_results_pushButton.setObjectName(u"copy_results_pushButton")
-        self.copy_results_pushButton.setIcon(icon75)
+        self.copy_results_pushButton.setIcon(icon76)
 
         self.horizontalLayout_2.addWidget(self.copy_results_pushButton)
 
         self.copy_numpy_button = QPushButton(self.frame_8)
         self.copy_numpy_button.setObjectName(u"copy_numpy_button")
-        self.copy_numpy_button.setIcon(icon83)
+        self.copy_numpy_button.setIcon(icon84)
 
         self.horizontalLayout_2.addWidget(self.copy_numpy_button)
 
         self.saveResultsButton = QPushButton(self.frame_8)
         self.saveResultsButton.setObjectName(u"saveResultsButton")
         self.saveResultsButton.setIcon(icon3)
 
         self.horizontalLayout_2.addWidget(self.saveResultsButton)
 
         self.plot_data_pushButton = QPushButton(self.frame_8)
         self.plot_data_pushButton.setObjectName(u"plot_data_pushButton")
-        self.plot_data_pushButton.setIcon(icon74)
+        self.plot_data_pushButton.setIcon(icon75)
 
         self.horizontalLayout_2.addWidget(self.plot_data_pushButton)
 
 
         self.verticalLayout_24.addWidget(self.frame_8)
 
 
         self.verticalLayout_40.addWidget(self.frame_5)
 
-        self.tabWidget_4.addTab(self.tab_7, icon83, "")
+        self.tabWidget_4.addTab(self.tab_7, icon84, "")
         self.tab_14 = QWidget()
         self.tab_14.setObjectName(u"tab_14")
         self.verticalLayout_41 = QVBoxLayout(self.tab_14)
         self.verticalLayout_41.setObjectName(u"verticalLayout_41")
         self.verticalLayout_41.setContentsMargins(-1, 6, -1, -1)
         self.resultsLogsTreeView = QTreeView(self.tab_14)
         self.resultsLogsTreeView.setObjectName(u"resultsLogsTreeView")
@@ -1209,15 +1215,15 @@
         self.frame_56 = QFrame(self.tab_14)
         self.frame_56.setObjectName(u"frame_56")
         self.frame_56.setFrameShape(QFrame.NoFrame)
         self.frame_56.setFrameShadow(QFrame.Raised)
         self.horizontalLayout_5 = QHBoxLayout(self.frame_56)
         self.horizontalLayout_5.setObjectName(u"horizontalLayout_5")
         self.horizontalLayout_5.setContentsMargins(0, 0, 0, 0)
-        self.horizontalSpacer_16 = QSpacerItem(866, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_16 = QSpacerItem(866, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_5.addItem(self.horizontalSpacer_16)
 
         self.saveResultsLogsButton = QPushButton(self.frame_56)
         self.saveResultsLogsButton.setObjectName(u"saveResultsLogsButton")
         self.saveResultsLogsButton.setIcon(icon3)
 
@@ -1230,15 +1236,15 @@
         self.results_splitter.addWidget(self.tabWidget_4)
 
         self.verticalLayout_28.addWidget(self.results_splitter)
 
 
         self.verticalLayout_13.addWidget(self.frame_33)
 
-        self.tabWidget.addTab(self.ResultsTab, icon74, "")
+        self.tabWidget.addTab(self.ResultsTab, icon75, "")
         self.main_console_tab = QWidget()
         self.main_console_tab.setObjectName(u"main_console_tab")
         self.verticalLayout_22 = QVBoxLayout(self.main_console_tab)
         self.verticalLayout_22.setObjectName(u"verticalLayout_22")
         self.verticalLayout_22.setContentsMargins(0, 0, 0, 0)
         self.frame_10 = QFrame(self.main_console_tab)
         self.frame_10.setObjectName(u"frame_10")
@@ -1289,17 +1295,17 @@
         self.label_98 = QLabel(self.frame_55)
         self.label_98.setObjectName(u"label_98")
 
         self.horizontalLayout_3.addWidget(self.label_98)
 
         self.runSourceCodeButton = QPushButton(self.frame_55)
         self.runSourceCodeButton.setObjectName(u"runSourceCodeButton")
-        icon89 = QIcon()
-        icon89.addFile(u":/Icons/icons/next.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.runSourceCodeButton.setIcon(icon89)
+        icon90 = QIcon()
+        icon90.addFile(u":/Icons/icons/next.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.runSourceCodeButton.setIcon(icon90)
 
         self.horizontalLayout_3.addWidget(self.runSourceCodeButton)
 
 
         self.verticalLayout_35.addWidget(self.frame_55)
 
         self.sourceCodeTextEdit = QPlainTextEdit(self.frame_11)
@@ -1326,17 +1332,17 @@
         self.tabWidget_2.setTabsClosable(False)
         self.tabWidget_2.setMovable(True)
         self.pythonConsoleTab = QWidget()
         self.pythonConsoleTab.setObjectName(u"pythonConsoleTab")
         self.verticalLayout_33 = QVBoxLayout(self.pythonConsoleTab)
         self.verticalLayout_33.setObjectName(u"verticalLayout_33")
         self.verticalLayout_33.setContentsMargins(0, 0, 0, 0)
-        icon90 = QIcon()
-        icon90.addFile(u":/Icons/icons/console.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.tabWidget_2.addTab(self.pythonConsoleTab, icon90, "")
+        icon91 = QIcon()
+        icon91.addFile(u":/Icons/icons/console.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.tabWidget_2.addTab(self.pythonConsoleTab, icon91, "")
         self.sourceCodeTab = QWidget()
         self.sourceCodeTab.setObjectName(u"sourceCodeTab")
         self.verticalLayout_39 = QVBoxLayout(self.sourceCodeTab)
         self.verticalLayout_39.setObjectName(u"verticalLayout_39")
         self.verticalLayout_39.setContentsMargins(6, 0, 6, 0)
         self.sourceCodeTreeView = QTreeView(self.sourceCodeTab)
         self.sourceCodeTreeView.setObjectName(u"sourceCodeTreeView")
@@ -1352,15 +1358,15 @@
         self.splitter_4.addWidget(self.console_splitter)
 
         self.verticalLayout_34.addWidget(self.splitter_4)
 
 
         self.verticalLayout_22.addWidget(self.frame_10)
 
-        self.tabWidget.addTab(self.main_console_tab, icon90, "")
+        self.tabWidget.addTab(self.main_console_tab, icon91, "")
         self.SettingsTab = QWidget()
         self.SettingsTab.setObjectName(u"SettingsTab")
         self.gridLayout_8 = QGridLayout(self.SettingsTab)
         self.gridLayout_8.setObjectName(u"gridLayout_8")
         self.settings_tabWidget = QTabWidget(self.SettingsTab)
         self.settings_tabWidget.setObjectName(u"settings_tabWidget")
         self.settings_tabWidget.setEnabled(True)
@@ -1438,15 +1444,15 @@
         self.gridLayout_22.addWidget(self.distributed_slack_checkBox, 4, 0, 1, 2)
 
         self.label_2 = QLabel(self.frame_19)
         self.label_2.setObjectName(u"label_2")
 
         self.gridLayout_22.addWidget(self.label_2, 0, 0, 1, 1)
 
-        self.verticalSpacer_10 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_10 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_22.addItem(self.verticalSpacer_10, 15, 0, 1, 1)
 
         self.label_11 = QLabel(self.frame_19)
         self.label_11.setObjectName(u"label_11")
 
         self.gridLayout_22.addWidget(self.label_11, 11, 0, 1, 1)
@@ -1555,15 +1561,15 @@
         self.verticalLayout_4.addWidget(self.apply_impedance_tolerances_checkBox)
 
         self.override_branch_controls_checkBox = QCheckBox(self.frame_36)
         self.override_branch_controls_checkBox.setObjectName(u"override_branch_controls_checkBox")
 
         self.verticalLayout_4.addWidget(self.override_branch_controls_checkBox)
 
-        self.verticalSpacer_14 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_14 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_4.addItem(self.verticalSpacer_14)
 
 
         self.gridLayout_9.addWidget(self.frame_36, 2, 1, 1, 1)
 
         self.line_14 = QFrame(self.frame_13)
@@ -1573,15 +1579,15 @@
         brush2.setStyle(Qt.SolidPattern)
         palette2.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette2.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette2.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_14.setPalette(palette2)
         self.line_14.setFrameShadow(QFrame.Plain)
         self.line_14.setLineWidth(4)
-        self.line_14.setFrameShape(QFrame.HLine)
+        self.line_14.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_9.addWidget(self.line_14, 1, 0, 1, 2)
 
         self.frame_20 = QFrame(self.frame_13)
         self.frame_20.setObjectName(u"frame_20")
         self.frame_20.setFrameShape(QFrame.NoFrame)
         self.frame_20.setFrameShadow(QFrame.Raised)
@@ -1615,15 +1621,15 @@
 
 
         self.gridLayout_9.addWidget(self.frame_20, 0, 0, 1, 2)
 
 
         self.horizontalLayout_23.addWidget(self.frame_13)
 
-        self.horizontalSpacer_5 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_5 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_23.addItem(self.horizontalSpacer_5)
 
         self.settings_tabWidget.addTab(self.tab_3, icon5, "")
         self.tab_5 = QWidget()
         self.tab_5.setObjectName(u"tab_5")
         self.horizontalLayout_10 = QHBoxLayout(self.tab_5)
@@ -1670,15 +1676,15 @@
         palette4 = QPalette()
         palette4.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette4.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette4.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_17.setPalette(palette4)
         self.line_17.setFrameShadow(QFrame.Plain)
         self.line_17.setLineWidth(4)
-        self.line_17.setFrameShape(QFrame.HLine)
+        self.line_17.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_2.addWidget(self.line_17, 1, 0, 1, 3)
 
         self.vs_departure_comboBox = QComboBox(self.frame_21)
         self.vs_departure_comboBox.setObjectName(u"vs_departure_comboBox")
 
         self.gridLayout_2.addWidget(self.vs_departure_comboBox, 11, 1, 1, 2)
@@ -1772,22 +1778,22 @@
 
         self.start_vs_from_default_radioButton = QRadioButton(self.frame_21)
         self.start_vs_from_default_radioButton.setObjectName(u"start_vs_from_default_radioButton")
         self.start_vs_from_default_radioButton.setChecked(True)
 
         self.gridLayout_2.addWidget(self.start_vs_from_default_radioButton, 7, 0, 1, 3)
 
-        self.verticalSpacer_7 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_7 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_2.addItem(self.verticalSpacer_7, 16, 0, 1, 3)
 
 
         self.horizontalLayout_10.addWidget(self.frame_21)
 
-        self.horizontalSpacer_24 = QSpacerItem(589, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_24 = QSpacerItem(589, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_10.addItem(self.horizontalSpacer_24)
 
         self.settings_tabWidget.addTab(self.tab_5, icon10, "")
         self.tab_4 = QWidget()
         self.tab_4.setObjectName(u"tab_4")
         self.gridLayout_10 = QGridLayout(self.tab_4)
@@ -1838,15 +1844,15 @@
         self.gridLayout_18.addWidget(self.opf_time_grouping_comboBox, 1, 1, 1, 1)
 
         self.mip_solver_comboBox = QComboBox(self.groupBox)
         self.mip_solver_comboBox.setObjectName(u"mip_solver_comboBox")
 
         self.gridLayout_18.addWidget(self.mip_solver_comboBox, 0, 1, 1, 1)
 
-        self.verticalSpacer_18 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_18 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_18.addItem(self.verticalSpacer_18, 10, 0, 1, 1)
 
         self.label_132 = QLabel(self.groupBox)
         self.label_132.setObjectName(u"label_132")
 
         self.gridLayout_18.addWidget(self.label_132, 4, 0, 1, 2)
@@ -1860,15 +1866,15 @@
         self.save_mip_checkBox.setObjectName(u"save_mip_checkBox")
 
         self.gridLayout_18.addWidget(self.save_mip_checkBox, 9, 0, 1, 2)
 
 
         self.gridLayout_10.addWidget(self.groupBox, 4, 3, 1, 1)
 
-        self.horizontalSpacer_10 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_10 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.gridLayout_10.addItem(self.horizontalSpacer_10, 4, 5, 1, 1)
 
         self.groupBox_3 = QGroupBox(self.tab_4)
         self.groupBox_3.setObjectName(u"groupBox_3")
         self.groupBox_3.setFont(font3)
         self.gridLayout_27 = QGridLayout(self.groupBox_3)
@@ -1884,15 +1890,15 @@
         self.gridLayout_27.addWidget(self.ips_method_comboBox, 0, 1, 1, 1)
 
         self.label_125 = QLabel(self.groupBox_3)
         self.label_125.setObjectName(u"label_125")
 
         self.gridLayout_27.addWidget(self.label_125, 0, 0, 1, 1)
 
-        self.verticalSpacer_21 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_21 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_27.addItem(self.verticalSpacer_21, 7, 0, 1, 1)
 
         self.label_126 = QLabel(self.groupBox_3)
         self.label_126.setObjectName(u"label_126")
 
         self.gridLayout_27.addWidget(self.label_126, 1, 0, 1, 1)
@@ -1964,15 +1970,15 @@
         palette7 = QPalette()
         palette7.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette7.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette7.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_16.setPalette(palette7)
         self.line_16.setFrameShadow(QFrame.Plain)
         self.line_16.setLineWidth(4)
-        self.line_16.setFrameShape(QFrame.HLine)
+        self.line_16.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_10.addWidget(self.line_16, 2, 0, 1, 5)
 
         self.groupBox_2 = QGroupBox(self.tab_4)
         self.groupBox_2.setObjectName(u"groupBox_2")
         self.groupBox_2.setFont(font3)
         self.gridLayout_26 = QGridLayout(self.groupBox_2)
@@ -1983,15 +1989,15 @@
         self.gridLayout_26.addWidget(self.label_128, 1, 0, 1, 1)
 
         self.label_42 = QLabel(self.groupBox_2)
         self.label_42.setObjectName(u"label_42")
 
         self.gridLayout_26.addWidget(self.label_42, 0, 0, 1, 1)
 
-        self.verticalSpacer_5 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_5 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_26.addItem(self.verticalSpacer_5, 7, 0, 1, 1)
 
         self.lpf_solver_comboBox = QComboBox(self.groupBox_2)
         self.lpf_solver_comboBox.setObjectName(u"lpf_solver_comboBox")
 
         self.gridLayout_26.addWidget(self.lpf_solver_comboBox, 0, 1, 1, 1)
@@ -2041,15 +2047,15 @@
         self.gridLayout_13.setObjectName(u"gridLayout_13")
         self.groupBox_6 = QGroupBox(self.tab_12)
         self.groupBox_6.setObjectName(u"groupBox_6")
         self.groupBox_6.setFlat(False)
         self.groupBox_6.setCheckable(False)
         self.gridLayout_29 = QGridLayout(self.groupBox_6)
         self.gridLayout_29.setObjectName(u"gridLayout_29")
-        self.verticalSpacer_24 = QSpacerItem(20, 393, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_24 = QSpacerItem(20, 393, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_29.addItem(self.verticalSpacer_24, 3, 0, 1, 1)
 
         self.n1ConsiderationCheckBox = QCheckBox(self.groupBox_6)
         self.n1ConsiderationCheckBox.setObjectName(u"n1ConsiderationCheckBox")
         self.n1ConsiderationCheckBox.setChecked(True)
 
@@ -2067,15 +2073,15 @@
         self.atcThresholdSpinBox.setValue(0.050000000000000)
 
         self.gridLayout_29.addWidget(self.atcThresholdSpinBox, 1, 0, 1, 2)
 
 
         self.gridLayout_13.addWidget(self.groupBox_6, 3, 3, 2, 1)
 
-        self.horizontalSpacer_6 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_6 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.gridLayout_13.addItem(self.horizontalSpacer_6, 3, 4, 2, 1)
 
         self.label_97 = QLabel(self.tab_12)
         self.label_97.setObjectName(u"label_97")
         self.label_97.setMinimumSize(QSize(24, 24))
         self.label_97.setMaximumSize(QSize(24, 24))
@@ -2100,23 +2106,23 @@
         palette9 = QPalette()
         palette9.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette9.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette9.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_27.setPalette(palette9)
         self.line_27.setFrameShadow(QFrame.Plain)
         self.line_27.setLineWidth(4)
-        self.line_27.setFrameShape(QFrame.HLine)
+        self.line_27.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_13.addWidget(self.line_27, 1, 0, 1, 4)
 
         self.groupBox_4 = QGroupBox(self.tab_12)
         self.groupBox_4.setObjectName(u"groupBox_4")
         self.gridLayout_20 = QGridLayout(self.groupBox_4)
         self.gridLayout_20.setObjectName(u"gridLayout_20")
-        self.verticalSpacer_22 = QSpacerItem(20, 325, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_22 = QSpacerItem(20, 325, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_20.addItem(self.verticalSpacer_22, 5, 0, 1, 1)
 
         self.label_30 = QLabel(self.groupBox_4)
         self.label_30.setObjectName(u"label_30")
 
         self.gridLayout_20.addWidget(self.label_30, 3, 0, 1, 1)
@@ -2176,15 +2182,15 @@
 
         self.skipNtcGenerationLimitsCheckBox = QCheckBox(self.groupBox_5)
         self.skipNtcGenerationLimitsCheckBox.setObjectName(u"skipNtcGenerationLimitsCheckBox")
         self.skipNtcGenerationLimitsCheckBox.setChecked(True)
 
         self.gridLayout_15.addWidget(self.skipNtcGenerationLimitsCheckBox, 0, 0, 1, 2)
 
-        self.verticalSpacer_23 = QSpacerItem(20, 168, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_23 = QSpacerItem(20, 168, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_15.addItem(self.verticalSpacer_23, 12, 1, 1, 1)
 
         self.ntcAlphaSpinBox = QSpinBox(self.groupBox_5)
         self.ntcAlphaSpinBox.setObjectName(u"ntcAlphaSpinBox")
         self.ntcAlphaSpinBox.setMaximum(100)
         self.ntcAlphaSpinBox.setValue(5)
@@ -2248,15 +2254,15 @@
         palette10 = QPalette()
         palette10.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette10.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette10.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_26.setPalette(palette10)
         self.line_26.setFrameShadow(QFrame.Plain)
         self.line_26.setLineWidth(4)
-        self.line_26.setFrameShape(QFrame.HLine)
+        self.line_26.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_4.addWidget(self.line_26, 1, 0, 1, 2)
 
         self.label_95 = QLabel(self.frame_40)
         self.label_95.setObjectName(u"label_95")
         palette11 = QPalette()
         palette11.setBrush(QPalette.Active, QPalette.WindowText, brush3)
@@ -2315,21 +2321,17 @@
         self.splitter_2.addWidget(self.frame_35)
 
         self.gridLayout_4.addWidget(self.splitter_2, 2, 0, 1, 2)
 
 
         self.horizontalLayout_12.addWidget(self.frame_40)
 
-        self.horizontalSpacer_11 = QSpacerItem(553, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
-
-        self.horizontalLayout_12.addItem(self.horizontalSpacer_11)
-
-        icon91 = QIcon()
-        icon91.addFile(u":/Icons/icons/area_transfer.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.settings_tabWidget.addTab(self.tab, icon91, "")
+        icon92 = QIcon()
+        icon92.addFile(u":/Icons/icons/area_transfer.svg", QSize(), QIcon.Normal, QIcon.Off)
+        self.settings_tabWidget.addTab(self.tab, icon92, "")
         self.tab_9 = QWidget()
         self.tab_9.setObjectName(u"tab_9")
         self.horizontalLayout_8 = QHBoxLayout(self.tab_9)
         self.horizontalLayout_8.setObjectName(u"horizontalLayout_8")
         self.frame_32 = QFrame(self.tab_9)
         self.frame_32.setObjectName(u"frame_32")
         self.frame_32.setFrameShape(QFrame.NoFrame)
@@ -2373,19 +2375,19 @@
         palette12 = QPalette()
         palette12.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette12.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette12.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_22.setPalette(palette12)
         self.line_22.setFrameShadow(QFrame.Plain)
         self.line_22.setLineWidth(4)
-        self.line_22.setFrameShape(QFrame.HLine)
+        self.line_22.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_14.addWidget(self.line_22, 1, 0, 1, 2)
 
-        self.verticalSpacer_12 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_12 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_14.addItem(self.verticalSpacer_12, 8, 0, 1, 1)
 
         self.frame_42 = QFrame(self.frame_32)
         self.frame_42.setObjectName(u"frame_42")
         self.frame_42.setFrameShape(QFrame.NoFrame)
         self.frame_42.setFrameShadow(QFrame.Raised)
@@ -2433,15 +2435,15 @@
         self.label_124.setObjectName(u"label_124")
 
         self.gridLayout_14.addWidget(self.label_124, 5, 0, 1, 1)
 
 
         self.horizontalLayout_8.addWidget(self.frame_32)
 
-        self.horizontalSpacer_8 = QSpacerItem(781, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_8 = QSpacerItem(781, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_8.addItem(self.horizontalSpacer_8)
 
         self.settings_tabWidget.addTab(self.tab_9, icon24, "")
         self.tab_11 = QWidget()
         self.tab_11.setObjectName(u"tab_11")
         self.horizontalLayout_42 = QHBoxLayout(self.tab_11)
@@ -2482,15 +2484,15 @@
         self.gridLayout_28.addWidget(self.label_53, 11, 0, 1, 1)
 
         self.label_119 = QLabel(self.frame_76)
         self.label_119.setObjectName(u"label_119")
 
         self.gridLayout_28.addWidget(self.label_119, 3, 0, 1, 2)
 
-        self.verticalSpacer_19 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_19 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_28.addItem(self.verticalSpacer_19, 16, 0, 1, 2)
 
         self.srap_top_n_SpinBox = QSpinBox(self.frame_76)
         self.srap_top_n_SpinBox.setObjectName(u"srap_top_n_SpinBox")
         self.srap_top_n_SpinBox.setMinimum(1)
         self.srap_top_n_SpinBox.setMaximum(9999999)
@@ -2557,15 +2559,15 @@
         palette15 = QPalette()
         palette15.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette15.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette15.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_25.setPalette(palette15)
         self.line_25.setFrameShadow(QFrame.Plain)
         self.line_25.setLineWidth(4)
-        self.line_25.setFrameShape(QFrame.HLine)
+        self.line_25.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_28.addWidget(self.line_25, 2, 0, 1, 2)
 
         self.label_1322 = QLabel(self.frame_76)
         self.label_1322.setObjectName(u"label_1322")
 
         self.gridLayout_28.addWidget(self.label_1322, 12, 0, 1, 1)
@@ -2581,217 +2583,40 @@
         self.contingency_deadband_SpinBox.setValue(0.050000000000000)
 
         self.gridLayout_28.addWidget(self.contingency_deadband_SpinBox, 7, 1, 1, 1)
 
 
         self.horizontalLayout_42.addWidget(self.frame_76)
 
-        self.horizontalSpacer_28 = QSpacerItem(828, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_28 = QSpacerItem(828, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_42.addItem(self.horizontalSpacer_28)
 
         self.settings_tabWidget.addTab(self.tab_11, icon41, "")
-        self.tab_6 = QWidget()
-        self.tab_6.setObjectName(u"tab_6")
-        self.gridLayout_12 = QGridLayout(self.tab_6)
-        self.gridLayout_12.setObjectName(u"gridLayout_12")
-        self.horizontalSpacer_12 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
-
-        self.gridLayout_12.addItem(self.horizontalSpacer_12, 2, 2, 1, 1)
-
-        self.frame_15 = QFrame(self.tab_6)
-        self.frame_15.setObjectName(u"frame_15")
-        self.frame_15.setMinimumSize(QSize(300, 0))
-        self.frame_15.setFrameShape(QFrame.NoFrame)
-        self.frame_15.setFrameShadow(QFrame.Raised)
-        self.gridLayout_6 = QGridLayout(self.frame_15)
-        self.gridLayout_6.setObjectName(u"gridLayout_6")
-        self.gridLayout_6.setContentsMargins(-1, 0, -1, -1)
-        self.max_iterations_stochastic_spinBox = QSpinBox(self.frame_15)
-        self.max_iterations_stochastic_spinBox.setObjectName(u"max_iterations_stochastic_spinBox")
-        self.max_iterations_stochastic_spinBox.setMinimum(10)
-        self.max_iterations_stochastic_spinBox.setMaximum(99999999)
-        self.max_iterations_stochastic_spinBox.setValue(1000)
-
-        self.gridLayout_6.addWidget(self.max_iterations_stochastic_spinBox, 6, 1, 1, 1)
-
-        self.verticalSpacer_8 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout_6.addItem(self.verticalSpacer_8, 7, 0, 1, 1)
-
-        self.stochastic_pf_method_comboBox = QComboBox(self.frame_15)
-        self.stochastic_pf_method_comboBox.setObjectName(u"stochastic_pf_method_comboBox")
-
-        self.gridLayout_6.addWidget(self.stochastic_pf_method_comboBox, 3, 1, 1, 1)
-
-        self.tolerance_stochastic_spinBox = QSpinBox(self.frame_15)
-        self.tolerance_stochastic_spinBox.setObjectName(u"tolerance_stochastic_spinBox")
-        self.tolerance_stochastic_spinBox.setMinimum(1)
-        self.tolerance_stochastic_spinBox.setMaximum(20)
-        self.tolerance_stochastic_spinBox.setValue(4)
-
-        self.gridLayout_6.addWidget(self.tolerance_stochastic_spinBox, 5, 1, 1, 1)
-
-        self.frame_45 = QFrame(self.frame_15)
-        self.frame_45.setObjectName(u"frame_45")
-        self.frame_45.setFrameShape(QFrame.NoFrame)
-        self.frame_45.setFrameShadow(QFrame.Raised)
-        self.horizontalLayout_17 = QHBoxLayout(self.frame_45)
-        self.horizontalLayout_17.setObjectName(u"horizontalLayout_17")
-        self.horizontalLayout_17.setContentsMargins(0, 0, 0, 0)
-        self.label_75 = QLabel(self.frame_45)
-        self.label_75.setObjectName(u"label_75")
-        self.label_75.setMinimumSize(QSize(24, 24))
-        self.label_75.setMaximumSize(QSize(24, 24))
-        self.label_75.setPixmap(QPixmap(u":/Icons/icons/stochastic_power_flow.svg"))
-        self.label_75.setScaledContents(True)
-
-        self.horizontalLayout_17.addWidget(self.label_75)
-
-        self.label_47 = QLabel(self.frame_45)
-        self.label_47.setObjectName(u"label_47")
-        palette16 = QPalette()
-        palette16.setBrush(QPalette.Active, QPalette.WindowText, brush3)
-        palette16.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
-        palette16.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.label_47.setPalette(palette16)
-        self.label_47.setFont(font2)
-        self.label_47.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
-
-        self.horizontalLayout_17.addWidget(self.label_47)
-
-
-        self.gridLayout_6.addWidget(self.frame_45, 0, 0, 1, 2)
-
-        self.line_4 = QFrame(self.frame_15)
-        self.line_4.setObjectName(u"line_4")
-        palette17 = QPalette()
-        palette17.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette17.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette17.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_4.setPalette(palette17)
-        self.line_4.setFrameShadow(QFrame.Plain)
-        self.line_4.setLineWidth(4)
-        self.line_4.setFrameShape(QFrame.HLine)
-
-        self.gridLayout_6.addWidget(self.line_4, 1, 0, 1, 2)
-
-        self.label_13 = QLabel(self.frame_15)
-        self.label_13.setObjectName(u"label_13")
-
-        self.gridLayout_6.addWidget(self.label_13, 6, 0, 1, 1)
-
-        self.label_55 = QLabel(self.frame_15)
-        self.label_55.setObjectName(u"label_55")
-
-        self.gridLayout_6.addWidget(self.label_55, 3, 0, 1, 1)
-
-        self.label_12 = QLabel(self.frame_15)
-        self.label_12.setObjectName(u"label_12")
-
-        self.gridLayout_6.addWidget(self.label_12, 5, 0, 1, 1)
-
-
-        self.gridLayout_12.addWidget(self.frame_15, 2, 0, 1, 1)
-
-        self.frame_22 = QFrame(self.tab_6)
-        self.frame_22.setObjectName(u"frame_22")
-        self.frame_22.setFrameShape(QFrame.NoFrame)
-        self.frame_22.setFrameShadow(QFrame.Raised)
-        self.verticalLayout_11 = QVBoxLayout(self.frame_22)
-        self.verticalLayout_11.setObjectName(u"verticalLayout_11")
-        self.verticalLayout_11.setContentsMargins(-1, 0, -1, -1)
-        self.frame_47 = QFrame(self.frame_22)
-        self.frame_47.setObjectName(u"frame_47")
-        self.frame_47.setFrameShape(QFrame.NoFrame)
-        self.frame_47.setFrameShadow(QFrame.Raised)
-        self.horizontalLayout_19 = QHBoxLayout(self.frame_47)
-        self.horizontalLayout_19.setObjectName(u"horizontalLayout_19")
-        self.horizontalLayout_19.setContentsMargins(0, 0, 0, 0)
-        self.label_78 = QLabel(self.frame_47)
-        self.label_78.setObjectName(u"label_78")
-        self.label_78.setMinimumSize(QSize(24, 24))
-        self.label_78.setMaximumSize(QSize(24, 24))
-        self.label_78.setPixmap(QPixmap(u":/Icons/icons/blackout.svg"))
-        self.label_78.setScaledContents(True)
-
-        self.horizontalLayout_19.addWidget(self.label_78)
-
-        self.label_79 = QLabel(self.frame_47)
-        self.label_79.setObjectName(u"label_79")
-        palette18 = QPalette()
-        palette18.setBrush(QPalette.Active, QPalette.WindowText, brush3)
-        palette18.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
-        palette18.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.label_79.setPalette(palette18)
-        self.label_79.setFont(font2)
-        self.label_79.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
-
-        self.horizontalLayout_19.addWidget(self.label_79)
-
-
-        self.verticalLayout_11.addWidget(self.frame_47)
-
-        self.line_10 = QFrame(self.frame_22)
-        self.line_10.setObjectName(u"line_10")
-        palette19 = QPalette()
-        palette19.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette19.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette19.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_10.setPalette(palette19)
-        self.line_10.setFrameShadow(QFrame.Plain)
-        self.line_10.setLineWidth(4)
-        self.line_10.setFrameShape(QFrame.HLine)
-
-        self.verticalLayout_11.addWidget(self.line_10)
-
-        self.label_28 = QLabel(self.frame_22)
-        self.label_28.setObjectName(u"label_28")
-
-        self.verticalLayout_11.addWidget(self.label_28)
-
-        self.cascading_islands_spinBox = QSpinBox(self.frame_22)
-        self.cascading_islands_spinBox.setObjectName(u"cascading_islands_spinBox")
-        self.cascading_islands_spinBox.setMinimum(1)
-        self.cascading_islands_spinBox.setMaximum(999999)
-        self.cascading_islands_spinBox.setValue(2)
-
-        self.verticalLayout_11.addWidget(self.cascading_islands_spinBox)
-
-        self.verticalSpacer_6 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.verticalLayout_11.addItem(self.verticalSpacer_6)
-
-
-        self.gridLayout_12.addWidget(self.frame_22, 2, 1, 1, 1)
-
-        icon92 = QIcon()
-        icon92.addFile(u":/Icons/icons/stochastic_power_flow.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.settings_tabWidget.addTab(self.tab_6, icon92, "")
         self.tab_2 = QWidget()
         self.tab_2.setObjectName(u"tab_2")
         self.horizontalLayout_6 = QHBoxLayout(self.tab_2)
         self.horizontalLayout_6.setObjectName(u"horizontalLayout_6")
         self.frame_18 = QFrame(self.tab_2)
         self.frame_18.setObjectName(u"frame_18")
         self.frame_18.setFrameShape(QFrame.NoFrame)
         self.frame_18.setFrameShadow(QFrame.Raised)
         self.gridLayout_21 = QGridLayout(self.frame_18)
         self.gridLayout_21.setObjectName(u"gridLayout_21")
         self.gridLayout_21.setContentsMargins(-1, 0, -1, -1)
         self.line_24 = QFrame(self.frame_18)
         self.line_24.setObjectName(u"line_24")
-        palette20 = QPalette()
-        palette20.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette20.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette20.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_24.setPalette(palette20)
+        palette16 = QPalette()
+        palette16.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette16.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette16.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_24.setPalette(palette16)
         self.line_24.setFrameShadow(QFrame.Plain)
         self.line_24.setLineWidth(4)
-        self.line_24.setFrameShape(QFrame.HLine)
+        self.line_24.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_21.addWidget(self.line_24, 14, 0, 1, 2)
 
         self.label_44 = QLabel(self.frame_18)
         self.label_44.setObjectName(u"label_44")
 
         self.gridLayout_21.addWidget(self.label_44, 17, 0, 1, 2)
@@ -2816,34 +2641,34 @@
         self.node_distances_elements_spinBox.setMaximum(99999)
         self.node_distances_elements_spinBox.setValue(2)
 
         self.gridLayout_21.addWidget(self.node_distances_elements_spinBox, 16, 0, 1, 2)
 
         self.label_121 = QLabel(self.frame_18)
         self.label_121.setObjectName(u"label_121")
-        palette21 = QPalette()
-        palette21.setBrush(QPalette.Active, QPalette.WindowText, brush3)
-        palette21.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
-        palette21.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.label_121.setPalette(palette21)
+        palette17 = QPalette()
+        palette17.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        palette17.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
+        palette17.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_121.setPalette(palette17)
         self.label_121.setFont(font2)
         self.label_121.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
 
         self.gridLayout_21.addWidget(self.label_121, 18, 1, 1, 1)
 
         self.line_30 = QFrame(self.frame_18)
         self.line_30.setObjectName(u"line_30")
-        palette22 = QPalette()
-        palette22.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette22.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette22.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_30.setPalette(palette22)
+        palette18 = QPalette()
+        palette18.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette18.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette18.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_30.setPalette(palette18)
         self.line_30.setFrameShadow(QFrame.Plain)
         self.line_30.setLineWidth(4)
-        self.line_30.setFrameShape(QFrame.HLine)
+        self.line_30.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_21.addWidget(self.line_30, 19, 0, 1, 2)
 
         self.investment_evaluation_method_ComboBox = QComboBox(self.frame_18)
         self.investment_evaluation_method_ComboBox.setObjectName(u"investment_evaluation_method_ComboBox")
 
         self.gridLayout_21.addWidget(self.investment_evaluation_method_ComboBox, 21, 0, 1, 2)
@@ -2861,15 +2686,15 @@
         self.label_120.setMinimumSize(QSize(24, 24))
         self.label_120.setMaximumSize(QSize(24, 24))
         self.label_120.setPixmap(QPixmap(u":/Icons/icons/expansion_planning.svg"))
         self.label_120.setScaledContents(True)
 
         self.gridLayout_21.addWidget(self.label_120, 18, 0, 1, 1)
 
-        self.verticalSpacer_16 = QSpacerItem(20, 250, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_16 = QSpacerItem(20, 250, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_21.addItem(self.verticalSpacer_16, 24, 1, 1, 1)
 
         self.label_7 = QLabel(self.frame_18)
         self.label_7.setObjectName(u"label_7")
 
         self.gridLayout_21.addWidget(self.label_7, 12, 0, 1, 2)
@@ -2886,34 +2711,34 @@
         self.label_3 = QLabel(self.frame_18)
         self.label_3.setObjectName(u"label_3")
 
         self.gridLayout_21.addWidget(self.label_3, 20, 0, 1, 2)
 
         self.label_89 = QLabel(self.frame_18)
         self.label_89.setObjectName(u"label_89")
-        palette23 = QPalette()
-        palette23.setBrush(QPalette.Active, QPalette.WindowText, brush3)
-        palette23.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
-        palette23.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.label_89.setPalette(palette23)
+        palette19 = QPalette()
+        palette19.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        palette19.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
+        palette19.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_89.setPalette(palette19)
         self.label_89.setFont(font2)
         self.label_89.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
 
         self.gridLayout_21.addWidget(self.label_89, 13, 1, 1, 1)
 
         self.line_29 = QFrame(self.frame_18)
         self.line_29.setObjectName(u"line_29")
-        palette24 = QPalette()
-        palette24.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette24.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette24.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_29.setPalette(palette24)
+        palette20 = QPalette()
+        palette20.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette20.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette20.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_29.setPalette(palette20)
         self.line_29.setFrameShadow(QFrame.Plain)
         self.line_29.setLineWidth(4)
-        self.line_29.setFrameShape(QFrame.HLine)
+        self.line_29.setFrameShape(QFrame.Shape.HLine)
 
         self.gridLayout_21.addWidget(self.line_29, 9, 0, 1, 3)
 
         self.label_51 = QLabel(self.frame_18)
         self.label_51.setObjectName(u"label_51")
 
         self.gridLayout_21.addWidget(self.label_51, 22, 0, 1, 2)
@@ -2923,19 +2748,19 @@
         self.frame_59.setFrameShape(QFrame.NoFrame)
         self.frame_59.setFrameShadow(QFrame.Raised)
         self.horizontalLayout_32 = QHBoxLayout(self.frame_59)
         self.horizontalLayout_32.setObjectName(u"horizontalLayout_32")
         self.horizontalLayout_32.setContentsMargins(0, 0, 0, 0)
         self.label_93 = QLabel(self.frame_59)
         self.label_93.setObjectName(u"label_93")
-        palette25 = QPalette()
-        palette25.setBrush(QPalette.Active, QPalette.WindowText, brush3)
-        palette25.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
-        palette25.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.label_93.setPalette(palette25)
+        palette21 = QPalette()
+        palette21.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        palette21.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
+        palette21.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_93.setPalette(palette21)
         self.label_93.setFont(font2)
         self.label_93.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
 
         self.horizontalLayout_32.addWidget(self.label_93)
 
 
         self.gridLayout_21.addWidget(self.frame_59, 8, 1, 1, 1)
@@ -2955,21 +2780,156 @@
         self.max_investments_evluation_number_spinBox.setValue(4)
 
         self.gridLayout_21.addWidget(self.max_investments_evluation_number_spinBox, 23, 0, 1, 2)
 
 
         self.horizontalLayout_6.addWidget(self.frame_18)
 
-        self.horizontalSpacer_3 = QSpacerItem(935, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.frame_15 = QFrame(self.tab_2)
+        self.frame_15.setObjectName(u"frame_15")
+        self.frame_15.setMinimumSize(QSize(300, 0))
+        self.frame_15.setFrameShape(QFrame.NoFrame)
+        self.frame_15.setFrameShadow(QFrame.Raised)
+        self.gridLayout_6 = QGridLayout(self.frame_15)
+        self.gridLayout_6.setObjectName(u"gridLayout_6")
+        self.gridLayout_6.setContentsMargins(-1, 0, -1, -1)
+        self.stochastic_pf_method_comboBox = QComboBox(self.frame_15)
+        self.stochastic_pf_method_comboBox.setObjectName(u"stochastic_pf_method_comboBox")
+
+        self.gridLayout_6.addWidget(self.stochastic_pf_method_comboBox, 3, 2, 1, 1)
+
+        self.label_55 = QLabel(self.frame_15)
+        self.label_55.setObjectName(u"label_55")
+
+        self.gridLayout_6.addWidget(self.label_55, 3, 0, 1, 2)
+
+        self.label_78 = QLabel(self.frame_15)
+        self.label_78.setObjectName(u"label_78")
+        self.label_78.setMinimumSize(QSize(24, 24))
+        self.label_78.setMaximumSize(QSize(24, 24))
+        self.label_78.setPixmap(QPixmap(u":/Icons/icons/blackout.svg"))
+        self.label_78.setScaledContents(True)
+
+        self.gridLayout_6.addWidget(self.label_78, 8, 0, 1, 1)
+
+        self.label_79 = QLabel(self.frame_15)
+        self.label_79.setObjectName(u"label_79")
+        palette22 = QPalette()
+        palette22.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        palette22.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
+        palette22.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_79.setPalette(palette22)
+        self.label_79.setFont(font2)
+        self.label_79.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
+
+        self.gridLayout_6.addWidget(self.label_79, 8, 1, 1, 2)
+
+        self.label_12 = QLabel(self.frame_15)
+        self.label_12.setObjectName(u"label_12")
+
+        self.gridLayout_6.addWidget(self.label_12, 5, 0, 1, 2)
+
+        self.label_13 = QLabel(self.frame_15)
+        self.label_13.setObjectName(u"label_13")
+
+        self.gridLayout_6.addWidget(self.label_13, 6, 0, 1, 2)
+
+        self.label_47 = QLabel(self.frame_15)
+        self.label_47.setObjectName(u"label_47")
+        palette23 = QPalette()
+        palette23.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        palette23.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
+        palette23.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_47.setPalette(palette23)
+        self.label_47.setFont(font2)
+        self.label_47.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
+
+        self.gridLayout_6.addWidget(self.label_47, 0, 1, 1, 2)
+
+        self.line_4 = QFrame(self.frame_15)
+        self.line_4.setObjectName(u"line_4")
+        palette24 = QPalette()
+        palette24.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette24.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette24.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_4.setPalette(palette24)
+        self.line_4.setFrameShadow(QFrame.Plain)
+        self.line_4.setLineWidth(4)
+        self.line_4.setFrameShape(QFrame.Shape.HLine)
+
+        self.gridLayout_6.addWidget(self.line_4, 1, 0, 1, 3)
+
+        self.label_138 = QLabel(self.frame_15)
+        self.label_138.setObjectName(u"label_138")
+
+        self.gridLayout_6.addWidget(self.label_138, 7, 0, 1, 3)
+
+        self.line_10 = QFrame(self.frame_15)
+        self.line_10.setObjectName(u"line_10")
+        palette25 = QPalette()
+        palette25.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette25.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette25.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_10.setPalette(palette25)
+        self.line_10.setFrameShadow(QFrame.Plain)
+        self.line_10.setLineWidth(4)
+        self.line_10.setFrameShape(QFrame.Shape.HLine)
+
+        self.gridLayout_6.addWidget(self.line_10, 9, 0, 1, 3)
+
+        self.max_iterations_stochastic_spinBox = QSpinBox(self.frame_15)
+        self.max_iterations_stochastic_spinBox.setObjectName(u"max_iterations_stochastic_spinBox")
+        self.max_iterations_stochastic_spinBox.setMinimum(10)
+        self.max_iterations_stochastic_spinBox.setMaximum(99999999)
+        self.max_iterations_stochastic_spinBox.setValue(1000)
+
+        self.gridLayout_6.addWidget(self.max_iterations_stochastic_spinBox, 6, 2, 1, 1)
+
+        self.verticalSpacer_8 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+
+        self.gridLayout_6.addItem(self.verticalSpacer_8, 12, 1, 1, 1)
+
+        self.tolerance_stochastic_spinBox = QSpinBox(self.frame_15)
+        self.tolerance_stochastic_spinBox.setObjectName(u"tolerance_stochastic_spinBox")
+        self.tolerance_stochastic_spinBox.setMinimum(1)
+        self.tolerance_stochastic_spinBox.setMaximum(20)
+        self.tolerance_stochastic_spinBox.setValue(4)
+
+        self.gridLayout_6.addWidget(self.tolerance_stochastic_spinBox, 5, 2, 1, 1)
+
+        self.label_75 = QLabel(self.frame_15)
+        self.label_75.setObjectName(u"label_75")
+        self.label_75.setMinimumSize(QSize(24, 24))
+        self.label_75.setMaximumSize(QSize(24, 24))
+        self.label_75.setPixmap(QPixmap(u":/Icons/icons/stochastic_power_flow.svg"))
+        self.label_75.setScaledContents(True)
+
+        self.gridLayout_6.addWidget(self.label_75, 0, 0, 1, 1)
+
+        self.label_28 = QLabel(self.frame_15)
+        self.label_28.setObjectName(u"label_28")
+
+        self.gridLayout_6.addWidget(self.label_28, 10, 0, 1, 3)
+
+        self.cascading_islands_spinBox = QSpinBox(self.frame_15)
+        self.cascading_islands_spinBox.setObjectName(u"cascading_islands_spinBox")
+        self.cascading_islands_spinBox.setMinimum(1)
+        self.cascading_islands_spinBox.setMaximum(999999)
+        self.cascading_islands_spinBox.setValue(2)
+
+        self.gridLayout_6.addWidget(self.cascading_islands_spinBox, 11, 0, 1, 3)
+
+
+        self.horizontalLayout_6.addWidget(self.frame_15)
+
+        self.horizontalSpacer_3 = QSpacerItem(935, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_6.addItem(self.horizontalSpacer_3)
 
-        icon93 = QIcon()
-        icon93.addFile(u":/Icons/icons/ml.svg", QSize(), QIcon.Normal, QIcon.Off)
-        self.settings_tabWidget.addTab(self.tab_2, icon93, "")
+        self.settings_tabWidget.addTab(self.tab_2, icon54, "")
         self.tab_13 = QWidget()
         self.tab_13.setObjectName(u"tab_13")
         self.gridLayout_17 = QGridLayout(self.tab_13)
         self.gridLayout_17.setObjectName(u"gridLayout_17")
         self.frame_39 = QFrame(self.tab_13)
         self.frame_39.setObjectName(u"frame_39")
         self.frame_39.setFrameShape(QFrame.NoFrame)
@@ -3013,15 +2973,15 @@
         palette27 = QPalette()
         palette27.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette27.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette27.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_21.setPalette(palette27)
         self.line_21.setFrameShadow(QFrame.Plain)
         self.line_21.setLineWidth(4)
-        self.line_21.setFrameShape(QFrame.HLine)
+        self.line_21.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayout_36.addWidget(self.line_21)
 
         self.label_24 = QLabel(self.frame_39)
         self.label_24.setObjectName(u"label_24")
         self.label_24.setTextFormat(Qt.PlainText)
         self.label_24.setScaledContents(True)
@@ -3045,15 +3005,15 @@
         palette28 = QPalette()
         palette28.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette28.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette28.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_13.setPalette(palette28)
         self.line_13.setFrameShadow(QFrame.Plain)
         self.line_13.setLineWidth(4)
-        self.line_13.setFrameShape(QFrame.HLine)
+        self.line_13.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayout_36.addWidget(self.line_13)
 
         self.label_60 = QLabel(self.frame_39)
         self.label_60.setObjectName(u"label_60")
 
         self.verticalLayout_36.addWidget(self.label_60)
@@ -3072,15 +3032,15 @@
         self.frame_52.setFrameShadow(QFrame.Raised)
         self.horizontalLayout_24 = QHBoxLayout(self.frame_52)
         self.horizontalLayout_24.setObjectName(u"horizontalLayout_24")
         self.horizontalLayout_24.setContentsMargins(0, 0, 0, 0)
 
         self.verticalLayout_36.addWidget(self.frame_52)
 
-        self.verticalSpacer_13 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_13 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_36.addItem(self.verticalSpacer_13)
 
 
         self.gridLayout_17.addWidget(self.frame_39, 0, 1, 1, 1)
 
         self.frame_31 = QFrame(self.tab_13)
@@ -3126,15 +3086,15 @@
         palette30 = QPalette()
         palette30.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette30.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette30.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_8.setPalette(palette30)
         self.line_8.setFrameShadow(QFrame.Plain)
         self.line_8.setLineWidth(4)
-        self.line_8.setFrameShape(QFrame.HLine)
+        self.line_8.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayout_25.addWidget(self.line_8)
 
         self.frame_23 = QFrame(self.frame_31)
         self.frame_23.setObjectName(u"frame_23")
         self.frame_23.setFrameShape(QFrame.NoFrame)
         self.frame_23.setFrameShadow(QFrame.Raised)
@@ -3157,22 +3117,22 @@
         self.rating_override_checkBox.setObjectName(u"rating_override_checkBox")
 
         self.verticalLayout_15.addWidget(self.rating_override_checkBox)
 
 
         self.verticalLayout_25.addWidget(self.frame_23)
 
-        self.verticalSpacer_15 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_15 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_25.addItem(self.verticalSpacer_15)
 
 
         self.gridLayout_17.addWidget(self.frame_31, 0, 2, 1, 1)
 
-        self.horizontalSpacer_18 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_18 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.gridLayout_17.addItem(self.horizontalSpacer_18, 0, 3, 1, 1)
 
         self.frame_27 = QFrame(self.tab_13)
         self.frame_27.setObjectName(u"frame_27")
         self.frame_27.setFrameShape(QFrame.NoFrame)
         self.frame_27.setFrameShadow(QFrame.Raised)
@@ -3215,15 +3175,15 @@
         palette32 = QPalette()
         palette32.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette32.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette32.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_20.setPalette(palette32)
         self.line_20.setFrameShadow(QFrame.Plain)
         self.line_20.setLineWidth(4)
-        self.line_20.setFrameShape(QFrame.HLine)
+        self.line_20.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayout_21.addWidget(self.line_20)
 
         self.label_59 = QLabel(self.frame_27)
         self.label_59.setObjectName(u"label_59")
 
         self.verticalLayout_21.addWidget(self.label_59)
@@ -3241,15 +3201,15 @@
 
         self.rxThresholdSpinBox = QSpinBox(self.frame_27)
         self.rxThresholdSpinBox.setObjectName(u"rxThresholdSpinBox")
         self.rxThresholdSpinBox.setValue(5)
 
         self.verticalLayout_21.addWidget(self.rxThresholdSpinBox)
 
-        self.verticalSpacer_11 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_11 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_21.addItem(self.verticalSpacer_11)
 
 
         self.gridLayout_17.addWidget(self.frame_27, 0, 0, 1, 1)
 
         self.settings_tabWidget.addTab(self.tab_13, icon13, "")
@@ -3301,15 +3261,15 @@
         palette34 = QPalette()
         palette34.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette34.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette34.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_9.setPalette(palette34)
         self.line_9.setFrameShadow(QFrame.Plain)
         self.line_9.setLineWidth(4)
-        self.line_9.setFrameShape(QFrame.HLine)
+        self.line_9.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayout_31.addWidget(self.line_9)
 
         self.frame_70 = QFrame(self.frame_46)
         self.frame_70.setObjectName(u"frame_70")
         self.frame_70.setFrameShape(QFrame.NoFrame)
         self.frame_70.setFrameShadow(QFrame.Raised)
@@ -3444,15 +3404,15 @@
         self.gridLayout.addWidget(self.label, 6, 0, 1, 1)
 
         self.palette_comboBox = QComboBox(self.frame_58)
         self.palette_comboBox.setObjectName(u"palette_comboBox")
 
         self.gridLayout.addWidget(self.palette_comboBox, 3, 0, 1, 2)
 
-        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout.addItem(self.verticalSpacer_4, 14, 0, 1, 1)
 
         self.label_113 = QLabel(self.frame_58)
         self.label_113.setObjectName(u"label_113")
 
         self.gridLayout.addWidget(self.label_113, 4, 0, 1, 1)
@@ -3516,15 +3476,15 @@
         self.verticalLayout_38.addWidget(self.label_118)
 
         self.tile_provider_comboBox = QComboBox(self.frame_73)
         self.tile_provider_comboBox.setObjectName(u"tile_provider_comboBox")
 
         self.verticalLayout_38.addWidget(self.tile_provider_comboBox)
 
-        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_38.addItem(self.verticalSpacer_2)
 
 
         self.horizontalLayout_39.addWidget(self.frame_73)
 
 
@@ -3577,15 +3537,15 @@
         palette40 = QPalette()
         palette40.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette40.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette40.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_6.setPalette(palette40)
         self.line_6.setFrameShadow(QFrame.Plain)
         self.line_6.setLineWidth(4)
-        self.line_6.setFrameShape(QFrame.HLine)
+        self.line_6.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayout_7.addWidget(self.line_6)
 
         self.frame_24 = QFrame(self.frame_3)
         self.frame_24.setObjectName(u"frame_24")
         self.frame_24.setFrameShape(QFrame.NoFrame)
         self.frame_24.setFrameShadow(QFrame.Raised)
@@ -3613,140 +3573,185 @@
         self.plt_style_comboBox.setObjectName(u"plt_style_comboBox")
 
         self.verticalLayout_16.addWidget(self.plt_style_comboBox)
 
 
         self.verticalLayout_7.addWidget(self.frame_24)
 
-        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_7.addItem(self.verticalSpacer)
 
 
         self.horizontalLayout_18.addWidget(self.frame_3)
 
-        self.horizontalSpacer_15 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_15 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_18.addItem(self.horizontalSpacer_15)
 
-        self.settings_tabWidget.addTab(self.tab_10, icon66, "")
+        self.settings_tabWidget.addTab(self.tab_10, icon67, "")
         self.tab_8 = QWidget()
         self.tab_8.setObjectName(u"tab_8")
         self.horizontalLayout_40 = QHBoxLayout(self.tab_8)
         self.horizontalLayout_40.setObjectName(u"horizontalLayout_40")
         self.frame_77 = QFrame(self.tab_8)
         self.frame_77.setObjectName(u"frame_77")
         self.frame_77.setMinimumSize(QSize(300, 0))
         self.frame_77.setFrameShape(QFrame.NoFrame)
         self.frame_77.setFrameShadow(QFrame.Raised)
-        self.verticalLayout_37 = QVBoxLayout(self.frame_77)
-        self.verticalLayout_37.setObjectName(u"verticalLayout_37")
+        self.gridLayout_11 = QGridLayout(self.frame_77)
+        self.gridLayout_11.setObjectName(u"gridLayout_11")
         self.label_115 = QLabel(self.frame_77)
         self.label_115.setObjectName(u"label_115")
+        palette41 = QPalette()
+        palette41.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        brush4 = QBrush(QColor(0, 0, 0, 255))
+        brush4.setStyle(Qt.SolidPattern)
+        palette41.setBrush(QPalette.Inactive, QPalette.WindowText, brush4)
+        palette41.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_115.setPalette(palette41)
         self.label_115.setFont(font2)
 
-        self.verticalLayout_37.addWidget(self.label_115)
+        self.gridLayout_11.addWidget(self.label_115, 0, 1, 1, 1)
 
-        self.line_28 = QFrame(self.frame_77)
-        self.line_28.setObjectName(u"line_28")
-        palette41 = QPalette()
-        palette41.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette41.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette41.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_28.setPalette(palette41)
-        self.line_28.setFrameShadow(QFrame.Plain)
-        self.line_28.setLineWidth(4)
-        self.line_28.setFrameShape(QFrame.HLine)
+        self.verticalSpacer_20 = QSpacerItem(20, 436, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+
+        self.gridLayout_11.addItem(self.verticalSpacer_20, 7, 1, 1, 1)
 
-        self.verticalLayout_37.addWidget(self.line_28)
+        self.label_136 = QLabel(self.frame_77)
+        self.label_136.setObjectName(u"label_136")
+        self.label_136.setMinimumSize(QSize(24, 24))
+        self.label_136.setMaximumSize(QSize(24, 24))
+        self.label_136.setPixmap(QPixmap(u":/Icons/icons/new2c.svg"))
+        self.label_136.setScaledContents(True)
+
+        self.gridLayout_11.addWidget(self.label_136, 0, 0, 1, 1)
 
         self.label_39 = QLabel(self.frame_77)
         self.label_39.setObjectName(u"label_39")
 
-        self.verticalLayout_37.addWidget(self.label_39)
+        self.gridLayout_11.addWidget(self.label_39, 2, 0, 1, 2)
 
-        self.file_information_label = QLabel(self.frame_77)
-        self.file_information_label.setObjectName(u"file_information_label")
-        self.file_information_label.setWordWrap(True)
-        self.file_information_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse|Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
+        self.line_28 = QFrame(self.frame_77)
+        self.line_28.setObjectName(u"line_28")
+        palette42 = QPalette()
+        palette42.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette42.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette42.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_28.setPalette(palette42)
+        self.line_28.setFrameShadow(QFrame.Plain)
+        self.line_28.setLineWidth(4)
+        self.line_28.setFrameShape(QFrame.Shape.HLine)
 
-        self.verticalLayout_37.addWidget(self.file_information_label)
+        self.gridLayout_11.addWidget(self.line_28, 1, 0, 1, 2)
 
-        self.model_version_label = QLabel(self.frame_77)
-        self.model_version_label.setObjectName(u"model_version_label")
+        self.saveResultsCheckBox = QCheckBox(self.frame_77)
+        self.saveResultsCheckBox.setObjectName(u"saveResultsCheckBox")
 
-        self.verticalLayout_37.addWidget(self.model_version_label)
+        self.gridLayout_11.addWidget(self.saveResultsCheckBox, 6, 0, 1, 2)
 
         self.user_name_label = QLabel(self.frame_77)
         self.user_name_label.setObjectName(u"user_name_label")
 
-        self.verticalLayout_37.addWidget(self.user_name_label)
+        self.gridLayout_11.addWidget(self.user_name_label, 5, 0, 1, 2)
 
-        self.saveResultsCheckBox = QCheckBox(self.frame_77)
-        self.saveResultsCheckBox.setObjectName(u"saveResultsCheckBox")
+        self.model_version_label = QLabel(self.frame_77)
+        self.model_version_label.setObjectName(u"model_version_label")
 
-        self.verticalLayout_37.addWidget(self.saveResultsCheckBox)
+        self.gridLayout_11.addWidget(self.model_version_label, 4, 0, 1, 2)
 
-        self.verticalSpacer_20 = QSpacerItem(20, 436, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.file_information_label = QLabel(self.frame_77)
+        self.file_information_label.setObjectName(u"file_information_label")
+        self.file_information_label.setWordWrap(True)
+        self.file_information_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse|Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
 
-        self.verticalLayout_37.addItem(self.verticalSpacer_20)
+        self.gridLayout_11.addWidget(self.file_information_label, 3, 0, 1, 2)
 
 
         self.horizontalLayout_40.addWidget(self.frame_77)
 
         self.frame_79 = QFrame(self.tab_8)
         self.frame_79.setObjectName(u"frame_79")
         self.frame_79.setMinimumSize(QSize(300, 0))
         self.frame_79.setFrameShape(QFrame.NoFrame)
         self.frame_79.setFrameShadow(QFrame.Raised)
         self.gridLayout_5 = QGridLayout(self.frame_79)
         self.gridLayout_5.setObjectName(u"gridLayout_5")
-        self.verticalSpacer_25 = QSpacerItem(20, 436, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout_5.addItem(self.verticalSpacer_25, 5, 0, 1, 1)
-
         self.cgmes_boundary_set_label = QLabel(self.frame_79)
         self.cgmes_boundary_set_label.setObjectName(u"cgmes_boundary_set_label")
 
-        self.gridLayout_5.addWidget(self.cgmes_boundary_set_label, 3, 0, 1, 1)
+        self.gridLayout_5.addWidget(self.cgmes_boundary_set_label, 6, 0, 1, 2)
 
-        self.selectCGMESBoundarySetButton = QPushButton(self.frame_79)
-        self.selectCGMESBoundarySetButton.setObjectName(u"selectCGMESBoundarySetButton")
-        self.selectCGMESBoundarySetButton.setMaximumSize(QSize(80, 16777215))
+        self.verticalSpacer_25 = QSpacerItem(20, 436, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
-        self.gridLayout_5.addWidget(self.selectCGMESBoundarySetButton, 3, 1, 1, 1)
+        self.gridLayout_5.addItem(self.verticalSpacer_25, 10, 1, 1, 1)
 
         self.label_90 = QLabel(self.frame_79)
         self.label_90.setObjectName(u"label_90")
 
-        self.gridLayout_5.addWidget(self.label_90, 2, 0, 1, 2)
+        self.gridLayout_5.addWidget(self.label_90, 5, 0, 1, 3)
+
+        self.label_134 = QLabel(self.frame_79)
+        self.label_134.setObjectName(u"label_134")
+        palette43 = QPalette()
+        palette43.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        palette43.setBrush(QPalette.Inactive, QPalette.WindowText, brush4)
+        palette43.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_134.setPalette(palette43)
+        self.label_134.setFont(font2)
+
+        self.gridLayout_5.addWidget(self.label_134, 0, 1, 1, 2)
+
+        self.selectCGMESBoundarySetButton = QPushButton(self.frame_79)
+        self.selectCGMESBoundarySetButton.setObjectName(u"selectCGMESBoundarySetButton")
+        self.selectCGMESBoundarySetButton.setMaximumSize(QSize(80, 16777215))
+
+        self.gridLayout_5.addWidget(self.selectCGMESBoundarySetButton, 6, 2, 1, 1)
 
         self.line_31 = QFrame(self.frame_79)
         self.line_31.setObjectName(u"line_31")
-        palette42 = QPalette()
-        palette42.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette42.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette42.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_31.setPalette(palette42)
+        palette44 = QPalette()
+        palette44.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette44.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette44.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_31.setPalette(palette44)
         self.line_31.setFrameShadow(QFrame.Plain)
         self.line_31.setLineWidth(4)
-        self.line_31.setFrameShape(QFrame.HLine)
+        self.line_31.setFrameShape(QFrame.Shape.HLine)
 
-        self.gridLayout_5.addWidget(self.line_31, 1, 0, 1, 2)
+        self.gridLayout_5.addWidget(self.line_31, 1, 0, 1, 3)
 
-        self.label_134 = QLabel(self.frame_79)
-        self.label_134.setObjectName(u"label_134")
-        self.label_134.setFont(font2)
+        self.label_137 = QLabel(self.frame_79)
+        self.label_137.setObjectName(u"label_137")
+        self.label_137.setMinimumSize(QSize(24, 24))
+        self.label_137.setMaximumSize(QSize(24, 24))
+        self.label_137.setPixmap(QPixmap(u":/Icons/icons/new2.svg"))
+        self.label_137.setScaledContents(True)
+
+        self.gridLayout_5.addWidget(self.label_137, 0, 0, 1, 1)
+
+        self.label_102 = QLabel(self.frame_79)
+        self.label_102.setObjectName(u"label_102")
+
+        self.gridLayout_5.addWidget(self.label_102, 4, 0, 1, 2)
+
+        self.cgmes_version_comboBox = QComboBox(self.frame_79)
+        self.cgmes_version_comboBox.setObjectName(u"cgmes_version_comboBox")
 
-        self.gridLayout_5.addWidget(self.label_134, 0, 0, 1, 2)
+        self.gridLayout_5.addWidget(self.cgmes_version_comboBox, 3, 0, 1, 3)
+
+        self.label_135 = QLabel(self.frame_79)
+        self.label_135.setObjectName(u"label_135")
+
+        self.gridLayout_5.addWidget(self.label_135, 2, 0, 1, 3)
 
 
         self.horizontalLayout_40.addWidget(self.frame_79)
 
-        self.horizontalSpacer_27 = QSpacerItem(659, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_27 = QSpacerItem(659, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_40.addItem(self.horizontalSpacer_27)
 
         self.settings_tabWidget.addTab(self.tab_8, icon4, "")
 
         self.gridLayout_8.addWidget(self.settings_tabWidget, 0, 2, 1, 1)
 
@@ -3770,37 +3775,37 @@
         self.label_68.setPixmap(QPixmap(u":/Icons/icons/gear.svg"))
         self.label_68.setScaledContents(True)
 
         self.horizontalLayout_13.addWidget(self.label_68)
 
         self.label_69 = QLabel(self.frame_41)
         self.label_69.setObjectName(u"label_69")
-        palette43 = QPalette()
-        palette43.setBrush(QPalette.Active, QPalette.WindowText, brush3)
-        palette43.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
-        palette43.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.label_69.setPalette(palette43)
+        palette45 = QPalette()
+        palette45.setBrush(QPalette.Active, QPalette.WindowText, brush3)
+        palette45.setBrush(QPalette.Inactive, QPalette.WindowText, brush3)
+        palette45.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.label_69.setPalette(palette45)
         self.label_69.setFont(font2)
         self.label_69.setAlignment(Qt.AlignBottom|Qt.AlignLeading|Qt.AlignLeft)
 
         self.horizontalLayout_13.addWidget(self.label_69)
 
 
         self.verticalLayout_12.addWidget(self.frame_41)
 
         self.line_5 = QFrame(self.frame_7)
         self.line_5.setObjectName(u"line_5")
-        palette44 = QPalette()
-        palette44.setBrush(QPalette.Active, QPalette.WindowText, brush2)
-        palette44.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
-        palette44.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
-        self.line_5.setPalette(palette44)
+        palette46 = QPalette()
+        palette46.setBrush(QPalette.Active, QPalette.WindowText, brush2)
+        palette46.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
+        palette46.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
+        self.line_5.setPalette(palette46)
         self.line_5.setFrameShadow(QFrame.Plain)
         self.line_5.setLineWidth(4)
-        self.line_5.setFrameShape(QFrame.HLine)
+        self.line_5.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayout_12.addWidget(self.line_5)
 
         self.frame_25 = QFrame(self.frame_7)
         self.frame_25.setObjectName(u"frame_25")
         self.frame_25.setFrameShape(QFrame.NoFrame)
         self.frame_25.setFrameShadow(QFrame.Raised)
@@ -3844,14 +3849,25 @@
         self.defaultBusVoltageSpinBox.setObjectName(u"defaultBusVoltageSpinBox")
         self.defaultBusVoltageSpinBox.setDecimals(1)
         self.defaultBusVoltageSpinBox.setMaximum(999999999.000000000000000)
         self.defaultBusVoltageSpinBox.setValue(10.000000000000000)
 
         self.verticalLayout_17.addWidget(self.defaultBusVoltageSpinBox)
 
+        self.label_101 = QLabel(self.frame_25)
+        self.label_101.setObjectName(u"label_101")
+
+        self.verticalLayout_17.addWidget(self.label_101)
+
+        self.snapshot_dateTimeEdit = QDateTimeEdit(self.frame_25)
+        self.snapshot_dateTimeEdit.setObjectName(u"snapshot_dateTimeEdit")
+        self.snapshot_dateTimeEdit.setCalendarPopup(True)
+
+        self.verticalLayout_17.addWidget(self.snapshot_dateTimeEdit)
+
         self.label_40 = QLabel(self.frame_25)
         self.label_40.setObjectName(u"label_40")
 
         self.verticalLayout_17.addWidget(self.label_40)
 
         self.label_31 = QLabel(self.frame_25)
         self.label_31.setObjectName(u"label_31")
@@ -3863,15 +3879,15 @@
         self.engineComboBox.setObjectName(u"engineComboBox")
 
         self.verticalLayout_17.addWidget(self.engineComboBox)
 
 
         self.verticalLayout_12.addWidget(self.frame_25)
 
-        self.verticalSpacer_3 = QSpacerItem(20, 363, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_3 = QSpacerItem(20, 363, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_12.addItem(self.verticalSpacer_3)
 
         self.dark_mode_checkBox = QCheckBox(self.frame_7)
         self.dark_mode_checkBox.setObjectName(u"dark_mode_checkBox")
 
         self.verticalLayout_12.addWidget(self.dark_mode_checkBox)
@@ -3949,15 +3965,15 @@
         font6 = QFont()
         font6.setPointSize(8)
         self.toolBar.setFont(font6)
         self.toolBar.setMovable(False)
         self.toolBar.setIconSize(QSize(26, 26))
         self.toolBar.setToolButtonStyle(Qt.ToolButtonIconOnly)
         self.toolBar.setFloatable(False)
-        mainWindow.addToolBar(Qt.TopToolBarArea, self.toolBar)
+        mainWindow.addToolBar(Qt.ToolBarArea.TopToolBarArea, self.toolBar)
 
         self.menuBar.addAction(self.menuProject.menuAction())
         self.menuBar.addAction(self.menuActions.menuAction())
         self.menuBar.addAction(self.menuDiagrams.menuAction())
         self.menuBar.addAction(self.menuModel.menuAction())
         self.menuBar.addAction(self.menuSimulations.menuAction())
         self.menuBar.addAction(self.menuAbout.menuAction())
@@ -4013,14 +4029,15 @@
         self.menuSimulations.addAction(self.actionAdd_selected_to_contingency)
         self.menuSimulations.addAction(self.actionATC)
         self.menuSimulations.addAction(self.actionATC_Time_Series)
         self.menuModel.addAction(self.actionAuto_rate_branches)
         self.menuModel.addAction(self.actionDetect_transformers)
         self.menuModel.addAction(self.actionEdit_simulation_time_limits)
         self.menuModel.addAction(self.actionProcess_topology)
+        self.menuModel.addAction(self.actionDetect_substations)
         self.menuModel.addAction(self.actionFuse_devices)
         self.menuModel.addAction(self.actionre_index_time)
         self.menuModel.addAction(self.actionScale)
         self.menuModel.addSeparator()
         self.menuModel.addAction(self.actionLaunch_data_analysis_tool)
         self.menuModel.addAction(self.actionFix_generators_active_based_on_the_power)
         self.menuModel.addAction(self.actionFix_loads_active_based_on_the_power)
@@ -4337,15 +4354,15 @@
         self.actionInitialize_contingencies.setText(QCoreApplication.translate("mainWindow", u"Initialize contingencies", None))
 #if QT_CONFIG(tooltip)
         self.actionInitialize_contingencies.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Contingencies wizard</span></p><p>Launch the contingencies wizard to automatically set up the contingency objects</p></body></html>", None))
 #endif // QT_CONFIG(tooltip)
         self.actionExport_contingencies.setText(QCoreApplication.translate("mainWindow", u"Contingencies", None))
         self.actionAdd_selected_to_contingency.setText(QCoreApplication.translate("mainWindow", u"Add selected as new contingency", None))
 #if QT_CONFIG(tooltip)
-        self.actionAdd_selected_to_contingency.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Contingency analysis</span></p><p>Create a new contingency from the schematic selection</p></body></html>", None))
+        self.actionAdd_selected_to_contingency.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Add contingency</span></p><p>Create a new contingency from the schematic selection</p></body></html>", None))
 #endif // QT_CONFIG(tooltip)
 #if QT_CONFIG(shortcut)
         self.actionAdd_selected_to_contingency.setShortcut(QCoreApplication.translate("mainWindow", u"Ctrl+A, Ctrl+C", None))
 #endif // QT_CONFIG(shortcut)
         self.actionAdd_selected_as_new_investment.setText(QCoreApplication.translate("mainWindow", u"Add selected as new investment", None))
 #if QT_CONFIG(tooltip)
         self.actionAdd_selected_as_new_investment.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Investments</span></p><p>Create new investment with the schematic selection</p></body></html>", None))
@@ -4403,14 +4420,15 @@
         self.actionSelect_buses_by_country.setText(QCoreApplication.translate("mainWindow", u"Select buses by country", None))
         self.actionScale.setText(QCoreApplication.translate("mainWindow", u"Scale", None))
 #if QT_CONFIG(tooltip)
         self.actionScale.setToolTip(QCoreApplication.translate("mainWindow", u"Scale the system load and or generation", None))
 #endif // QT_CONFIG(tooltip)
         self.actionDisable_all_results_tags.setText(QCoreApplication.translate("mainWindow", u"Disable all results tags", None))
         self.actionEnable_all_results_tags.setText(QCoreApplication.translate("mainWindow", u"Enable all results tags", None))
+        self.actionDetect_substations.setText(QCoreApplication.translate("mainWindow", u"Detect substations", None))
 #if QT_CONFIG(tooltip)
         self.grid_name_line_edit.setToolTip(QCoreApplication.translate("mainWindow", u"Name of the grid model", None))
 #endif // QT_CONFIG(tooltip)
 #if QT_CONFIG(tooltip)
         self.diagramsListView.setToolTip(QCoreApplication.translate("mainWindow", u"List of available diagrams", None))
 #endif // QT_CONFIG(tooltip)
 #if QT_CONFIG(tooltip)
@@ -4886,27 +4904,14 @@
         self.label_1322.setText(QCoreApplication.translate("mainWindow", u"SRAP top N", None))
 #if QT_CONFIG(tooltip)
         self.label_27.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p>Amount of contingency loading with respect to the base situation loading that triggers the report of the contingency. This is specially useful when we want to avoig reporting contingencies that are not significant with respect to the base situation.</p></body></html>", None))
 #endif // QT_CONFIG(tooltip)
         self.label_27.setText(QCoreApplication.translate("mainWindow", u"Contingency dead band", None))
         self.contingency_deadband_SpinBox.setSuffix(QCoreApplication.translate("mainWindow", u" %", None))
         self.settings_tabWidget.setTabText(self.settings_tabWidget.indexOf(self.tab_11), QCoreApplication.translate("mainWindow", u"Con", None))
-        self.tolerance_stochastic_spinBox.setPrefix(QCoreApplication.translate("mainWindow", u"1e-", None))
-        self.label_75.setText("")
-        self.label_47.setText(QCoreApplication.translate("mainWindow", u"Stochastic power flow", None))
-        self.label_13.setText(QCoreApplication.translate("mainWindow", u"Samples", None))
-        self.label_55.setText(QCoreApplication.translate("mainWindow", u"Method", None))
-        self.label_12.setText(QCoreApplication.translate("mainWindow", u"Voltage variance", None))
-        self.label_78.setText("")
-        self.label_79.setText(QCoreApplication.translate("mainWindow", u"Cascading", None))
-        self.label_28.setText(QCoreApplication.translate("mainWindow", u"Aditional islands until stop", None))
-        self.settings_tabWidget.setTabText(self.settings_tabWidget.indexOf(self.tab_6), QCoreApplication.translate("mainWindow", u"Sto", None))
-#if QT_CONFIG(tooltip)
-        self.settings_tabWidget.setTabToolTip(self.settings_tabWidget.indexOf(self.tab_6), QCoreApplication.translate("mainWindow", u"Stochastic power flow settings", None))
-#endif // QT_CONFIG(tooltip)
         self.label_44.setText("")
         self.label_88.setText("")
         self.label_33.setText(QCoreApplication.translate("mainWindow", u"Number of clusters", None))
 #if QT_CONFIG(tooltip)
         self.node_distances_elements_spinBox.setToolTip(QCoreApplication.translate("mainWindow", u"Minimum size of the group", None))
 #endif // QT_CONFIG(tooltip)
 #if QT_CONFIG(statustip)
@@ -4932,14 +4937,24 @@
         self.node_distances_sigma_doubleSpinBox.setToolTip(QCoreApplication.translate("mainWindow", u"M\u00e1ximum standard deviation to determine the groups", None))
 #endif // QT_CONFIG(tooltip)
         self.node_distances_sigma_doubleSpinBox.setSuffix(QCoreApplication.translate("mainWindow", u" \u03c3", None))
 #if QT_CONFIG(tooltip)
         self.max_investments_evluation_number_spinBox.setToolTip(QCoreApplication.translate("mainWindow", u"Number of maximum evaluations for the optimization methods", None))
 #endif // QT_CONFIG(tooltip)
         self.max_investments_evluation_number_spinBox.setSuffix(QCoreApplication.translate("mainWindow", u" x number of investments", None))
+        self.label_55.setText(QCoreApplication.translate("mainWindow", u"Method", None))
+        self.label_78.setText("")
+        self.label_79.setText(QCoreApplication.translate("mainWindow", u"Cascading", None))
+        self.label_12.setText(QCoreApplication.translate("mainWindow", u"Voltage variance", None))
+        self.label_13.setText(QCoreApplication.translate("mainWindow", u"Samples", None))
+        self.label_47.setText(QCoreApplication.translate("mainWindow", u"Stochastic power flow", None))
+        self.label_138.setText("")
+        self.tolerance_stochastic_spinBox.setPrefix(QCoreApplication.translate("mainWindow", u"1e-", None))
+        self.label_75.setText("")
+        self.label_28.setText(QCoreApplication.translate("mainWindow", u"Aditional islands until stop", None))
         self.settings_tabWidget.setTabText(self.settings_tabWidget.indexOf(self.tab_2), QCoreApplication.translate("mainWindow", u"ML", None))
 #if QT_CONFIG(tooltip)
         self.settings_tabWidget.setTabToolTip(self.settings_tabWidget.indexOf(self.tab_2), QCoreApplication.translate("mainWindow", u"Machine learning related settings", None))
 #endif // QT_CONFIG(tooltip)
         self.label_82.setText("")
         self.label_83.setText(QCoreApplication.translate("mainWindow", u"Node layout", None))
         self.label_24.setText(QCoreApplication.translate("mainWindow", u"Automatic layout algorithm", None))
@@ -4964,14 +4979,15 @@
         self.label_80.setText("")
         self.label_81.setText(QCoreApplication.translate("mainWindow", u"Grid reduction", None))
         self.label_59.setText(QCoreApplication.translate("mainWindow", u"Select branch types to reduce", None))
         self.rxThresholdCheckBox.setText(QCoreApplication.translate("mainWindow", u"Filter by r+x under threshold", None))
 #if QT_CONFIG(tooltip)
         self.rxThresholdSpinBox.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p>Exponent of the threshold to use.</p><p>threshold = 1x10^-factor</p><p>i.e.</p><p>factor=3</p><p>threshold = 1e-3</p></body></html>", None))
 #endif // QT_CONFIG(tooltip)
+        self.rxThresholdSpinBox.setPrefix(QCoreApplication.translate("mainWindow", u"1e-", None))
         self.settings_tabWidget.setTabText(self.settings_tabWidget.indexOf(self.tab_13), QCoreApplication.translate("mainWindow", u"Tplgy", None))
 #if QT_CONFIG(tooltip)
         self.settings_tabWidget.setTabToolTip(self.settings_tabWidget.indexOf(self.tab_13), QCoreApplication.translate("mainWindow", u"Topology related settings", None))
 #endif // QT_CONFIG(tooltip)
         self.label_76.setText("")
         self.label_49.setText(QCoreApplication.translate("mainWindow", u"Draw", None))
         self.label_56.setText(QCoreApplication.translate("mainWindow", u"Nodes", None))
@@ -5002,32 +5018,36 @@
         self.plt_style_comboBox.setToolTip(QCoreApplication.translate("mainWindow", u"MatPlotlib plot styles to choose from", None))
 #endif // QT_CONFIG(tooltip)
         self.settings_tabWidget.setTabText(self.settings_tabWidget.indexOf(self.tab_10), QCoreApplication.translate("mainWindow", u"Viz", None))
 #if QT_CONFIG(tooltip)
         self.settings_tabWidget.setTabToolTip(self.settings_tabWidget.indexOf(self.tab_10), QCoreApplication.translate("mainWindow", u"Visualization related settings", None))
 #endif // QT_CONFIG(tooltip)
         self.label_115.setText(QCoreApplication.translate("mainWindow", u"File Information", None))
+        self.label_136.setText("")
         self.label_39.setText(QCoreApplication.translate("mainWindow", u"File path", None))
-        self.file_information_label.setText(QCoreApplication.translate("mainWindow", u"...", None))
-        self.model_version_label.setText(QCoreApplication.translate("mainWindow", u"...", None))
-        self.user_name_label.setText(QCoreApplication.translate("mainWindow", u"...", None))
 #if QT_CONFIG(tooltip)
         self.saveResultsCheckBox.setToolTip(QCoreApplication.translate("mainWindow", u"If checked, the results are stored inside the gridcal file in a compressed format.", None))
 #endif // QT_CONFIG(tooltip)
         self.saveResultsCheckBox.setText(QCoreApplication.translate("mainWindow", u"Save results in .gridcal files", None))
+        self.user_name_label.setText(QCoreApplication.translate("mainWindow", u"...", None))
+        self.model_version_label.setText(QCoreApplication.translate("mainWindow", u"...", None))
+        self.file_information_label.setText(QCoreApplication.translate("mainWindow", u"...", None))
 #if QT_CONFIG(tooltip)
         self.cgmes_boundary_set_label.setToolTip(QCoreApplication.translate("mainWindow", u"Path of the CGMES default boundary set (single zip file)", None))
 #endif // QT_CONFIG(tooltip)
         self.cgmes_boundary_set_label.setText(QCoreApplication.translate("mainWindow", u"...", None))
+        self.label_90.setText(QCoreApplication.translate("mainWindow", u"Boundary set", None))
+        self.label_134.setText(QCoreApplication.translate("mainWindow", u"CGMES", None))
 #if QT_CONFIG(tooltip)
         self.selectCGMESBoundarySetButton.setToolTip(QCoreApplication.translate("mainWindow", u"Select the CGMES boundary set (single zip file)", None))
 #endif // QT_CONFIG(tooltip)
         self.selectCGMESBoundarySetButton.setText(QCoreApplication.translate("mainWindow", u"Select", None))
-        self.label_90.setText(QCoreApplication.translate("mainWindow", u"Boundary set", None))
-        self.label_134.setText(QCoreApplication.translate("mainWindow", u"CGMES", None))
+        self.label_137.setText("")
+        self.label_102.setText("")
+        self.label_135.setText(QCoreApplication.translate("mainWindow", u"Export version", None))
         self.settings_tabWidget.setTabText(self.settings_tabWidget.indexOf(self.tab_8), QCoreApplication.translate("mainWindow", u"File", None))
         self.label_68.setText("")
         self.label_69.setText(QCoreApplication.translate("mainWindow", u"General settings", None))
         self.label_57.setText(QCoreApplication.translate("mainWindow", u"Base power", None))
 #if QT_CONFIG(tooltip)
         self.sbase_doubleSpinBox.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Base power</span></p><p>Despite all the bibliography, changing this number to anything other than 100 MVA, might change the meaning of what sensible per-unit voltage are.</p><p>This is, 1.0 is no longer the nominal voltage and so on.</p></body></html>", None))
 #endif // QT_CONFIG(tooltip)
@@ -5038,14 +5058,15 @@
 #endif // QT_CONFIG(tooltip)
         self.fbase_doubleSpinBox.setSuffix(QCoreApplication.translate("mainWindow", u" Hz", None))
         self.label_35.setText(QCoreApplication.translate("mainWindow", u"Default bus voltage", None))
 #if QT_CONFIG(tooltip)
         self.defaultBusVoltageSpinBox.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Bus default voltage</span></p><p>This is the voltage that drag&amp;drop buses have when they are created from the schematic.</p></body></html>", None))
 #endif // QT_CONFIG(tooltip)
         self.defaultBusVoltageSpinBox.setSuffix(QCoreApplication.translate("mainWindow", u" kV", None))
+        self.label_101.setText(QCoreApplication.translate("mainWindow", u"Snapshot time", None))
         self.label_40.setText("")
         self.label_31.setText(QCoreApplication.translate("mainWindow", u"Engine", None))
 #if QT_CONFIG(tooltip)
         self.engineComboBox.setToolTip(QCoreApplication.translate("mainWindow", u"Engine to be used when available", None))
 #endif // QT_CONFIG(tooltip)
         self.dark_mode_checkBox.setText(QCoreApplication.translate("mainWindow", u"Dark mode", None))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.SettingsTab), QCoreApplication.translate("mainWindow", u"Settings", None))
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/update_gui_file.py` & `GridCal-5.1.5/GridCal/Gui/Main/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/ConsoleLog.py` & `GridCal-5.1.5/GridCal/Gui/Main/ConsoleLog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'ConsoleLog.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.1
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/object_select_window.py` & `GridCal-5.1.5/GridCal/Gui/Main/object_select_window.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/simulations.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/simulations.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/io.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,15 @@
             diagram = self.get_selected_diagram_widget()
             if diagram is not None:
                 if isinstance(diagram, DiagramEditorWidget):
                     diagram.center_nodes()
 
         self.collect_memory()
         self.setup_time_sliders()
+        self.get_circuit_snapshot_datetime()
 
     def add_circuit(self):
         """
         Prompt to add another circuit
         """
         self.open_file_threaded(post_function=self.post_add_circuit)
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/base_gui.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/base_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Scripting/scripting.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/scripting.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Settings/configuration.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Settings/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 
         # check boxes
         self.ui.dark_mode_checkBox.clicked.connect(self.change_theme_mode)
 
         # buttons
         self.ui.selectCGMESBoundarySetButton.clicked.connect(self.select_cgmes_boundary_set)
 
+        # DateTime change
+        self.ui.snapshot_dateTimeEdit.dateTimeChanged.connect(self.snapshot_datetime_changed)
+
     def change_theme_mode(self) -> None:
         """
         Change the GUI theme
         """
         custom_colors = {"primary": "#00aa88ff",
                          "primary>list.selectionBackground": "#00aa88be"}
 
@@ -393,20 +396,26 @@
                     self.save_gui_config()
                     print("Config file was erroneous, wrote a new one")
 
     def select_cgmes_boundary_set(self):
         """
         Select the current boundary set
         """
-        files_types = ("Boundary set (*.zip)")
+        files_types = "Boundary set (*.zip)"
 
         dialogue = QtWidgets.QFileDialog(None,
                                          caption='Select Boundary set file',
                                          directory=self.project_directory,
                                          filter=files_types)
-        # dialogue.setOption(QtWidgets.QFileDialog.Option.DontUseNativeDialog, True)
-
         if dialogue.exec():
             filenames = dialogue.selectedFiles()
             if len(filenames) > 0:
                 self.current_boundary_set = filenames[0]
                 self.ui.cgmes_boundary_set_label.setText(self.current_boundary_set)
+
+    def snapshot_datetime_changed(self):
+        """
+        Upon change of the snapshot datetime, change the circuit snapshot datetime
+        """
+        date_time_value = self.ui.snapshot_dateTimeEdit.dateTime().toPython()
+
+        self.circuit.snapshot_time = date_time_value
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/objects.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from GridCalEngine.DataStructures.numerical_circuit import NumericalCircuit, compile_numerical_circuit_at
 import GridCalEngine.basic_structures as bs
 import GridCalEngine.Devices as dev
 import GridCal.Gui.GuiFunctions as gf
 import GridCalEngine.Utils.Filtering as flt
 from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.Devices.types import ALL_DEV_TYPES
+from GridCalEngine.Topology.detect_substations import detect_substations
 from GridCal.Gui.Analysis.object_plot_analysis import object_histogram_analysis
 from GridCal.Gui.messages import yes_no_question, error_msg, warning_msg, info_msg
 from GridCal.Gui.Main.SubClasses.Model.diagrams import DiagramsMain
 from GridCal.Gui.TowerBuilder.LineBuilderDialogue import TowerBuilderGUI
 from GridCal.Gui.GeneralDialogues import LogsDialogue
 from GridCal.Gui.Diagrams.DiagramEditorWidget.diagram_editor_widget import DiagramEditorWidget
 from GridCal.Gui.SystemScaler.system_scaler import SystemScaler
@@ -64,14 +65,15 @@
         self.ui.add_object_pushButton.clicked.connect(self.add_objects)
         self.ui.structure_analysis_pushButton.clicked.connect(self.objects_histogram_analysis_plot)
 
         # menu trigger
         self.ui.actionDelete_inconsistencies.triggered.connect(self.delete_inconsistencies)
         self.ui.actionClean_database.triggered.connect(self.clean_database)
         self.ui.actionScale.triggered.connect(self.scale)
+        self.ui.actionDetect_substations.triggered.connect(self.detect_substations)
 
         # tree click
         self.ui.dataStructuresTreeView.clicked.connect(self.view_objects_data)
 
         # line edit enter
         self.ui.smart_search_lineEdit.returnPressed.connect(self.objects_smart_search)
         # self.ui.time_series_search.returnPressed.connect(self.timeseries_search)
@@ -1027,14 +1029,27 @@
         """
         Show the system scaler window
         The scaler window may modify the circuit
         """
         system_scaler_window = SystemScaler(grid=self.circuit, parent=self)
         system_scaler_window.exec()
 
+    def detect_substations(self):
+        """
+        Call the detect substations logc
+        """
+
+        ok = yes_no_question("Do you want to try to detect substations and voltage levels in the grid model?",
+                             "Detect substations")
+
+        if ok:
+            val = 1.0 / (10.0**self.ui.rxThresholdSpinBox.value())
+            detect_substations(grid=self.circuit,
+                               r_x_threshold=val)
+
     def show_objects_context_menu(self, pos: QtCore.QPoint):
         """
         Show diagrams list view context menu
         :param pos: Relative click position
         """
         context_menu = QtWidgets.QMenu(parent=self.ui.diagramsListView)
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/time_events.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/time_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
         # --------------------------------------------------------------------------------------------------------------
         self.ui.actionre_index_time.triggered.connect(self.re_index_time)
 
         # Buttons
         self.ui.new_profiles_structure_pushButton.clicked.connect(self.new_profiles_structure)
         self.ui.delete_profiles_structure_pushButton.clicked.connect(self.delete_profiles_structure)
-        # self.ui.set_profile_state_button.clicked.connect(self.set_profiles_state_to_grid)
         self.ui.edit_profiles_pushButton.clicked.connect(self.import_profiles)
         self.ui.edit_profiles_from_models_pushButton.clicked.connect(self.import_profiles_from_models)
         self.ui.set_profile_state_button.clicked.connect(self.set_profile_state_to_snapshot)
         self.ui.profile_add_pushButton.clicked.connect(lambda: self.modify_profiles('+'))
         self.ui.profile_subtract_pushButton.clicked.connect(lambda: self.modify_profiles('-'))
         self.ui.profile_multiply_pushButton.clicked.connect(lambda: self.modify_profiles('*'))
         self.ui.profile_divide_pushButton.clicked.connect(lambda: self.modify_profiles('/'))
@@ -457,22 +456,30 @@
         else:
             warning_msg("You need to declare a time profile first.\n\n"
                         "Then, this button will show the dialogue to\n"
                         "load the data from the models at the time steps\n"
                         "that you prefer.\n\n"
                         "Use the 'Create profiles button'.")
 
+    def get_circuit_snapshot_datetime(self):
+        """
+        Set the datetime from the circuit
+        """
+        val = self.circuit.snapshot_time
+        self.ui.snapshot_dateTimeEdit.setDateTime(val)
+
     def set_profile_state_to_snapshot(self):
         """
         Set the selected profiles state in the grid
         """
         idx = self.ui.db_step_slider.value()
 
         if idx > -1:
             self.circuit.set_state(t=idx)
+            self.get_circuit_snapshot_datetime()
         else:
             info_msg('Select a time series step to copy to the snapshot', 'Set snapshot')
 
     def copy_profiles(self):
         """
         Copy the current displayed profiles to the clipboard
         """
```

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/diagrams.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/diagrams.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Main/SubClasses/Results/results.py` & `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Results/results.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Visualization/visualization.py` & `GridCal-5.1.5/GridCal/Gui/Visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/Visualization/palettes.py` & `GridCal-5.1.5/GridCal/Gui/Visualization/palettes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SyncDialogue/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/SyncDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SyncDialogue/sync_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/SyncDialogue/sync_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SyncDialogue/gui.py` & `GridCal-5.1.5/GridCal/Gui/SyncDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py` & `GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SolarPowerWizard/gui.py` & `GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/RosetaExplorer/MainWindow.py` & `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/RosetaExplorer/update_gui_file.py` & `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/RosetaExplorer/RosetaExplorer.py` & `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/RosetaExplorer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/RosetaExplorer/ConsoleWidget.py` & `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/RosetaExplorer/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/LoadDesigner/load_designer.py` & `GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/LoadDesigner/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/LoadDesigner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/LoadDesigner/load_designer_ui.py` & `GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py` & `GridCal-5.1.5/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/WindPowerWizard/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/WindPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/WindPowerWizard/gui.py` & `GridCal-5.1.5/GridCal/Gui/WindPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SystemScaler/system_scaler.py` & `GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SystemScaler/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/SystemScaler/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SystemScaler/system_scaler_ui.py` & `GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TreeModelViewer/MainWindow.py` & `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TreeModelViewer/update_gui_file.py` & `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TreeModelViewer/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/TreeModelViewer/TreeModelViewer.py` & `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/TreeModelViewer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/gui.py` & `GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/GridGenerator/grid_generator_dialogue.py` & `GridCal-5.1.5/GridCal/Gui/GridGenerator/grid_generator_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/GridGenerator/icons_rc.py` & `GridCal-5.1.5/GridCal/Gui/GridGenerator/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/GridCal/Gui/GridGenerator/gui.py` & `GridCal-5.1.5/GridCal/Gui/GridGenerator/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.4/setup.py` & `GridCal-5.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                             'data/transformers.csv',
                             'data/wires.csv',
                             'data/sequence_lines.csv'],
                 }
 
 dependencies = ['setuptools>=41.0.1',
                 'wheel>=0.37.2',
-                "PySide6>=5.15",  # 5.14 breaks the UI generation for development
+                "PySide6<=6.6.3.1",  # 5.14 breaks the UI generation for development, 6.7.0 breaks all
                 "numpy>=1.19.0",
                 "scipy>=1.0.0",
                 "networkx>=2.1",
                 "pandas>=1.0",
                 "ortools>=9.8.0",
                 "xlwt>=1.3.0",
                 "xlrd>=1.1.0",
```

### Comparing `GridCal-5.1.4/PKG-INFO` & `GridCal-5.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCal
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

