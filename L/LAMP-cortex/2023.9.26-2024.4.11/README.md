# Comparing `tmp/lamp_cortex-2023.9.26.tar.gz` & `tmp/lamp_cortex-2024.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamp_cortex-2023.9.26.tar", max compression
+gzip compressed data, was "lamp_cortex-2024.4.11.tar", max compression
```

## Comparing `lamp_cortex-2023.9.26.tar` & `lamp_cortex-2024.4.11.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1544 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/LICENSE.md
--rw-r--r--   0        0        0     6652 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/README.md
--rw-r--r--   0        0        0      495 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/__init__.py
--rw-r--r--   0        0        0       71 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/__main__.py
--rw-r--r--   0        0        0    47672 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/feature_types.py
--rw-r--r--   0        0        0    17384 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/participant_ext.py
--rw-r--r--   0        0        0        0 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/primary/__init__.py
--rw-r--r--   0        0        0     3313 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/primary/acc_jerk.py
--rw-r--r--   0        0        0     5200 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/primary/game_level_scores.py
--rw-r--r--   0        0        0     5357 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/primary/screen_active.py
--rw-r--r--   0        0        0    16154 2023-09-26 18:44:11.976719 lamp_cortex-2023.9.26/cortex/primary/significant_locations.py
--rw-r--r--   0        0        0     5447 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/primary/survey_scores.py
--rw-r--r--   0        0        0     3846 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/primary/trips.py
--rw-r--r--   0        0        0        0 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/__init__.py
--rw-r--r--   0        0        0     1408 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/accelerometer.py
--rw-r--r--   0        0        0     2092 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/ambient_light.py
--rw-r--r--   0        0        0     1188 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/analytics.py
--rw-r--r--   0        0        0      983 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/balloon_risk.py
--rw-r--r--   0        0        0     1286 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/bluetooth.py
--rw-r--r--   0        0        0     1216 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/calls.py
--rw-r--r--   0        0        0     1036 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/cats_and_dogs.py
--rw-r--r--   0        0        0     3537 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/device_motion.py
--rw-r--r--   0        0        0     1632 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/device_state.py
--rw-r--r--   0        0        0     1617 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/device_usage.py
--rw-r--r--   0        0        0     1304 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/gps.py
--rw-r--r--   0        0        0     1238 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/gyroscope.py
--rw-r--r--   0        0        0     1854 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/jewels_a.py
--rw-r--r--   0        0        0     1854 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/jewels_b.py
--rw-r--r--   0        0        0     1724 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/messages_usage.py
--rw-r--r--   0        0        0     1300 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/nearby_device.py
--rw-r--r--   0        0        0     1929 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/phone_usage.py
--rw-r--r--   0        0        0     1062 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/pop_the_bubbles.py
--rw-r--r--   0        0        0     1606 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/screen_state.py
--rw-r--r--   0        0        0     1338 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/sleep.py
--rw-r--r--   0        0        0      686 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/sms.py
--rw-r--r--   0        0        0     1044 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/spatial_span.py
--rw-r--r--   0        0        0     1021 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/steps.py
--rw-r--r--   0        0        0     4512 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/survey.py
--rw-r--r--   0        0        0      710 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/telephony.py
--rw-r--r--   0        0        0     2022 2023-09-26 18:44:11.980719 lamp_cortex-2023.9.26/cortex/raw/visits.py
--rw-r--r--   0        0        0    10118 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/run.py
--rw-r--r--   0        0        0        0 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/__init__.py
--rw-r--r--   0        0        0     4016 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/app_time.py
--rw-r--r--   0        0        0     1674 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/call_degree.py
--rw-r--r--   0        0        0     2732 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/call_duration.py
--rw-r--r--   0        0        0     2197 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/call_number.py
--rw-r--r--   0        0        0     4076 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/data_quality.py
--rw-r--r--   0        0        0     1690 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/entropy.py
--rw-r--r--   0        0        0     1792 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/game_results.py
--rw-r--r--   0        0        0     1703 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/healthkit_sleep_duration.py
--rw-r--r--   0        0        0     1594 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/hometime.py
--rw-r--r--   0        0        0     7662 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/inactive_duration.py
--rw-r--r--   0        0        0     1473 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/nearby_device_count.py
--rw-r--r--   0        0        0     1916 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/screen_duration.py
--rw-r--r--   0        0        0     5794 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/step_count.py
--rw-r--r--   0        0        0     1360 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/survey_results.py
--rw-r--r--   0        0        0     1619 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/trip_distance.py
--rw-r--r--   0        0        0     1411 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/secondary/trip_duration.py
--rw-r--r--   0        0        0    10120 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/study_ext.py
--rw-r--r--   0        0        0        0 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/__init__.py
--rw-r--r--   0        0        0    12534 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/db.py
--rw-r--r--   0        0        0     1575 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/example_module_specs.json
--rw-r--r--   0        0        0    10467 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/example_modules.json
--rw-r--r--   0        0        0     1527 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/misc_functions.py
--rw-r--r--   0        0        0     8234 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/module_scheduler.py
--rw-r--r--   0        0        0     5758 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/notifications.py
--rw-r--r--   0        0        0     9435 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/utils/useful_functions.py
--rw-r--r--   0        0        0        0 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/visualizations/__init__.py
--rw-r--r--   0        0        0    13510 2023-09-26 18:44:11.984719 lamp_cortex-2023.9.26/cortex/visualizations/correlation_functions.py
--rw-r--r--   0        0        0  2385556 2023-09-26 18:44:12.008719 lamp_cortex-2023.9.26/cortex/visualizations/correlation_plots.ipynb
--rw-r--r--   0        0        0    19820 2023-09-26 18:44:12.008719 lamp_cortex-2023.9.26/cortex/visualizations/data_quality.py
--rw-r--r--   0        0        0     4137 2023-09-26 18:44:12.008719 lamp_cortex-2023.9.26/cortex/visualizations/example_scoring.json
--rw-r--r--   0        0        0    36125 2023-09-26 18:44:12.008719 lamp_cortex-2023.9.26/cortex/visualizations/participant.py
--rwxr-xr-x   0        0        0      280 2023-09-26 18:44:12.008719 lamp_cortex-2023.9.26/cortex/visualizations/run_data_quality.sh
--rw-r--r--   0        0        0     1199 2023-09-26 18:44:33.852581 lamp_cortex-2023.9.26/pyproject.toml
--rw-r--r--   0        0        0     8308 1970-01-01 00:00:00.000000 lamp_cortex-2023.9.26/PKG-INFO
+-rw-r--r--   0        0        0     1544 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/LICENSE.md
+-rw-r--r--   0        0        0     6652 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/README.md
+-rw-r--r--   0        0        0      495 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/__init__.py
+-rw-r--r--   0        0        0       71 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/__main__.py
+-rw-r--r--   0        0        0    47767 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/feature_types.py
+-rw-r--r--   0        0        0    17384 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/participant_ext.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/__init__.py
+-rw-r--r--   0        0        0     3313 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/acc_jerk.py
+-rw-r--r--   0        0        0     5200 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/game_level_scores.py
+-rw-r--r--   0        0        0     5357 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/screen_active.py
+-rw-r--r--   0        0        0    16154 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/significant_locations.py
+-rw-r--r--   0        0        0     5447 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/survey_scores.py
+-rw-r--r--   0        0        0     3846 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/primary/trips.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/__init__.py
+-rw-r--r--   0        0        0     1408 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/accelerometer.py
+-rw-r--r--   0        0        0     2092 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/ambient_light.py
+-rw-r--r--   0        0        0     1188 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/analytics.py
+-rw-r--r--   0        0        0      983 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/balloon_risk.py
+-rw-r--r--   0        0        0     1286 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/bluetooth.py
+-rw-r--r--   0        0        0     1216 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/calls.py
+-rw-r--r--   0        0        0     1036 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/cats_and_dogs.py
+-rw-r--r--   0        0        0     3537 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/device_motion.py
+-rw-r--r--   0        0        0     1632 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/device_state.py
+-rw-r--r--   0        0        0     1617 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/device_usage.py
+-rw-r--r--   0        0        0     1304 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/gps.py
+-rw-r--r--   0        0        0     1238 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/gyroscope.py
+-rw-r--r--   0        0        0     1854 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/jewels_a.py
+-rw-r--r--   0        0        0     1854 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/jewels_b.py
+-rw-r--r--   0        0        0     1724 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/messages_usage.py
+-rw-r--r--   0        0        0     1300 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/nearby_device.py
+-rw-r--r--   0        0        0     1929 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/phone_usage.py
+-rw-r--r--   0        0        0     1062 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/pop_the_bubbles.py
+-rw-r--r--   0        0        0     1606 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/screen_state.py
+-rw-r--r--   0        0        0     1338 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/sleep.py
+-rw-r--r--   0        0        0      686 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/sms.py
+-rw-r--r--   0        0        0     1044 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/spatial_span.py
+-rw-r--r--   0        0        0     1021 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/steps.py
+-rw-r--r--   0        0        0     4512 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/survey.py
+-rw-r--r--   0        0        0      710 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/telephony.py
+-rw-r--r--   0        0        0     2022 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/visits.py
+-rw-r--r--   0        0        0    10252 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/run.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/__init__.py
+-rw-r--r--   0        0        0     4016 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/app_time.py
+-rw-r--r--   0        0        0     1674 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/call_degree.py
+-rw-r--r--   0        0        0     2732 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/call_duration.py
+-rw-r--r--   0        0        0     2197 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/call_number.py
+-rw-r--r--   0        0        0     4076 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/data_quality.py
+-rw-r--r--   0        0        0     1690 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/entropy.py
+-rw-r--r--   0        0        0     1792 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/game_results.py
+-rw-r--r--   0        0        0     1703 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/healthkit_sleep_duration.py
+-rw-r--r--   0        0        0     1594 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/hometime.py
+-rw-r--r--   0        0        0     7666 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/inactive_duration.py
+-rw-r--r--   0        0        0     1473 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/nearby_device_count.py
+-rw-r--r--   0        0        0     1916 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/screen_duration.py
+-rw-r--r--   0        0        0     5794 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/step_count.py
+-rw-r--r--   0        0        0     1360 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/survey_results.py
+-rw-r--r--   0        0        0     1619 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/trip_distance.py
+-rw-r--r--   0        0        0     1411 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/trip_duration.py
+-rw-r--r--   0        0        0    10120 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/study_ext.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/__init__.py
+-rw-r--r--   0        0        0    12534 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/db.py
+-rw-r--r--   0        0        0     1575 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/example_module_specs.json
+-rw-r--r--   0        0        0    10467 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/example_modules.json
+-rw-r--r--   0        0        0     1527 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/misc_functions.py
+-rw-r--r--   0        0        0     8234 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/utils/module_scheduler.py
+-rw-r--r--   0        0        0     5758 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/utils/notifications.py
+-rw-r--r--   0        0        0     9435 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/utils/useful_functions.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/visualizations/__init__.py
+-rw-r--r--   0        0        0    13510 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/visualizations/correlation_functions.py
+-rw-r--r--   0        0        0  2385556 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/correlation_plots.ipynb
+-rw-r--r--   0        0        0    19820 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/data_quality.py
+-rw-r--r--   0        0        0     4137 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/example_scoring.json
+-rw-r--r--   0        0        0    36829 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/participant.py
+-rwxr-xr-x   0        0        0      280 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/run_data_quality.sh
+-rw-r--r--   0        0        0     1198 2024-04-11 15:37:47.822866 lamp_cortex-2024.4.11/pyproject.toml
+-rw-r--r--   0        0        0     8359 1970-01-01 00:00:00.000000 lamp_cortex-2024.4.11/PKG-INFO
```

### Comparing `lamp_cortex-2023.9.26/LICENSE.md` & `lamp_cortex-2024.4.11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/README.md` & `lamp_cortex-2024.4.11/README.md`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/feature_types.py` & `lamp_cortex-2024.4.11/cortex/feature_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -758,17 +758,19 @@
                     k: v.default
                     for k, v in signature.parameters.items()
                     if v.default is not inspect.Parameter.empty
                 }
 
             kwgs = _get_default_args(func)
             kwgs.update(kwargs)
-            timestamp_list = list(range(kwgs['start'], kwgs['end'], kwgs['resolution']))
+            n_res = int((kwgs['end'] - kwgs['start'])/kwgs['resolution'])
+            ts_list = [(kwgs['start'] + i*kwgs['resolution'], kwgs['start'] + (i+1)*kwgs['resolution'])
+                       for i in range(n_res)]
             data = []
-            for window in reversed([*zip(timestamp_list[:-1], timestamp_list[1:])]):
+            for window in reversed(ts_list):
                 window_start, window_end = window[0], window[1]
                 _result = func(**{**kwgs, 'start':window_start, 'end':window_end})
                 data.append(_result)
 
             # TODO: Require primary feature dependencies to be primary features (or raw features?)!
             data = sorted(data,key=lambda x: x['timestamp']) if data else []
             _event = {'timestamp': kwgs['start'],
```

### Comparing `lamp_cortex-2023.9.26/cortex/participant_ext.py` & `lamp_cortex-2024.4.11/cortex/participant_ext.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/primary/acc_jerk.py` & `lamp_cortex-2024.4.11/cortex/primary/acc_jerk.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/primary/game_level_scores.py` & `lamp_cortex-2024.4.11/cortex/primary/game_level_scores.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/primary/screen_active.py` & `lamp_cortex-2024.4.11/cortex/primary/screen_active.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/primary/significant_locations.py` & `lamp_cortex-2024.4.11/cortex/primary/significant_locations.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/primary/survey_scores.py` & `lamp_cortex-2024.4.11/cortex/primary/survey_scores.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/primary/trips.py` & `lamp_cortex-2024.4.11/cortex/primary/trips.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/accelerometer.py` & `lamp_cortex-2024.4.11/cortex/raw/accelerometer.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/ambient_light.py` & `lamp_cortex-2024.4.11/cortex/raw/ambient_light.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/analytics.py` & `lamp_cortex-2024.4.11/cortex/raw/analytics.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/balloon_risk.py` & `lamp_cortex-2024.4.11/cortex/raw/balloon_risk.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/bluetooth.py` & `lamp_cortex-2024.4.11/cortex/raw/bluetooth.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/calls.py` & `lamp_cortex-2024.4.11/cortex/raw/calls.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/cats_and_dogs.py` & `lamp_cortex-2024.4.11/cortex/raw/cats_and_dogs.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/device_motion.py` & `lamp_cortex-2024.4.11/cortex/raw/device_motion.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/device_state.py` & `lamp_cortex-2024.4.11/cortex/raw/device_state.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/device_usage.py` & `lamp_cortex-2024.4.11/cortex/raw/device_usage.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/gps.py` & `lamp_cortex-2024.4.11/cortex/raw/gps.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/gyroscope.py` & `lamp_cortex-2024.4.11/cortex/raw/gyroscope.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/jewels_a.py` & `lamp_cortex-2024.4.11/cortex/raw/jewels_a.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/jewels_b.py` & `lamp_cortex-2024.4.11/cortex/raw/jewels_b.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/messages_usage.py` & `lamp_cortex-2024.4.11/cortex/raw/messages_usage.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/nearby_device.py` & `lamp_cortex-2024.4.11/cortex/raw/nearby_device.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/phone_usage.py` & `lamp_cortex-2024.4.11/cortex/raw/phone_usage.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/pop_the_bubbles.py` & `lamp_cortex-2024.4.11/cortex/raw/pop_the_bubbles.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/screen_state.py` & `lamp_cortex-2024.4.11/cortex/raw/screen_state.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/sleep.py` & `lamp_cortex-2024.4.11/cortex/raw/sleep.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/sms.py` & `lamp_cortex-2024.4.11/cortex/raw/sms.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/spatial_span.py` & `lamp_cortex-2024.4.11/cortex/raw/spatial_span.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/steps.py` & `lamp_cortex-2024.4.11/cortex/raw/steps.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/survey.py` & `lamp_cortex-2024.4.11/cortex/raw/survey.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/telephony.py` & `lamp_cortex-2024.4.11/cortex/raw/telephony.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/raw/visits.py` & `lamp_cortex-2024.4.11/cortex/raw/visits.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/run.py` & `lamp_cortex-2024.4.11/cortex/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,17 @@
             params_f = {}
             if f in feature_params:
                 params_f = feature_params[f]
 
             _res = get_feature_for_participant(participant, f, params_f, start,
                                                end, resolution, cache)
 
+            if _res is None:
+                log.info("Participant has no passive data. Returning None.")
+                return None
             _res2 = pd.DataFrame.from_dict(_res['data'])
             if _res2.shape[0] > 0:
                 # If no data exists, don't bother appending the df.
                 _res2.insert(0, 'id', participant) # prepend 'id' column
                 if hasattr(primary, f):
                     _res2.timestamp = _res2.start
                 _results[f] = pd.concat([_results[f], _res2])
```

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/app_time.py` & `lamp_cortex-2024.4.11/cortex/secondary/app_time.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/call_degree.py` & `lamp_cortex-2024.4.11/cortex/secondary/call_degree.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/call_duration.py` & `lamp_cortex-2024.4.11/cortex/secondary/call_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/call_number.py` & `lamp_cortex-2024.4.11/cortex/secondary/call_number.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/data_quality.py` & `lamp_cortex-2024.4.11/cortex/secondary/data_quality.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/entropy.py` & `lamp_cortex-2024.4.11/cortex/secondary/entropy.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/game_results.py` & `lamp_cortex-2024.4.11/cortex/secondary/game_results.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/healthkit_sleep_duration.py` & `lamp_cortex-2024.4.11/cortex/secondary/healthkit_sleep_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/hometime.py` & `lamp_cortex-2024.4.11/cortex/secondary/hometime.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/inactive_duration.py` & `lamp_cortex-2024.4.11/cortex/secondary/inactive_duration.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         Args:
             df: the dataframe holding accelerometer jerk data
         Returns:
             List of tuples (start, end) of inactive periods based on acc_jerk
     """
     acc_df['above_threshold'] = acc_df['acc_jerk'] > jerk_threshold
     acc_df['prev_above'] = acc_df['above_threshold'].shift()
-    acc_df = acc_df[~acc_df['above_threshold']]
+    acc_df = acc_df[~acc_df['above_threshold']][1:]
     acc_df = acc_df[acc_df['prev_above']]
     if not acc_df.empty:
         acc_df['end'] = acc_df['start'].shift()
         acc_df = acc_df.dropna()
         tuples = [tuple(x) for x in acc_df[['end', 'start']].values]
         return tuples
     return None
```

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/nearby_device_count.py` & `lamp_cortex-2024.4.11/cortex/secondary/nearby_device_count.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/screen_duration.py` & `lamp_cortex-2024.4.11/cortex/secondary/screen_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/step_count.py` & `lamp_cortex-2024.4.11/cortex/secondary/step_count.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/survey_results.py` & `lamp_cortex-2024.4.11/cortex/secondary/survey_results.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/trip_distance.py` & `lamp_cortex-2024.4.11/cortex/secondary/trip_distance.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/secondary/trip_duration.py` & `lamp_cortex-2024.4.11/cortex/secondary/trip_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/study_ext.py` & `lamp_cortex-2024.4.11/cortex/study_ext.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/utils/db.py` & `lamp_cortex-2024.4.11/cortex/utils/db.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/utils/example_module_specs.json` & `lamp_cortex-2024.4.11/cortex/utils/example_module_specs.json`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/utils/example_modules.json` & `lamp_cortex-2024.4.11/cortex/utils/example_modules.json`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/utils/misc_functions.py` & `lamp_cortex-2024.4.11/cortex/utils/misc_functions.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/utils/module_scheduler.py` & `lamp_cortex-2024.4.11/cortex/utils/module_scheduler.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/utils/notifications.py` & `lamp_cortex-2024.4.11/cortex/utils/notifications.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/utils/useful_functions.py` & `lamp_cortex-2024.4.11/cortex/utils/useful_functions.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/visualizations/correlation_functions.py` & `lamp_cortex-2024.4.11/cortex/visualizations/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/visualizations/correlation_plots.ipynb` & `lamp_cortex-2024.4.11/cortex/visualizations/correlation_plots.ipynb`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/visualizations/data_quality.py` & `lamp_cortex-2024.4.11/cortex/visualizations/data_quality.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/visualizations/example_scoring.json` & `lamp_cortex-2024.4.11/cortex/visualizations/example_scoring.json`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2023.9.26/cortex/visualizations/participant.py` & `lamp_cortex-2024.4.11/cortex/visualizations/participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,26 +30,27 @@
     if set_to_utc_midnight:
         return shift_time(start_timestamp,0), shift_time(end_timestamp,0)
     return start_timestamp, end_timestamp
 
 def passive(id_list,
             sensor_info=[{"sensor": "lamp.gps", 'target_hz': 0.1, 'display_name': "GPS_Quality"},
             {"sensor": "lamp.accelerometer", 'target_hz': 3, 'display_name':"Accel_Quality"}],
-            show_graphs=True, attach_graphs=True, display_graphs=True,
+            show_graphs=True, attach_graphs='all', display_graphs=True,
             days_ago=0, sample_length=7,
             set_to_utc_midnight=True, reporter_func=print,
             return_dict=False, reset=False):
     """ Generates and attaches participant-level passive data quality graphs.
     Stores data from previous runs as attachments to speed up outputs.
 
         Args:
             id_list: a string or array of strings of LAMP ids
                     (participant, study, researcher)
             show_graphs: if True, graphs are displayed in the output
-            attach_graphs: if True, graphs are attached to the participant
+            attach_graphs: if True, graphs are attached to the participant. If 'heatmap', attach
+            only heatmap. If 'scatter', attach only scatterplot.
             display_graphs: if True, graphs are attached to the study and researcher for display
             days_ago: the number of days ago the analysis should end.
                         If 0, analysis ends on the current timestamp
             sample_length: The number of days to query data for
             set_to_utc_midnight: If True, timestamps are adjusted to UTC midnight
             reporter_func: The function that should output important logging info.
                         Use with a webhook, for example logging to slack
@@ -207,26 +208,38 @@
                 heatmap.display()
             (summary_dictionary[participant]
              [sensor['display_name']]['graph']['scatter'])=scatter.to_dict()
 
             (summary_dictionary[participant]
              [sensor['display_name']]['graph']['heatmap'])=heatmap.to_dict()
 
-            if attach_graphs:
-                name = f"lamp.dashboard.experimental.{sensor['display_name']}"
+            name = f"lamp.dashboard.experimental.{sensor['display_name']}"
+            if attach_graphs == 'all' or attach_graphs == True:
                 set_graph(participant,
                          key=name+'_scatter',
                          graph=scatter.to_dict(),
                          display_on_patient_portal=display_graphs,
                          set_on_parents=True)
                 set_graph(participant,
                          key=name+"_heatmap",
                          graph=heatmap.to_dict(),
                          display_on_patient_portal=display_graphs,
                          set_on_parents=True)
+            elif attach_graphs == 'scatter':
+                set_graph(participant,
+                         key=name+'_scatter',
+                         graph=scatter.to_dict(),
+                         display_on_patient_portal=display_graphs,
+                         set_on_parents=True)
+            elif attach_graphs == 'heatmap':
+                set_graph(participant,
+                         key=name+"_heatmap",
+                         graph=heatmap.to_dict(),
+                         display_on_patient_portal=display_graphs,
+                         set_on_parents=True)
 
     reporter_func("All done, bye bye!")
     if return_dict:
         return summary_dictionary
     return None
 
 def active(id_list,
```

### Comparing `lamp_cortex-2023.9.26/pyproject.toml` & `lamp_cortex-2024.4.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LAMP-cortex"
-version = "2023.09.26"
+version = "2024.4.11"
 license = "BSD-3-Clause"
 description = "The Cortex data analysis toolkit for the LAMP Platform."
 authors = ["Division of Digital Psychiatry at Beth Israel Deaconess Medical Center <team@digitalpsych.org>"]
 readme = "README.md"
 homepage = "https://docs.lamp.digital"
 documentation = "https://docs.lamp.digital"
 repository = "https://github.com/BIDMCDigitalPsychiatry/LAMP-cortex"
```

### Comparing `lamp_cortex-2023.9.26/PKG-INFO` & `lamp_cortex-2024.4.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: LAMP-cortex
-Version: 2023.9.26
+Version: 2024.4.11
 Summary: The Cortex data analysis toolkit for the LAMP Platform.
 Home-page: https://docs.lamp.digital
 License: BSD-3-Clause
 Keywords: LAMP Cortex
 Author: Division of Digital Psychiatry at Beth Israel Deaconess Medical Center
 Author-email: team@digitalpsych.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: DateTime (>=4.3,<5.0)
 Requires-Dist: LAMP-core (>=2021.5.18,<2022.0.0)
 Requires-Dist: altair (>=4.1.0,<5.0.0)
 Requires-Dist: compress-pickle (>=2.0.1,<3.0.0)
 Requires-Dist: fastdtw (>=0.3.4,<0.4.0)
 Requires-Dist: geopy (>=2.1.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
```

