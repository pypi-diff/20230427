# Comparing `tmp/mux_python-3.8.0.tar.gz` & `tmp/mux_python-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mux_python-3.8.0.tar", last modified: Fri Jan 13 15:43:46 2023, max compression
+gzip compressed data, was "mux_python-3.9.0.tar", last modified: Wed Feb 22 21:19:34 2023, max compression
```

## Comparing `mux_python-3.8.0.tar` & `mux_python-3.9.0.tar`

### file list

```diff
@@ -1,342 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:43:46.518855 mux_python-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-13 15:43:10.000000 mux_python-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-01-13 15:43:46.518855 mux_python-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-01-13 15:43:10.000000 mux_python-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:43:46.482853 mux_python-3.8.0/mux_python/
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:43:46.482853 mux_python-3.8.0/mux_python/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89509 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/assets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/delivery_usage_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/dimensions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25607 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/direct_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/errors_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/filters_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/incidents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   121963 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/live_streams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47577 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/metrics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36071 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/monitoring_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/playback_id_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34265 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/playback_restrictions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36605 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/real_time_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60170 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/spaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36121 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/transcription_vocabularies_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/url_signing_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api/video_views_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27525 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:43:46.498854 mux_python-3.8.0/mux_python/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/abridged_video_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    27679 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset_master.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset_non_standard_input_reasons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset_recording_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset_static_renditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/asset_static_renditions_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/breakdown_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/broadcast_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/broadcast_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/broadcast_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/broadcast_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_asset_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_broadcast_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_live_stream_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_playback_id_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_playback_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_playback_restriction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_simulcast_target_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_space_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_track_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_track_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_transcription_vocabulary_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/create_upload_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/dimension_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/disable_live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/enable_live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/export_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/export_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/filter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_asset_input_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_asset_or_live_stream_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_asset_or_live_stream_id_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_asset_or_live_stream_id_response_data_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_asset_playback_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_live_stream_playback_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_metric_timeseries_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_monitoring_breakdown_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_monitoring_histogram_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_monitoring_histogram_timeseries_response_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_monitoring_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_overall_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_real_time_breakdown_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_real_time_histogram_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_real_time_histogram_timeseries_response_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/get_real_time_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/incident_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/incident_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/incident_notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/incident_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/input_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/input_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/input_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/input_settings_overlay_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/input_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_all_metric_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_assets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_breakdown_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_delivery_usage_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_dimension_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_dimensions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_errors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_exports_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_filter_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_filters_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_filters_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_incidents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_insights_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_live_streams_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_monitoring_dimensions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_monitoring_dimensions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_monitoring_metrics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_playback_restrictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_real_time_dimensions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_real_time_metrics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_related_incidents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_signing_keys_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_spaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_transcription_vocabularies_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_video_view_exports_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/list_video_views_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    31798 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/live_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/live_stream_embedded_subtitle_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/live_stream_generated_subtitle_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/live_stream_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/monitoring_breakdown_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/monitoring_histogram_timeseries_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/monitoring_histogram_timeseries_bucket_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/monitoring_histogram_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/monitoring_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/overall_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/playback_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/playback_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/playback_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/playback_restriction_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/real_time_breakdown_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/real_time_histogram_timeseries_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/real_time_histogram_timeseries_bucket_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/real_time_histogram_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/real_time_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/referrer_domain_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/signal_live_stream_complete_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/signing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/signing_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/simulcast_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/simulcast_target_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/space_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/space_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/space_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/start_space_broadcast_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/stop_space_broadcast_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21077 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/transcription_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/transcription_vocabulary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_asset_master_access_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_asset_mp4_support_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_asset_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_live_stream_embedded_subtitles_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_live_stream_generated_subtitles_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_live_stream_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_referrer_domain_restriction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/update_transcription_vocabulary_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/upload_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)   101240 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/video_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/video_view_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/models/video_view_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-01-13 15:43:10.000000 mux_python-3.8.0/mux_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:43:46.482853 mux_python-3.8.0/mux_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-01-13 15:43:46.000000 mux_python-3.8.0/mux_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-01-13 15:43:46.000000 mux_python-3.8.0/mux_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 15:43:46.000000 mux_python-3.8.0/mux_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-13 15:43:46.000000 mux_python-3.8.0/mux_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-13 15:43:46.000000 mux_python-3.8.0/mux_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-13 15:43:46.518855 mux_python-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-01-13 15:43:10.000000 mux_python-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:43:46.518855 mux_python-3.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_abridged_video_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset_non_standard_input_reasons.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset_recording_times.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset_static_renditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_asset_static_renditions_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_assets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_breakdown_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_broadcast_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_broadcast_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_broadcast_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_broadcast_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_asset_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_broadcast_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_live_stream_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_playback_id_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_playback_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_playback_restriction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_simulcast_target_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_space_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_track_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_track_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_transcription_vocabulary_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_create_upload_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_delivery_usage_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_dimension_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_dimensions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_direct_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_disable_live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_enable_live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_errors_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_export_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_export_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_filter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_filters_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_asset_input_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_asset_or_live_stream_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_asset_or_live_stream_id_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_asset_or_live_stream_id_response_data_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_asset_playback_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_live_stream_playback_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_metric_timeseries_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_monitoring_breakdown_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_monitoring_histogram_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_monitoring_histogram_timeseries_response_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_monitoring_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_overall_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_real_time_breakdown_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_real_time_histogram_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_real_time_histogram_timeseries_response_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_get_real_time_timeseries_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_incident.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_incident_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_incident_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_incident_notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_incident_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_incidents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_input_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_input_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_input_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_input_settings_overlay_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_input_track.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_all_metric_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_assets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_breakdown_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_delivery_usage_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_dimension_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_dimensions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_errors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_exports_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_filter_values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_filters_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_filters_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_incidents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_insights_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_live_streams_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_monitoring_dimensions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_monitoring_dimensions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_monitoring_metrics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_playback_restrictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_real_time_dimensions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_real_time_dimensions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_real_time_metrics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_related_incidents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_signing_keys_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_spaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_transcription_vocabularies_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_video_view_exports_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_list_video_views_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_live_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_live_stream_embedded_subtitle_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_live_stream_generated_subtitle_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_live_stream_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_live_streams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_metrics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_monitoring_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_monitoring_breakdown_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_monitoring_histogram_timeseries_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_monitoring_histogram_timeseries_bucket_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_monitoring_histogram_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_monitoring_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_overall_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_playback_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_playback_id_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_playback_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_playback_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_playback_restriction_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_playback_restrictions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_real_time_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_real_time_breakdown_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_real_time_histogram_timeseries_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_real_time_histogram_timeseries_bucket_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_real_time_histogram_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_real_time_timeseries_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_referrer_domain_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_score.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_signal_live_stream_complete_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_signing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_signing_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_simulcast_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_simulcast_target_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_space_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_space_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_space_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_spaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_start_space_broadcast_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_stop_space_broadcast_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_transcription_vocabularies_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_transcription_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_transcription_vocabulary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_asset_master_access_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_asset_mp4_support_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_asset_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_live_stream_embedded_subtitles_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_live_stream_generated_subtitles_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_live_stream_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_referrer_domain_restriction_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_update_transcription_vocabulary_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_upload_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_url_signing_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_video_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_video_view_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_video_view_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-13 15:43:10.000000 mux_python-3.8.0/test/test_video_views_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 21:19:34.440383 mux_python-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-22 21:18:54.000000 mux_python-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-02-22 21:19:34.440383 mux_python-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-02-22 21:18:54.000000 mux_python-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 21:19:34.392383 mux_python-3.9.0/mux_python/
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 21:19:34.396383 mux_python-3.9.0/mux_python/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89509 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/assets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/delivery_usage_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/dimensions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25607 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/direct_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/errors_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/filters_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/incidents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121963 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/live_streams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47577 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/metrics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36071 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/monitoring_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/playback_id_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34265 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/playback_restrictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36605 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/real_time_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60170 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/spaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36121 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/transcription_vocabularies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/url_signing_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api/video_views_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27525 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 21:19:34.416383 mux_python-3.9.0/mux_python/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/abridged_video_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27679 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset_non_standard_input_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset_recording_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset_static_renditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/asset_static_renditions_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/breakdown_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/broadcast_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/broadcast_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/broadcast_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/broadcast_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_broadcast_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_live_stream_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_playback_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_playback_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_playback_restriction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_simulcast_target_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_space_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_track_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_track_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_transcription_vocabulary_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/create_upload_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/delivery_report_delivered_seconds_by_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/dimension_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/disable_live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/enable_live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/export_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/export_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/filter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_asset_input_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_asset_or_live_stream_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_asset_or_live_stream_id_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_asset_or_live_stream_id_response_data_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_asset_playback_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_live_stream_playback_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_metric_timeseries_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_monitoring_breakdown_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_monitoring_histogram_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_monitoring_histogram_timeseries_response_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_monitoring_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_overall_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_real_time_breakdown_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_real_time_histogram_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_real_time_histogram_timeseries_response_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/get_real_time_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/incident_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/incident_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/incident_notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/incident_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/input_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/input_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/input_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/input_settings_overlay_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/input_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_all_metric_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_assets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_breakdown_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_delivery_usage_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_dimension_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_dimensions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_errors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_exports_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_filter_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_filters_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_filters_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_incidents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_insights_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_live_streams_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_monitoring_dimensions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_monitoring_dimensions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_monitoring_metrics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_playback_restrictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_real_time_dimensions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_real_time_metrics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_related_incidents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_signing_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_spaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_transcription_vocabularies_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_video_view_exports_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/list_video_views_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31798 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/live_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/live_stream_embedded_subtitle_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/live_stream_generated_subtitle_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/live_stream_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/monitoring_breakdown_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/monitoring_histogram_timeseries_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/monitoring_histogram_timeseries_bucket_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/monitoring_histogram_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/monitoring_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/overall_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/playback_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/playback_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/playback_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/playback_restriction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/real_time_breakdown_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/real_time_histogram_timeseries_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/real_time_histogram_timeseries_bucket_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/real_time_histogram_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/real_time_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/referrer_domain_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/signal_live_stream_complete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/signing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/signing_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/simulcast_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/simulcast_target_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/space_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/space_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/space_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/start_space_broadcast_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/stop_space_broadcast_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/transcription_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/transcription_vocabulary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_asset_master_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_asset_mp4_support_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_live_stream_embedded_subtitles_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_live_stream_generated_subtitles_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_live_stream_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_referrer_domain_restriction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/update_transcription_vocabulary_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/upload_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101240 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/video_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/video_view_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/models/video_view_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-02-22 21:18:54.000000 mux_python-3.9.0/mux_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 21:19:34.392383 mux_python-3.9.0/mux_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-02-22 21:19:34.000000 mux_python-3.9.0/mux_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-02-22 21:19:34.000000 mux_python-3.9.0/mux_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 21:19:34.000000 mux_python-3.9.0/mux_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-22 21:19:34.000000 mux_python-3.9.0/mux_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 21:19:34.000000 mux_python-3.9.0/mux_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-22 21:19:34.440383 mux_python-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-02-22 21:18:54.000000 mux_python-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 21:19:34.440383 mux_python-3.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_abridged_video_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset_non_standard_input_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset_recording_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset_static_renditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_asset_static_renditions_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_assets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_breakdown_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_broadcast_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_broadcast_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_broadcast_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_broadcast_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_broadcast_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_live_stream_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_playback_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_playback_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_playback_restriction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_simulcast_target_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_space_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_track_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_track_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_transcription_vocabulary_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_create_upload_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_delivery_report_delivered_seconds_by_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_delivery_usage_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_dimension_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_dimensions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_direct_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_disable_live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_enable_live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_errors_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_export_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_export_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_filter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_filters_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_asset_input_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_asset_or_live_stream_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_asset_or_live_stream_id_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_asset_or_live_stream_id_response_data_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_asset_playback_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_live_stream_playback_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_metric_timeseries_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_monitoring_breakdown_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_monitoring_histogram_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_monitoring_histogram_timeseries_response_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_monitoring_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_overall_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_real_time_breakdown_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_real_time_histogram_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_real_time_histogram_timeseries_response_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_get_real_time_timeseries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_incident_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_incident_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_incident_notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_incident_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_incidents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_input_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_input_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_input_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_input_settings_overlay_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_input_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_all_metric_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_assets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_breakdown_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_delivery_usage_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_dimension_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_dimensions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_errors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_exports_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_filter_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_filters_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_filters_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_incidents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_insights_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_live_streams_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_monitoring_dimensions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_monitoring_dimensions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_monitoring_metrics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_playback_restrictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_real_time_dimensions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_real_time_dimensions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_real_time_metrics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_related_incidents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_signing_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_spaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_transcription_vocabularies_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_video_view_exports_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_list_video_views_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_live_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_live_stream_embedded_subtitle_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_live_stream_generated_subtitle_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_live_stream_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_live_streams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_metrics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_monitoring_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_monitoring_breakdown_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_monitoring_histogram_timeseries_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_monitoring_histogram_timeseries_bucket_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_monitoring_histogram_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_monitoring_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_overall_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_playback_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_playback_id_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_playback_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_playback_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_playback_restriction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_playback_restrictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_real_time_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_real_time_breakdown_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_real_time_histogram_timeseries_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_real_time_histogram_timeseries_bucket_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_real_time_histogram_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_real_time_timeseries_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_referrer_domain_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_signal_live_stream_complete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_signing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_signing_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_simulcast_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_simulcast_target_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_space_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_space_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_space_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_spaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_start_space_broadcast_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_stop_space_broadcast_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_transcription_vocabularies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_transcription_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_transcription_vocabulary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_asset_master_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_asset_mp4_support_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_live_stream_embedded_subtitles_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_live_stream_generated_subtitles_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_live_stream_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_referrer_domain_restriction_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_update_transcription_vocabulary_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_upload_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_url_signing_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_video_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_video_view_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_video_view_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-22 21:18:54.000000 mux_python-3.9.0/test/test_video_views_api.py
```

### Comparing `mux_python-3.8.0/LICENSE` & `mux_python-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/PKG-INFO` & `mux_python-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mux_python
-Version: 3.8.0
+Version: 3.9.0
 Summary: Mux API
 Home-page: https://github.com/muxinc/mux-python
 Author: Mux DevEx
 Author-email: devex@mux.com
 Keywords: OpenAPI,OpenAPI-Generator,Mux API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mux_python Version: 3.8.0 Summary: Mux API Home-
+Metadata-Version: 2.1 Name: mux_python Version: 3.9.0 Summary: Mux API Home-
 page: https://github.com/muxinc/mux-python Author: Mux DevEx Author-email:
 devex@mux.com Keywords: OpenAPI,OpenAPI-Generator,Mux API Description-Content-
 Type: text/markdown License-File: LICENSE ![Mux Python Banner](github-python-
 sdk.png)
   [https://img.shields.io/pypi/v/mux_python] [https://github.com/muxinc/mux-
                 python/workflows/Integration%20Test/badge.svg]
                       PyPI | Mux_Docs | Mux_API_Reference
```

### Comparing `mux_python-3.8.0/README.md` & `mux_python-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/__init__.py` & `mux_python-3.9.0/mux_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: devex@mux.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "3.8.0"
+__version__ = "3.9.0"
 
 # import apis into sdk package
 from mux_python.api.assets_api import AssetsApi
 from mux_python.api.delivery_usage_api import DeliveryUsageApi
 from mux_python.api.dimensions_api import DimensionsApi
 from mux_python.api.direct_uploads_api import DirectUploadsApi
 from mux_python.api.errors_api import ErrorsApi
@@ -71,14 +71,15 @@
 from mux_python.models.create_simulcast_target_request import CreateSimulcastTargetRequest
 from mux_python.models.create_space_request import CreateSpaceRequest
 from mux_python.models.create_track_request import CreateTrackRequest
 from mux_python.models.create_track_response import CreateTrackResponse
 from mux_python.models.create_transcription_vocabulary_request import CreateTranscriptionVocabularyRequest
 from mux_python.models.create_upload_request import CreateUploadRequest
 from mux_python.models.delivery_report import DeliveryReport
+from mux_python.models.delivery_report_delivered_seconds_by_resolution import DeliveryReportDeliveredSecondsByResolution
 from mux_python.models.dimension_value import DimensionValue
 from mux_python.models.disable_live_stream_response import DisableLiveStreamResponse
 from mux_python.models.enable_live_stream_response import EnableLiveStreamResponse
 from mux_python.models.error import Error
 from mux_python.models.export_date import ExportDate
 from mux_python.models.export_file import ExportFile
 from mux_python.models.filter_value import FilterValue
```

### Comparing `mux_python-3.8.0/mux_python/api/__init__.py` & `mux_python-3.9.0/mux_python/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/assets_api.py` & `mux_python-3.9.0/mux_python/api/assets_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/delivery_usage_api.py` & `mux_python-3.9.0/mux_python/api/delivery_usage_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/dimensions_api.py` & `mux_python-3.9.0/mux_python/api/dimensions_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/direct_uploads_api.py` & `mux_python-3.9.0/mux_python/api/direct_uploads_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/errors_api.py` & `mux_python-3.9.0/mux_python/api/errors_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/exports_api.py` & `mux_python-3.9.0/mux_python/api/exports_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/filters_api.py` & `mux_python-3.9.0/mux_python/api/filters_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/incidents_api.py` & `mux_python-3.9.0/mux_python/api/incidents_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/live_streams_api.py` & `mux_python-3.9.0/mux_python/api/live_streams_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/metrics_api.py` & `mux_python-3.9.0/mux_python/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/monitoring_api.py` & `mux_python-3.9.0/mux_python/api/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/playback_id_api.py` & `mux_python-3.9.0/mux_python/api/playback_id_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/playback_restrictions_api.py` & `mux_python-3.9.0/mux_python/api/playback_restrictions_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/real_time_api.py` & `mux_python-3.9.0/mux_python/api/real_time_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/spaces_api.py` & `mux_python-3.9.0/mux_python/api/spaces_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/transcription_vocabularies_api.py` & `mux_python-3.9.0/mux_python/api/transcription_vocabularies_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/url_signing_keys_api.py` & `mux_python-3.9.0/mux_python/api/url_signing_keys_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api/video_views_api.py` & `mux_python-3.9.0/mux_python/api/video_views_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/api_client.py` & `mux_python-3.9.0/mux_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.8.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.9.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `mux_python-3.8.0/mux_python/configuration.py` & `mux_python-3.9.0/mux_python/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 3.8.0".\
+               "SDK Package Version: 3.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `mux_python-3.8.0/mux_python/exceptions.py` & `mux_python-3.9.0/mux_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/__init__.py` & `mux_python-3.9.0/mux_python/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from mux_python.models.create_simulcast_target_request import CreateSimulcastTargetRequest
 from mux_python.models.create_space_request import CreateSpaceRequest
 from mux_python.models.create_track_request import CreateTrackRequest
 from mux_python.models.create_track_response import CreateTrackResponse
 from mux_python.models.create_transcription_vocabulary_request import CreateTranscriptionVocabularyRequest
 from mux_python.models.create_upload_request import CreateUploadRequest
 from mux_python.models.delivery_report import DeliveryReport
+from mux_python.models.delivery_report_delivered_seconds_by_resolution import DeliveryReportDeliveredSecondsByResolution
 from mux_python.models.dimension_value import DimensionValue
 from mux_python.models.disable_live_stream_response import DisableLiveStreamResponse
 from mux_python.models.enable_live_stream_response import EnableLiveStreamResponse
 from mux_python.models.error import Error
 from mux_python.models.export_date import ExportDate
 from mux_python.models.export_file import ExportFile
 from mux_python.models.filter_value import FilterValue
```

### Comparing `mux_python-3.8.0/mux_python/models/abridged_video_view.py` & `mux_python-3.9.0/mux_python/models/abridged_video_view.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset.py` & `mux_python-3.9.0/mux_python/models/asset.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset_errors.py` & `mux_python-3.9.0/mux_python/models/asset_errors.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset_master.py` & `mux_python-3.9.0/mux_python/models/asset_master.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset_non_standard_input_reasons.py` & `mux_python-3.9.0/mux_python/models/asset_non_standard_input_reasons.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset_recording_times.py` & `mux_python-3.9.0/mux_python/models/asset_recording_times.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset_response.py` & `mux_python-3.9.0/mux_python/models/asset_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset_static_renditions.py` & `mux_python-3.9.0/mux_python/models/asset_static_renditions.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/asset_static_renditions_files.py` & `mux_python-3.9.0/mux_python/models/asset_static_renditions_files.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/breakdown_value.py` & `mux_python-3.9.0/mux_python/models/breakdown_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/broadcast.py` & `mux_python-3.9.0/mux_python/models/broadcast.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/broadcast_layout.py` & `mux_python-3.9.0/mux_python/models/broadcast_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     """
 
     """
     allowed enum values
     """
     GALLERY = "gallery"
     ACTIVE_SPEAKER = "active-speaker"
+    CROP = "crop"
 
-    allowable_values = [GALLERY, ACTIVE_SPEAKER]  # noqa: E501
+    allowable_values = [GALLERY, ACTIVE_SPEAKER, CROP]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `mux_python-3.8.0/mux_python/models/broadcast_resolution.py` & `mux_python-3.9.0/mux_python/models/broadcast_resolution.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/broadcast_response.py` & `mux_python-3.9.0/mux_python/models/broadcast_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/broadcast_status.py` & `mux_python-3.9.0/mux_python/models/broadcast_status.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_asset_request.py` & `mux_python-3.9.0/mux_python/models/create_asset_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_broadcast_request.py` & `mux_python-3.9.0/mux_python/models/create_broadcast_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_live_stream_request.py` & `mux_python-3.9.0/mux_python/models/create_live_stream_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_playback_id_request.py` & `mux_python-3.9.0/mux_python/models/create_playback_id_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_playback_id_response.py` & `mux_python-3.9.0/mux_python/models/create_playback_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_playback_restriction_request.py` & `mux_python-3.9.0/mux_python/models/create_playback_restriction_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_simulcast_target_request.py` & `mux_python-3.9.0/mux_python/models/create_simulcast_target_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_space_request.py` & `mux_python-3.9.0/mux_python/models/create_space_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_track_request.py` & `mux_python-3.9.0/mux_python/models/create_track_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_track_response.py` & `mux_python-3.9.0/mux_python/models/create_track_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_transcription_vocabulary_request.py` & `mux_python-3.9.0/mux_python/models/create_transcription_vocabulary_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/create_upload_request.py` & `mux_python-3.9.0/mux_python/models/create_upload_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/delivery_report.py` & `mux_python-3.9.0/mux_python/models/delivery_report.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,42 +40,45 @@
         'live_stream_id': 'str',
         'asset_id': 'str',
         'passthrough': 'str',
         'created_at': 'str',
         'deleted_at': 'str',
         'asset_state': 'str',
         'asset_duration': 'float',
-        'delivered_seconds': 'float'
+        'delivered_seconds': 'float',
+        'delivered_seconds_by_resolution': 'DeliveryReportDeliveredSecondsByResolution'
     }
 
     attribute_map = {
         'live_stream_id': 'live_stream_id',
         'asset_id': 'asset_id',
         'passthrough': 'passthrough',
         'created_at': 'created_at',
         'deleted_at': 'deleted_at',
         'asset_state': 'asset_state',
         'asset_duration': 'asset_duration',
-        'delivered_seconds': 'delivered_seconds'
+        'delivered_seconds': 'delivered_seconds',
+        'delivered_seconds_by_resolution': 'delivered_seconds_by_resolution'
     }
 
-    def __init__(self, live_stream_id=None, asset_id=None, passthrough=None, created_at=None, deleted_at=None, asset_state=None, asset_duration=None, delivered_seconds=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, live_stream_id=None, asset_id=None, passthrough=None, created_at=None, deleted_at=None, asset_state=None, asset_duration=None, delivered_seconds=None, delivered_seconds_by_resolution=None, local_vars_configuration=None):  # noqa: E501
         """DeliveryReport - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._live_stream_id = None
         self._asset_id = None
         self._passthrough = None
         self._created_at = None
         self._deleted_at = None
         self._asset_state = None
         self._asset_duration = None
         self._delivered_seconds = None
+        self._delivered_seconds_by_resolution = None
         self.discriminator = None
 
         if live_stream_id is not None:
             self.live_stream_id = live_stream_id
         if asset_id is not None:
             self.asset_id = asset_id
         if passthrough is not None:
@@ -86,14 +89,16 @@
             self.deleted_at = deleted_at
         if asset_state is not None:
             self.asset_state = asset_state
         if asset_duration is not None:
             self.asset_duration = asset_duration
         if delivered_seconds is not None:
             self.delivered_seconds = delivered_seconds
+        if delivered_seconds_by_resolution is not None:
+            self.delivered_seconds_by_resolution = delivered_seconds_by_resolution
 
     @property
     def live_stream_id(self):
         """Gets the live_stream_id of this DeliveryReport.  # noqa: E501
 
         Unique identifier for the live stream that created the asset.  # noqa: E501
 
@@ -277,14 +282,35 @@
 
         :param delivered_seconds: The delivered_seconds of this DeliveryReport.  # noqa: E501
         :type delivered_seconds: float
         """
 
         self._delivered_seconds = delivered_seconds
 
+    @property
+    def delivered_seconds_by_resolution(self):
+        """Gets the delivered_seconds_by_resolution of this DeliveryReport.  # noqa: E501
+
+
+        :return: The delivered_seconds_by_resolution of this DeliveryReport.  # noqa: E501
+        :rtype: DeliveryReportDeliveredSecondsByResolution
+        """
+        return self._delivered_seconds_by_resolution
+
+    @delivered_seconds_by_resolution.setter
+    def delivered_seconds_by_resolution(self, delivered_seconds_by_resolution):
+        """Sets the delivered_seconds_by_resolution of this DeliveryReport.
+
+
+        :param delivered_seconds_by_resolution: The delivered_seconds_by_resolution of this DeliveryReport.  # noqa: E501
+        :type delivered_seconds_by_resolution: DeliveryReportDeliveredSecondsByResolution
+        """
+
+        self._delivered_seconds_by_resolution = delivered_seconds_by_resolution
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `mux_python-3.8.0/mux_python/models/dimension_value.py` & `mux_python-3.9.0/mux_python/models/dimension_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/disable_live_stream_response.py` & `mux_python-3.9.0/mux_python/models/disable_live_stream_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/enable_live_stream_response.py` & `mux_python-3.9.0/mux_python/models/enable_live_stream_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/error.py` & `mux_python-3.9.0/mux_python/models/error.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/export_date.py` & `mux_python-3.9.0/mux_python/models/export_date.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/export_file.py` & `mux_python-3.9.0/mux_python/models/export_file.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/filter_value.py` & `mux_python-3.9.0/mux_python/models/filter_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_asset_input_info_response.py` & `mux_python-3.9.0/mux_python/models/get_asset_input_info_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_asset_or_live_stream_id_response.py` & `mux_python-3.9.0/mux_python/models/get_asset_or_live_stream_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_asset_or_live_stream_id_response_data.py` & `mux_python-3.9.0/mux_python/models/get_asset_or_live_stream_id_response_data.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_asset_or_live_stream_id_response_data_object.py` & `mux_python-3.9.0/mux_python/models/get_asset_or_live_stream_id_response_data_object.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_asset_playback_id_response.py` & `mux_python-3.9.0/mux_python/models/get_asset_playback_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_live_stream_playback_id_response.py` & `mux_python-3.9.0/mux_python/models/get_live_stream_playback_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_metric_timeseries_data_response.py` & `mux_python-3.9.0/mux_python/models/get_metric_timeseries_data_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_monitoring_breakdown_response.py` & `mux_python-3.9.0/mux_python/models/get_monitoring_breakdown_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_monitoring_histogram_timeseries_response.py` & `mux_python-3.9.0/mux_python/models/get_monitoring_histogram_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_monitoring_histogram_timeseries_response_meta.py` & `mux_python-3.9.0/mux_python/models/get_monitoring_histogram_timeseries_response_meta.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_monitoring_timeseries_response.py` & `mux_python-3.9.0/mux_python/models/get_monitoring_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_overall_values_response.py` & `mux_python-3.9.0/mux_python/models/get_overall_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_real_time_breakdown_response.py` & `mux_python-3.9.0/mux_python/models/get_real_time_breakdown_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_real_time_histogram_timeseries_response.py` & `mux_python-3.9.0/mux_python/models/get_real_time_histogram_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_real_time_histogram_timeseries_response_meta.py` & `mux_python-3.9.0/mux_python/models/get_real_time_histogram_timeseries_response_meta.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/get_real_time_timeseries_response.py` & `mux_python-3.9.0/mux_python/models/get_real_time_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/incident.py` & `mux_python-3.9.0/mux_python/models/incident.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/incident_breakdown.py` & `mux_python-3.9.0/mux_python/models/incident_breakdown.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/incident_notification.py` & `mux_python-3.9.0/mux_python/models/incident_notification.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/incident_notification_rule.py` & `mux_python-3.9.0/mux_python/models/incident_notification_rule.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/incident_response.py` & `mux_python-3.9.0/mux_python/models/incident_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/input_file.py` & `mux_python-3.9.0/mux_python/models/input_file.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/input_info.py` & `mux_python-3.9.0/mux_python/models/input_info.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/input_settings.py` & `mux_python-3.9.0/mux_python/models/input_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/input_settings_overlay_settings.py` & `mux_python-3.9.0/mux_python/models/input_settings_overlay_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/input_track.py` & `mux_python-3.9.0/mux_python/models/input_track.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/insight.py` & `mux_python-3.9.0/mux_python/models/insight.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_all_metric_values_response.py` & `mux_python-3.9.0/mux_python/models/list_all_metric_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_assets_response.py` & `mux_python-3.9.0/mux_python/models/list_assets_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_breakdown_values_response.py` & `mux_python-3.9.0/mux_python/models/list_breakdown_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_delivery_usage_response.py` & `mux_python-3.9.0/mux_python/models/list_delivery_usage_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_dimension_values_response.py` & `mux_python-3.9.0/mux_python/models/list_dimension_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_dimensions_response.py` & `mux_python-3.9.0/mux_python/models/list_dimensions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_errors_response.py` & `mux_python-3.9.0/mux_python/models/list_errors_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_exports_response.py` & `mux_python-3.9.0/mux_python/models/list_exports_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_filter_values_response.py` & `mux_python-3.9.0/mux_python/models/list_filter_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_filters_response.py` & `mux_python-3.9.0/mux_python/models/list_filters_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_filters_response_data.py` & `mux_python-3.9.0/mux_python/models/list_filters_response_data.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_incidents_response.py` & `mux_python-3.9.0/mux_python/models/list_incidents_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_insights_response.py` & `mux_python-3.9.0/mux_python/models/list_insights_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_live_streams_response.py` & `mux_python-3.9.0/mux_python/models/list_live_streams_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_monitoring_dimensions_response.py` & `mux_python-3.9.0/mux_python/models/list_monitoring_dimensions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_monitoring_dimensions_response_data.py` & `mux_python-3.9.0/mux_python/models/list_monitoring_dimensions_response_data.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_monitoring_metrics_response.py` & `mux_python-3.9.0/mux_python/models/list_monitoring_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_playback_restrictions_response.py` & `mux_python-3.9.0/mux_python/models/list_playback_restrictions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_real_time_dimensions_response.py` & `mux_python-3.9.0/mux_python/models/list_real_time_dimensions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_real_time_metrics_response.py` & `mux_python-3.9.0/mux_python/models/list_real_time_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_related_incidents_response.py` & `mux_python-3.9.0/mux_python/models/list_related_incidents_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_signing_keys_response.py` & `mux_python-3.9.0/mux_python/models/list_signing_keys_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_spaces_response.py` & `mux_python-3.9.0/mux_python/models/list_spaces_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_transcription_vocabularies_response.py` & `mux_python-3.9.0/mux_python/models/list_transcription_vocabularies_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_uploads_response.py` & `mux_python-3.9.0/mux_python/models/list_uploads_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_video_view_exports_response.py` & `mux_python-3.9.0/mux_python/models/list_video_view_exports_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/list_video_views_response.py` & `mux_python-3.9.0/mux_python/models/list_video_views_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/live_stream.py` & `mux_python-3.9.0/mux_python/models/live_stream.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/live_stream_embedded_subtitle_settings.py` & `mux_python-3.9.0/mux_python/models/live_stream_embedded_subtitle_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/live_stream_generated_subtitle_settings.py` & `mux_python-3.9.0/mux_python/models/live_stream_generated_subtitle_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/live_stream_response.py` & `mux_python-3.9.0/mux_python/models/live_stream_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/live_stream_status.py` & `mux_python-3.9.0/mux_python/models/live_stream_status.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/metric.py` & `mux_python-3.9.0/mux_python/models/metric.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/monitoring_breakdown_value.py` & `mux_python-3.9.0/mux_python/models/monitoring_breakdown_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/monitoring_histogram_timeseries_bucket.py` & `mux_python-3.9.0/mux_python/models/monitoring_histogram_timeseries_bucket.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/monitoring_histogram_timeseries_bucket_values.py` & `mux_python-3.9.0/mux_python/models/monitoring_histogram_timeseries_bucket_values.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/monitoring_histogram_timeseries_datapoint.py` & `mux_python-3.9.0/mux_python/models/monitoring_histogram_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/monitoring_timeseries_datapoint.py` & `mux_python-3.9.0/mux_python/models/monitoring_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/notification_rule.py` & `mux_python-3.9.0/mux_python/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/overall_values.py` & `mux_python-3.9.0/mux_python/models/overall_values.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/playback_id.py` & `mux_python-3.9.0/mux_python/models/playback_id.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/playback_policy.py` & `mux_python-3.9.0/mux_python/models/playback_policy.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/playback_restriction.py` & `mux_python-3.9.0/mux_python/models/playback_restriction.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/playback_restriction_response.py` & `mux_python-3.9.0/mux_python/models/playback_restriction_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/real_time_breakdown_value.py` & `mux_python-3.9.0/mux_python/models/real_time_breakdown_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/real_time_histogram_timeseries_bucket.py` & `mux_python-3.9.0/mux_python/models/real_time_histogram_timeseries_bucket.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/real_time_histogram_timeseries_bucket_values.py` & `mux_python-3.9.0/mux_python/models/real_time_histogram_timeseries_bucket_values.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/real_time_histogram_timeseries_datapoint.py` & `mux_python-3.9.0/mux_python/models/real_time_histogram_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/real_time_timeseries_datapoint.py` & `mux_python-3.9.0/mux_python/models/real_time_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/referrer_domain_restriction.py` & `mux_python-3.9.0/mux_python/models/referrer_domain_restriction.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/score.py` & `mux_python-3.9.0/mux_python/models/score.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/signal_live_stream_complete_response.py` & `mux_python-3.9.0/mux_python/models/signal_live_stream_complete_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/signing_key.py` & `mux_python-3.9.0/mux_python/models/signing_key.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/signing_key_response.py` & `mux_python-3.9.0/mux_python/models/signing_key_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/simulcast_target.py` & `mux_python-3.9.0/mux_python/models/simulcast_target.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/simulcast_target_response.py` & `mux_python-3.9.0/mux_python/models/simulcast_target_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/space.py` & `mux_python-3.9.0/mux_python/models/space.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/space_response.py` & `mux_python-3.9.0/mux_python/models/space_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/space_status.py` & `mux_python-3.9.0/mux_python/models/space_status.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/space_type.py` & `mux_python-3.9.0/mux_python/models/space_type.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/start_space_broadcast_response.py` & `mux_python-3.9.0/mux_python/models/start_space_broadcast_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/stop_space_broadcast_response.py` & `mux_python-3.9.0/mux_python/models/stop_space_broadcast_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/track.py` & `mux_python-3.9.0/mux_python/models/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,15 +482,15 @@
         """Sets the status of this Track.
 
         The status of the track. This parameter is only set for `text` type tracks.  # noqa: E501
 
         :param status: The status of this Track.  # noqa: E501
         :type status: str
         """
-        allowed_values = ["preparing", "ready", "errored"]  # noqa: E501
+        allowed_values = ["preparing", "ready", "errored", "deleted"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and status not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
                 .format(status, allowed_values)
             )
 
         self._status = status
```

### Comparing `mux_python-3.8.0/mux_python/models/transcription_vocabulary.py` & `mux_python-3.9.0/mux_python/models/transcription_vocabulary.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/transcription_vocabulary_response.py` & `mux_python-3.9.0/mux_python/models/transcription_vocabulary_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_asset_master_access_request.py` & `mux_python-3.9.0/mux_python/models/update_asset_master_access_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_asset_mp4_support_request.py` & `mux_python-3.9.0/mux_python/models/update_asset_mp4_support_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_asset_request.py` & `mux_python-3.9.0/mux_python/models/update_asset_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_live_stream_embedded_subtitles_request.py` & `mux_python-3.9.0/mux_python/models/update_live_stream_embedded_subtitles_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_live_stream_generated_subtitles_request.py` & `mux_python-3.9.0/mux_python/models/update_live_stream_generated_subtitles_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_live_stream_request.py` & `mux_python-3.9.0/mux_python/models/update_live_stream_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_referrer_domain_restriction_request.py` & `mux_python-3.9.0/mux_python/models/update_referrer_domain_restriction_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/update_transcription_vocabulary_request.py` & `mux_python-3.9.0/mux_python/models/update_transcription_vocabulary_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/upload.py` & `mux_python-3.9.0/mux_python/models/upload.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/upload_error.py` & `mux_python-3.9.0/mux_python/models/upload_error.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/upload_response.py` & `mux_python-3.9.0/mux_python/models/upload_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/video_view.py` & `mux_python-3.9.0/mux_python/models/video_view.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/video_view_event.py` & `mux_python-3.9.0/mux_python/models/video_view_event.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/models/video_view_response.py` & `mux_python-3.9.0/mux_python/models/video_view_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python/rest.py` & `mux_python-3.9.0/mux_python/rest.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/mux_python.egg-info/PKG-INFO` & `mux_python-3.9.0/mux_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mux-python
-Version: 3.8.0
+Version: 3.9.0
 Summary: Mux API
 Home-page: https://github.com/muxinc/mux-python
 Author: Mux DevEx
 Author-email: devex@mux.com
 Keywords: OpenAPI,OpenAPI-Generator,Mux API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mux-python Version: 3.8.0 Summary: Mux API Home-
+Metadata-Version: 2.1 Name: mux-python Version: 3.9.0 Summary: Mux API Home-
 page: https://github.com/muxinc/mux-python Author: Mux DevEx Author-email:
 devex@mux.com Keywords: OpenAPI,OpenAPI-Generator,Mux API Description-Content-
 Type: text/markdown License-File: LICENSE ![Mux Python Banner](github-python-
 sdk.png)
   [https://img.shields.io/pypi/v/mux_python] [https://github.com/muxinc/mux-
                 python/workflows/Integration%20Test/badge.svg]
                       PyPI | Mux_Docs | Mux_API_Reference
```

### Comparing `mux_python-3.8.0/mux_python.egg-info/SOURCES.txt` & `mux_python-3.9.0/mux_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 mux_python/models/create_simulcast_target_request.py
 mux_python/models/create_space_request.py
 mux_python/models/create_track_request.py
 mux_python/models/create_track_response.py
 mux_python/models/create_transcription_vocabulary_request.py
 mux_python/models/create_upload_request.py
 mux_python/models/delivery_report.py
+mux_python/models/delivery_report_delivered_seconds_by_resolution.py
 mux_python/models/dimension_value.py
 mux_python/models/disable_live_stream_response.py
 mux_python/models/enable_live_stream_response.py
 mux_python/models/error.py
 mux_python/models/export_date.py
 mux_python/models/export_file.py
 mux_python/models/filter_value.py
@@ -198,14 +199,15 @@
 test/test_create_simulcast_target_request.py
 test/test_create_space_request.py
 test/test_create_track_request.py
 test/test_create_track_response.py
 test/test_create_transcription_vocabulary_request.py
 test/test_create_upload_request.py
 test/test_delivery_report.py
+test/test_delivery_report_delivered_seconds_by_resolution.py
 test/test_delivery_usage_api.py
 test/test_dimension_value.py
 test/test_dimensions_api.py
 test/test_direct_uploads_api.py
 test/test_disable_live_stream_response.py
 test/test_enable_live_stream_response.py
 test/test_error.py
```

### Comparing `mux_python-3.8.0/setup.py` & `mux_python-3.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 
 import os
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "mux_python"
-VERSION = "3.8.0"
+VERSION = "3.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `mux_python-3.8.0/test/test_abridged_video_view.py` & `mux_python-3.9.0/test/test_abridged_video_view.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset.py` & `mux_python-3.9.0/test/test_asset.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset_errors.py` & `mux_python-3.9.0/test/test_asset_errors.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset_master.py` & `mux_python-3.9.0/test/test_asset_master.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset_non_standard_input_reasons.py` & `mux_python-3.9.0/test/test_asset_non_standard_input_reasons.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset_recording_times.py` & `mux_python-3.9.0/test/test_asset_recording_times.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset_response.py` & `mux_python-3.9.0/test/test_asset_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset_static_renditions.py` & `mux_python-3.9.0/test/test_asset_static_renditions.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_asset_static_renditions_files.py` & `mux_python-3.9.0/test/test_asset_static_renditions_files.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_assets_api.py` & `mux_python-3.9.0/test/test_assets_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_breakdown_value.py` & `mux_python-3.9.0/test/test_breakdown_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_broadcast.py` & `mux_python-3.9.0/test/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_broadcast_layout.py` & `mux_python-3.9.0/test/test_broadcast_layout.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_broadcast_resolution.py` & `mux_python-3.9.0/test/test_broadcast_resolution.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_broadcast_response.py` & `mux_python-3.9.0/test/test_broadcast_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_broadcast_status.py` & `mux_python-3.9.0/test/test_broadcast_status.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_asset_request.py` & `mux_python-3.9.0/test/test_create_asset_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_broadcast_request.py` & `mux_python-3.9.0/test/test_create_broadcast_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_live_stream_request.py` & `mux_python-3.9.0/test/test_create_live_stream_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_playback_id_request.py` & `mux_python-3.9.0/test/test_create_playback_id_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_playback_id_response.py` & `mux_python-3.9.0/test/test_create_playback_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_playback_restriction_request.py` & `mux_python-3.9.0/test/test_create_playback_restriction_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_simulcast_target_request.py` & `mux_python-3.9.0/test/test_create_simulcast_target_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_space_request.py` & `mux_python-3.9.0/test/test_create_space_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_track_request.py` & `mux_python-3.9.0/test/test_create_track_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_track_response.py` & `mux_python-3.9.0/test/test_create_track_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_transcription_vocabulary_request.py` & `mux_python-3.9.0/test/test_create_transcription_vocabulary_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_create_upload_request.py` & `mux_python-3.9.0/test/test_create_upload_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_delivery_report.py` & `mux_python-3.9.0/test/test_delivery_report.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_delivery_usage_api.py` & `mux_python-3.9.0/test/test_delivery_usage_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_dimension_value.py` & `mux_python-3.9.0/test/test_dimension_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_dimensions_api.py` & `mux_python-3.9.0/test/test_dimensions_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_direct_uploads_api.py` & `mux_python-3.9.0/test/test_direct_uploads_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_disable_live_stream_response.py` & `mux_python-3.9.0/test/test_disable_live_stream_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_enable_live_stream_response.py` & `mux_python-3.9.0/test/test_enable_live_stream_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_error.py` & `mux_python-3.9.0/test/test_error.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_errors_api.py` & `mux_python-3.9.0/test/test_errors_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_export_date.py` & `mux_python-3.9.0/test/test_export_date.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_export_file.py` & `mux_python-3.9.0/test/test_export_file.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_exports_api.py` & `mux_python-3.9.0/test/test_exports_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_filter_value.py` & `mux_python-3.9.0/test/test_filter_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_filters_api.py` & `mux_python-3.9.0/test/test_filters_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_asset_input_info_response.py` & `mux_python-3.9.0/test/test_get_asset_input_info_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_asset_or_live_stream_id_response.py` & `mux_python-3.9.0/test/test_get_asset_or_live_stream_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_asset_or_live_stream_id_response_data.py` & `mux_python-3.9.0/test/test_get_asset_or_live_stream_id_response_data.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_asset_or_live_stream_id_response_data_object.py` & `mux_python-3.9.0/test/test_get_asset_or_live_stream_id_response_data_object.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_asset_playback_id_response.py` & `mux_python-3.9.0/test/test_get_asset_playback_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_live_stream_playback_id_response.py` & `mux_python-3.9.0/test/test_get_live_stream_playback_id_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_metric_timeseries_data_response.py` & `mux_python-3.9.0/test/test_get_metric_timeseries_data_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_monitoring_breakdown_response.py` & `mux_python-3.9.0/test/test_get_monitoring_breakdown_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_monitoring_histogram_timeseries_response.py` & `mux_python-3.9.0/test/test_get_monitoring_histogram_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_monitoring_histogram_timeseries_response_meta.py` & `mux_python-3.9.0/test/test_get_monitoring_histogram_timeseries_response_meta.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_monitoring_timeseries_response.py` & `mux_python-3.9.0/test/test_get_monitoring_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_overall_values_response.py` & `mux_python-3.9.0/test/test_get_overall_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_real_time_breakdown_response.py` & `mux_python-3.9.0/test/test_get_real_time_breakdown_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_real_time_histogram_timeseries_response.py` & `mux_python-3.9.0/test/test_get_real_time_histogram_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_real_time_histogram_timeseries_response_meta.py` & `mux_python-3.9.0/test/test_get_real_time_histogram_timeseries_response_meta.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_get_real_time_timeseries_response.py` & `mux_python-3.9.0/test/test_get_real_time_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_incident.py` & `mux_python-3.9.0/test/test_incident.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_incident_breakdown.py` & `mux_python-3.9.0/test/test_incident_breakdown.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_incident_notification.py` & `mux_python-3.9.0/test/test_incident_notification.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_incident_notification_rule.py` & `mux_python-3.9.0/test/test_incident_notification_rule.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_incident_response.py` & `mux_python-3.9.0/test/test_incident_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_incidents_api.py` & `mux_python-3.9.0/test/test_incidents_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_input_file.py` & `mux_python-3.9.0/test/test_input_file.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_input_info.py` & `mux_python-3.9.0/test/test_input_info.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_input_settings.py` & `mux_python-3.9.0/test/test_input_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_input_settings_overlay_settings.py` & `mux_python-3.9.0/test/test_input_settings_overlay_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_input_track.py` & `mux_python-3.9.0/test/test_input_track.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_insight.py` & `mux_python-3.9.0/test/test_insight.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_all_metric_values_response.py` & `mux_python-3.9.0/test/test_list_all_metric_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_assets_response.py` & `mux_python-3.9.0/test/test_list_assets_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_breakdown_values_response.py` & `mux_python-3.9.0/test/test_list_breakdown_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_delivery_usage_response.py` & `mux_python-3.9.0/test/test_list_delivery_usage_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_dimension_values_response.py` & `mux_python-3.9.0/test/test_list_dimension_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_dimensions_response.py` & `mux_python-3.9.0/test/test_list_dimensions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_errors_response.py` & `mux_python-3.9.0/test/test_list_errors_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_exports_response.py` & `mux_python-3.9.0/test/test_list_exports_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_filter_values_response.py` & `mux_python-3.9.0/test/test_list_filter_values_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_filters_response.py` & `mux_python-3.9.0/test/test_list_filters_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_filters_response_data.py` & `mux_python-3.9.0/test/test_list_filters_response_data.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_incidents_response.py` & `mux_python-3.9.0/test/test_list_incidents_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_insights_response.py` & `mux_python-3.9.0/test/test_list_insights_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_live_streams_response.py` & `mux_python-3.9.0/test/test_list_live_streams_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_monitoring_dimensions_response.py` & `mux_python-3.9.0/test/test_list_monitoring_dimensions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_monitoring_dimensions_response_data.py` & `mux_python-3.9.0/test/test_list_monitoring_dimensions_response_data.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_monitoring_metrics_response.py` & `mux_python-3.9.0/test/test_list_monitoring_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_playback_restrictions_response.py` & `mux_python-3.9.0/test/test_list_playback_restrictions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_real_time_dimensions_response.py` & `mux_python-3.9.0/test/test_list_real_time_dimensions_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_real_time_dimensions_response_data.py` & `mux_python-3.9.0/test/test_list_real_time_dimensions_response_data.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_real_time_metrics_response.py` & `mux_python-3.9.0/test/test_list_real_time_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_related_incidents_response.py` & `mux_python-3.9.0/test/test_list_related_incidents_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_signing_keys_response.py` & `mux_python-3.9.0/test/test_list_signing_keys_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_spaces_response.py` & `mux_python-3.9.0/test/test_list_spaces_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_transcription_vocabularies_response.py` & `mux_python-3.9.0/test/test_list_transcription_vocabularies_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_uploads_response.py` & `mux_python-3.9.0/test/test_list_uploads_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_video_view_exports_response.py` & `mux_python-3.9.0/test/test_list_video_view_exports_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_list_video_views_response.py` & `mux_python-3.9.0/test/test_list_video_views_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_live_stream.py` & `mux_python-3.9.0/test/test_live_stream.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_live_stream_embedded_subtitle_settings.py` & `mux_python-3.9.0/test/test_live_stream_embedded_subtitle_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_live_stream_generated_subtitle_settings.py` & `mux_python-3.9.0/test/test_live_stream_generated_subtitle_settings.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_live_stream_response.py` & `mux_python-3.9.0/test/test_live_stream_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_live_stream_status.py` & `mux_python-3.9.0/test/test_live_stream_status.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_live_streams_api.py` & `mux_python-3.9.0/test/test_live_streams_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_metric.py` & `mux_python-3.9.0/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_metrics_api.py` & `mux_python-3.9.0/test/test_metrics_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_monitoring_api.py` & `mux_python-3.9.0/test/test_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_monitoring_breakdown_value.py` & `mux_python-3.9.0/test/test_monitoring_breakdown_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_monitoring_histogram_timeseries_bucket.py` & `mux_python-3.9.0/test/test_monitoring_histogram_timeseries_bucket.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_monitoring_histogram_timeseries_bucket_values.py` & `mux_python-3.9.0/test/test_monitoring_histogram_timeseries_bucket_values.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_monitoring_histogram_timeseries_datapoint.py` & `mux_python-3.9.0/test/test_monitoring_histogram_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_monitoring_timeseries_datapoint.py` & `mux_python-3.9.0/test/test_monitoring_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_notification_rule.py` & `mux_python-3.9.0/test/test_notification_rule.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_overall_values.py` & `mux_python-3.9.0/test/test_overall_values.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_playback_id.py` & `mux_python-3.9.0/test/test_playback_id.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_playback_id_api.py` & `mux_python-3.9.0/test/test_playback_id_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_playback_policy.py` & `mux_python-3.9.0/test/test_playback_policy.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_playback_restriction.py` & `mux_python-3.9.0/test/test_playback_restriction.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_playback_restriction_response.py` & `mux_python-3.9.0/test/test_playback_restriction_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_playback_restrictions_api.py` & `mux_python-3.9.0/test/test_playback_restrictions_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_real_time_api.py` & `mux_python-3.9.0/test/test_real_time_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_real_time_breakdown_value.py` & `mux_python-3.9.0/test/test_real_time_breakdown_value.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_real_time_histogram_timeseries_bucket.py` & `mux_python-3.9.0/test/test_real_time_histogram_timeseries_bucket.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_real_time_histogram_timeseries_bucket_values.py` & `mux_python-3.9.0/test/test_real_time_histogram_timeseries_bucket_values.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_real_time_histogram_timeseries_datapoint.py` & `mux_python-3.9.0/test/test_real_time_histogram_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_real_time_timeseries_datapoint.py` & `mux_python-3.9.0/test/test_real_time_timeseries_datapoint.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_referrer_domain_restriction.py` & `mux_python-3.9.0/test/test_referrer_domain_restriction.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_score.py` & `mux_python-3.9.0/test/test_score.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_signal_live_stream_complete_response.py` & `mux_python-3.9.0/test/test_signal_live_stream_complete_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_signing_key.py` & `mux_python-3.9.0/test/test_signing_key.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_signing_key_response.py` & `mux_python-3.9.0/test/test_signing_key_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_simulcast_target.py` & `mux_python-3.9.0/test/test_simulcast_target.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_simulcast_target_response.py` & `mux_python-3.9.0/test/test_simulcast_target_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_space.py` & `mux_python-3.9.0/test/test_space.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_space_response.py` & `mux_python-3.9.0/test/test_space_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_space_status.py` & `mux_python-3.9.0/test/test_space_status.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_space_type.py` & `mux_python-3.9.0/test/test_space_type.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_spaces_api.py` & `mux_python-3.9.0/test/test_spaces_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_start_space_broadcast_response.py` & `mux_python-3.9.0/test/test_start_space_broadcast_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_stop_space_broadcast_response.py` & `mux_python-3.9.0/test/test_stop_space_broadcast_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_track.py` & `mux_python-3.9.0/test/test_track.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_transcription_vocabularies_api.py` & `mux_python-3.9.0/test/test_transcription_vocabularies_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_transcription_vocabulary.py` & `mux_python-3.9.0/test/test_transcription_vocabulary.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_transcription_vocabulary_response.py` & `mux_python-3.9.0/test/test_transcription_vocabulary_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_asset_master_access_request.py` & `mux_python-3.9.0/test/test_update_asset_master_access_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_asset_mp4_support_request.py` & `mux_python-3.9.0/test/test_update_asset_mp4_support_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_asset_request.py` & `mux_python-3.9.0/test/test_update_asset_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_live_stream_embedded_subtitles_request.py` & `mux_python-3.9.0/test/test_update_live_stream_embedded_subtitles_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_live_stream_generated_subtitles_request.py` & `mux_python-3.9.0/test/test_update_live_stream_generated_subtitles_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_live_stream_request.py` & `mux_python-3.9.0/test/test_update_live_stream_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_referrer_domain_restriction_request.py` & `mux_python-3.9.0/test/test_update_referrer_domain_restriction_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_update_transcription_vocabulary_request.py` & `mux_python-3.9.0/test/test_update_transcription_vocabulary_request.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_upload.py` & `mux_python-3.9.0/test/test_upload.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_upload_error.py` & `mux_python-3.9.0/test/test_upload_error.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_upload_response.py` & `mux_python-3.9.0/test/test_upload_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_url_signing_keys_api.py` & `mux_python-3.9.0/test/test_url_signing_keys_api.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_video_view.py` & `mux_python-3.9.0/test/test_video_view.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_video_view_event.py` & `mux_python-3.9.0/test/test_video_view_event.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_video_view_response.py` & `mux_python-3.9.0/test/test_video_view_response.py`

 * *Files identical despite different names*

### Comparing `mux_python-3.8.0/test/test_video_views_api.py` & `mux_python-3.9.0/test/test_video_views_api.py`

 * *Files identical despite different names*

