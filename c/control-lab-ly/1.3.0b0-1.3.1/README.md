# Comparing `tmp/control-lab-ly-1.3.0b0.tar.gz` & `tmp/control-lab-ly-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.3.0b0.tar", last modified: Mon Feb 19 04:50:26 2024, max compression
+gzip compressed data, was "control-lab-ly-1.3.1.tar", last modified: Thu Apr 11 09:12:18 2024, max compression
```

## Comparing `control-lab-ly-1.3.0b0.tar` & `control-lab-ly-1.3.1.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.776821 control-lab-ly-1.3.0b0/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.3.0b0/LICENSE.md
--rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/MANIFEST.in
--rw-rw-rw-   0        0        0    25840 2024-02-19 04:50:26.776323 control-lab-ly-1.3.0b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.464041 control-lab-ly-1.3.0b0/docs/
--rw-rw-rw-   0        0        0    11209 2024-02-19 04:48:39.000000 control-lab-ly-1.3.0b0/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.3.0b0/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.3.0b0/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.3.0b0/docs/LICENSE.md
--rw-rw-rw-   0        0        0    13173 2024-02-16 02:53:34.000000 control-lab-ly-1.3.0b0/docs/README.md
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.467065 control-lab-ly-1.3.0b0/docs/assets/
--rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.3.0b0/docs/assets/Documentation guide.png
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.3.0b0/pyproject.toml
--rw-rw-rw-   0        0        0     1502 2024-02-19 04:50:26.778495 control-lab-ly-1.3.0b0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.3.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.374153 control-lab-ly-1.3.0b0/src/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.774329 control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    25840 2024-02-19 04:50:26.000000 control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7183 2024-02-19 04:50:26.000000 control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 04:50:26.000000 control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2024-02-19 04:50:26.000000 control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-19 04:50:26.000000 control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.481481 control-lab-ly-1.3.0b0/src/controllably/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.487287 control-lab-ly-1.3.0b0/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.491766 control-lab-ly-1.3.0b0/src/controllably/Compound/ForceClamper/
--rw-rw-rw-   0        0        0      261 2023-07-31 07:45:25.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/ForceClamper/__init__.py
--rw-rw-rw-   0        0        0     6299 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/ForceClamper/forceclamper_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.494826 control-lab-ly-1.3.0b0/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.498379 control-lab-ly-1.3.0b0/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    18427 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8214 2023-07-03 06:35:57.000000 control-lab-ly-1.3.0b0/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.500383 control-lab-ly-1.3.0b0/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.511562 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.525773 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/
--rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/__init__.py
--rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/maker_panel.py
--rw-rw-rw-   0        0        0     7976 2023-10-29 17:05:20.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/measurer_panel.py
--rw-rw-rw-   0        0        0    16511 2023-08-08 14:17:29.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/mover_panel.py
--rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
--rw-rw-rw-   0        0        0     4019 2024-02-07 03:02:59.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.534444 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/
--rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/__init__.py
--rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/loader_panel.py
--rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/pop_ups.py
--rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/templates.py
--rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/compound_panel.py
--rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0    14719 2023-09-05 05:32:23.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/guide_panel.py
--rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Control/GUI/multichannel_panel.py
--rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.3.0b0/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.539769 control-lab-ly-1.3.0b0/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.543769 control-lab-ly-1.3.0b0/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    11305 2023-08-02 03:11:01.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.546990 control-lab-ly-1.3.0b0/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9920 2023-07-25 02:35:05.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.549492 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.555088 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/
--rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/__init__.py
--rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.560829 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
--rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
--rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
--rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.564436 control-lab-ly-1.3.0b0/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0    11489 2023-07-12 03:09:07.000000 control-lab-ly-1.3.0b0/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     4136 2024-01-10 14:43:02.000000 control-lab-ly-1.3.0b0/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.574916 control-lab-ly-1.3.0b0/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.576416 control-lab-ly-1.3.0b0/src/controllably/Measure/Chemical/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.579972 control-lab-ly-1.3.0b0/src/controllably/Measure/Chemical/Sentron/
--rw-rw-rw-   0        0        0      259 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Chemical/Sentron/__init__.py
--rw-rw-rw-   0        0        0     7175 2024-02-16 02:09:56.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py
--rw-rw-rw-   0        0        0        0 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Chemical/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.584002 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.593464 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      377 2023-11-21 07:02:23.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    23170 2024-02-06 09:02:29.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2175 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.597516 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      302 2023-11-22 02:06:57.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    16747 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.605592 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.612870 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10789 2023-08-29 02:36:35.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.618286 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3549 2023-10-12 08:34:58.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0      247 2023-08-10 08:59:40.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0     8576 2023-08-29 02:54:55.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/load_cell_utils.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.625735 control-lab-ly-1.3.0b0/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      258 2023-08-11 05:01:25.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     9941 2023-08-11 05:02:02.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0     8206 2023-07-31 02:56:41.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/Physical/force_sensor_utils.py
--rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    14577 2023-08-14 02:29:33.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.628814 control-lab-ly-1.3.0b0/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.643112 control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      360 2024-01-03 07:23:50.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0    14600 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0    11041 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     9678 2024-01-03 09:37:19.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/grbl_lib.py
--rw-rw-rw-   0        0        0     9224 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.646824 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.657429 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.661254 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24212 2023-08-08 13:17:57.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    18542 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0    10073 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     6199 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    12736 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    37565 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.664419 control-lab-ly-1.3.0b0/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.674651 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.679745 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.687923 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    30135 2024-01-18 08:07:41.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.693266 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    32219 2023-11-08 05:13:56.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3457 2023-08-03 05:19:47.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.695290 control-lab-ly-1.3.0b0/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.698290 control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.704301 control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8815 2024-02-07 03:03:00.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.3.0b0/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.709999 control-lab-ly-1.3.0b0/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.713088 control-lab-ly-1.3.0b0/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.718248 control-lab-ly-1.3.0b0/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2024-01-29 16:02:35.000000 control-lab-ly-1.3.0b0/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.723375 control-lab-ly-1.3.0b0/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.0b0/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.3.0b0/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.726469 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.732033 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0      224 2023-07-28 03:13:38.000000 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/Flir/__init__.py
--rw-rw-rw-   0        0        0     1562 2023-08-10 02:38:36.000000 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/Flir/ax8_lib.py
--rw-rw-rw-   0        0        0    17276 2024-01-29 16:02:57.000000 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/Flir/ax8_utils.py
--rw-rw-rw-   0        0        0      225 2023-08-08 11:08:14.000000 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.737533 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     3128 2023-08-08 11:07:54.000000 control-lab-ly-1.3.0b0/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15703 2024-01-29 15:34:00.000000 control-lab-ly-1.3.0b0/src/controllably/View/image.py
--rw-rw-rw-   0        0        0    17271 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.751509 control-lab-ly-1.3.0b0/src/controllably/misc/
--rw-rw-rw-   0        0        0      661 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0     9550 2024-01-04 15:54:27.000000 control-lab-ly-1.3.0b0/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     8551 2024-01-12 10:16:16.000000 control-lab-ly-1.3.0b0/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    23338 2024-01-05 06:55:29.000000 control-lab-ly-1.3.0b0/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.3.0b0/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     5480 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.754271 control-lab-ly-1.3.0b0/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.756271 control-lab-ly-1.3.0b0/src/controllably/misc/templates/library/
--rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/library/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.758946 control-lab-ly-1.3.0b0/src/controllably/misc/templates/library/plugins/
--rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/library/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/library/plugins/my_plugin.py
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.764002 control-lab-ly-1.3.0b0/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.770323 control-lab-ly-1.3.0b0/src/controllably/misc/templates/tools/
--rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/tools/__init__.py
--rw-rw-rw-   0        0        0      439 2024-02-16 02:09:43.000000 control-lab-ly-1.3.0b0/src/controllably/misc/templates/tools/registry.yaml
-drwxrwxrwx   0        0        0        0 2024-02-19 04:50:26.772001 control-lab-ly-1.3.0b0/tests/
--rw-rw-rw-   0        0        0      363 2023-07-20 03:51:29.000000 control-lab-ly-1.3.0b0/tests/test_init.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.646182 control-lab-ly-1.3.1/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    26329 2024-04-11 09:12:18.645682 control-lab-ly-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.300680 control-lab-ly-1.3.1/docs/
+-rw-rw-rw-   0        0        0    11700 2024-04-11 09:06:45.000000 control-lab-ly-1.3.1/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.3.1/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.3.1/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    13173 2024-02-16 02:53:34.000000 control-lab-ly-1.3.1/docs/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.302433 control-lab-ly-1.3.1/docs/assets/
+-rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.3.1/docs/assets/Documentation guide.png
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1499 2024-04-11 09:12:18.651222 control-lab-ly-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.158280 control-lab-ly-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.642682 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    26329 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7183 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.319774 control-lab-ly-1.3.1/src/controllably/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.323275 control-lab-ly-1.3.1/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.326854 control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/
+-rw-rw-rw-   0        0        0      261 2023-07-31 07:45:25.000000 control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/__init__.py
+-rw-rw-rw-   0        0        0     6299 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/forceclamper_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.333628 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.337128 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    18427 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8214 2023-07-03 06:35:57.000000 control-lab-ly-1.3.1/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.338628 control-lab-ly-1.3.1/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.349834 control-lab-ly-1.3.1/src/controllably/Control/GUI/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.359846 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/
+-rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/__init__.py
+-rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/maker_panel.py
+-rw-rw-rw-   0        0        0     7976 2023-10-29 17:05:20.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/measurer_panel.py
+-rw-rw-rw-   0        0        0    16511 2023-08-08 14:17:29.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/mover_panel.py
+-rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+-rw-rw-rw-   0        0        0     4019 2024-02-07 03:02:59.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.373850 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/
+-rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/loader_panel.py
+-rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/pop_ups.py
+-rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/templates.py
+-rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0    14719 2023-09-05 05:32:23.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/guide_panel.py
+-rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/multichannel_panel.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.3.1/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.377350 control-lab-ly-1.3.1/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.383371 control-lab-ly-1.3.1/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    11341 2024-04-09 07:38:31.000000 control-lab-ly-1.3.1/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.387888 control-lab-ly-1.3.1/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9920 2023-07-25 02:35:05.000000 control-lab-ly-1.3.1/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.389387 control-lab-ly-1.3.1/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.393415 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.402341 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.405441 control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0    11489 2023-07-12 03:09:07.000000 control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     4136 2024-01-10 14:43:02.000000 control-lab-ly-1.3.1/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.414122 control-lab-ly-1.3.1/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.417882 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.421215 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/
+-rw-rw-rw-   0        0        0      259 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/__init__.py
+-rw-rw-rw-   0        0        0     7175 2024-02-16 02:09:56.000000 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.425408 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.436102 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      377 2023-11-21 07:02:23.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    23227 2024-04-05 09:10:59.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2175 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.439660 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      302 2023-11-22 02:06:57.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    17922 2024-04-11 05:01:17.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.445196 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.454651 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10789 2023-08-29 02:36:35.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.458678 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3549 2023-10-12 08:34:58.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0      247 2023-08-10 08:59:40.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0     8576 2023-08-29 02:54:55.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/load_cell_utils.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.467193 control-lab-ly-1.3.1/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      258 2023-08-11 05:01:25.000000 control-lab-ly-1.3.1/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     9941 2023-08-11 05:02:02.000000 control-lab-ly-1.3.1/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0     8206 2023-07-31 02:56:41.000000 control-lab-ly-1.3.1/src/controllably/Measure/Physical/force_sensor_utils.py
+-rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    14577 2023-08-14 02:29:33.000000 control-lab-ly-1.3.1/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.470192 control-lab-ly-1.3.1/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.479062 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      360 2024-01-03 07:23:50.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0    14600 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0    11446 2024-04-11 06:29:22.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     9678 2024-01-03 09:37:19.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/grbl_lib.py
+-rw-rw-rw-   0        0        0     9224 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.486156 control-lab-ly-1.3.1/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.494191 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.500265 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24212 2023-08-08 13:17:57.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    18542 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0    10073 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     6199 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    12736 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    37565 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.503765 control-lab-ly-1.3.1/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.510950 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.519380 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.524337 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    30840 2024-02-20 08:20:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.530024 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    32219 2023-11-08 05:13:56.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3457 2023-08-03 05:19:47.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.534395 control-lab-ly-1.3.1/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.537394 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.541395 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8815 2024-02-07 03:03:00.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.3.1/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.552235 control-lab-ly-1.3.1/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.557030 control-lab-ly-1.3.1/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.560561 control-lab-ly-1.3.1/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2024-01-29 16:02:35.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.566583 control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.572714 control-lab-ly-1.3.1/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.584412 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0      224 2023-07-28 03:13:38.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/__init__.py
+-rw-rw-rw-   0        0        0     1562 2023-08-10 02:38:36.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_lib.py
+-rw-rw-rw-   0        0        0    17276 2024-01-29 16:02:57.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_utils.py
+-rw-rw-rw-   0        0        0      225 2023-08-08 11:08:14.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.591730 control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     3128 2023-08-08 11:07:54.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15703 2024-01-29 15:34:00.000000 control-lab-ly-1.3.1/src/controllably/View/image.py
+-rw-rw-rw-   0        0        0    17271 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.613029 control-lab-ly-1.3.1/src/controllably/misc/
+-rw-rw-rw-   0        0        0      661 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0     9550 2024-01-04 15:54:27.000000 control-lab-ly-1.3.1/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     8551 2024-01-12 10:16:16.000000 control-lab-ly-1.3.1/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    24907 2024-02-20 10:17:37.000000 control-lab-ly-1.3.1/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     5480 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.619494 control-lab-ly-1.3.1/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.621494 control-lab-ly-1.3.1/src/controllably/misc/templates/library/
+-rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/library/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.625055 control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/
+-rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/my_plugin.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.631471 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.638640 control-lab-ly-1.3.1/src/controllably/misc/templates/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/tools/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/tools/registry.yaml
+drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.640647 control-lab-ly-1.3.1/tests/
+-rw-rw-rw-   0        0        0      363 2023-07-20 03:51:29.000000 control-lab-ly-1.3.1/tests/test_init.py
```

### Comparing `control-lab-ly-1.3.0b0/LICENSE.md` & `control-lab-ly-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/PKG-INFO` & `control-lab-ly-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.3.0b0
+Version: 1.3.1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -24,15 +24,15 @@
 License-File: LICENSE.md
 Requires-Dist: Markdown>=3.3
 Requires-Dist: numpy>=1.19
 Requires-Dist: opencv_python>=4.5.0
 Requires-Dist: pandas>=1.2
 Requires-Dist: pyModbusTCP>=0.2
 Requires-Dist: pyserial>=3.5
-Requires-Dist: PySimpleGUI>=4.60
+Requires-Dist: PySimpleGUI~=4.60
 Requires-Dist: PyVISA>=1.12
 Requires-Dist: PyVISA-py>=0.7
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: tkhtmlview>=0.2
 
 # Control.lab.ly
 Lab Equipment Automation Package
@@ -369,14 +369,27 @@
 
 ## License
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
+## Version 1.3.1
+Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
+### Added
+- implementation of `TriContinent.pullback()`
+- new `Well` properties and option in return list of wells by rows instead of columns
+
+### Changed
+- fix bugs in `Peltier` (`setTemperature()` and `getTemperature()`)
+- fix bugs in `Ender` (`setTemperature()` and `getTemperature()`)
+- fix bug in `Keithley.setFunction()`
+- generalise `IV_Scan` to take either currents or voltages
+
+
 ## Version 1.3.0
 Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
 ### Added
 - added check for poor physical connection with `PiezoRoboticsDevice`
 - Keithley
   - added new subclasses of `KeithleyDevice`: `DAQ6510` and `SMU2450`
   - added way to read and save model name of `KeithleyDevice`
```

### Comparing `control-lab-ly-1.3.0b0/docs/CHANGELOG.md` & `control-lab-ly-1.3.1/docs/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Change Log
 
+## Version 1.3.1
+Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
+### Added
+- implementation of `TriContinent.pullback()`
+- new `Well` properties and option in return list of wells by rows instead of columns
+
+### Changed
+- fix bugs in `Peltier` (`setTemperature()` and `getTemperature()`)
+- fix bugs in `Ender` (`setTemperature()` and `getTemperature()`)
+- fix bug in `Keithley.setFunction()`
+- generalise `IV_Scan` to take either currents or voltages
+
+
 ## Version 1.3.0
 Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
 ### Added
 - added check for poor physical connection with `PiezoRoboticsDevice`
 - Keithley
   - added new subclasses of `KeithleyDevice`: `DAQ6510` and `SMU2450`
   - added way to read and save model name of `KeithleyDevice`
```

### Comparing `control-lab-ly-1.3.0b0/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.3.1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/docs/LICENSE.md` & `control-lab-ly-1.3.1/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/docs/README.md` & `control-lab-ly-1.3.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/docs/assets/Documentation guide.png` & `control-lab-ly-1.3.1/docs/assets/Documentation guide.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/setup.cfg` & `control-lab-ly-1.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e33  y..version = 1.3
-00000030: 2e30 2d62 300d 0a64 6573 6372 6970 7469  .0-b0..descripti
-00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
-00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
-00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
-00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
-00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
-000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000b0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000c0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000d0: 0d0a 6175 7468 6f72 203d 2043 6861 6e67  ..author = Chang
-000000e0: 204a 6965 204c 656f 6e67 0d0a 6175 7468   Jie Leong..auth
-000000f0: 6f72 5f65 6d61 696c 203d 2063 6861 6e67  or_email = chang
-00000100: 6a69 652e 6c65 6f6e 6740 6f75 746c 6f6f  jie.leong@outloo
-00000110: 6b2e 636f 6d0d 0a75 726c 203d 2068 7474  k.com..url = htt
-00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000130: 6b79 6c65 6a65 616e 6c65 7769 732f 636f  kylejeanlewis/co
-00000140: 6e74 726f 6c2d 6c61 622d 6c65 0d0a 7072  ntrol-lab-le..pr
-00000150: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-00000160: 4769 7448 7562 203d 2068 7474 7073 3a2f  GitHub = https:/
-00000170: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
-00000180: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
-00000190: 6c2d 6c61 622d 6c65 0d0a 0944 6f63 756d  l-lab-le...Docum
-000001a0: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
-000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
-000001c0: 6c65 6a65 616e 6c65 7769 732f 636f 6e74  lejeanlewis/cont
-000001d0: 726f 6c2d 6c61 622d 6c65 2f62 6c6f 622f  rol-lab-le/blob/
-000001e0: 6d61 696e 2f64 6f63 732f 5245 4144 4d45  main/docs/README
-000001f0: 2e6d 640d 0a09 4368 616e 6765 6c6f 6720  .md...Changelog 
-00000200: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000210: 2e63 6f6d 2f6b 796c 656a 6561 6e6c 6577  .com/kylejeanlew
-00000220: 6973 2f63 6f6e 7472 6f6c 2d6c 6162 2d6c  is/control-lab-l
-00000230: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
-00000240: 2f43 4841 4e47 454c 4f47 2e6d 640d 0a09  /CHANGELOG.md...
-00000250: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
-00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
-00000270: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
-00000280: 6f6c 2d6c 6162 2d6c 652f 6973 7375 6573  ol-lab-le/issues
-00000290: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
-000002a0: 0a6b 6579 776f 7264 7320 3d20 0d0a 0970  .keywords = ...p
-000002b0: 7974 686f 6e0d 0a09 6c61 6220 6175 746f  ython...lab auto
-000002c0: 6d61 7469 6f6e 0d0a 636c 6173 7369 6669  mation..classifi
-000002d0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000002e0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
-000002f0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
-00000300: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000310: 4465 7665 6c6f 7065 7273 0d0a 0949 6e74  Developers...Int
-00000320: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000330: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000340: 6368 0d0a 094c 6963 656e 7365 203a 3a20  ch...License :: 
-00000350: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000360: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
-00000370: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000380: 3a20 4d69 6372 6f73 6f66 7420 3a3a 2057  : Microsoft :: W
-00000390: 696e 646f 7773 0d0a 0950 726f 6772 616d  indows...Program
-000003a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-000003c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003e0: 2033 2e38 0d0a 0954 6f70 6963 203a 3a20   3.8...Topic :: 
-000003f0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
-00000400: 6565 7269 6e67 0d0a 0d0a 5b6f 7074 696f  eering....[optio
-00000410: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-00000420: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-00000430: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
-00000440: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000450: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
-00000460: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000470: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
-00000480: 7569 7265 7320 3d20 0d0a 094d 6172 6b64  uires = ...Markd
-00000490: 6f77 6e3e 3d33 2e33 0d0a 096e 756d 7079  own>=3.3...numpy
-000004a0: 3e3d 312e 3139 0d0a 096f 7065 6e63 765f  >=1.19...opencv_
-000004b0: 7079 7468 6f6e 3e3d 342e 352e 300d 0a09  python>=4.5.0...
-000004c0: 7061 6e64 6173 3e3d 312e 320d 0a09 7079  pandas>=1.2...py
-000004d0: 4d6f 6462 7573 5443 503e 3d30 2e32 0d0a  ModbusTCP>=0.2..
-000004e0: 0970 7973 6572 6961 6c3e 3d33 2e35 0d0a  .pyserial>=3.5..
-000004f0: 0950 7953 696d 706c 6547 5549 3e3d 342e  .PySimpleGUI>=4.
-00000500: 3630 0d0a 0950 7956 4953 413e 3d31 2e31  60...PyVISA>=1.1
-00000510: 320d 0a09 5079 5649 5341 2d70 793e 3d30  2...PyVISA-py>=0
-00000520: 2e37 0d0a 0950 7959 414d 4c3e 3d36 2e30  .7...PyYAML>=6.0
-00000530: 0d0a 0974 6b68 746d 6c76 6965 773e 3d30  ...tkhtmlview>=0
-00000540: 2e32 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .2....[options.p
-00000550: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000560: 6865 7265 203d 2073 7263 0d0a 6578 636c  here = src..excl
-00000570: 7564 6520 3d20 7465 7374 730d 0a0d 0a5b  ude = tests....[
-00000580: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-00000590: 6461 7461 5d0d 0a2a 203d 202a 2e6a 736f  data]..* = *.jso
-000005a0: 6e2c 202a 2e79 616d 6c2c 202a 2e70 6e67  n, *.yaml, *.png
-000005b0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000005c0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000005d0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000030: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
+00000040: 3d20 4c61 6220 4571 7569 706d 656e 7420  = Lab Equipment 
+00000050: 4175 746f 6d61 7469 6f6e 2050 6163 6b61  Automation Packa
+00000060: 6765 0d0a 6c6f 6e67 5f64 6573 6372 6970  ge..long_descrip
+00000070: 7469 6f6e 203d 2066 696c 653a 2064 6f63  tion = file: doc
+00000080: 732f 5245 4144 4d45 2e6d 642c 2064 6f63  s/README.md, doc
+00000090: 732f 4348 414e 4745 4c4f 472e 6d64 0d0a  s/CHANGELOG.md..
+000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000b0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000c0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
+000000d0: 7574 686f 7220 3d20 4368 616e 6720 4a69  uthor = Chang Ji
+000000e0: 6520 4c65 6f6e 670d 0a61 7574 686f 725f  e Leong..author_
+000000f0: 656d 6169 6c20 3d20 6368 616e 676a 6965  email = changjie
+00000100: 2e6c 656f 6e67 406f 7574 6c6f 6f6b 2e63  .leong@outlook.c
+00000110: 6f6d 0d0a 7572 6c20 3d20 6874 7470 733a  om..url = https:
+00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
+00000130: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
+00000140: 6f6c 2d6c 6162 2d6c 650d 0a70 726f 6a65  ol-lab-le..proje
+00000150: 6374 5f75 726c 7320 3d20 0d0a 0947 6974  ct_urls = ...Git
+00000160: 4875 6220 3d20 6874 7470 733a 2f2f 6769  Hub = https://gi
+00000170: 7468 7562 2e63 6f6d 2f6b 796c 656a 6561  thub.com/kylejea
+00000180: 6e6c 6577 6973 2f63 6f6e 7472 6f6c 2d6c  nlewis/control-l
+00000190: 6162 2d6c 650d 0a09 446f 6375 6d65 6e74  ab-le...Document
+000001a0: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
+000001b0: 6769 7468 7562 2e63 6f6d 2f6b 796c 656a  github.com/kylej
+000001c0: 6561 6e6c 6577 6973 2f63 6f6e 7472 6f6c  eanlewis/control
+000001d0: 2d6c 6162 2d6c 652f 626c 6f62 2f6d 6169  -lab-le/blob/mai
+000001e0: 6e2f 646f 6373 2f52 4541 444d 452e 6d64  n/docs/README.md
+000001f0: 0d0a 0943 6861 6e67 656c 6f67 203d 2068  ...Changelog = h
+00000200: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000210: 6d2f 6b79 6c65 6a65 616e 6c65 7769 732f  m/kylejeanlewis/
+00000220: 636f 6e74 726f 6c2d 6c61 622d 6c65 2f62  control-lab-le/b
+00000230: 6c6f 622f 6d61 696e 2f64 6f63 732f 4348  lob/main/docs/CH
+00000240: 414e 4745 4c4f 472e 6d64 0d0a 0954 7261  ANGELOG.md...Tra
+00000250: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+00000260: 6974 6875 622e 636f 6d2f 6b79 6c65 6a65  ithub.com/kyleje
+00000270: 616e 6c65 7769 732f 636f 6e74 726f 6c2d  anlewis/control-
+00000280: 6c61 622d 6c65 2f69 7373 7565 730d 0a6c  lab-le/issues..l
+00000290: 6963 656e 7365 203d 204d 4954 0d0a 6b65  icense = MIT..ke
+000002a0: 7977 6f72 6473 203d 200d 0a09 7079 7468  ywords = ...pyth
+000002b0: 6f6e 0d0a 096c 6162 2061 7574 6f6d 6174  on...lab automat
+000002c0: 696f 6e0d 0a63 6c61 7373 6966 6965 7273  ion..classifiers
+000002d0: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
+000002e0: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
+000002f0: 416c 7068 610d 0a09 496e 7465 6e64 6564  Alpha...Intended
+00000300: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000310: 656c 6f70 6572 730d 0a09 496e 7465 6e64  elopers...Intend
+00000320: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
+00000330: 6369 656e 6365 2f52 6573 6561 7263 680d  cience/Research.
+00000340: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+00000350: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+00000360: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+00000370: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
+00000380: 6963 726f 736f 6674 203a 3a20 5769 6e64  icrosoft :: Wind
+00000390: 6f77 730d 0a09 5072 6f67 7261 6d6d 696e  ows...Programmin
+000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003b0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+000003c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000003d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000003e0: 380d 0a09 546f 7069 6320 3a3a 2053 6369  8...Topic :: Sci
+000003f0: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000400: 696e 670d 0a0d 0a5b 6f70 7469 6f6e 735d  ing....[options]
+00000410: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000420: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+00000430: 6573 203d 2066 696e 643a 0d0a 696e 636c  es = find:..incl
+00000440: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+00000450: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
+00000460: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+00000470: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000480: 6573 203d 200d 0a09 4d61 726b 646f 776e  es = ...Markdown
+00000490: 3e3d 332e 330d 0a09 6e75 6d70 793e 3d31  >=3.3...numpy>=1
+000004a0: 2e31 390d 0a09 6f70 656e 6376 5f70 7974  .19...opencv_pyt
+000004b0: 686f 6e3e 3d34 2e35 2e30 0d0a 0970 616e  hon>=4.5.0...pan
+000004c0: 6461 733e 3d31 2e32 0d0a 0970 794d 6f64  das>=1.2...pyMod
+000004d0: 6275 7354 4350 3e3d 302e 320d 0a09 7079  busTCP>=0.2...py
+000004e0: 7365 7269 616c 3e3d 332e 350d 0a09 5079  serial>=3.5...Py
+000004f0: 5369 6d70 6c65 4755 497e 3d34 2e36 300d  SimpleGUI~=4.60.
+00000500: 0a09 5079 5649 5341 3e3d 312e 3132 0d0a  ..PyVISA>=1.12..
+00000510: 0950 7956 4953 412d 7079 3e3d 302e 370d  .PyVISA-py>=0.7.
+00000520: 0a09 5079 5941 4d4c 3e3d 362e 300d 0a09  ..PyYAML>=6.0...
+00000530: 746b 6874 6d6c 7669 6577 3e3d 302e 320d  tkhtmlview>=0.2.
+00000540: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000550: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000560: 6520 3d20 7372 630d 0a65 7863 6c75 6465  e = src..exclude
+00000570: 203d 2074 6573 7473 0d0a 0d0a 5b6f 7074   = tests....[opt
+00000580: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
+00000590: 615d 0d0a 2a20 3d20 2a2e 6a73 6f6e 2c20  a]..* = *.json, 
+000005a0: 2a2e 7961 6d6c 2c20 2a2e 706e 670d 0a0d  *.yaml, *.png...
+000005b0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000005c0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000005d0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.3.1/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.3.0b0
+Version: 1.3.1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -24,15 +24,15 @@
 License-File: LICENSE.md
 Requires-Dist: Markdown>=3.3
 Requires-Dist: numpy>=1.19
 Requires-Dist: opencv_python>=4.5.0
 Requires-Dist: pandas>=1.2
 Requires-Dist: pyModbusTCP>=0.2
 Requires-Dist: pyserial>=3.5
-Requires-Dist: PySimpleGUI>=4.60
+Requires-Dist: PySimpleGUI~=4.60
 Requires-Dist: PyVISA>=1.12
 Requires-Dist: PyVISA-py>=0.7
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: tkhtmlview>=0.2
 
 # Control.lab.ly
 Lab Equipment Automation Package
@@ -369,14 +369,27 @@
 
 ## License
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
+## Version 1.3.1
+Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
+### Added
+- implementation of `TriContinent.pullback()`
+- new `Well` properties and option in return list of wells by rows instead of columns
+
+### Changed
+- fix bugs in `Peltier` (`setTemperature()` and `getTemperature()`)
+- fix bugs in `Ender` (`setTemperature()` and `getTemperature()`)
+- fix bug in `Keithley.setFunction()`
+- generalise `IV_Scan` to take either currents or voltages
+
+
 ## Version 1.3.0
 Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
 ### Added
 - added check for poor physical connection with `PiezoRoboticsDevice`
 - Keithley
   - added new subclasses of `KeithleyDevice`: `DAQ6510` and `SMU2450`
   - added way to read and save model name of `KeithleyDevice`
```

### Comparing `control-lab-ly-1.3.0b0/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.3.1/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Compound/ForceClamper/forceclamper_utils.py` & `control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/forceclamper_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.3.1/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/__init__.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/maker_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/maker_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/measurer_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/mover_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Basic/viewer_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/loader_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/pop_ups.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/pop_ups.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/Elements/templates.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/templates.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/compound_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/compound_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/guide_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/guide_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Control/GUI/multichannel_panel.py` & `control-lab-ly-1.3.1/src/controllably/Control/GUI/multichannel_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.3.1/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,18 +137,18 @@
         Returns:
             tuple[float]: set temperature, current temperature
         """
         response = self._read()
         now = datetime.now()
         try:
             values = [float(v) for v in response.split(';')]
-            self.set_temperature, self.temperature, self._cold_point, self._power = values
         except ValueError:
             print(response)
         else:
+            self.set_temperature, self.temperature, self._cold_point, self._power = values
             response = tuple(values)
             ready = (abs(self.set_temperature - self.temperature)<=self.tolerance)
             if not ready:
                 pass
             elif not self._stabilize_time:
                 self._stabilize_time = time.perf_counter()
                 print(response)
@@ -280,20 +280,21 @@
         try:
             device = serial.Serial(port, baudrate, timeout=timeout)
         except Exception as e:
             print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
         else:
+            self.device = device
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
             time.sleep(1)
             self.getTemperature()
             print(self.temperature)
-        self.device = device
+        # self.device = device
         return
     
     def _loop_feedback(self):
         """Loop to constantly read from device"""
         print('Listening...')
         while self.flags['get_feedback']:
             if self.flags['pause_feedback']:
```

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.3.1/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py` & `control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py` & `control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py` & `control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Make/make_utils.py` & `control-lab-ly-1.3.1/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,16 @@
         Set the function for either the sense or source terminals
 
         Args:
             function (str): type of function
             sense (bool, optional): whether to set the sense terminal. Defaults to True.
         """
         terminal = 'SENSe' if sense else 'SOURce'
-        return self._query(f'{terminal}:FUNCtion "{function}"')
+        function = f'"{function}"' if sense else function
+        return self._query(f'{terminal}:FUNCtion {function}')
     
     def setSource(self, value:float):
         """
         Set the source to a specified value
 
         Args:
             value (float): value to set source to
```

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import csv
 import pandas as pd
 import time
 from typing import Optional, Protocol
 
 # Local application imports
 from ....program_utils import Program
-from ..keithley_lib import SenseDetails, SourceDetails
+from ..keithley_lib import SenseDetails, SourceDetails, CURRENT_LIMITS, VOLTAGE_LIMITS
 print(f"Import: OK <{__name__}>")
 
 class Device(Protocol):
     sense: SenseDetails
     source: SourceDetails
     def beep(self, *args, **kwargs):
         ...
@@ -63,16 +63,19 @@
     
     ### Methods
     - `run`: run the measurement program
     
     ==========
     
     ### Parameters:
+        sense_limit (float, optional): measurement limit. Defaults to 1A or 200V.
+        currents (iterable, optional): current values to measure. Defaults to (0,).
+        voltages (iterable, optional): voltage values to measure. Defaults to (0,).
         count (int, optional): number of readings to take and average over. Defaults to 1.
-        currents (iterable): current values to measure. Defaults to (0,).
+        four_point (bool, optional): whether to use four point probe. Defaults to True.
     """
     
     def __init__(self, 
         device: Device, 
         parameters: Optional[dict] = None,
         verbose: bool = False, 
         **kwargs
@@ -88,24 +91,43 @@
         super().__init__(device=device, parameters=parameters, verbose=verbose, **kwargs)
         return
     
     def run(self):
         """Run the measurement program"""
         device = self.device
         count = self.parameters.get('count', 1)
+        four_point = self.parameters.get('four_point', True)
+        
+        if 'voltages' in self.parameters:
+            _source = 'voltage'
+            _sense = 'current'
+            values = self.parameters.get('voltages', (0,))
+            limits = VOLTAGE_LIMITS
+            sense_limit = CURRENT_LIMITS[-1]
+        elif 'currents' in self.parameters:
+            _source = 'current'
+            _sense = 'voltage'
+            values = self.parameters.get('currents', (0,))
+            limits = CURRENT_LIMITS
+            sense_limit = VOLTAGE_LIMITS[-1]
+        else:
+            raise Exception('Please provide either "voltages" or "currents" as a parameter')
+        max_value = max([abs(v) for v in values])
+        source_limit = min([l for l in limits if l >= max_value])
+        sense_limit = self.parameters.get('sense_limit', sense_limit)
         
         device.reset()
         device.sendCommands(['ROUTe:TERMinals FRONT'])
-        device.configureSource('current', measure_limit=200)
-        device.configureSense('voltage', limit=200, four_point=True, count=count)
+        device.configureSource(_source, limit=source_limit, measure_limit=sense_limit)
+        device.configureSense(_sense, limit=sense_limit, four_point=four_point, count=count)
         device.makeBuffer()
         device.beep()
         
-        for current in self.parameters.get('currents', (0,)):
-            device.setSource(value=current)
+        for value in values:
+            device.setSource(value=value)
             device.toggleOutput(on=True)
             device.run()
             time.sleep(0.1*count)
         time.sleep(1)
         self.data_df = device.readAll()
         device.beep()
         device.getErrors()
```

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Mechanical/load_cell_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/load_cell_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/Physical/force_sensor_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/Physical/force_sensor_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/__init__.py` & `control-lab-ly-1.3.1/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.3.1/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,22 +149,29 @@
         """
         Retrieve set temperature and actual temperature from device
         
         Returns:
             tuple[float]: set temperature, current temperature
         """
         responses = self._query('M105')  # Use 'M155 S<seconds>' to auto-report temperatures in S-second intervals. S0 to disable.
-        temperatures = [r for r in responses if '@' in r]
-        bed_temperatures = temperatures[-1].split(':')[2].split(' ')[:2]
-        temperature, set_temperature = bed_temperatures
-        self.temperature = float(temperature)
-        self.set_temperature = float(set_temperature[1:])
-        
-        ready = (abs(self.set_temperature - self.temperature)<=self.tolerance)
-        self.setFlag(temperature_reached=ready)
+        try:
+            temperatures = [r for r in responses if '@' in r]
+        except Exception as e:
+            raise e
+        else:
+            bed_temperatures = temperatures[-1].split(':')[2].split(' ')[:2]
+            temperature, set_temperature = bed_temperatures
+            self.temperature = float(temperature)
+            self.set_temperature = float(set_temperature[1:])
+        
+            ready = (abs(self.set_temperature - self.temperature)<=self.tolerance)
+            self.setFlag(temperature_reached=ready)
+            if ready:
+                print(bed_temperatures)
+                print(f"Temperature of {self.set_temperature}°C reached!")
         return self.set_temperature, self.temperature
     
     def holdTemperature(self, temperature:float, time_s:float):
         """
         Hold target temperature for desired duration
 
         Args:
@@ -215,40 +222,46 @@
         Checks and returns whether target temperature has been reached
 
         Returns:
             bool: whether target temperature has been reached
         """
         return self.flags['temperature_reached']
     
-    def setTemperature(self, set_temperature: float, blocking:bool = True):
+    def setTemperature(self, temperature: float, blocking:bool = True):
         """
         Set the temperature of the 3-D printer platform bed
 
         Args:
-            set_temperature (float): set point for platform temperature
+            temperature (float): set point for platform temperature
             blocking (bool, optional): whether to wait for temperature to reach set point. Defaults to True.
         """
-        if set_temperature < self.temperature_range[0] or set_temperature > self.temperature_range[1]:
+        if temperature < self.temperature_range[0] or temperature > self.temperature_range[1]:
             print(f'Please select a temperature between {self.temperature_range[0]} and {self.temperature_range[1]}°C.')
             return False
-        set_temperature = round( min(max(set_temperature,0), 110) )
-        command = f'M190 R{set_temperature}\n' if blocking else f'M140 S{set_temperature}\n'
-        
-        print(f"New set temperature at {set_temperature}°C")
-        if blocking:
-            print(f"Waiting for temperature to reach {set_temperature}°C")
+        temperature = round( min(max(temperature,0), 110) )
+        command = f'M190 S{temperature}\n'
         try:
             self._query(command)
         except Exception as e:
             print('Unable to heat stage!')
             if self.verbose:
                 print(e)
             return
         else:
+            while self.set_temperature != float(temperature):
+                self.getTemperature()
+        print(f"New set temperature at {temperature}°C")
+        
+        if blocking:
+            print(f"Waiting for temperature to reach {self.set_temperature}°C")
+        while not self.isAtTemperature():
             self.getTemperature()
+            time.sleep(0.1)
+            if not blocking:
+                break
         self.setFlag(temperature_reached=blocking)
         return
 
     def stop(self):
         """Halt all movement and print current coordinates"""
         self._query("M410")
         time.sleep(1)
```

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/grbl_lib.py` & `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/grbl_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Move/move_utils.py` & `control-lab-ly-1.3.1/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,16 +522,41 @@
         Returns:
             str: command string
         """
         command = self.rinse(cycles=cycles, channel=channel, print_message=False)
         print(f"Priming complete")
         return command
     
-    def pullback(self, channel: Optional[Union[int, tuple[int]]] = None, **kwargs) -> bool: # NOTE: no implementation
-        return ''
+    @_compound_action
+    def pullback(self, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> str:
+        """
+        Dispense desired volume of reagent
+
+        Args:
+            channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
+        """
+        steps = min(int(10/self.resolution), self.limits-self.position)
+        self.queue([
+            self.setStartSpeed(50),
+            self.setTopSpeed(200),
+            self.setSpeedRamp(1),
+            self.setValve('O'),
+            self.moveBy(abs(steps))
+        ], channel=channel)
+        command = self.current_pump.command
+        print(f"Pump: {self.name}")
+        print(f"Pulling back...")
+        self.run()
+        return command
 
     def queue(self, actions:list[str], channel:Optional[int] = None) -> str:
         """
         Queue several commands together before sending to the device
 
         Args:
             actions (list[str]): list of command strings
```

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.3.1/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.3.1/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/Thermal/Flir/ax8_lib.py` & `control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/Thermal/Flir/ax8_utils.py` & `control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.3.1/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/image.py` & `control-lab-ly-1.3.1/src/controllably/View/image.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/View/view_utils.py` & `control-lab-ly-1.3.1/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/__init__.py` & `control-lab-ly-1.3.1/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/decorators.py` & `control-lab-ly-1.3.1/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/factory.py` & `control-lab-ly-1.3.1/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/helper.py` & `control-lab-ly-1.3.1/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/layout.py` & `control-lab-ly-1.3.1/src/controllably/misc/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,31 @@
     ### Constructor
     Args:
         `labware_info` (dict): dictionary of truncated Labware information (name, slot, reference point)
         `name` (str): name of well
         `details` (dict[str, Union[float, tuple[float]]]): well details
     
     ### Attributes
+    - `content` (dict): contains the details of the contents within the well
     - `details` (dict): well details; dictionary of depth, total liquid volume, shape, diameter, x,y,z
     - `name` (str): name of well
     - `reference_point` (tuple[int]): bottom left reference corner of Labware
+    - `volume` (float): volume of contents in well
     
     ### Properties
+    - `base_area` (float): base area of well in mm^2
     - `bottom` (np.ndarray): bottom of well
     - `center` (np.ndarray): center of well
     - `depth` (float): well depth
     - `diameter` (float): well diameter
+    - `dimensions` (tuple[float]): dimensions of base in mm
+    - `level` (float): level of contents in well
     - `middle` (np.ndarray): middle of well
     - `offset` (np.ndarray): well offset from Labware reference point
+    - `shape` (str): shape of well
     - `top` (np.ndarray): top of well
     
     ### Methods
     - `fromBottom`: offset from bottom of well
     - `fromMiddle`: offset from middle of well
     - `fromTop`: offset from top of well
     """
@@ -56,27 +62,39 @@
         Instantiate the class
 
         Args:
             labware_info (dict): dictionary of truncated Labware information (name, slot, reference point)
             name (str): name of well
             details (dict[str, Union[float, tuple[float]]]): well details
         """
+        self.content = {}
         self.details = details  # depth,totalLiquidVolume,shape,diameter,x,y,z
         self.name = name
         self.reference_point = labware_info.get('reference_point', (0,0,0))
+        self.volume = 0
         
         self._labware_name = labware_info.get('name','')
         self._labware_slot = labware_info.get('slot','')
         pass
     
     def __repr__(self) -> str:
         return f"{self.name} in {self._labware_name} at Slot {self._labware_slot}" 
     
     # Properties
     @property
+    def base_area(self) -> float:
+        """Base area in mm^2"""
+        area_mm2 = 1
+        if self.shape == 'circular':
+            area_mm2 = 3.141592/4 * self.dimensions[0]**2
+        elif self.shape == 'rectangular':
+            area_mm2 = self.dimensions[0] * self.dimensions[1]
+        return area_mm2
+    
+    @property
     def bottom(self) -> np.ndarray:
         return self.center
     
     @property
     def center(self) -> np.ndarray:
         return np.array(self.reference_point) + self.offset
     
@@ -85,26 +103,45 @@
         return self.details.get('depth', 0)
     
     @property
     def diameter(self) -> float:
         return self.details.get('diameter', 0)
     
     @property
+    def dimensions(self) -> tuple[float]:
+        """Dimensions of base in mm"""
+        dim = []
+        if self.shape == 'circular':
+            dim.append(self.diameter)
+        elif self.shape == 'rectangular':
+            dim.append(self.details.get('xDimension',0))
+            dim.append(self.details.get('yDimension',0))
+        return tuple(dim)
+    
+    @property
+    def level(self) -> float:
+        return self.volume / self.base_area
+        
+    @property
     def middle(self) -> np.ndarray:
         depth = self.details.get('depth', 0)
         return self.center + np.array((0,0,depth/2))
         
     @property
     def offset(self) -> np.ndarray:
         x = self.details.get('x', 0)
         y = self.details.get('y', 0)
         z = self.details.get('z', 0)
         return np.array((x,y,z))
     
     @property
+    def shape(self) -> str:
+        return self.details.get('shape', '')
+    
+    @property
     def top(self) -> np.ndarray:
         depth = self.details.get('depth', 0)
         return self.center + np.array((0,0,depth))
     
     def fromBottom(self, offset:tuple[float]) -> np.ndarray:
         """
         Offset from bottom of well
@@ -227,14 +264,15 @@
             slot (str): deck slot number
             bottom_left_coordinates (tuple[float]): coordinates of bottom left corner (i.e. reference point)
             labware_file (str): filepath of Labware JSON file
             package (Optional[str], optional): name of package to look in. Defaults to None.
         """
         self.details = helper.read_json(json_file=labware_file, package=package)
         self.name = self.details.get('metadata',{}).get('displayName', '')
+        self.order_wells_by_rows = False
         self._reference_point = tuple(bottom_left_coordinates)
         self.slot = slot
         self._wells = {}
         self._load_wells()
         pass
     
     def __repr__(self) -> str:
@@ -288,18 +326,22 @@
     @property
     def rows_list(self) -> list[list[int]]:
         columns = self.columns_list
         return [list(z) for z in zip(*columns)]
        
     @property
     def wells(self) -> dict[str, Well]:
+        if self.order_wells_by_rows:
+            return {w:self._wells[w] for l in self.rows_list for w in l}
         return self._wells
     
     @property
     def wells_list(self) -> list[Well]:
+        if self.order_wells_by_rows:
+            return [self._wells[w] for l in self.rows_list for w in l]
         return [self._wells[well] for well in self.details.get('wells',{})]
 
     def at(self, name:str) -> Well:
         """
         Get `Well` using its name.
         Alias for `getWell()`.
```

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/logger.py` & `control-lab-ly-1.3.1/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.3.1/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/templates/library/plugins/my_plugin.py` & `control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/my_plugin.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.3.1/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.3.1/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.0b0/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.3.1/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

