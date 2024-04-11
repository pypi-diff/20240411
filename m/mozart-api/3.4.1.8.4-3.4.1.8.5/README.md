# Comparing `tmp/mozart_api-3.4.1.8.4.tar.gz` & `tmp/mozart_api-3.4.1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozart_api-3.4.1.8.4.tar", max compression
+gzip compressed data, was "mozart_api-3.4.1.8.5.tar", max compression
```

## Comparing `mozart_api-3.4.1.8.4.tar` & `mozart_api-3.4.1.8.5.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rwxr-xr-x   0        0        0     1074 2024-03-26 16:52:03.073128 mozart_api-3.4.1.8.4/LICENSE
--rw-r--r--   0        0        0     1899 2024-03-26 16:52:04.929490 mozart_api-3.4.1.8.4/README.md
--rw-r--r--   0        0        0    15806 2024-03-26 16:52:06.242559 mozart_api-3.4.1.8.4/mozart_api/__init__.py
--rw-r--r--   0        0        0      861 2024-03-26 16:52:06.583133 mozart_api-3.4.1.8.4/mozart_api/api/__init__.py
--rw-r--r--   0        0        0    58560 2024-03-26 16:52:07.166125 mozart_api-3.4.1.8.4/mozart_api/api/beolink_api.py
--rw-r--r--   0        0        0     5916 2024-03-26 16:52:06.660571 mozart_api-3.4.1.8.4/mozart_api/api/bluetooth_api.py
--rw-r--r--   0        0        0     6911 2024-03-26 16:52:06.625843 mozart_api-3.4.1.8.4/mozart_api/api/content_api.py
--rw-r--r--   0        0        0     6678 2024-03-26 16:52:06.637021 mozart_api-3.4.1.8.4/mozart_api/api/deezer_api.py
--rw-r--r--   0        0        0   310525 2024-03-26 16:52:08.573699 mozart_api-3.4.1.8.4/mozart_api/api/mozart_api.py
--rw-r--r--   0        0        0     7207 2024-03-26 16:52:06.639091 mozart_api-3.4.1.8.4/mozart_api/api/overlay_api.py
--rw-r--r--   0        0        0    63930 2024-03-26 16:52:07.328320 mozart_api-3.4.1.8.4/mozart_api/api/playback_api.py
--rw-r--r--   0        0        0    15022 2024-03-26 16:52:06.691065 mozart_api-3.4.1.8.4/mozart_api/api/power_api.py
--rw-r--r--   0        0        0    11648 2024-03-26 16:52:06.738710 mozart_api-3.4.1.8.4/mozart_api/api/product_api.py
--rw-r--r--   0        0        0    17464 2024-03-26 16:52:07.010550 mozart_api-3.4.1.8.4/mozart_api/api/remote_api.py
--rw-r--r--   0        0        0    21712 2024-03-26 16:52:06.885609 mozart_api-3.4.1.8.4/mozart_api/api/scenes_api.py
--rw-r--r--   0        0        0    27344 2024-03-26 16:52:07.010720 mozart_api-3.4.1.8.4/mozart_api/api/settings_api.py
--rw-r--r--   0        0        0     5915 2024-03-26 16:52:06.757526 mozart_api-3.4.1.8.4/mozart_api/api/software_update_api.py
--rw-r--r--   0        0        0    69249 2024-03-26 16:52:07.422384 mozart_api-3.4.1.8.4/mozart_api/api/sound_api.py
--rw-r--r--   0        0        0     5839 2024-03-26 16:52:06.851992 mozart_api-3.4.1.8.4/mozart_api/api/speaker_group_api.py
--rw-r--r--   0        0        0     7369 2024-03-26 16:52:06.962191 mozart_api-3.4.1.8.4/mozart_api/api/stand_api.py
--rw-r--r--   0        0        0    27639 2024-03-26 16:52:06.378049 mozart_api-3.4.1.8.4/mozart_api/api_client.py
--rw-r--r--   0        0        0      827 2024-03-26 16:52:06.110279 mozart_api-3.4.1.8.4/mozart_api/api_response.py
--rw-r--r--   0        0        0    14126 2024-03-26 16:52:06.243411 mozart_api-3.4.1.8.4/mozart_api/configuration.py
--rw-r--r--   0        0        0     5369 2024-03-26 16:52:06.166466 mozart_api-3.4.1.8.4/mozart_api/exceptions.py
--rw-r--r--   0        0        0    14480 2024-03-26 16:52:08.930069 mozart_api-3.4.1.8.4/mozart_api/models/__init__.py
--rw-r--r--   0        0        0    12106 2024-03-26 16:52:09.072083 mozart_api-3.4.1.8.4/mozart_api/models/action.py
--rw-r--r--   0        0        0     2601 2024-03-26 16:52:08.864194 mozart_api-3.4.1.8.4/mozart_api/models/alarm_timer_event_data.py
--rw-r--r--   0        0        0     2004 2024-03-26 16:52:08.834030 mozart_api-3.4.1.8.4/mozart_api/models/alarm_triggered_info.py
--rw-r--r--   0        0        0     1830 2024-03-26 16:52:08.890653 mozart_api-3.4.1.8.4/mozart_api/models/ambience.py
--rw-r--r--   0        0        0     3047 2024-03-26 16:52:08.859372 mozart_api-3.4.1.8.4/mozart_api/models/ambience_feature.py
--rw-r--r--   0        0        0     2841 2024-03-26 16:52:08.860536 mozart_api-3.4.1.8.4/mozart_api/models/ambience_range.py
--rw-r--r--   0        0        0     2179 2024-03-26 16:52:08.855434 mozart_api-3.4.1.8.4/mozart_api/models/art.py
--rw-r--r--   0        0        0     1821 2024-03-26 16:52:08.892524 mozart_api-3.4.1.8.4/mozart_api/models/balance.py
--rw-r--r--   0        0        0     2991 2024-03-26 16:52:08.951740 mozart_api-3.4.1.8.4/mozart_api/models/balance_feature.py
--rw-r--r--   0        0        0     2786 2024-03-26 16:52:08.925092 mozart_api-3.4.1.8.4/mozart_api/models/balance_range.py
--rw-r--r--   0        0        0     1722 2024-03-26 16:52:08.894310 mozart_api-3.4.1.8.4/mozart_api/models/bass.py
--rw-r--r--   0        0        0     2929 2024-03-26 16:52:08.947926 mozart_api-3.4.1.8.4/mozart_api/models/bass_feature.py
--rw-r--r--   0        0        0     2056 2024-03-26 16:52:08.947953 mozart_api-3.4.1.8.4/mozart_api/models/bass_management.py
--rw-r--r--   0        0        0     3309 2024-03-26 16:52:08.969394 mozart_api-3.4.1.8.4/mozart_api/models/bass_management_feature.py
--rw-r--r--   0        0        0     2907 2024-03-26 16:52:08.951940 mozart_api-3.4.1.8.4/mozart_api/models/bass_management_range.py
--rw-r--r--   0        0        0     2781 2024-03-26 16:52:08.971037 mozart_api-3.4.1.8.4/mozart_api/models/bass_range.py
--rw-r--r--   0        0        0     2838 2024-03-26 16:52:09.008403 mozart_api-3.4.1.8.4/mozart_api/models/battery_state.py
--rw-r--r--   0        0        0     2251 2024-03-26 16:52:08.990211 mozart_api-3.4.1.8.4/mozart_api/models/beo_remote_button.py
--rw-r--r--   0        0        0     1870 2024-03-26 16:52:08.979953 mozart_api-3.4.1.8.4/mozart_api/models/beolink_available_listener.py
--rw-r--r--   0        0        0     3795 2024-03-26 16:52:09.094376 mozart_api-3.4.1.8.4/mozart_api/models/beolink_experience.py
--rw-r--r--   0        0        0     3301 2024-03-26 16:52:09.068595 mozart_api-3.4.1.8.4/mozart_api/models/beolink_experiences_result.py
--rw-r--r--   0        0        0     2222 2024-03-26 16:52:09.069290 mozart_api-3.4.1.8.4/mozart_api/models/beolink_join_request.py
--rw-r--r--   0        0        0     3644 2024-03-26 16:52:09.093912 mozart_api-3.4.1.8.4/mozart_api/models/beolink_join_result.py
--rw-r--r--   0        0        0     1926 2024-03-26 16:52:09.008460 mozart_api-3.4.1.8.4/mozart_api/models/beolink_leader.py
--rw-r--r--   0        0        0     1798 2024-03-26 16:52:09.069023 mozart_api-3.4.1.8.4/mozart_api/models/beolink_listener.py
--rw-r--r--   0        0        0     1910 2024-03-26 16:52:09.072039 mozart_api-3.4.1.8.4/mozart_api/models/beolink_peer.py
--rw-r--r--   0        0        0     2066 2024-03-26 16:52:09.092959 mozart_api-3.4.1.8.4/mozart_api/models/bluetooth_device.py
--rw-r--r--   0        0        0     2433 2024-03-26 16:52:09.141286 mozart_api-3.4.1.8.4/mozart_api/models/bluetooth_device_list.py
--rw-r--r--   0        0        0     1969 2024-03-26 16:52:09.108124 mozart_api-3.4.1.8.4/mozart_api/models/button_event.py
--rw-r--r--   0        0        0     2058 2024-03-26 16:52:09.142031 mozart_api-3.4.1.8.4/mozart_api/models/compression.py
--rw-r--r--   0        0        0     3288 2024-03-26 16:52:09.238116 mozart_api-3.4.1.8.4/mozart_api/models/compression_feature.py
--rw-r--r--   0        0        0     2860 2024-03-26 16:52:09.220037 mozart_api-3.4.1.8.4/mozart_api/models/compression_range.py
--rw-r--r--   0        0        0     3182 2024-03-26 16:52:09.211794 mozart_api-3.4.1.8.4/mozart_api/models/content_item.py
--rw-r--r--   0        0        0     2217 2024-03-26 16:52:09.238077 mozart_api-3.4.1.8.4/mozart_api/models/directivity.py
--rw-r--r--   0        0        0     3477 2024-03-26 16:52:09.290664 mozart_api-3.4.1.8.4/mozart_api/models/directivity_feature.py
--rw-r--r--   0        0        0     2890 2024-03-26 16:52:09.278859 mozart_api-3.4.1.8.4/mozart_api/models/directivity_range.py
--rw-r--r--   0        0        0     2483 2024-03-26 16:52:09.215233 mozart_api-3.4.1.8.4/mozart_api/models/error_model.py
--rw-r--r--   0        0        0     1803 2024-03-26 16:52:09.244288 mozart_api-3.4.1.8.4/mozart_api/models/fader.py
--rw-r--r--   0        0        0     2959 2024-03-26 16:52:09.276964 mozart_api-3.4.1.8.4/mozart_api/models/fader_feature.py
--rw-r--r--   0        0        0     2756 2024-03-26 16:52:09.296702 mozart_api-3.4.1.8.4/mozart_api/models/fader_range.py
--rw-r--r--   0        0        0     2023 2024-03-26 16:52:09.271889 mozart_api-3.4.1.8.4/mozart_api/models/hdmi_input.py
--rw-r--r--   0        0        0     2994 2024-03-26 16:52:09.315328 mozart_api-3.4.1.8.4/mozart_api/models/hdmi_video_format.py
--rw-r--r--   0        0        0     1784 2024-03-26 16:52:09.310182 mozart_api-3.4.1.8.4/mozart_api/models/home_control_ixp.py
--rw-r--r--   0        0        0     2041 2024-03-26 16:52:09.370415 mozart_api-3.4.1.8.4/mozart_api/models/home_control_uri.py
--rw-r--r--   0        0        0     2400 2024-03-26 16:52:09.327334 mozart_api-3.4.1.8.4/mozart_api/models/install_record_id_state.py
--rw-r--r--   0        0        0     2251 2024-03-26 16:52:09.337053 mozart_api-3.4.1.8.4/mozart_api/models/latency_profile.py
--rw-r--r--   0        0        0     3428 2024-03-26 16:52:09.370731 mozart_api-3.4.1.8.4/mozart_api/models/lge_tv_sound_settings.py
--rw-r--r--   0        0        0     5073 2024-03-26 16:52:09.373865 mozart_api-3.4.1.8.4/mozart_api/models/listening_mode.py
--rw-r--r--   0        0        0     9541 2024-03-26 16:52:09.596370 mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_features.py
--rw-r--r--   0        0        0     5136 2024-03-26 16:52:09.419613 mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_props.py
--rw-r--r--   0        0        0     2586 2024-03-26 16:52:09.375724 mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_ref.py
--rw-r--r--   0        0        0     4893 2024-03-26 16:52:09.444870 mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_trigger.py
--rw-r--r--   0        0        0     1746 2024-03-26 16:52:09.422477 mozart_api-3.4.1.8.4/mozart_api/models/loudness.py
--rw-r--r--   0        0        0     2095 2024-03-26 16:52:09.430744 mozart_api-3.4.1.8.4/mozart_api/models/microphone_state.py
--rw-r--r--   0        0        0     3028 2024-03-26 16:52:09.443123 mozart_api-3.4.1.8.4/mozart_api/models/microphones_state.py
--rw-r--r--   0        0        0     4208 2024-03-26 16:52:09.421867 mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request.py
--rw-r--r--   0        0        0     2482 2024-03-26 16:52:09.425657 mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_common.py
--rw-r--r--   0        0        0     2432 2024-03-26 16:52:09.445174 mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_from_usb.py
--rw-r--r--   0        0        0     2245 2024-03-26 16:52:09.505764 mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_from_usb_from_usb.py
--rw-r--r--   0        0        0     2629 2024-03-26 16:52:09.561920 mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_text_to_speech.py
--rw-r--r--   0        0        0     2745 2024-03-26 16:52:09.463688 mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py
--rw-r--r--   0        0        0     2197 2024-03-26 16:52:09.521063 mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_uri.py
--rw-r--r--   0        0        0     3054 2024-03-26 16:52:09.596657 mozart_api-3.4.1.8.4/mozart_api/models/paired_remote.py
--rw-r--r--   0        0        0     2429 2024-03-26 16:52:09.518530 mozart_api-3.4.1.8.4/mozart_api/models/paired_remote_response.py
--rw-r--r--   0        0        0     4141 2024-03-26 16:52:09.593936 mozart_api-3.4.1.8.4/mozart_api/models/play_queue_item.py
--rw-r--r--   0        0        0     2148 2024-03-26 16:52:09.539134 mozart_api-3.4.1.8.4/mozart_api/models/play_queue_item_type.py
--rw-r--r--   0        0        0     2501 2024-03-26 16:52:09.593454 mozart_api-3.4.1.8.4/mozart_api/models/play_queue_settings.py
--rw-r--r--   0        0        0    10707 2024-03-26 16:52:09.861070 mozart_api-3.4.1.8.4/mozart_api/models/playback_content_metadata.py
--rw-r--r--   0        0        0     2326 2024-03-26 16:52:09.725410 mozart_api-3.4.1.8.4/mozart_api/models/playback_error.py
--rw-r--r--   0        0        0     2357 2024-03-26 16:52:09.746804 mozart_api-3.4.1.8.4/mozart_api/models/playback_progress.py
--rw-r--r--   0        0        0     3655 2024-03-26 16:52:09.721280 mozart_api-3.4.1.8.4/mozart_api/models/playback_state.py
--rw-r--r--   0        0        0     2314 2024-03-26 16:52:09.696867 mozart_api-3.4.1.8.4/mozart_api/models/power_link_trigger.py
--rw-r--r--   0        0        0     2207 2024-03-26 16:52:09.786783 mozart_api-3.4.1.8.4/mozart_api/models/power_state_enum.py
--rw-r--r--   0        0        0     4122 2024-03-26 16:52:09.831263 mozart_api-3.4.1.8.4/mozart_api/models/preset.py
--rw-r--r--   0        0        0     2348 2024-03-26 16:52:09.781458 mozart_api-3.4.1.8.4/mozart_api/models/product_curtain_status.py
--rw-r--r--   0        0        0     2029 2024-03-26 16:52:09.761087 mozart_api-3.4.1.8.4/mozart_api/models/product_friendly_name.py
--rw-r--r--   0        0        0     5885 2024-03-26 16:52:09.969273 mozart_api-3.4.1.8.4/mozart_api/models/product_state.py
--rw-r--r--   0        0        0     7313 2024-03-26 16:52:09.964214 mozart_api-3.4.1.8.4/mozart_api/models/remote_menu_item.py
--rw-r--r--   0        0        0     6255 2024-03-26 16:52:09.868635 mozart_api-3.4.1.8.4/mozart_api/models/remote_menu_item_properties.py
--rw-r--r--   0        0        0     2628 2024-03-26 16:52:09.812553 mozart_api-3.4.1.8.4/mozart_api/models/remote_ui_key_state.py
--rw-r--r--   0        0        0     2362 2024-03-26 16:52:09.844821 mozart_api-3.4.1.8.4/mozart_api/models/rendering_state.py
--rw-r--r--   0        0        0     2014 2024-03-26 16:52:09.831298 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation.py
--rw-r--r--   0        0        0     2857 2024-03-26 16:52:09.865826 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_current_measurement.py
--rw-r--r--   0        0        0     1850 2024-03-26 16:52:09.866225 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_debug.py
--rw-r--r--   0        0        0     1866 2024-03-26 16:52:09.866196 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_enabled.py
--rw-r--r--   0        0        0     2843 2024-03-26 16:52:09.876847 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_error_details.py
--rw-r--r--   0        0        0     2838 2024-03-26 16:52:09.939861 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_feature.py
--rw-r--r--   0        0        0     4906 2024-03-26 16:52:10.018516 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_info.py
--rw-r--r--   0        0        0     4096 2024-03-26 16:52:09.936407 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_measurement_error.py
--rw-r--r--   0        0        0     7000 2024-03-26 16:52:09.995935 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_properties.py
--rw-r--r--   0        0        0     2538 2024-03-26 16:52:09.974121 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_range.py
--rw-r--r--   0        0        0     2020 2024-03-26 16:52:09.944163 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_response.py
--rw-r--r--   0        0        0     5639 2024-03-26 16:52:10.107794 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_result.py
--rw-r--r--   0        0        0     6652 2024-03-26 16:52:10.081404 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_state.py
--rw-r--r--   0        0        0     2293 2024-03-26 16:52:09.976601 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_state_value.py
--rw-r--r--   0        0        0     2492 2024-03-26 16:52:10.027956 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_type.py
--rw-r--r--   0        0        0     2033 2024-03-26 16:52:10.027908 mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_version.py
--rw-r--r--   0        0        0     4392 2024-03-26 16:52:10.081274 mozart_api-3.4.1.8.4/mozart_api/models/scene.py
--rw-r--r--   0        0        0     2533 2024-03-26 16:52:10.085498 mozart_api-3.4.1.8.4/mozart_api/models/scene_classification.py
--rw-r--r--   0        0        0     2201 2024-03-26 16:52:10.087515 mozart_api-3.4.1.8.4/mozart_api/models/scene_match.py
--rw-r--r--   0        0        0     3710 2024-03-26 16:52:10.105460 mozart_api-3.4.1.8.4/mozart_api/models/scene_properties.py
--rw-r--r--   0        0        0     2855 2024-03-26 16:52:10.091683 mozart_api-3.4.1.8.4/mozart_api/models/scene_trigger_base_properties.py
--rw-r--r--   0        0        0     3104 2024-03-26 16:52:10.111041 mozart_api-3.4.1.8.4/mozart_api/models/software_update_state.py
--rw-r--r--   0        0        0     3668 2024-03-26 16:52:10.132954 mozart_api-3.4.1.8.4/mozart_api/models/software_update_status.py
--rw-r--r--   0        0        0     2623 2024-03-26 16:52:10.131292 mozart_api-3.4.1.8.4/mozart_api/models/sound_adjustments.py
--rw-r--r--   0        0        0    11453 2024-03-26 16:52:10.312904 mozart_api-3.4.1.8.4/mozart_api/models/sound_feature_set.py
--rw-r--r--   0        0        0     3432 2024-03-26 16:52:10.134439 mozart_api-3.4.1.8.4/mozart_api/models/sound_settings.py
--rw-r--r--   0        0        0     1994 2024-03-26 16:52:10.131327 mozart_api-3.4.1.8.4/mozart_api/models/sound_tone_touch.py
--rw-r--r--   0        0        0     2993 2024-03-26 16:52:10.140780 mozart_api-3.4.1.8.4/mozart_api/models/source.py
--rw-r--r--   0        0        0     2332 2024-03-26 16:52:10.143824 mozart_api-3.4.1.8.4/mozart_api/models/source_array.py
--rw-r--r--   0        0        0     2042 2024-03-26 16:52:10.144186 mozart_api-3.4.1.8.4/mozart_api/models/source_type_enum.py
--rw-r--r--   0        0        0     1921 2024-03-26 16:52:10.206945 mozart_api-3.4.1.8.4/mozart_api/models/spatial_envelopment.py
--rw-r--r--   0        0        0     3184 2024-03-26 16:52:10.181616 mozart_api-3.4.1.8.4/mozart_api/models/spatial_envelopment_feature.py
--rw-r--r--   0        0        0     2967 2024-03-26 16:52:10.185033 mozart_api-3.4.1.8.4/mozart_api/models/spatial_envelopment_range.py
--rw-r--r--   0        0        0     1876 2024-03-26 16:52:10.175977 mozart_api-3.4.1.8.4/mozart_api/models/spatial_height.py
--rw-r--r--   0        0        0     3104 2024-03-26 16:52:10.192023 mozart_api-3.4.1.8.4/mozart_api/models/spatial_height_feature.py
--rw-r--r--   0        0        0     2892 2024-03-26 16:52:10.202639 mozart_api-3.4.1.8.4/mozart_api/models/spatial_height_range.py
--rw-r--r--   0        0        0     2155 2024-03-26 16:52:10.190192 mozart_api-3.4.1.8.4/mozart_api/models/spatial_processing.py
--rw-r--r--   0        0        0     3429 2024-03-26 16:52:10.245995 mozart_api-3.4.1.8.4/mozart_api/models/spatial_processing_feature.py
--rw-r--r--   0        0        0     2952 2024-03-26 16:52:10.237784 mozart_api-3.4.1.8.4/mozart_api/models/spatial_processing_range.py
--rw-r--r--   0        0        0     1894 2024-03-26 16:52:10.213594 mozart_api-3.4.1.8.4/mozart_api/models/spatial_surround.py
--rw-r--r--   0        0        0     3136 2024-03-26 16:52:10.255958 mozart_api-3.4.1.8.4/mozart_api/models/spatial_surround_feature.py
--rw-r--r--   0        0        0     2922 2024-03-26 16:52:10.254966 mozart_api-3.4.1.8.4/mozart_api/models/spatial_surround_range.py
--rw-r--r--   0        0        0     1867 2024-03-26 16:52:10.246518 mozart_api-3.4.1.8.4/mozart_api/models/spatial_width.py
--rw-r--r--   0        0        0     3088 2024-03-26 16:52:10.258726 mozart_api-3.4.1.8.4/mozart_api/models/spatial_width_feature.py
--rw-r--r--   0        0        0     2877 2024-03-26 16:52:10.256163 mozart_api-3.4.1.8.4/mozart_api/models/spatial_width_range.py
--rw-r--r--   0        0        0     6647 2024-03-26 16:52:10.329312 mozart_api-3.4.1.8.4/mozart_api/models/speaker_group.py
--rw-r--r--   0        0        0     5030 2024-03-26 16:52:10.364132 mozart_api-3.4.1.8.4/mozart_api/models/speaker_group_member.py
--rw-r--r--   0        0        0     2607 2024-03-26 16:52:10.308981 mozart_api-3.4.1.8.4/mozart_api/models/speaker_group_member_location.py
--rw-r--r--   0        0        0     2145 2024-03-26 16:52:10.314831 mozart_api-3.4.1.8.4/mozart_api/models/speaker_group_overview.py
--rw-r--r--   0        0        0     4386 2024-03-26 16:52:10.329374 mozart_api-3.4.1.8.4/mozart_api/models/speaker_link_member_status.py
--rw-r--r--   0        0        0     2952 2024-03-26 16:52:10.364529 mozart_api-3.4.1.8.4/mozart_api/models/speaker_link_status.py
--rw-r--r--   0        0        0     2159 2024-03-26 16:52:10.307170 mozart_api-3.4.1.8.4/mozart_api/models/speaker_role_enum.py
--rw-r--r--   0        0        0     1876 2024-03-26 16:52:10.329399 mozart_api-3.4.1.8.4/mozart_api/models/speech_enhance.py
--rw-r--r--   0        0        0     3104 2024-03-26 16:52:10.343050 mozart_api-3.4.1.8.4/mozart_api/models/speech_enhance_feature.py
--rw-r--r--   0        0        0     2892 2024-03-26 16:52:10.363582 mozart_api-3.4.1.8.4/mozart_api/models/speech_enhance_range.py
--rw-r--r--   0        0        0     1810 2024-03-26 16:52:10.343929 mozart_api-3.4.1.8.4/mozart_api/models/stand_connected.py
--rw-r--r--   0        0        0     2875 2024-03-26 16:52:10.371105 mozart_api-3.4.1.8.4/mozart_api/models/stand_movement.py
--rw-r--r--   0        0        0     1824 2024-03-26 16:52:10.364152 mozart_api-3.4.1.8.4/mozart_api/models/stand_position.py
--rw-r--r--   0        0        0     2488 2024-03-26 16:52:10.365316 mozart_api-3.4.1.8.4/mozart_api/models/tone_touch.py
--rw-r--r--   0        0        0     1817 2024-03-26 16:52:10.363848 mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_type.py
--rw-r--r--   0        0        0     2922 2024-03-26 16:52:10.387162 mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_type_range.py
--rw-r--r--   0        0        0     3051 2024-03-26 16:52:10.431213 mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_x_feature.py
--rw-r--r--   0        0        0     3051 2024-03-26 16:52:10.400872 mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_y_feature.py
--rw-r--r--   0        0        0     1740 2024-03-26 16:52:10.390787 mozart_api-3.4.1.8.4/mozart_api/models/treble.py
--rw-r--r--   0        0        0     2961 2024-03-26 16:52:10.469318 mozart_api-3.4.1.8.4/mozart_api/models/treble_feature.py
--rw-r--r--   0        0        0     2811 2024-03-26 16:52:10.407064 mozart_api-3.4.1.8.4/mozart_api/models/treble_range.py
--rw-r--r--   0        0        0     2283 2024-03-26 16:52:10.403447 mozart_api-3.4.1.8.4/mozart_api/models/tv_info_event_data.py
--rw-r--r--   0        0        0     2135 2024-03-26 16:52:10.405205 mozart_api-3.4.1.8.4/mozart_api/models/tv_integration_types.py
--rw-r--r--   0        0        0     2988 2024-03-26 16:52:10.469009 mozart_api-3.4.1.8.4/mozart_api/models/tv_properties.py
--rw-r--r--   0        0        0     2212 2024-03-26 16:52:10.429638 mozart_api-3.4.1.8.4/mozart_api/models/tv_sound_settings.py
--rw-r--r--   0        0        0     3290 2024-03-26 16:52:10.479191 mozart_api-3.4.1.8.4/mozart_api/models/tv_state.py
--rw-r--r--   0        0        0     1716 2024-03-26 16:52:10.451050 mozart_api-3.4.1.8.4/mozart_api/models/uri.py
--rw-r--r--   0        0        0     1780 2024-03-26 16:52:10.451599 mozart_api-3.4.1.8.4/mozart_api/models/user_flow.py
--rw-r--r--   0        0        0     3777 2024-03-26 16:52:10.482894 mozart_api-3.4.1.8.4/mozart_api/models/video_pixel_format.py
--rw-r--r--   0        0        0     2488 2024-03-26 16:52:10.476171 mozart_api-3.4.1.8.4/mozart_api/models/video_timings.py
--rw-r--r--   0        0        0     1768 2024-03-26 16:52:10.468969 mozart_api-3.4.1.8.4/mozart_api/models/volume_level.py
--rw-r--r--   0        0        0     1762 2024-03-26 16:52:10.487124 mozart_api-3.4.1.8.4/mozart_api/models/volume_mute.py
--rw-r--r--   0        0        0     2623 2024-03-26 16:52:10.521968 mozart_api-3.4.1.8.4/mozart_api/models/volume_settings.py
--rw-r--r--   0        0        0     3438 2024-03-26 16:52:10.522395 mozart_api-3.4.1.8.4/mozart_api/models/volume_state.py
--rw-r--r--   0        0        0     2572 2024-03-26 16:52:10.537938 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_active_hdmi_input_signal.py
--rw-r--r--   0        0        0     2593 2024-03-26 16:52:10.526569 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_active_listening_mode.py
--rw-r--r--   0        0        0     2593 2024-03-26 16:52:10.525611 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_active_speaker_group.py
--rw-r--r--   0        0        0     2526 2024-03-26 16:52:10.539092 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_alarm_timer.py
--rw-r--r--   0        0        0     2553 2024-03-26 16:52:10.514695 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_alarm_triggered.py
--rw-r--r--   0        0        0     2472 2024-03-26 16:52:10.558268 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_battery.py
--rw-r--r--   0        0        0     2549 2024-03-26 16:52:10.575817 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_beo_remote_button.py
--rw-r--r--   0        0        0     2607 2024-03-26 16:52:10.560520 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_beolink_experiences_result.py
--rw-r--r--   0        0        0     2523 2024-03-26 16:52:10.559074 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_beolink_join_result.py
--rw-r--r--   0        0        0     2460 2024-03-26 16:52:10.571650 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_button.py
--rw-r--r--   0        0        0     2513 2024-03-26 16:52:10.571705 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_curtains.py
--rw-r--r--   0        0        0     2597 2024-03-26 16:52:10.605534 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_hdmi_video_format_signal.py
--rw-r--r--   0        0        0     2601 2024-03-26 16:52:10.577651 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_notification.py
--rw-r--r--   0        0        0     2524 2024-03-26 16:52:10.594262 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_error.py
--rw-r--r--   0        0        0     2589 2024-03-26 16:52:10.593771 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_metadata.py
--rw-r--r--   0        0        0     2560 2024-03-26 16:52:10.595057 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_progress.py
--rw-r--r--   0        0        0     2503 2024-03-26 16:52:10.605484 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_source.py
--rw-r--r--   0        0        0     2528 2024-03-26 16:52:10.608061 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_state.py
--rw-r--r--   0        0        0     2505 2024-03-26 16:52:10.605853 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_power_state.py
--rw-r--r--   0        0        0     2642 2024-03-26 16:52:10.613251 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_puc_install_remote_id_status.py
--rw-r--r--   0        0        0     2461 2024-03-26 16:52:10.643236 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_role.py
--rw-r--r--   0        0        0     2943 2024-03-26 16:52:10.647125 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py
--rw-r--r--   0        0        0     2642 2024-03-26 16:52:10.629609 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_room_compensation_state.py
--rw-r--r--   0        0        0     2597 2024-03-26 16:52:10.691597 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_software_update_state.py
--rw-r--r--   0        0        0     2524 2024-03-26 16:52:10.657486 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_sound_settings.py
--rw-r--r--   0        0        0     2487 2024-03-26 16:52:10.644441 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_source_change.py
--rw-r--r--   0        0        0     2135 2024-03-26 16:52:10.644535 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_speaker_group_changed.py
--rw-r--r--   0        0        0     2629 2024-03-26 16:52:10.661969 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_speaker_link_status_changed.py
--rw-r--r--   0        0        0     2536 2024-03-26 16:52:10.694372 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_stand_connected.py
--rw-r--r--   0        0        0     2524 2024-03-26 16:52:10.692710 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_stand_position.py
--rw-r--r--   0        0        0     2478 2024-03-26 16:52:10.694940 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_tv_info.py
--rw-r--r--   0        0        0     2460 2024-03-26 16:52:10.704517 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_volume.py
--rw-r--r--   0        0        0     2482 2024-03-26 16:52:10.695285 mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_wisa_out_state.py
--rw-r--r--   0        0        0     3208 2024-03-26 16:52:10.696690 mozart_api-3.4.1.8.4/mozart_api/models/websocket_notification_tag.py
--rw-r--r--   0        0        0     2199 2024-03-26 16:52:10.713461 mozart_api-3.4.1.8.4/mozart_api/models/wisa_out_state.py
--rw-r--r--   0        0        0    11539 2024-03-26 16:52:06.258978 mozart_api-3.4.1.8.4/mozart_api/mozart_cli.py
--rw-r--r--   0        0        0    23809 2024-03-26 16:52:06.384320 mozart_api-3.4.1.8.4/mozart_api/mozart_client.py
--rw-r--r--   0        0        0        0 2024-03-26 16:52:02.913401 mozart_api-3.4.1.8.4/mozart_api/py.typed
--rw-r--r--   0        0        0     9536 2024-03-26 16:52:06.232029 mozart_api-3.4.1.8.4/mozart_api/rest.py
--rw-r--r--   0        0        0     1427 2024-03-26 16:52:05.873088 mozart_api-3.4.1.8.4/pyproject.toml
--rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 mozart_api-3.4.1.8.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-04-11 13:52:30.256453 mozart_api-3.4.1.8.5/LICENSE
+-rw-r--r--   0        0        0     1899 2024-04-11 13:52:31.730456 mozart_api-3.4.1.8.5/README.md
+-rw-r--r--   0        0        0    15806 2024-04-11 13:52:32.941431 mozart_api-3.4.1.8.5/mozart_api/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-11 13:52:33.267147 mozart_api-3.4.1.8.5/mozart_api/api/__init__.py
+-rw-r--r--   0        0        0    58731 2024-04-11 13:52:33.782603 mozart_api-3.4.1.8.5/mozart_api/api/beolink_api.py
+-rw-r--r--   0        0        0     6011 2024-04-11 13:52:33.272519 mozart_api-3.4.1.8.5/mozart_api/api/bluetooth_api.py
+-rw-r--r--   0        0        0     7082 2024-04-11 13:52:33.298470 mozart_api-3.4.1.8.5/mozart_api/api/content_api.py
+-rw-r--r--   0        0        0     6838 2024-04-11 13:52:33.305402 mozart_api-3.4.1.8.5/mozart_api/api/deezer_api.py
+-rw-r--r--   0        0        0   310727 2024-04-11 13:52:35.273346 mozart_api-3.4.1.8.5/mozart_api/api/mozart_api.py
+-rw-r--r--   0        0        0     7367 2024-04-11 13:52:33.315997 mozart_api-3.4.1.8.5/mozart_api/api/overlay_api.py
+-rw-r--r--   0        0        0    64124 2024-04-11 13:52:33.908095 mozart_api-3.4.1.8.5/mozart_api/api/playback_api.py
+-rw-r--r--   0        0        0    15117 2024-04-11 13:52:33.435209 mozart_api-3.4.1.8.5/mozart_api/api/power_api.py
+-rw-r--r--   0        0        0    11808 2024-04-11 13:52:33.374223 mozart_api-3.4.1.8.5/mozart_api/api/product_api.py
+-rw-r--r--   0        0        0    17635 2024-04-11 13:52:33.538643 mozart_api-3.4.1.8.5/mozart_api/api/remote_api.py
+-rw-r--r--   0        0        0    21883 2024-04-11 13:52:33.624467 mozart_api-3.4.1.8.5/mozart_api/api/scenes_api.py
+-rw-r--r--   0        0        0    27504 2024-04-11 13:52:33.679934 mozart_api-3.4.1.8.5/mozart_api/api/settings_api.py
+-rw-r--r--   0        0        0     6010 2024-04-11 13:52:33.423295 mozart_api-3.4.1.8.5/mozart_api/api/software_update_api.py
+-rw-r--r--   0        0        0    69417 2024-04-11 13:52:34.100365 mozart_api-3.4.1.8.5/mozart_api/api/sound_api.py
+-rw-r--r--   0        0        0     5934 2024-04-11 13:52:33.527934 mozart_api-3.4.1.8.5/mozart_api/api/speaker_group_api.py
+-rw-r--r--   0        0        0     7541 2024-04-11 13:52:33.707271 mozart_api-3.4.1.8.5/mozart_api/api/stand_api.py
+-rw-r--r--   0        0        0    27639 2024-04-11 13:52:33.124981 mozart_api-3.4.1.8.5/mozart_api/api_client.py
+-rw-r--r--   0        0        0      913 2024-04-11 13:52:32.813371 mozart_api-3.4.1.8.5/mozart_api/api_response.py
+-rw-r--r--   0        0        0    14126 2024-04-11 13:52:32.986278 mozart_api-3.4.1.8.5/mozart_api/configuration.py
+-rw-r--r--   0        0        0     5369 2024-04-11 13:52:32.891074 mozart_api-3.4.1.8.5/mozart_api/exceptions.py
+-rw-r--r--   0        0        0    14480 2024-04-11 13:52:35.695378 mozart_api-3.4.1.8.5/mozart_api/models/__init__.py
+-rw-r--r--   0        0        0    12222 2024-04-11 13:52:35.759256 mozart_api-3.4.1.8.5/mozart_api/models/action.py
+-rw-r--r--   0        0        0     2691 2024-04-11 13:52:35.596349 mozart_api-3.4.1.8.5/mozart_api/models/alarm_timer_event_data.py
+-rw-r--r--   0        0        0     2098 2024-04-11 13:52:35.593091 mozart_api-3.4.1.8.5/mozart_api/models/alarm_triggered_info.py
+-rw-r--r--   0        0        0     1929 2024-04-11 13:52:35.587794 mozart_api-3.4.1.8.5/mozart_api/models/ambience.py
+-rw-r--r--   0        0        0     3156 2024-04-11 13:52:35.613057 mozart_api-3.4.1.8.5/mozart_api/models/ambience_feature.py
+-rw-r--r--   0        0        0     2926 2024-04-11 13:52:35.613087 mozart_api-3.4.1.8.5/mozart_api/models/ambience_range.py
+-rw-r--r--   0        0        0     2277 2024-04-11 13:52:35.614618 mozart_api-3.4.1.8.5/mozart_api/models/art.py
+-rw-r--r--   0        0        0     1920 2024-04-11 13:52:35.632650 mozart_api-3.4.1.8.5/mozart_api/models/balance.py
+-rw-r--r--   0        0        0     3100 2024-04-11 13:52:35.664038 mozart_api-3.4.1.8.5/mozart_api/models/balance_feature.py
+-rw-r--r--   0        0        0     2871 2024-04-11 13:52:35.648435 mozart_api-3.4.1.8.5/mozart_api/models/balance_range.py
+-rw-r--r--   0        0        0     1807 2024-04-11 13:52:35.647512 mozart_api-3.4.1.8.5/mozart_api/models/bass.py
+-rw-r--r--   0        0        0     3025 2024-04-11 13:52:35.685588 mozart_api-3.4.1.8.5/mozart_api/models/bass_feature.py
+-rw-r--r--   0        0        0     2152 2024-04-11 13:52:35.664209 mozart_api-3.4.1.8.5/mozart_api/models/bass_management.py
+-rw-r--r--   0        0        0     3416 2024-04-11 13:52:35.680064 mozart_api-3.4.1.8.5/mozart_api/models/bass_management_feature.py
+-rw-r--r--   0        0        0     2992 2024-04-11 13:52:35.696024 mozart_api-3.4.1.8.5/mozart_api/models/bass_management_range.py
+-rw-r--r--   0        0        0     2866 2024-04-11 13:52:35.693799 mozart_api-3.4.1.8.5/mozart_api/models/bass_range.py
+-rw-r--r--   0        0        0     2936 2024-04-11 13:52:35.698433 mozart_api-3.4.1.8.5/mozart_api/models/battery_state.py
+-rw-r--r--   0        0        0     2348 2024-04-11 13:52:35.709117 mozart_api-3.4.1.8.5/mozart_api/models/beo_remote_button.py
+-rw-r--r--   0        0        0     1955 2024-04-11 13:52:35.722077 mozart_api-3.4.1.8.5/mozart_api/models/beolink_available_listener.py
+-rw-r--r--   0        0        0     3904 2024-04-11 13:52:35.747730 mozart_api-3.4.1.8.5/mozart_api/models/beolink_experience.py
+-rw-r--r--   0        0        0     3408 2024-04-11 13:52:35.748267 mozart_api-3.4.1.8.5/mozart_api/models/beolink_experiences_result.py
+-rw-r--r--   0        0        0     2308 2024-04-11 13:52:35.784261 mozart_api-3.4.1.8.5/mozart_api/models/beolink_join_request.py
+-rw-r--r--   0        0        0     3741 2024-04-11 13:52:35.784137 mozart_api-3.4.1.8.5/mozart_api/models/beolink_join_result.py
+-rw-r--r--   0        0        0     2011 2024-04-11 13:52:35.738902 mozart_api-3.4.1.8.5/mozart_api/models/beolink_leader.py
+-rw-r--r--   0        0        0     1883 2024-04-11 13:52:35.763800 mozart_api-3.4.1.8.5/mozart_api/models/beolink_listener.py
+-rw-r--r--   0        0        0     1995 2024-04-11 13:52:35.789078 mozart_api-3.4.1.8.5/mozart_api/models/beolink_peer.py
+-rw-r--r--   0        0        0     2157 2024-04-11 13:52:35.819514 mozart_api-3.4.1.8.5/mozart_api/models/bluetooth_device.py
+-rw-r--r--   0        0        0     2511 2024-04-11 13:52:35.834016 mozart_api-3.4.1.8.5/mozart_api/models/bluetooth_device_list.py
+-rw-r--r--   0        0        0     2055 2024-04-11 13:52:35.809715 mozart_api-3.4.1.8.5/mozart_api/models/button_event.py
+-rw-r--r--   0        0        0     2154 2024-04-11 13:52:35.806596 mozart_api-3.4.1.8.5/mozart_api/models/compression.py
+-rw-r--r--   0        0        0     3395 2024-04-11 13:52:35.932213 mozart_api-3.4.1.8.5/mozart_api/models/compression_feature.py
+-rw-r--r--   0        0        0     2945 2024-04-11 13:52:35.923430 mozart_api-3.4.1.8.5/mozart_api/models/compression_range.py
+-rw-r--r--   0        0        0     3289 2024-04-11 13:52:35.878283 mozart_api-3.4.1.8.5/mozart_api/models/content_item.py
+-rw-r--r--   0        0        0     2313 2024-04-11 13:52:35.906039 mozart_api-3.4.1.8.5/mozart_api/models/directivity.py
+-rw-r--r--   0        0        0     3584 2024-04-11 13:52:36.007569 mozart_api-3.4.1.8.5/mozart_api/models/directivity_feature.py
+-rw-r--r--   0        0        0     2975 2024-04-11 13:52:35.935852 mozart_api-3.4.1.8.5/mozart_api/models/directivity_range.py
+-rw-r--r--   0        0        0     2569 2024-04-11 13:52:35.883597 mozart_api-3.4.1.8.5/mozart_api/models/error_model.py
+-rw-r--r--   0        0        0     1902 2024-04-11 13:52:35.878225 mozart_api-3.4.1.8.5/mozart_api/models/fader.py
+-rw-r--r--   0        0        0     3068 2024-04-11 13:52:35.943416 mozart_api-3.4.1.8.5/mozart_api/models/fader_feature.py
+-rw-r--r--   0        0        0     2841 2024-04-11 13:52:35.993690 mozart_api-3.4.1.8.5/mozart_api/models/fader_range.py
+-rw-r--r--   0        0        0     2109 2024-04-11 13:52:35.993298 mozart_api-3.4.1.8.5/mozart_api/models/hdmi_input.py
+-rw-r--r--   0        0        0     3078 2024-04-11 13:52:35.999010 mozart_api-3.4.1.8.5/mozart_api/models/hdmi_video_format.py
+-rw-r--r--   0        0        0     1863 2024-04-11 13:52:35.957677 mozart_api-3.4.1.8.5/mozart_api/models/home_control_ixp.py
+-rw-r--r--   0        0        0     2120 2024-04-11 13:52:35.994303 mozart_api-3.4.1.8.5/mozart_api/models/home_control_uri.py
+-rw-r--r--   0        0        0     2490 2024-04-11 13:52:36.006949 mozart_api-3.4.1.8.5/mozart_api/models/install_record_id_state.py
+-rw-r--r--   0        0        0     2341 2024-04-11 13:52:35.994553 mozart_api-3.4.1.8.5/mozart_api/models/latency_profile.py
+-rw-r--r--   0        0        0     3537 2024-04-11 13:52:36.059675 mozart_api-3.4.1.8.5/mozart_api/models/lge_tv_sound_settings.py
+-rw-r--r--   0        0        0     5261 2024-04-11 13:52:36.124139 mozart_api-3.4.1.8.5/mozart_api/models/listening_mode.py
+-rw-r--r--   0        0        0     9617 2024-04-11 13:52:36.139515 mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_features.py
+-rw-r--r--   0        0        0     5324 2024-04-11 13:52:36.092749 mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_props.py
+-rw-r--r--   0        0        0     2680 2024-04-11 13:52:36.159829 mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_ref.py
+-rw-r--r--   0        0        0     5084 2024-04-11 13:52:36.083934 mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_trigger.py
+-rw-r--r--   0        0        0     1826 2024-04-11 13:52:36.102558 mozart_api-3.4.1.8.5/mozart_api/models/loudness.py
+-rw-r--r--   0        0        0     2185 2024-04-11 13:52:36.073883 mozart_api-3.4.1.8.5/mozart_api/models/microphone_state.py
+-rw-r--r--   0        0        0     3104 2024-04-11 13:52:36.099449 mozart_api-3.4.1.8.5/mozart_api/models/microphones_state.py
+-rw-r--r--   0        0        0     4292 2024-04-11 13:52:36.139720 mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request.py
+-rw-r--r--   0        0        0     2565 2024-04-11 13:52:36.131911 mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_common.py
+-rw-r--r--   0        0        0     2508 2024-04-11 13:52:36.138663 mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_from_usb.py
+-rw-r--r--   0        0        0     2327 2024-04-11 13:52:36.143607 mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_from_usb_from_usb.py
+-rw-r--r--   0        0        0     2705 2024-04-11 13:52:36.143427 mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_text_to_speech.py
+-rw-r--r--   0        0        0     2839 2024-04-11 13:52:36.221835 mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py
+-rw-r--r--   0        0        0     2266 2024-04-11 13:52:36.159855 mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_uri.py
+-rw-r--r--   0        0        0     3168 2024-04-11 13:52:36.233384 mozart_api-3.4.1.8.5/mozart_api/models/paired_remote.py
+-rw-r--r--   0        0        0     2507 2024-04-11 13:52:36.165974 mozart_api-3.4.1.8.5/mozart_api/models/paired_remote_response.py
+-rw-r--r--   0        0        0     4250 2024-04-11 13:52:36.241903 mozart_api-3.4.1.8.5/mozart_api/models/play_queue_item.py
+-rw-r--r--   0        0        0     2244 2024-04-11 13:52:36.176132 mozart_api-3.4.1.8.5/mozart_api/models/play_queue_item_type.py
+-rw-r--r--   0        0        0     2603 2024-04-11 13:52:36.189368 mozart_api-3.4.1.8.5/mozart_api/models/play_queue_settings.py
+-rw-r--r--   0        0        0    10825 2024-04-11 13:52:36.344416 mozart_api-3.4.1.8.5/mozart_api/models/playback_content_metadata.py
+-rw-r--r--   0        0        0     2406 2024-04-11 13:52:36.237417 mozart_api-3.4.1.8.5/mozart_api/models/playback_error.py
+-rw-r--r--   0        0        0     2454 2024-04-11 13:52:36.211902 mozart_api-3.4.1.8.5/mozart_api/models/playback_progress.py
+-rw-r--r--   0        0        0     3724 2024-04-11 13:52:36.233044 mozart_api-3.4.1.8.5/mozart_api/models/playback_state.py
+-rw-r--r--   0        0        0     2400 2024-04-11 13:52:36.248156 mozart_api-3.4.1.8.5/mozart_api/models/power_link_trigger.py
+-rw-r--r--   0        0        0     2297 2024-04-11 13:52:36.289869 mozart_api-3.4.1.8.5/mozart_api/models/power_state_enum.py
+-rw-r--r--   0        0        0     4218 2024-04-11 13:52:36.307690 mozart_api-3.4.1.8.5/mozart_api/models/preset.py
+-rw-r--r--   0        0        0     2450 2024-04-11 13:52:36.261293 mozart_api-3.4.1.8.5/mozart_api/models/product_curtain_status.py
+-rw-r--r--   0        0        0     2115 2024-04-11 13:52:36.289745 mozart_api-3.4.1.8.5/mozart_api/models/product_friendly_name.py
+-rw-r--r--   0        0        0     5961 2024-04-11 13:52:36.374277 mozart_api-3.4.1.8.5/mozart_api/models/product_state.py
+-rw-r--r--   0        0        0     7432 2024-04-11 13:52:36.349491 mozart_api-3.4.1.8.5/mozart_api/models/remote_menu_item.py
+-rw-r--r--   0        0        0     6374 2024-04-11 13:52:36.337738 mozart_api-3.4.1.8.5/mozart_api/models/remote_menu_item_properties.py
+-rw-r--r--   0        0        0     2725 2024-04-11 13:52:36.289769 mozart_api-3.4.1.8.5/mozart_api/models/remote_ui_key_state.py
+-rw-r--r--   0        0        0     2452 2024-04-11 13:52:36.345629 mozart_api-3.4.1.8.5/mozart_api/models/rendering_state.py
+-rw-r--r--   0        0        0     2109 2024-04-11 13:52:36.345066 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation.py
+-rw-r--r--   0        0        0     2954 2024-04-11 13:52:36.345050 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_current_measurement.py
+-rw-r--r--   0        0        0     1930 2024-04-11 13:52:36.344540 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_debug.py
+-rw-r--r--   0        0        0     1946 2024-04-11 13:52:36.390612 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_enabled.py
+-rw-r--r--   0        0        0     2928 2024-04-11 13:52:36.416591 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_error_details.py
+-rw-r--r--   0        0        0     2941 2024-04-11 13:52:36.463048 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_feature.py
+-rw-r--r--   0        0        0     4982 2024-04-11 13:52:36.463797 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_info.py
+-rw-r--r--   0        0        0     4193 2024-04-11 13:52:36.399290 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_measurement_error.py
+-rw-r--r--   0        0        0     7257 2024-04-11 13:52:36.466127 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_properties.py
+-rw-r--r--   0        0        0     2641 2024-04-11 13:52:36.416288 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_range.py
+-rw-r--r--   0        0        0     2112 2024-04-11 13:52:36.423391 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_response.py
+-rw-r--r--   0        0        0     5746 2024-04-11 13:52:36.502931 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_result.py
+-rw-r--r--   0        0        0     6762 2024-04-11 13:52:36.478327 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_state.py
+-rw-r--r--   0        0        0     2383 2024-04-11 13:52:36.528393 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_state_value.py
+-rw-r--r--   0        0        0     2589 2024-04-11 13:52:36.483507 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_type.py
+-rw-r--r--   0        0        0     2109 2024-04-11 13:52:36.482389 mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_version.py
+-rw-r--r--   0        0        0     4507 2024-04-11 13:52:36.539386 mozart_api-3.4.1.8.5/mozart_api/models/scene.py
+-rw-r--r--   0        0        0     2630 2024-04-11 13:52:36.545567 mozart_api-3.4.1.8.5/mozart_api/models/scene_classification.py
+-rw-r--r--   0        0        0     2296 2024-04-11 13:52:36.519879 mozart_api-3.4.1.8.5/mozart_api/models/scene_match.py
+-rw-r--r--   0        0        0     3814 2024-04-11 13:52:36.557579 mozart_api-3.4.1.8.5/mozart_api/models/scene_properties.py
+-rw-r--r--   0        0        0     2951 2024-04-11 13:52:36.539030 mozart_api-3.4.1.8.5/mozart_api/models/scene_trigger_base_properties.py
+-rw-r--r--   0        0        0     3212 2024-04-11 13:52:36.547895 mozart_api-3.4.1.8.5/mozart_api/models/software_update_state.py
+-rw-r--r--   0        0        0     3777 2024-04-11 13:52:36.582380 mozart_api-3.4.1.8.5/mozart_api/models/software_update_status.py
+-rw-r--r--   0        0        0     2802 2024-04-11 13:52:36.585372 mozart_api-3.4.1.8.5/mozart_api/models/sound_adjustments.py
+-rw-r--r--   0        0        0    11529 2024-04-11 13:52:36.714297 mozart_api-3.4.1.8.5/mozart_api/models/sound_feature_set.py
+-rw-r--r--   0        0        0     3508 2024-04-11 13:52:36.595886 mozart_api-3.4.1.8.5/mozart_api/models/sound_settings.py
+-rw-r--r--   0        0        0     2086 2024-04-11 13:52:36.583527 mozart_api-3.4.1.8.5/mozart_api/models/sound_tone_touch.py
+-rw-r--r--   0        0        0     3092 2024-04-11 13:52:36.612574 mozart_api-3.4.1.8.5/mozart_api/models/source.py
+-rw-r--r--   0        0        0     2410 2024-04-11 13:52:36.581025 mozart_api-3.4.1.8.5/mozart_api/models/source_array.py
+-rw-r--r--   0        0        0     2128 2024-04-11 13:52:36.614732 mozart_api-3.4.1.8.5/mozart_api/models/source_type_enum.py
+-rw-r--r--   0        0        0     2020 2024-04-11 13:52:36.609378 mozart_api-3.4.1.8.5/mozart_api/models/spatial_envelopment.py
+-rw-r--r--   0        0        0     3293 2024-04-11 13:52:36.671071 mozart_api-3.4.1.8.5/mozart_api/models/spatial_envelopment_feature.py
+-rw-r--r--   0        0        0     3052 2024-04-11 13:52:36.648434 mozart_api-3.4.1.8.5/mozart_api/models/spatial_envelopment_range.py
+-rw-r--r--   0        0        0     1975 2024-04-11 13:52:36.649311 mozart_api-3.4.1.8.5/mozart_api/models/spatial_height.py
+-rw-r--r--   0        0        0     3213 2024-04-11 13:52:36.657719 mozart_api-3.4.1.8.5/mozart_api/models/spatial_height_feature.py
+-rw-r--r--   0        0        0     2977 2024-04-11 13:52:36.649425 mozart_api-3.4.1.8.5/mozart_api/models/spatial_height_range.py
+-rw-r--r--   0        0        0     2251 2024-04-11 13:52:36.671045 mozart_api-3.4.1.8.5/mozart_api/models/spatial_processing.py
+-rw-r--r--   0        0        0     3536 2024-04-11 13:52:36.671081 mozart_api-3.4.1.8.5/mozart_api/models/spatial_processing_feature.py
+-rw-r--r--   0        0        0     3037 2024-04-11 13:52:36.703296 mozart_api-3.4.1.8.5/mozart_api/models/spatial_processing_range.py
+-rw-r--r--   0        0        0     1993 2024-04-11 13:52:36.688982 mozart_api-3.4.1.8.5/mozart_api/models/spatial_surround.py
+-rw-r--r--   0        0        0     3245 2024-04-11 13:52:36.700440 mozart_api-3.4.1.8.5/mozart_api/models/spatial_surround_feature.py
+-rw-r--r--   0        0        0     3007 2024-04-11 13:52:36.703972 mozart_api-3.4.1.8.5/mozart_api/models/spatial_surround_range.py
+-rw-r--r--   0        0        0     1966 2024-04-11 13:52:36.709171 mozart_api-3.4.1.8.5/mozart_api/models/spatial_width.py
+-rw-r--r--   0        0        0     3197 2024-04-11 13:52:36.734387 mozart_api-3.4.1.8.5/mozart_api/models/spatial_width_feature.py
+-rw-r--r--   0        0        0     2962 2024-04-11 13:52:36.729960 mozart_api-3.4.1.8.5/mozart_api/models/spatial_width_range.py
+-rw-r--r--   0        0        0     6763 2024-04-11 13:52:36.797475 mozart_api-3.4.1.8.5/mozart_api/models/speaker_group.py
+-rw-r--r--   0        0        0     5135 2024-04-11 13:52:36.780245 mozart_api-3.4.1.8.5/mozart_api/models/speaker_group_member.py
+-rw-r--r--   0        0        0     2692 2024-04-11 13:52:36.759460 mozart_api-3.4.1.8.5/mozart_api/models/speaker_group_member_location.py
+-rw-r--r--   0        0        0     2242 2024-04-11 13:52:36.734415 mozart_api-3.4.1.8.5/mozart_api/models/speaker_group_overview.py
+-rw-r--r--   0        0        0     4491 2024-04-11 13:52:36.872856 mozart_api-3.4.1.8.5/mozart_api/models/speaker_link_member_status.py
+-rw-r--r--   0        0        0     3059 2024-04-11 13:52:36.760389 mozart_api-3.4.1.8.5/mozart_api/models/speaker_link_status.py
+-rw-r--r--   0        0        0     2249 2024-04-11 13:52:36.778829 mozart_api-3.4.1.8.5/mozart_api/models/speaker_role_enum.py
+-rw-r--r--   0        0        0     1975 2024-04-11 13:52:36.779209 mozart_api-3.4.1.8.5/mozart_api/models/speech_enhance.py
+-rw-r--r--   0        0        0     3213 2024-04-11 13:52:36.793561 mozart_api-3.4.1.8.5/mozart_api/models/speech_enhance_feature.py
+-rw-r--r--   0        0        0     2977 2024-04-11 13:52:36.817724 mozart_api-3.4.1.8.5/mozart_api/models/speech_enhance_range.py
+-rw-r--r--   0        0        0     1890 2024-04-11 13:52:36.815535 mozart_api-3.4.1.8.5/mozart_api/models/stand_connected.py
+-rw-r--r--   0        0        0     3105 2024-04-11 13:52:36.825145 mozart_api-3.4.1.8.5/mozart_api/models/stand_movement.py
+-rw-r--r--   0        0        0     1916 2024-04-11 13:52:36.826177 mozart_api-3.4.1.8.5/mozart_api/models/stand_position.py
+-rw-r--r--   0        0        0     2557 2024-04-11 13:52:36.849000 mozart_api-3.4.1.8.5/mozart_api/models/tone_touch.py
+-rw-r--r--   0        0        0     1916 2024-04-11 13:52:36.826599 mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_type.py
+-rw-r--r--   0        0        0     3007 2024-04-11 13:52:36.849619 mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_type_range.py
+-rw-r--r--   0        0        0     3160 2024-04-11 13:52:36.875084 mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_x_feature.py
+-rw-r--r--   0        0        0     3160 2024-04-11 13:52:36.909037 mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_y_feature.py
+-rw-r--r--   0        0        0     1825 2024-04-11 13:52:36.858031 mozart_api-3.4.1.8.5/mozart_api/models/treble.py
+-rw-r--r--   0        0        0     3057 2024-04-11 13:52:36.867064 mozart_api-3.4.1.8.5/mozart_api/models/treble_feature.py
+-rw-r--r--   0        0        0     2896 2024-04-11 13:52:36.877520 mozart_api-3.4.1.8.5/mozart_api/models/treble_range.py
+-rw-r--r--   0        0        0     2352 2024-04-11 13:52:36.903993 mozart_api-3.4.1.8.5/mozart_api/models/tv_info_event_data.py
+-rw-r--r--   0        0        0     2225 2024-04-11 13:52:36.894982 mozart_api-3.4.1.8.5/mozart_api/models/tv_integration_types.py
+-rw-r--r--   0        0        0     3086 2024-04-11 13:52:36.922708 mozart_api-3.4.1.8.5/mozart_api/models/tv_properties.py
+-rw-r--r--   0        0        0     2281 2024-04-11 13:52:36.908749 mozart_api-3.4.1.8.5/mozart_api/models/tv_sound_settings.py
+-rw-r--r--   0        0        0     3366 2024-04-11 13:52:36.925050 mozart_api-3.4.1.8.5/mozart_api/models/tv_state.py
+-rw-r--r--   0        0        0     1795 2024-04-11 13:52:36.907854 mozart_api-3.4.1.8.5/mozart_api/models/uri.py
+-rw-r--r--   0        0        0     1866 2024-04-11 13:52:36.908864 mozart_api-3.4.1.8.5/mozart_api/models/user_flow.py
+-rw-r--r--   0        0        0     3886 2024-04-11 13:52:37.066035 mozart_api-3.4.1.8.5/mozart_api/models/video_pixel_format.py
+-rw-r--r--   0        0        0     2599 2024-04-11 13:52:36.944543 mozart_api-3.4.1.8.5/mozart_api/models/video_timings.py
+-rw-r--r--   0        0        0     1847 2024-04-11 13:52:36.998760 mozart_api-3.4.1.8.5/mozart_api/models/volume_level.py
+-rw-r--r--   0        0        0     1842 2024-04-11 13:52:36.944403 mozart_api-3.4.1.8.5/mozart_api/models/volume_mute.py
+-rw-r--r--   0        0        0     2692 2024-04-11 13:52:36.998822 mozart_api-3.4.1.8.5/mozart_api/models/volume_settings.py
+-rw-r--r--   0        0        0     3507 2024-04-11 13:52:37.000570 mozart_api-3.4.1.8.5/mozart_api/models/volume_state.py
+-rw-r--r--   0        0        0     2659 2024-04-11 13:52:36.999169 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_active_hdmi_input_signal.py
+-rw-r--r--   0        0        0     2680 2024-04-11 13:52:37.038668 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_active_listening_mode.py
+-rw-r--r--   0        0        0     2680 2024-04-11 13:52:37.027413 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_active_speaker_group.py
+-rw-r--r--   0        0        0     2613 2024-04-11 13:52:37.029503 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_alarm_timer.py
+-rw-r--r--   0        0        0     2640 2024-04-11 13:52:37.091117 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_alarm_triggered.py
+-rw-r--r--   0        0        0     2559 2024-04-11 13:52:37.037902 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_battery.py
+-rw-r--r--   0        0        0     2636 2024-04-11 13:52:37.053750 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_beo_remote_button.py
+-rw-r--r--   0        0        0     2693 2024-04-11 13:52:37.052442 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_beolink_experiences_result.py
+-rw-r--r--   0        0        0     2609 2024-04-11 13:52:37.074595 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_beolink_join_result.py
+-rw-r--r--   0        0        0     2547 2024-04-11 13:52:37.074568 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_button.py
+-rw-r--r--   0        0        0     2600 2024-04-11 13:52:37.073643 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_curtains.py
+-rw-r--r--   0        0        0     2684 2024-04-11 13:52:37.074284 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_hdmi_video_format_signal.py
+-rw-r--r--   0        0        0     2688 2024-04-11 13:52:37.104502 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_notification.py
+-rw-r--r--   0        0        0     2611 2024-04-11 13:52:37.108518 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_error.py
+-rw-r--r--   0        0        0     2676 2024-04-11 13:52:37.150944 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_metadata.py
+-rw-r--r--   0        0        0     2647 2024-04-11 13:52:37.104473 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_progress.py
+-rw-r--r--   0        0        0     2590 2024-04-11 13:52:37.139475 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_source.py
+-rw-r--r--   0        0        0     2615 2024-04-11 13:52:37.104493 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_state.py
+-rw-r--r--   0        0        0     2592 2024-04-11 13:52:37.137062 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_power_state.py
+-rw-r--r--   0        0        0     2729 2024-04-11 13:52:37.151083 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_puc_install_remote_id_status.py
+-rw-r--r--   0        0        0     2548 2024-04-11 13:52:37.151423 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_role.py
+-rw-r--r--   0        0        0     3030 2024-04-11 13:52:37.153411 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py
+-rw-r--r--   0        0        0     2729 2024-04-11 13:52:37.148020 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_room_compensation_state.py
+-rw-r--r--   0        0        0     2684 2024-04-11 13:52:37.151826 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_software_update_state.py
+-rw-r--r--   0        0        0     2611 2024-04-11 13:52:37.213474 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_sound_settings.py
+-rw-r--r--   0        0        0     2574 2024-04-11 13:52:37.205188 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_source_change.py
+-rw-r--r--   0        0        0     2221 2024-04-11 13:52:37.181550 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_speaker_group_changed.py
+-rw-r--r--   0        0        0     2716 2024-04-11 13:52:37.182449 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_speaker_link_status_changed.py
+-rw-r--r--   0        0        0     2623 2024-04-11 13:52:37.206767 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_stand_connected.py
+-rw-r--r--   0        0        0     2611 2024-04-11 13:52:37.176596 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_stand_position.py
+-rw-r--r--   0        0        0     2565 2024-04-11 13:52:37.192794 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_tv_info.py
+-rw-r--r--   0        0        0     2547 2024-04-11 13:52:37.202598 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_volume.py
+-rw-r--r--   0        0        0     2568 2024-04-11 13:52:37.207618 mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_wisa_out_state.py
+-rw-r--r--   0        0        0     3298 2024-04-11 13:52:37.219797 mozart_api-3.4.1.8.5/mozart_api/models/websocket_notification_tag.py
+-rw-r--r--   0        0        0     2289 2024-04-11 13:52:37.214466 mozart_api-3.4.1.8.5/mozart_api/models/wisa_out_state.py
+-rw-r--r--   0        0        0    11539 2024-04-11 13:52:33.001494 mozart_api-3.4.1.8.5/mozart_api/mozart_cli.py
+-rw-r--r--   0        0        0    23809 2024-04-11 13:52:33.085664 mozart_api-3.4.1.8.5/mozart_api/mozart_client.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:52:30.179739 mozart_api-3.4.1.8.5/mozart_api/py.typed
+-rw-r--r--   0        0        0     9536 2024-04-11 13:52:32.954274 mozart_api-3.4.1.8.5/mozart_api/rest.py
+-rw-r--r--   0        0        0     1422 2024-04-11 13:52:32.421106 mozart_api-3.4.1.8.5/pyproject.toml
+-rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 mozart_api-3.4.1.8.5/PKG-INFO
```

### Comparing `mozart_api-3.4.1.8.4/LICENSE` & `mozart_api-3.4.1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/README.md` & `mozart_api-3.4.1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/mozart_api/__init__.py` & `mozart_api-3.4.1.8.5/mozart_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: support@bang-olufsen.dk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "3.4.1.8.4"
+__version__ = "3.4.1.8.5"
 
 # import apis into sdk package
 from mozart_api.api.beolink_api import BeolinkApi
 from mozart_api.api.bluetooth_api import BluetoothApi
 from mozart_api.api.content_api import ContentApi
 from mozart_api.api.deezer_api import DeezerApi
 from mozart_api.api.overlay_api import OverlayApi
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/__init__.py` & `mozart_api-3.4.1.8.5/mozart_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/beolink_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/beolink_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictStr
+
+try:
+    from pydantic.v1 import Field, StrictStr
+except ImportError:
+    from pydantic import Field, StrictStr
+
 
 from typing import List, Optional
 
 from mozart_api.models.beolink_available_listener import BeolinkAvailableListener
 from mozart_api.models.beolink_join_request import BeolinkJoinRequest
 from mozart_api.models.beolink_join_result import BeolinkJoinResult
 from mozart_api.models.beolink_listener import BeolinkListener
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/bluetooth_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/bluetooth_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from mozart_api.models.bluetooth_device_list import BluetoothDeviceList
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
 from mozart_api.exceptions import ApiTypeError, ApiValueError  # noqa: F401
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/content_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/content_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictStr
+
+try:
+    from pydantic.v1 import Field, StrictStr
+except ImportError:
+    from pydantic import Field, StrictStr
+
 
 from typing import Dict, Optional
 
 from mozart_api.models.content_item import ContentItem
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/deezer_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/deezer_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field
+
+try:
+    from pydantic.v1 import Field
+except ImportError:
+    from pydantic import Field
+
 
 from typing import Optional
 
 from mozart_api.models.user_flow import UserFlow
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/mozart_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/mozart_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBool, StrictInt, StrictStr, conint
+
+try:
+    from pydantic.v1 import Field, StrictBool, StrictInt, StrictStr, conint
+except ImportError:
+    from pydantic import Field, StrictBool, StrictInt, StrictStr, conint
+
 
 from typing import Any, Dict, List, Optional
 
 from mozart_api.models.bass import Bass
 from mozart_api.models.battery_state import BatteryState
 from mozart_api.models.beolink_available_listener import BeolinkAvailableListener
 from mozart_api.models.beolink_join_request import BeolinkJoinRequest
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/overlay_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/overlay_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field
+
+try:
+    from pydantic.v1 import Field
+except ImportError:
+    from pydantic import Field
+
 
 from mozart_api.models.overlay_play_request import OverlayPlayRequest
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
 from mozart_api.exceptions import ApiTypeError, ApiValueError  # noqa: F401
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/playback_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/playback_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBool, StrictInt, StrictStr
+
+try:
+    from pydantic.v1 import Field, StrictBool, StrictInt, StrictStr
+except ImportError:
+    from pydantic import Field, StrictBool, StrictInt, StrictStr
+
 
 from typing import Any, Dict, Optional
 
 from mozart_api.models.play_queue_item import PlayQueueItem
 from mozart_api.models.play_queue_settings import PlayQueueSettings
 from mozart_api.models.playback_state import PlaybackState
 from mozart_api.models.source_array import SourceArray
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/power_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/power_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from mozart_api.models.battery_state import BatteryState
 from mozart_api.models.power_state_enum import PowerStateEnum
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/product_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/product_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field
+
+try:
+    from pydantic.v1 import Field
+except ImportError:
+    from pydantic import Field
+
 
 from mozart_api.models.product_friendly_name import ProductFriendlyName
 from mozart_api.models.product_state import ProductState
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
 from mozart_api.exceptions import ApiTypeError, ApiValueError  # noqa: F401
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/remote_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/remote_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictStr
+
+try:
+    from pydantic.v1 import Field, StrictStr
+except ImportError:
+    from pydantic import Field, StrictStr
+
 
 from typing import Dict, Optional
 
 from mozart_api.models.remote_menu_item import RemoteMenuItem
 from mozart_api.models.remote_ui_key_state import RemoteUIKeyState
 
 from mozart_api.api_client import ApiClient
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/scenes_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/scenes_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictStr
+
+try:
+    from pydantic.v1 import Field, StrictStr
+except ImportError:
+    from pydantic import Field, StrictStr
+
 
 from typing import Dict
 
 from mozart_api.models.scene import Scene
 from mozart_api.models.scene_match import SceneMatch
 from mozart_api.models.scene_properties import SceneProperties
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/settings_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/settings_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field
+
+try:
+    from pydantic.v1 import Field
+except ImportError:
+    from pydantic import Field
+
 
 from typing import Dict
 
 from mozart_api.models.home_control_ixp import HomeControlIxp
 from mozart_api.models.home_control_uri import HomeControlUri
 from mozart_api.models.paired_remote_response import PairedRemoteResponse
 from mozart_api.models.preset import Preset
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/software_update_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/software_update_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from mozart_api.models.software_update_status import SoftwareUpdateStatus
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
 from mozart_api.exceptions import ApiTypeError, ApiValueError  # noqa: F401
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/sound_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/sound_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, conint
+
+try:
+    from pydantic.v1 import Field, conint
+except ImportError:
+    from pydantic import Field, conint
+
 
 from typing import Dict, List
 
 from mozart_api.models.bass import Bass
 from mozart_api.models.directivity import Directivity
 from mozart_api.models.listening_mode import ListeningMode
 from mozart_api.models.listening_mode_ref import ListeningModeRef
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/speaker_group_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/speaker_group_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from mozart_api.models.speaker_group_overview import SpeakerGroupOverview
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
 from mozart_api.exceptions import ApiTypeError, ApiValueError  # noqa: F401
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api/stand_api.py` & `mozart_api-3.4.1.8.5/mozart_api/api/stand_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+
+try:
+    from pydantic.v1 import validate_arguments, ValidationError
+except ImportError:
+    from pydantic import validate_arguments, ValidationError
+
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBool
+
+try:
+    from pydantic.v1 import Field, StrictBool
+except ImportError:
+    from pydantic import Field, StrictBool
+
 
 from typing import Optional
 
 from mozart_api.models.stand_movement import StandMovement
 
 from mozart_api.api_client import ApiClient
 from mozart_api.api_response import ApiResponse
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api_client.py` & `mozart_api-3.4.1.8.5/mozart_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "OpenAPI-Generator/3.4.1.8.4/python"
+        self.user_agent = "OpenAPI-Generator/3.4.1.8.5/python"
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/api_response.py` & `mozart_api-3.4.1.8.5/mozart_api/api_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """API response object."""
 
 from __future__ import annotations
 from typing import Any, Dict, Optional
-from pydantic import Field, StrictInt, StrictStr
+
+try:
+    from pydantic.v1 import Field, StrictInt, StrictStr
+except ImportError:
+    from pydantic import Field, StrictInt, StrictStr
 
 
 class ApiResponse:
     """
     API response object
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/configuration.py` & `mozart_api-3.4.1.8.5/mozart_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 0.2.0\n"
-            "SDK Package Version: 3.4.1.8.4".format(
+            "SDK Package Version: 3.4.1.8.5".format(
                 env=sys.platform, pyversion=sys.version
             )
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/exceptions.py` & `mozart_api-3.4.1.8.5/mozart_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/__init__.py` & `mozart_api-3.4.1.8.5/mozart_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/action.py` & `mozart_api-3.4.1.8.5/mozart_api/models/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
-from pydantic import BaseModel, Field, StrictStr, confloat, conint, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, confloat, conint, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, confloat, conint, validator
+
 from mozart_api.models.play_queue_item import PlayQueueItem
 from mozart_api.models.play_queue_settings import PlayQueueSettings
 from mozart_api.models.source_type_enum import SourceTypeEnum
 from mozart_api.models.stand_position import StandPosition
 
 
 class Action(BaseModel):
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/alarm_timer_event_data.py` & `mozart_api-3.4.1.8.5/mozart_api/models/alarm_timer_event_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class AlarmTimerEventData(BaseModel):
     """
     AlarmTimerEventData
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/alarm_triggered_info.py` & `mozart_api-3.4.1.8.5/mozart_api/models/alarm_triggered_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, constr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, constr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, constr
 
 
 class AlarmTriggeredInfo(BaseModel):
     """
     AlarmTriggeredInfo
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/ambience.py` & `mozart_api-3.4.1.8.5/mozart_api/models/ambience.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
 
 class Ambience(BaseModel):
     """
     Ambience
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/ambience_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/ambience_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.ambience import Ambience
 
 
 class AmbienceFeature(BaseModel):
     """
     AmbienceFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/ambience_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/ambience_range.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.ambience import Ambience
 
 
 class AmbienceRange(BaseModel):
     """
     AmbienceRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/art.py` & `mozart_api-3.4.1.8.5/mozart_api/models/art.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr
 
 
 class Art(BaseModel):
     """
     Art
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/balance.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speech_enhance.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
-class Balance(BaseModel):
+
+class SpeechEnhance(BaseModel):
     """
-    Balance
+    SpeechEnhance
     """
 
     value: Union[StrictFloat, StrictInt] = Field(
-        ..., description="Selected balance value"
+        ..., description="Selected speech-enhance value"
     )
     __properties = ["value"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -44,27 +48,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Balance:
-        """Create an instance of Balance from a JSON string"""
+    def from_json(cls, json_str: str) -> SpeechEnhance:
+        """Create an instance of SpeechEnhance from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Balance:
-        """Create an instance of Balance from a dict"""
+    def from_dict(cls, obj: dict) -> SpeechEnhance:
+        """Create an instance of SpeechEnhance from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Balance.parse_obj(obj)
+            return SpeechEnhance.parse_obj(obj)
 
-        _obj = Balance.parse_obj({"value": obj.get("value")})
+        _obj = SpeechEnhance.parse_obj({"value": obj.get("value")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/balance_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/balance_feature.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.balance import Balance
 
 
 class BalanceFeature(BaseModel):
     """
     BalanceFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/balance_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/balance_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.balance import Balance
 
 
 class BalanceRange(BaseModel):
     """
     BalanceRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bass.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bass.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictInt
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt
 
 
 class Bass(BaseModel):
     """
     Bass
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bass_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bass_feature.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, conlist
+
 from mozart_api.models.bass import Bass
 
 
 class BassFeature(BaseModel):
     """
     BassFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bass_management.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bass_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr, validator
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class BassManagement(BaseModel):
     """
     BassManagement
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bass_management_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bass_management_feature.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.bass_management import BassManagement
 
 
 class BassManagementFeature(BaseModel):
     """
     BassManagementFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bass_management_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bass_management_range.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.bass_management import BassManagement
 
 
 class BassManagementRange(BaseModel):
     """
     BassManagementRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bass_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bass_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.bass import Bass
 
 
 class BassRange(BaseModel):
     """
     BassRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/battery_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/battery_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictInt
 
 
 class BatteryState(BaseModel):
     """
     BatteryState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beo_remote_button.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beo_remote_button.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class BeoRemoteButton(BaseModel):
     """
     BeoRemoteButton
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_available_listener.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_available_listener.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class BeolinkAvailableListener(BaseModel):
     """
     BeolinkAvailableListener
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_experience.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_experience.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
 
 
 class BeolinkExperience(BaseModel):
     """
     BeolinkExperience
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_experiences_result.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_experiences_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.beolink_experience import BeolinkExperience
 
 
 class BeolinkExperiencesResult(BaseModel):
     """
     BeolinkExperiencesResult
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_join_request.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_join_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class BeolinkJoinRequest(BaseModel):
     """
     BeolinkJoinRequest
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_join_result.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_join_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class BeolinkJoinResult(BaseModel):
     """
     BeolinkJoinResult
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_leader.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_leader.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class BeolinkLeader(BaseModel):
     """
     BeolinkLeader
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_listener.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_listener.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class BeolinkListener(BaseModel):
     """
     BeolinkListener
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/beolink_peer.py` & `mozart_api-3.4.1.8.5/mozart_api/models/beolink_peer.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class BeolinkPeer(BaseModel):
     """
     BeolinkPeer
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bluetooth_device.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bluetooth_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictBool, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, StrictBool, StrictStr
+except ImportError:
+    from pydantic import BaseModel, StrictBool, StrictStr
 
 
 class BluetoothDevice(BaseModel):
     """
     BluetoothDevice
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/bluetooth_device_list.py` & `mozart_api-3.4.1.8.5/mozart_api/models/bluetooth_device_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, conlist
+
+try:
+    from pydantic.v1 import BaseModel, conlist
+except ImportError:
+    from pydantic import BaseModel, conlist
+
 from mozart_api.models.bluetooth_device import BluetoothDevice
 
 
 class BluetoothDeviceList(BaseModel):
     """
     BluetoothDeviceList
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/button_event.py` & `mozart_api-3.4.1.8.5/mozart_api/models/button_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class ButtonEvent(BaseModel):
     """
     ButtonEvent
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/compression.py` & `mozart_api-3.4.1.8.5/mozart_api/models/compression.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr, validator
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class Compression(BaseModel):
     """
     Compression
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/compression_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/compression_feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.compression import Compression
 
 
 class CompressionFeature(BaseModel):
     """
     CompressionFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/compression_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/compression_range.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.compression import Compression
 
 
 class CompressionRange(BaseModel):
     """
     CompressionRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/content_item.py` & `mozart_api-3.4.1.8.5/mozart_api/models/content_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.source_type_enum import SourceTypeEnum
 
 
 class ContentItem(BaseModel):
     """
     ContentItem
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/directivity.py` & `mozart_api-3.4.1.8.5/mozart_api/models/directivity.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr, validator
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class Directivity(BaseModel):
     """
     Directivity
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/directivity_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/directivity_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.directivity import Directivity
 
 
 class DirectivityFeature(BaseModel):
     """
     DirectivityFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/directivity_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/directivity_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.directivity import Directivity
 
 
 class DirectivityRange(BaseModel):
     """
     DirectivityRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/error_model.py` & `mozart_api-3.4.1.8.5/mozart_api/models/error_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class ErrorModel(BaseModel):
     """
     the general error model  # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/fader.py` & `mozart_api-3.4.1.8.5/mozart_api/models/fader.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
 
 class Fader(BaseModel):
     """
     Fader
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/fader_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/fader_feature.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.fader import Fader
 
 
 class FaderFeature(BaseModel):
     """
     FaderFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/fader_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/fader_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.fader import Fader
 
 
 class FaderRange(BaseModel):
     """
     FaderRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/hdmi_input.py` & `mozart_api-3.4.1.8.5/mozart_api/models/hdmi_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class HdmiInput(BaseModel):
     """
     HdmiInput
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/hdmi_video_format.py` & `mozart_api-3.4.1.8.5/mozart_api/models/hdmi_video_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, conint
+
+try:
+    from pydantic.v1 import BaseModel, Field, conint
+except ImportError:
+    from pydantic import BaseModel, Field, conint
+
 from mozart_api.models.video_pixel_format import VideoPixelFormat
 from mozart_api.models.video_timings import VideoTimings
 
 
 class HdmiVideoFormat(BaseModel):
     """
     HdmiVideoFormat
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/home_control_ixp.py` & `mozart_api-3.4.1.8.5/mozart_api/models/home_control_ixp.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr
+except ImportError:
+    from pydantic import BaseModel, StrictStr
 
 
 class HomeControlIxp(BaseModel):
     """
     HomeControlIxp
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/home_control_uri.py` & `mozart_api-3.4.1.8.5/mozart_api/models/home_control_uri.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr
+except ImportError:
+    from pydantic import BaseModel, StrictStr
 
 
 class HomeControlUri(BaseModel):
     """
     HomeControlUri
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/install_record_id_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/install_record_id_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class InstallRecordIdState(BaseModel):
     """
     InstallRecordIdState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/latency_profile.py` & `mozart_api-3.4.1.8.5/mozart_api/models/latency_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class LatencyProfile(BaseModel):
     """
     The latency profile of this speaker group. Needed to handle Beolab's with latency dependant audio quality. Default is set to performance.   # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/lge_tv_sound_settings.py` & `mozart_api-3.4.1.8.5/mozart_api/models/lge_tv_sound_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
 
 
 class LgeTvSoundSettings(BaseModel):
     """
     LgeTvSoundSettings
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/listening_mode.py` & `mozart_api-3.4.1.8.5/mozart_api/models/listening_mode.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conint, conlist, constr, validator
+
+try:
+    from pydantic.v1 import (
+        BaseModel,
+        Field,
+        StrictStr,
+        conint,
+        conlist,
+        constr,
+        validator,
+    )
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conint, conlist, constr, validator
+
 from mozart_api.models.listening_mode_features import ListeningModeFeatures
 from mozart_api.models.listening_mode_trigger import ListeningModeTrigger
 
 
 class ListeningMode(BaseModel):
     """
     ListeningMode
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_features.py` & `mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.ambience import Ambience
 from mozart_api.models.balance import Balance
 from mozart_api.models.bass_management import BassManagement
 from mozart_api.models.compression import Compression
 from mozart_api.models.directivity import Directivity
 from mozart_api.models.fader import Fader
 from mozart_api.models.room_compensation import RoomCompensation
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_props.py` & `mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_props.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conint, conlist, constr, validator
+
+try:
+    from pydantic.v1 import (
+        BaseModel,
+        Field,
+        StrictStr,
+        conint,
+        conlist,
+        constr,
+        validator,
+    )
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conint, conlist, constr, validator
+
 from mozart_api.models.listening_mode_features import ListeningModeFeatures
 from mozart_api.models.listening_mode_trigger import ListeningModeTrigger
 
 
 class ListeningModeProps(BaseModel):
     """
     ListeningModeProps
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_ref.py` & `mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_ref.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, conint
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conint
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conint
 
 
 class ListeningModeRef(BaseModel):
     """
     Reference to a listening mode  # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/listening_mode_trigger.py` & `mozart_api-3.4.1.8.5/mozart_api/models/listening_mode_trigger.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,28 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, ValidationError, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
+
 from mozart_api.models.power_link_trigger import PowerLinkTrigger
 from typing import Union, Any, List, TYPE_CHECKING
-from pydantic import StrictStr, Field
+
+try:
+    from pydantic.v1 import StrictStr, Field
+except ImportError:
+    from pydantic import StrictStr, Field
+
 
 LISTENINGMODETRIGGER_ONE_OF_SCHEMAS = ["PowerLinkTrigger"]
 
 
 class ListeningModeTrigger(BaseModel):
     """
     ListeningModeTrigger
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/loudness.py` & `mozart_api-3.4.1.8.5/mozart_api/models/loudness.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictBool
+
+try:
+    from pydantic.v1 import BaseModel, StrictBool
+except ImportError:
+    from pydantic import BaseModel, StrictBool
 
 
 class Loudness(BaseModel):
     """
     Loudness
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/microphone_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/microphone_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class MicrophoneState(BaseModel):
     """
     MicrophoneState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/microphones_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/microphones_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.microphone_state import MicrophoneState
 
 
 class MicrophonesState(BaseModel):
     """
     state of microphones, both physical switches and software state  # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request.py` & `mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, conint
+
+try:
+    from pydantic.v1 import BaseModel, Field, conint
+except ImportError:
+    from pydantic import BaseModel, Field, conint
+
 from mozart_api.models.overlay_play_request_from_usb_from_usb import (
     OverlayPlayRequestFromUsbFromUsb,
 )
 from mozart_api.models.overlay_play_request_text_to_speech_text_to_speech import (
     OverlayPlayRequestTextToSpeechTextToSpeech,
 )
 from mozart_api.models.uri import Uri
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_common.py` & `mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_common.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, conint
+
+try:
+    from pydantic.v1 import BaseModel, Field, conint
+except ImportError:
+    from pydantic import BaseModel, Field, conint
 
 
 class OverlayPlayRequestCommon(BaseModel):
     """
     OverlayPlayRequestCommon
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_from_usb.py` & `mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_from_usb.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.overlay_play_request_from_usb_from_usb import (
     OverlayPlayRequestFromUsbFromUsb,
 )
 
 
 class OverlayPlayRequestFromUsb(BaseModel):
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_from_usb_from_usb.py` & `mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_from_usb_from_usb.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, constr
+try:
+    from pydantic.v1 import BaseModel, Field, constr
+except ImportError:
+    from pydantic import BaseModel, Field, constr
 
 
 class OverlayPlayRequestFromUsbFromUsb(BaseModel):
     """
     OverlayPlayRequestFromUsbFromUsb
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_text_to_speech.py` & `mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_text_to_speech.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.overlay_play_request_text_to_speech_text_to_speech import (
     OverlayPlayRequestTextToSpeechTextToSpeech,
 )
 
 
 class OverlayPlayRequestTextToSpeech(BaseModel):
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py` & `mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, constr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, constr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, constr
 
 
 class OverlayPlayRequestTextToSpeechTextToSpeech(BaseModel):
     """
     Object used for performing a text-to-speech operation on the product.   # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/overlay_play_request_uri.py` & `mozart_api-3.4.1.8.5/mozart_api/models/overlay_play_request_uri.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel
+
+try:
+    from pydantic.v1 import BaseModel
+except ImportError:
+    from pydantic import BaseModel
+
 from mozart_api.models.uri import Uri
 
 
 class OverlayPlayRequestUri(BaseModel):
     """
     OverlayPlayRequestUri
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/paired_remote.py` & `mozart_api-3.4.1.8.5/mozart_api/models/paired_remote.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conint, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conint, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conint, conlist, validator
 
 
 class PairedRemote(BaseModel):
     """
     PairedRemote
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/paired_remote_response.py` & `mozart_api-3.4.1.8.5/mozart_api/models/paired_remote_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, conlist
+
+try:
+    from pydantic.v1 import BaseModel, conlist
+except ImportError:
+    from pydantic import BaseModel, conlist
+
 from mozart_api.models.paired_remote import PairedRemote
 
 
 class PairedRemoteResponse(BaseModel):
     """
     PairedRemoteResponse
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/play_queue_item.py` & `mozart_api-3.4.1.8.5/mozart_api/models/play_queue_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+
 from mozart_api.models.play_queue_item_type import PlayQueueItemType
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
 
 
 class PlayQueueItem(BaseModel):
     """
     PlayQueueItem
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/play_queue_item_type.py` & `mozart_api-3.4.1.8.5/mozart_api/models/play_queue_item_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr, validator
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class PlayQueueItemType(BaseModel):
     """
     PlayQueueItemType
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/play_queue_settings.py` & `mozart_api-3.4.1.8.5/mozart_api/models/play_queue_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictBool, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictBool, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictBool, StrictStr, validator
 
 
 class PlayQueueSettings(BaseModel):
     """
     PlayQueueSettings
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/playback_content_metadata.py` & `mozart_api-3.4.1.8.5/mozart_api/models/playback_content_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, validator
+
 from mozart_api.models.art import Art
 from mozart_api.models.beolink_leader import BeolinkLeader
 
 
 class PlaybackContentMetadata(BaseModel):
     """
     PlaybackContentMetadata
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/playback_error.py` & `mozart_api-3.4.1.8.5/mozart_api/models/playback_error.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr
+except ImportError:
+    from pydantic import BaseModel, StrictStr
+
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
 
 
 class PlaybackError(BaseModel):
     """
     PlaybackError
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/playback_progress.py` & `mozart_api-3.4.1.8.5/mozart_api/models/playback_progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 
 class PlaybackProgress(BaseModel):
     """
     PlaybackProgress
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/playback_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/playback_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel
+
+try:
+    from pydantic.v1 import BaseModel
+except ImportError:
+    from pydantic import BaseModel
+
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
 from mozart_api.models.playback_progress import PlaybackProgress
 from mozart_api.models.rendering_state import RenderingState
 from mozart_api.models.source import Source
 
 
 class PlaybackState(BaseModel):
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/power_link_trigger.py` & `mozart_api-3.4.1.8.5/mozart_api/models/power_link_trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt
 
 
 class PowerLinkTrigger(BaseModel):
     """
     PowerLinkTrigger
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/power_state_enum.py` & `mozart_api-3.4.1.8.5/mozart_api/models/power_state_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class PowerStateEnum(BaseModel):
     """
     PowerStateEnum
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/preset.py` & `mozart_api-3.4.1.8.5/mozart_api/models/preset.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist
+
 from mozart_api.models.action import Action
 from mozart_api.models.content_item import ContentItem
 from mozart_api.models.source_type_enum import SourceTypeEnum
 
 
 class Preset(BaseModel):
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/product_curtain_status.py` & `mozart_api-3.4.1.8.5/mozart_api/models/product_curtain_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictBool, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictBool, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictBool, StrictStr, validator
 
 
 class ProductCurtainStatus(BaseModel):
     """
     ProductCurtainStatus
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/product_friendly_name.py` & `mozart_api-3.4.1.8.5/mozart_api/models/product_friendly_name.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class ProductFriendlyName(BaseModel):
     """
     ProductFriendlyName
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/product_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/product_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.microphones_state import MicrophonesState
 from mozart_api.models.playback_state import PlaybackState
 from mozart_api.models.power_state_enum import PowerStateEnum
 from mozart_api.models.software_update_state import SoftwareUpdateState
 from mozart_api.models.sound_settings import SoundSettings
 from mozart_api.models.source import Source
 from mozart_api.models.tv_state import TvState
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/remote_menu_item.py` & `mozart_api-3.4.1.8.5/mozart_api/models/remote_menu_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, validator
+
 from mozart_api.models.action import Action
 from mozart_api.models.content_item import ContentItem
 
 
 class RemoteMenuItem(BaseModel):
     """
     RemoteMenuItem
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/remote_menu_item_properties.py` & `mozart_api-3.4.1.8.5/mozart_api/models/remote_menu_item_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, validator
+
 from mozart_api.models.action import Action
 
 
 class RemoteMenuItemProperties(BaseModel):
     """
     RemoteMenuItemProperties
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/remote_ui_key_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/remote_ui_key_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class RemoteUIKeyState(BaseModel):
     """
     RemoteUIKeyState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/rendering_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/rendering_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class RenderingState(BaseModel):
     """
     RenderingState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist
 
 
 class RoomCompensation(BaseModel):
     """
     RoomCompensation
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_current_measurement.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_current_measurement.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class RoomCompensationCurrentMeasurement(BaseModel):
     """
     State and speaker ID of the currently running measurement. Is only relevant for advanced room compensation.   # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_debug.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_debug.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictBool
+
+try:
+    from pydantic.v1 import BaseModel, StrictBool
+except ImportError:
+    from pydantic import BaseModel, StrictBool
 
 
 class RoomCompensationDebug(BaseModel):
     """
     RoomCompensationDebug
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_enabled.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_enabled.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictBool
+
+try:
+    from pydantic.v1 import BaseModel, StrictBool
+except ImportError:
+    from pydantic import BaseModel, StrictBool
 
 
 class RoomCompensationEnabled(BaseModel):
     """
     RoomCompensationEnabled
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_error_details.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_error_details.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.room_compensation_measurement_error import (
     RoomCompensationMeasurementError,
 )
 
 
 class RoomCompensationErrorDetails(BaseModel):
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_feature.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conint, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conint, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conint, conlist
 
 
 class RoomCompensationFeature(BaseModel):
     """
     RoomCompensationFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_info.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.room_compensation_debug import RoomCompensationDebug
 from mozart_api.models.room_compensation_enabled import RoomCompensationEnabled
 from mozart_api.models.room_compensation_result import RoomCompensationResult
 from mozart_api.models.room_compensation_state import RoomCompensationState
 from mozart_api.models.room_compensation_type import RoomCompensationType
 from mozart_api.models.room_compensation_version import RoomCompensationVersion
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_measurement_error.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_measurement_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class RoomCompensationMeasurementError(BaseModel):
     """
     RoomCompensationMeasurementError
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_properties.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,36 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conint, conlist, validator
+
+try:
+    from pydantic.v1 import (
+        BaseModel,
+        Field,
+        StrictBool,
+        StrictStr,
+        conint,
+        conlist,
+        validator,
+    )
+except ImportError:
+    from pydantic import (
+        BaseModel,
+        Field,
+        StrictBool,
+        StrictStr,
+        conint,
+        conlist,
+        validator,
+    )
+
 from mozart_api.models.latency_profile import LatencyProfile
 
 
 class RoomCompensationProperties(BaseModel):
     """
     RoomCompensationProperties
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_range.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conint, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conint, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conint, conlist
 
 
 class RoomCompensationRange(BaseModel):
     """
     RoomCompensationRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_response.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, StrictFloat, StrictInt
 
 
 class RoomCompensationResponse(BaseModel):
     """
     RoomCompensationResponse
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_result.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.room_compensation_response import RoomCompensationResponse
 from mozart_api.models.speaker_group import SpeakerGroup
 
 
 class RoomCompensationResult(BaseModel):
     """
     RoomCompensationResult
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
+
 from mozart_api.models.room_compensation_error_details import (
     RoomCompensationErrorDetails,
 )
 from mozart_api.models.room_compensation_properties import RoomCompensationProperties
 
 
 class RoomCompensationState(BaseModel):
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_state_value.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_state_value.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class RoomCompensationStateValue(BaseModel):
     """
     RoomCompensationStateValue
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_type.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class RoomCompensationType(BaseModel):
     """
     RoomCompensationType
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/room_compensation_version.py` & `mozart_api-3.4.1.8.5/mozart_api/models/room_compensation_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, conint
+
+try:
+    from pydantic.v1 import BaseModel, conint
+except ImportError:
+    from pydantic import BaseModel, conint
 
 
 class RoomCompensationVersion(BaseModel):
     """
     RoomCompensationVersion
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/scene.py` & `mozart_api-3.4.1.8.5/mozart_api/models/scene.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+
 from mozart_api.models.action import Action
 
 
 class Scene(BaseModel):
     """
     Scene
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/scene_classification.py` & `mozart_api-3.4.1.8.5/mozart_api/models/scene_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class SceneClassification(BaseModel):
     """
     SceneClassification
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/scene_match.py` & `mozart_api-3.4.1.8.5/mozart_api/models/scene_match.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist
 
 
 class SceneMatch(BaseModel):
     """
     SceneMatch
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/scene_properties.py` & `mozart_api-3.4.1.8.5/mozart_api/models/scene_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, constr
+
 from mozart_api.models.action import Action
 
 
 class SceneProperties(BaseModel):
     """
     SceneProperties
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/scene_trigger_base_properties.py` & `mozart_api-3.4.1.8.5/mozart_api/models/scene_trigger_base_properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist
+
 from mozart_api.models.action import Action
 
 
 class SceneTriggerBaseProperties(BaseModel):
     """
     Base properties for a scene trigger  # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/software_update_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/software_update_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
 
 
 class SoftwareUpdateState(BaseModel):
     """
     SoftwareUpdateState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/software_update_status.py` & `mozart_api-3.4.1.8.5/mozart_api/models/software_update_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+
 from mozart_api.models.software_update_state import SoftwareUpdateState
 
 
 class SoftwareUpdateStatus(BaseModel):
     """
     SoftwareUpdateStatus
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/sound_adjustments.py` & `mozart_api-3.4.1.8.5/mozart_api/models/sound_adjustments.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr
+
+try:
+    from pydantic.v1 import (
+        BaseModel,
+        Field,
+        StrictBool,
+        StrictFloat,
+        StrictInt,
+        StrictStr,
+    )
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 
 
 class SoundAdjustments(BaseModel):
     """
     SoundAdjustments
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/sound_feature_set.py` & `mozart_api-3.4.1.8.5/mozart_api/models/sound_feature_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.ambience_feature import AmbienceFeature
 from mozart_api.models.balance_feature import BalanceFeature
 from mozart_api.models.bass_feature import BassFeature
 from mozart_api.models.bass_management_feature import BassManagementFeature
 from mozart_api.models.compression_feature import CompressionFeature
 from mozart_api.models.directivity_feature import DirectivityFeature
 from mozart_api.models.fader_feature import FaderFeature
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/sound_settings.py` & `mozart_api-3.4.1.8.5/mozart_api/models/sound_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.room_compensation_info import RoomCompensationInfo
 from mozart_api.models.sound_adjustments import SoundAdjustments
 from mozart_api.models.sound_tone_touch import SoundToneTouch
 
 
 class SoundSettings(BaseModel):
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/sound_tone_touch.py` & `mozart_api-3.4.1.8.5/mozart_api/models/sound_tone_touch.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, StrictFloat, StrictInt
 
 
 class SoundToneTouch(BaseModel):
     """
     SoundToneTouch
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/source.py` & `mozart_api-3.4.1.8.5/mozart_api/models/source.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr
+
 from mozart_api.models.source_type_enum import SourceTypeEnum
 
 
 class Source(BaseModel):
     """
     Source
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/source_array.py` & `mozart_api-3.4.1.8.5/mozart_api/models/source_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, conlist
+
+try:
+    from pydantic.v1 import BaseModel, conlist
+except ImportError:
+    from pydantic import BaseModel, conlist
+
 from mozart_api.models.source import Source
 
 
 class SourceArray(BaseModel):
     """
     SourceArray
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/source_type_enum.py` & `mozart_api-3.4.1.8.5/mozart_api/models/source_type_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
 
 class SourceTypeEnum(BaseModel):
     """
     SourceTypeEnum
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_envelopment.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_envelopment.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
 
 class SpatialEnvelopment(BaseModel):
     """
     SpatialEnvelopment
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_envelopment_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_envelopment_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.spatial_envelopment import SpatialEnvelopment
 
 
 class SpatialEnvelopmentFeature(BaseModel):
     """
     SpatialEnvelopmentFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_envelopment_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_envelopment_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.spatial_envelopment import SpatialEnvelopment
 
 
 class SpatialEnvelopmentRange(BaseModel):
     """
     SpatialEnvelopmentRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_height.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_width.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
-class SpatialHeight(BaseModel):
+
+class SpatialWidth(BaseModel):
     """
-    SpatialHeight
+    SpatialWidth
     """
 
     value: Union[StrictFloat, StrictInt] = Field(
-        ..., description="Selected spatial-height value"
+        ..., description="Selected spatial-width value"
     )
     __properties = ["value"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -44,27 +48,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SpatialHeight:
-        """Create an instance of SpatialHeight from a JSON string"""
+    def from_json(cls, json_str: str) -> SpatialWidth:
+        """Create an instance of SpatialWidth from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SpatialHeight:
-        """Create an instance of SpatialHeight from a dict"""
+    def from_dict(cls, obj: dict) -> SpatialWidth:
+        """Create an instance of SpatialWidth from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SpatialHeight.parse_obj(obj)
+            return SpatialWidth.parse_obj(obj)
 
-        _obj = SpatialHeight.parse_obj({"value": obj.get("value")})
+        _obj = SpatialWidth.parse_obj({"value": obj.get("value")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_height_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_height_feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.spatial_height import SpatialHeight
 
 
 class SpatialHeightFeature(BaseModel):
     """
     SpatialHeightFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_height_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_height_range.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.spatial_height import SpatialHeight
 
 
 class SpatialHeightRange(BaseModel):
     """
     SpatialHeightRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_processing.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr, validator
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, validator
 
 
 class SpatialProcessing(BaseModel):
     """
     SpatialProcessing
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_processing_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_processing_feature.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.spatial_processing import SpatialProcessing
 
 
 class SpatialProcessingFeature(BaseModel):
     """
     SpatialProcessingFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_processing_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_processing_range.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.spatial_processing import SpatialProcessing
 
 
 class SpatialProcessingRange(BaseModel):
     """
     SpatialProcessingRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_surround.py` & `mozart_api-3.4.1.8.5/mozart_api/models/user_flow.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
+from typing import Optional
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class SpatialSurround(BaseModel):
+
+class UserFlow(BaseModel):
     """
-    SpatialSurround
+    UserFlow
     """
 
-    value: Union[StrictFloat, StrictInt] = Field(
-        ..., description="Selected spatial-surround value"
-    )
-    __properties = ["value"]
+    user_id: Optional[StrictStr] = Field(None, alias="userId")
+    __properties = ["userId"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -44,27 +46,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SpatialSurround:
-        """Create an instance of SpatialSurround from a JSON string"""
+    def from_json(cls, json_str: str) -> UserFlow:
+        """Create an instance of UserFlow from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SpatialSurround:
-        """Create an instance of SpatialSurround from a dict"""
+    def from_dict(cls, obj: dict) -> UserFlow:
+        """Create an instance of UserFlow from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SpatialSurround.parse_obj(obj)
+            return UserFlow.parse_obj(obj)
 
-        _obj = SpatialSurround.parse_obj({"value": obj.get("value")})
+        _obj = UserFlow.parse_obj({"user_id": obj.get("userId")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_surround_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_surround_feature.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.spatial_surround import SpatialSurround
 
 
 class SpatialSurroundFeature(BaseModel):
     """
     SpatialSurroundFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_surround_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_surround_range.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.spatial_surround import SpatialSurround
 
 
 class SpatialSurroundRange(BaseModel):
     """
     SpatialSurroundRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_width.py` & `mozart_api-3.4.1.8.5/mozart_api/models/stand_connected.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
+from typing import Optional
 
+try:
+    from pydantic.v1 import BaseModel, StrictBool
+except ImportError:
+    from pydantic import BaseModel, StrictBool
 
-class SpatialWidth(BaseModel):
+
+class StandConnected(BaseModel):
     """
-    SpatialWidth
+    StandConnected
     """
 
-    value: Union[StrictFloat, StrictInt] = Field(
-        ..., description="Selected spatial-width value"
-    )
-    __properties = ["value"]
+    connected: Optional[StrictBool] = None
+    __properties = ["connected"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -44,27 +46,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SpatialWidth:
-        """Create an instance of SpatialWidth from a JSON string"""
+    def from_json(cls, json_str: str) -> StandConnected:
+        """Create an instance of StandConnected from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SpatialWidth:
-        """Create an instance of SpatialWidth from a dict"""
+    def from_dict(cls, obj: dict) -> StandConnected:
+        """Create an instance of StandConnected from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SpatialWidth.parse_obj(obj)
+            return StandConnected.parse_obj(obj)
 
-        _obj = SpatialWidth.parse_obj({"value": obj.get("value")})
+        _obj = StandConnected.parse_obj({"connected": obj.get("connected")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_width_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_width_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.spatial_width import SpatialWidth
 
 
 class SpatialWidthFeature(BaseModel):
     """
     SpatialWidthFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/spatial_width_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_width_range.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.spatial_width import SpatialWidth
 
 
 class SpatialWidthRange(BaseModel):
     """
     SpatialWidthRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speaker_group.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speaker_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conint, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conint, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr, conint, conlist
+
 from mozart_api.models.latency_profile import LatencyProfile
 from mozart_api.models.speaker_group_member import SpeakerGroupMember
 
 
 class SpeakerGroup(BaseModel):
     """
     SpeakerGroup
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speaker_group_member.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speaker_group_member.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
-from pydantic import BaseModel, Field, StrictStr, confloat, conint
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, confloat, conint
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, confloat, conint
+
 from mozart_api.models.speaker_group_member_location import SpeakerGroupMemberLocation
 
 
 class SpeakerGroupMember(BaseModel):
     """
     SpeakerGroupMember
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speaker_group_member_location.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speaker_group_member_location.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictInt
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt
 
 
 class SpeakerGroupMemberLocation(BaseModel):
     """
     Coordinates of the speaker position in cm. Location is only relevant when the group is based on the automatic role assignment of advanced room compensation. The location is relative to the external microphone used during advanced room compensation measurements:   x=0, y=0, z=0: The location of the external microphone used during measurement.   x<0: To the left of the external microphone.   x>0: To the right of the external microphone.   y<0: Behind the external microphone.   y>0: In front of the external microphone.   z<0: Above the external microphone (may not be reliable).   z>0: Below the external microphone (may not be reliable).   # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speaker_group_overview.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speaker_group_overview.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr
 
 
 class SpeakerGroupOverview(BaseModel):
     """
     SpeakerGroupOverview
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speaker_link_member_status.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speaker_link_member_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, constr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, constr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, constr, validator
 
 
 class SpeakerLinkMemberStatus(BaseModel):
     """
     SpeakerLinkMemberStatus
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speaker_link_status.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speaker_link_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, conlist, validator
+
 from mozart_api.models.speaker_link_member_status import SpeakerLinkMemberStatus
 
 
 class SpeakerLinkStatus(BaseModel):
     """
     SpeakerLinkStatus
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speaker_role_enum.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speaker_role_enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class SpeakerRoleEnum(BaseModel):
     """
     SpeakerRoleEnum
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speech_enhance.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,25 +16,27 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
-class SpeechEnhance(BaseModel):
+
+class ToneTouchType(BaseModel):
     """
-    SpeechEnhance
+    ToneTouchType
     """
 
-    value: Union[StrictFloat, StrictInt] = Field(
-        ..., description="Selected speech-enhance value"
-    )
+    value: Union[StrictFloat, StrictInt] = Field(...)
     __properties = ["value"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -44,27 +46,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SpeechEnhance:
-        """Create an instance of SpeechEnhance from a JSON string"""
+    def from_json(cls, json_str: str) -> ToneTouchType:
+        """Create an instance of ToneTouchType from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SpeechEnhance:
-        """Create an instance of SpeechEnhance from a dict"""
+    def from_dict(cls, obj: dict) -> ToneTouchType:
+        """Create an instance of ToneTouchType from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SpeechEnhance.parse_obj(obj)
+            return ToneTouchType.parse_obj(obj)
 
-        _obj = SpeechEnhance.parse_obj({"value": obj.get("value")})
+        _obj = ToneTouchType.parse_obj({"value": obj.get("value")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speech_enhance_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speech_enhance_feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.speech_enhance import SpeechEnhance
 
 
 class SpeechEnhanceFeature(BaseModel):
     """
     SpeechEnhanceFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/speech_enhance_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/speech_enhance_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.speech_enhance import SpeechEnhance
 
 
 class SpeechEnhanceRange(BaseModel):
     """
     SpeechEnhanceRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/stand_connected.py` & `mozart_api-3.4.1.8.5/mozart_api/models/stand_position.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,25 +15,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictBool
+from typing import Optional, Union
 
+try:
+    from pydantic.v1 import BaseModel, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, StrictFloat, StrictInt
 
-class StandConnected(BaseModel):
+
+class StandPosition(BaseModel):
     """
-    StandConnected
+    StandPosition
     """
 
-    connected: Optional[StrictBool] = None
-    __properties = ["connected"]
+    angle: Optional[Union[StrictFloat, StrictInt]] = None
+    __properties = ["angle"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -42,27 +46,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StandConnected:
-        """Create an instance of StandConnected from a JSON string"""
+    def from_json(cls, json_str: str) -> StandPosition:
+        """Create an instance of StandPosition from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StandConnected:
-        """Create an instance of StandConnected from a dict"""
+    def from_dict(cls, obj: dict) -> StandPosition:
+        """Create an instance of StandPosition from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return StandConnected.parse_obj(obj)
+            return StandPosition.parse_obj(obj)
 
-        _obj = StandConnected.parse_obj({"connected": obj.get("connected")})
+        _obj = StandPosition.parse_obj({"angle": obj.get("angle")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/stand_movement.py` & `mozart_api-3.4.1.8.5/mozart_api/models/stand_movement.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,35 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
-from pydantic import (
-    BaseModel,
-    Field,
-    StrictBool,
-    StrictFloat,
-    StrictInt,
-    StrictStr,
-    validator,
-)
+
+try:
+    from pydantic.v1 import (
+        BaseModel,
+        Field,
+        StrictBool,
+        StrictFloat,
+        StrictInt,
+        StrictStr,
+        validator,
+    )
+except ImportError:
+    from pydantic import (
+        BaseModel,
+        Field,
+        StrictBool,
+        StrictFloat,
+        StrictInt,
+        StrictStr,
+        validator,
+    )
 
 
 class StandMovement(BaseModel):
     """
     StandMovement
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/stand_position.py` & `mozart_api-3.4.1.8.5/mozart_api/models/treble.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt
 
 
-class StandPosition(BaseModel):
+class Treble(BaseModel):
     """
-    StandPosition
+    Treble
     """
 
-    angle: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties = ["angle"]
+    value: StrictInt = Field(..., description="Selected treble value")
+    __properties = ["value"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -42,27 +44,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StandPosition:
-        """Create an instance of StandPosition from a JSON string"""
+    def from_json(cls, json_str: str) -> Treble:
+        """Create an instance of Treble from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StandPosition:
-        """Create an instance of StandPosition from a dict"""
+    def from_dict(cls, obj: dict) -> Treble:
+        """Create an instance of Treble from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return StandPosition.parse_obj(obj)
+            return Treble.parse_obj(obj)
 
-        _obj = StandPosition.parse_obj({"angle": obj.get("angle")})
+        _obj = Treble.parse_obj({"value": obj.get("value")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tone_touch.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tone_touch.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel
+
+try:
+    from pydantic.v1 import BaseModel
+except ImportError:
+    from pydantic import BaseModel
+
 from mozart_api.models.tone_touch_type import ToneTouchType
 
 
 class ToneTouch(BaseModel):
     """
     ToneTouch
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_type.py` & `mozart_api-3.4.1.8.5/mozart_api/models/uri.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,25 +15,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt
+from typing import Optional
 
+try:
+    from pydantic.v1 import BaseModel, StrictStr
+except ImportError:
+    from pydantic import BaseModel, StrictStr
 
-class ToneTouchType(BaseModel):
+
+class Uri(BaseModel):
     """
-    ToneTouchType
+    Uri
     """
 
-    value: Union[StrictFloat, StrictInt] = Field(...)
-    __properties = ["value"]
+    location: Optional[StrictStr] = None
+    __properties = ["location"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -42,27 +46,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToneTouchType:
-        """Create an instance of ToneTouchType from a JSON string"""
+    def from_json(cls, json_str: str) -> Uri:
+        """Create an instance of Uri from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToneTouchType:
-        """Create an instance of ToneTouchType from a dict"""
+    def from_dict(cls, obj: dict) -> Uri:
+        """Create an instance of Uri from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToneTouchType.parse_obj(obj)
+            return Uri.parse_obj(obj)
 
-        _obj = ToneTouchType.parse_obj({"value": obj.get("value")})
+        _obj = Uri.parse_obj({"location": obj.get("location")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_type_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_type_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
+
 from mozart_api.models.tone_touch_type import ToneTouchType
 
 
 class ToneTouchTypeRange(BaseModel):
     """
     ToneTouchTypeRange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_x_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_y_feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
+
 from mozart_api.models.tone_touch_type import ToneTouchType
 
 
-class ToneTouchXFeature(BaseModel):
+class ToneTouchYFeature(BaseModel):
     """
-    ToneTouchXFeature
+    ToneTouchYFeature
     """
 
     value: Union[StrictFloat, StrictInt] = Field(...)
     default: ToneTouchType = Field(...)
     range: conlist(ToneTouchType, unique_items=True) = Field(
         ..., description="Product and role specific tone touch X or Y range"
     )
@@ -47,16 +52,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToneTouchXFeature:
-        """Create an instance of ToneTouchXFeature from a JSON string"""
+    def from_json(cls, json_str: str) -> ToneTouchYFeature:
+        """Create an instance of ToneTouchYFeature from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of default
         if self.default:
@@ -67,23 +72,23 @@
             for _item in self.range:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["range"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToneTouchXFeature:
-        """Create an instance of ToneTouchXFeature from a dict"""
+    def from_dict(cls, obj: dict) -> ToneTouchYFeature:
+        """Create an instance of ToneTouchYFeature from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToneTouchXFeature.parse_obj(obj)
+            return ToneTouchYFeature.parse_obj(obj)
 
-        _obj = ToneTouchXFeature.parse_obj(
+        _obj = ToneTouchYFeature.parse_obj(
             {
                 "value": obj.get("value"),
                 "default": (
                     ToneTouchType.from_dict(obj.get("default"))
                     if obj.get("default") is not None
                     else None
                 ),
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tone_touch_y_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/volume_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,30 +15,32 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
-from mozart_api.models.tone_touch_type import ToneTouchType
+from typing import Optional
 
+try:
+    from pydantic.v1 import BaseModel
+except ImportError:
+    from pydantic import BaseModel
 
-class ToneTouchYFeature(BaseModel):
+from mozart_api.models.volume_level import VolumeLevel
+
+
+class VolumeSettings(BaseModel):
     """
-    ToneTouchYFeature
+    VolumeSettings
     """
 
-    value: Union[StrictFloat, StrictInt] = Field(...)
-    default: ToneTouchType = Field(...)
-    range: conlist(ToneTouchType, unique_items=True) = Field(
-        ..., description="Product and role specific tone touch X or Y range"
-    )
-    __properties = ["value", "default", "range"]
+    default: Optional[VolumeLevel] = None
+    maximum: Optional[VolumeLevel] = None
+    __properties = ["default", "maximum"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -47,51 +49,46 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToneTouchYFeature:
-        """Create an instance of ToneTouchYFeature from a JSON string"""
+    def from_json(cls, json_str: str) -> VolumeSettings:
+        """Create an instance of VolumeSettings from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of default
         if self.default:
             _dict["default"] = self.default.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in range (list)
-        _items = []
-        if self.range:
-            for _item in self.range:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["range"] = _items
+        # override the default output from pydantic by calling `to_dict()` of maximum
+        if self.maximum:
+            _dict["maximum"] = self.maximum.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToneTouchYFeature:
-        """Create an instance of ToneTouchYFeature from a dict"""
+    def from_dict(cls, obj: dict) -> VolumeSettings:
+        """Create an instance of VolumeSettings from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToneTouchYFeature.parse_obj(obj)
+            return VolumeSettings.parse_obj(obj)
 
-        _obj = ToneTouchYFeature.parse_obj(
+        _obj = VolumeSettings.parse_obj(
             {
-                "value": obj.get("value"),
                 "default": (
-                    ToneTouchType.from_dict(obj.get("default"))
+                    VolumeLevel.from_dict(obj.get("default"))
                     if obj.get("default") is not None
                     else None
                 ),
-                "range": (
-                    [ToneTouchType.from_dict(_item) for _item in obj.get("range")]
-                    if obj.get("range") is not None
+                "maximum": (
+                    VolumeLevel.from_dict(obj.get("maximum"))
+                    if obj.get("maximum") is not None
                     else None
                 ),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/treble.py` & `mozart_api-3.4.1.8.5/mozart_api/models/treble_range.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,24 +15,34 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictInt
+from typing import List
 
+try:
+    from pydantic.v1 import BaseModel, Field, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, conlist
 
-class Treble(BaseModel):
+from mozart_api.models.treble import Treble
+
+
+class TrebleRange(BaseModel):
     """
-    Treble
+    TrebleRange
     """
 
-    value: StrictInt = Field(..., description="Selected treble value")
-    __properties = ["value"]
+    default: Treble = Field(...)
+    range: conlist(Treble, unique_items=True) = Field(
+        ..., description="Product and role specific treble range"
+    )
+    __properties = ["default", "range"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -41,27 +51,50 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Treble:
-        """Create an instance of Treble from a JSON string"""
+    def from_json(cls, json_str: str) -> TrebleRange:
+        """Create an instance of TrebleRange from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of default
+        if self.default:
+            _dict["default"] = self.default.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in range (list)
+        _items = []
+        if self.range:
+            for _item in self.range:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["range"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Treble:
-        """Create an instance of Treble from a dict"""
+    def from_dict(cls, obj: dict) -> TrebleRange:
+        """Create an instance of TrebleRange from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Treble.parse_obj(obj)
+            return TrebleRange.parse_obj(obj)
 
-        _obj = Treble.parse_obj({"value": obj.get("value")})
+        _obj = TrebleRange.parse_obj(
+            {
+                "default": (
+                    Treble.from_dict(obj.get("default"))
+                    if obj.get("default") is not None
+                    else None
+                ),
+                "range": (
+                    [Treble.from_dict(_item) for _item in obj.get("range")]
+                    if obj.get("range") is not None
+                    else None
+                ),
+            }
+        )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/treble_feature.py` & `mozart_api-3.4.1.8.5/mozart_api/models/treble_feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictInt, conlist
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, conlist
+
 from mozart_api.models.treble import Treble
 
 
 class TrebleFeature(BaseModel):
     """
     TrebleFeature
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/treble_range.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_role.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List
-from pydantic import BaseModel, Field, conlist
-from mozart_api.models.treble import Treble
+from typing import Optional
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class TrebleRange(BaseModel):
+from mozart_api.models.speaker_role_enum import SpeakerRoleEnum
+
+
+class WebSocketEventRole(BaseModel):
     """
-    TrebleRange
+    WebSocketEventRole
     """
 
-    default: Treble = Field(...)
-    range: conlist(Treble, unique_items=True) = Field(
-        ..., description="Product and role specific treble range"
-    )
-    __properties = ["default", "range"]
+    event_data: Optional[SpeakerRoleEnum] = Field(None, alias="eventData")
+    event_type: Optional[StrictStr] = Field(None, alias="eventType")
+    __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -46,50 +49,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> TrebleRange:
-        """Create an instance of TrebleRange from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventRole:
+        """Create an instance of WebSocketEventRole from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of default
-        if self.default:
-            _dict["default"] = self.default.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in range (list)
-        _items = []
-        if self.range:
-            for _item in self.range:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["range"] = _items
+        # override the default output from pydantic by calling `to_dict()` of event_data
+        if self.event_data:
+            _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> TrebleRange:
-        """Create an instance of TrebleRange from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventRole:
+        """Create an instance of WebSocketEventRole from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return TrebleRange.parse_obj(obj)
+            return WebSocketEventRole.parse_obj(obj)
 
-        _obj = TrebleRange.parse_obj(
+        _obj = WebSocketEventRole.parse_obj(
             {
-                "default": (
-                    Treble.from_dict(obj.get("default"))
-                    if obj.get("default") is not None
-                    else None
-                ),
-                "range": (
-                    [Treble.from_dict(_item) for _item in obj.get("range")]
-                    if obj.get("range") is not None
+                "event_data": (
+                    SpeakerRoleEnum.from_dict(obj.get("eventData"))
+                    if obj.get("eventData") is not None
                     else None
                 ),
+                "event_type": obj.get("eventType"),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tv_info_event_data.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tv_info_event_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel
+
+try:
+    from pydantic.v1 import BaseModel
+except ImportError:
+    from pydantic import BaseModel
+
 from mozart_api.models.tv_integration_types import TvIntegrationTypes
 
 
 class TvInfoEventData(BaseModel):
     """
     TvInfoEventData
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tv_integration_types.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tv_integration_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class TvIntegrationTypes(BaseModel):
     """
     TvIntegrationTypes
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tv_properties.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tv_properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictInt, StrictStr
+
 from mozart_api.models.tv_integration_types import TvIntegrationTypes
 
 
 class TvProperties(BaseModel):
     """
     TvProperties
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tv_sound_settings.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tv_sound_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel
+
+try:
+    from pydantic.v1 import BaseModel
+except ImportError:
+    from pydantic import BaseModel
+
 from mozart_api.models.lge_tv_sound_settings import LgeTvSoundSettings
 
 
 class TvSoundSettings(BaseModel):
     """
     TvSoundSettings
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/tv_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tv_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field
+
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field
+
 from mozart_api.models.tv_integration_types import TvIntegrationTypes
 from mozart_api.models.tv_properties import TvProperties
 from mozart_api.models.tv_sound_settings import TvSoundSettings
 
 
 class TvState(BaseModel):
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/user_flow.py` & `mozart_api-3.4.1.8.5/mozart_api/models/volume_mute.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,24 +16,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
 
+try:
+    from pydantic.v1 import BaseModel, StrictBool
+except ImportError:
+    from pydantic import BaseModel, StrictBool
 
-class UserFlow(BaseModel):
+
+class VolumeMute(BaseModel):
     """
-    UserFlow
+    VolumeMute
     """
 
-    user_id: Optional[StrictStr] = Field(None, alias="userId")
-    __properties = ["userId"]
+    muted: Optional[StrictBool] = None
+    __properties = ["muted"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -42,27 +46,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserFlow:
-        """Create an instance of UserFlow from a JSON string"""
+    def from_json(cls, json_str: str) -> VolumeMute:
+        """Create an instance of VolumeMute from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserFlow:
-        """Create an instance of UserFlow from a dict"""
+    def from_dict(cls, obj: dict) -> VolumeMute:
+        """Create an instance of VolumeMute from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UserFlow.parse_obj(obj)
+            return VolumeMute.parse_obj(obj)
 
-        _obj = UserFlow.parse_obj({"user_id": obj.get("userId")})
+        _obj = VolumeMute.parse_obj({"muted": obj.get("muted")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/video_pixel_format.py` & `mozart_api-3.4.1.8.5/mozart_api/models/video_pixel_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
 
 
 class VideoPixelFormat(BaseModel):
     """
     VideoPixelFormat
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/video_timings.py` & `mozart_api-3.4.1.8.5/mozart_api/models/video_timings.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictBool, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt
 
 
 class VideoTimings(BaseModel):
     """
     VideoTimings
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/volume_level.py` & `mozart_api-3.4.1.8.5/mozart_api/models/volume_level.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictInt
+
+try:
+    from pydantic.v1 import BaseModel, StrictInt
+except ImportError:
+    from pydantic import BaseModel, StrictInt
 
 
 class VolumeLevel(BaseModel):
     """
     VolumeLevel
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/volume_mute.py` & `mozart_api-3.4.1.8.5/mozart_api/models/spatial_surround.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictBool
+from typing import Union
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
-class VolumeMute(BaseModel):
+
+class SpatialSurround(BaseModel):
     """
-    VolumeMute
+    SpatialSurround
     """
 
-    muted: Optional[StrictBool] = None
-    __properties = ["muted"]
+    value: Union[StrictFloat, StrictInt] = Field(
+        ..., description="Selected spatial-surround value"
+    )
+    __properties = ["value"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -42,27 +48,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VolumeMute:
-        """Create an instance of VolumeMute from a JSON string"""
+    def from_json(cls, json_str: str) -> SpatialSurround:
+        """Create an instance of SpatialSurround from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VolumeMute:
-        """Create an instance of VolumeMute from a dict"""
+    def from_dict(cls, obj: dict) -> SpatialSurround:
+        """Create an instance of SpatialSurround from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return VolumeMute.parse_obj(obj)
+            return SpatialSurround.parse_obj(obj)
 
-        _obj = VolumeMute.parse_obj({"muted": obj.get("muted")})
+        _obj = SpatialSurround.parse_obj({"value": obj.get("value")})
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/volume_settings.py` & `mozart_api-3.4.1.8.5/mozart_api/models/tone_touch_x_feature.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,27 +15,35 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel
-from mozart_api.models.volume_level import VolumeLevel
+from typing import List, Union
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist
+except ImportError:
+    from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
 
-class VolumeSettings(BaseModel):
+from mozart_api.models.tone_touch_type import ToneTouchType
+
+
+class ToneTouchXFeature(BaseModel):
     """
-    VolumeSettings
+    ToneTouchXFeature
     """
 
-    default: Optional[VolumeLevel] = None
-    maximum: Optional[VolumeLevel] = None
-    __properties = ["default", "maximum"]
+    value: Union[StrictFloat, StrictInt] = Field(...)
+    default: ToneTouchType = Field(...)
+    range: conlist(ToneTouchType, unique_items=True) = Field(
+        ..., description="Product and role specific tone touch X or Y range"
+    )
+    __properties = ["value", "default", "range"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -44,46 +52,51 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VolumeSettings:
-        """Create an instance of VolumeSettings from a JSON string"""
+    def from_json(cls, json_str: str) -> ToneTouchXFeature:
+        """Create an instance of ToneTouchXFeature from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of default
         if self.default:
             _dict["default"] = self.default.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of maximum
-        if self.maximum:
-            _dict["maximum"] = self.maximum.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in range (list)
+        _items = []
+        if self.range:
+            for _item in self.range:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["range"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VolumeSettings:
-        """Create an instance of VolumeSettings from a dict"""
+    def from_dict(cls, obj: dict) -> ToneTouchXFeature:
+        """Create an instance of ToneTouchXFeature from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return VolumeSettings.parse_obj(obj)
+            return ToneTouchXFeature.parse_obj(obj)
 
-        _obj = VolumeSettings.parse_obj(
+        _obj = ToneTouchXFeature.parse_obj(
             {
+                "value": obj.get("value"),
                 "default": (
-                    VolumeLevel.from_dict(obj.get("default"))
+                    ToneTouchType.from_dict(obj.get("default"))
                     if obj.get("default") is not None
                     else None
                 ),
-                "maximum": (
-                    VolumeLevel.from_dict(obj.get("maximum"))
-                    if obj.get("maximum") is not None
+                "range": (
+                    [ToneTouchType.from_dict(_item) for _item in obj.get("range")]
+                    if obj.get("range") is not None
                     else None
                 ),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/volume_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/volume_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel
+
+try:
+    from pydantic.v1 import BaseModel
+except ImportError:
+    from pydantic import BaseModel
+
 from mozart_api.models.volume_level import VolumeLevel
 from mozart_api.models.volume_mute import VolumeMute
 
 
 class VolumeState(BaseModel):
     """
     VolumeState
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_active_hdmi_input_signal.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_active_hdmi_input_signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.hdmi_input import HdmiInput
 
 
 class WebSocketEventActiveHdmiInputSignal(BaseModel):
     """
     WebSocketEventActiveHdmiInputSignal
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_active_listening_mode.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_active_listening_mode.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.listening_mode_props import ListeningModeProps
 
 
 class WebSocketEventActiveListeningMode(BaseModel):
     """
     WebSocketEventActiveListeningMode
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_active_speaker_group.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_speaker_group_changed.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,24 +16,27 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-from mozart_api.models.speaker_group_overview import SpeakerGroupOverview
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class WebSocketEventActiveSpeakerGroup(BaseModel):
+
+class WebSocketEventSpeakerGroupChanged(BaseModel):
     """
-    WebSocketEventActiveSpeakerGroup
+    WebSocketEventSpeakerGroupChanged
     """
 
-    event_data: Optional[SpeakerGroupOverview] = Field(None, alias="eventData")
+    event_data: Optional[StrictStr] = Field(None, alias="eventData")
     event_type: Optional[StrictStr] = Field(None, alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -44,39 +47,29 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventActiveSpeakerGroup:
-        """Create an instance of WebSocketEventActiveSpeakerGroup from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventSpeakerGroupChanged:
+        """Create an instance of WebSocketEventSpeakerGroupChanged from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of event_data
-        if self.event_data:
-            _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventActiveSpeakerGroup:
-        """Create an instance of WebSocketEventActiveSpeakerGroup from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventSpeakerGroupChanged:
+        """Create an instance of WebSocketEventSpeakerGroupChanged from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventActiveSpeakerGroup.parse_obj(obj)
+            return WebSocketEventSpeakerGroupChanged.parse_obj(obj)
 
-        _obj = WebSocketEventActiveSpeakerGroup.parse_obj(
-            {
-                "event_data": (
-                    SpeakerGroupOverview.from_dict(obj.get("eventData"))
-                    if obj.get("eventData") is not None
-                    else None
-                ),
-                "event_type": obj.get("eventType"),
-            }
+        _obj = WebSocketEventSpeakerGroupChanged.parse_obj(
+            {"event_data": obj.get("eventData"), "event_type": obj.get("eventType")}
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_alarm_timer.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_alarm_timer.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.alarm_timer_event_data import AlarmTimerEventData
 
 
 class WebSocketEventAlarmTimer(BaseModel):
     """
     WebSocketEventAlarmTimer
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_alarm_triggered.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_alarm_triggered.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.alarm_triggered_info import AlarmTriggeredInfo
 
 
 class WebSocketEventAlarmTriggered(BaseModel):
     """
     WebSocketEventAlarmTriggered
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_battery.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_battery.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.battery_state import BatteryState
 
 
 class WebSocketEventBattery(BaseModel):
     """
     WebSocketEventBattery
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_beo_remote_button.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_beo_remote_button.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.beo_remote_button import BeoRemoteButton
 
 
 class WebSocketEventBeoRemoteButton(BaseModel):
     """
     WebSocketEventBeoRemoteButton
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_beolink_experiences_result.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_beolink_experiences_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.beolink_experiences_result import BeolinkExperiencesResult
 
 
 class WebSocketEventBeolinkExperiencesResult(BaseModel):
     """
     WebSocketEventBeolinkExperiencesResult
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_beolink_join_result.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_beolink_join_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.beolink_join_result import BeolinkJoinResult
 
 
 class WebSocketEventBeolinkJoinResult(BaseModel):
     """
     WebSocketEventBeolinkJoinResult
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_button.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_button.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.button_event import ButtonEvent
 
 
 class WebSocketEventButton(BaseModel):
     """
     WebSocketEventButton
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_curtains.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_curtains.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.product_curtain_status import ProductCurtainStatus
 
 
 class WebSocketEventCurtains(BaseModel):
     """
     WebSocketEventCurtains
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_hdmi_video_format_signal.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_hdmi_video_format_signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.hdmi_video_format import HdmiVideoFormat
 
 
 class WebSocketEventHdmiVideoFormatSignal(BaseModel):
     """
     WebSocketEventHdmiVideoFormatSignal
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_notification.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.websocket_notification_tag import WebsocketNotificationTag
 
 
 class WebSocketEventNotification(BaseModel):
     """
     This telegram is used to send a tagged notification.  # noqa: E501
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_error.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.playback_error import PlaybackError
 
 
 class WebSocketEventPlaybackError(BaseModel):
     """
     WebSocketEventPlaybackError
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_metadata.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
 
 
 class WebSocketEventPlaybackMetadata(BaseModel):
     """
     WebSocketEventPlaybackMetadata
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_progress.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-from mozart_api.models.playback_progress import PlaybackProgress
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class WebSocketEventPlaybackProgress(BaseModel):
+from mozart_api.models.source import Source
+
+
+class WebSocketEventPlaybackSource(BaseModel):
     """
-    WebSocketEventPlaybackProgress
+    WebSocketEventPlaybackSource
     """
 
-    event_data: Optional[PlaybackProgress] = Field(None, alias="eventData")
+    event_data: Optional[Source] = Field(None, alias="eventData")
     event_type: Optional[StrictStr] = Field(None, alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -44,39 +49,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventPlaybackProgress:
-        """Create an instance of WebSocketEventPlaybackProgress from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventPlaybackSource:
+        """Create an instance of WebSocketEventPlaybackSource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of event_data
         if self.event_data:
             _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventPlaybackProgress:
-        """Create an instance of WebSocketEventPlaybackProgress from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventPlaybackSource:
+        """Create an instance of WebSocketEventPlaybackSource from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventPlaybackProgress.parse_obj(obj)
+            return WebSocketEventPlaybackSource.parse_obj(obj)
 
-        _obj = WebSocketEventPlaybackProgress.parse_obj(
+        _obj = WebSocketEventPlaybackSource.parse_obj(
             {
                 "event_data": (
-                    PlaybackProgress.from_dict(obj.get("eventData"))
+                    Source.from_dict(obj.get("eventData"))
                     if obj.get("eventData") is not None
                     else None
                 ),
                 "event_type": obj.get("eventType"),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_source.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-from mozart_api.models.source import Source
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class WebSocketEventPlaybackSource(BaseModel):
+from mozart_api.models.rendering_state import RenderingState
+
+
+class WebSocketEventPlaybackState(BaseModel):
     """
-    WebSocketEventPlaybackSource
+    WebSocketEventPlaybackState
     """
 
-    event_data: Optional[Source] = Field(None, alias="eventData")
+    event_data: Optional[RenderingState] = Field(None, alias="eventData")
     event_type: Optional[StrictStr] = Field(None, alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -44,39 +49,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventPlaybackSource:
-        """Create an instance of WebSocketEventPlaybackSource from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventPlaybackState:
+        """Create an instance of WebSocketEventPlaybackState from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of event_data
         if self.event_data:
             _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventPlaybackSource:
-        """Create an instance of WebSocketEventPlaybackSource from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventPlaybackState:
+        """Create an instance of WebSocketEventPlaybackState from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventPlaybackSource.parse_obj(obj)
+            return WebSocketEventPlaybackState.parse_obj(obj)
 
-        _obj = WebSocketEventPlaybackSource.parse_obj(
+        _obj = WebSocketEventPlaybackState.parse_obj(
             {
                 "event_data": (
-                    Source.from_dict(obj.get("eventData"))
+                    RenderingState.from_dict(obj.get("eventData"))
                     if obj.get("eventData") is not None
                     else None
                 ),
                 "event_type": obj.get("eventType"),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_playback_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_tv_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-from mozart_api.models.rendering_state import RenderingState
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class WebSocketEventPlaybackState(BaseModel):
+from mozart_api.models.tv_info_event_data import TvInfoEventData
+
+
+class WebSocketEventTvInfo(BaseModel):
     """
-    WebSocketEventPlaybackState
+    WebSocketEventTvInfo
     """
 
-    event_data: Optional[RenderingState] = Field(None, alias="eventData")
+    event_data: Optional[TvInfoEventData] = Field(None, alias="eventData")
     event_type: Optional[StrictStr] = Field(None, alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -44,39 +49,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventPlaybackState:
-        """Create an instance of WebSocketEventPlaybackState from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventTvInfo:
+        """Create an instance of WebSocketEventTvInfo from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of event_data
         if self.event_data:
             _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventPlaybackState:
-        """Create an instance of WebSocketEventPlaybackState from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventTvInfo:
+        """Create an instance of WebSocketEventTvInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventPlaybackState.parse_obj(obj)
+            return WebSocketEventTvInfo.parse_obj(obj)
 
-        _obj = WebSocketEventPlaybackState.parse_obj(
+        _obj = WebSocketEventTvInfo.parse_obj(
             {
                 "event_data": (
-                    RenderingState.from_dict(obj.get("eventData"))
+                    TvInfoEventData.from_dict(obj.get("eventData"))
                     if obj.get("eventData") is not None
                     else None
                 ),
                 "event_type": obj.get("eventType"),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_power_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_power_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.power_state_enum import PowerStateEnum
 
 
 class WebSocketEventPowerState(BaseModel):
     """
     WebSocketEventPowerState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_puc_install_remote_id_status.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_puc_install_remote_id_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.install_record_id_state import InstallRecordIdState
 
 
 class WebSocketEventPucInstallRemoteIdStatus(BaseModel):
     """
     WebSocketEventPucInstallRemoteIdStatus
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_role.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_playback_progress.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-from mozart_api.models.speaker_role_enum import SpeakerRoleEnum
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class WebSocketEventRole(BaseModel):
+from mozart_api.models.playback_progress import PlaybackProgress
+
+
+class WebSocketEventPlaybackProgress(BaseModel):
     """
-    WebSocketEventRole
+    WebSocketEventPlaybackProgress
     """
 
-    event_data: Optional[SpeakerRoleEnum] = Field(None, alias="eventData")
+    event_data: Optional[PlaybackProgress] = Field(None, alias="eventData")
     event_type: Optional[StrictStr] = Field(None, alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -44,39 +49,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventRole:
-        """Create an instance of WebSocketEventRole from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventPlaybackProgress:
+        """Create an instance of WebSocketEventPlaybackProgress from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of event_data
         if self.event_data:
             _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventRole:
-        """Create an instance of WebSocketEventRole from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventPlaybackProgress:
+        """Create an instance of WebSocketEventPlaybackProgress from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventRole.parse_obj(obj)
+            return WebSocketEventPlaybackProgress.parse_obj(obj)
 
-        _obj = WebSocketEventRole.parse_obj(
+        _obj = WebSocketEventPlaybackProgress.parse_obj(
             {
                 "event_data": (
-                    SpeakerRoleEnum.from_dict(obj.get("eventData"))
+                    PlaybackProgress.from_dict(obj.get("eventData"))
                     if obj.get("eventData") is not None
                     else None
                 ),
                 "event_type": obj.get("eventType"),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.room_compensation_current_measurement import (
     RoomCompensationCurrentMeasurement,
 )
 
 
 class WebSocketEventRoomCompensationCurrentMeasurementEvent(BaseModel):
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_room_compensation_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_room_compensation_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.room_compensation_state_value import RoomCompensationStateValue
 
 
 class WebSocketEventRoomCompensationState(BaseModel):
     """
     WebSocketEventRoomCompensationState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_software_update_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_software_update_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.software_update_state import SoftwareUpdateState
 
 
 class WebSocketEventSoftwareUpdateState(BaseModel):
     """
     WebSocketEventSoftwareUpdateState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_sound_settings.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_sound_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.sound_settings import SoundSettings
 
 
 class WebSocketEventSoundSettings(BaseModel):
     """
     WebSocketEventSoundSettings
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_source_change.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_source_change.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.source import Source
 
 
 class WebSocketEventSourceChange(BaseModel):
     """
     WebSocketEventSourceChange
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_speaker_group_changed.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_stand_connected.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class WebSocketEventSpeakerGroupChanged(BaseModel):
+from mozart_api.models.stand_connected import StandConnected
+
+
+class WebSocketEventStandConnected(BaseModel):
     """
-    WebSocketEventSpeakerGroupChanged
+    WebSocketEventStandConnected
     """
 
-    event_data: Optional[StrictStr] = Field(None, alias="eventData")
+    event_data: Optional[StandConnected] = Field(None, alias="eventData")
     event_type: Optional[StrictStr] = Field(None, alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -43,29 +49,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventSpeakerGroupChanged:
-        """Create an instance of WebSocketEventSpeakerGroupChanged from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventStandConnected:
+        """Create an instance of WebSocketEventStandConnected from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of event_data
+        if self.event_data:
+            _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventSpeakerGroupChanged:
-        """Create an instance of WebSocketEventSpeakerGroupChanged from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventStandConnected:
+        """Create an instance of WebSocketEventStandConnected from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventSpeakerGroupChanged.parse_obj(obj)
+            return WebSocketEventStandConnected.parse_obj(obj)
 
-        _obj = WebSocketEventSpeakerGroupChanged.parse_obj(
-            {"event_data": obj.get("eventData"), "event_type": obj.get("eventType")}
+        _obj = WebSocketEventStandConnected.parse_obj(
+            {
+                "event_data": (
+                    StandConnected.from_dict(obj.get("eventData"))
+                    if obj.get("eventData") is not None
+                    else None
+                ),
+                "event_type": obj.get("eventType"),
+            }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_speaker_link_status_changed.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_speaker_link_status_changed.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.speaker_link_status import SpeakerLinkStatus
 
 
 class WebSocketEventSpeakerLinkStatusChanged(BaseModel):
     """
     WebSocketEventSpeakerLinkStatusChanged
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_stand_position.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_stand_position.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.stand_position import StandPosition
 
 
 class WebSocketEventStandPosition(BaseModel):
     """
     WebSocketEventStandPosition
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_tv_info.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_wisa_out_state.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-from mozart_api.models.tv_info_event_data import TvInfoEventData
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
+from mozart_api.models.wisa_out_state import WisaOutState
 
-class WebSocketEventTvInfo(BaseModel):
+
+class WebSocketEventWisaOutState(BaseModel):
     """
-    WebSocketEventTvInfo
+    Speaker Discovery State changed  # noqa: E501
     """
 
-    event_data: Optional[TvInfoEventData] = Field(None, alias="eventData")
-    event_type: Optional[StrictStr] = Field(None, alias="eventType")
+    event_data: WisaOutState = Field(..., alias="eventData")
+    event_type: StrictStr = Field(..., alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -44,39 +47,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventTvInfo:
-        """Create an instance of WebSocketEventTvInfo from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventWisaOutState:
+        """Create an instance of WebSocketEventWisaOutState from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of event_data
         if self.event_data:
             _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventTvInfo:
-        """Create an instance of WebSocketEventTvInfo from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventWisaOutState:
+        """Create an instance of WebSocketEventWisaOutState from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventTvInfo.parse_obj(obj)
+            return WebSocketEventWisaOutState.parse_obj(obj)
 
-        _obj = WebSocketEventTvInfo.parse_obj(
+        _obj = WebSocketEventWisaOutState.parse_obj(
             {
                 "event_data": (
-                    TvInfoEventData.from_dict(obj.get("eventData"))
+                    WisaOutState.from_dict(obj.get("eventData"))
                     if obj.get("eventData") is not None
                     else None
                 ),
                 "event_type": obj.get("eventType"),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_volume.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_volume.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
+
 from mozart_api.models.volume_state import VolumeState
 
 
 class WebSocketEventVolume(BaseModel):
     """
     WebSocketEventVolume
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/web_socket_event_wisa_out_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/web_socket_event_active_speaker_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
-from mozart_api.models.wisa_out_state import WisaOutState
+from typing import Optional
 
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr
 
-class WebSocketEventWisaOutState(BaseModel):
+from mozart_api.models.speaker_group_overview import SpeakerGroupOverview
+
+
+class WebSocketEventActiveSpeakerGroup(BaseModel):
     """
-    Speaker Discovery State changed  # noqa: E501
+    WebSocketEventActiveSpeakerGroup
     """
 
-    event_data: WisaOutState = Field(..., alias="eventData")
-    event_type: StrictStr = Field(..., alias="eventType")
+    event_data: Optional[SpeakerGroupOverview] = Field(None, alias="eventData")
+    event_type: Optional[StrictStr] = Field(None, alias="eventType")
     __properties = ["eventData", "eventType"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -43,39 +49,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebSocketEventWisaOutState:
-        """Create an instance of WebSocketEventWisaOutState from a JSON string"""
+    def from_json(cls, json_str: str) -> WebSocketEventActiveSpeakerGroup:
+        """Create an instance of WebSocketEventActiveSpeakerGroup from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of event_data
         if self.event_data:
             _dict["eventData"] = self.event_data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebSocketEventWisaOutState:
-        """Create an instance of WebSocketEventWisaOutState from a dict"""
+    def from_dict(cls, obj: dict) -> WebSocketEventActiveSpeakerGroup:
+        """Create an instance of WebSocketEventActiveSpeakerGroup from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebSocketEventWisaOutState.parse_obj(obj)
+            return WebSocketEventActiveSpeakerGroup.parse_obj(obj)
 
-        _obj = WebSocketEventWisaOutState.parse_obj(
+        _obj = WebSocketEventActiveSpeakerGroup.parse_obj(
             {
                 "event_data": (
-                    WisaOutState.from_dict(obj.get("eventData"))
+                    SpeakerGroupOverview.from_dict(obj.get("eventData"))
                     if obj.get("eventData") is not None
                     else None
                 ),
                 "event_type": obj.get("eventType"),
             }
         )
         return _obj
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/websocket_notification_tag.py` & `mozart_api-3.4.1.8.5/mozart_api/models/websocket_notification_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class WebsocketNotificationTag(BaseModel):
     """
     WebsocketNotificationTag
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/models/wisa_out_state.py` & `mozart_api-3.4.1.8.5/mozart_api/models/wisa_out_state.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr, validator
+
+try:
+    from pydantic.v1 import BaseModel, StrictStr, validator
+except ImportError:
+    from pydantic import BaseModel, StrictStr, validator
 
 
 class WisaOutState(BaseModel):
     """
     WisaOutState
     """
```

### Comparing `mozart_api-3.4.1.8.4/mozart_api/mozart_cli.py` & `mozart_api-3.4.1.8.5/mozart_api/mozart_cli.py`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/mozart_api/mozart_client.py` & `mozart_api-3.4.1.8.5/mozart_api/mozart_client.py`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/mozart_api/rest.py` & `mozart_api-3.4.1.8.5/mozart_api/rest.py`

 * *Files identical despite different names*

### Comparing `mozart_api-3.4.1.8.4/pyproject.toml` & `mozart_api-3.4.1.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mozart_api"
-version = "3.4.1.8.4"
+version = "3.4.1.8.5"
 description = "Mozart platform API"
 authors = [
     "BangOlufsen <support@bang-olufsen.dk>",
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bang-olufsen/mozart-open-api"
@@ -29,15 +29,15 @@
     "test",
 ]
 
 [tool.poetry.dependencies]
 urllib3 = ">= 1.25.3"
 python-dateutil = ">=2.8.2"
 aiohttp = ">=3.8.3"
-pydantic = "^1.10.5, <2"
+pydantic = ">=1.10"
 aenum = ">=3.1.11"
 aioconsole = ">=0.4.1"
 inflection = ">=0.5.1"
 typing-extensions = ">=4.7.1"
 zeroconf = ">=0.25.1"
 websockets = ">=12.0"
 python = ">=3.11"
```

### Comparing `mozart_api-3.4.1.8.4/PKG-INFO` & `mozart_api-3.4.1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozart_api
-Version: 3.4.1.8.4
+Version: 3.4.1.8.5
 Summary: Mozart platform API
 Home-page: https://pypi.org/project/mozart-api/
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Mozart platform API
 Author: BangOlufsen
 Author-email: support@bang-olufsen.dk
 Requires-Python: >=3.11
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia
 Requires-Dist: aenum (>=3.1.11)
 Requires-Dist: aioconsole (>=0.4.1)
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: inflection (>=0.5.1)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=1.10)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: typing-extensions (>=4.7.1)
 Requires-Dist: urllib3 (>=1.25.3)
 Requires-Dist: websockets (>=12.0)
 Requires-Dist: zeroconf (>=0.25.1)
 Project-URL: Bug Tracker, https://github.com/bang-olufsen/mozart-open-api/issues
 Project-URL: Documentation, https://bang-olufsen.github.io/mozart-open-api/
```

