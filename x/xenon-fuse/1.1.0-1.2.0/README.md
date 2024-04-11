# Comparing `tmp/xenon_fuse-1.1.0.tar.gz` & `tmp/xenon_fuse-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenon_fuse-1.1.0.tar", max compression
+gzip compressed data, was "xenon_fuse-1.2.0.tar", max compression
```

## Comparing `xenon_fuse-1.1.0.tar` & `xenon_fuse-1.2.0.tar`

### file list

```diff
@@ -1,50 +1,59 @@
--rw-r--r--   0        0        0     1536 2024-03-20 12:20:27.869819 xenon_fuse-1.1.0/LICENSE
--rw-r--r--   0        0        0     1726 2024-03-20 12:20:27.869819 xenon_fuse-1.1.0/README.md
--rw-r--r--   0        0        0      160 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/__init__.py
--rw-r--r--   0        0        0     9144 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/common.py
--rw-r--r--   0        0        0     8063 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/context.py
--rw-r--r--   0        0        0     1566 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugin.py
--rw-r--r--   0        0        0      241 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/__init__.py
--rw-r--r--   0        0        0      478 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/README.md
--rw-r--r--   0        0        0      527 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/__init__.py
--rw-r--r--   0        0        0     9317 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/csv_input.py
--rw-r--r--   0        0        0    13389 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/electron_drift.py
--rw-r--r--   0        0        0     4556 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/electron_extraction.py
--rw-r--r--   0        0        0     3161 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/electron_timing.py
--rw-r--r--   0        0        0     5471 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/s1_photon_hits.py
--rw-r--r--   0        0        0    13652 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/s1_photon_propagation.py
--rw-r--r--   0        0        0    37468 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/s2_photon_propagation.py
--rw-r--r--   0        0        0     9188 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/detector_physics/secondary_scintillation.py
--rw-r--r--   0        0        0      647 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/README.md
--rw-r--r--   0        0        0      459 2024-03-20 12:20:27.877819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/__init__.py
--rw-r--r--   0        0        0    10054 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/detector_volumes.py
--rw-r--r--   0        0        0     2317 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/electric_field.py
--rw-r--r--   0        0        0     4574 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/find_cluster.py
--rw-r--r--   0        0        0    22304 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/input.py
--rw-r--r--   0        0        0     5346 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/merge_cluster.py
--rw-r--r--   0        0        0      456 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/microphysics_summary.py
--rw-r--r--   0        0        0     4297 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/wfsim_connection.py
--rw-r--r--   0        0        0    17666 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/micro_physics/yields.py
--rw-r--r--   0        0        0      152 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/README.md
--rw-r--r--   0        0        0      251 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/__init__.py
--rw-r--r--   0        0        0     9569 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/photon_pulses.py
--rw-r--r--   0        0        0      436 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/photon_summary.py
--rw-r--r--   0        0        0     9013 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
--rw-r--r--   0        0        0    20900 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
--rw-r--r--   0        0        0      293 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/truth_information/__init__.py
--rw-r--r--   0        0        0     2789 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/truth_information/cluster_tagging.py
--rw-r--r--   0        0        0     2278 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/truth_information/event_truth.py
--rw-r--r--   0        0        0     7499 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/truth_information/peak_truth.py
--rw-r--r--   0        0        0     4754 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/truth_information/records_truth.py
--rw-r--r--   0        0        0     1544 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/plugins/truth_information/surviving_clusters.py
--rw-r--r--   0        0        0      895 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/vertical_merger_plugin.py
--rw-r--r--   0        0        0     1041 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/fuse/volume_plugin.py
--rw-r--r--   0        0        0     1169 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      823 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/tests/_utils.py
--rw-r--r--   0        0        0     1770 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/tests/test_DetectorPhysics_csv.py
--rw-r--r--   0        0        0     3299 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/tests/test_FullChain.py
--rw-r--r--   0        0        0     2490 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/tests/test_MicroPhysics.py
--rw-r--r--   0        0        0     4560 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/tests/test_deterministic_seed.py
--rw-r--r--   0        0        0     7827 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/tests/test_input.py
--rw-r--r--   0        0        0     4775 2024-03-20 12:20:27.881819 xenon_fuse-1.1.0/tests/test_plugin_versions_in_doc.py
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 xenon_fuse-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1536 2024-04-11 16:49:58.763337 xenon_fuse-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1726 2024-04-11 16:49:58.763337 xenon_fuse-1.2.0/README.md
+-rw-r--r--   0        0        0      160 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/__init__.py
+-rw-r--r--   0        0        0     9142 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/common.py
+-rw-r--r--   0        0        0     9554 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/context.py
+-rw-r--r--   0        0        0     2639 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugin.py
+-rw-r--r--   0        0        0      241 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/README.md
+-rw-r--r--   0        0        0      593 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/__init__.py
+-rw-r--r--   0        0        0     9196 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/csv_input.py
+-rw-r--r--   0        0        0      615 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py
+-rw-r--r--   0        0        0      803 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py
+-rw-r--r--   0        0        0     2550 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py
+-rw-r--r--   0        0        0      974 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py
+-rw-r--r--   0        0        0     2017 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py
+-rw-r--r--   0        0        0      837 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py
+-rw-r--r--   0        0        0     8539 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py
+-rw-r--r--   0        0        0    14746 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_drift.py
+-rw-r--r--   0        0        0     4556 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_extraction.py
+-rw-r--r--   0        0        0     3121 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_timing.py
+-rw-r--r--   0        0        0     5471 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_hits.py
+-rw-r--r--   0        0        0    13699 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_propagation.py
+-rw-r--r--   0        0        0    35274 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/s2_photon_propagation.py
+-rw-r--r--   0        0        0     9188 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/secondary_scintillation.py
+-rw-r--r--   0        0        0      647 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/README.md
+-rw-r--r--   0        0        0      459 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/__init__.py
+-rw-r--r--   0        0        0    10138 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/detector_volumes.py
+-rw-r--r--   0        0        0     2314 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/electric_field.py
+-rw-r--r--   0        0        0     4574 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/find_cluster.py
+-rw-r--r--   0        0        0    22316 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/input.py
+-rw-r--r--   0        0        0     5342 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/merge_cluster.py
+-rw-r--r--   0        0        0      456 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/microphysics_summary.py
+-rw-r--r--   0        0        0     4295 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/wfsim_connection.py
+-rw-r--r--   0        0        0    17709 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/yields.py
+-rw-r--r--   0        0        0      152 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/README.md
+-rw-r--r--   0        0        0      251 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/__init__.py
+-rw-r--r--   0        0        0     9569 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/photon_pulses.py
+-rw-r--r--   0        0        0      436 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/photon_summary.py
+-rw-r--r--   0        0        0     9013 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
+-rw-r--r--   0        0        0    20113 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
+-rw-r--r--   0        0        0      293 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/__init__.py
+-rw-r--r--   0        0        0     2789 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/cluster_tagging.py
+-rw-r--r--   0        0        0     2278 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/event_truth.py
+-rw-r--r--   0        0        0     8349 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/peak_truth.py
+-rw-r--r--   0        0        0     4754 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/records_truth.py
+-rw-r--r--   0        0        0     1543 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/surviving_clusters.py
+-rw-r--r--   0        0        0      895 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/vertical_merger_plugin.py
+-rw-r--r--   0        0        0     1041 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/volume_plugin.py
+-rw-r--r--   0        0        0     1169 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      823 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/_utils.py
+-rw-r--r--   0        0        0     1770 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_DetectorPhysics_csv.py
+-rw-r--r--   0        0        0     3299 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_FullChain.py
+-rw-r--r--   0        0        0     4900 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_FullChain_w_DelayedElectrons.py
+-rw-r--r--   0        0        0     2490 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_MicroPhysics.py
+-rw-r--r--   0        0        0     4560 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_deterministic_seed.py
+-rw-r--r--   0        0        0     7827 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_input.py
+-rw-r--r--   0        0        0     5000 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_plugin_random_seed.py
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 xenon_fuse-1.2.0/PKG-INFO
```

### Comparing `xenon_fuse-1.1.0/LICENSE` & `xenon_fuse-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/README.md` & `xenon_fuse-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/fuse/common.py` & `xenon_fuse-1.2.0/fuse/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,17 @@
     clusters = [0]
     c = 0
     n_cluster = 0
     for value in diff:
         if value <= scale:
             clusters.append(c)
             n_cluster += 1
-
         elif n_cluster + 1 < n_min:
             clusters.append(c)
             n_cluster += 1
-
         elif value > scale:
             c = c + 1
             clusters.append(c)
             n_cluster = 0
 
     clusters = np.array(clusters)
     clusters_undo_sort = clusters[idx_undo_sort]
```

### Comparing `xenon_fuse-1.1.0/fuse/context.py` & `xenon_fuse-1.2.0/fuse/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,35 @@
     fuse.detector_physics.ElectronDrift,
     fuse.detector_physics.ElectronExtraction,
     fuse.detector_physics.ElectronTiming,
     fuse.detector_physics.SecondaryScintillation,
     fuse.detector_physics.S2PhotonPropagation,
 ]
 
+# Plugins to simulate delayed electrons
+delayed_electron_simulation_plugins = [
+    fuse.detector_physics.delayed_electrons.PhotoIonizationElectrons,
+    fuse.detector_physics.delayed_electrons.DelayedElectronsDrift,
+    fuse.detector_physics.delayed_electrons.DelayedElectronsExtraction,
+    fuse.detector_physics.delayed_electrons.DelayedElectronsTiming,
+    fuse.detector_physics.delayed_electrons.DelayedElectronsSecondaryScintillation,
+    fuse.detector_physics.delayed_electrons.S1PhotonHitsEmpty,
+]
+
+# Plugins to merge delayed and regular electrons
+delayed_electron_merger_plugins = [
+    fuse.detector_physics.delayed_electrons.DriftedElectronsMerger,
+    fuse.detector_physics.delayed_electrons.ExtractedElectronsMerger,
+    fuse.detector_physics.delayed_electrons.ElectronTimingMerger,
+    fuse.detector_physics.delayed_electrons.SecondaryScintillationPhotonsMerger,
+    fuse.detector_physics.delayed_electrons.SecondaryScintillationPhotonSumMerger,
+    fuse.detector_physics.delayed_electrons.MicrophysicsSummaryMerger,
+    fuse.detector_physics.delayed_electrons.S1PhotonHitsMerger,
+]
+
 # Plugins to simulate PMTs and DAQ
 pmt_and_daq_plugins = [
     fuse.pmt_and_daq.PMTAfterPulses,
     fuse.pmt_and_daq.PhotonSummary,
     fuse.pmt_and_daq.PulseWindow,
     fuse.pmt_and_daq.PMTResponseAndDAQ,
 ]
@@ -134,14 +155,22 @@
     for plugin in s1_simulation_plugins:
         st.register(plugin)
 
     # Register S2 plugins
     for plugin in s2_simulation_plugins:
         st.register(plugin)
 
+    # Register delayed Electrons plugins
+    for plugin in delayed_electron_simulation_plugins:
+        st.register(plugin)
+
+    # Register merger plugins.
+    for plugin in delayed_electron_merger_plugins:
+        st.register(plugin)
+
     # Register PMT and DAQ plugins
     for plugin in pmt_and_daq_plugins:
         st.register(plugin)
 
     # Register truth plugins
     for plugin in truth_information_plugins:
         st.register(plugin)
@@ -179,18 +208,21 @@
 def set_simulation_config_file(context, config_file_name):
     """Function to loop over the plugin config and replace
     SIMULATION_CONFIG_FILE with the actual file name."""
     for data_type, plugin in context._plugin_class_registry.items():
         for option_key, option in plugin.takes_config.items():
             if isinstance(option.default, str) and "SIMULATION_CONFIG_FILE.json" in option.default:
                 context.config[option_key] = option.default.replace(
-                    "SIMULATION_CONFIG_FILE.json",
-                    config_file_name,
+                    "SIMULATION_CONFIG_FILE.json", config_file_name
                 )
 
+            # Special case for the photoionization_modifier
+            if option_key == "photoionization_modifier":
+                context.config[option_key] = option.default
+
 
 @URLConfig.register("pattern_map")
 def pattern_map(map_data, pmt_mask, method="WeightedNearestNeighbors"):
     """Pattern map handling."""
 
     if "compressed" in map_data:
         compressor, dtype, shape = map_data["compressed"]
```

### Comparing `xenon_fuse-1.1.0/fuse/plugin.py` & `xenon_fuse-1.2.0/fuse/plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,47 +8,74 @@
 
 class FuseBasePlugin(strax.Plugin):
     """Base plugin for fuse plugins."""
 
     # Forbid rechunking
     rechunk_on_save = False
 
-    # Lets wait 10 minutes for the plugin to finish
-    input_timeout = 600
+    # Lets wait 15 minutes for the plugin to finish.. PI takes a while to run
+    input_timeout = 900
 
     # Config options
     debug = straxen.URLConfig(
         default=False,
         type=bool,
         track=False,
         help="Show debug informations",
     )
 
     deterministic_seed = straxen.URLConfig(
         default=True,
         type=bool,
-        help="Set the random seed from lineage and run_id, or pull the seed from the OS.",
+        help="Set the random seed from lineage and run_id, or pull the seed from the OS",
+    )
+
+    user_defined_random_seed = straxen.URLConfig(
+        default=None,
+        help="Define the random seed manually. You need to set deterministic_seed to False",
     )
 
     def setup(self):
         super().setup()
 
         log = logging.getLogger(f"{self.__class__.__name__}")
 
         if self.debug:
             log.setLevel("DEBUG")
             log.debug(f"Running {self.__class__.__name__} version {self.__version__} in debug mode")
         else:
             log.setLevel("INFO")
 
         if self.deterministic_seed:
+
+            if self.user_defined_random_seed is not None:
+                log.warning(
+                    "deterministic_seed is set to True. "
+                    "The provided user_defined_random_seed will not be used!"
+                )
+
             hash_string = strax.deterministic_hash((self.run_id, self.lineage))
             self.seed = int(hash_string.encode().hex(), 16)
             self.rng = np.random.default_rng(seed=self.seed)
-            log.debug(f"Generating random numbers from seed {self.seed}")
+            log.debug(f"Generating random numbers from deterministic seed {self.seed}")
         else:
-            self.rng = np.random.default_rng()
-            log.debug("Generating random numbers with seed pulled from OS")
+
+            if self.user_defined_random_seed is not None:
+
+                assert (
+                    isinstance(self.user_defined_random_seed, int)
+                    and self.user_defined_random_seed > 0
+                ), "user_defined_random_seed must be a positive integer!"
+
+                self.seed = self.user_defined_random_seed
+                self.rng = np.random.default_rng(self.user_defined_random_seed)
+                log.info(
+                    "Generating random numbers with user"
+                    f"defined seed {self.user_defined_random_seed}"
+                )
+            else:
+                self.rng = np.random.default_rng()
+                log.debug("Generating random numbers with seed pulled from OS")
 
 
 class FuseBaseDownChunkingPlugin(strax.DownChunkingPlugin, FuseBasePlugin):
     """Base plugin for fuse DownChunkingPlugins."""
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/__init__.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 from .s2_photon_propagation import *
 
 from . import secondary_scintillation
 from .secondary_scintillation import *
 
 from . import csv_input
 from .csv_input import *
+
+from . import delayed_electrons
+from .delayed_electrons import *
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/csv_input.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/csv_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,65 +16,57 @@
 
 
 @export
 class ChunkCsvInput(FuseBasePlugin):
     """Plugin which reads a CSV file containing instructions for the detector
     physics simulation and returns the data in chunks."""
 
-    __version__ = "0.2.0"
+    __version__ = "0.2.1"
 
     depends_on: Tuple = tuple()
     provides = "microphysics_summary"
     data_kind = "interactions_in_roi"
 
     save_when = strax.SaveWhen.TARGET
 
     source_done = False
 
     dtype = [
         (("x position of the cluster [cm]", "x"), np.float32),
         (("y position of the cluster [cm]", "y"), np.float32),
         (("z position of the cluster [cm]", "z"), np.float32),
-        (("Number of photons at interaction position.", "photons"), np.int32),
-        (("Number of electrons at interaction position.", "electrons"), np.int32),
-        (("Number of excitons at interaction position.", "excitons"), np.int32),
+        (("Number of photons at interaction position", "photons"), np.int32),
+        (("Number of electrons at interaction position", "electrons"), np.int32),
+        (("Number of excitons at interaction position", "excitons"), np.int32),
         (("Electric field value at the cluster position [V/cm]", "e_field"), np.float32),
         (("Energy of the cluster [keV]", "ed"), np.float32),
         (("NEST interaction type", "nestid"), np.int8),
         (("ID of the cluster", "cluster_id"), np.int32),
-        (
-            ("Time of the interaction [ns]", "t"),
-            np.int64,
-        ),  # Remove them later as they are not in the usual micropyhsics summary
-        (
-            ("Geant4 event ID", "eventid"),
-            np.int32,
-        ),  # Remove them later as they are not in the usual micropyhsics summary
     ]
     dtype = dtype + strax.time_fields
 
     # Config options
     input_file = straxen.URLConfig(
         track=False,
         infer_type=False,
         help="CSV file to read",
     )
 
     separation_scale = straxen.URLConfig(
         default=1e8,
         type=(int, float),
-        help="separation_scale",
+        help="Start a new chunk when the previous cluster is separated by this time scale",
     )
 
     source_rate = straxen.URLConfig(
         default=1,
         type=(int, float),
-        help="Source rate used to generate event times"
-        "Use a value >0 to generate event times in fuse"
-        "Use source_rate = 0 to use event times from the input file (only for csv input)",
+        help="Source rate used to generate event times. "
+        "Use a value >0 to generate event times in fuse. "
+        "Use source_rate = 0 to use event times from the input file (only for csv input).",
     )
 
     n_interactions_per_chunk = straxen.URLConfig(
         default=1e5,
         type=(int, float),
         help="n_interactions_per_chunk",
     )
@@ -92,19 +84,21 @@
         )
         self.file_reader_iterator = self.file_reader.output_chunk()
 
     def compute(self):
         try:
             chunk_data, chunk_left, chunk_right, source_done = next(self.file_reader_iterator)
             chunk_data["endtime"] = chunk_data["time"]
+            data = np.zeros(len(chunk_data), dtype=self.dtype)
+            strax.copy_to_buffer(chunk_data, data, "_bring_data_into_correct_format")
 
             self.source_done = source_done
 
             return self.chunk(
-                start=chunk_left, end=chunk_right, data=chunk_data, data_type="geant4_interactions"
+                start=chunk_left, end=chunk_right, data=data, data_type="geant4_interactions"
             )
 
         except StopIteration:
             raise RuntimeError("Bug in chunk building!")
 
     def source_finished(self):
         return self.source_done
@@ -146,17 +140,17 @@
         self.first_chunk_left = np.int64(first_chunk_left)
         self.debug = debug
 
         self.dtype = [
             (("x position of the cluster [cm]", "x"), np.float32),
             (("y position of the cluster [cm]", "y"), np.float32),
             (("z position of the cluster [cm]", "z"), np.float32),
-            (("Number of photons at interaction position.", "photons"), np.int32),
-            (("Number of electrons at interaction position.", "electrons"), np.int32),
-            (("Number of excitons at interaction position.", "excitons"), np.int32),
+            (("Number of photons at interaction position", "photons"), np.int32),
+            (("Number of electrons at interaction position", "electrons"), np.int32),
+            (("Number of excitons at interaction position", "excitons"), np.int32),
             (("Electric field value at the cluster position [V/cm]", "e_field"), np.float32),
             (("Energy of the cluster [keV]", "ed"), np.float32),
             (("NEST interaction type", "nestid"), np.int8),
             (("ID of the cluster", "cluster_id"), np.int32),
             (
                 ("Time of the interaction", "t"),
                 np.int64,
@@ -221,15 +215,15 @@
 
         if (len(chunk_start) > 1) & (len(chunk_end) > 1):
             gap_length = chunk_start[1:] - chunk_end[:-1]
             gap_length = np.append(gap_length, gap_length[-1] + self.last_chunk_length)
             chunk_bounds = chunk_end + np.int64(self.chunk_delay_fraction * gap_length)
             self.chunk_bounds = np.append(chunk_start[0] - self.first_chunk_left, chunk_bounds)
         else:
-            log.warning("Only one Chunk! Rate to high?")
+            log.warning("Only one Chunk! Rate too high?")
             self.chunk_bounds = [
                 chunk_start[0] - self.first_chunk_left,
                 chunk_end[0] + self.last_chunk_length,
             ]
 
         source_done = False
         unique_chunk_index_values = np.unique(chunk_idx)
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/electron_drift.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_drift.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import logging
-
-import numpy as np
 import strax
 import straxen
+import logging
+import numpy as np
 
 from ...plugin import FuseBasePlugin
 
 export, __all__ = strax.exporter()
 
 logging.basicConfig(handlers=[logging.StreamHandler()])
 log = logging.getLogger("fuse.detector_physics.electron_drift")
@@ -18,15 +17,15 @@
     the liquid gas interface.
 
     The plugin simulates the effect of a charge insensitive volume and
     the loss of electrons due to impurities. Additionally, the drift
     time and observed position is calculated.
     """
 
-    __version__ = "0.2.0"
+    __version__ = "0.3.0"
 
     depends_on = "microphysics_summary"
     provides = "drifted_electrons"
     data_kind = "interactions_in_roi"
 
     dtype = [
         (
@@ -164,14 +163,32 @@
         "&key=field_distortion_comsol_map"
         "&fmt=json.gz"
         "&method=WeightedNearestNeighbors",
         cache=True,
         help="Field distortion map used in fuse (Check if we can remove _fuse from the name)",
     )
 
+    gate_to_anode_distance = straxen.URLConfig(
+        default="take://resource://"
+        "SIMULATION_CONFIG_FILE.json?"
+        "&fmt=json"
+        "&take=gate_to_anode_distance",
+        cache=True,
+        help="Distance between the liquid surface and anode in cm",
+    )
+
+    elr_gas_gap_length = straxen.URLConfig(
+        default="take://resource://"
+        "SIMULATION_CONFIG_FILE.json?"
+        "&fmt=json"
+        "&take=elr_gas_gap_length",
+        cache=True,
+        help="Distance between the gate and anode in cm",
+    )
+
     def setup(self):
         super().setup()
 
         # Can this be done via URL config?
         if self.field_distortion_model == "inverse_fdc":
             self.fdc_map_fuse.scale_coordinates([1.0, 1.0, -self.drift_velocity_liquid])
 
@@ -238,19 +255,25 @@
         n_electron = self.rng.binomial(n=n_electron, p=interaction_in_civ)
 
         # Absorb electrons during the drift
         # Average drift time of the electrons
         drift_time_mean, drift_time_spread = self.get_s2_drift_time_params(
             xy_int=np.array([x, y]).T, z_int=z
         )
-        electron_lifetime_correction = np.exp(-1 * drift_time_mean / self.electron_lifetime_liquid)
 
-        n_electron = self.rng.binomial(
-            n=n_electron.astype(np.int32), p=electron_lifetime_correction
-        )
+        if self.electron_lifetime_liquid > 0:
+            electron_lifetime_correction = np.exp(
+                -1 * drift_time_mean / self.electron_lifetime_liquid
+            )
+
+            n_electron = self.rng.binomial(
+                n=n_electron.astype(np.int32), p=electron_lifetime_correction
+            )
+        else:
+            log.debug("No electron lifetime applied")
 
         result = np.zeros(len(interactions_in_roi), dtype=self.dtype)
         result["time"] = interactions_in_roi["time"]
         result["endtime"] = interactions_in_roi["endtime"]
         result["n_electron_interface"][mask] = n_electron
         result["drift_time_mean"][mask] = drift_time_mean
         result["drift_time_spread"][mask] = drift_time_spread
@@ -323,26 +346,46 @@
 
         Args:
             z_int: 1d array of true z (floats)
             xy_int: 2d array of true xy positions (floats)
         Returns:
             returns two arrays of floats (mean drift time, drift time spread)
         """
-        drift_velocity_liquid = self.get_avg_drift_velocity(z_int, xy_int)
+        liquid_level = self.gate_to_anode_distance - self.elr_gas_gap_length
+        drift_velocity_below_gate = self.get_avg_drift_velocity(z_int, xy_int)
+        drift_velocity_above_gate = liquid_level / self.drift_time_gate
         if self.enable_diffusion_longitudinal_map:
             diffusion_constant_longitudinal = self.diffusion_longitudinal_map(
                 z_int, xy_int
             )  # cm²/ns
         else:
             diffusion_constant_longitudinal = self.diffusion_constant_longitudinal
 
-        drift_time_mean = -z_int / drift_velocity_liquid + self.drift_time_gate
+        drift_time_below_gate = -z_int / drift_velocity_below_gate
+        drift_time_above_gate = self.drift_time_gate
+
+        drift_time_mean = drift_time_below_gate + drift_time_above_gate
         drift_time_mean = np.clip(drift_time_mean, 0, np.inf)
-        drift_time_spread = np.sqrt(2 * diffusion_constant_longitudinal * drift_time_mean)
-        drift_time_spread /= drift_velocity_liquid
+
+        drift_time_spread_below_gate_squared = (
+            2
+            * diffusion_constant_longitudinal
+            * drift_time_below_gate
+            / drift_velocity_below_gate**2
+        )
+        drift_time_spread_above_gate_squared = (
+            2
+            * diffusion_constant_longitudinal
+            * drift_time_above_gate
+            / drift_velocity_above_gate**2
+        )
+        drift_time_spread = np.sqrt(
+            drift_time_spread_below_gate_squared + drift_time_spread_above_gate_squared
+        )
+
         return drift_time_mean, drift_time_spread
 
     def get_avg_drift_velocity(self, z, xy):
         """Calculate s2 drift time mean and spread
         Args:
             z: 1d array of z (floats)
             xy: 2d array of xy positions (floats)
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/electron_extraction.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_extraction.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/electron_timing.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,22 @@
     """Plugin to simulate the arrival times of electrons extracted from the
     liquid phase.
 
     It includes both the drift time and the time needed for the
     extraction.
     """
 
-    __version__ = "0.2.0"
+    __version__ = "0.2.1"
 
-    depends_on = ("drifted_electrons", "extracted_electrons", "microphysics_summary")
+    depends_on = ("microphysics_summary", "drifted_electrons", "extracted_electrons")
     provides = "electron_time"
     data_kind = "individual_electrons"
 
     save_when = strax.SaveWhen.TARGET
 
-    data_kind = "individual_electrons"
-
     dtype = [
         (("x position of the electron [cm]", "x"), np.float32),
         (("y position of the electron [cm]", "y"), np.float32),
         (("ID of the cluster creating the electron", "cluster_id"), np.int32),
     ]
     dtype = dtype + strax.time_fields
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/s1_photon_hits.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_hits.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/s1_photon_propagation.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_propagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     """Base plugin to simulate the propagation of S1 photons in the detector.
     Photons are randomly assigned to PMT channels based on their starting
     position and the timing of the photons is calculated.
 
     Note: The timing calculation is defined in the child plugin.
     """
 
-    __version__ = "0.3.0"
+    __version__ = "0.3.1"
 
-    depends_on = ("s1_photons", "microphysics_summary")
+    depends_on = ("microphysics_summary", "s1_photons")
     provides = "propagated_s1_photons"
-    data_kind = "S1_photons"
+    data_kind = "s1_photons"
 
     save_when = strax.SaveWhen.TARGET
 
     dtype = [
         (("PMT channel of the photon", "channel"), np.int16),
         (("Photon creates a double photo-electron emission", "dpe"), np.bool_),
         (("Sampled PMT gain for the photon", "photon_gain"), np.int32),
@@ -136,15 +136,15 @@
         cache=True,
         help="S1 pattern map",
     )
 
     def setup(self):
         super().setup()
 
-        if self.deterministic_seed:
+        if self.deterministic_seed or (self.user_defined_random_seed is not None):
             # Dont know but nestpy seems to have a problem with large seeds
             self.short_seed = int(repr(self.seed)[-8:])
             log.debug(f"Generating nestpy random numbers from seed {self.short_seed}")
         else:
             log.debug("Generating random numbers with seed pulled from OS")
 
         self.gains = pmt_gains(
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/s2_photon_propagation.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/s2_photon_propagation.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,27 @@
     """Base plugin to simulate the propagation of S2 photons in the detector.
     Photons are randomly assigned to PMT channels based on their starting
     position and the timing of the photons is calculated.
 
     Note: The timing calculation is defined in the child plugin.
     """
 
-    __version__ = "0.3.1"
+    __version__ = "0.3.3"
 
     depends_on = (
-        "electron_time",
-        "s2_photons",
-        "extracted_electrons",
-        "drifted_electrons",
-        "s2_photons_sum",
-        "microphysics_summary",
+        "merged_electron_time",
+        "merged_s2_photons",
+        "merged_extracted_electrons",
+        "merged_drifted_electrons",
+        "merged_s2_photons_sum",
+        "merged_microphysics_summary",
     )
+
     provides = "propagated_s2_photons"
-    data_kind = "S2_photons"
+    data_kind = "s2_photons"
 
     save_when = strax.SaveWhen.TARGET
 
     dtype = [
         (("PMT channel of the photon", "channel"), np.int16),
         (("Photon creates a double photo-electron emission", "dpe"), np.bool_),
         (("Sampled PMT gain for the photon", "photon_gain"), np.int32),
@@ -314,15 +315,15 @@
 
             def rz_map(z, xy, **kwargs):
                 r = np.sqrt(xy[:, 0] ** 2 + xy[:, 1] ** 2)
                 return self.field_dependencies_map_tmp(np.array([r, z]).T, **kwargs)
 
             self.field_dependencies_map = rz_map
 
-    def compute(self, individual_electrons, interactions_in_roi, start, end):
+    def compute(self, interactions_in_roi, individual_electrons, start, end):
         # Just apply this to clusters with photons
         mask = interactions_in_roi["n_electron_extracted"] > 0
 
         if len(individual_electrons) == 0:
             yield self.chunk(start=start, end=end, data=np.zeros(0, dtype=self.dtype))
             return
 
@@ -343,94 +344,40 @@
         n_chunks = len(electron_chunks)
         if n_chunks > 1:
             log.info("Chunk size exceeding file size target. " f"Downchunking to {n_chunks} chunks")
 
         last_start = start
         if n_chunks > 1:
             for electron_group in electron_chunks[:-1]:
-                unique_clusters_in_group = np.unique(electron_group["cluster_id"])
-                interactions_chunk = interactions_in_roi[mask][
-                    np.isin(interactions_in_roi["cluster_id"][mask], unique_clusters_in_group)
-                ]
-
-                # Sort both the interactions and the electrons by cluster_id
-                # We will later sort by time again when yielding the data.
-                sort_index_ic = np.argsort(interactions_chunk["cluster_id"])
-                sort_index_eg = np.argsort(electron_group["cluster_id"])
-                interactions_chunk = interactions_chunk[sort_index_ic]
-                electron_group = electron_group[sort_index_eg]
-
-                positions = np.array([interactions_chunk["x_obs"], interactions_chunk["y_obs"]]).T
-
-                _photon_channels = self.photon_channels(
-                    interactions_chunk["n_electron_extracted"],
-                    interactions_chunk["z_obs"],
-                    positions,
-                    interactions_chunk["drift_time_mean"],
-                    interactions_chunk["sum_s2_photons"],
-                )
-
-                _photon_timings = self.photon_timings(
-                    positions,
-                    interactions_chunk["sum_s2_photons"],
-                    _photon_channels,
-                ).astype(np.int64)
-
-                # Repeat for n photons per electron # Should this be before adding delays?
-                _photon_timings += np.repeat(electron_group["time"], electron_group["n_s2_photons"])
-
-                _cluster_id = np.repeat(
-                    interactions_chunk["cluster_id"], interactions_chunk["sum_s2_photons"]
-                )
-
-                # Do i want to save both -> timings with and without pmt transit time spread?
-                # Correct for PMT Transit Time Spread
-                _photon_timings = pmt_transit_time_spread(
-                    _photon_timings=_photon_timings,
-                    pmt_transit_time_mean=self.pmt_transit_time_mean,
-                    pmt_transit_time_spread=self.pmt_transit_time_spread,
-                    rng=self.rng,
-                )
-
-                _photon_gains, _photon_is_dpe = photon_gain_calculation(
-                    _photon_channels=_photon_channels,
-                    p_double_pe_emision=self.p_double_pe_emision,
-                    gains=self.gains,
-                    spe_scaling_factor_distributions=self.spe_scaling_factor_distributions,
-                    rng=self.rng,
-                )
-
-                result = build_photon_propagation_output(
-                    dtype=self.dtype,
-                    _photon_timings=_photon_timings,
-                    _photon_channels=_photon_channels,
-                    _photon_gains=_photon_gains,
-                    _photon_is_dpe=_photon_is_dpe,
-                    _cluster_id=_cluster_id,
-                    photon_type=2,
-                )
-
-                result = strax.sort_by_time(result)
+                result = self.compute_chunk(interactions_in_roi, mask, electron_group)
 
                 # Move the chunk bound 90% of the minimal gap length to
                 # the next photon to make space for afterpluses
                 chunk_end = np.max(strax.endtime(result)) + np.int64(
                     self.min_electron_gap_length_for_splitting * 0.9
                 )
                 chunk = self.chunk(start=last_start, end=chunk_end, data=result)
                 last_start = chunk_end
                 yield chunk
 
         # And the last chunk
         electron_group = electron_chunks[-1]
+        result = self.compute_chunk(interactions_in_roi, mask, electron_group)
+
+        chunk = self.chunk(start=last_start, end=end, data=result)
+        yield chunk
+
+    def compute_chunk(self, interactions_in_roi, mask, electron_group):
         unique_clusters_in_group = np.unique(electron_group["cluster_id"])
         interactions_chunk = interactions_in_roi[mask][
             np.isin(interactions_in_roi["cluster_id"][mask], unique_clusters_in_group)
         ]
 
+        # Sort both the interactions and the electrons by cluster_id
+        # We will later sort by time again when yielding the data.
         sort_index_ic = np.argsort(interactions_chunk["cluster_id"])
         sort_index_eg = np.argsort(electron_group["cluster_id"])
         interactions_chunk = interactions_chunk[sort_index_ic]
         electron_group = electron_group[sort_index_eg]
 
         positions = np.array([interactions_chunk["x_obs"], interactions_chunk["y_obs"]]).T
 
@@ -444,20 +391,23 @@
 
         _photon_timings = self.photon_timings(
             positions,
             interactions_chunk["sum_s2_photons"],
             _photon_channels,
         ).astype(np.int64)
 
+        # Repeat for n photons per electron # Should this be before adding delays?
         _photon_timings += np.repeat(electron_group["time"], electron_group["n_s2_photons"])
 
         _cluster_id = np.repeat(
             interactions_chunk["cluster_id"], interactions_chunk["sum_s2_photons"]
         )
 
+        # Do i want to save both -> timings with and without pmt transit time spread?
+        # Correct for PMT Transit Time Spread
         _photon_timings = pmt_transit_time_spread(
             _photon_timings=_photon_timings,
             pmt_transit_time_mean=self.pmt_transit_time_mean,
             pmt_transit_time_spread=self.pmt_transit_time_spread,
             rng=self.rng,
         )
 
@@ -477,16 +427,15 @@
             _photon_is_dpe=_photon_is_dpe,
             _cluster_id=_cluster_id,
             photon_type=2,
         )
 
         result = strax.sort_by_time(result)
 
-        chunk = self.chunk(start=last_start, end=end, data=result)
-        yield chunk
+        return result
 
     def photon_channels(self, n_electron, z_obs, positions, drift_time_mean, n_photons):
         channels = np.arange(self.n_tpc_pmts).astype(np.int64)
         top_index = np.arange(self.n_top_pmts)
         bottom_index = np.arange(self.n_top_pmts, self.n_tpc_pmts)
 
         if self.diffusion_constant_transverse > 0:
@@ -737,22 +686,22 @@
 
     child_plugin = True
 
     pressure = straxen.URLConfig(
         default="take://resource://SIMULATION_CONFIG_FILE.json?&fmt=json&take=pressure",
         type=(int, float),
         cache=True,
-        help="pressure",
+        help="Pressure of liquid xenon [bar/e], while e is the elementary charge",
     )
 
     temperature = straxen.URLConfig(
         default="take://resource://SIMULATION_CONFIG_FILE.json?&fmt=json&take=temperature",
         type=(int, float),
         cache=True,
-        help="temperature",
+        help="Temperature of liquid xenon [K]",
     )
 
     gas_drift_velocity_slope = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=gas_drift_velocity_slope",
         type=(int, float),
@@ -807,22 +756,22 @@
 
     gate_to_anode_distance = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=gate_to_anode_distance",
         type=(int, float),
         cache=True,
-        help="gate_to_anode_distance",
+        help="Top of gate to bottom of anode (not considering perpendicular wires) [cm]",
     )
 
     anode_voltage = straxen.URLConfig(
         default="take://resource://SIMULATION_CONFIG_FILE.json?&fmt=json&take=anode_voltage",
         type=(int, float),
         cache=True,
-        help="anode_voltage",
+        help="Voltage of anode [V]",
     )
 
     lxe_dielectric_constant = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=lxe_dielectric_constant",
         type=(int, float),
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/detector_physics/secondary_scintillation.py` & `xenon_fuse-1.2.0/fuse/plugins/detector_physics/secondary_scintillation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 
     __version__ = "0.2.0"
 
     result_name_photons = "s2_photons"
     result_name_photons_sum = "s2_photons_sum"
 
     depends_on = (
+        "microphysics_summary",
         "drifted_electrons",
         "extracted_electrons",
         "electron_time",
-        "microphysics_summary",
     )
     provides = (result_name_photons, result_name_photons_sum)
     data_kind = {
         result_name_photons: "individual_electrons",
         result_name_photons_sum: "interactions_in_roi",
     }
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/README.md` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/README.md`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/detector_volumes.py` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/detector_volumes.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     to ``True``.
     """
 
     depends_on = "clustered_interactions"
 
     provides = "tpc_interactions"
     data_kind = "tpc_interactions"
-    __version__ = "0.3.0"
+    __version__ = "0.3.1"
 
     # Can we import this from MergeCluster and just add the needed fields?
     dtype = [
         (("x position of the cluster [cm]", "x"), np.float32),
         (("y position of the cluster [cm]", "y"), np.float32),
         (("z position of the cluster [cm]", "z"), np.float32),
         (("Energy of the cluster [keV]", "ed"), np.float32),
@@ -53,17 +53,17 @@
         (("Mass number of the interacting particle", "A"), np.int8),
         (("Charge number of the interacting particle", "Z"), np.int8),
         (("Geant4 event ID", "evtid"), np.int32),
         (("x position of the primary particle [cm]", "x_pri"), np.float32),
         (("y position of the primary particle [cm]", "y_pri"), np.float32),
         (("z position of the primary particle [cm]", "z_pri"), np.float32),
         (("ID of the cluster", "cluster_id"), np.int32),
-        (("Xenon density at the cluster position.", "xe_density"), np.float32),
-        (("ID of the volume in which the cluster occured.", "vol_id"), np.int8),
-        (("Flag indicating if a cluster can create a S2 signal.", "create_S2"), np.bool_),
+        (("Xenon density at the cluster position", "xe_density"), np.float32),
+        (("ID of the volume in which the cluster occured", "vol_id"), np.int8),
+        (("Flag indicating if a cluster can create a S2 signal", "create_S2"), np.bool_),
     ]
 
     dtype = dtype + strax.time_fields
 
     # Config options
     # Define the TPC volume
     xenonnt_z_cathode = straxen.URLConfig(
@@ -122,15 +122,15 @@
     to ``False``.
     """
 
     depends_on = "clustered_interactions"
 
     provides = "below_cathode_interactions"
     data_kind = "below_cathode_interactions"
-    __version__ = "0.3.0"
+    __version__ = "0.3.1"
 
     # Can we import this from MergeCluster and just add the needed fields?
     dtype = [
         (("x position of the cluster [cm]", "x"), np.float32),
         (("y position of the cluster [cm]", "y"), np.float32),
         (("z position of the cluster [cm]", "z"), np.float32),
         (("Energy of the cluster [keV]", "ed"), np.float32),
@@ -138,17 +138,17 @@
         (("Mass number of the interacting particle", "A"), np.int8),
         (("Charge number of the interacting particle", "Z"), np.int8),
         (("Geant4 event ID", "evtid"), np.int32),
         (("x position of the primary particle [cm]", "x_pri"), np.float32),
         (("y position of the primary particle [cm]", "y_pri"), np.float32),
         (("z position of the primary particle [cm]", "z_pri"), np.float32),
         (("ID of the cluster", "cluster_id"), np.int32),
-        (("Xenon density at the cluster position.", "xe_density"), np.float32),
-        (("ID of the volume in which the cluster occured.", "vol_id"), np.int8),
-        (("Flag indicating if a cluster can create a S2 signal.", "create_S2"), np.bool_),
+        (("Xenon density at the cluster position", "xe_density"), np.float32),
+        (("ID of the volume in which the cluster occured", "vol_id"), np.int8),
+        (("Flag indicating if a cluster can create a S2 signal", "create_S2"), np.bool_),
     ]
 
     dtype = dtype + strax.time_fields
 
     # Config options
     # Define the volume
     xenonnt_z_cathode = straxen.URLConfig(
@@ -205,15 +205,15 @@
     meant to go into a vertical merger plugin.
     """
 
     depends_on = "clustered_interactions"
 
     provides = "gas_phase_interactions"
     data_kind = "gas_phase_interactions"
-    __version__ = "0.3.0"
+    __version__ = "0.3.1"
 
     # Can we import this from MergeCluster and just add the needed fields?
     dtype = [
         (("x position of the cluster [cm]", "x"), np.float32),
         (("y position of the cluster [cm]", "y"), np.float32),
         (("z position of the cluster [cm]", "z"), np.float32),
         (("Energy of the cluster [keV]", "ed"), np.float32),
@@ -221,51 +221,51 @@
         (("Mass number of the interacting particle", "A"), np.int8),
         (("Charge number of the interacting particle", "Z"), np.int8),
         (("Geant4 event ID", "evtid"), np.int32),
         (("x position of the primary particle [cm]", "x_pri"), np.float32),
         (("y position of the primary particle [cm]", "y_pri"), np.float32),
         (("z position of the primary particle [cm]", "z_pri"), np.float32),
         (("ID of the cluster", "cluster_id"), np.int32),
-        (("Xenon density at the cluster position.", "xe_density"), np.float32),
-        (("ID of the volume in which the cluster occured.", "vol_id"), np.int8),
-        (("Flag indicating if a cluster can create a S2 signal.", "create_S2"), np.bool_),
+        (("Xenon density at the cluster position", "xe_density"), np.float32),
+        (("ID of the volume in which the cluster occured", "vol_id"), np.int8),
+        (("Flag indicating if a cluster can create a S2 signal", "create_S2"), np.bool_),
     ]
 
     dtype = dtype + strax.time_fields
 
     # Config options
     # Define the volume
     xenonnt_z_top_pmts = straxen.URLConfig(
         default=7.3936,  # cm
         type=(int, float),
-        help="xenonnt_z_top_pmts",
+        help="Position of the top of gas phase [cm]",
     )
 
     xenonnt_z_lxe = straxen.URLConfig(
         default=0.416,  # cm ... liquid-gas interface
         type=(int, float),
-        help="xenonnt_z_lxe",
+        help="Position of the bottom of gas phase [cm]",
     )
 
     xenonnt_sensitive_volume_radius = straxen.URLConfig(
         default=66.4,  # cm
         type=(int, float),
-        help="xenonnt_sensitive_volume_radius",
+        help="Radius of the XENONnT TPC [cm]",
     )
 
     xenon_density_gas_phase = straxen.URLConfig(
         default=0.0177,
         type=(int, float),
-        help="xenon_density",
+        help="Density of XENON in the gas phase [g/cm3]",
     )
 
     create_S2_xenonnt_gas_phase = straxen.URLConfig(
         default=False,
         type=bool,
-        help="No S2s in gas",
+        help="Whether generate S2s in gas phase",
     )
 
     def compute(self, clustered_interactions):
         # Call the ROI function:
         mask = self.in_ROI(
             clustered_interactions,
             self.xenonnt_z_lxe,
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/electric_field.py` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/electric_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @export
 class ElectricField(FuseBasePlugin):
     """Plugin that calculates the electric field values for the cluster
     position."""
 
     __version__ = "0.2.2"
 
-    depends_on = ("interactions_in_roi",)
+    depends_on = "interactions_in_roi"
     provides = "electric_field_values"
     data_kind = "interactions_in_roi"
 
     save_when = strax.SaveWhen.TARGET
 
     dtype = [
         (("Electric field value at the cluster position [V/cm]", "e_field"), np.float32),
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/find_cluster.py` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/find_cluster.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/input.py` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class ChunkInput(FuseBasePlugin):
     """Plugin to read XENONnT Geant4 root or csv files.
 
     The plugin can distribute the events in time based on a source rate
     and will create multiple chunks of data if needed.
     """
 
-    __version__ = "0.3.1"
+    __version__ = "0.3.2"
 
     depends_on: Tuple = tuple()
     provides = "geant4_interactions"
 
     source_done = False
 
     dtype = [
@@ -43,17 +43,17 @@
         (("Particle type", "type"), "<U18"),
         (("Geant4 track ID", "trackid"), np.int16),
         (("Particle type of the parent particle", "parenttype"), "<U18"),
         (("Trackid of the parent particle", "parentid"), np.int16),
         (("Geant4 process creating the particle", "creaproc"), "<U25"),
         (("Geant4 process responsible for the energy deposit", "edproc"), "<U25"),
         (("Geant4 event ID", "evtid"), np.int32),
-        (("x position of the primary particle", "x_pri"), np.float32),
-        (("y position of the primary particle", "y_pri"), np.float32),
-        (("z position of the primary particle", "z_pri"), np.float32),
+        (("x position of the primary particle [cm]", "x_pri"), np.float32),
+        (("y position of the primary particle [cm]", "y_pri"), np.float32),
+        (("z position of the primary particle [cm]", "z_pri"), np.float32),
     ]
 
     dtype = dtype + strax.time_fields
 
     save_when = strax.SaveWhen.TARGET
 
     source_done = False
@@ -82,32 +82,32 @@
         "Use a value >0 to generate event times in fuse"
         "Use source_rate = 0 to use event times from the input file (only for csv input)",
     )
 
     cut_delayed = straxen.URLConfig(
         default=9e18,
         type=(int, float),
-        help="All interactions happening after this time (including the event time) will be cut.",
+        help="All interactions happening after this time (including the event time) will be cut",
     )
 
     n_interactions_per_chunk = straxen.URLConfig(
         default=1e5,
         type=(int, float),
         help="Minimum number of interaction per chunk",
     )
 
     entry_start = straxen.URLConfig(
         default=0,
         type=(int, float),
-        help="Geant4 event to start simulation from.",
+        help="Geant4 event to start simulation from",
     )
 
     entry_stop = straxen.URLConfig(
         default=None,
-        help="Geant4 event to stop simulation at. If None, all events are simulated.",
+        help="Geant4 event to stop simulation at. If None, all events are simulated",
     )
 
     cut_by_eventid = straxen.URLConfig(
         default=False,
         type=bool,
         help="If selected, the next two arguments act on the G4 event id, "
         "and not the entry number (default)",
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/merge_cluster.py` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/merge_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     is calculated as the energy weighted average of the times of the
     energy deposits. The energy of the merged cluster is the sum of the
     individual energy depositions. The cluster is then classified based
     on either the first interaction in the cluster or the most energetic
     interaction.
     """
 
-    __version__ = "0.3.0"
+    __version__ = "0.3.1"
 
     depends_on = ("geant4_interactions", "cluster_index")
 
     provides = "clustered_interactions"
     data_kind = "clustered_interactions"
 
     save_when = strax.SaveWhen.TARGET
@@ -43,33 +43,33 @@
         (("Mass number of the interacting particle", "A"), np.int8),
         (("Charge number of the interacting particle", "Z"), np.int8),
         (("Geant4 event ID", "evtid"), np.int32),
         (("x position of the primary particle [cm]", "x_pri"), np.float32),
         (("y position of the primary particle [cm]", "y_pri"), np.float32),
         (("z position of the primary particle [cm]", "z_pri"), np.float32),
         (("ID of the cluster", "cluster_id"), np.int32),
-        (("Xenon density at the cluster position. Will be set later.", "xe_density"), np.float32),
-        (("ID of the volume in which the cluster occured. Will be set later.", "vol_id"), np.int8),
+        (("Xenon density at the cluster position. Will be set later", "xe_density"), np.float32),
+        (("ID of the volume in which the cluster occured. Will be set later", "vol_id"), np.int8),
         (
             (
-                "Flag indicating if a cluster can create a S2 signal. Will be set later.",
+                "Flag indicating if a cluster can create a S2 signal. Will be set later",
                 "create_S2",
             ),
             np.bool_,
         ),
     ]
 
     dtype = dtype + strax.time_fields
 
     # Config options
     tag_cluster_by = straxen.URLConfig(
         default="take://resource://SIMULATION_CONFIG_FILE.json?fmt=json&take=tag_cluster_by",
         cache=True,
         help="Decide if you tag the cluster "
-        "according to first interaction (time) or most energetic (energy) one.",
+        "according to first interaction (time) or most energetic (energy) one",
     )
 
     def compute(self, geant4_interactions):
         if len(geant4_interactions) == 0:
             return np.zeros(0, dtype=self.dtype)
 
         result = np.zeros(len(np.unique(geant4_interactions["cluster_ids"])), dtype=self.dtype)
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/wfsim_connection.py` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/wfsim_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 
 logging.basicConfig(handlers=[logging.StreamHandler()])
 log = logging.getLogger("fuse.micro_physics.output")
 
 
 @export
 class output_plugin(FuseBasePlugin):
-    __version__ = "0.2.0"
+    __version__ = "0.2.1"
 
-    depends_on = ["interactions_in_roi", "quanta", "electric_field_values"]  # Add times later
+    depends_on = ("interactions_in_roi", "quanta", "electric_field_values")  # Add times later
 
     provides = "wfsim_instructions"
     data_kind = "wfsim_instructions"
 
     save_when = strax.SaveWhen.TARGET
 
     dtype = [
-        (("Waveform simulator event number.", "event_number"), np.int32),
+        (("Waveform simulator event number", "event_number"), np.int32),
         (("Quanta type (S1 photons or S2 electrons)", "type"), np.int8),
         (("Time of the interaction [ns]", "time"), np.int64),
         (("End Time of the interaction [ns]", "endtime"), np.int64),
         (("X position of the cluster [cm]", "x"), np.float32),
         (("Y position of the cluster [cm]", "y"), np.float32),
         (("Z position of the cluster [cm]", "z"), np.float32),
         (("Number of quanta", "amp"), np.int32),
-        (("Recoil type of interaction.", "recoil"), np.int8),
+        (("Recoil type of interaction", "recoil"), np.int8),
         (("Energy deposit of interaction", "e_dep"), np.float32),
         (("Eventid like in geant4 output rootfile", "g4id"), np.int32),
         (("Volume id giving the detector subvolume", "vol_id"), np.int32),
         (("Local field [ V / cm ]", "local_field"), np.float64),
         (("Number of excitons", "n_excitons"), np.int32),
         (("X position of the primary particle [cm]", "x_pri"), np.float32),
         (("Y position of the primary particle [cm]", "y_pri"), np.float32),
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/micro_physics/yields.py` & `xenon_fuse-1.2.0/fuse/plugins/micro_physics/yields.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 
 
 @export
 class NestYields(FuseBasePlugin):
     """Plugin that calculates the number of photons, electrons and excitons
     produced by energy deposit using nestpy."""
 
-    __version__ = "0.2.0"
+    __version__ = "0.2.1"
 
-    depends_on = ["interactions_in_roi", "electric_field_values"]
+    depends_on = ("interactions_in_roi", "electric_field_values")
     provides = "quanta"
     data_kind = "interactions_in_roi"
 
     dtype = [
-        (("Number of photons at interaction position.", "photons"), np.int32),
-        (("Number of electrons at interaction position.", "electrons"), np.int32),
-        (("Number of excitons at interaction position.", "excitons"), np.int32),
+        (("Number of photons at interaction position", "photons"), np.int32),
+        (("Number of electrons at interaction position", "electrons"), np.int32),
+        (("Number of excitons at interaction position", "excitons"), np.int32),
     ]
 
     dtype = dtype + strax.time_fields
 
     save_when = strax.SaveWhen.TARGET
 
     def setup(self):
         super().setup()
 
-        if self.deterministic_seed:
+        if self.deterministic_seed or (self.user_defined_random_seed is not None):
             # Dont know but nestpy seems to have a problem with large seeds
             self.short_seed = int(repr(self.seed)[-8:])
             log.debug(f"Generating nest random numbers starting with seed {self.short_seed}")
         else:
             log.debug("Generating random numbers with seed pulled from OS")
 
         self.quanta_from_NEST = np.vectorize(self._quanta_from_NEST)
@@ -166,15 +166,15 @@
 
         return photons, electrons, excitons
 
 
 class BetaYields(strax.Plugin):
     __version__ = "0.1.1"
 
-    depends_on = ["interactions_in_roi", "electric_field_values"]
+    depends_on = ("interactions_in_roi", "electric_field_values")
     provides = "quanta"
     data_kind = "interactions_in_roi"
 
     dtype = [
         ("photons", np.int32),
         ("electrons", np.int32),
         ("excitons", np.int32),
@@ -215,15 +215,15 @@
     cs2_spline_path = straxen.URLConfig(
         help="cs2_spline_path",
     )
 
     deterministic_seed = straxen.URLConfig(
         default=True,
         type=bool,
-        help="Set the random seed from lineage and run_id, or pull the seed from the OS.",
+        help="Set the random seed from lineage and run_id, or pull the seed from the OS",
     )
 
     def setup(self):
         if self.debug:
             log.setLevel("DEBUG")
             log.debug(f"Running BetaYields version {self.__version__} in debug mode")
         else:
@@ -304,15 +304,15 @@
 
         return beta_photons, beta_electrons, q_.excitons
 
 
 class BBFYields(FuseBasePlugin):
     __version__ = "0.1.1"
 
-    depends_on = ["interactions_in_roi", "electric_field_values"]
+    depends_on = ("interactions_in_roi", "electric_field_values")
     provides = "quanta"
 
     dtype = [
         ("photons", np.int32),
         ("electrons", np.int32),
         ("excitons", np.int32),
     ]
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/photon_pulses.py` & `xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/photon_pulses.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/pmt_afterpulses.py` & `xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_afterpulses.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     S1 and S2 signals to create a waveform.
     """
 
     __version__ = "0.3.1"
 
     depends_on = ("propagated_s2_photons", "propagated_s1_photons")
     provides = "pmt_afterpulses"
-    data_kind = "AP_photons"
+    data_kind = "ap_photons"
 
     save_when = strax.SaveWhen.TARGET
 
     dtype = [
         (("PMT channel of the photon", "channel"), np.int16),
         (("Photon creates a double photo-electron emission", "dpe"), np.bool_),
         (("Sampled PMT gain for the photon", "photon_gain"), np.int32),
@@ -119,21 +119,21 @@
         self.uniform_to_pmt_ap = self.photon_ap_cdfs
 
         for k in self.uniform_to_pmt_ap.keys():
             for q in self.uniform_to_pmt_ap[k].keys():
                 if isinstance(self.uniform_to_pmt_ap[k][q], list):
                     self.uniform_to_pmt_ap[k][q] = np.array(self.uniform_to_pmt_ap[k][q])
 
-    def compute(self, S1_photons, S2_photons):
-        if not self.enable_pmt_afterpulses or (len(S1_photons) == 0 and len(S2_photons) == 0):
+    def compute(self, s1_photons, s2_photons):
+        if not self.enable_pmt_afterpulses or (len(s1_photons) == 0 and len(s2_photons) == 0):
             return np.zeros(0, dtype=self.dtype)
 
-        merged_photons = np.concatenate([S1_photons, S2_photons])
-        S1_photons = None
-        S2_photons = None
+        merged_photons = np.concatenate([s1_photons, s2_photons])
+        s1_photons = None
+        s2_photons = None
 
         # Sort all photons by time
         sortind = np.argsort(merged_photons["time"])
         merged_photons = merged_photons[sortind]
 
         _photon_timings = merged_photons["time"]
         _photon_channels = merged_photons["channel"]
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py` & `xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     First the single PMT waveform is simulated based on the photon
     timing and gain information. Next the waveform is converted to ADC
     counts, noise and a baseline are added. Then hitfinding is performed
     and the found intervals are split into multiple fragments of fixed
     length (if needed). Finally the data is saved as raw_records.
     """
 
-    __version__ = "0.1.3"
+    __version__ = "0.1.4"
 
     depends_on = ("photon_summary", "pulse_ids", "pulse_windows")
 
     provides = "raw_records"
     data_kind = "raw_records"
 
     dtype = strax.raw_record_dtype(samples_per_record=strax.DEFAULT_RECORD_LENGTH)
@@ -244,56 +244,34 @@
 
         # convert photons to numba list for njit
         _photons = List()
         [_photons.append(x) for x in photons]
 
         if n_chunks > 1:
             for pulse_group in pulse_window_chunks[:-1]:
-                # use an upper limit for the waveform buffer
-                length_waveform_buffer = np.int32(
-                    np.sum(np.ceil(pulse_group["length"] / strax.DEFAULT_RECORD_LENGTH))
-                )
-                waveform_buffer = np.zeros(length_waveform_buffer, dtype=self.dtype)
-
-                buffer_level = build_waveform(
-                    pulse_group,
-                    _photons,
-                    unique_photon_pulse_ids,
-                    waveform_buffer,
-                    self.dt,
-                    self._pmt_current_templates,
-                    self.current_2_adc,
-                    self.noise_data["arr_0"],
-                    self.enable_noise,
-                    self.digitizer_reference_baseline,
-                    self.thresholds,
-                    self.trigger_window,
-                )
-
-                records = waveform_buffer[:buffer_level]
-
-                # Digitzier saturation
-                # Clip negative values to 0
-                records["data"][records["data"] < 0] = 0
-
-                records = strax.sort_by_time(records)
-
+                records = self.compute_chunk(_photons, unique_photon_pulse_ids, pulse_group)
                 chunk_end = np.max(strax.endtime(records))
                 chunk = self.chunk(start=last_start, end=chunk_end, data=records)
                 last_start = chunk_end
                 yield chunk
 
         # And the last chunk
+        records = self.compute_chunk(_photons, unique_photon_pulse_ids, pulse_window_chunks[-1])
+        chunk = self.chunk(start=last_start, end=end, data=records)
+        yield chunk
+
+    def compute_chunk(self, _photons, unique_photon_pulse_ids, pulse_group):
+        # use an upper limit for the waveform buffer
         length_waveform_buffer = np.int32(
-            np.sum(np.ceil(pulse_window_chunks[-1]["length"] / strax.DEFAULT_RECORD_LENGTH))
+            np.sum(np.ceil(pulse_group["length"] / strax.DEFAULT_RECORD_LENGTH))
         )
         waveform_buffer = np.zeros(length_waveform_buffer, dtype=self.dtype)
 
         buffer_level = build_waveform(
-            pulse_window_chunks[-1],
+            pulse_group,
             _photons,
             unique_photon_pulse_ids,
             waveform_buffer,
             self.dt,
             self._pmt_current_templates,
             self.current_2_adc,
             self.noise_data["arr_0"],
@@ -304,19 +282,17 @@
         )
 
         records = waveform_buffer[:buffer_level]
 
         # Digitzier saturation
         # Clip negative values to 0
         records["data"][records["data"] < 0] = 0
-
         records = strax.sort_by_time(records)
 
-        chunk = self.chunk(start=last_start, end=end, data=records)
-        yield chunk
+        return records
 
     def init_pmt_current_templates(self):
         """Create spe templates, for 10ns sample duration and 1ns rounding we
         have:
 
         _pmt_current_templates[i] : photon timing fall between [10*m+i,
         10*m+i+1) (i, m are integers)
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/truth_information/cluster_tagging.py` & `xenon_fuse-1.2.0/fuse/plugins/truth_information/cluster_tagging.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 @export
 class ClusterTagging(strax.Plugin):
     """Plugin to tag if clusters contribute to the main or alternative
     s1/s2."""
 
-    __version__ = "0.0.2"
+    __version__ = "0.0.3"
 
-    depends_on = ("peak_basics", "microphysics_summary", "event_basics", "photon_summary")
+    depends_on = ("microphysics_summary", "photon_summary", "peak_basics", "event_basics")
     provides = "tagged_clusters"
     data_kind = "interactions_in_roi"
 
     dtype = [
         ("in_main_s1", np.bool_),
         ("in_main_s2", np.bool_),
         ("in_alt_s1", np.bool_),
@@ -23,15 +23,15 @@
         ("photons_in_main_s1", np.int32),
         ("photons_in_main_s2", np.int32),
         ("photons_in_alt_s1", np.int32),
         ("photons_in_alt_s2", np.int32),
     ]
     dtype = dtype + strax.time_fields
 
-    def compute(self, peaks, interactions_in_roi, events, propagated_photons):
+    def compute(self, interactions_in_roi, propagated_photons, peaks, events):
         peaks_in_event = strax.split_by_containment(peaks, events)
         photon_in_event = strax.split_touching_windows(propagated_photons, events)
 
         result = np.zeros(len(interactions_in_roi), dtype=self.dtype)
         result["time"] = interactions_in_roi["time"]
         result["endtime"] = interactions_in_roi["endtime"]
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/truth_information/event_truth.py` & `xenon_fuse-1.2.0/fuse/plugins/truth_information/event_truth.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import numpy as np
 
 export, __all__ = strax.exporter()
 
 
 @export
 class EventTruth(strax.Plugin):
-    __version__ = "0.0.2"
+    __version__ = "0.0.3"
 
-    depends_on = ("peak_truth", "microphysics_summary", "event_basics", "photon_summary")
+    depends_on = ("microphysics_summary", "photon_summary", "peak_truth", "event_basics")
     provides = "event_truth"
     data_kind = "events"
 
     dtype = [
         ("x_obs_truth", np.float32),
         ("y_obs_truth", np.float32),
         ("z_obs_truth", np.float32),
         ("energy_of_main_peaks_truth", np.float32),
         ("total_energy_in_event_truth", np.float32),
     ]
     dtype = dtype + strax.time_fields
 
-    def compute(self, peaks, propagated_photons, interactions_in_roi, events):
+    def compute(self, interactions_in_roi, propagated_photons, peaks, events):
         peaks_in_event = strax.split_by_containment(peaks, events)
         photons_per_event = strax.split_by_containment(propagated_photons, events)
 
         n_events = len(events)
 
         result = np.zeros(n_events, dtype=self.dtype)
         result["time"] = events["time"]
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/truth_information/peak_truth.py` & `xenon_fuse-1.2.0/fuse/plugins/truth_information/peak_truth.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,35 +5,37 @@
 from ...common import pmt_gains
 
 export, __all__ = strax.exporter()
 
 
 @export
 class PeakTruth(strax.OverlapWindowPlugin):
-    __version__ = "0.0.3"
+    __version__ = "0.0.5"
 
     depends_on = (
         "photon_summary",
         "peak_basics",
-        "microphysics_summary",
-        "s1_photons",
-        "s2_photons_sum",
-        "drifted_electrons",
+        "merged_microphysics_summary",
+        "merged_s1_photons",
+        "merged_s2_photons_sum",
+        "merged_drifted_electrons",
     )
     provides = "peak_truth"
     data_kind = "peaks"
 
     dtype = [
         ("s1_photons_in_peak", np.int32),
         ("s2_photons_in_peak", np.int32),
         ("ap_photons_in_peak", np.int32),
+        ("pi_photons_in_peak", np.int32),
         ("raw_area_truth", np.float32),
         ("observable_energy_truth", np.float32),
         ("number_of_contributing_clusters_s1", np.int16),
         ("number_of_contributing_clusters_s2", np.int16),
+        ("number_of_contributing_delayed_electrons", np.int16),
         ("average_x_of_contributing_clusters", np.float32),
         ("average_y_of_contributing_clusters", np.float32),
         ("average_z_of_contributing_clusters", np.float32),
         ("average_x_obs_of_contributing_clusters", np.float32),
         ("average_y_obs_of_contributing_clusters", np.float32),
         ("average_z_obs_of_contributing_clusters", np.float32),
     ]
@@ -128,29 +130,36 @@
 
                 unique_contributing_clusters, photons_per_cluster = np.unique(
                     photons_in_peaks[i][photon_cut]["cluster_id"], return_counts=True
                 )
 
                 if photon_type == "s1":
                     result["number_of_contributing_clusters_s1"][i] = np.sum(
-                        unique_contributing_clusters > 0
+                        unique_contributing_clusters != 0
                     )
                     contributing_clusters_s1 = _get_cluster_information(
                         interactions_in_roi, unique_contributing_clusters
                     )
                     photons_per_cluster_s1 = photons_per_cluster
                 elif photon_type == "s2":
                     result["number_of_contributing_clusters_s2"][i] = np.sum(
                         unique_contributing_clusters > 0
                     )
+                    result["number_of_contributing_delayed_electrons"][i] = np.sum(
+                        unique_contributing_clusters < 0
+                    )
                     contributing_clusters_s2 = _get_cluster_information(
                         interactions_in_roi, unique_contributing_clusters
                     )
                     photons_per_cluster_s2 = photons_per_cluster
 
+                    # Get the number of photons from delayed electrons
+                    photon_cut &= photons_in_peaks[i]["cluster_id"] < 0
+                    result["pi_photons_in_peak"][i] = np.sum(photon_cut)
+
             if (result["s1_photons_in_peak"][i] + result["s2_photons_in_peak"][i]) > 0:
                 positions_to_evaluate = ["x", "y", "z", "x_obs", "y_obs", "z_obs"]
 
                 for position in positions_to_evaluate:
                     result_name = "average_" + position + "_of_contributing_clusters"
 
                     result[result_name][i] = weighted_position_average(
@@ -175,16 +184,23 @@
                     * contributing_clusters_s1["ed"]
                 )
                 # Sum up up the two:
                 result["observable_energy_truth"][i] = np.sum(
                     energy_of_s1_photons_in_peak
                 ) + np.sum(energy_of_s2_photons_in_peak)
 
+                # Calculate the raw area truth
+                # exclude PMT AP photons as well as photons from delayed electrons
+                masked_photons = photons_in_peaks[i]
+                masked_photons = masked_photons[
+                    (masked_photons["photon_type"] != 0) & (masked_photons["cluster_id"] > 0)
+                ]
+
                 result["raw_area_truth"][i] = np.sum(
-                    photons_in_peaks[i]["photon_gain"] / self.gains[photons_in_peaks[i]["channel"]]
+                    masked_photons["photon_gain"] / self.gains[masked_photons["channel"]]
                 )
 
         return result
 
 
 def _get_cluster_information(interactions_in_roi, unique_contributing_clusters):
     contributing_cluster_informations = interactions_in_roi[
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/truth_information/records_truth.py` & `xenon_fuse-1.2.0/fuse/plugins/truth_information/records_truth.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 export, __all__ = strax.exporter()
 
 
 @export
 class RecordsTruth(strax.Plugin):
     """Plugin that computes the truth information for raw_records."""
 
-    __version__ = "0.0.1"
+    __version__ = "0.0.2"
 
-    depends_on = ("raw_records", "photon_summary")
+    depends_on = ("photon_summary", "raw_records")
     provides = "records_truth"
 
     dtype = [
         (("Number of S1 photons in record", "s1_photons_in_record"), np.int32),
         (("Number of S2 photons in record", "s2_photons_in_record"), np.int32),
         (("Number of AP photons in record", "ap_photons_in_record"), np.int32),
         (("Sum of the photon gains", "raw_area"), np.float32),
@@ -63,15 +63,15 @@
         self.gains = pmt_gains(
             self.gain_model_mc,
             digitizer_voltage_range=self.digitizer_voltage_range,
             digitizer_bits=self.digitizer_bits,
             pmt_circuit_load_resistor=self.pmt_circuit_load_resistor,
         )
 
-    def compute(self, raw_records, propagated_photons):
+    def compute(self, propagated_photons, raw_records):
         result = np.zeros(len(raw_records), dtype=self.dtype)
         result["time"] = raw_records["time"]
         result["length"] = raw_records["length"]
         result["dt"] = raw_records["dt"]
         result["channel"] = raw_records["channel"]
 
         photons_per_channel, unique_photon_channels = split_photons_by_channel(propagated_photons)
```

### Comparing `xenon_fuse-1.1.0/fuse/plugins/truth_information/surviving_clusters.py` & `xenon_fuse-1.2.0/fuse/plugins/truth_information/surviving_clusters.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 import numpy as np
 
 export, __all__ = strax.exporter()
 
 
 @export
 class SurvivingClusters(strax.Plugin):
-    __version__ = "0.0.2"
+    __version__ = "0.0.3"
 
-    depends_on = ("peak_basics", "photon_summary", "microphysics_summary")
+    depends_on = ("microphysics_summary", "photon_summary", "peak_basics")
     provides = "surviving_clusters"
+    data_kind = "interactions_in_roi"
 
     dtype = [
         ("creating_a_photon", np.bool_),
         ("in_a_peak", np.bool_),
     ]
     dtype += strax.time_fields
 
-    data_kind = "interactions_in_roi"
-
-    def compute(self, peaks, propagated_photons, interactions_in_roi):
+    def compute(self, interactions_in_roi, propagated_photons, peaks):
         # Check if the cluster contributes to any cluster
         cluster_creating_a_photon = np.isin(
             interactions_in_roi["cluster_id"], np.unique(propagated_photons["cluster_id"])
         )
 
         photons_per_peaks = strax.split_touching_windows(propagated_photons, peaks)
```

### Comparing `xenon_fuse-1.1.0/fuse/vertical_merger_plugin.py` & `xenon_fuse-1.2.0/fuse/vertical_merger_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/fuse/volume_plugin.py` & `xenon_fuse-1.2.0/fuse/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/pyproject.toml` & `xenon_fuse-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xenon-fuse"
-version = "1.1.0"
+version = "1.2.0"
 description = "XENON Framework for Unified Simulations of Events"
 authors = [
   "Henning Schulze Eißing, <h_schu55@uni-muenster.de>",
   "Diego Ramírez García, <diego.ramirez@physik.uzh.ch>",
 ]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `xenon_fuse-1.1.0/tests/_utils.py` & `xenon_fuse-1.2.0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/tests/test_DetectorPhysics_csv.py` & `xenon_fuse-1.2.0/tests/test_DetectorPhysics_csv.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/tests/test_FullChain.py` & `xenon_fuse-1.2.0/tests/test_FullChain.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/tests/test_MicroPhysics.py` & `xenon_fuse-1.2.0/tests/test_MicroPhysics.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/tests/test_deterministic_seed.py` & `xenon_fuse-1.2.0/tests/test_deterministic_seed.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/tests/test_input.py` & `xenon_fuse-1.2.0/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.1.0/PKG-INFO` & `xenon_fuse-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenon-fuse
-Version: 1.1.0
+Version: 1.2.0
 Summary: XENON Framework for Unified Simulations of Events
 Home-page: https://github.com/XENONnT/fuse
 Author: Henning Schulze Eißing,
 Author-email: h_schu55@uni-muenster.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

