# Comparing `tmp/visionai-0.3.2.tar.gz` & `tmp/visionai-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-0.3.2.tar", max compression
+gzip compressed data, was "visionai-0.3.3.tar", max compression
```

## Comparing `visionai-0.3.2.tar` & `visionai-0.3.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0    35148 2023-04-26 05:27:22.102663 visionai-0.3.2/LICENSE
--rw-r--r--   0        0        0    14097 2023-04-26 05:27:22.102663 visionai-0.3.2/README.md
--rw-r--r--   0        0        0      666 2023-04-26 05:27:22.102663 visionai-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/__init__.py
--rw-r--r--   0        0        0       28 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/__main__.py
--rw-r--r--   0        0        0     1369 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/apiutils/api.py
--rw-r--r--   0        0        0     3742 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/README.md
--rw-r--r--   0        0        0      495 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/__init__.py
--rw-r--r--   0        0        0      941 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/auth_app.py
--rw-r--r--   0        0        0    11314 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/camera_app.py
--rw-r--r--   0        0        0     5639 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/commands.py
--rw-r--r--   0        0        0     1626 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/device_app.py
--rw-r--r--   0        0        0        0 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/get_config_values.py
--rw-r--r--   0        0        0     3326 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/models_app.py
--rw-r--r--   0        0        0     6229 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/pipeline_app.py
--rw-r--r--   0        0        0    11404 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/scenario_app.py
--rw-r--r--   0        0        0      900 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/start_stop_influx_db.py
--rw-r--r--   0        0        0      938 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/start_stop_model_server.py
--rw-r--r--   0        0        0      944 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/start_stop_redis_grafana.py
--rw-r--r--   0        0        0      894 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/start_stop_web_app.py
--rw-r--r--   0        0        0      421 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/stop_cmd.py
--rw-r--r--   0        0        0     7307 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/cli/web_app.py
--rw-r--r--   0        0        0       87 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/config/.gitignore
--rw-r--r--   0        0        0        0 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/config/.gitkeep
--rw-r--r--   0        0        0     1624 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/config/camera-schema.json
--rw-r--r--   0        0        0      475 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/config/download_schema.py
--rw-r--r--   0        0        0     5702 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/config.py
--rw-r--r--   0        0        0        0 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/events/__init__.py
--rw-r--r--   0        0        0     5001 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/events/events_engine.py
--rw-r--r--   0        0        0     4645 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/main.py
--rw-r--r--   0        0        0        6 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models/.gitignore
--rw-r--r--   0        0        0     2055 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models/README.md
--rw-r--r--   0        0        0        0 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models/__init__.py
--rw-r--r--   0        0        0    17211 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models/common.py
--rw-r--r--   0        0        0    25516 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models/plots.py
--rw-r--r--   0        0        0    15970 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models/triton_client.py
--rw-r--r--   0        0        0     2260 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models/triton_client_yolov5.py
--rw-r--r--   0        0        0        2 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models-repo/.gitignore
--rw-r--r--   0        0        0        0 2023-04-26 05:27:22.102663 visionai-0.3.2/visionai/models-repo/.gitkeep
--rw-r--r--   0        0        0    12833 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/README.md
--rw-r--r--   0        0        0     2676 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/__init__.py
--rw-r--r--   0        0        0     5741 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/capture_media.py
--rw-r--r--   0        0        0    10906 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/ergonomics_detection.py
--rw-r--r--   0        0        0     2370 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/face_blur.py
--rw-r--r--   0        0        0     2868 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/firearms_detection.py
--rw-r--r--   0        0        0     5759 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/occupancy_monitoring.py
--rw-r--r--   0        0        0    16207 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/people_taking_picture_detection.py
--rw-r--r--   0        0        0     5220 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/ppe_detection.py
--rw-r--r--   0        0        0     6900 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/productivity_detection.py
--rw-r--r--   0        0        0     3467 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/restricted_zone.py
--rw-r--r--   0        0        0   144646 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/scenarios.json
--rw-r--r--   0        0        0     9363 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/slip_and_fall_detection.py
--rw-r--r--   0        0        0     2842 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/smoke_and_fire_detection.py
--rw-r--r--   0        0        0     2021 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/scenarios/smoking_detection.py
--rw-r--r--   0        0        0        0 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/__init__.py
--rw-r--r--   0        0        0      660 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/docker-compose.yml
--rw-r--r--   0        0        0      862 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_auth.py
--rw-r--r--   0        0        0     7325 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_camera.py
--rw-r--r--   0        0        0     1588 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_device.py
--rw-r--r--   0        0        0     1375 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_main.py
--rw-r--r--   0        0        0     1296 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_models.py
--rw-r--r--   0        0        0     2475 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_pipeline.py
--rw-r--r--   0        0        0     2494 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_scenario.py
--rw-r--r--   0        0        0     2656 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_stop_cmd.py
--rw-r--r--   0        0        0     2903 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_cli_web.py
--rw-r--r--   0        0        0     1624 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_config_download_schema.py
--rw-r--r--   0        0        0      770 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_deps.py
--rw-r--r--   0        0        0      696 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_docker_cli.py
--rw-r--r--   0        0        0      606 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_ergonomics_scenario.py
--rw-r--r--   0        0        0      576 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_face_blur_scenario.py
--rw-r--r--   0        0        0      599 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_firearm_scenario.py
--rw-r--r--   0        0        0      630 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_occupancy_monitoring_scenario.py
--rw-r--r--   0        0        0      768 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_opencv_stream.py
--rw-r--r--   0        0        0      630 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_people_taking_picture_scenario.py
--rw-r--r--   0        0        0      565 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_ppe_scenario.py
--rw-r--r--   0        0        0     2846 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_redis_grafana.py
--rw-r--r--   0        0        0      580 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_restricted_zone_scenario.py
--rw-r--r--   0        0        0     2742 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_scenarios_json.py
--rw-r--r--   0        0        0      631 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_slip_and_fall_scenario.py
--rw-r--r--   0        0        0      722 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_smoke_and_fire_scenario.py
--rw-r--r--   0        0        0      595 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/tests/test_smoking_scenario.py
--rw-r--r--   0        0        0     1766 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/util/__init__.py
--rw-r--r--   0        0        0    13339 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/util/docker_utils.py
--rw-r--r--   0        0        0     4688 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/util/download_models.py
--rw-r--r--   0        0        0    16148 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/util/general.py
--rw-r--r--   0        0        0    13828 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/util/image_utils.py
--rw-r--r--   0        0        0    14600 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/util/metrics.py
--rw-r--r--   0        0        0     9226 2023-04-26 05:27:22.106663 visionai-0.3.2/visionai/util/track.py
--rw-r--r--   0        0        0    14903 1970-01-01 00:00:00.000000 visionai-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-26 07:08:37.246760 visionai-0.3.3/LICENSE
+-rw-r--r--   0        0        0    14097 2023-04-26 07:08:37.250760 visionai-0.3.3/README.md
+-rw-r--r--   0        0        0      666 2023-04-26 07:08:37.250760 visionai-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/__main__.py
+-rw-r--r--   0        0        0     1369 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/apiutils/api.py
+-rw-r--r--   0        0        0     3742 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/README.md
+-rw-r--r--   0        0        0      495 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/__init__.py
+-rw-r--r--   0        0        0      941 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/auth_app.py
+-rw-r--r--   0        0        0    11314 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/camera_app.py
+-rw-r--r--   0        0        0     5735 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/commands.py
+-rw-r--r--   0        0        0     1626 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/device_app.py
+-rw-r--r--   0        0        0        0 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/get_config_values.py
+-rw-r--r--   0        0        0     3326 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/models_app.py
+-rw-r--r--   0        0        0     6229 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/pipeline_app.py
+-rw-r--r--   0        0        0    11404 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/scenario_app.py
+-rw-r--r--   0        0        0      900 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/start_stop_influx_db.py
+-rw-r--r--   0        0        0      938 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/start_stop_model_server.py
+-rw-r--r--   0        0        0      944 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/start_stop_redis_grafana.py
+-rw-r--r--   0        0        0      894 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/start_stop_web_app.py
+-rw-r--r--   0        0        0      421 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/stop_cmd.py
+-rw-r--r--   0        0        0     7307 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/cli/web_app.py
+-rw-r--r--   0        0        0       87 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/config/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/config/.gitkeep
+-rw-r--r--   0        0        0     1624 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/config/camera-schema.json
+-rw-r--r--   0        0        0      475 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/config/download_schema.py
+-rw-r--r--   0        0        0     5702 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/config.py
+-rw-r--r--   0        0        0        0 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/events/__init__.py
+-rw-r--r--   0        0        0     5001 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/events/events_engine.py
+-rw-r--r--   0        0        0     4504 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/main.py
+-rw-r--r--   0        0        0        6 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models/.gitignore
+-rw-r--r--   0        0        0     2055 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models/__init__.py
+-rw-r--r--   0        0        0    17211 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models/common.py
+-rw-r--r--   0        0        0    25516 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models/plots.py
+-rw-r--r--   0        0        0    15970 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models/triton_client.py
+-rw-r--r--   0        0        0     2260 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models/triton_client_yolov5.py
+-rw-r--r--   0        0        0        2 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models-repo/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/models-repo/.gitkeep
+-rw-r--r--   0        0        0    12833 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/README.md
+-rw-r--r--   0        0        0     2676 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/__init__.py
+-rw-r--r--   0        0        0     5741 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/capture_media.py
+-rw-r--r--   0        0        0    10906 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/ergonomics_detection.py
+-rw-r--r--   0        0        0     2370 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/face_blur.py
+-rw-r--r--   0        0        0     2868 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/firearms_detection.py
+-rw-r--r--   0        0        0     5759 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/occupancy_monitoring.py
+-rw-r--r--   0        0        0    16207 2023-04-26 07:08:37.250760 visionai-0.3.3/visionai/scenarios/people_taking_picture_detection.py
+-rw-r--r--   0        0        0     5220 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/scenarios/ppe_detection.py
+-rw-r--r--   0        0        0     6900 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/scenarios/productivity_detection.py
+-rw-r--r--   0        0        0     3467 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/scenarios/restricted_zone.py
+-rw-r--r--   0        0        0   144646 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/scenarios/scenarios.json
+-rw-r--r--   0        0        0     9363 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/scenarios/slip_and_fall_detection.py
+-rw-r--r--   0        0        0     2842 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/scenarios/smoke_and_fire_detection.py
+-rw-r--r--   0        0        0     2021 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/scenarios/smoking_detection.py
+-rw-r--r--   0        0        0        0 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/docker-compose.yml
+-rw-r--r--   0        0        0      862 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_auth.py
+-rw-r--r--   0        0        0     7325 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_camera.py
+-rw-r--r--   0        0        0     1588 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_device.py
+-rw-r--r--   0        0        0     1375 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_main.py
+-rw-r--r--   0        0        0     1296 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_models.py
+-rw-r--r--   0        0        0     2475 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_pipeline.py
+-rw-r--r--   0        0        0     2494 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_scenario.py
+-rw-r--r--   0        0        0     2656 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_stop_cmd.py
+-rw-r--r--   0        0        0     2903 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_cli_web.py
+-rw-r--r--   0        0        0     1624 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_config_download_schema.py
+-rw-r--r--   0        0        0      770 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_deps.py
+-rw-r--r--   0        0        0      696 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_docker_cli.py
+-rw-r--r--   0        0        0      606 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_ergonomics_scenario.py
+-rw-r--r--   0        0        0      576 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_face_blur_scenario.py
+-rw-r--r--   0        0        0      599 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_firearm_scenario.py
+-rw-r--r--   0        0        0      630 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_occupancy_monitoring_scenario.py
+-rw-r--r--   0        0        0      768 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_opencv_stream.py
+-rw-r--r--   0        0        0      630 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_people_taking_picture_scenario.py
+-rw-r--r--   0        0        0      565 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_ppe_scenario.py
+-rw-r--r--   0        0        0     2846 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_redis_grafana.py
+-rw-r--r--   0        0        0      580 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_restricted_zone_scenario.py
+-rw-r--r--   0        0        0     2742 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_scenarios_json.py
+-rw-r--r--   0        0        0      631 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_slip_and_fall_scenario.py
+-rw-r--r--   0        0        0      722 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_smoke_and_fire_scenario.py
+-rw-r--r--   0        0        0      595 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/tests/test_smoking_scenario.py
+-rw-r--r--   0        0        0     1766 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/util/__init__.py
+-rw-r--r--   0        0        0    13339 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/util/docker_utils.py
+-rw-r--r--   0        0        0     4688 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/util/download_models.py
+-rw-r--r--   0        0        0    16148 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/util/general.py
+-rw-r--r--   0        0        0    13828 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/util/image_utils.py
+-rw-r--r--   0        0        0    14600 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/util/metrics.py
+-rw-r--r--   0        0        0     9226 2023-04-26 07:08:37.254760 visionai-0.3.3/visionai/util/track.py
+-rw-r--r--   0        0        0    14903 1970-01-01 00:00:00.000000 visionai-0.3.3/PKG-INFO
```

### Comparing `visionai-0.3.2/LICENSE` & `visionai-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/README.md` & `visionai-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/pyproject.toml` & `visionai-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "visionai"
-version = "0.3.2"
+version = "0.3.3"
 description = "Vision AI toolkit"
 authors = ["Harsh Murari <hmurari@visionify.ai>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `visionai-0.3.2/visionai/apiutils/api.py` & `visionai-0.3.3/visionai/apiutils/api.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/README.md` & `visionai-0.3.3/visionai/cli/README.md`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/auth_app.py` & `visionai-0.3.3/visionai/cli/auth_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/camera_app.py` & `visionai-0.3.3/visionai/cli/camera_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/commands.py` & `visionai-0.3.3/visionai/cli/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 
         if web_api_running is False:
             # from config import VISIONAI_API_CONTAINER_NAME, VISIONAI_API_PORT, VISIONAI_API_DOCKER_IMAGE,VISIONAI_API_URL
             print(f'Starting web service API at port {VISIONAI_API_PORT}')
 
             if sys.platform == 'win32':
                 DOCKER_SOCK = '//var/run/docker.sock'
+            elif sys.platform == 'darwin':
+                DOCKER_SOCK = '/var/run/docker.sock'
             else:
                 DOCKER_SOCK = '/var/run/docker.sock'
 
             docker_container_start(
                 container_name=VISIONAI_API_CONTAINER_NAME,
                 image=VISIONAI_API_DOCKER_IMAGE,
                 portmap={3002:VISIONAI_API_PORT},
```

### Comparing `visionai-0.3.2/visionai/cli/device_app.py` & `visionai-0.3.3/visionai/cli/device_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/models_app.py` & `visionai-0.3.3/visionai/cli/models_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/pipeline_app.py` & `visionai-0.3.3/visionai/cli/pipeline_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/scenario_app.py` & `visionai-0.3.3/visionai/cli/scenario_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/start_stop_influx_db.py` & `visionai-0.3.3/visionai/cli/start_stop_influx_db.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/start_stop_model_server.py` & `visionai-0.3.3/visionai/cli/start_stop_model_server.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/start_stop_redis_grafana.py` & `visionai-0.3.3/visionai/cli/start_stop_redis_grafana.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/start_stop_web_app.py` & `visionai-0.3.3/visionai/cli/start_stop_web_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/cli/web_app.py` & `visionai-0.3.3/visionai/cli/web_app.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/config/camera-schema.json` & `visionai-0.3.3/visionai/config/camera-schema.json`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/config.py` & `visionai-0.3.3/visionai/config.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/events/events_engine.py` & `visionai-0.3.3/visionai/events/events_engine.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/main.py` & `visionai-0.3.3/visionai/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,22 +41,18 @@
 
 app.add_typer(models_app, name='model', help='Manage models')
 app.add_typer(models_app, name='models', hidden=True)
 
 app.add_typer(influx_db, name='influx', help='InfluxDB commands')
 app.add_typer(influx_db, name='influxdb', hidden=True)
 
-app.add_typer(models_server_app, name='Triton server', help='triton server commands')
-app.add_typer(models_server_app, name='Models', hidden=True)
-
-app.add_typer(redis_grafana_app, name='Redis Grafana', help='redis  Grafana commands')
-app.add_typer(redis_grafana_app, name='Redis', hidden=True)
-
-app.add_typer(web_app, name='Web app', help='web app commands')
-app.add_typer(web_app, name='Dashbaord', hidden=True)
+app.add_typer(models_server_app, name='triton', help='triton server commands')
+app.add_typer(redis_grafana_app, name='redis', help='redis & grafana commands')
+app.add_typer(web_app, name='web', help='Web-app commands')
+app.add_typer(web_app, name='dashboard', hidden=True)
 
 
 
 @app.command('init')
 def init(
     env: str = typer.Option('Enter .env file path', help='', prompt=True)
 ):
```

### Comparing `visionai-0.3.2/visionai/models/README.md` & `visionai-0.3.3/visionai/models/README.md`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/models/common.py` & `visionai-0.3.3/visionai/models/common.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/models/plots.py` & `visionai-0.3.3/visionai/models/plots.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/models/triton_client.py` & `visionai-0.3.3/visionai/models/triton_client.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/models/triton_client_yolov5.py` & `visionai-0.3.3/visionai/models/triton_client_yolov5.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/README.md` & `visionai-0.3.3/visionai/scenarios/README.md`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/__init__.py` & `visionai-0.3.3/visionai/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/capture_media.py` & `visionai-0.3.3/visionai/scenarios/capture_media.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/ergonomics_detection.py` & `visionai-0.3.3/visionai/scenarios/ergonomics_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/face_blur.py` & `visionai-0.3.3/visionai/scenarios/face_blur.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/firearms_detection.py` & `visionai-0.3.3/visionai/scenarios/firearms_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/occupancy_monitoring.py` & `visionai-0.3.3/visionai/scenarios/occupancy_monitoring.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/people_taking_picture_detection.py` & `visionai-0.3.3/visionai/scenarios/people_taking_picture_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/ppe_detection.py` & `visionai-0.3.3/visionai/scenarios/ppe_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/productivity_detection.py` & `visionai-0.3.3/visionai/scenarios/productivity_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/restricted_zone.py` & `visionai-0.3.3/visionai/scenarios/restricted_zone.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/scenarios.json` & `visionai-0.3.3/visionai/scenarios/scenarios.json`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/slip_and_fall_detection.py` & `visionai-0.3.3/visionai/scenarios/slip_and_fall_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/smoke_and_fire_detection.py` & `visionai-0.3.3/visionai/scenarios/smoke_and_fire_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/scenarios/smoking_detection.py` & `visionai-0.3.3/visionai/scenarios/smoking_detection.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/docker-compose.yml` & `visionai-0.3.3/visionai/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_auth.py` & `visionai-0.3.3/visionai/tests/test_cli_auth.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_camera.py` & `visionai-0.3.3/visionai/tests/test_cli_camera.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_device.py` & `visionai-0.3.3/visionai/tests/test_cli_device.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_main.py` & `visionai-0.3.3/visionai/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_models.py` & `visionai-0.3.3/visionai/tests/test_cli_models.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_pipeline.py` & `visionai-0.3.3/visionai/tests/test_cli_pipeline.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_scenario.py` & `visionai-0.3.3/visionai/tests/test_cli_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_stop_cmd.py` & `visionai-0.3.3/visionai/tests/test_cli_stop_cmd.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_cli_web.py` & `visionai-0.3.3/visionai/tests/test_cli_web.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_config_download_schema.py` & `visionai-0.3.3/visionai/tests/test_config_download_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_deps.py` & `visionai-0.3.3/visionai/tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_docker_cli.py` & `visionai-0.3.3/visionai/tests/test_docker_cli.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_ergonomics_scenario.py` & `visionai-0.3.3/visionai/tests/test_ergonomics_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_face_blur_scenario.py` & `visionai-0.3.3/visionai/tests/test_face_blur_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_firearm_scenario.py` & `visionai-0.3.3/visionai/tests/test_firearm_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_occupancy_monitoring_scenario.py` & `visionai-0.3.3/visionai/tests/test_occupancy_monitoring_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_opencv_stream.py` & `visionai-0.3.3/visionai/tests/test_opencv_stream.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_people_taking_picture_scenario.py` & `visionai-0.3.3/visionai/tests/test_people_taking_picture_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_ppe_scenario.py` & `visionai-0.3.3/visionai/tests/test_ppe_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_redis_grafana.py` & `visionai-0.3.3/visionai/tests/test_redis_grafana.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_restricted_zone_scenario.py` & `visionai-0.3.3/visionai/tests/test_restricted_zone_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_scenarios_json.py` & `visionai-0.3.3/visionai/tests/test_scenarios_json.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_slip_and_fall_scenario.py` & `visionai-0.3.3/visionai/tests/test_slip_and_fall_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_smoke_and_fire_scenario.py` & `visionai-0.3.3/visionai/tests/test_smoke_and_fire_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/tests/test_smoking_scenario.py` & `visionai-0.3.3/visionai/tests/test_smoking_scenario.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/util/__init__.py` & `visionai-0.3.3/visionai/util/__init__.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/util/docker_utils.py` & `visionai-0.3.3/visionai/util/docker_utils.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/util/download_models.py` & `visionai-0.3.3/visionai/util/download_models.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/util/general.py` & `visionai-0.3.3/visionai/util/general.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/util/image_utils.py` & `visionai-0.3.3/visionai/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/util/metrics.py` & `visionai-0.3.3/visionai/util/metrics.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/visionai/util/track.py` & `visionai-0.3.3/visionai/util/track.py`

 * *Files identical despite different names*

### Comparing `visionai-0.3.2/PKG-INFO` & `visionai-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai
-Version: 0.3.2
+Version: 0.3.3
 Summary: Vision AI toolkit
 License: GPL-3.0-only
 Author: Harsh Murari
 Author-email: hmurari@visionify.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: visionai Version: 0.3.2 Summary: Vision AI toolkit
+Metadata-Version: 2.1 Name: visionai Version: 0.3.3 Summary: Vision AI toolkit
 License: GPL-3.0-only Author: Harsh Murari Author-email: hmurari@visionify.ai
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: docker (>=5.0.3,<7.0.0) Requires-
```

