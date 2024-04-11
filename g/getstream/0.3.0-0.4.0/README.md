# Comparing `tmp/getstream-0.3.0.tar.gz` & `tmp/getstream-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getstream-0.3.0.tar", max compression
+gzip compressed data, was "getstream-0.4.0.tar", max compression
```

## Comparing `getstream-0.3.0.tar` & `getstream-0.4.0.tar`

### file list

```diff
@@ -1,555 +1,555 @@
--rw-r--r--   0        0        0    14205 2023-07-11 09:24:31.518666 getstream-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     3918 2023-11-15 09:53:17.481311 getstream-0.3.0/README.md
--rw-r--r--   0        0        0       98 2024-03-06 06:15:35.459426 getstream-0.3.0/getstream/__init__.py
--rw-r--r--   0        0        0       46 2023-07-07 15:26:52.041698 getstream-0.3.0/getstream/async_/__init__.py
--rw-r--r--   0        0        0      965 2023-04-24 16:13:28.085563 getstream-0.3.0/getstream/async_/base.py
--rw-r--r--   0        0        0      225 2023-05-05 11:48:07.700181 getstream-0.3.0/getstream/async_/stream.py
--rw-r--r--   0        0        0     1422 2023-11-15 09:53:17.481818 getstream-0.3.0/getstream/base.py
--rw-r--r--   0        0        0        0 2023-10-26 15:09:14.788653 getstream-0.3.0/getstream/chat/__init__.py
--rw-r--r--   0        0        0       47 2023-07-07 15:27:10.735770 getstream-0.3.0/getstream/chat/async_/__init__.py
--rw-r--r--   0        0        0      140 2023-05-05 11:47:33.873776 getstream-0.3.0/getstream/chat/async_/chat.py
--rw-r--r--   0        0        0        0 2023-10-26 15:07:47.200051 getstream-0.3.0/getstream/chat/models/__init__.py
--rw-r--r--   0        0        0      616 2023-10-25 08:58:18.671682 getstream-0.3.0/getstream/chat/models/action.py
--rw-r--r--   0        0        0      695 2023-10-25 08:58:18.671917 getstream-0.3.0/getstream/chat/models/action_request.py
--rw-r--r--   0        0        0      312 2023-10-25 08:58:18.672318 getstream-0.3.0/getstream/chat/models/agora_call.py
--rw-r--r--   0        0        0      637 2023-10-25 08:58:18.672462 getstream-0.3.0/getstream/chat/models/any_event.py
--rw-r--r--   0        0        0      816 2023-11-15 09:53:17.482317 getstream-0.3.0/getstream/chat/models/api_error.py
--rw-r--r--   0        0        0     1204 2023-10-25 08:58:18.672762 getstream-0.3.0/getstream/chat/models/apn_config_fields.py
--rw-r--r--   0        0        0     1307 2023-10-25 08:58:18.672908 getstream-0.3.0/getstream/chat/models/apn_config_request.py
--rw-r--r--   0        0        0      361 2023-10-26 15:09:01.347212 getstream-0.3.0/getstream/chat/models/apns.py
--rw-r--r--   0        0        0     4505 2023-10-25 08:58:18.673366 getstream-0.3.0/getstream/chat/models/app.py
--rw-r--r--   0        0        0      494 2023-10-25 08:58:18.673531 getstream-0.3.0/getstream/chat/models/async_moderation_callback_config_request.py
--rw-r--r--   0        0        0      669 2023-10-25 08:58:18.673678 getstream-0.3.0/getstream/chat/models/async_moderation_configuration_request.py
--rw-r--r--   0        0        0     2556 2023-10-25 08:58:18.673821 getstream-0.3.0/getstream/chat/models/attachment.py
--rw-r--r--   0        0        0     2643 2023-10-25 08:58:18.673987 getstream-0.3.0/getstream/chat/models/attachment_request.py
--rw-r--r--   0        0        0      723 2023-10-26 15:09:14.790299 getstream-0.3.0/getstream/chat/models/audio_settings.py
--rw-r--r--   0        0        0     1033 2023-10-25 08:58:18.674292 getstream-0.3.0/getstream/chat/models/automod_details.py
--rw-r--r--   0        0        0      321 2023-10-26 15:09:01.378280 getstream-0.3.0/getstream/chat/models/backstage_settings.py
--rw-r--r--   0        0        0     1366 2023-10-25 08:58:18.674779 getstream-0.3.0/getstream/chat/models/ban_request.py
--rw-r--r--   0        0        0     1546 2023-10-25 08:58:18.675032 getstream-0.3.0/getstream/chat/models/ban_response.py
--rw-r--r--   0        0        0     1094 2023-10-25 08:58:18.675225 getstream-0.3.0/getstream/chat/models/block_list.py
--rw-r--r--   0        0        0      445 2023-10-25 08:58:18.675444 getstream-0.3.0/getstream/chat/models/broadcast_settings.py
--rw-r--r--   0        0        0      744 2023-10-25 08:58:18.675872 getstream-0.3.0/getstream/chat/models/call.py
--rw-r--r--   0        0        0     1970 2023-10-25 08:58:18.676013 getstream-0.3.0/getstream/chat/models/call_settings.py
--rw-r--r--   0        0        0     1411 2023-10-25 08:58:18.676145 getstream-0.3.0/getstream/chat/models/call_type.py
--rw-r--r--   0        0        0     3811 2023-10-25 08:58:18.676286 getstream-0.3.0/getstream/chat/models/campaign.py
--rw-r--r--   0        0        0     1091 2023-10-25 08:58:18.676459 getstream-0.3.0/getstream/chat/models/campaign_data_request.py
--rw-r--r--   0        0        0      546 2023-10-25 08:58:18.676607 getstream-0.3.0/getstream/chat/models/campaign_sort.py
--rw-r--r--   0        0        0      379 2023-10-25 08:58:18.676754 getstream-0.3.0/getstream/chat/models/campaign_sort_field.py
--rw-r--r--   0        0        0     1227 2023-10-25 08:58:18.676917 getstream-0.3.0/getstream/chat/models/campaign_updateable_fields_request.py
--rw-r--r--   0        0        0     3190 2023-10-25 08:58:18.677066 getstream-0.3.0/getstream/chat/models/channel.py
--rw-r--r--   0        0        0     2644 2023-10-25 08:58:18.677219 getstream-0.3.0/getstream/chat/models/channel_config.py
--rw-r--r--   0        0        0     1485 2023-10-25 08:58:18.677374 getstream-0.3.0/getstream/chat/models/channel_config_request.py
--rw-r--r--   0        0        0     2829 2023-10-25 08:58:18.677523 getstream-0.3.0/getstream/chat/models/channel_config_with_info.py
--rw-r--r--   0        0        0     3600 2023-10-25 08:58:18.677671 getstream-0.3.0/getstream/chat/models/channel_config_with_info_request.py
--rw-r--r--   0        0        0      648 2023-10-25 08:58:18.677821 getstream-0.3.0/getstream/chat/models/channel_created_event.py
--rw-r--r--   0        0        0     1139 2023-10-25 08:58:18.677960 getstream-0.3.0/getstream/chat/models/channel_deleted_event.py
--rw-r--r--   0        0        0     1231 2023-10-25 08:58:18.678092 getstream-0.3.0/getstream/chat/models/channel_export_request.py
--rw-r--r--   0        0        0      847 2023-10-25 08:58:18.678246 getstream-0.3.0/getstream/chat/models/channel_frozen_event.py
--rw-r--r--   0        0        0     1650 2023-10-25 08:58:18.678395 getstream-0.3.0/getstream/chat/models/channel_get_or_create_request.py
--rw-r--r--   0        0        0     1279 2023-10-25 08:58:18.678539 getstream-0.3.0/getstream/chat/models/channel_hidden_event.py
--rw-r--r--   0        0        0     1056 2023-10-25 08:58:18.678685 getstream-0.3.0/getstream/chat/models/channel_kicked_event.py
--rw-r--r--   0        0        0     2798 2023-10-25 08:58:18.678856 getstream-0.3.0/getstream/chat/models/channel_member.py
--rw-r--r--   0        0        0     3061 2023-10-25 08:58:18.679027 getstream-0.3.0/getstream/chat/models/channel_member_request.py
--rw-r--r--   0        0        0      596 2023-10-25 08:58:18.679174 getstream-0.3.0/getstream/chat/models/channel_messages.py
--rw-r--r--   0        0        0     1463 2023-10-25 08:58:18.679329 getstream-0.3.0/getstream/chat/models/channel_mute.py
--rw-r--r--   0        0        0     1648 2023-10-25 08:58:18.679486 getstream-0.3.0/getstream/chat/models/channel_mute_request.py
--rw-r--r--   0        0        0      646 2023-10-25 08:58:18.679633 getstream-0.3.0/getstream/chat/models/channel_muted_event.py
--rw-r--r--   0        0        0     1929 2023-10-25 08:58:18.679810 getstream-0.3.0/getstream/chat/models/channel_request.py
--rw-r--r--   0        0        0     4341 2023-10-25 08:58:18.680190 getstream-0.3.0/getstream/chat/models/channel_response.py
--rw-r--r--   0        0        0     4563 2023-10-25 08:58:18.680421 getstream-0.3.0/getstream/chat/models/channel_response_request.py
--rw-r--r--   0        0        0     2153 2023-10-25 08:58:18.680555 getstream-0.3.0/getstream/chat/models/channel_state_response.py
--rw-r--r--   0        0        0     2093 2023-10-25 08:58:18.680706 getstream-0.3.0/getstream/chat/models/channel_state_response_fields.py
--rw-r--r--   0        0        0      514 2023-10-25 08:58:18.680850 getstream-0.3.0/getstream/chat/models/channel_stop_watching_request.py
--rw-r--r--   0        0        0     1059 2023-10-25 08:58:18.680997 getstream-0.3.0/getstream/chat/models/channel_truncated_event.py
--rw-r--r--   0        0        0     2942 2023-10-25 08:58:18.681136 getstream-0.3.0/getstream/chat/models/channel_type_config.py
--rw-r--r--   0        0        0      849 2023-10-25 08:58:18.681275 getstream-0.3.0/getstream/chat/models/channel_un_frozen_event.py
--rw-r--r--   0        0        0      648 2023-10-25 08:58:18.681421 getstream-0.3.0/getstream/chat/models/channel_unmuted_event.py
--rw-r--r--   0        0        0     1441 2023-10-25 08:58:18.681570 getstream-0.3.0/getstream/chat/models/channel_updated_event.py
--rw-r--r--   0        0        0     1022 2023-10-25 08:58:18.681737 getstream-0.3.0/getstream/chat/models/channel_visible_event.py
--rw-r--r--   0        0        0      555 2023-10-25 08:58:18.681905 getstream-0.3.0/getstream/chat/models/channels_response.py
--rw-r--r--   0        0        0     8795 2023-10-25 08:58:18.682134 getstream-0.3.0/getstream/chat/models/chat_event.py
--rw-r--r--   0        0        0     1389 2023-10-25 08:58:18.682297 getstream-0.3.0/getstream/chat/models/check_push_request.py
--rw-r--r--   0        0        0     1204 2023-10-25 08:58:18.682451 getstream-0.3.0/getstream/chat/models/check_push_response.py
--rw-r--r--   0        0        0      567 2023-10-25 08:58:18.682667 getstream-0.3.0/getstream/chat/models/check_sqs_request.py
--rw-r--r--   0        0        0      612 2023-10-25 08:58:18.682867 getstream-0.3.0/getstream/chat/models/check_sqs_response.py
--rw-r--r--   0        0        0     1206 2023-10-25 08:58:18.683030 getstream-0.3.0/getstream/chat/models/command.py
--rw-r--r--   0        0        0      636 2023-10-25 08:58:18.683193 getstream-0.3.0/getstream/chat/models/command_request.py
--rw-r--r--   0        0        0      649 2023-10-25 08:58:18.683360 getstream-0.3.0/getstream/chat/models/config.py
--rw-r--r--   0        0        0      656 2023-10-25 08:58:18.683500 getstream-0.3.0/getstream/chat/models/config_request.py
--rw-r--r--   0        0        0      590 2023-10-25 08:58:18.683644 getstream-0.3.0/getstream/chat/models/connect_request.py
--rw-r--r--   0        0        0      410 2023-10-25 08:58:18.683791 getstream-0.3.0/getstream/chat/models/create_block_list_request.py
--rw-r--r--   0        0        0      789 2023-10-25 08:58:18.683936 getstream-0.3.0/getstream/chat/models/create_call_request.py
--rw-r--r--   0        0        0      757 2023-10-25 08:58:18.684063 getstream-0.3.0/getstream/chat/models/create_call_response.py
--rw-r--r--   0        0        0      419 2023-10-25 08:58:18.684188 getstream-0.3.0/getstream/chat/models/create_campaign_request.py
--rw-r--r--   0        0        0      517 2023-10-25 08:58:18.684315 getstream-0.3.0/getstream/chat/models/create_campaign_response.py
--rw-r--r--   0        0        0     2595 2023-10-25 08:58:18.684455 getstream-0.3.0/getstream/chat/models/create_channel_type_request.py
--rw-r--r--   0        0        0     2962 2023-10-25 08:58:18.684590 getstream-0.3.0/getstream/chat/models/create_channel_type_response.py
--rw-r--r--   0        0        0      580 2023-10-25 08:58:18.684724 getstream-0.3.0/getstream/chat/models/create_command_request.py
--rw-r--r--   0        0        0      511 2023-10-25 08:58:18.684856 getstream-0.3.0/getstream/chat/models/create_command_response.py
--rw-r--r--   0        0        0      963 2023-10-26 15:09:14.791262 getstream-0.3.0/getstream/chat/models/create_device_request.py
--rw-r--r--   0        0        0      427 2023-10-25 08:58:18.685111 getstream-0.3.0/getstream/chat/models/create_import_request.py
--rw-r--r--   0        0        0      528 2023-10-25 08:58:18.685316 getstream-0.3.0/getstream/chat/models/create_import_response.py
--rw-r--r--   0        0        0      394 2023-10-25 08:58:18.685512 getstream-0.3.0/getstream/chat/models/create_import_url_request.py
--rw-r--r--   0        0        0      456 2023-10-25 08:58:18.685645 getstream-0.3.0/getstream/chat/models/create_import_url_response.py
--rw-r--r--   0        0        0      314 2023-10-25 08:58:18.685764 getstream-0.3.0/getstream/chat/models/create_role_request.py
--rw-r--r--   0        0        0      427 2023-10-25 08:58:18.685898 getstream-0.3.0/getstream/chat/models/create_role_response.py
--rw-r--r--   0        0        0      413 2023-10-25 08:58:18.686044 getstream-0.3.0/getstream/chat/models/create_segment_request.py
--rw-r--r--   0        0        0      511 2023-10-25 08:58:18.686190 getstream-0.3.0/getstream/chat/models/create_segment_response.py
--rw-r--r--   0        0        0      598 2023-10-25 08:58:18.686317 getstream-0.3.0/getstream/chat/models/deactivate_user_request.py
--rw-r--r--   0        0        0      502 2023-10-25 08:58:18.686447 getstream-0.3.0/getstream/chat/models/deactivate_user_response.py
--rw-r--r--   0        0        0      613 2023-10-25 08:58:18.686573 getstream-0.3.0/getstream/chat/models/deactivate_users_request.py
--rw-r--r--   0        0        0      392 2023-10-25 08:58:18.686697 getstream-0.3.0/getstream/chat/models/deactivate_users_response.py
--rw-r--r--   0        0        0      327 2023-10-25 08:58:18.686817 getstream-0.3.0/getstream/chat/models/delete_campaign_response.py
--rw-r--r--   0        0        0      536 2023-10-25 08:58:18.686948 getstream-0.3.0/getstream/chat/models/delete_channel_response.py
--rw-r--r--   0        0        0      494 2023-10-25 08:58:18.687075 getstream-0.3.0/getstream/chat/models/delete_channels_request.py
--rw-r--r--   0        0        0      656 2023-10-25 08:58:18.687218 getstream-0.3.0/getstream/chat/models/delete_channels_response.py
--rw-r--r--   0        0        0      434 2023-10-25 08:58:18.687362 getstream-0.3.0/getstream/chat/models/delete_channels_result.py
--rw-r--r--   0        0        0      384 2023-10-25 08:58:18.687488 getstream-0.3.0/getstream/chat/models/delete_command_response.py
--rw-r--r--   0        0        0      326 2023-10-25 08:58:18.687607 getstream-0.3.0/getstream/chat/models/delete_segment_response.py
--rw-r--r--   0        0        0      562 2023-10-25 08:58:18.687743 getstream-0.3.0/getstream/chat/models/delete_user_response.py
--rw-r--r--   0        0        0      792 2023-10-25 08:58:18.687867 getstream-0.3.0/getstream/chat/models/delete_users_request.py
--rw-r--r--   0        0        0      388 2023-10-25 08:58:18.687992 getstream-0.3.0/getstream/chat/models/delete_users_response.py
--rw-r--r--   0        0        0     1229 2023-10-26 15:09:14.792110 getstream-0.3.0/getstream/chat/models/device.py
--rw-r--r--   0        0        0      472 2023-10-25 08:58:18.688246 getstream-0.3.0/getstream/chat/models/device_error_info.py
--rw-r--r--   0        0        0      617 2023-10-25 08:58:18.688369 getstream-0.3.0/getstream/chat/models/device_fields.py
--rw-r--r--   0        0        0     1320 2023-10-25 08:58:18.688499 getstream-0.3.0/getstream/chat/models/device_request.py
--rw-r--r--   0        0        0      608 2023-10-25 08:58:18.688618 getstream-0.3.0/getstream/chat/models/error_result.py
--rw-r--r--   0        0        0     2952 2023-10-25 08:58:18.688732 getstream-0.3.0/getstream/chat/models/event.py
--rw-r--r--   0        0        0      433 2023-10-26 15:09:14.792601 getstream-0.3.0/getstream/chat/models/event_notification_settings.py
--rw-r--r--   0        0        0     3198 2023-10-25 08:58:18.689140 getstream-0.3.0/getstream/chat/models/event_request.py
--rw-r--r--   0        0        0      479 2023-10-25 08:58:18.689384 getstream-0.3.0/getstream/chat/models/event_response.py
--rw-r--r--   0        0        0      983 2023-10-25 08:58:18.689515 getstream-0.3.0/getstream/chat/models/export_channels_request.py
--rw-r--r--   0        0        0      391 2023-10-25 08:58:18.689637 getstream-0.3.0/getstream/chat/models/export_channels_response.py
--rw-r--r--   0        0        0      543 2023-10-25 08:58:18.689763 getstream-0.3.0/getstream/chat/models/export_channels_result.py
--rw-r--r--   0        0        0      837 2023-10-25 08:58:18.689897 getstream-0.3.0/getstream/chat/models/export_user_response.py
--rw-r--r--   0        0        0      354 2023-10-25 08:58:18.690027 getstream-0.3.0/getstream/chat/models/export_users_request.py
--rw-r--r--   0        0        0      388 2023-10-25 08:58:18.690147 getstream-0.3.0/getstream/chat/models/export_users_response.py
--rw-r--r--   0        0        0      425 2023-10-25 08:58:18.690266 getstream-0.3.0/getstream/chat/models/field.py
--rw-r--r--   0        0        0      533 2023-10-25 08:58:18.690388 getstream-0.3.0/getstream/chat/models/field_request.py
--rw-r--r--   0        0        0      323 2023-10-25 08:58:18.690516 getstream-0.3.0/getstream/chat/models/file_delete_response.py
--rw-r--r--   0        0        0      724 2023-10-25 08:58:18.690640 getstream-0.3.0/getstream/chat/models/file_upload_config.py
--rw-r--r--   0        0        0      837 2023-10-25 08:58:18.690762 getstream-0.3.0/getstream/chat/models/file_upload_config_request.py
--rw-r--r--   0        0        0      550 2023-10-25 08:58:18.690887 getstream-0.3.0/getstream/chat/models/file_upload_request.py
--rw-r--r--   0        0        0      540 2023-10-25 08:58:18.691010 getstream-0.3.0/getstream/chat/models/file_upload_response.py
--rw-r--r--   0        0        0      837 2023-10-25 08:58:18.691144 getstream-0.3.0/getstream/chat/models/firebase_config_fields.py
--rw-r--r--   0        0        0      978 2023-10-25 08:58:18.691273 getstream-0.3.0/getstream/chat/models/firebase_config_request.py
--rw-r--r--   0        0        0     2544 2023-10-25 08:58:18.691396 getstream-0.3.0/getstream/chat/models/flag.py
--rw-r--r--   0        0        0      457 2023-10-25 08:58:18.691532 getstream-0.3.0/getstream/chat/models/flag_details.py
--rw-r--r--   0        0        0      793 2023-10-25 08:58:18.691648 getstream-0.3.0/getstream/chat/models/flag_feedback.py
--rw-r--r--   0        0        0      733 2023-10-25 08:58:18.691783 getstream-0.3.0/getstream/chat/models/flag_message_details.py
--rw-r--r--   0        0        0      787 2023-10-25 08:58:18.691915 getstream-0.3.0/getstream/chat/models/flag_request.py
--rw-r--r--   0        0        0      473 2023-10-25 08:58:18.692033 getstream-0.3.0/getstream/chat/models/flag_response.py
--rw-r--r--   0        0        0      346 2023-10-26 15:09:01.808957 getstream-0.3.0/getstream/chat/models/geofence_settings.py
--rw-r--r--   0        0        0      426 2023-10-25 08:58:18.692373 getstream-0.3.0/getstream/chat/models/get_application_response.py
--rw-r--r--   0        0        0      521 2023-10-25 08:58:18.692498 getstream-0.3.0/getstream/chat/models/get_block_list_response.py
--rw-r--r--   0        0        0      557 2023-10-25 08:58:18.692620 getstream-0.3.0/getstream/chat/models/get_call_token_request.py
--rw-r--r--   0        0        0      632 2023-10-25 08:58:18.692737 getstream-0.3.0/getstream/chat/models/get_call_token_response.py
--rw-r--r--   0        0        0     1283 2023-10-25 08:58:18.692858 getstream-0.3.0/getstream/chat/models/get_command_response.py
--rw-r--r--   0        0        0      466 2023-10-25 08:58:18.692986 getstream-0.3.0/getstream/chat/models/get_custom_permission_response.py
--rw-r--r--   0        0        0     1418 2023-10-25 08:58:18.693116 getstream-0.3.0/getstream/chat/models/get_export_channels_status_response.py
--rw-r--r--   0        0        0      525 2023-10-25 08:58:18.693241 getstream-0.3.0/getstream/chat/models/get_import_response.py
--rw-r--r--   0        0        0      479 2023-10-25 08:58:18.693363 getstream-0.3.0/getstream/chat/models/get_many_messages_response.py
--rw-r--r--   0        0        0     2625 2023-10-25 08:58:18.693490 getstream-0.3.0/getstream/chat/models/get_og_response.py
--rw-r--r--   0        0        0      884 2023-10-25 08:58:18.693602 getstream-0.3.0/getstream/chat/models/get_rate_limits_response.py
--rw-r--r--   0        0        0      481 2023-10-25 08:58:18.693729 getstream-0.3.0/getstream/chat/models/get_reactions_response.py
--rw-r--r--   0        0        0      474 2023-10-25 08:58:18.693853 getstream-0.3.0/getstream/chat/models/get_replies_response.py
--rw-r--r--   0        0        0     1327 2023-10-25 08:58:18.694034 getstream-0.3.0/getstream/chat/models/get_task_response.py
--rw-r--r--   0        0        0      396 2023-10-25 08:58:18.694221 getstream-0.3.0/getstream/chat/models/guest_request.py
--rw-r--r--   0        0        0      567 2023-10-25 08:58:18.694526 getstream-0.3.0/getstream/chat/models/guest_response.py
--rw-r--r--   0        0        0      862 2023-10-26 15:09:14.793399 getstream-0.3.0/getstream/chat/models/health_check_event.py
--rw-r--r--   0        0        0      671 2023-10-25 08:58:18.694754 getstream-0.3.0/getstream/chat/models/hide_channel_request.py
--rw-r--r--   0        0        0      324 2023-10-25 08:58:18.694878 getstream-0.3.0/getstream/chat/models/hide_channel_response.py
--rw-r--r--   0        0        0      489 2023-10-25 08:58:18.694991 getstream-0.3.0/getstream/chat/models/hls_settings.py
--rw-r--r--   0        0        0      378 2023-10-25 08:58:18.695112 getstream-0.3.0/getstream/chat/models/hms_call.py
--rw-r--r--   0        0        0      515 2023-10-25 08:58:18.695231 getstream-0.3.0/getstream/chat/models/huawei_config_fields.py
--rw-r--r--   0        0        0      556 2023-10-25 08:58:18.695352 getstream-0.3.0/getstream/chat/models/huawei_config_request.py
--rw-r--r--   0        0        0      546 2023-10-25 08:58:18.695493 getstream-0.3.0/getstream/chat/models/image_data.py
--rw-r--r--   0        0        0      702 2023-10-25 08:58:18.695623 getstream-0.3.0/getstream/chat/models/image_data_request.py
--rw-r--r--   0        0        0      490 2023-10-25 08:58:18.695743 getstream-0.3.0/getstream/chat/models/image_size.py
--rw-r--r--   0        0        0      622 2023-10-25 08:58:18.695868 getstream-0.3.0/getstream/chat/models/image_size_request.py
--rw-r--r--   0        0        0      758 2023-10-25 08:58:18.695996 getstream-0.3.0/getstream/chat/models/image_upload_request.py
--rw-r--r--   0        0        0      726 2023-10-25 08:58:18.696122 getstream-0.3.0/getstream/chat/models/image_upload_response.py
--rw-r--r--   0        0        0      975 2023-10-25 08:58:18.696251 getstream-0.3.0/getstream/chat/models/images.py
--rw-r--r--   0        0        0     1284 2023-10-25 08:58:18.696370 getstream-0.3.0/getstream/chat/models/images_request.py
--rw-r--r--   0        0        0     1408 2023-10-25 08:58:18.696494 getstream-0.3.0/getstream/chat/models/import_task.py
--rw-r--r--   0        0        0      728 2023-10-25 08:58:18.696609 getstream-0.3.0/getstream/chat/models/import_task_history.py
--rw-r--r--   0        0        0      461 2023-10-25 08:58:18.696729 getstream-0.3.0/getstream/chat/models/label.py
--rw-r--r--   0        0        0      453 2023-10-25 08:58:18.696851 getstream-0.3.0/getstream/chat/models/label_thresholds.py
--rw-r--r--   0        0        0      460 2023-10-25 08:58:18.696972 getstream-0.3.0/getstream/chat/models/label_thresholds_request.py
--rw-r--r--   0        0        0      436 2023-10-25 08:58:18.697093 getstream-0.3.0/getstream/chat/models/limit_info.py
--rw-r--r--   0        0        0      488 2023-10-25 08:58:18.697221 getstream-0.3.0/getstream/chat/models/list_block_list_response.py
--rw-r--r--   0        0        0      541 2023-10-25 08:58:18.697339 getstream-0.3.0/getstream/chat/models/list_channel_types_response.py
--rw-r--r--   0        0        0      476 2023-10-25 08:58:18.697456 getstream-0.3.0/getstream/chat/models/list_commands_response.py
--rw-r--r--   0        0        0      470 2023-10-26 15:09:14.793996 getstream-0.3.0/getstream/chat/models/list_devices_response.py
--rw-r--r--   0        0        0      493 2023-10-25 08:58:18.697700 getstream-0.3.0/getstream/chat/models/list_imports_response.py
--rw-r--r--   0        0        0      494 2023-10-25 08:58:18.697827 getstream-0.3.0/getstream/chat/models/list_permissions_response.py
--rw-r--r--   0        0        0      548 2023-10-25 08:58:18.697954 getstream-0.3.0/getstream/chat/models/list_push_providers_response.py
--rw-r--r--   0        0        0      458 2023-10-25 08:58:18.698079 getstream-0.3.0/getstream/chat/models/list_roles_response.py
--rw-r--r--   0        0        0      561 2023-10-25 08:58:18.698212 getstream-0.3.0/getstream/chat/models/mark_channels_read_request.py
--rw-r--r--   0        0        0      661 2023-10-25 08:58:18.698378 getstream-0.3.0/getstream/chat/models/mark_read_request.py
--rw-r--r--   0        0        0      531 2023-10-25 08:58:18.698502 getstream-0.3.0/getstream/chat/models/mark_read_response.py
--rw-r--r--   0        0        0      625 2023-10-25 08:58:18.698632 getstream-0.3.0/getstream/chat/models/mark_unread_request.py
--rw-r--r--   0        0        0     1274 2023-10-25 08:58:18.698763 getstream-0.3.0/getstream/chat/models/member_added_event.py
--rw-r--r--   0        0        0     1194 2023-10-25 08:58:18.698939 getstream-0.3.0/getstream/chat/models/member_removed_event.py
--rw-r--r--   0        0        0     1276 2023-10-25 08:58:18.699136 getstream-0.3.0/getstream/chat/models/member_updated_event.py
--rw-r--r--   0        0        0      488 2023-10-25 08:58:18.699519 getstream-0.3.0/getstream/chat/models/members_response.py
--rw-r--r--   0        0        0     4607 2023-10-25 08:58:18.699794 getstream-0.3.0/getstream/chat/models/message.py
--rw-r--r--   0        0        0      721 2023-10-25 08:58:18.699924 getstream-0.3.0/getstream/chat/models/message_action_request.py
--rw-r--r--   0        0        0     1478 2023-10-25 08:58:18.700051 getstream-0.3.0/getstream/chat/models/message_deleted_event.py
--rw-r--r--   0        0        0     2668 2023-10-25 08:58:18.700180 getstream-0.3.0/getstream/chat/models/message_flag.py
--rw-r--r--   0        0        0     1306 2023-10-25 08:58:18.700307 getstream-0.3.0/getstream/chat/models/message_flagged_event.py
--rw-r--r--   0        0        0     1894 2023-10-25 08:58:18.700434 getstream-0.3.0/getstream/chat/models/message_moderation_result.py
--rw-r--r--   0        0        0     1477 2023-10-25 08:58:18.700564 getstream-0.3.0/getstream/chat/models/message_new_event.py
--rw-r--r--   0        0        0     2591 2023-10-25 08:58:18.700693 getstream-0.3.0/getstream/chat/models/message_pagination_params_request.py
--rw-r--r--   0        0        0     1229 2023-10-25 08:58:18.700823 getstream-0.3.0/getstream/chat/models/message_read_event.py
--rw-r--r--   0        0        0     2899 2023-10-25 08:58:18.700954 getstream-0.3.0/getstream/chat/models/message_request.py
--rw-r--r--   0        0        0     5213 2023-10-25 08:58:18.701161 getstream-0.3.0/getstream/chat/models/message_request_1.py
--rw-r--r--   0        0        0      505 2023-10-25 08:58:18.701281 getstream-0.3.0/getstream/chat/models/message_response.py
--rw-r--r--   0        0        0     1181 2023-10-25 08:58:18.701405 getstream-0.3.0/getstream/chat/models/message_unblocked_event.py
--rw-r--r--   0        0        0     1405 2023-10-25 08:58:18.701526 getstream-0.3.0/getstream/chat/models/message_updated_event.py
--rw-r--r--   0        0        0      677 2023-10-25 08:58:18.701650 getstream-0.3.0/getstream/chat/models/message_with_pending_metadata_response.py
--rw-r--r--   0        0        0      594 2023-10-25 08:58:18.701771 getstream-0.3.0/getstream/chat/models/moderation_response.py
--rw-r--r--   0        0        0      778 2023-10-25 08:58:18.701897 getstream-0.3.0/getstream/chat/models/moderation_response_request.py
--rw-r--r--   0        0        0      750 2023-10-25 08:58:18.702017 getstream-0.3.0/getstream/chat/models/mute_channel_request.py
--rw-r--r--   0        0        0      825 2023-10-25 08:58:18.702142 getstream-0.3.0/getstream/chat/models/mute_channel_response.py
--rw-r--r--   0        0        0      723 2023-10-25 08:58:18.702259 getstream-0.3.0/getstream/chat/models/mute_user_request.py
--rw-r--r--   0        0        0      764 2023-10-25 08:58:18.702382 getstream-0.3.0/getstream/chat/models/mute_user_response.py
--rw-r--r--   0        0        0     1242 2023-10-25 08:58:18.702511 getstream-0.3.0/getstream/chat/models/notification_added_to_channel_event.py
--rw-r--r--   0        0        0     1151 2023-10-25 08:58:18.702629 getstream-0.3.0/getstream/chat/models/notification_channel_deleted_event.py
--rw-r--r--   0        0        0      774 2023-10-25 08:58:18.702752 getstream-0.3.0/getstream/chat/models/notification_channel_mutes_updated_event.py
--rw-r--r--   0        0        0     1071 2023-10-25 08:58:18.702883 getstream-0.3.0/getstream/chat/models/notification_channel_truncated_event.py
--rw-r--r--   0        0        0     1388 2023-10-25 08:58:18.703010 getstream-0.3.0/getstream/chat/models/notification_invite_accepted_event.py
--rw-r--r--   0        0        0     1388 2023-10-25 08:58:18.703140 getstream-0.3.0/getstream/chat/models/notification_invite_rejected_event.py
--rw-r--r--   0        0        0     1381 2023-10-25 08:58:18.703256 getstream-0.3.0/getstream/chat/models/notification_invited_event.py
--rw-r--r--   0        0        0     1531 2023-10-25 08:58:18.703369 getstream-0.3.0/getstream/chat/models/notification_mark_read_event.py
--rw-r--r--   0        0        0     2091 2023-10-25 08:58:18.703493 getstream-0.3.0/getstream/chat/models/notification_mark_unread_event.py
--rw-r--r--   0        0        0      767 2023-10-25 08:58:18.703621 getstream-0.3.0/getstream/chat/models/notification_mutes_updated_event.py
--rw-r--r--   0        0        0     1265 2023-10-25 08:58:18.703742 getstream-0.3.0/getstream/chat/models/notification_new_message_event.py
--rw-r--r--   0        0        0     1392 2023-10-25 08:58:18.703864 getstream-0.3.0/getstream/chat/models/notification_removed_from_channel_event.py
--rw-r--r--   0        0        0      873 2023-10-26 15:09:14.794332 getstream-0.3.0/getstream/chat/models/notification_settings.py
--rw-r--r--   0        0        0      310 2023-10-25 08:58:18.704099 getstream-0.3.0/getstream/chat/models/only_user_id_request.py
--rw-r--r--   0        0        0     3278 2023-10-25 08:58:18.704217 getstream-0.3.0/getstream/chat/models/own_user.py
--rw-r--r--   0        0        0     3850 2023-10-25 08:58:18.704334 getstream-0.3.0/getstream/chat/models/own_user_request.py
--rw-r--r--   0        0        0      801 2023-10-25 08:58:18.704444 getstream-0.3.0/getstream/chat/models/pagination_params_request.py
--rw-r--r--   0        0        0      861 2023-10-25 08:58:18.704560 getstream-0.3.0/getstream/chat/models/pending_message.py
--rw-r--r--   0        0        0      973 2023-10-25 08:58:18.704669 getstream-0.3.0/getstream/chat/models/permission.py
--rw-r--r--   0        0        0     1224 2023-10-25 08:58:18.704784 getstream-0.3.0/getstream/chat/models/policy.py
--rw-r--r--   0        0        0      798 2023-10-25 08:58:18.704909 getstream-0.3.0/getstream/chat/models/policy_request.py
--rw-r--r--   0        0        0      665 2023-10-25 08:58:18.705029 getstream-0.3.0/getstream/chat/models/policy_request_1.py
--rw-r--r--   0        0        0      486 2023-10-25 08:58:18.705135 getstream-0.3.0/getstream/chat/models/push_config_request.py
--rw-r--r--   0        0        0     1216 2023-10-25 08:58:18.705245 getstream-0.3.0/getstream/chat/models/push_notification_fields.py
--rw-r--r--   0        0        0      796 2023-10-25 08:58:18.705435 getstream-0.3.0/getstream/chat/models/push_notification_settings.py
--rw-r--r--   0        0        0      803 2023-10-25 08:58:18.705551 getstream-0.3.0/getstream/chat/models/push_notification_settings_request.py
--rw-r--r--   0        0        0     3775 2023-10-25 08:58:18.705668 getstream-0.3.0/getstream/chat/models/push_provider.py
--rw-r--r--   0        0        0     3926 2023-10-25 08:58:18.705790 getstream-0.3.0/getstream/chat/models/push_provider_request.py
--rw-r--r--   0        0        0     4086 2023-10-25 08:58:18.705921 getstream-0.3.0/getstream/chat/models/push_provider_response.py
--rw-r--r--   0        0        0     2349 2023-10-25 08:58:18.706043 getstream-0.3.0/getstream/chat/models/query_banned_users_request.py
--rw-r--r--   0        0        0      485 2023-10-25 08:58:18.706168 getstream-0.3.0/getstream/chat/models/query_banned_users_response.py
--rw-r--r--   0        0        0      657 2023-10-25 08:58:18.706289 getstream-0.3.0/getstream/chat/models/query_campaigns_request.py
--rw-r--r--   0        0        0      886 2023-10-25 08:58:18.706413 getstream-0.3.0/getstream/chat/models/query_campaigns_response.py
--rw-r--r--   0        0        0     1744 2023-10-25 08:58:18.706535 getstream-0.3.0/getstream/chat/models/query_channels_request.py
--rw-r--r--   0        0        0     3098 2023-10-26 15:09:14.794908 getstream-0.3.0/getstream/chat/models/query_members_request.py
--rw-r--r--   0        0        0      838 2023-10-25 08:58:18.706781 getstream-0.3.0/getstream/chat/models/query_message_flags_request.py
--rw-r--r--   0        0        0      488 2023-10-25 08:58:18.706897 getstream-0.3.0/getstream/chat/models/query_message_flags_response.py
--rw-r--r--   0        0        0      658 2023-10-25 08:58:18.707017 getstream-0.3.0/getstream/chat/models/query_recipients_request.py
--rw-r--r--   0        0        0     1028 2023-10-25 08:58:18.707147 getstream-0.3.0/getstream/chat/models/query_recipients_response.py
--rw-r--r--   0        0        0      656 2023-10-25 08:58:18.707263 getstream-0.3.0/getstream/chat/models/query_segments_request.py
--rw-r--r--   0        0        0      477 2023-10-25 08:58:18.707386 getstream-0.3.0/getstream/chat/models/query_segments_response.py
--rw-r--r--   0        0        0     1603 2023-10-25 08:58:18.707509 getstream-0.3.0/getstream/chat/models/query_users_request.py
--rw-r--r--   0        0        0     1265 2023-10-25 08:58:18.707637 getstream-0.3.0/getstream/chat/models/reaction.py
--rw-r--r--   0        0        0     1567 2023-10-25 08:58:18.707757 getstream-0.3.0/getstream/chat/models/reaction_deleted_event.py
--rw-r--r--   0        0        0     1563 2023-10-25 08:58:18.707885 getstream-0.3.0/getstream/chat/models/reaction_new_event.py
--rw-r--r--   0        0        0      674 2023-10-25 08:58:18.708017 getstream-0.3.0/getstream/chat/models/reaction_removal_response.py
--rw-r--r--   0        0        0      803 2023-10-25 08:58:18.708139 getstream-0.3.0/getstream/chat/models/reaction_request.py
--rw-r--r--   0        0        0      667 2023-10-26 15:09:14.795218 getstream-0.3.0/getstream/chat/models/reaction_response.py
--rw-r--r--   0        0        0     1346 2023-10-25 08:58:18.708384 getstream-0.3.0/getstream/chat/models/reaction_updated_event.py
--rw-r--r--   0        0        0      670 2023-10-25 08:58:18.708508 getstream-0.3.0/getstream/chat/models/reactivate_user_request.py
--rw-r--r--   0        0        0      502 2023-10-25 08:58:18.708625 getstream-0.3.0/getstream/chat/models/reactivate_user_response.py
--rw-r--r--   0        0        0      603 2023-10-25 08:58:18.708749 getstream-0.3.0/getstream/chat/models/reactivate_users_request.py
--rw-r--r--   0        0        0      392 2023-10-25 08:58:18.708868 getstream-0.3.0/getstream/chat/models/reactivate_users_response.py
--rw-r--r--   0        0        0      955 2023-10-25 08:58:18.708989 getstream-0.3.0/getstream/chat/models/read.py
--rw-r--r--   0        0        0     1228 2023-10-25 08:58:18.709107 getstream-0.3.0/getstream/chat/models/recipient.py
--rw-r--r--   0        0        0      446 2023-10-25 08:58:18.709225 getstream-0.3.0/getstream/chat/models/record_settings.py
--rw-r--r--   0        0        0      313 2023-10-26 15:09:02.046131 getstream-0.3.0/getstream/chat/models/response.py
--rw-r--r--   0        0        0      355 2023-10-25 08:58:18.709586 getstream-0.3.0/getstream/chat/models/restore_users_request.py
--rw-r--r--   0        0        0      517 2023-10-25 08:58:18.709710 getstream-0.3.0/getstream/chat/models/resume_campaign_response.py
--rw-r--r--   0        0        0      471 2023-10-26 15:09:02.059585 getstream-0.3.0/getstream/chat/models/ring_settings.py
--rw-r--r--   0        0        0     1024 2023-10-25 08:58:18.710024 getstream-0.3.0/getstream/chat/models/role.py
--rw-r--r--   0        0        0      405 2023-10-25 08:58:18.710139 getstream-0.3.0/getstream/chat/models/schedule_campaign_request.py
--rw-r--r--   0        0        0      519 2023-10-25 08:58:18.710247 getstream-0.3.0/getstream/chat/models/schedule_campaign_response.py
--rw-r--r--   0        0        0      434 2023-10-26 15:09:02.074120 getstream-0.3.0/getstream/chat/models/screensharing_settings.py
--rw-r--r--   0        0        0     1056 2023-10-25 08:58:18.710499 getstream-0.3.0/getstream/chat/models/search_request.py
--rw-r--r--   0        0        0      871 2023-10-25 08:58:18.710612 getstream-0.3.0/getstream/chat/models/search_response.py
--rw-r--r--   0        0        0      474 2023-10-25 08:58:18.710723 getstream-0.3.0/getstream/chat/models/search_result.py
--rw-r--r--   0        0        0     4738 2023-10-25 08:58:18.710901 getstream-0.3.0/getstream/chat/models/search_result_message.py
--rw-r--r--   0        0        0      709 2023-10-25 08:58:18.711015 getstream-0.3.0/getstream/chat/models/search_warning.py
--rw-r--r--   0        0        0     1339 2023-10-25 08:58:18.711135 getstream-0.3.0/getstream/chat/models/segment.py
--rw-r--r--   0        0        0      594 2023-10-25 08:58:18.711282 getstream-0.3.0/getstream/chat/models/segment_data_request.py
--rw-r--r--   0        0        0      692 2023-10-25 08:58:18.711395 getstream-0.3.0/getstream/chat/models/segment_updateable_fields_request.py
--rw-r--r--   0        0        0      386 2023-10-26 15:09:14.795578 getstream-0.3.0/getstream/chat/models/send_event_request.py
--rw-r--r--   0        0        0     1178 2023-10-25 08:58:18.711624 getstream-0.3.0/getstream/chat/models/send_message_request.py
--rw-r--r--   0        0        0      734 2023-10-26 15:09:14.796180 getstream-0.3.0/getstream/chat/models/send_reaction_request.py
--rw-r--r--   0        0        0      428 2023-10-25 08:58:18.711851 getstream-0.3.0/getstream/chat/models/send_user_custom_event_request.py
--rw-r--r--   0        0        0      556 2023-10-25 08:58:18.711969 getstream-0.3.0/getstream/chat/models/show_channel_request.py
--rw-r--r--   0        0        0      324 2023-10-25 08:58:18.712076 getstream-0.3.0/getstream/chat/models/show_channel_response.py
--rw-r--r--   0        0        0      467 2023-10-25 08:58:18.712181 getstream-0.3.0/getstream/chat/models/sort_param.py
--rw-r--r--   0        0        0      474 2023-10-26 15:09:02.167719 getstream-0.3.0/getstream/chat/models/sort_param_request.py
--rw-r--r--   0        0        0      515 2023-10-25 08:58:18.712399 getstream-0.3.0/getstream/chat/models/stop_campaign_response.py
--rw-r--r--   0        0        0      325 2023-10-25 08:58:18.712518 getstream-0.3.0/getstream/chat/models/stop_watching_response.py
--rw-r--r--   0        0        0     1446 2023-10-25 08:58:18.712627 getstream-0.3.0/getstream/chat/models/sync_request.py
--rw-r--r--   0        0        0      596 2023-10-25 08:58:18.712745 getstream-0.3.0/getstream/chat/models/sync_response.py
--rw-r--r--   0        0        0      441 2023-10-26 15:09:14.796674 getstream-0.3.0/getstream/chat/models/target_resolution.py
--rw-r--r--   0        0        0      349 2023-10-25 08:58:18.713049 getstream-0.3.0/getstream/chat/models/test_campaign_request.py
--rw-r--r--   0        0        0      623 2023-10-25 08:58:18.713160 getstream-0.3.0/getstream/chat/models/test_campaign_response.py
--rw-r--r--   0        0        0      679 2023-10-25 08:58:18.713267 getstream-0.3.0/getstream/chat/models/thresholds.py
--rw-r--r--   0        0        0      722 2023-10-25 08:58:18.713375 getstream-0.3.0/getstream/chat/models/thresholds_request.py
--rw-r--r--   0        0        0      406 2023-10-26 15:09:02.167671 getstream-0.3.0/getstream/chat/models/transcription_settings.py
--rw-r--r--   0        0        0      328 2023-10-25 08:58:18.713609 getstream-0.3.0/getstream/chat/models/translate_message_request.py
--rw-r--r--   0        0        0     1351 2023-10-25 08:58:18.713740 getstream-0.3.0/getstream/chat/models/truncate_channel_request.py
--rw-r--r--   0        0        0      694 2023-10-25 08:58:18.713850 getstream-0.3.0/getstream/chat/models/truncate_channel_response.py
--rw-r--r--   0        0        0     1125 2023-10-25 08:58:18.713957 getstream-0.3.0/getstream/chat/models/typing_start_event.py
--rw-r--r--   0        0        0     1124 2023-10-25 08:58:18.714067 getstream-0.3.0/getstream/chat/models/typing_stop_event.py
--rw-r--r--   0        0        0      824 2023-10-25 08:58:18.714176 getstream-0.3.0/getstream/chat/models/unmute_channel_request.py
--rw-r--r--   0        0        0      319 2023-10-25 08:58:18.714414 getstream-0.3.0/getstream/chat/models/unmute_response.py
--rw-r--r--   0        0        0      793 2023-10-25 08:58:18.714527 getstream-0.3.0/getstream/chat/models/unmute_user_request.py
--rw-r--r--   0        0        0     5778 2023-10-25 08:58:18.714701 getstream-0.3.0/getstream/chat/models/update_app_request.py
--rw-r--r--   0        0        0      482 2023-10-25 08:58:18.714804 getstream-0.3.0/getstream/chat/models/update_block_list_request.py
--rw-r--r--   0        0        0      479 2023-10-25 08:58:18.714904 getstream-0.3.0/getstream/chat/models/update_campaign_request.py
--rw-r--r--   0        0        0      517 2023-10-25 08:58:18.715020 getstream-0.3.0/getstream/chat/models/update_campaign_response.py
--rw-r--r--   0        0        0      713 2023-10-25 08:58:18.715134 getstream-0.3.0/getstream/chat/models/update_channel_partial_request.py
--rw-r--r--   0        0        0      692 2023-10-25 08:58:18.715242 getstream-0.3.0/getstream/chat/models/update_channel_partial_response.py
--rw-r--r--   0        0        0     2211 2023-10-25 08:58:18.715348 getstream-0.3.0/getstream/chat/models/update_channel_request.py
--rw-r--r--   0        0        0      841 2023-10-25 08:58:18.715456 getstream-0.3.0/getstream/chat/models/update_channel_response.py
--rw-r--r--   0        0        0     3054 2023-10-25 08:58:18.715567 getstream-0.3.0/getstream/chat/models/update_channel_type_request.py
--rw-r--r--   0        0        0     2962 2023-10-25 08:58:18.715683 getstream-0.3.0/getstream/chat/models/update_channel_type_response.py
--rw-r--r--   0        0        0      604 2023-10-25 08:58:18.715807 getstream-0.3.0/getstream/chat/models/update_command_request.py
--rw-r--r--   0        0        0      511 2023-10-25 08:58:18.715934 getstream-0.3.0/getstream/chat/models/update_command_response.py
--rw-r--r--   0        0        0      832 2023-10-25 08:58:18.716062 getstream-0.3.0/getstream/chat/models/update_message_partial_request.py
--rw-r--r--   0        0        0      700 2023-10-25 08:58:18.716182 getstream-0.3.0/getstream/chat/models/update_message_request.py
--rw-r--r--   0        0        0      473 2023-10-25 08:58:18.716296 getstream-0.3.0/getstream/chat/models/update_segment_request.py
--rw-r--r--   0        0        0      511 2023-10-25 08:58:18.716407 getstream-0.3.0/getstream/chat/models/update_segment_response.py
--rw-r--r--   0        0        0      484 2023-10-25 08:58:18.716512 getstream-0.3.0/getstream/chat/models/update_user_partial_request.py
--rw-r--r--   0        0        0      439 2023-10-25 08:58:18.716615 getstream-0.3.0/getstream/chat/models/update_users_request.py
--rw-r--r--   0        0        0      484 2023-10-25 08:58:18.716803 getstream-0.3.0/getstream/chat/models/update_users_response.py
--rw-r--r--   0        0        0      499 2023-10-25 08:58:18.716914 getstream-0.3.0/getstream/chat/models/upsert_push_provider_request.py
--rw-r--r--   0        0        0      517 2023-10-25 08:58:18.717082 getstream-0.3.0/getstream/chat/models/upsert_push_provider_response.py
--rw-r--r--   0        0        0     1622 2023-10-25 08:58:18.717262 getstream-0.3.0/getstream/chat/models/user_banned_event.py
--rw-r--r--   0        0        0      739 2023-10-25 08:58:18.717586 getstream-0.3.0/getstream/chat/models/user_custom_event_request.py
--rw-r--r--   0        0        0      900 2023-10-25 08:58:18.717696 getstream-0.3.0/getstream/chat/models/user_deactivated_event.py
--rw-r--r--   0        0        0     1120 2023-10-25 08:58:18.717807 getstream-0.3.0/getstream/chat/models/user_deleted_event.py
--rw-r--r--   0        0        0     1053 2023-10-25 08:58:18.717917 getstream-0.3.0/getstream/chat/models/user_flagged_event.py
--rw-r--r--   0        0        0     1386 2023-10-25 08:58:18.718026 getstream-0.3.0/getstream/chat/models/user_mute.py
--rw-r--r--   0        0        0     1556 2023-10-25 08:58:18.718138 getstream-0.3.0/getstream/chat/models/user_mute_request.py
--rw-r--r--   0        0        0     1051 2023-10-25 08:58:18.718249 getstream-0.3.0/getstream/chat/models/user_muted_event.py
--rw-r--r--   0        0        0     3281 2024-02-05 13:29:16.706111 getstream-0.3.0/getstream/chat/models/user_object.py
--rw-r--r--   0        0        0     1814 2023-10-25 08:58:18.718539 getstream-0.3.0/getstream/chat/models/user_object_request.py
--rw-r--r--   0        0        0      827 2023-10-25 08:58:18.718645 getstream-0.3.0/getstream/chat/models/user_presence_changed_event.py
--rw-r--r--   0        0        0      823 2023-10-25 08:58:18.718754 getstream-0.3.0/getstream/chat/models/user_reactivated_event.py
--rw-r--r--   0        0        0      811 2023-10-26 15:09:14.797466 getstream-0.3.0/getstream/chat/models/user_request.py
--rw-r--r--   0        0        0     3360 2023-10-26 15:09:14.797704 getstream-0.3.0/getstream/chat/models/user_response.py
--rw-r--r--   0        0        0     1165 2023-10-25 08:58:18.719080 getstream-0.3.0/getstream/chat/models/user_unbanned_event.py
--rw-r--r--   0        0        0     1053 2023-10-25 08:58:18.719189 getstream-0.3.0/getstream/chat/models/user_unmuted_event.py
--rw-r--r--   0        0        0      988 2023-10-25 08:58:18.719302 getstream-0.3.0/getstream/chat/models/user_unread_reminder_event.py
--rw-r--r--   0        0        0      819 2023-10-25 08:58:18.719412 getstream-0.3.0/getstream/chat/models/user_updated_event.py
--rw-r--r--   0        0        0     1183 2023-10-25 08:58:18.719550 getstream-0.3.0/getstream/chat/models/user_watching_start_event.py
--rw-r--r--   0        0        0     1100 2023-10-25 08:58:18.719743 getstream-0.3.0/getstream/chat/models/user_watching_stop_event.py
--rw-r--r--   0        0        0      479 2023-10-25 08:58:18.720170 getstream-0.3.0/getstream/chat/models/users_response.py
--rw-r--r--   0        0        0      768 2023-10-26 15:09:14.798312 getstream-0.3.0/getstream/chat/models/video_settings.py
--rw-r--r--   0        0        0      395 2023-10-26 15:09:02.291531 getstream-0.3.0/getstream/chat/models/ws_client_event.py
--rw-r--r--   0        0        0      549 2023-10-25 08:58:18.720526 getstream-0.3.0/getstream/chat/models/xiaomi_config_fields.py
--rw-r--r--   0        0        0      590 2023-10-25 08:58:18.720634 getstream-0.3.0/getstream/chat/models/xiaomi_config_request.py
--rw-r--r--   0        0        0       64 2023-10-10 11:41:14.142640 getstream-0.3.0/getstream/chat/sync/__init__.py
--rw-r--r--   0        0        0      212 2023-10-10 11:41:14.143094 getstream-0.3.0/getstream/chat/sync/chat.py
--rw-r--r--   0        0        0       52 2023-07-07 15:29:51.349357 getstream-0.3.0/getstream/cli/__init__.py
--rw-r--r--   0        0        0      997 2023-11-15 09:53:17.482753 getstream-0.3.0/getstream/cli/create_token.py
--rw-r--r--   0        0        0      925 2023-06-06 11:12:09.256010 getstream-0.3.0/getstream/config.py
--rw-r--r--   0        0        0       46 2024-03-06 06:15:35.459409 getstream-0.3.0/getstream/generic.py
--rw-r--r--   0        0        0        0 2024-03-06 06:11:28.258211 getstream-0.3.0/getstream/models/__init__.py
--rw-r--r--   0        0        0      323 2023-10-26 15:09:30.638378 getstream-0.3.0/getstream/models/accept_call_response.py
--rw-r--r--   0        0        0      816 2024-03-25 09:35:04.030840 getstream-0.3.0/getstream/models/api_error.py
--rw-r--r--   0        0        0      361 2024-03-06 06:15:35.459327 getstream-0.3.0/getstream/models/apns.py
--rw-r--r--   0        0        0      445 2024-03-06 06:15:35.459099 getstream-0.3.0/getstream/models/apns_request.py
--rw-r--r--   0        0        0      801 2024-03-25 09:35:04.031404 getstream-0.3.0/getstream/models/audio_settings.py
--rw-r--r--   0        0        0      999 2024-03-25 09:35:04.031696 getstream-0.3.0/getstream/models/audio_settings_request.py
--rw-r--r--   0        0        0      569 2024-03-25 09:35:04.032072 getstream-0.3.0/getstream/models/azure_request.py
--rw-r--r--   0        0        0      321 2024-03-06 06:15:35.470086 getstream-0.3.0/getstream/models/backstage_settings.py
--rw-r--r--   0        0        0      381 2024-03-06 06:15:35.473379 getstream-0.3.0/getstream/models/backstage_settings_request.py
--rw-r--r--   0        0        0      319 2024-03-06 06:15:35.547330 getstream-0.3.0/getstream/models/block_user_request.py
--rw-r--r--   0        0        0      322 2024-03-06 06:15:35.478084 getstream-0.3.0/getstream/models/block_user_response.py
--rw-r--r--   0        0        0      989 2023-10-26 15:13:34.099436 getstream-0.3.0/getstream/models/blocked_user_event.py
--rw-r--r--   0        0        0      559 2024-03-06 06:15:35.576934 getstream-0.3.0/getstream/models/broadcast_settings_request.py
--rw-r--r--   0        0        0      473 2024-03-06 06:15:35.491305 getstream-0.3.0/getstream/models/broadcast_settings_response.py
--rw-r--r--   0        0        0      958 2023-10-26 15:13:34.100711 getstream-0.3.0/getstream/models/call_accepted_event.py
--rw-r--r--   0        0        0      999 2023-10-26 15:13:34.101924 getstream-0.3.0/getstream/models/call_created_event.py
--rw-r--r--   0        0        0     1021 2023-10-26 15:13:34.102478 getstream-0.3.0/getstream/models/call_ended_event.py
--rw-r--r--   0        0        0      725 2023-10-26 15:13:34.102877 getstream-0.3.0/getstream/models/call_hls_broadcasting_failed_event.py
--rw-r--r--   0        0        0      808 2023-10-26 15:09:30.784351 getstream-0.3.0/getstream/models/call_hls_broadcasting_started_event.py
--rw-r--r--   0        0        0      726 2023-10-26 15:09:30.784639 getstream-0.3.0/getstream/models/call_hls_broadcasting_stopped_event.py
--rw-r--r--   0        0        0      379 2024-03-06 06:15:35.485235 getstream-0.3.0/getstream/models/call_ingress_response.py
--rw-r--r--   0        0        0      838 2023-10-26 15:09:30.831320 getstream-0.3.0/getstream/models/call_live_started_event.py
--rw-r--r--   0        0        0     1003 2023-10-26 15:13:34.103311 getstream-0.3.0/getstream/models/call_member_added_event.py
--rw-r--r--   0        0        0      934 2023-10-26 15:13:34.103924 getstream-0.3.0/getstream/models/call_member_removed_event.py
--rw-r--r--   0        0        0     1005 2023-10-26 15:13:34.104386 getstream-0.3.0/getstream/models/call_member_updated_event.py
--rw-r--r--   0        0        0     1142 2023-10-26 15:13:34.104853 getstream-0.3.0/getstream/models/call_member_updated_permission_event.py
--rw-r--r--   0        0        0     1197 2023-10-26 15:13:34.107283 getstream-0.3.0/getstream/models/call_notification_event.py
--rw-r--r--   0        0        0      853 2024-03-25 09:35:04.032399 getstream-0.3.0/getstream/models/call_participant_response.py
--rw-r--r--   0        0        0      855 2023-10-26 15:13:34.108923 getstream-0.3.0/getstream/models/call_reaction_event.py
--rw-r--r--   0        0        0      938 2024-03-06 06:15:35.512927 getstream-0.3.0/getstream/models/call_recording.py
--rw-r--r--   0        0        0      719 2023-10-26 15:09:30.869125 getstream-0.3.0/getstream/models/call_recording_failed_event.py
--rw-r--r--   0        0        0      864 2023-10-26 15:09:30.866274 getstream-0.3.0/getstream/models/call_recording_ready_event.py
--rw-r--r--   0        0        0      720 2023-10-26 15:09:30.865388 getstream-0.3.0/getstream/models/call_recording_started_event.py
--rw-r--r--   0        0        0      720 2023-10-26 15:09:30.876122 getstream-0.3.0/getstream/models/call_recording_stopped_event.py
--rw-r--r--   0        0        0      958 2023-10-26 15:13:34.110607 getstream-0.3.0/getstream/models/call_rejected_event.py
--rw-r--r--   0        0        0     1514 2024-03-25 09:35:04.032855 getstream-0.3.0/getstream/models/call_request.py
--rw-r--r--   0        0        0     3093 2024-03-25 09:35:04.033241 getstream-0.3.0/getstream/models/call_response.py
--rw-r--r--   0        0        0     1189 2023-10-26 15:13:34.112748 getstream-0.3.0/getstream/models/call_ring_event.py
--rw-r--r--   0        0        0      909 2023-10-26 15:13:34.113417 getstream-0.3.0/getstream/models/call_session_ended_event.py
--rw-r--r--   0        0        0      983 2023-10-26 15:13:34.114186 getstream-0.3.0/getstream/models/call_session_participant_joined_event.py
--rw-r--r--   0        0        0      981 2023-10-26 15:13:34.115220 getstream-0.3.0/getstream/models/call_session_participant_left_event.py
--rw-r--r--   0        0        0     2140 2024-03-25 09:35:04.033663 getstream-0.3.0/getstream/models/call_session_response.py
--rw-r--r--   0        0        0      911 2023-10-26 15:13:34.117557 getstream-0.3.0/getstream/models/call_session_started_event.py
--rw-r--r--   0        0        0     2343 2024-03-25 09:35:04.034001 getstream-0.3.0/getstream/models/call_settings_request.py
--rw-r--r--   0        0        0     1956 2024-03-25 09:35:04.034387 getstream-0.3.0/getstream/models/call_settings_response.py
--rw-r--r--   0        0        0      850 2024-03-06 06:15:35.563247 getstream-0.3.0/getstream/models/call_state_response_fields.py
--rw-r--r--   0        0        0      942 2024-03-25 09:35:04.034642 getstream-0.3.0/getstream/models/call_transcription.py
--rw-r--r--   0        0        0     1471 2024-03-25 09:35:04.034949 getstream-0.3.0/getstream/models/call_type_response.py
--rw-r--r--   0        0        0      985 2023-10-26 15:09:31.065346 getstream-0.3.0/getstream/models/call_updated_event.py
--rw-r--r--   0        0        0      890 2023-10-26 15:13:34.119184 getstream-0.3.0/getstream/models/call_user_muted.py
--rw-r--r--   0        0        0      333 2024-03-25 09:35:04.035176 getstream-0.3.0/getstream/models/check_external_storage_response.py
--rw-r--r--   0        0        0      706 2024-03-25 09:35:04.035618 getstream-0.3.0/getstream/models/connect_user_details_request.py
--rw-r--r--   0        0        0      848 2023-10-26 15:13:34.120348 getstream-0.3.0/getstream/models/connected_event.py
--rw-r--r--   0        0        0      838 2023-11-15 09:53:17.483717 getstream-0.3.0/getstream/models/connection_error_event.py
--rw-r--r--   0        0        0     1028 2024-03-25 09:35:04.035867 getstream-0.3.0/getstream/models/create_call_type_request.py
--rw-r--r--   0        0        0     1543 2024-03-25 09:35:04.036317 getstream-0.3.0/getstream/models/create_call_type_response.py
--rw-r--r--   0        0        0      958 2024-03-25 09:35:04.036740 getstream-0.3.0/getstream/models/create_device_request.py
--rw-r--r--   0        0        0     1021 2024-03-25 09:35:04.037055 getstream-0.3.0/getstream/models/create_external_storage_request.py
--rw-r--r--   0        0        0      334 2024-03-25 09:35:04.037251 getstream-0.3.0/getstream/models/create_external_storage_response.py
--rw-r--r--   0        0        0      378 2024-03-06 06:15:35.674062 getstream-0.3.0/getstream/models/create_guest_request.py
--rw-r--r--   0        0        0      522 2024-03-06 06:21:17.287873 getstream-0.3.0/getstream/models/create_guest_response.py
--rw-r--r--   0        0        0      593 2023-10-26 15:13:34.122234 getstream-0.3.0/getstream/models/credentials.py
--rw-r--r--   0        0        0      934 2023-10-26 15:13:34.122492 getstream-0.3.0/getstream/models/custom_video_event.py
--rw-r--r--   0        0        0      334 2024-03-25 09:35:04.037550 getstream-0.3.0/getstream/models/delete_external_storage_response.py
--rw-r--r--   0        0        0     1165 2024-03-25 09:35:04.037857 getstream-0.3.0/getstream/models/device.py
--rw-r--r--   0        0        0      967 2024-03-25 09:35:04.038282 getstream-0.3.0/getstream/models/edge_response.py
--rw-r--r--   0        0        0      330 2024-03-06 06:15:35.692633 getstream-0.3.0/getstream/models/egress_hls_response.py
--rw-r--r--   0        0        0      688 2024-03-25 09:35:04.038637 getstream-0.3.0/getstream/models/egress_response.py
--rw-r--r--   0        0        0      441 2024-03-06 06:15:35.696336 getstream-0.3.0/getstream/models/egress_rtmp_response.py
--rw-r--r--   0        0        0      320 2024-03-06 06:15:35.698360 getstream-0.3.0/getstream/models/end_call_response.py
--rw-r--r--   0        0        0      428 2024-03-06 06:15:35.703743 getstream-0.3.0/getstream/models/event_notification_settings.py
--rw-r--r--   0        0        0      547 2024-03-06 06:15:35.715932 getstream-0.3.0/getstream/models/event_notification_settings_request.py
--rw-r--r--   0        0        0      498 2024-03-25 09:35:04.038912 getstream-0.3.0/getstream/models/external_storage_response.py
--rw-r--r--   0        0        0      346 2024-03-06 06:15:35.715939 getstream-0.3.0/getstream/models/geofence_settings.py
--rw-r--r--   0        0        0      401 2024-03-06 06:15:35.722197 getstream-0.3.0/getstream/models/geofence_settings_request.py
--rw-r--r--   0        0        0      908 2024-03-25 09:35:04.039228 getstream-0.3.0/getstream/models/get_call_response.py
--rw-r--r--   0        0        0     1540 2024-03-25 09:35:04.039537 getstream-0.3.0/getstream/models/get_call_type_response.py
--rw-r--r--   0        0        0      477 2024-03-25 09:35:04.039759 getstream-0.3.0/getstream/models/get_edges_response.py
--rw-r--r--   0        0        0      732 2024-03-25 09:35:04.040027 getstream-0.3.0/getstream/models/get_or_create_call_request.py
--rw-r--r--   0        0        0      981 2024-03-25 09:35:04.040347 getstream-0.3.0/getstream/models/get_or_create_call_response.py
--rw-r--r--   0        0        0      906 2024-03-25 09:35:04.040630 getstream-0.3.0/getstream/models/go_live_request.py
--rw-r--r--   0        0        0      443 2024-03-06 06:15:35.745863 getstream-0.3.0/getstream/models/go_live_response.py
--rw-r--r--   0        0        0      721 2023-10-26 15:09:31.234394 getstream-0.3.0/getstream/models/health_check_event.py
--rw-r--r--   0        0        0      785 2024-03-25 09:35:04.040934 getstream-0.3.0/getstream/models/hls_settings_request.py
--rw-r--r--   0        0        0      630 2024-03-25 09:35:04.041294 getstream-0.3.0/getstream/models/hls_settings_response.py
--rw-r--r--   0        0        0      469 2023-10-26 15:13:34.127380 getstream-0.3.0/getstream/models/ice_server.py
--rw-r--r--   0        0        0      994 2023-10-26 15:13:34.128243 getstream-0.3.0/getstream/models/join_call_request.py
--rw-r--r--   0        0        0     1107 2023-10-26 15:13:34.128472 getstream-0.3.0/getstream/models/join_call_response.py
--rw-r--r--   0        0        0      609 2024-03-25 09:35:04.041673 getstream-0.3.0/getstream/models/layout_settings.py
--rw-r--r--   0        0        0      692 2024-03-25 09:35:04.042015 getstream-0.3.0/getstream/models/layout_settings_request.py
--rw-r--r--   0        0        0      523 2024-03-06 06:15:35.801110 getstream-0.3.0/getstream/models/list_call_type_response.py
--rw-r--r--   0        0        0      465 2024-03-06 06:15:35.783893 getstream-0.3.0/getstream/models/list_devices_response.py
--rw-r--r--   0        0        0      565 2024-03-25 09:35:04.042234 getstream-0.3.0/getstream/models/list_external_storage_response.py
--rw-r--r--   0        0        0      496 2024-03-06 06:15:35.801125 getstream-0.3.0/getstream/models/list_recordings_response.py
--rw-r--r--   0        0        0      534 2024-03-25 09:35:04.042523 getstream-0.3.0/getstream/models/list_transcriptions_response.py
--rw-r--r--   0        0        0      516 2024-03-25 09:35:04.042857 getstream-0.3.0/getstream/models/member_request.py
--rw-r--r--   0        0        0     1479 2024-03-25 09:35:04.043072 getstream-0.3.0/getstream/models/member_response.py
--rw-r--r--   0        0        0      921 2024-03-25 09:35:04.043383 getstream-0.3.0/getstream/models/mute_users_request.py
--rw-r--r--   0        0        0      322 2024-03-06 06:15:35.818187 getstream-0.3.0/getstream/models/mute_users_response.py
--rw-r--r--   0        0        0      868 2024-03-25 09:35:04.043687 getstream-0.3.0/getstream/models/notification_settings.py
--rw-r--r--   0        0        0     1075 2024-03-06 06:15:35.899753 getstream-0.3.0/getstream/models/notification_settings_request.py
--rw-r--r--   0        0        0     1386 2024-03-06 06:18:16.737051 getstream-0.3.0/getstream/models/own_capability.py
--rw-r--r--   0        0        0     1694 2023-10-26 15:13:34.133032 getstream-0.3.0/getstream/models/own_user_response.py
--rw-r--r--   0        0        0      942 2023-10-26 15:13:34.133637 getstream-0.3.0/getstream/models/permission_request_event.py
--rw-r--r--   0        0        0      383 2024-03-06 06:15:35.844488 getstream-0.3.0/getstream/models/pin_request.py
--rw-r--r--   0        0        0      316 2024-03-06 06:15:35.844616 getstream-0.3.0/getstream/models/pin_response.py
--rw-r--r--   0        0        0      929 2024-03-25 09:35:04.043997 getstream-0.3.0/getstream/models/query_calls_request.py
--rw-r--r--   0        0        0      688 2024-03-06 06:15:35.899481 getstream-0.3.0/getstream/models/query_calls_response.py
--rw-r--r--   0        0        0      958 2024-03-25 09:35:04.044349 getstream-0.3.0/getstream/models/query_members_request.py
--rw-r--r--   0        0        0      665 2024-03-06 06:18:16.738466 getstream-0.3.0/getstream/models/query_members_response.py
--rw-r--r--   0        0        0      693 2023-10-26 15:09:31.379785 getstream-0.3.0/getstream/models/reaction_response.py
--rw-r--r--   0        0        0      737 2024-03-06 06:15:35.928883 getstream-0.3.0/getstream/models/record_settings_request.py
--rw-r--r--   0        0        0      588 2024-03-25 09:35:04.044696 getstream-0.3.0/getstream/models/record_settings_response.py
--rw-r--r--   0        0        0      323 2023-10-26 15:09:31.363208 getstream-0.3.0/getstream/models/reject_call_response.py
--rw-r--r--   0        0        0      366 2023-10-26 15:09:31.368213 getstream-0.3.0/getstream/models/request_permission_request.py
--rw-r--r--   0        0        0      330 2023-10-26 15:09:31.372119 getstream-0.3.0/getstream/models/request_permission_response.py
--rw-r--r--   0        0        0      313 2024-03-06 06:15:35.923519 getstream-0.3.0/getstream/models/response.py
--rw-r--r--   0        0        0      471 2024-03-25 09:35:04.045060 getstream-0.3.0/getstream/models/ring_settings.py
--rw-r--r--   0        0        0      555 2024-03-06 06:15:35.941172 getstream-0.3.0/getstream/models/ring_settings_request.py
--rw-r--r--   0        0        0      314 2024-03-06 06:15:35.942057 getstream-0.3.0/getstream/models/rtmp_ingress.py
--rw-r--r--   0        0        0      559 2024-03-25 09:35:04.045304 getstream-0.3.0/getstream/models/s_3_request.py
--rw-r--r--   0        0        0      434 2024-03-25 09:35:04.045936 getstream-0.3.0/getstream/models/screensharing_settings.py
--rw-r--r--   0        0        0      518 2024-03-06 06:15:35.991696 getstream-0.3.0/getstream/models/screensharing_settings_request.py
--rw-r--r--   0        0        0      373 2024-03-25 09:35:04.046541 getstream-0.3.0/getstream/models/send_event_request.py
--rw-r--r--   0        0        0      322 2024-03-06 06:15:36.002956 getstream-0.3.0/getstream/models/send_event_response.py
--rw-r--r--   0        0        0      573 2023-10-26 15:13:34.138347 getstream-0.3.0/getstream/models/send_reaction_request.py
--rw-r--r--   0        0        0      469 2023-10-26 15:09:31.397508 getstream-0.3.0/getstream/models/send_reaction_response.py
--rw-r--r--   0        0        0      446 2023-10-26 15:13:34.141505 getstream-0.3.0/getstream/models/sfu_response.py
--rw-r--r--   0        0        0      228 2024-03-06 06:18:16.739513 getstream-0.3.0/getstream/models/sort_param_request.py
--rw-r--r--   0        0        0      407 2024-03-06 06:15:36.024035 getstream-0.3.0/getstream/models/start_hls_broadcasting_response.py
--rw-r--r--   0        0        0      429 2024-03-25 09:35:04.046791 getstream-0.3.0/getstream/models/start_recording_request.py
--rw-r--r--   0        0        0      327 2024-03-06 06:15:36.024502 getstream-0.3.0/getstream/models/start_recording_response.py
--rw-r--r--   0        0        0      441 2024-03-25 09:35:04.047037 getstream-0.3.0/getstream/models/start_transcription_request.py
--rw-r--r--   0        0        0      331 2024-03-06 06:15:36.108076 getstream-0.3.0/getstream/models/start_transcription_response.py
--rw-r--r--   0        0        0      332 2024-03-06 06:15:36.036673 getstream-0.3.0/getstream/models/stop_hls_broadcasting_response.py
--rw-r--r--   0        0        0      445 2024-03-06 06:15:36.042631 getstream-0.3.0/getstream/models/stop_live_response.py
--rw-r--r--   0        0        0      326 2024-03-06 06:15:36.037038 getstream-0.3.0/getstream/models/stop_recording_response.py
--rw-r--r--   0        0        0      330 2024-03-06 06:15:36.036638 getstream-0.3.0/getstream/models/stop_transcription_response.py
--rw-r--r--   0        0        0      441 2024-03-25 09:35:04.047453 getstream-0.3.0/getstream/models/target_resolution.py
--rw-r--r--   0        0        0      549 2024-03-06 06:18:07.364495 getstream-0.3.0/getstream/models/target_resolution_request.py
--rw-r--r--   0        0        0      324 2024-03-06 06:15:36.046316 getstream-0.3.0/getstream/models/thumbnail_response.py
--rw-r--r--   0        0        0      322 2024-03-06 06:15:36.045681 getstream-0.3.0/getstream/models/thumbnails_settings.py
--rw-r--r--   0        0        0      382 2024-03-06 06:15:36.053491 getstream-0.3.0/getstream/models/thumbnails_settings_request.py
--rw-r--r--   0        0        0      406 2024-03-06 06:15:36.057901 getstream-0.3.0/getstream/models/transcription_settings.py
--rw-r--r--   0        0        0      504 2024-03-06 06:15:36.115718 getstream-0.3.0/getstream/models/transcription_settings_request.py
--rw-r--r--   0        0        0      321 2024-03-06 06:15:36.062333 getstream-0.3.0/getstream/models/unblock_user_request.py
--rw-r--r--   0        0        0      324 2024-03-06 06:15:36.068417 getstream-0.3.0/getstream/models/unblock_user_response.py
--rw-r--r--   0        0        0      836 2023-10-26 15:13:34.142754 getstream-0.3.0/getstream/models/unblocked_user_event.py
--rw-r--r--   0        0        0      385 2024-03-06 06:18:07.365436 getstream-0.3.0/getstream/models/unpin_request.py
--rw-r--r--   0        0        0      318 2024-03-06 06:15:36.072233 getstream-0.3.0/getstream/models/unpin_response.py
--rw-r--r--   0        0        0      610 2024-03-06 06:15:36.086926 getstream-0.3.0/getstream/models/update_call_members_request.py
--rw-r--r--   0        0        0      496 2024-03-06 06:15:36.080013 getstream-0.3.0/getstream/models/update_call_members_response.py
--rw-r--r--   0        0        0      972 2024-03-25 09:35:04.047709 getstream-0.3.0/getstream/models/update_call_request.py
--rw-r--r--   0        0        0      911 2024-03-25 09:35:04.048031 getstream-0.3.0/getstream/models/update_call_response.py
--rw-r--r--   0        0        0      850 2024-03-25 09:35:04.048318 getstream-0.3.0/getstream/models/update_call_type_request.py
--rw-r--r--   0        0        0     1413 2024-03-25 09:35:04.048639 getstream-0.3.0/getstream/models/update_call_type_response.py
--rw-r--r--   0        0        0      963 2024-03-25 09:35:04.048822 getstream-0.3.0/getstream/models/update_external_storage_request.py
--rw-r--r--   0        0        0      570 2024-03-25 09:35:04.049052 getstream-0.3.0/getstream/models/update_external_storage_response.py
--rw-r--r--   0        0        0      624 2024-03-06 06:15:36.147605 getstream-0.3.0/getstream/models/update_user_permissions_request.py
--rw-r--r--   0        0        0      334 2024-03-06 06:15:36.123340 getstream-0.3.0/getstream/models/update_user_permissions_response.py
--rw-r--r--   0        0        0     1039 2023-10-26 15:13:34.143762 getstream-0.3.0/getstream/models/updated_call_permissions_event.py
--rw-r--r--   0        0        0      884 2024-03-25 09:35:04.049275 getstream-0.3.0/getstream/models/user_request.py
--rw-r--r--   0        0        0     1624 2024-03-25 09:35:04.049605 getstream-0.3.0/getstream/models/user_response.py
--rw-r--r--   0        0        0     5688 2023-10-26 15:09:31.765367 getstream-0.3.0/getstream/models/video_event.py
--rw-r--r--   0        0        0      763 2024-03-06 06:15:36.186449 getstream-0.3.0/getstream/models/video_settings.py
--rw-r--r--   0        0        0      968 2024-03-06 06:15:36.219247 getstream-0.3.0/getstream/models/video_settings_request.py
--rw-r--r--   0        0        0      514 2024-03-06 06:15:36.171604 getstream-0.3.0/getstream/models/ws_auth_message_request.py
--rw-r--r--   0        0        0      383 2023-10-26 15:09:31.677417 getstream-0.3.0/getstream/models/ws_call_event.py
--rw-r--r--   0        0        0      395 2023-10-26 15:09:31.678880 getstream-0.3.0/getstream/models/ws_client_event.py
--rw-r--r--   0        0        0     1168 2024-03-06 06:15:36.222459 getstream-0.3.0/getstream/rate_limit.py
--rw-r--r--   0        0        0     1209 2024-03-06 06:25:20.787577 getstream-0.3.0/getstream/stream_response.py
--rw-r--r--   0        0        0       41 2023-10-25 08:58:18.748254 getstream-0.3.0/getstream/sync/__init__.py
--rw-r--r--   0        0        0     4481 2024-03-06 06:18:07.369409 getstream-0.3.0/getstream/sync/base.py
--rw-r--r--   0        0        0     9113 2023-11-15 09:53:17.484346 getstream-0.3.0/getstream/sync/stream.py
--rw-r--r--   0        0        0     7403 2023-11-15 09:53:17.485082 getstream-0.3.0/getstream/users/sync/client.py
--rw-r--r--   0        0        0     1671 2023-10-25 08:58:18.749193 getstream-0.3.0/getstream/utils.py
--rw-r--r--   0        0        0       18 2024-03-25 09:35:04.049888 getstream-0.3.0/getstream/version.py
--rw-r--r--   0        0        0      141 2024-02-12 08:30:27.994264 getstream-0.3.0/getstream/video/__init__.py
--rw-r--r--   0        0        0       48 2023-07-07 15:29:51.351074 getstream-0.3.0/getstream/video/async_/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 09:15:27.009605 getstream-0.3.0/getstream/video/async_/call.py
--rw-r--r--   0        0        0      142 2023-05-05 11:43:39.447192 getstream-0.3.0/getstream/video/async_/client.py
--rw-r--r--   0        0        0      754 2023-11-15 09:53:17.485376 getstream-0.3.0/getstream/video/exceptions.py
--rw-r--r--   0        0        0       46 2023-10-25 08:58:18.749971 getstream-0.3.0/getstream/video/sync/__init__.py
--rw-r--r--   0        0        0    37798 2024-03-25 09:35:04.050336 getstream-0.3.0/getstream/video/sync/base_client.py
--rw-r--r--   0        0        0    30723 2024-03-25 09:35:04.050758 getstream-0.3.0/getstream/video/sync/client.py
--rw-r--r--   0        0        0      672 2024-03-25 09:35:04.051065 getstream-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 getstream-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    14205 2023-07-11 09:24:31.518666 getstream-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     3918 2023-11-15 09:53:17.481311 getstream-0.4.0/README.md
+-rw-r--r--   0        0        0       98 2024-03-06 06:15:35.459426 getstream-0.4.0/getstream/__init__.py
+-rw-r--r--   0        0        0       46 2023-07-07 15:26:52.041698 getstream-0.4.0/getstream/async_/__init__.py
+-rw-r--r--   0        0        0      965 2023-04-24 16:13:28.085563 getstream-0.4.0/getstream/async_/base.py
+-rw-r--r--   0        0        0      225 2023-05-05 11:48:07.700181 getstream-0.4.0/getstream/async_/stream.py
+-rw-r--r--   0        0        0     1422 2023-11-15 09:53:17.481818 getstream-0.4.0/getstream/base.py
+-rw-r--r--   0        0        0        0 2023-10-26 15:09:14.788653 getstream-0.4.0/getstream/chat/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-07 15:27:10.735770 getstream-0.4.0/getstream/chat/async_/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-05 11:47:33.873776 getstream-0.4.0/getstream/chat/async_/chat.py
+-rw-r--r--   0        0        0        0 2023-10-26 15:07:47.200051 getstream-0.4.0/getstream/chat/models/__init__.py
+-rw-r--r--   0        0        0      616 2023-10-25 08:58:18.671682 getstream-0.4.0/getstream/chat/models/action.py
+-rw-r--r--   0        0        0      695 2023-10-25 08:58:18.671917 getstream-0.4.0/getstream/chat/models/action_request.py
+-rw-r--r--   0        0        0      312 2023-10-25 08:58:18.672318 getstream-0.4.0/getstream/chat/models/agora_call.py
+-rw-r--r--   0        0        0      637 2023-10-25 08:58:18.672462 getstream-0.4.0/getstream/chat/models/any_event.py
+-rw-r--r--   0        0        0      816 2023-11-15 09:53:17.482317 getstream-0.4.0/getstream/chat/models/api_error.py
+-rw-r--r--   0        0        0     1204 2023-10-25 08:58:18.672762 getstream-0.4.0/getstream/chat/models/apn_config_fields.py
+-rw-r--r--   0        0        0     1307 2023-10-25 08:58:18.672908 getstream-0.4.0/getstream/chat/models/apn_config_request.py
+-rw-r--r--   0        0        0      361 2023-10-26 15:09:01.347212 getstream-0.4.0/getstream/chat/models/apns.py
+-rw-r--r--   0        0        0     4505 2023-10-25 08:58:18.673366 getstream-0.4.0/getstream/chat/models/app.py
+-rw-r--r--   0        0        0      494 2023-10-25 08:58:18.673531 getstream-0.4.0/getstream/chat/models/async_moderation_callback_config_request.py
+-rw-r--r--   0        0        0      669 2023-10-25 08:58:18.673678 getstream-0.4.0/getstream/chat/models/async_moderation_configuration_request.py
+-rw-r--r--   0        0        0     2556 2023-10-25 08:58:18.673821 getstream-0.4.0/getstream/chat/models/attachment.py
+-rw-r--r--   0        0        0     2643 2023-10-25 08:58:18.673987 getstream-0.4.0/getstream/chat/models/attachment_request.py
+-rw-r--r--   0        0        0      723 2023-10-26 15:09:14.790299 getstream-0.4.0/getstream/chat/models/audio_settings.py
+-rw-r--r--   0        0        0     1033 2023-10-25 08:58:18.674292 getstream-0.4.0/getstream/chat/models/automod_details.py
+-rw-r--r--   0        0        0      321 2023-10-26 15:09:01.378280 getstream-0.4.0/getstream/chat/models/backstage_settings.py
+-rw-r--r--   0        0        0     1366 2023-10-25 08:58:18.674779 getstream-0.4.0/getstream/chat/models/ban_request.py
+-rw-r--r--   0        0        0     1546 2023-10-25 08:58:18.675032 getstream-0.4.0/getstream/chat/models/ban_response.py
+-rw-r--r--   0        0        0     1094 2023-10-25 08:58:18.675225 getstream-0.4.0/getstream/chat/models/block_list.py
+-rw-r--r--   0        0        0      445 2023-10-25 08:58:18.675444 getstream-0.4.0/getstream/chat/models/broadcast_settings.py
+-rw-r--r--   0        0        0      744 2023-10-25 08:58:18.675872 getstream-0.4.0/getstream/chat/models/call.py
+-rw-r--r--   0        0        0     1970 2023-10-25 08:58:18.676013 getstream-0.4.0/getstream/chat/models/call_settings.py
+-rw-r--r--   0        0        0     1411 2023-10-25 08:58:18.676145 getstream-0.4.0/getstream/chat/models/call_type.py
+-rw-r--r--   0        0        0     3811 2023-10-25 08:58:18.676286 getstream-0.4.0/getstream/chat/models/campaign.py
+-rw-r--r--   0        0        0     1091 2023-10-25 08:58:18.676459 getstream-0.4.0/getstream/chat/models/campaign_data_request.py
+-rw-r--r--   0        0        0      546 2023-10-25 08:58:18.676607 getstream-0.4.0/getstream/chat/models/campaign_sort.py
+-rw-r--r--   0        0        0      379 2023-10-25 08:58:18.676754 getstream-0.4.0/getstream/chat/models/campaign_sort_field.py
+-rw-r--r--   0        0        0     1227 2023-10-25 08:58:18.676917 getstream-0.4.0/getstream/chat/models/campaign_updateable_fields_request.py
+-rw-r--r--   0        0        0     3190 2023-10-25 08:58:18.677066 getstream-0.4.0/getstream/chat/models/channel.py
+-rw-r--r--   0        0        0     2644 2023-10-25 08:58:18.677219 getstream-0.4.0/getstream/chat/models/channel_config.py
+-rw-r--r--   0        0        0     1485 2023-10-25 08:58:18.677374 getstream-0.4.0/getstream/chat/models/channel_config_request.py
+-rw-r--r--   0        0        0     2829 2023-10-25 08:58:18.677523 getstream-0.4.0/getstream/chat/models/channel_config_with_info.py
+-rw-r--r--   0        0        0     3600 2023-10-25 08:58:18.677671 getstream-0.4.0/getstream/chat/models/channel_config_with_info_request.py
+-rw-r--r--   0        0        0      648 2023-10-25 08:58:18.677821 getstream-0.4.0/getstream/chat/models/channel_created_event.py
+-rw-r--r--   0        0        0     1139 2023-10-25 08:58:18.677960 getstream-0.4.0/getstream/chat/models/channel_deleted_event.py
+-rw-r--r--   0        0        0     1231 2023-10-25 08:58:18.678092 getstream-0.4.0/getstream/chat/models/channel_export_request.py
+-rw-r--r--   0        0        0      847 2023-10-25 08:58:18.678246 getstream-0.4.0/getstream/chat/models/channel_frozen_event.py
+-rw-r--r--   0        0        0     1650 2023-10-25 08:58:18.678395 getstream-0.4.0/getstream/chat/models/channel_get_or_create_request.py
+-rw-r--r--   0        0        0     1279 2023-10-25 08:58:18.678539 getstream-0.4.0/getstream/chat/models/channel_hidden_event.py
+-rw-r--r--   0        0        0     1056 2023-10-25 08:58:18.678685 getstream-0.4.0/getstream/chat/models/channel_kicked_event.py
+-rw-r--r--   0        0        0     2798 2023-10-25 08:58:18.678856 getstream-0.4.0/getstream/chat/models/channel_member.py
+-rw-r--r--   0        0        0     3061 2023-10-25 08:58:18.679027 getstream-0.4.0/getstream/chat/models/channel_member_request.py
+-rw-r--r--   0        0        0      596 2023-10-25 08:58:18.679174 getstream-0.4.0/getstream/chat/models/channel_messages.py
+-rw-r--r--   0        0        0     1463 2023-10-25 08:58:18.679329 getstream-0.4.0/getstream/chat/models/channel_mute.py
+-rw-r--r--   0        0        0     1648 2023-10-25 08:58:18.679486 getstream-0.4.0/getstream/chat/models/channel_mute_request.py
+-rw-r--r--   0        0        0      646 2023-10-25 08:58:18.679633 getstream-0.4.0/getstream/chat/models/channel_muted_event.py
+-rw-r--r--   0        0        0     1929 2023-10-25 08:58:18.679810 getstream-0.4.0/getstream/chat/models/channel_request.py
+-rw-r--r--   0        0        0     4341 2023-10-25 08:58:18.680190 getstream-0.4.0/getstream/chat/models/channel_response.py
+-rw-r--r--   0        0        0     4563 2023-10-25 08:58:18.680421 getstream-0.4.0/getstream/chat/models/channel_response_request.py
+-rw-r--r--   0        0        0     2153 2023-10-25 08:58:18.680555 getstream-0.4.0/getstream/chat/models/channel_state_response.py
+-rw-r--r--   0        0        0     2093 2023-10-25 08:58:18.680706 getstream-0.4.0/getstream/chat/models/channel_state_response_fields.py
+-rw-r--r--   0        0        0      514 2023-10-25 08:58:18.680850 getstream-0.4.0/getstream/chat/models/channel_stop_watching_request.py
+-rw-r--r--   0        0        0     1059 2023-10-25 08:58:18.680997 getstream-0.4.0/getstream/chat/models/channel_truncated_event.py
+-rw-r--r--   0        0        0     2942 2023-10-25 08:58:18.681136 getstream-0.4.0/getstream/chat/models/channel_type_config.py
+-rw-r--r--   0        0        0      849 2023-10-25 08:58:18.681275 getstream-0.4.0/getstream/chat/models/channel_un_frozen_event.py
+-rw-r--r--   0        0        0      648 2023-10-25 08:58:18.681421 getstream-0.4.0/getstream/chat/models/channel_unmuted_event.py
+-rw-r--r--   0        0        0     1441 2023-10-25 08:58:18.681570 getstream-0.4.0/getstream/chat/models/channel_updated_event.py
+-rw-r--r--   0        0        0     1022 2023-10-25 08:58:18.681737 getstream-0.4.0/getstream/chat/models/channel_visible_event.py
+-rw-r--r--   0        0        0      555 2023-10-25 08:58:18.681905 getstream-0.4.0/getstream/chat/models/channels_response.py
+-rw-r--r--   0        0        0     8795 2023-10-25 08:58:18.682134 getstream-0.4.0/getstream/chat/models/chat_event.py
+-rw-r--r--   0        0        0     1389 2023-10-25 08:58:18.682297 getstream-0.4.0/getstream/chat/models/check_push_request.py
+-rw-r--r--   0        0        0     1204 2023-10-25 08:58:18.682451 getstream-0.4.0/getstream/chat/models/check_push_response.py
+-rw-r--r--   0        0        0      567 2023-10-25 08:58:18.682667 getstream-0.4.0/getstream/chat/models/check_sqs_request.py
+-rw-r--r--   0        0        0      612 2023-10-25 08:58:18.682867 getstream-0.4.0/getstream/chat/models/check_sqs_response.py
+-rw-r--r--   0        0        0     1206 2023-10-25 08:58:18.683030 getstream-0.4.0/getstream/chat/models/command.py
+-rw-r--r--   0        0        0      636 2023-10-25 08:58:18.683193 getstream-0.4.0/getstream/chat/models/command_request.py
+-rw-r--r--   0        0        0      649 2023-10-25 08:58:18.683360 getstream-0.4.0/getstream/chat/models/config.py
+-rw-r--r--   0        0        0      656 2023-10-25 08:58:18.683500 getstream-0.4.0/getstream/chat/models/config_request.py
+-rw-r--r--   0        0        0      590 2023-10-25 08:58:18.683644 getstream-0.4.0/getstream/chat/models/connect_request.py
+-rw-r--r--   0        0        0      410 2023-10-25 08:58:18.683791 getstream-0.4.0/getstream/chat/models/create_block_list_request.py
+-rw-r--r--   0        0        0      789 2023-10-25 08:58:18.683936 getstream-0.4.0/getstream/chat/models/create_call_request.py
+-rw-r--r--   0        0        0      757 2023-10-25 08:58:18.684063 getstream-0.4.0/getstream/chat/models/create_call_response.py
+-rw-r--r--   0        0        0      419 2023-10-25 08:58:18.684188 getstream-0.4.0/getstream/chat/models/create_campaign_request.py
+-rw-r--r--   0        0        0      517 2023-10-25 08:58:18.684315 getstream-0.4.0/getstream/chat/models/create_campaign_response.py
+-rw-r--r--   0        0        0     2595 2023-10-25 08:58:18.684455 getstream-0.4.0/getstream/chat/models/create_channel_type_request.py
+-rw-r--r--   0        0        0     2962 2023-10-25 08:58:18.684590 getstream-0.4.0/getstream/chat/models/create_channel_type_response.py
+-rw-r--r--   0        0        0      580 2023-10-25 08:58:18.684724 getstream-0.4.0/getstream/chat/models/create_command_request.py
+-rw-r--r--   0        0        0      511 2023-10-25 08:58:18.684856 getstream-0.4.0/getstream/chat/models/create_command_response.py
+-rw-r--r--   0        0        0      963 2023-10-26 15:09:14.791262 getstream-0.4.0/getstream/chat/models/create_device_request.py
+-rw-r--r--   0        0        0      427 2023-10-25 08:58:18.685111 getstream-0.4.0/getstream/chat/models/create_import_request.py
+-rw-r--r--   0        0        0      528 2023-10-25 08:58:18.685316 getstream-0.4.0/getstream/chat/models/create_import_response.py
+-rw-r--r--   0        0        0      394 2023-10-25 08:58:18.685512 getstream-0.4.0/getstream/chat/models/create_import_url_request.py
+-rw-r--r--   0        0        0      456 2023-10-25 08:58:18.685645 getstream-0.4.0/getstream/chat/models/create_import_url_response.py
+-rw-r--r--   0        0        0      314 2023-10-25 08:58:18.685764 getstream-0.4.0/getstream/chat/models/create_role_request.py
+-rw-r--r--   0        0        0      427 2023-10-25 08:58:18.685898 getstream-0.4.0/getstream/chat/models/create_role_response.py
+-rw-r--r--   0        0        0      413 2023-10-25 08:58:18.686044 getstream-0.4.0/getstream/chat/models/create_segment_request.py
+-rw-r--r--   0        0        0      511 2023-10-25 08:58:18.686190 getstream-0.4.0/getstream/chat/models/create_segment_response.py
+-rw-r--r--   0        0        0      598 2023-10-25 08:58:18.686317 getstream-0.4.0/getstream/chat/models/deactivate_user_request.py
+-rw-r--r--   0        0        0      502 2023-10-25 08:58:18.686447 getstream-0.4.0/getstream/chat/models/deactivate_user_response.py
+-rw-r--r--   0        0        0      613 2023-10-25 08:58:18.686573 getstream-0.4.0/getstream/chat/models/deactivate_users_request.py
+-rw-r--r--   0        0        0      392 2023-10-25 08:58:18.686697 getstream-0.4.0/getstream/chat/models/deactivate_users_response.py
+-rw-r--r--   0        0        0      327 2023-10-25 08:58:18.686817 getstream-0.4.0/getstream/chat/models/delete_campaign_response.py
+-rw-r--r--   0        0        0      536 2023-10-25 08:58:18.686948 getstream-0.4.0/getstream/chat/models/delete_channel_response.py
+-rw-r--r--   0        0        0      494 2023-10-25 08:58:18.687075 getstream-0.4.0/getstream/chat/models/delete_channels_request.py
+-rw-r--r--   0        0        0      656 2023-10-25 08:58:18.687218 getstream-0.4.0/getstream/chat/models/delete_channels_response.py
+-rw-r--r--   0        0        0      434 2023-10-25 08:58:18.687362 getstream-0.4.0/getstream/chat/models/delete_channels_result.py
+-rw-r--r--   0        0        0      384 2023-10-25 08:58:18.687488 getstream-0.4.0/getstream/chat/models/delete_command_response.py
+-rw-r--r--   0        0        0      326 2023-10-25 08:58:18.687607 getstream-0.4.0/getstream/chat/models/delete_segment_response.py
+-rw-r--r--   0        0        0      562 2023-10-25 08:58:18.687743 getstream-0.4.0/getstream/chat/models/delete_user_response.py
+-rw-r--r--   0        0        0      792 2023-10-25 08:58:18.687867 getstream-0.4.0/getstream/chat/models/delete_users_request.py
+-rw-r--r--   0        0        0      388 2023-10-25 08:58:18.687992 getstream-0.4.0/getstream/chat/models/delete_users_response.py
+-rw-r--r--   0        0        0     1229 2023-10-26 15:09:14.792110 getstream-0.4.0/getstream/chat/models/device.py
+-rw-r--r--   0        0        0      472 2023-10-25 08:58:18.688246 getstream-0.4.0/getstream/chat/models/device_error_info.py
+-rw-r--r--   0        0        0      617 2023-10-25 08:58:18.688369 getstream-0.4.0/getstream/chat/models/device_fields.py
+-rw-r--r--   0        0        0     1320 2023-10-25 08:58:18.688499 getstream-0.4.0/getstream/chat/models/device_request.py
+-rw-r--r--   0        0        0      608 2023-10-25 08:58:18.688618 getstream-0.4.0/getstream/chat/models/error_result.py
+-rw-r--r--   0        0        0     2952 2023-10-25 08:58:18.688732 getstream-0.4.0/getstream/chat/models/event.py
+-rw-r--r--   0        0        0      433 2023-10-26 15:09:14.792601 getstream-0.4.0/getstream/chat/models/event_notification_settings.py
+-rw-r--r--   0        0        0     3198 2023-10-25 08:58:18.689140 getstream-0.4.0/getstream/chat/models/event_request.py
+-rw-r--r--   0        0        0      479 2023-10-25 08:58:18.689384 getstream-0.4.0/getstream/chat/models/event_response.py
+-rw-r--r--   0        0        0      983 2023-10-25 08:58:18.689515 getstream-0.4.0/getstream/chat/models/export_channels_request.py
+-rw-r--r--   0        0        0      391 2023-10-25 08:58:18.689637 getstream-0.4.0/getstream/chat/models/export_channels_response.py
+-rw-r--r--   0        0        0      543 2023-10-25 08:58:18.689763 getstream-0.4.0/getstream/chat/models/export_channels_result.py
+-rw-r--r--   0        0        0      837 2023-10-25 08:58:18.689897 getstream-0.4.0/getstream/chat/models/export_user_response.py
+-rw-r--r--   0        0        0      354 2023-10-25 08:58:18.690027 getstream-0.4.0/getstream/chat/models/export_users_request.py
+-rw-r--r--   0        0        0      388 2023-10-25 08:58:18.690147 getstream-0.4.0/getstream/chat/models/export_users_response.py
+-rw-r--r--   0        0        0      425 2023-10-25 08:58:18.690266 getstream-0.4.0/getstream/chat/models/field.py
+-rw-r--r--   0        0        0      533 2023-10-25 08:58:18.690388 getstream-0.4.0/getstream/chat/models/field_request.py
+-rw-r--r--   0        0        0      323 2023-10-25 08:58:18.690516 getstream-0.4.0/getstream/chat/models/file_delete_response.py
+-rw-r--r--   0        0        0      724 2023-10-25 08:58:18.690640 getstream-0.4.0/getstream/chat/models/file_upload_config.py
+-rw-r--r--   0        0        0      837 2023-10-25 08:58:18.690762 getstream-0.4.0/getstream/chat/models/file_upload_config_request.py
+-rw-r--r--   0        0        0      550 2023-10-25 08:58:18.690887 getstream-0.4.0/getstream/chat/models/file_upload_request.py
+-rw-r--r--   0        0        0      540 2023-10-25 08:58:18.691010 getstream-0.4.0/getstream/chat/models/file_upload_response.py
+-rw-r--r--   0        0        0      837 2023-10-25 08:58:18.691144 getstream-0.4.0/getstream/chat/models/firebase_config_fields.py
+-rw-r--r--   0        0        0      978 2023-10-25 08:58:18.691273 getstream-0.4.0/getstream/chat/models/firebase_config_request.py
+-rw-r--r--   0        0        0     2544 2023-10-25 08:58:18.691396 getstream-0.4.0/getstream/chat/models/flag.py
+-rw-r--r--   0        0        0      457 2023-10-25 08:58:18.691532 getstream-0.4.0/getstream/chat/models/flag_details.py
+-rw-r--r--   0        0        0      793 2023-10-25 08:58:18.691648 getstream-0.4.0/getstream/chat/models/flag_feedback.py
+-rw-r--r--   0        0        0      733 2023-10-25 08:58:18.691783 getstream-0.4.0/getstream/chat/models/flag_message_details.py
+-rw-r--r--   0        0        0      787 2023-10-25 08:58:18.691915 getstream-0.4.0/getstream/chat/models/flag_request.py
+-rw-r--r--   0        0        0      473 2023-10-25 08:58:18.692033 getstream-0.4.0/getstream/chat/models/flag_response.py
+-rw-r--r--   0        0        0      346 2023-10-26 15:09:01.808957 getstream-0.4.0/getstream/chat/models/geofence_settings.py
+-rw-r--r--   0        0        0      426 2023-10-25 08:58:18.692373 getstream-0.4.0/getstream/chat/models/get_application_response.py
+-rw-r--r--   0        0        0      521 2023-10-25 08:58:18.692498 getstream-0.4.0/getstream/chat/models/get_block_list_response.py
+-rw-r--r--   0        0        0      557 2023-10-25 08:58:18.692620 getstream-0.4.0/getstream/chat/models/get_call_token_request.py
+-rw-r--r--   0        0        0      632 2023-10-25 08:58:18.692737 getstream-0.4.0/getstream/chat/models/get_call_token_response.py
+-rw-r--r--   0        0        0     1283 2023-10-25 08:58:18.692858 getstream-0.4.0/getstream/chat/models/get_command_response.py
+-rw-r--r--   0        0        0      466 2023-10-25 08:58:18.692986 getstream-0.4.0/getstream/chat/models/get_custom_permission_response.py
+-rw-r--r--   0        0        0     1418 2023-10-25 08:58:18.693116 getstream-0.4.0/getstream/chat/models/get_export_channels_status_response.py
+-rw-r--r--   0        0        0      525 2023-10-25 08:58:18.693241 getstream-0.4.0/getstream/chat/models/get_import_response.py
+-rw-r--r--   0        0        0      479 2023-10-25 08:58:18.693363 getstream-0.4.0/getstream/chat/models/get_many_messages_response.py
+-rw-r--r--   0        0        0     2625 2023-10-25 08:58:18.693490 getstream-0.4.0/getstream/chat/models/get_og_response.py
+-rw-r--r--   0        0        0      884 2023-10-25 08:58:18.693602 getstream-0.4.0/getstream/chat/models/get_rate_limits_response.py
+-rw-r--r--   0        0        0      481 2023-10-25 08:58:18.693729 getstream-0.4.0/getstream/chat/models/get_reactions_response.py
+-rw-r--r--   0        0        0      474 2023-10-25 08:58:18.693853 getstream-0.4.0/getstream/chat/models/get_replies_response.py
+-rw-r--r--   0        0        0     1327 2023-10-25 08:58:18.694034 getstream-0.4.0/getstream/chat/models/get_task_response.py
+-rw-r--r--   0        0        0      396 2023-10-25 08:58:18.694221 getstream-0.4.0/getstream/chat/models/guest_request.py
+-rw-r--r--   0        0        0      567 2023-10-25 08:58:18.694526 getstream-0.4.0/getstream/chat/models/guest_response.py
+-rw-r--r--   0        0        0      862 2023-10-26 15:09:14.793399 getstream-0.4.0/getstream/chat/models/health_check_event.py
+-rw-r--r--   0        0        0      671 2023-10-25 08:58:18.694754 getstream-0.4.0/getstream/chat/models/hide_channel_request.py
+-rw-r--r--   0        0        0      324 2023-10-25 08:58:18.694878 getstream-0.4.0/getstream/chat/models/hide_channel_response.py
+-rw-r--r--   0        0        0      489 2023-10-25 08:58:18.694991 getstream-0.4.0/getstream/chat/models/hls_settings.py
+-rw-r--r--   0        0        0      378 2023-10-25 08:58:18.695112 getstream-0.4.0/getstream/chat/models/hms_call.py
+-rw-r--r--   0        0        0      515 2023-10-25 08:58:18.695231 getstream-0.4.0/getstream/chat/models/huawei_config_fields.py
+-rw-r--r--   0        0        0      556 2023-10-25 08:58:18.695352 getstream-0.4.0/getstream/chat/models/huawei_config_request.py
+-rw-r--r--   0        0        0      546 2023-10-25 08:58:18.695493 getstream-0.4.0/getstream/chat/models/image_data.py
+-rw-r--r--   0        0        0      702 2023-10-25 08:58:18.695623 getstream-0.4.0/getstream/chat/models/image_data_request.py
+-rw-r--r--   0        0        0      490 2023-10-25 08:58:18.695743 getstream-0.4.0/getstream/chat/models/image_size.py
+-rw-r--r--   0        0        0      622 2023-10-25 08:58:18.695868 getstream-0.4.0/getstream/chat/models/image_size_request.py
+-rw-r--r--   0        0        0      758 2023-10-25 08:58:18.695996 getstream-0.4.0/getstream/chat/models/image_upload_request.py
+-rw-r--r--   0        0        0      726 2023-10-25 08:58:18.696122 getstream-0.4.0/getstream/chat/models/image_upload_response.py
+-rw-r--r--   0        0        0      975 2023-10-25 08:58:18.696251 getstream-0.4.0/getstream/chat/models/images.py
+-rw-r--r--   0        0        0     1284 2023-10-25 08:58:18.696370 getstream-0.4.0/getstream/chat/models/images_request.py
+-rw-r--r--   0        0        0     1408 2023-10-25 08:58:18.696494 getstream-0.4.0/getstream/chat/models/import_task.py
+-rw-r--r--   0        0        0      728 2023-10-25 08:58:18.696609 getstream-0.4.0/getstream/chat/models/import_task_history.py
+-rw-r--r--   0        0        0      461 2023-10-25 08:58:18.696729 getstream-0.4.0/getstream/chat/models/label.py
+-rw-r--r--   0        0        0      453 2023-10-25 08:58:18.696851 getstream-0.4.0/getstream/chat/models/label_thresholds.py
+-rw-r--r--   0        0        0      460 2023-10-25 08:58:18.696972 getstream-0.4.0/getstream/chat/models/label_thresholds_request.py
+-rw-r--r--   0        0        0      436 2023-10-25 08:58:18.697093 getstream-0.4.0/getstream/chat/models/limit_info.py
+-rw-r--r--   0        0        0      488 2023-10-25 08:58:18.697221 getstream-0.4.0/getstream/chat/models/list_block_list_response.py
+-rw-r--r--   0        0        0      541 2023-10-25 08:58:18.697339 getstream-0.4.0/getstream/chat/models/list_channel_types_response.py
+-rw-r--r--   0        0        0      476 2023-10-25 08:58:18.697456 getstream-0.4.0/getstream/chat/models/list_commands_response.py
+-rw-r--r--   0        0        0      470 2023-10-26 15:09:14.793996 getstream-0.4.0/getstream/chat/models/list_devices_response.py
+-rw-r--r--   0        0        0      493 2023-10-25 08:58:18.697700 getstream-0.4.0/getstream/chat/models/list_imports_response.py
+-rw-r--r--   0        0        0      494 2023-10-25 08:58:18.697827 getstream-0.4.0/getstream/chat/models/list_permissions_response.py
+-rw-r--r--   0        0        0      548 2023-10-25 08:58:18.697954 getstream-0.4.0/getstream/chat/models/list_push_providers_response.py
+-rw-r--r--   0        0        0      458 2023-10-25 08:58:18.698079 getstream-0.4.0/getstream/chat/models/list_roles_response.py
+-rw-r--r--   0        0        0      561 2023-10-25 08:58:18.698212 getstream-0.4.0/getstream/chat/models/mark_channels_read_request.py
+-rw-r--r--   0        0        0      661 2023-10-25 08:58:18.698378 getstream-0.4.0/getstream/chat/models/mark_read_request.py
+-rw-r--r--   0        0        0      531 2023-10-25 08:58:18.698502 getstream-0.4.0/getstream/chat/models/mark_read_response.py
+-rw-r--r--   0        0        0      625 2023-10-25 08:58:18.698632 getstream-0.4.0/getstream/chat/models/mark_unread_request.py
+-rw-r--r--   0        0        0     1274 2023-10-25 08:58:18.698763 getstream-0.4.0/getstream/chat/models/member_added_event.py
+-rw-r--r--   0        0        0     1194 2023-10-25 08:58:18.698939 getstream-0.4.0/getstream/chat/models/member_removed_event.py
+-rw-r--r--   0        0        0     1276 2023-10-25 08:58:18.699136 getstream-0.4.0/getstream/chat/models/member_updated_event.py
+-rw-r--r--   0        0        0      488 2023-10-25 08:58:18.699519 getstream-0.4.0/getstream/chat/models/members_response.py
+-rw-r--r--   0        0        0     4607 2023-10-25 08:58:18.699794 getstream-0.4.0/getstream/chat/models/message.py
+-rw-r--r--   0        0        0      721 2023-10-25 08:58:18.699924 getstream-0.4.0/getstream/chat/models/message_action_request.py
+-rw-r--r--   0        0        0     1478 2023-10-25 08:58:18.700051 getstream-0.4.0/getstream/chat/models/message_deleted_event.py
+-rw-r--r--   0        0        0     2668 2023-10-25 08:58:18.700180 getstream-0.4.0/getstream/chat/models/message_flag.py
+-rw-r--r--   0        0        0     1306 2023-10-25 08:58:18.700307 getstream-0.4.0/getstream/chat/models/message_flagged_event.py
+-rw-r--r--   0        0        0     1894 2023-10-25 08:58:18.700434 getstream-0.4.0/getstream/chat/models/message_moderation_result.py
+-rw-r--r--   0        0        0     1477 2023-10-25 08:58:18.700564 getstream-0.4.0/getstream/chat/models/message_new_event.py
+-rw-r--r--   0        0        0     2591 2023-10-25 08:58:18.700693 getstream-0.4.0/getstream/chat/models/message_pagination_params_request.py
+-rw-r--r--   0        0        0     1229 2023-10-25 08:58:18.700823 getstream-0.4.0/getstream/chat/models/message_read_event.py
+-rw-r--r--   0        0        0     2899 2023-10-25 08:58:18.700954 getstream-0.4.0/getstream/chat/models/message_request.py
+-rw-r--r--   0        0        0     5213 2023-10-25 08:58:18.701161 getstream-0.4.0/getstream/chat/models/message_request_1.py
+-rw-r--r--   0        0        0      505 2023-10-25 08:58:18.701281 getstream-0.4.0/getstream/chat/models/message_response.py
+-rw-r--r--   0        0        0     1181 2023-10-25 08:58:18.701405 getstream-0.4.0/getstream/chat/models/message_unblocked_event.py
+-rw-r--r--   0        0        0     1405 2023-10-25 08:58:18.701526 getstream-0.4.0/getstream/chat/models/message_updated_event.py
+-rw-r--r--   0        0        0      677 2023-10-25 08:58:18.701650 getstream-0.4.0/getstream/chat/models/message_with_pending_metadata_response.py
+-rw-r--r--   0        0        0      594 2023-10-25 08:58:18.701771 getstream-0.4.0/getstream/chat/models/moderation_response.py
+-rw-r--r--   0        0        0      778 2023-10-25 08:58:18.701897 getstream-0.4.0/getstream/chat/models/moderation_response_request.py
+-rw-r--r--   0        0        0      750 2023-10-25 08:58:18.702017 getstream-0.4.0/getstream/chat/models/mute_channel_request.py
+-rw-r--r--   0        0        0      825 2023-10-25 08:58:18.702142 getstream-0.4.0/getstream/chat/models/mute_channel_response.py
+-rw-r--r--   0        0        0      723 2023-10-25 08:58:18.702259 getstream-0.4.0/getstream/chat/models/mute_user_request.py
+-rw-r--r--   0        0        0      764 2023-10-25 08:58:18.702382 getstream-0.4.0/getstream/chat/models/mute_user_response.py
+-rw-r--r--   0        0        0     1242 2023-10-25 08:58:18.702511 getstream-0.4.0/getstream/chat/models/notification_added_to_channel_event.py
+-rw-r--r--   0        0        0     1151 2023-10-25 08:58:18.702629 getstream-0.4.0/getstream/chat/models/notification_channel_deleted_event.py
+-rw-r--r--   0        0        0      774 2023-10-25 08:58:18.702752 getstream-0.4.0/getstream/chat/models/notification_channel_mutes_updated_event.py
+-rw-r--r--   0        0        0     1071 2023-10-25 08:58:18.702883 getstream-0.4.0/getstream/chat/models/notification_channel_truncated_event.py
+-rw-r--r--   0        0        0     1388 2023-10-25 08:58:18.703010 getstream-0.4.0/getstream/chat/models/notification_invite_accepted_event.py
+-rw-r--r--   0        0        0     1388 2023-10-25 08:58:18.703140 getstream-0.4.0/getstream/chat/models/notification_invite_rejected_event.py
+-rw-r--r--   0        0        0     1381 2023-10-25 08:58:18.703256 getstream-0.4.0/getstream/chat/models/notification_invited_event.py
+-rw-r--r--   0        0        0     1531 2023-10-25 08:58:18.703369 getstream-0.4.0/getstream/chat/models/notification_mark_read_event.py
+-rw-r--r--   0        0        0     2091 2023-10-25 08:58:18.703493 getstream-0.4.0/getstream/chat/models/notification_mark_unread_event.py
+-rw-r--r--   0        0        0      767 2023-10-25 08:58:18.703621 getstream-0.4.0/getstream/chat/models/notification_mutes_updated_event.py
+-rw-r--r--   0        0        0     1265 2023-10-25 08:58:18.703742 getstream-0.4.0/getstream/chat/models/notification_new_message_event.py
+-rw-r--r--   0        0        0     1392 2023-10-25 08:58:18.703864 getstream-0.4.0/getstream/chat/models/notification_removed_from_channel_event.py
+-rw-r--r--   0        0        0      873 2023-10-26 15:09:14.794332 getstream-0.4.0/getstream/chat/models/notification_settings.py
+-rw-r--r--   0        0        0      310 2023-10-25 08:58:18.704099 getstream-0.4.0/getstream/chat/models/only_user_id_request.py
+-rw-r--r--   0        0        0     3278 2023-10-25 08:58:18.704217 getstream-0.4.0/getstream/chat/models/own_user.py
+-rw-r--r--   0        0        0     3850 2023-10-25 08:58:18.704334 getstream-0.4.0/getstream/chat/models/own_user_request.py
+-rw-r--r--   0        0        0      801 2023-10-25 08:58:18.704444 getstream-0.4.0/getstream/chat/models/pagination_params_request.py
+-rw-r--r--   0        0        0      861 2023-10-25 08:58:18.704560 getstream-0.4.0/getstream/chat/models/pending_message.py
+-rw-r--r--   0        0        0      973 2023-10-25 08:58:18.704669 getstream-0.4.0/getstream/chat/models/permission.py
+-rw-r--r--   0        0        0     1224 2023-10-25 08:58:18.704784 getstream-0.4.0/getstream/chat/models/policy.py
+-rw-r--r--   0        0        0      798 2023-10-25 08:58:18.704909 getstream-0.4.0/getstream/chat/models/policy_request.py
+-rw-r--r--   0        0        0      665 2023-10-25 08:58:18.705029 getstream-0.4.0/getstream/chat/models/policy_request_1.py
+-rw-r--r--   0        0        0      486 2023-10-25 08:58:18.705135 getstream-0.4.0/getstream/chat/models/push_config_request.py
+-rw-r--r--   0        0        0     1216 2023-10-25 08:58:18.705245 getstream-0.4.0/getstream/chat/models/push_notification_fields.py
+-rw-r--r--   0        0        0      796 2023-10-25 08:58:18.705435 getstream-0.4.0/getstream/chat/models/push_notification_settings.py
+-rw-r--r--   0        0        0      803 2023-10-25 08:58:18.705551 getstream-0.4.0/getstream/chat/models/push_notification_settings_request.py
+-rw-r--r--   0        0        0     3775 2023-10-25 08:58:18.705668 getstream-0.4.0/getstream/chat/models/push_provider.py
+-rw-r--r--   0        0        0     3926 2023-10-25 08:58:18.705790 getstream-0.4.0/getstream/chat/models/push_provider_request.py
+-rw-r--r--   0        0        0     4086 2023-10-25 08:58:18.705921 getstream-0.4.0/getstream/chat/models/push_provider_response.py
+-rw-r--r--   0        0        0     2349 2023-10-25 08:58:18.706043 getstream-0.4.0/getstream/chat/models/query_banned_users_request.py
+-rw-r--r--   0        0        0      485 2023-10-25 08:58:18.706168 getstream-0.4.0/getstream/chat/models/query_banned_users_response.py
+-rw-r--r--   0        0        0      657 2023-10-25 08:58:18.706289 getstream-0.4.0/getstream/chat/models/query_campaigns_request.py
+-rw-r--r--   0        0        0      886 2023-10-25 08:58:18.706413 getstream-0.4.0/getstream/chat/models/query_campaigns_response.py
+-rw-r--r--   0        0        0     1744 2023-10-25 08:58:18.706535 getstream-0.4.0/getstream/chat/models/query_channels_request.py
+-rw-r--r--   0        0        0     3098 2023-10-26 15:09:14.794908 getstream-0.4.0/getstream/chat/models/query_members_request.py
+-rw-r--r--   0        0        0      838 2023-10-25 08:58:18.706781 getstream-0.4.0/getstream/chat/models/query_message_flags_request.py
+-rw-r--r--   0        0        0      488 2023-10-25 08:58:18.706897 getstream-0.4.0/getstream/chat/models/query_message_flags_response.py
+-rw-r--r--   0        0        0      658 2023-10-25 08:58:18.707017 getstream-0.4.0/getstream/chat/models/query_recipients_request.py
+-rw-r--r--   0        0        0     1028 2023-10-25 08:58:18.707147 getstream-0.4.0/getstream/chat/models/query_recipients_response.py
+-rw-r--r--   0        0        0      656 2023-10-25 08:58:18.707263 getstream-0.4.0/getstream/chat/models/query_segments_request.py
+-rw-r--r--   0        0        0      477 2023-10-25 08:58:18.707386 getstream-0.4.0/getstream/chat/models/query_segments_response.py
+-rw-r--r--   0        0        0     1603 2023-10-25 08:58:18.707509 getstream-0.4.0/getstream/chat/models/query_users_request.py
+-rw-r--r--   0        0        0     1265 2023-10-25 08:58:18.707637 getstream-0.4.0/getstream/chat/models/reaction.py
+-rw-r--r--   0        0        0     1567 2023-10-25 08:58:18.707757 getstream-0.4.0/getstream/chat/models/reaction_deleted_event.py
+-rw-r--r--   0        0        0     1563 2023-10-25 08:58:18.707885 getstream-0.4.0/getstream/chat/models/reaction_new_event.py
+-rw-r--r--   0        0        0      674 2023-10-25 08:58:18.708017 getstream-0.4.0/getstream/chat/models/reaction_removal_response.py
+-rw-r--r--   0        0        0      803 2023-10-25 08:58:18.708139 getstream-0.4.0/getstream/chat/models/reaction_request.py
+-rw-r--r--   0        0        0      667 2023-10-26 15:09:14.795218 getstream-0.4.0/getstream/chat/models/reaction_response.py
+-rw-r--r--   0        0        0     1346 2023-10-25 08:58:18.708384 getstream-0.4.0/getstream/chat/models/reaction_updated_event.py
+-rw-r--r--   0        0        0      670 2023-10-25 08:58:18.708508 getstream-0.4.0/getstream/chat/models/reactivate_user_request.py
+-rw-r--r--   0        0        0      502 2023-10-25 08:58:18.708625 getstream-0.4.0/getstream/chat/models/reactivate_user_response.py
+-rw-r--r--   0        0        0      603 2023-10-25 08:58:18.708749 getstream-0.4.0/getstream/chat/models/reactivate_users_request.py
+-rw-r--r--   0        0        0      392 2023-10-25 08:58:18.708868 getstream-0.4.0/getstream/chat/models/reactivate_users_response.py
+-rw-r--r--   0        0        0      955 2023-10-25 08:58:18.708989 getstream-0.4.0/getstream/chat/models/read.py
+-rw-r--r--   0        0        0     1228 2023-10-25 08:58:18.709107 getstream-0.4.0/getstream/chat/models/recipient.py
+-rw-r--r--   0        0        0      446 2023-10-25 08:58:18.709225 getstream-0.4.0/getstream/chat/models/record_settings.py
+-rw-r--r--   0        0        0      313 2023-10-26 15:09:02.046131 getstream-0.4.0/getstream/chat/models/response.py
+-rw-r--r--   0        0        0      355 2023-10-25 08:58:18.709586 getstream-0.4.0/getstream/chat/models/restore_users_request.py
+-rw-r--r--   0        0        0      517 2023-10-25 08:58:18.709710 getstream-0.4.0/getstream/chat/models/resume_campaign_response.py
+-rw-r--r--   0        0        0      471 2023-10-26 15:09:02.059585 getstream-0.4.0/getstream/chat/models/ring_settings.py
+-rw-r--r--   0        0        0     1024 2023-10-25 08:58:18.710024 getstream-0.4.0/getstream/chat/models/role.py
+-rw-r--r--   0        0        0      405 2023-10-25 08:58:18.710139 getstream-0.4.0/getstream/chat/models/schedule_campaign_request.py
+-rw-r--r--   0        0        0      519 2023-10-25 08:58:18.710247 getstream-0.4.0/getstream/chat/models/schedule_campaign_response.py
+-rw-r--r--   0        0        0      434 2023-10-26 15:09:02.074120 getstream-0.4.0/getstream/chat/models/screensharing_settings.py
+-rw-r--r--   0        0        0     1056 2023-10-25 08:58:18.710499 getstream-0.4.0/getstream/chat/models/search_request.py
+-rw-r--r--   0        0        0      871 2023-10-25 08:58:18.710612 getstream-0.4.0/getstream/chat/models/search_response.py
+-rw-r--r--   0        0        0      474 2023-10-25 08:58:18.710723 getstream-0.4.0/getstream/chat/models/search_result.py
+-rw-r--r--   0        0        0     4738 2023-10-25 08:58:18.710901 getstream-0.4.0/getstream/chat/models/search_result_message.py
+-rw-r--r--   0        0        0      709 2023-10-25 08:58:18.711015 getstream-0.4.0/getstream/chat/models/search_warning.py
+-rw-r--r--   0        0        0     1339 2023-10-25 08:58:18.711135 getstream-0.4.0/getstream/chat/models/segment.py
+-rw-r--r--   0        0        0      594 2023-10-25 08:58:18.711282 getstream-0.4.0/getstream/chat/models/segment_data_request.py
+-rw-r--r--   0        0        0      692 2023-10-25 08:58:18.711395 getstream-0.4.0/getstream/chat/models/segment_updateable_fields_request.py
+-rw-r--r--   0        0        0      386 2023-10-26 15:09:14.795578 getstream-0.4.0/getstream/chat/models/send_event_request.py
+-rw-r--r--   0        0        0     1178 2023-10-25 08:58:18.711624 getstream-0.4.0/getstream/chat/models/send_message_request.py
+-rw-r--r--   0        0        0      734 2023-10-26 15:09:14.796180 getstream-0.4.0/getstream/chat/models/send_reaction_request.py
+-rw-r--r--   0        0        0      428 2023-10-25 08:58:18.711851 getstream-0.4.0/getstream/chat/models/send_user_custom_event_request.py
+-rw-r--r--   0        0        0      556 2023-10-25 08:58:18.711969 getstream-0.4.0/getstream/chat/models/show_channel_request.py
+-rw-r--r--   0        0        0      324 2023-10-25 08:58:18.712076 getstream-0.4.0/getstream/chat/models/show_channel_response.py
+-rw-r--r--   0        0        0      467 2023-10-25 08:58:18.712181 getstream-0.4.0/getstream/chat/models/sort_param.py
+-rw-r--r--   0        0        0      474 2023-10-26 15:09:02.167719 getstream-0.4.0/getstream/chat/models/sort_param_request.py
+-rw-r--r--   0        0        0      515 2023-10-25 08:58:18.712399 getstream-0.4.0/getstream/chat/models/stop_campaign_response.py
+-rw-r--r--   0        0        0      325 2023-10-25 08:58:18.712518 getstream-0.4.0/getstream/chat/models/stop_watching_response.py
+-rw-r--r--   0        0        0     1446 2023-10-25 08:58:18.712627 getstream-0.4.0/getstream/chat/models/sync_request.py
+-rw-r--r--   0        0        0      596 2023-10-25 08:58:18.712745 getstream-0.4.0/getstream/chat/models/sync_response.py
+-rw-r--r--   0        0        0      441 2023-10-26 15:09:14.796674 getstream-0.4.0/getstream/chat/models/target_resolution.py
+-rw-r--r--   0        0        0      349 2023-10-25 08:58:18.713049 getstream-0.4.0/getstream/chat/models/test_campaign_request.py
+-rw-r--r--   0        0        0      623 2023-10-25 08:58:18.713160 getstream-0.4.0/getstream/chat/models/test_campaign_response.py
+-rw-r--r--   0        0        0      679 2023-10-25 08:58:18.713267 getstream-0.4.0/getstream/chat/models/thresholds.py
+-rw-r--r--   0        0        0      722 2023-10-25 08:58:18.713375 getstream-0.4.0/getstream/chat/models/thresholds_request.py
+-rw-r--r--   0        0        0      406 2023-10-26 15:09:02.167671 getstream-0.4.0/getstream/chat/models/transcription_settings.py
+-rw-r--r--   0        0        0      328 2023-10-25 08:58:18.713609 getstream-0.4.0/getstream/chat/models/translate_message_request.py
+-rw-r--r--   0        0        0     1351 2023-10-25 08:58:18.713740 getstream-0.4.0/getstream/chat/models/truncate_channel_request.py
+-rw-r--r--   0        0        0      694 2023-10-25 08:58:18.713850 getstream-0.4.0/getstream/chat/models/truncate_channel_response.py
+-rw-r--r--   0        0        0     1125 2023-10-25 08:58:18.713957 getstream-0.4.0/getstream/chat/models/typing_start_event.py
+-rw-r--r--   0        0        0     1124 2023-10-25 08:58:18.714067 getstream-0.4.0/getstream/chat/models/typing_stop_event.py
+-rw-r--r--   0        0        0      824 2023-10-25 08:58:18.714176 getstream-0.4.0/getstream/chat/models/unmute_channel_request.py
+-rw-r--r--   0        0        0      319 2023-10-25 08:58:18.714414 getstream-0.4.0/getstream/chat/models/unmute_response.py
+-rw-r--r--   0        0        0      793 2023-10-25 08:58:18.714527 getstream-0.4.0/getstream/chat/models/unmute_user_request.py
+-rw-r--r--   0        0        0     5778 2023-10-25 08:58:18.714701 getstream-0.4.0/getstream/chat/models/update_app_request.py
+-rw-r--r--   0        0        0      482 2023-10-25 08:58:18.714804 getstream-0.4.0/getstream/chat/models/update_block_list_request.py
+-rw-r--r--   0        0        0      479 2023-10-25 08:58:18.714904 getstream-0.4.0/getstream/chat/models/update_campaign_request.py
+-rw-r--r--   0        0        0      517 2023-10-25 08:58:18.715020 getstream-0.4.0/getstream/chat/models/update_campaign_response.py
+-rw-r--r--   0        0        0      713 2023-10-25 08:58:18.715134 getstream-0.4.0/getstream/chat/models/update_channel_partial_request.py
+-rw-r--r--   0        0        0      692 2023-10-25 08:58:18.715242 getstream-0.4.0/getstream/chat/models/update_channel_partial_response.py
+-rw-r--r--   0        0        0     2211 2023-10-25 08:58:18.715348 getstream-0.4.0/getstream/chat/models/update_channel_request.py
+-rw-r--r--   0        0        0      841 2023-10-25 08:58:18.715456 getstream-0.4.0/getstream/chat/models/update_channel_response.py
+-rw-r--r--   0        0        0     3054 2023-10-25 08:58:18.715567 getstream-0.4.0/getstream/chat/models/update_channel_type_request.py
+-rw-r--r--   0        0        0     2962 2023-10-25 08:58:18.715683 getstream-0.4.0/getstream/chat/models/update_channel_type_response.py
+-rw-r--r--   0        0        0      604 2023-10-25 08:58:18.715807 getstream-0.4.0/getstream/chat/models/update_command_request.py
+-rw-r--r--   0        0        0      511 2023-10-25 08:58:18.715934 getstream-0.4.0/getstream/chat/models/update_command_response.py
+-rw-r--r--   0        0        0      832 2023-10-25 08:58:18.716062 getstream-0.4.0/getstream/chat/models/update_message_partial_request.py
+-rw-r--r--   0        0        0      700 2023-10-25 08:58:18.716182 getstream-0.4.0/getstream/chat/models/update_message_request.py
+-rw-r--r--   0        0        0      473 2023-10-25 08:58:18.716296 getstream-0.4.0/getstream/chat/models/update_segment_request.py
+-rw-r--r--   0        0        0      511 2023-10-25 08:58:18.716407 getstream-0.4.0/getstream/chat/models/update_segment_response.py
+-rw-r--r--   0        0        0      484 2023-10-25 08:58:18.716512 getstream-0.4.0/getstream/chat/models/update_user_partial_request.py
+-rw-r--r--   0        0        0      439 2023-10-25 08:58:18.716615 getstream-0.4.0/getstream/chat/models/update_users_request.py
+-rw-r--r--   0        0        0      484 2023-10-25 08:58:18.716803 getstream-0.4.0/getstream/chat/models/update_users_response.py
+-rw-r--r--   0        0        0      499 2023-10-25 08:58:18.716914 getstream-0.4.0/getstream/chat/models/upsert_push_provider_request.py
+-rw-r--r--   0        0        0      517 2023-10-25 08:58:18.717082 getstream-0.4.0/getstream/chat/models/upsert_push_provider_response.py
+-rw-r--r--   0        0        0     1622 2023-10-25 08:58:18.717262 getstream-0.4.0/getstream/chat/models/user_banned_event.py
+-rw-r--r--   0        0        0      739 2023-10-25 08:58:18.717586 getstream-0.4.0/getstream/chat/models/user_custom_event_request.py
+-rw-r--r--   0        0        0      900 2023-10-25 08:58:18.717696 getstream-0.4.0/getstream/chat/models/user_deactivated_event.py
+-rw-r--r--   0        0        0     1120 2023-10-25 08:58:18.717807 getstream-0.4.0/getstream/chat/models/user_deleted_event.py
+-rw-r--r--   0        0        0     1053 2023-10-25 08:58:18.717917 getstream-0.4.0/getstream/chat/models/user_flagged_event.py
+-rw-r--r--   0        0        0     1386 2023-10-25 08:58:18.718026 getstream-0.4.0/getstream/chat/models/user_mute.py
+-rw-r--r--   0        0        0     1556 2023-10-25 08:58:18.718138 getstream-0.4.0/getstream/chat/models/user_mute_request.py
+-rw-r--r--   0        0        0     1051 2023-10-25 08:58:18.718249 getstream-0.4.0/getstream/chat/models/user_muted_event.py
+-rw-r--r--   0        0        0     3281 2024-02-05 13:29:16.706111 getstream-0.4.0/getstream/chat/models/user_object.py
+-rw-r--r--   0        0        0     1814 2023-10-25 08:58:18.718539 getstream-0.4.0/getstream/chat/models/user_object_request.py
+-rw-r--r--   0        0        0      827 2023-10-25 08:58:18.718645 getstream-0.4.0/getstream/chat/models/user_presence_changed_event.py
+-rw-r--r--   0        0        0      823 2023-10-25 08:58:18.718754 getstream-0.4.0/getstream/chat/models/user_reactivated_event.py
+-rw-r--r--   0        0        0      811 2023-10-26 15:09:14.797466 getstream-0.4.0/getstream/chat/models/user_request.py
+-rw-r--r--   0        0        0     3360 2023-10-26 15:09:14.797704 getstream-0.4.0/getstream/chat/models/user_response.py
+-rw-r--r--   0        0        0     1165 2023-10-25 08:58:18.719080 getstream-0.4.0/getstream/chat/models/user_unbanned_event.py
+-rw-r--r--   0        0        0     1053 2023-10-25 08:58:18.719189 getstream-0.4.0/getstream/chat/models/user_unmuted_event.py
+-rw-r--r--   0        0        0      988 2023-10-25 08:58:18.719302 getstream-0.4.0/getstream/chat/models/user_unread_reminder_event.py
+-rw-r--r--   0        0        0      819 2023-10-25 08:58:18.719412 getstream-0.4.0/getstream/chat/models/user_updated_event.py
+-rw-r--r--   0        0        0     1183 2023-10-25 08:58:18.719550 getstream-0.4.0/getstream/chat/models/user_watching_start_event.py
+-rw-r--r--   0        0        0     1100 2023-10-25 08:58:18.719743 getstream-0.4.0/getstream/chat/models/user_watching_stop_event.py
+-rw-r--r--   0        0        0      479 2023-10-25 08:58:18.720170 getstream-0.4.0/getstream/chat/models/users_response.py
+-rw-r--r--   0        0        0      768 2023-10-26 15:09:14.798312 getstream-0.4.0/getstream/chat/models/video_settings.py
+-rw-r--r--   0        0        0      395 2023-10-26 15:09:02.291531 getstream-0.4.0/getstream/chat/models/ws_client_event.py
+-rw-r--r--   0        0        0      549 2023-10-25 08:58:18.720526 getstream-0.4.0/getstream/chat/models/xiaomi_config_fields.py
+-rw-r--r--   0        0        0      590 2023-10-25 08:58:18.720634 getstream-0.4.0/getstream/chat/models/xiaomi_config_request.py
+-rw-r--r--   0        0        0       64 2023-10-10 11:41:14.142640 getstream-0.4.0/getstream/chat/sync/__init__.py
+-rw-r--r--   0        0        0      212 2023-10-10 11:41:14.143094 getstream-0.4.0/getstream/chat/sync/chat.py
+-rw-r--r--   0        0        0       52 2023-07-07 15:29:51.349357 getstream-0.4.0/getstream/cli/__init__.py
+-rw-r--r--   0        0        0      997 2023-11-15 09:53:17.482753 getstream-0.4.0/getstream/cli/create_token.py
+-rw-r--r--   0        0        0      925 2023-06-06 11:12:09.256010 getstream-0.4.0/getstream/config.py
+-rw-r--r--   0        0        0       46 2024-03-06 06:15:35.459409 getstream-0.4.0/getstream/generic.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:11:28.258211 getstream-0.4.0/getstream/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-10-26 15:09:30.638378 getstream-0.4.0/getstream/models/accept_call_response.py
+-rw-r--r--   0        0        0      816 2024-03-25 09:35:04.030840 getstream-0.4.0/getstream/models/api_error.py
+-rw-r--r--   0        0        0      361 2024-03-06 06:15:35.459327 getstream-0.4.0/getstream/models/apns.py
+-rw-r--r--   0        0        0      445 2024-03-06 06:15:35.459099 getstream-0.4.0/getstream/models/apns_request.py
+-rw-r--r--   0        0        0      801 2024-03-25 09:35:04.031404 getstream-0.4.0/getstream/models/audio_settings.py
+-rw-r--r--   0        0        0      999 2024-03-25 09:35:04.031696 getstream-0.4.0/getstream/models/audio_settings_request.py
+-rw-r--r--   0        0        0      569 2024-03-25 09:35:04.032072 getstream-0.4.0/getstream/models/azure_request.py
+-rw-r--r--   0        0        0      321 2024-03-06 06:15:35.470086 getstream-0.4.0/getstream/models/backstage_settings.py
+-rw-r--r--   0        0        0      381 2024-03-06 06:15:35.473379 getstream-0.4.0/getstream/models/backstage_settings_request.py
+-rw-r--r--   0        0        0      319 2024-03-06 06:15:35.547330 getstream-0.4.0/getstream/models/block_user_request.py
+-rw-r--r--   0        0        0      322 2024-03-06 06:15:35.478084 getstream-0.4.0/getstream/models/block_user_response.py
+-rw-r--r--   0        0        0      989 2023-10-26 15:13:34.099436 getstream-0.4.0/getstream/models/blocked_user_event.py
+-rw-r--r--   0        0        0      559 2024-03-06 06:15:35.576934 getstream-0.4.0/getstream/models/broadcast_settings_request.py
+-rw-r--r--   0        0        0      473 2024-03-06 06:15:35.491305 getstream-0.4.0/getstream/models/broadcast_settings_response.py
+-rw-r--r--   0        0        0      958 2023-10-26 15:13:34.100711 getstream-0.4.0/getstream/models/call_accepted_event.py
+-rw-r--r--   0        0        0      999 2023-10-26 15:13:34.101924 getstream-0.4.0/getstream/models/call_created_event.py
+-rw-r--r--   0        0        0     1021 2023-10-26 15:13:34.102478 getstream-0.4.0/getstream/models/call_ended_event.py
+-rw-r--r--   0        0        0      725 2023-10-26 15:13:34.102877 getstream-0.4.0/getstream/models/call_hls_broadcasting_failed_event.py
+-rw-r--r--   0        0        0      808 2023-10-26 15:09:30.784351 getstream-0.4.0/getstream/models/call_hls_broadcasting_started_event.py
+-rw-r--r--   0        0        0      726 2023-10-26 15:09:30.784639 getstream-0.4.0/getstream/models/call_hls_broadcasting_stopped_event.py
+-rw-r--r--   0        0        0      379 2024-03-06 06:15:35.485235 getstream-0.4.0/getstream/models/call_ingress_response.py
+-rw-r--r--   0        0        0      838 2023-10-26 15:09:30.831320 getstream-0.4.0/getstream/models/call_live_started_event.py
+-rw-r--r--   0        0        0     1003 2023-10-26 15:13:34.103311 getstream-0.4.0/getstream/models/call_member_added_event.py
+-rw-r--r--   0        0        0      934 2023-10-26 15:13:34.103924 getstream-0.4.0/getstream/models/call_member_removed_event.py
+-rw-r--r--   0        0        0     1005 2023-10-26 15:13:34.104386 getstream-0.4.0/getstream/models/call_member_updated_event.py
+-rw-r--r--   0        0        0     1142 2023-10-26 15:13:34.104853 getstream-0.4.0/getstream/models/call_member_updated_permission_event.py
+-rw-r--r--   0        0        0     1197 2023-10-26 15:13:34.107283 getstream-0.4.0/getstream/models/call_notification_event.py
+-rw-r--r--   0        0        0      853 2024-03-25 09:35:04.032399 getstream-0.4.0/getstream/models/call_participant_response.py
+-rw-r--r--   0        0        0      855 2023-10-26 15:13:34.108923 getstream-0.4.0/getstream/models/call_reaction_event.py
+-rw-r--r--   0        0        0      938 2024-03-06 06:15:35.512927 getstream-0.4.0/getstream/models/call_recording.py
+-rw-r--r--   0        0        0      719 2023-10-26 15:09:30.869125 getstream-0.4.0/getstream/models/call_recording_failed_event.py
+-rw-r--r--   0        0        0      864 2023-10-26 15:09:30.866274 getstream-0.4.0/getstream/models/call_recording_ready_event.py
+-rw-r--r--   0        0        0      720 2023-10-26 15:09:30.865388 getstream-0.4.0/getstream/models/call_recording_started_event.py
+-rw-r--r--   0        0        0      720 2023-10-26 15:09:30.876122 getstream-0.4.0/getstream/models/call_recording_stopped_event.py
+-rw-r--r--   0        0        0      958 2023-10-26 15:13:34.110607 getstream-0.4.0/getstream/models/call_rejected_event.py
+-rw-r--r--   0        0        0     1514 2024-03-25 09:35:04.032855 getstream-0.4.0/getstream/models/call_request.py
+-rw-r--r--   0        0        0     3093 2024-03-25 09:35:04.033241 getstream-0.4.0/getstream/models/call_response.py
+-rw-r--r--   0        0        0     1189 2023-10-26 15:13:34.112748 getstream-0.4.0/getstream/models/call_ring_event.py
+-rw-r--r--   0        0        0      909 2023-10-26 15:13:34.113417 getstream-0.4.0/getstream/models/call_session_ended_event.py
+-rw-r--r--   0        0        0      983 2023-10-26 15:13:34.114186 getstream-0.4.0/getstream/models/call_session_participant_joined_event.py
+-rw-r--r--   0        0        0      981 2023-10-26 15:13:34.115220 getstream-0.4.0/getstream/models/call_session_participant_left_event.py
+-rw-r--r--   0        0        0     2140 2024-03-25 09:35:04.033663 getstream-0.4.0/getstream/models/call_session_response.py
+-rw-r--r--   0        0        0      911 2023-10-26 15:13:34.117557 getstream-0.4.0/getstream/models/call_session_started_event.py
+-rw-r--r--   0        0        0     2343 2024-03-25 09:35:04.034001 getstream-0.4.0/getstream/models/call_settings_request.py
+-rw-r--r--   0        0        0     1956 2024-03-25 09:35:04.034387 getstream-0.4.0/getstream/models/call_settings_response.py
+-rw-r--r--   0        0        0      850 2024-03-06 06:15:35.563247 getstream-0.4.0/getstream/models/call_state_response_fields.py
+-rw-r--r--   0        0        0      942 2024-03-25 09:35:04.034642 getstream-0.4.0/getstream/models/call_transcription.py
+-rw-r--r--   0        0        0     1471 2024-03-25 09:35:04.034949 getstream-0.4.0/getstream/models/call_type_response.py
+-rw-r--r--   0        0        0      985 2023-10-26 15:09:31.065346 getstream-0.4.0/getstream/models/call_updated_event.py
+-rw-r--r--   0        0        0      890 2023-10-26 15:13:34.119184 getstream-0.4.0/getstream/models/call_user_muted.py
+-rw-r--r--   0        0        0      333 2024-03-25 09:35:04.035176 getstream-0.4.0/getstream/models/check_external_storage_response.py
+-rw-r--r--   0        0        0      706 2024-03-25 09:35:04.035618 getstream-0.4.0/getstream/models/connect_user_details_request.py
+-rw-r--r--   0        0        0      848 2023-10-26 15:13:34.120348 getstream-0.4.0/getstream/models/connected_event.py
+-rw-r--r--   0        0        0      838 2023-11-15 09:53:17.483717 getstream-0.4.0/getstream/models/connection_error_event.py
+-rw-r--r--   0        0        0     1028 2024-03-25 09:35:04.035867 getstream-0.4.0/getstream/models/create_call_type_request.py
+-rw-r--r--   0        0        0     1543 2024-03-25 09:35:04.036317 getstream-0.4.0/getstream/models/create_call_type_response.py
+-rw-r--r--   0        0        0      958 2024-03-25 09:35:04.036740 getstream-0.4.0/getstream/models/create_device_request.py
+-rw-r--r--   0        0        0     1021 2024-03-25 09:35:04.037055 getstream-0.4.0/getstream/models/create_external_storage_request.py
+-rw-r--r--   0        0        0      334 2024-03-25 09:35:04.037251 getstream-0.4.0/getstream/models/create_external_storage_response.py
+-rw-r--r--   0        0        0      378 2024-03-06 06:15:35.674062 getstream-0.4.0/getstream/models/create_guest_request.py
+-rw-r--r--   0        0        0      522 2024-03-06 06:21:17.287873 getstream-0.4.0/getstream/models/create_guest_response.py
+-rw-r--r--   0        0        0      593 2023-10-26 15:13:34.122234 getstream-0.4.0/getstream/models/credentials.py
+-rw-r--r--   0        0        0      934 2023-10-26 15:13:34.122492 getstream-0.4.0/getstream/models/custom_video_event.py
+-rw-r--r--   0        0        0      334 2024-03-25 09:35:04.037550 getstream-0.4.0/getstream/models/delete_external_storage_response.py
+-rw-r--r--   0        0        0     1165 2024-03-25 09:35:04.037857 getstream-0.4.0/getstream/models/device.py
+-rw-r--r--   0        0        0      967 2024-03-25 09:35:04.038282 getstream-0.4.0/getstream/models/edge_response.py
+-rw-r--r--   0        0        0      330 2024-03-06 06:15:35.692633 getstream-0.4.0/getstream/models/egress_hls_response.py
+-rw-r--r--   0        0        0      688 2024-03-25 09:35:04.038637 getstream-0.4.0/getstream/models/egress_response.py
+-rw-r--r--   0        0        0      441 2024-03-06 06:15:35.696336 getstream-0.4.0/getstream/models/egress_rtmp_response.py
+-rw-r--r--   0        0        0      320 2024-03-06 06:15:35.698360 getstream-0.4.0/getstream/models/end_call_response.py
+-rw-r--r--   0        0        0      428 2024-03-06 06:15:35.703743 getstream-0.4.0/getstream/models/event_notification_settings.py
+-rw-r--r--   0        0        0      547 2024-03-06 06:15:35.715932 getstream-0.4.0/getstream/models/event_notification_settings_request.py
+-rw-r--r--   0        0        0      498 2024-03-25 09:35:04.038912 getstream-0.4.0/getstream/models/external_storage_response.py
+-rw-r--r--   0        0        0      346 2024-03-06 06:15:35.715939 getstream-0.4.0/getstream/models/geofence_settings.py
+-rw-r--r--   0        0        0      401 2024-03-06 06:15:35.722197 getstream-0.4.0/getstream/models/geofence_settings_request.py
+-rw-r--r--   0        0        0      908 2024-03-25 09:35:04.039228 getstream-0.4.0/getstream/models/get_call_response.py
+-rw-r--r--   0        0        0     1540 2024-03-25 09:35:04.039537 getstream-0.4.0/getstream/models/get_call_type_response.py
+-rw-r--r--   0        0        0      477 2024-03-25 09:35:04.039759 getstream-0.4.0/getstream/models/get_edges_response.py
+-rw-r--r--   0        0        0      732 2024-03-25 09:35:04.040027 getstream-0.4.0/getstream/models/get_or_create_call_request.py
+-rw-r--r--   0        0        0      981 2024-03-25 09:35:04.040347 getstream-0.4.0/getstream/models/get_or_create_call_response.py
+-rw-r--r--   0        0        0      906 2024-03-25 09:35:04.040630 getstream-0.4.0/getstream/models/go_live_request.py
+-rw-r--r--   0        0        0      443 2024-03-06 06:15:35.745863 getstream-0.4.0/getstream/models/go_live_response.py
+-rw-r--r--   0        0        0      721 2023-10-26 15:09:31.234394 getstream-0.4.0/getstream/models/health_check_event.py
+-rw-r--r--   0        0        0      785 2024-03-25 09:35:04.040934 getstream-0.4.0/getstream/models/hls_settings_request.py
+-rw-r--r--   0        0        0      630 2024-03-25 09:35:04.041294 getstream-0.4.0/getstream/models/hls_settings_response.py
+-rw-r--r--   0        0        0      469 2023-10-26 15:13:34.127380 getstream-0.4.0/getstream/models/ice_server.py
+-rw-r--r--   0        0        0      994 2023-10-26 15:13:34.128243 getstream-0.4.0/getstream/models/join_call_request.py
+-rw-r--r--   0        0        0     1107 2023-10-26 15:13:34.128472 getstream-0.4.0/getstream/models/join_call_response.py
+-rw-r--r--   0        0        0      609 2024-03-25 09:35:04.041673 getstream-0.4.0/getstream/models/layout_settings.py
+-rw-r--r--   0        0        0      692 2024-03-25 09:35:04.042015 getstream-0.4.0/getstream/models/layout_settings_request.py
+-rw-r--r--   0        0        0      523 2024-03-06 06:15:35.801110 getstream-0.4.0/getstream/models/list_call_type_response.py
+-rw-r--r--   0        0        0      465 2024-03-06 06:15:35.783893 getstream-0.4.0/getstream/models/list_devices_response.py
+-rw-r--r--   0        0        0      565 2024-03-25 09:35:04.042234 getstream-0.4.0/getstream/models/list_external_storage_response.py
+-rw-r--r--   0        0        0      496 2024-03-06 06:15:35.801125 getstream-0.4.0/getstream/models/list_recordings_response.py
+-rw-r--r--   0        0        0      534 2024-03-25 09:35:04.042523 getstream-0.4.0/getstream/models/list_transcriptions_response.py
+-rw-r--r--   0        0        0      516 2024-03-25 09:35:04.042857 getstream-0.4.0/getstream/models/member_request.py
+-rw-r--r--   0        0        0     1479 2024-03-25 09:35:04.043072 getstream-0.4.0/getstream/models/member_response.py
+-rw-r--r--   0        0        0      921 2024-03-25 09:35:04.043383 getstream-0.4.0/getstream/models/mute_users_request.py
+-rw-r--r--   0        0        0      322 2024-03-06 06:15:35.818187 getstream-0.4.0/getstream/models/mute_users_response.py
+-rw-r--r--   0        0        0      868 2024-03-25 09:35:04.043687 getstream-0.4.0/getstream/models/notification_settings.py
+-rw-r--r--   0        0        0     1075 2024-03-06 06:15:35.899753 getstream-0.4.0/getstream/models/notification_settings_request.py
+-rw-r--r--   0        0        0     2091 2024-04-11 19:07:16.766833 getstream-0.4.0/getstream/models/own_capability.py
+-rw-r--r--   0        0        0     1694 2023-10-26 15:13:34.133032 getstream-0.4.0/getstream/models/own_user_response.py
+-rw-r--r--   0        0        0      942 2023-10-26 15:13:34.133637 getstream-0.4.0/getstream/models/permission_request_event.py
+-rw-r--r--   0        0        0      383 2024-03-06 06:15:35.844488 getstream-0.4.0/getstream/models/pin_request.py
+-rw-r--r--   0        0        0      316 2024-03-06 06:15:35.844616 getstream-0.4.0/getstream/models/pin_response.py
+-rw-r--r--   0        0        0      929 2024-03-25 09:35:04.043997 getstream-0.4.0/getstream/models/query_calls_request.py
+-rw-r--r--   0        0        0      688 2024-03-06 06:15:35.899481 getstream-0.4.0/getstream/models/query_calls_response.py
+-rw-r--r--   0        0        0      958 2024-03-25 09:35:04.044349 getstream-0.4.0/getstream/models/query_members_request.py
+-rw-r--r--   0        0        0      665 2024-03-06 06:18:16.738466 getstream-0.4.0/getstream/models/query_members_response.py
+-rw-r--r--   0        0        0      693 2023-10-26 15:09:31.379785 getstream-0.4.0/getstream/models/reaction_response.py
+-rw-r--r--   0        0        0      737 2024-03-06 06:15:35.928883 getstream-0.4.0/getstream/models/record_settings_request.py
+-rw-r--r--   0        0        0      588 2024-03-25 09:35:04.044696 getstream-0.4.0/getstream/models/record_settings_response.py
+-rw-r--r--   0        0        0      323 2023-10-26 15:09:31.363208 getstream-0.4.0/getstream/models/reject_call_response.py
+-rw-r--r--   0        0        0      366 2023-10-26 15:09:31.368213 getstream-0.4.0/getstream/models/request_permission_request.py
+-rw-r--r--   0        0        0      330 2023-10-26 15:09:31.372119 getstream-0.4.0/getstream/models/request_permission_response.py
+-rw-r--r--   0        0        0      313 2024-03-06 06:15:35.923519 getstream-0.4.0/getstream/models/response.py
+-rw-r--r--   0        0        0      471 2024-03-25 09:35:04.045060 getstream-0.4.0/getstream/models/ring_settings.py
+-rw-r--r--   0        0        0      555 2024-03-06 06:15:35.941172 getstream-0.4.0/getstream/models/ring_settings_request.py
+-rw-r--r--   0        0        0      314 2024-03-06 06:15:35.942057 getstream-0.4.0/getstream/models/rtmp_ingress.py
+-rw-r--r--   0        0        0      559 2024-03-25 09:35:04.045304 getstream-0.4.0/getstream/models/s_3_request.py
+-rw-r--r--   0        0        0      434 2024-03-25 09:35:04.045936 getstream-0.4.0/getstream/models/screensharing_settings.py
+-rw-r--r--   0        0        0      518 2024-03-06 06:15:35.991696 getstream-0.4.0/getstream/models/screensharing_settings_request.py
+-rw-r--r--   0        0        0      373 2024-03-25 09:35:04.046541 getstream-0.4.0/getstream/models/send_event_request.py
+-rw-r--r--   0        0        0      322 2024-03-06 06:15:36.002956 getstream-0.4.0/getstream/models/send_event_response.py
+-rw-r--r--   0        0        0      573 2023-10-26 15:13:34.138347 getstream-0.4.0/getstream/models/send_reaction_request.py
+-rw-r--r--   0        0        0      469 2023-10-26 15:09:31.397508 getstream-0.4.0/getstream/models/send_reaction_response.py
+-rw-r--r--   0        0        0      446 2023-10-26 15:13:34.141505 getstream-0.4.0/getstream/models/sfu_response.py
+-rw-r--r--   0        0        0      228 2024-03-06 06:18:16.739513 getstream-0.4.0/getstream/models/sort_param_request.py
+-rw-r--r--   0        0        0      407 2024-03-06 06:15:36.024035 getstream-0.4.0/getstream/models/start_hls_broadcasting_response.py
+-rw-r--r--   0        0        0      429 2024-03-25 09:35:04.046791 getstream-0.4.0/getstream/models/start_recording_request.py
+-rw-r--r--   0        0        0      327 2024-03-06 06:15:36.024502 getstream-0.4.0/getstream/models/start_recording_response.py
+-rw-r--r--   0        0        0      441 2024-03-25 09:35:04.047037 getstream-0.4.0/getstream/models/start_transcription_request.py
+-rw-r--r--   0        0        0      331 2024-03-06 06:15:36.108076 getstream-0.4.0/getstream/models/start_transcription_response.py
+-rw-r--r--   0        0        0      332 2024-03-06 06:15:36.036673 getstream-0.4.0/getstream/models/stop_hls_broadcasting_response.py
+-rw-r--r--   0        0        0      445 2024-03-06 06:15:36.042631 getstream-0.4.0/getstream/models/stop_live_response.py
+-rw-r--r--   0        0        0      326 2024-03-06 06:15:36.037038 getstream-0.4.0/getstream/models/stop_recording_response.py
+-rw-r--r--   0        0        0      330 2024-03-06 06:15:36.036638 getstream-0.4.0/getstream/models/stop_transcription_response.py
+-rw-r--r--   0        0        0      441 2024-03-25 09:35:04.047453 getstream-0.4.0/getstream/models/target_resolution.py
+-rw-r--r--   0        0        0      549 2024-03-06 06:18:07.364495 getstream-0.4.0/getstream/models/target_resolution_request.py
+-rw-r--r--   0        0        0      324 2024-03-06 06:15:36.046316 getstream-0.4.0/getstream/models/thumbnail_response.py
+-rw-r--r--   0        0        0      322 2024-03-06 06:15:36.045681 getstream-0.4.0/getstream/models/thumbnails_settings.py
+-rw-r--r--   0        0        0      382 2024-03-06 06:15:36.053491 getstream-0.4.0/getstream/models/thumbnails_settings_request.py
+-rw-r--r--   0        0        0      406 2024-03-06 06:15:36.057901 getstream-0.4.0/getstream/models/transcription_settings.py
+-rw-r--r--   0        0        0      504 2024-03-06 06:15:36.115718 getstream-0.4.0/getstream/models/transcription_settings_request.py
+-rw-r--r--   0        0        0      321 2024-03-06 06:15:36.062333 getstream-0.4.0/getstream/models/unblock_user_request.py
+-rw-r--r--   0        0        0      324 2024-03-06 06:15:36.068417 getstream-0.4.0/getstream/models/unblock_user_response.py
+-rw-r--r--   0        0        0      836 2023-10-26 15:13:34.142754 getstream-0.4.0/getstream/models/unblocked_user_event.py
+-rw-r--r--   0        0        0      385 2024-03-06 06:18:07.365436 getstream-0.4.0/getstream/models/unpin_request.py
+-rw-r--r--   0        0        0      318 2024-03-06 06:15:36.072233 getstream-0.4.0/getstream/models/unpin_response.py
+-rw-r--r--   0        0        0      610 2024-03-06 06:15:36.086926 getstream-0.4.0/getstream/models/update_call_members_request.py
+-rw-r--r--   0        0        0      496 2024-03-06 06:15:36.080013 getstream-0.4.0/getstream/models/update_call_members_response.py
+-rw-r--r--   0        0        0      972 2024-03-25 09:35:04.047709 getstream-0.4.0/getstream/models/update_call_request.py
+-rw-r--r--   0        0        0      911 2024-03-25 09:35:04.048031 getstream-0.4.0/getstream/models/update_call_response.py
+-rw-r--r--   0        0        0      850 2024-03-25 09:35:04.048318 getstream-0.4.0/getstream/models/update_call_type_request.py
+-rw-r--r--   0        0        0     1413 2024-03-25 09:35:04.048639 getstream-0.4.0/getstream/models/update_call_type_response.py
+-rw-r--r--   0        0        0      963 2024-03-25 09:35:04.048822 getstream-0.4.0/getstream/models/update_external_storage_request.py
+-rw-r--r--   0        0        0      570 2024-03-25 09:35:04.049052 getstream-0.4.0/getstream/models/update_external_storage_response.py
+-rw-r--r--   0        0        0      624 2024-03-06 06:15:36.147605 getstream-0.4.0/getstream/models/update_user_permissions_request.py
+-rw-r--r--   0        0        0      334 2024-03-06 06:15:36.123340 getstream-0.4.0/getstream/models/update_user_permissions_response.py
+-rw-r--r--   0        0        0     1039 2023-10-26 15:13:34.143762 getstream-0.4.0/getstream/models/updated_call_permissions_event.py
+-rw-r--r--   0        0        0      884 2024-03-25 09:35:04.049275 getstream-0.4.0/getstream/models/user_request.py
+-rw-r--r--   0        0        0     1624 2024-03-25 09:35:04.049605 getstream-0.4.0/getstream/models/user_response.py
+-rw-r--r--   0        0        0     5688 2023-10-26 15:09:31.765367 getstream-0.4.0/getstream/models/video_event.py
+-rw-r--r--   0        0        0      763 2024-03-06 06:15:36.186449 getstream-0.4.0/getstream/models/video_settings.py
+-rw-r--r--   0        0        0      968 2024-03-06 06:15:36.219247 getstream-0.4.0/getstream/models/video_settings_request.py
+-rw-r--r--   0        0        0      514 2024-03-06 06:15:36.171604 getstream-0.4.0/getstream/models/ws_auth_message_request.py
+-rw-r--r--   0        0        0      383 2023-10-26 15:09:31.677417 getstream-0.4.0/getstream/models/ws_call_event.py
+-rw-r--r--   0        0        0      395 2023-10-26 15:09:31.678880 getstream-0.4.0/getstream/models/ws_client_event.py
+-rw-r--r--   0        0        0     1168 2024-03-06 06:15:36.222459 getstream-0.4.0/getstream/rate_limit.py
+-rw-r--r--   0        0        0     1209 2024-03-06 06:25:20.787577 getstream-0.4.0/getstream/stream_response.py
+-rw-r--r--   0        0        0       41 2023-10-25 08:58:18.748254 getstream-0.4.0/getstream/sync/__init__.py
+-rw-r--r--   0        0        0     4481 2024-03-06 06:18:07.369409 getstream-0.4.0/getstream/sync/base.py
+-rw-r--r--   0        0        0     9113 2023-11-15 09:53:17.484346 getstream-0.4.0/getstream/sync/stream.py
+-rw-r--r--   0        0        0     7403 2023-11-15 09:53:17.485082 getstream-0.4.0/getstream/users/sync/client.py
+-rw-r--r--   0        0        0     1671 2023-10-25 08:58:18.749193 getstream-0.4.0/getstream/utils.py
+-rw-r--r--   0        0        0       18 2024-04-11 19:07:16.767440 getstream-0.4.0/getstream/version.py
+-rw-r--r--   0        0        0      141 2024-02-12 08:30:27.994264 getstream-0.4.0/getstream/video/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-07 15:29:51.351074 getstream-0.4.0/getstream/video/async_/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 09:15:27.009605 getstream-0.4.0/getstream/video/async_/call.py
+-rw-r--r--   0        0        0      142 2023-05-05 11:43:39.447192 getstream-0.4.0/getstream/video/async_/client.py
+-rw-r--r--   0        0        0      754 2023-11-15 09:53:17.485376 getstream-0.4.0/getstream/video/exceptions.py
+-rw-r--r--   0        0        0       46 2023-10-25 08:58:18.749971 getstream-0.4.0/getstream/video/sync/__init__.py
+-rw-r--r--   0        0        0    37798 2024-03-25 09:35:04.050336 getstream-0.4.0/getstream/video/sync/base_client.py
+-rw-r--r--   0        0        0    30723 2024-03-25 09:35:04.050758 getstream-0.4.0/getstream/video/sync/client.py
+-rw-r--r--   0        0        0      672 2024-04-11 19:07:16.768031 getstream-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 getstream-0.4.0/PKG-INFO
```

### Comparing `getstream-0.3.0/LICENSE.md` & `getstream-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/README.md` & `getstream-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/async_/base.py` & `getstream-0.4.0/getstream/async_/base.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/base.py` & `getstream-0.4.0/getstream/base.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/action.py` & `getstream-0.4.0/getstream/chat/models/action.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/action_request.py` & `getstream-0.4.0/getstream/chat/models/action_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/any_event.py` & `getstream-0.4.0/getstream/chat/models/any_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/api_error.py` & `getstream-0.4.0/getstream/chat/models/api_error.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/apn_config_fields.py` & `getstream-0.4.0/getstream/chat/models/apn_config_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/apn_config_request.py` & `getstream-0.4.0/getstream/chat/models/apn_config_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/app.py` & `getstream-0.4.0/getstream/chat/models/app.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/async_moderation_configuration_request.py` & `getstream-0.4.0/getstream/chat/models/async_moderation_configuration_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/attachment.py` & `getstream-0.4.0/getstream/chat/models/attachment.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/attachment_request.py` & `getstream-0.4.0/getstream/chat/models/attachment_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/audio_settings.py` & `getstream-0.4.0/getstream/chat/models/audio_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/automod_details.py` & `getstream-0.4.0/getstream/chat/models/automod_details.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/ban_request.py` & `getstream-0.4.0/getstream/chat/models/ban_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/ban_response.py` & `getstream-0.4.0/getstream/chat/models/ban_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/block_list.py` & `getstream-0.4.0/getstream/chat/models/block_list.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/call.py` & `getstream-0.4.0/getstream/chat/models/call.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/call_settings.py` & `getstream-0.4.0/getstream/chat/models/call_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/call_type.py` & `getstream-0.4.0/getstream/chat/models/call_type.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/campaign.py` & `getstream-0.4.0/getstream/chat/models/campaign.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/campaign_data_request.py` & `getstream-0.4.0/getstream/chat/models/campaign_data_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/campaign_sort.py` & `getstream-0.4.0/getstream/chat/models/campaign_sort.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/campaign_updateable_fields_request.py` & `getstream-0.4.0/getstream/chat/models/campaign_updateable_fields_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel.py` & `getstream-0.4.0/getstream/chat/models/channel.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_config.py` & `getstream-0.4.0/getstream/chat/models/channel_config.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_config_request.py` & `getstream-0.4.0/getstream/chat/models/channel_config_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_config_with_info.py` & `getstream-0.4.0/getstream/chat/models/channel_config_with_info.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_config_with_info_request.py` & `getstream-0.4.0/getstream/chat/models/channel_config_with_info_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_created_event.py` & `getstream-0.4.0/getstream/chat/models/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_deleted_event.py` & `getstream-0.4.0/getstream/chat/models/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_export_request.py` & `getstream-0.4.0/getstream/chat/models/channel_export_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_frozen_event.py` & `getstream-0.4.0/getstream/chat/models/channel_frozen_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_get_or_create_request.py` & `getstream-0.4.0/getstream/chat/models/channel_get_or_create_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_hidden_event.py` & `getstream-0.4.0/getstream/chat/models/channel_hidden_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_kicked_event.py` & `getstream-0.4.0/getstream/chat/models/channel_kicked_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_member.py` & `getstream-0.4.0/getstream/chat/models/channel_member.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_member_request.py` & `getstream-0.4.0/getstream/chat/models/channel_member_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_messages.py` & `getstream-0.4.0/getstream/chat/models/channel_messages.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_mute.py` & `getstream-0.4.0/getstream/chat/models/channel_mute.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_mute_request.py` & `getstream-0.4.0/getstream/chat/models/channel_mute_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_muted_event.py` & `getstream-0.4.0/getstream/chat/models/channel_muted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_request.py` & `getstream-0.4.0/getstream/chat/models/channel_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_response.py` & `getstream-0.4.0/getstream/chat/models/channel_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_response_request.py` & `getstream-0.4.0/getstream/chat/models/channel_response_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_state_response.py` & `getstream-0.4.0/getstream/chat/models/channel_state_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_state_response_fields.py` & `getstream-0.4.0/getstream/chat/models/channel_state_response_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_stop_watching_request.py` & `getstream-0.4.0/getstream/chat/models/channel_stop_watching_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_truncated_event.py` & `getstream-0.4.0/getstream/chat/models/channel_truncated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_type_config.py` & `getstream-0.4.0/getstream/chat/models/channel_type_config.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_un_frozen_event.py` & `getstream-0.4.0/getstream/chat/models/channel_un_frozen_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_unmuted_event.py` & `getstream-0.4.0/getstream/chat/models/channel_unmuted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_updated_event.py` & `getstream-0.4.0/getstream/chat/models/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channel_visible_event.py` & `getstream-0.4.0/getstream/chat/models/channel_visible_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/channels_response.py` & `getstream-0.4.0/getstream/chat/models/channels_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/chat_event.py` & `getstream-0.4.0/getstream/chat/models/chat_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/check_push_request.py` & `getstream-0.4.0/getstream/chat/models/check_push_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/check_push_response.py` & `getstream-0.4.0/getstream/chat/models/check_push_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/check_sqs_request.py` & `getstream-0.4.0/getstream/chat/models/check_sqs_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/check_sqs_response.py` & `getstream-0.4.0/getstream/chat/models/check_sqs_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/command.py` & `getstream-0.4.0/getstream/chat/models/command.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/command_request.py` & `getstream-0.4.0/getstream/chat/models/command_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/config.py` & `getstream-0.4.0/getstream/chat/models/config.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/config_request.py` & `getstream-0.4.0/getstream/chat/models/config_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/connect_request.py` & `getstream-0.4.0/getstream/chat/models/connect_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_call_request.py` & `getstream-0.4.0/getstream/chat/models/create_call_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_call_response.py` & `getstream-0.4.0/getstream/chat/models/create_call_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_campaign_response.py` & `getstream-0.4.0/getstream/chat/models/create_campaign_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_channel_type_request.py` & `getstream-0.4.0/getstream/chat/models/create_channel_type_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_channel_type_response.py` & `getstream-0.4.0/getstream/chat/models/create_channel_type_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_command_request.py` & `getstream-0.4.0/getstream/chat/models/create_command_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_device_request.py` & `getstream-0.4.0/getstream/chat/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/create_import_response.py` & `getstream-0.4.0/getstream/chat/models/create_import_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/deactivate_user_request.py` & `getstream-0.4.0/getstream/chat/models/deactivate_user_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/deactivate_users_request.py` & `getstream-0.4.0/getstream/chat/models/deactivate_users_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/delete_channel_response.py` & `getstream-0.4.0/getstream/chat/models/delete_channel_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/delete_channels_response.py` & `getstream-0.4.0/getstream/chat/models/delete_channels_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/delete_user_response.py` & `getstream-0.4.0/getstream/chat/models/delete_user_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/delete_users_request.py` & `getstream-0.4.0/getstream/chat/models/delete_users_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/device.py` & `getstream-0.4.0/getstream/chat/models/device.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/device_fields.py` & `getstream-0.4.0/getstream/chat/models/device_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/device_request.py` & `getstream-0.4.0/getstream/chat/models/device_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/error_result.py` & `getstream-0.4.0/getstream/chat/models/error_result.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/event.py` & `getstream-0.4.0/getstream/chat/models/event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/event_request.py` & `getstream-0.4.0/getstream/chat/models/event_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/export_channels_request.py` & `getstream-0.4.0/getstream/chat/models/export_channels_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/export_channels_result.py` & `getstream-0.4.0/getstream/chat/models/export_channels_result.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/export_user_response.py` & `getstream-0.4.0/getstream/chat/models/export_user_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/field_request.py` & `getstream-0.4.0/getstream/chat/models/field_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/file_upload_config.py` & `getstream-0.4.0/getstream/chat/models/file_upload_config.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/file_upload_config_request.py` & `getstream-0.4.0/getstream/chat/models/file_upload_config_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/file_upload_request.py` & `getstream-0.4.0/getstream/chat/models/file_upload_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/file_upload_response.py` & `getstream-0.4.0/getstream/chat/models/file_upload_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/firebase_config_fields.py` & `getstream-0.4.0/getstream/chat/models/firebase_config_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/firebase_config_request.py` & `getstream-0.4.0/getstream/chat/models/firebase_config_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/flag.py` & `getstream-0.4.0/getstream/chat/models/flag.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/flag_feedback.py` & `getstream-0.4.0/getstream/chat/models/flag_feedback.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/flag_message_details.py` & `getstream-0.4.0/getstream/chat/models/flag_message_details.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/flag_request.py` & `getstream-0.4.0/getstream/chat/models/flag_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_block_list_response.py` & `getstream-0.4.0/getstream/chat/models/get_block_list_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_call_token_request.py` & `getstream-0.4.0/getstream/chat/models/get_call_token_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_call_token_response.py` & `getstream-0.4.0/getstream/chat/models/get_call_token_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_command_response.py` & `getstream-0.4.0/getstream/chat/models/get_command_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_export_channels_status_response.py` & `getstream-0.4.0/getstream/chat/models/get_export_channels_status_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_import_response.py` & `getstream-0.4.0/getstream/chat/models/get_import_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_og_response.py` & `getstream-0.4.0/getstream/chat/models/get_og_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_rate_limits_response.py` & `getstream-0.4.0/getstream/chat/models/get_rate_limits_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/get_task_response.py` & `getstream-0.4.0/getstream/chat/models/get_task_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/guest_response.py` & `getstream-0.4.0/getstream/chat/models/guest_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/health_check_event.py` & `getstream-0.4.0/getstream/chat/models/health_check_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/hide_channel_request.py` & `getstream-0.4.0/getstream/chat/models/hide_channel_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/huawei_config_fields.py` & `getstream-0.4.0/getstream/chat/models/huawei_config_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/huawei_config_request.py` & `getstream-0.4.0/getstream/chat/models/huawei_config_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/image_data.py` & `getstream-0.4.0/getstream/chat/models/image_data.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/image_data_request.py` & `getstream-0.4.0/getstream/chat/models/image_data_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/image_size_request.py` & `getstream-0.4.0/getstream/chat/models/image_size_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/image_upload_request.py` & `getstream-0.4.0/getstream/chat/models/image_upload_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/image_upload_response.py` & `getstream-0.4.0/getstream/chat/models/image_upload_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/images.py` & `getstream-0.4.0/getstream/chat/models/images.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/images_request.py` & `getstream-0.4.0/getstream/chat/models/images_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/import_task.py` & `getstream-0.4.0/getstream/chat/models/import_task.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/import_task_history.py` & `getstream-0.4.0/getstream/chat/models/import_task_history.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/list_channel_types_response.py` & `getstream-0.4.0/getstream/chat/models/list_channel_types_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/list_push_providers_response.py` & `getstream-0.4.0/getstream/chat/models/list_push_providers_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mark_channels_read_request.py` & `getstream-0.4.0/getstream/chat/models/mark_channels_read_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mark_read_request.py` & `getstream-0.4.0/getstream/chat/models/mark_read_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mark_read_response.py` & `getstream-0.4.0/getstream/chat/models/mark_read_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mark_unread_request.py` & `getstream-0.4.0/getstream/chat/models/mark_unread_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/member_added_event.py` & `getstream-0.4.0/getstream/chat/models/member_added_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/member_removed_event.py` & `getstream-0.4.0/getstream/chat/models/member_removed_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/member_updated_event.py` & `getstream-0.4.0/getstream/chat/models/member_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message.py` & `getstream-0.4.0/getstream/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_action_request.py` & `getstream-0.4.0/getstream/chat/models/message_action_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_deleted_event.py` & `getstream-0.4.0/getstream/chat/models/message_deleted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_flag.py` & `getstream-0.4.0/getstream/chat/models/message_flag.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_flagged_event.py` & `getstream-0.4.0/getstream/chat/models/message_flagged_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_moderation_result.py` & `getstream-0.4.0/getstream/chat/models/message_moderation_result.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_new_event.py` & `getstream-0.4.0/getstream/chat/models/message_new_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_pagination_params_request.py` & `getstream-0.4.0/getstream/chat/models/message_pagination_params_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_read_event.py` & `getstream-0.4.0/getstream/chat/models/message_read_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_request.py` & `getstream-0.4.0/getstream/chat/models/message_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_request_1.py` & `getstream-0.4.0/getstream/chat/models/message_request_1.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_unblocked_event.py` & `getstream-0.4.0/getstream/chat/models/message_unblocked_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_updated_event.py` & `getstream-0.4.0/getstream/chat/models/message_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/message_with_pending_metadata_response.py` & `getstream-0.4.0/getstream/chat/models/message_with_pending_metadata_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/moderation_response.py` & `getstream-0.4.0/getstream/chat/models/moderation_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/moderation_response_request.py` & `getstream-0.4.0/getstream/chat/models/moderation_response_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mute_channel_request.py` & `getstream-0.4.0/getstream/chat/models/mute_channel_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mute_channel_response.py` & `getstream-0.4.0/getstream/chat/models/mute_channel_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mute_user_request.py` & `getstream-0.4.0/getstream/chat/models/mute_user_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/mute_user_response.py` & `getstream-0.4.0/getstream/chat/models/mute_user_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_added_to_channel_event.py` & `getstream-0.4.0/getstream/chat/models/notification_added_to_channel_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_channel_deleted_event.py` & `getstream-0.4.0/getstream/chat/models/notification_channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_channel_mutes_updated_event.py` & `getstream-0.4.0/getstream/chat/models/notification_channel_mutes_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_channel_truncated_event.py` & `getstream-0.4.0/getstream/chat/models/notification_channel_truncated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_invite_accepted_event.py` & `getstream-0.4.0/getstream/chat/models/notification_invite_accepted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_invite_rejected_event.py` & `getstream-0.4.0/getstream/chat/models/notification_invite_rejected_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_invited_event.py` & `getstream-0.4.0/getstream/chat/models/notification_invited_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_mark_read_event.py` & `getstream-0.4.0/getstream/chat/models/notification_mark_read_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_mark_unread_event.py` & `getstream-0.4.0/getstream/chat/models/notification_mark_unread_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_mutes_updated_event.py` & `getstream-0.4.0/getstream/chat/models/notification_mutes_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_new_message_event.py` & `getstream-0.4.0/getstream/chat/models/notification_new_message_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_removed_from_channel_event.py` & `getstream-0.4.0/getstream/chat/models/notification_removed_from_channel_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/notification_settings.py` & `getstream-0.4.0/getstream/chat/models/notification_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/own_user.py` & `getstream-0.4.0/getstream/chat/models/own_user.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/own_user_request.py` & `getstream-0.4.0/getstream/chat/models/own_user_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/pagination_params_request.py` & `getstream-0.4.0/getstream/chat/models/pagination_params_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/pending_message.py` & `getstream-0.4.0/getstream/chat/models/pending_message.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/permission.py` & `getstream-0.4.0/getstream/chat/models/permission.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/policy.py` & `getstream-0.4.0/getstream/chat/models/policy.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/policy_request.py` & `getstream-0.4.0/getstream/chat/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/policy_request_1.py` & `getstream-0.4.0/getstream/chat/models/policy_request_1.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/push_notification_fields.py` & `getstream-0.4.0/getstream/chat/models/push_notification_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/push_notification_settings.py` & `getstream-0.4.0/getstream/chat/models/push_notification_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/push_notification_settings_request.py` & `getstream-0.4.0/getstream/chat/models/push_notification_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/push_provider.py` & `getstream-0.4.0/getstream/chat/models/push_provider.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/push_provider_request.py` & `getstream-0.4.0/getstream/chat/models/push_provider_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/push_provider_response.py` & `getstream-0.4.0/getstream/chat/models/push_provider_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_banned_users_request.py` & `getstream-0.4.0/getstream/chat/models/query_banned_users_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_campaigns_request.py` & `getstream-0.4.0/getstream/chat/models/query_campaigns_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_campaigns_response.py` & `getstream-0.4.0/getstream/chat/models/query_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_channels_request.py` & `getstream-0.4.0/getstream/chat/models/query_channels_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_members_request.py` & `getstream-0.4.0/getstream/chat/models/query_members_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_message_flags_request.py` & `getstream-0.4.0/getstream/chat/models/query_message_flags_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_recipients_request.py` & `getstream-0.4.0/getstream/chat/models/query_recipients_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_recipients_response.py` & `getstream-0.4.0/getstream/chat/models/query_recipients_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_segments_request.py` & `getstream-0.4.0/getstream/chat/models/query_segments_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/query_users_request.py` & `getstream-0.4.0/getstream/chat/models/query_users_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reaction.py` & `getstream-0.4.0/getstream/chat/models/reaction.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reaction_deleted_event.py` & `getstream-0.4.0/getstream/chat/models/reaction_deleted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reaction_new_event.py` & `getstream-0.4.0/getstream/chat/models/reaction_new_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reaction_removal_response.py` & `getstream-0.4.0/getstream/chat/models/reaction_removal_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reaction_request.py` & `getstream-0.4.0/getstream/chat/models/reaction_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reaction_response.py` & `getstream-0.4.0/getstream/chat/models/reaction_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reaction_updated_event.py` & `getstream-0.4.0/getstream/chat/models/reaction_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reactivate_user_request.py` & `getstream-0.4.0/getstream/chat/models/reactivate_user_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/reactivate_users_request.py` & `getstream-0.4.0/getstream/chat/models/reactivate_users_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/read.py` & `getstream-0.4.0/getstream/chat/models/read.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/recipient.py` & `getstream-0.4.0/getstream/chat/models/recipient.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/resume_campaign_response.py` & `getstream-0.4.0/getstream/chat/models/resume_campaign_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/role.py` & `getstream-0.4.0/getstream/chat/models/role.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/schedule_campaign_response.py` & `getstream-0.4.0/getstream/chat/models/schedule_campaign_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/search_request.py` & `getstream-0.4.0/getstream/chat/models/search_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/search_response.py` & `getstream-0.4.0/getstream/chat/models/search_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/search_result_message.py` & `getstream-0.4.0/getstream/chat/models/search_result_message.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/search_warning.py` & `getstream-0.4.0/getstream/chat/models/search_warning.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/segment.py` & `getstream-0.4.0/getstream/chat/models/segment.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/segment_data_request.py` & `getstream-0.4.0/getstream/chat/models/segment_data_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/segment_updateable_fields_request.py` & `getstream-0.4.0/getstream/chat/models/segment_updateable_fields_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/send_message_request.py` & `getstream-0.4.0/getstream/chat/models/send_message_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/send_reaction_request.py` & `getstream-0.4.0/getstream/chat/models/send_reaction_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/show_channel_request.py` & `getstream-0.4.0/getstream/chat/models/show_channel_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/stop_campaign_response.py` & `getstream-0.4.0/getstream/chat/models/stop_campaign_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/sync_request.py` & `getstream-0.4.0/getstream/chat/models/sync_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/sync_response.py` & `getstream-0.4.0/getstream/chat/models/sync_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/test_campaign_response.py` & `getstream-0.4.0/getstream/chat/models/test_campaign_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/thresholds.py` & `getstream-0.4.0/getstream/chat/models/thresholds.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/thresholds_request.py` & `getstream-0.4.0/getstream/chat/models/thresholds_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/truncate_channel_request.py` & `getstream-0.4.0/getstream/chat/models/truncate_channel_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/truncate_channel_response.py` & `getstream-0.4.0/getstream/chat/models/truncate_channel_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/typing_start_event.py` & `getstream-0.4.0/getstream/chat/models/typing_start_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/typing_stop_event.py` & `getstream-0.4.0/getstream/chat/models/typing_stop_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/unmute_channel_request.py` & `getstream-0.4.0/getstream/chat/models/unmute_channel_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/unmute_user_request.py` & `getstream-0.4.0/getstream/chat/models/unmute_user_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_app_request.py` & `getstream-0.4.0/getstream/chat/models/update_app_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_campaign_response.py` & `getstream-0.4.0/getstream/chat/models/update_campaign_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_channel_partial_request.py` & `getstream-0.4.0/getstream/chat/models/update_channel_partial_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_channel_partial_response.py` & `getstream-0.4.0/getstream/chat/models/update_channel_partial_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_channel_request.py` & `getstream-0.4.0/getstream/chat/models/update_channel_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_channel_response.py` & `getstream-0.4.0/getstream/chat/models/update_channel_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_channel_type_request.py` & `getstream-0.4.0/getstream/chat/models/update_channel_type_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_channel_type_response.py` & `getstream-0.4.0/getstream/chat/models/update_channel_type_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_command_request.py` & `getstream-0.4.0/getstream/chat/models/update_command_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_message_partial_request.py` & `getstream-0.4.0/getstream/chat/models/update_message_partial_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/update_message_request.py` & `getstream-0.4.0/getstream/chat/models/update_message_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/upsert_push_provider_response.py` & `getstream-0.4.0/getstream/chat/models/upsert_push_provider_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_banned_event.py` & `getstream-0.4.0/getstream/chat/models/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_custom_event_request.py` & `getstream-0.4.0/getstream/chat/models/user_custom_event_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_deactivated_event.py` & `getstream-0.4.0/getstream/chat/models/user_deactivated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_deleted_event.py` & `getstream-0.4.0/getstream/chat/models/user_deleted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_flagged_event.py` & `getstream-0.4.0/getstream/chat/models/user_flagged_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_mute.py` & `getstream-0.4.0/getstream/chat/models/user_mute.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_mute_request.py` & `getstream-0.4.0/getstream/chat/models/user_mute_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_muted_event.py` & `getstream-0.4.0/getstream/chat/models/user_muted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_object.py` & `getstream-0.4.0/getstream/chat/models/user_object.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_object_request.py` & `getstream-0.4.0/getstream/chat/models/user_object_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_presence_changed_event.py` & `getstream-0.4.0/getstream/chat/models/user_presence_changed_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_reactivated_event.py` & `getstream-0.4.0/getstream/chat/models/user_reactivated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_request.py` & `getstream-0.4.0/getstream/chat/models/user_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_response.py` & `getstream-0.4.0/getstream/chat/models/user_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_unbanned_event.py` & `getstream-0.4.0/getstream/chat/models/user_unbanned_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_unmuted_event.py` & `getstream-0.4.0/getstream/chat/models/user_unmuted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_unread_reminder_event.py` & `getstream-0.4.0/getstream/chat/models/user_unread_reminder_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_updated_event.py` & `getstream-0.4.0/getstream/chat/models/user_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_watching_start_event.py` & `getstream-0.4.0/getstream/chat/models/user_watching_start_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/user_watching_stop_event.py` & `getstream-0.4.0/getstream/chat/models/user_watching_stop_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/video_settings.py` & `getstream-0.4.0/getstream/chat/models/video_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/xiaomi_config_fields.py` & `getstream-0.4.0/getstream/chat/models/xiaomi_config_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/chat/models/xiaomi_config_request.py` & `getstream-0.4.0/getstream/chat/models/xiaomi_config_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/cli/create_token.py` & `getstream-0.4.0/getstream/cli/create_token.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/config.py` & `getstream-0.4.0/getstream/config.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/api_error.py` & `getstream-0.4.0/getstream/models/api_error.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/audio_settings.py` & `getstream-0.4.0/getstream/models/audio_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/audio_settings_request.py` & `getstream-0.4.0/getstream/models/audio_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/azure_request.py` & `getstream-0.4.0/getstream/models/azure_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/blocked_user_event.py` & `getstream-0.4.0/getstream/models/blocked_user_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/broadcast_settings_request.py` & `getstream-0.4.0/getstream/models/broadcast_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_accepted_event.py` & `getstream-0.4.0/getstream/models/call_accepted_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_created_event.py` & `getstream-0.4.0/getstream/models/call_created_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_ended_event.py` & `getstream-0.4.0/getstream/models/call_ended_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_hls_broadcasting_failed_event.py` & `getstream-0.4.0/getstream/models/call_hls_broadcasting_failed_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_hls_broadcasting_started_event.py` & `getstream-0.4.0/getstream/models/call_hls_broadcasting_started_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_hls_broadcasting_stopped_event.py` & `getstream-0.4.0/getstream/models/call_hls_broadcasting_stopped_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_live_started_event.py` & `getstream-0.4.0/getstream/models/call_live_started_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_member_added_event.py` & `getstream-0.4.0/getstream/models/call_member_added_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_member_removed_event.py` & `getstream-0.4.0/getstream/models/call_member_removed_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_member_updated_event.py` & `getstream-0.4.0/getstream/models/call_member_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_member_updated_permission_event.py` & `getstream-0.4.0/getstream/models/call_member_updated_permission_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_notification_event.py` & `getstream-0.4.0/getstream/models/call_notification_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_participant_response.py` & `getstream-0.4.0/getstream/models/call_participant_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_reaction_event.py` & `getstream-0.4.0/getstream/models/call_reaction_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_recording.py` & `getstream-0.4.0/getstream/models/call_recording.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_recording_failed_event.py` & `getstream-0.4.0/getstream/models/call_recording_failed_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_recording_ready_event.py` & `getstream-0.4.0/getstream/models/call_recording_ready_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_recording_started_event.py` & `getstream-0.4.0/getstream/models/call_recording_started_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_recording_stopped_event.py` & `getstream-0.4.0/getstream/models/call_recording_stopped_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_rejected_event.py` & `getstream-0.4.0/getstream/models/call_rejected_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_request.py` & `getstream-0.4.0/getstream/models/call_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_response.py` & `getstream-0.4.0/getstream/models/call_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_ring_event.py` & `getstream-0.4.0/getstream/models/call_ring_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_session_ended_event.py` & `getstream-0.4.0/getstream/models/call_session_ended_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_session_participant_joined_event.py` & `getstream-0.4.0/getstream/models/call_session_participant_joined_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_session_participant_left_event.py` & `getstream-0.4.0/getstream/models/call_session_participant_left_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_session_response.py` & `getstream-0.4.0/getstream/models/call_session_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_session_started_event.py` & `getstream-0.4.0/getstream/models/call_session_started_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_settings_request.py` & `getstream-0.4.0/getstream/models/call_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_settings_response.py` & `getstream-0.4.0/getstream/models/call_settings_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_state_response_fields.py` & `getstream-0.4.0/getstream/models/call_state_response_fields.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_transcription.py` & `getstream-0.4.0/getstream/models/call_transcription.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_type_response.py` & `getstream-0.4.0/getstream/models/call_type_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_updated_event.py` & `getstream-0.4.0/getstream/models/call_updated_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/call_user_muted.py` & `getstream-0.4.0/getstream/models/call_user_muted.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/connect_user_details_request.py` & `getstream-0.4.0/getstream/models/connect_user_details_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/connected_event.py` & `getstream-0.4.0/getstream/models/connected_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/connection_error_event.py` & `getstream-0.4.0/getstream/models/connection_error_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/create_call_type_request.py` & `getstream-0.4.0/getstream/models/create_call_type_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/create_call_type_response.py` & `getstream-0.4.0/getstream/models/create_call_type_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/create_device_request.py` & `getstream-0.4.0/getstream/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/create_external_storage_request.py` & `getstream-0.4.0/getstream/models/create_external_storage_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/create_guest_response.py` & `getstream-0.4.0/getstream/models/create_guest_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/credentials.py` & `getstream-0.4.0/getstream/models/credentials.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/custom_video_event.py` & `getstream-0.4.0/getstream/models/custom_video_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/device.py` & `getstream-0.4.0/getstream/models/device.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/edge_response.py` & `getstream-0.4.0/getstream/models/edge_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/egress_response.py` & `getstream-0.4.0/getstream/models/egress_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/event_notification_settings_request.py` & `getstream-0.4.0/getstream/models/event_notification_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/get_call_response.py` & `getstream-0.4.0/getstream/models/get_call_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/get_call_type_response.py` & `getstream-0.4.0/getstream/models/get_call_type_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/get_or_create_call_request.py` & `getstream-0.4.0/getstream/models/get_or_create_call_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/get_or_create_call_response.py` & `getstream-0.4.0/getstream/models/get_or_create_call_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/go_live_request.py` & `getstream-0.4.0/getstream/models/go_live_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/health_check_event.py` & `getstream-0.4.0/getstream/models/health_check_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/hls_settings_request.py` & `getstream-0.4.0/getstream/models/hls_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/hls_settings_response.py` & `getstream-0.4.0/getstream/models/hls_settings_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/join_call_request.py` & `getstream-0.4.0/getstream/models/join_call_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/join_call_response.py` & `getstream-0.4.0/getstream/models/join_call_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/layout_settings.py` & `getstream-0.4.0/getstream/models/layout_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/layout_settings_request.py` & `getstream-0.4.0/getstream/models/layout_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/list_call_type_response.py` & `getstream-0.4.0/getstream/models/list_call_type_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/list_external_storage_response.py` & `getstream-0.4.0/getstream/models/list_external_storage_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/list_transcriptions_response.py` & `getstream-0.4.0/getstream/models/list_transcriptions_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/member_request.py` & `getstream-0.4.0/getstream/models/member_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/member_response.py` & `getstream-0.4.0/getstream/models/member_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/mute_users_request.py` & `getstream-0.4.0/getstream/models/mute_users_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/notification_settings.py` & `getstream-0.4.0/getstream/models/notification_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/notification_settings_request.py` & `getstream-0.4.0/getstream/models/notification_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/own_user_response.py` & `getstream-0.4.0/getstream/models/own_user_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/permission_request_event.py` & `getstream-0.4.0/getstream/models/permission_request_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/query_calls_request.py` & `getstream-0.4.0/getstream/models/query_calls_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/query_calls_response.py` & `getstream-0.4.0/getstream/models/query_calls_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/query_members_request.py` & `getstream-0.4.0/getstream/models/query_members_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/query_members_response.py` & `getstream-0.4.0/getstream/models/query_members_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/reaction_response.py` & `getstream-0.4.0/getstream/models/reaction_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/record_settings_request.py` & `getstream-0.4.0/getstream/models/record_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/record_settings_response.py` & `getstream-0.4.0/getstream/models/record_settings_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/ring_settings_request.py` & `getstream-0.4.0/getstream/models/ring_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/s_3_request.py` & `getstream-0.4.0/getstream/models/s_3_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/screensharing_settings_request.py` & `getstream-0.4.0/getstream/models/screensharing_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/send_reaction_request.py` & `getstream-0.4.0/getstream/models/send_reaction_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/target_resolution_request.py` & `getstream-0.4.0/getstream/models/target_resolution_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/unblocked_user_event.py` & `getstream-0.4.0/getstream/models/unblocked_user_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_call_members_request.py` & `getstream-0.4.0/getstream/models/update_call_members_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_call_request.py` & `getstream-0.4.0/getstream/models/update_call_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_call_response.py` & `getstream-0.4.0/getstream/models/update_call_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_call_type_request.py` & `getstream-0.4.0/getstream/models/update_call_type_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_call_type_response.py` & `getstream-0.4.0/getstream/models/update_call_type_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_external_storage_request.py` & `getstream-0.4.0/getstream/models/update_external_storage_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_external_storage_response.py` & `getstream-0.4.0/getstream/models/update_external_storage_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/update_user_permissions_request.py` & `getstream-0.4.0/getstream/models/update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/updated_call_permissions_event.py` & `getstream-0.4.0/getstream/models/updated_call_permissions_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/user_request.py` & `getstream-0.4.0/getstream/models/user_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/user_response.py` & `getstream-0.4.0/getstream/models/user_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/video_event.py` & `getstream-0.4.0/getstream/models/video_event.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/video_settings.py` & `getstream-0.4.0/getstream/models/video_settings.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/video_settings_request.py` & `getstream-0.4.0/getstream/models/video_settings_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/models/ws_auth_message_request.py` & `getstream-0.4.0/getstream/models/ws_auth_message_request.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/rate_limit.py` & `getstream-0.4.0/getstream/rate_limit.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/stream_response.py` & `getstream-0.4.0/getstream/stream_response.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/sync/base.py` & `getstream-0.4.0/getstream/sync/base.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/sync/stream.py` & `getstream-0.4.0/getstream/sync/stream.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/users/sync/client.py` & `getstream-0.4.0/getstream/users/sync/client.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/utils.py` & `getstream-0.4.0/getstream/utils.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/video/exceptions.py` & `getstream-0.4.0/getstream/video/exceptions.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/video/sync/base_client.py` & `getstream-0.4.0/getstream/video/sync/base_client.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/getstream/video/sync/client.py` & `getstream-0.4.0/getstream/video/sync/client.py`

 * *Files identical despite different names*

### Comparing `getstream-0.3.0/pyproject.toml` & `getstream-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getstream"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["sachaarbonel <sacha.arbonel@hotmail.fr>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 httpx = "^0.19.0"
```

### Comparing `getstream-0.3.0/PKG-INFO` & `getstream-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getstream
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: sachaarbonel
 Author-email: sacha.arbonel@hotmail.fr
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

