# Comparing `tmp/aws-parallelcluster-3.5.1.tar.gz` & `tmp/aws-parallelcluster-3.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-3.5.1.tar", last modified: Tue Mar 28 20:04:48 2023, max compression
+gzip compressed data, was "aws-parallelcluster-3.6.0b1.tar", last modified: Thu Apr 27 20:58:59 2023, max compression
```

## Comparing `aws-parallelcluster-3.5.1.tar` & `aws-parallelcluster-3.6.0b1.tar`

### file list

```diff
@@ -1,258 +1,264 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.152795 aws-parallelcluster-3.5.1/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      114 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/MANIFEST.in
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1850 2023-03-28 20:04:48.152795 aws-parallelcluster-3.5.1/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      787 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/README
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-03-28 20:04:48.152795 aws-parallelcluster-3.5.1/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3443 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.112795 aws-parallelcluster-3.5.1/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.116795 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1850 2023-03-28 20:04:48.000000 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10400 2023-03-28 20:04:48.000000 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-03-28 20:04:48.000000 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      147 2023-03-28 20:04:48.000000 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-03-28 20:04:48.000000 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      801 2023-03-28 20:04:48.000000 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       36 2023-03-28 20:04:48.000000 aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.116795 aws-parallelcluster-3.5.1/src/pcluster/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.116795 aws-parallelcluster-3.5.1/src/pcluster/api/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.116795 aws-parallelcluster-3.5.1/src/pcluster/api/awslambda/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/awslambda/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2659 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/awslambda/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11252 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/awslambda/serverless_wsgi.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.120795 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      548 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4019 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4192 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_instances_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7167 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19236 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7697 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6289 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/image_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15354 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/controllers/image_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4143 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/converters.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1536 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/encoder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5812 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/errors.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7657 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/flask_app.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.128795 aws-parallelcluster-3.5.1/src/pcluster/api/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6121 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4682 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2128 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2428 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/base_model_.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3757 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3652 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/build_image_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3639 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/build_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/change.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1717 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/cloud_formation_resource_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1775 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/cloud_formation_stack_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2103 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9207 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8637 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1879 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1630 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4053 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/config_validation_message.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/conflict_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3813 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3875 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/create_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3751 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/create_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2302 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/delete_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2220 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/delete_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3397 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_cluster_instances_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17460 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3802 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19464 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4859 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/dryrun_operation_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6209 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2185 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_ami_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1488 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_ami_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6566 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2451 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/failure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3660 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/get_cluster_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2791 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/get_cluster_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3618 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/get_image_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2759 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/get_image_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1576 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/image_build_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1678 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/image_builder_image_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2053 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/image_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8609 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/image_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1615 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/image_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1484 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/instance_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2183 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/internal_service_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2161 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/limit_exceeded_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3024 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/list_cluster_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3200 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/list_clusters_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2992 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/list_image_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3108 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/list_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2315 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/list_official_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2373 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/log_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8592 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/log_stream.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2418 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/metadata.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1348 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/node_type.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/not_found_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1532 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/requested_compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/scheduler.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12343 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/stack_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2286 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/tag.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2172 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/unauthorized_client_error_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6155 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2594 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/update_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4944 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/update_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2377 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/update_compute_fleet_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3274 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/update_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4087 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/update_error.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1394 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/models/validation_level.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.128795 aws-parallelcluster-3.5.1/src/pcluster/api/openapi/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/openapi/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)   114697 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/openapi/openapi.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1388 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/typing_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8594 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/api/util.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.132795 aws-parallelcluster-3.5.1/src/pcluster/aws/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5634 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/aws_api.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15052 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/aws_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5430 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/batch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6992 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/cfn.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8480 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2234 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/dynamo.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21652 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/ec2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3313 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/efs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3795 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/fsx.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1351 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/iam.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      949 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      907 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/kms.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5687 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1801 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/resource_groups.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2097 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/route53.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7491 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/s3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/s3_resource.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1067 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/secretsmanager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1003 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/ssm.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      959 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/aws/sts.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.136795 aws-parallelcluster-3.5.1/src/pcluster/cli/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.136795 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4361 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/cluster_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      975 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5361 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/common.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.136795 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1486 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/command.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19988 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/easyconfig.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10146 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/networking.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5959 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/subnet_computation.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8348 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6726 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/dcv_connect.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      887 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/dcv_util.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3571 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/image_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3968 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/ssh.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1434 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/commands/version.py
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)    10935 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1116 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/exceptions.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3002 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4586 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/middleware.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7601 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/cli/model.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.136795 aws-parallelcluster-3.5.1/src/pcluster/config/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/config/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)   124676 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/config/cluster_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    14012 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/config/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12981 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/config/config_patch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11611 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/config/imagebuilder_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21748 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/config/update_policy.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10658 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/constants.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2624 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/imagebuilder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2364 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/launch_template_utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.140795 aws-parallelcluster-3.5.1/src/pcluster/lib/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      963 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/lib/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3558 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/lib/lib.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.140795 aws-parallelcluster-3.5.1/src/pcluster/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    56075 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/cluster.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12099 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/cluster_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13929 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12602 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/compute_fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    35260 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5037 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/imagebuilder_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16413 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/models/s3_bucket.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.140795 aws-parallelcluster-3.5.1/src/pcluster/networking/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/networking/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3769 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/networking/vpc_factory.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.112795 aws-parallelcluster-3.5.1/src/pcluster/resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.112795 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.140795 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.140795 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/alinux2/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1816 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/alinux2/Dockerfile
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1139 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/build-docker-images.sh
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      535 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/buildspec.yml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.140795 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1599 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     5466 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1954 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2882 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2457 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)      856 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/upload-docker-images.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.140795 aws-parallelcluster-3.5.1/src/pcluster/resources/compute_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10290 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/compute_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.112795 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.144795 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7610 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.144795 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10142 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       96 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       81 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2701 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13195 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1842 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3545 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2763 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.144795 aws-parallelcluster-3.5.1/src/pcluster/resources/head_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6468 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/head_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.144795 aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1919 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/custom_script.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10454 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8632 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11798 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15768 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6172 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.144795 aws-parallelcluster-3.5.1/src/pcluster/schemas/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/schemas/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    82157 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/schemas/cluster_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9750 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/schemas/common_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7968 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/schemas/imagebuilder_schema.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.148795 aws-parallelcluster-3.5.1/src/pcluster/templates/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    38565 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/awsbatch_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2856 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/cdk_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    40728 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/cdk_builder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    80793 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/cluster_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    24098 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/cw_dashboard_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    44186 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/imagebuilder_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      682 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/import_cdk.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13468 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/templates/slurm_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    14172 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.152795 aws-parallelcluster-3.5.1/src/pcluster/validators/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8763 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/awsbatch_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    61009 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/cluster_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2346 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3528 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/database_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7535 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/directory_service_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12873 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/ebs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    25736 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/ec2_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1212 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/efs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1739 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/feature_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9186 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/fsx_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4000 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/iam_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2361 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/imagebuilder_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12556 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/instances_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1414 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/kms_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9209 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/networking_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6046 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/s3_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7690 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/scheduler_plugin_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      825 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster/validators/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-03-28 20:04:48.152795 aws-parallelcluster-3.5.1/src/pcluster3_config_converter/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster3_config_converter/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    52964 2023-03-28 14:46:24.000000 aws-parallelcluster-3.5.1/src/pcluster3_config_converter/pcluster3_config_converter.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.624519 aws-parallelcluster-3.6.0b1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      114 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/MANIFEST.in
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1852 2023-04-27 20:58:59.624519 aws-parallelcluster-3.6.0b1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      787 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/README
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-04-27 20:58:59.624519 aws-parallelcluster-3.6.0b1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3447 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1852 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10682 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      147 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      803 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       36 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.588519 aws-parallelcluster-3.6.0b1/src/pcluster/api/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.588519 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2659 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11252 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/serverless_wsgi.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.588519 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      548 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4019 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4192 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_instances_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7167 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19236 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7697 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6289 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15354 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4143 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/converters.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1536 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/encoder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5812 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/errors.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7657 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/flask_app.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.600519 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6121 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4682 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2128 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2428 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/base_model_.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3757 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3652 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3639 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/change.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1717 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_resource_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1775 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_stack_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2103 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9207 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8637 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1879 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1630 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4053 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/config_validation_message.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/conflict_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3813 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3875 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3751 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2302 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2220 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3397 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_instances_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17460 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3802 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19464 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4859 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/dryrun_operation_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6209 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2185 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1488 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6566 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2451 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/failure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3660 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2791 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3618 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2759 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1576 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_build_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1678 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_builder_image_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2053 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8609 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1615 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1484 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/instance_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2183 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/internal_service_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2161 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/limit_exceeded_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3024 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_cluster_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3200 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_clusters_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2992 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_image_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3108 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2315 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_official_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2373 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8592 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_stream.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2418 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/metadata.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1348 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/node_type.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/not_found_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1532 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/requested_compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/scheduler.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12343 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/stack_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2286 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/tag.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2172 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/unauthorized_client_error_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6155 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2594 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4944 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2377 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3274 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4087 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_error.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1394 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/validation_level.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.600519 aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)   114697 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/openapi.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1388 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/typing_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8594 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/util.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.604519 aws-parallelcluster-3.6.0b1/src/pcluster/aws/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5634 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_api.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15716 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5430 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/batch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7832 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/cfn.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8480 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2234 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/dynamo.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21619 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/ec2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3313 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/efs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3795 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/fsx.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1351 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/iam.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      949 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      907 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/kms.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5687 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1801 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/resource_groups.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2097 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/route53.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7491 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3_resource.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1067 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/secretsmanager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1003 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/ssm.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      959 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/sts.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.604519 aws-parallelcluster-3.6.0b1/src/pcluster/cli/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4361 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/cluster_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      975 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5361 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/common.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1486 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/command.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    20572 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/easyconfig.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10146 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/networking.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5959 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/subnet_computation.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8348 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6742 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_connect.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      896 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_util.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3571 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/image_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3968 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/ssh.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1434 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/version.py
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)    10935 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1116 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/exceptions.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3002 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4586 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/middleware.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7601 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/model.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/config/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)   133673 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/cluster_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16981 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12981 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/config_patch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11611 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/imagebuilder_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21758 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/update_policy.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11490 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/constants.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2624 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/imagebuilder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2364 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/launch_template_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/lib/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      963 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/lib/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3558 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/lib/lib.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    58732 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12099 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13929 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12602 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/compute_fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    35260 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5037 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16902 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/s3_bucket.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/networking/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/networking/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3769 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/networking/vpc_factory.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/alinux2/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1816 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/alinux2/Dockerfile
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1139 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/build-docker-images.sh
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      535 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/buildspec.yml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1599 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     5466 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1954 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2882 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2457 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)      856 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/upload-docker-images.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/compute_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10447 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/compute_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7610 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10142 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       96 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       81 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2701 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13195 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1842 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3545 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2763 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/head_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6660 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/head_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.616519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1919 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/custom_script.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10585 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8732 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12214 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16131 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6319 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.616519 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    86365 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/cluster_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10452 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/common_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7968 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/imagebuilder_schema.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.616519 aws-parallelcluster-3.6.0b1/src/pcluster/templates/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    38565 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/awsbatch_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5999 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_artifacts_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3115 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    40959 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    62422 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cluster_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10026 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/compute_fleet_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    35904 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cw_dashboard_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    44224 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/imagebuilder_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      682 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/import_cdk.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17214 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/queue_group_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13562 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/slurm_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    18843 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.620519 aws-parallelcluster-3.6.0b1/src/pcluster/validators/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8763 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/awsbatch_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    64756 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/cluster_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5233 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3528 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/database_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7577 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/directory_service_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12873 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/ebs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    25736 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/ec2_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1212 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/efs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1739 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/feature_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9186 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/fsx_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4000 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/iam_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2361 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/imagebuilder_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12556 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/instances_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1414 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/kms_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1858 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/monitoring_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9209 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/networking_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6760 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/s3_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7690 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/scheduler_plugin_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5195 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/slurm_settings_validator.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4081 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/tags_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      825 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.620519 aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    52964 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/pcluster3_config_converter.py
```

### Comparing `aws-parallelcluster-3.5.1/PKG-INFO` & `aws-parallelcluster-3.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.5.1
+Version: 3.6.0b1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.5.1/README` & `aws-parallelcluster-3.6.0b1/README`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/setup.py` & `aws-parallelcluster-3.6.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def readme():
     """Read the README file and use it as long description."""
     with open(os.path.join(os.path.dirname(__file__), "README"), encoding="utf-8") as f:
         return f.read()
 
 
-VERSION = "3.5.1"
+VERSION = "3.6.0b1"
 CDK_VERSION = "1.137,!=1.153.0"
 REQUIRES = [
     "setuptools",
     "boto3>=1.16.14",
     "tabulate>=0.8.8,<=0.8.10",
     "PyYAML~=5.3",
     "jinja2~=3.0",
@@ -44,15 +44,15 @@
     "aws-cdk.aws-logs~=" + CDK_VERSION,
     "aws-cdk.aws-route53~=" + CDK_VERSION,
     "aws-cdk.aws-ssm~=" + CDK_VERSION,
     "aws-cdk.aws-sqs~=" + CDK_VERSION,
     "aws-cdk.aws-cloudformation~=" + CDK_VERSION,
     "werkzeug~=2.0",
     "connexion~=2.13.0",
-    "flask~=2.0",
+    "flask~=2.2.0",
     "jmespath~=0.10",
 ]
 
 LAMBDA_REQUIRES = [
     "aws-lambda-powertools~=1.14",
 ]
```

### Comparing `aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/PKG-INFO` & `aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.5.1
+Version: 3.6.0b1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/SOURCES.txt` & `aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -190,20 +190,23 @@
 src/pcluster/resources/imagebuilder/update_and_reboot.yaml
 src/pcluster/schemas/__init__.py
 src/pcluster/schemas/cluster_schema.py
 src/pcluster/schemas/common_schema.py
 src/pcluster/schemas/imagebuilder_schema.py
 src/pcluster/templates/__init__.py
 src/pcluster/templates/awsbatch_builder.py
+src/pcluster/templates/cdk_artifacts_manager.py
 src/pcluster/templates/cdk_builder.py
 src/pcluster/templates/cdk_builder_utils.py
 src/pcluster/templates/cluster_stack.py
+src/pcluster/templates/compute_fleet_stack.py
 src/pcluster/templates/cw_dashboard_builder.py
 src/pcluster/templates/imagebuilder_stack.py
 src/pcluster/templates/import_cdk.py
+src/pcluster/templates/queue_group_stack.py
 src/pcluster/templates/slurm_builder.py
 src/pcluster/validators/__init__.py
 src/pcluster/validators/awsbatch_validators.py
 src/pcluster/validators/cluster_validators.py
 src/pcluster/validators/common.py
 src/pcluster/validators/database_validators.py
 src/pcluster/validators/directory_service_validators.py
@@ -212,13 +215,16 @@
 src/pcluster/validators/efs_validators.py
 src/pcluster/validators/feature_validators.py
 src/pcluster/validators/fsx_validators.py
 src/pcluster/validators/iam_validators.py
 src/pcluster/validators/imagebuilder_validators.py
 src/pcluster/validators/instances_validators.py
 src/pcluster/validators/kms_validators.py
+src/pcluster/validators/monitoring_validators.py
 src/pcluster/validators/networking_validators.py
 src/pcluster/validators/s3_validators.py
 src/pcluster/validators/scheduler_plugin_validators.py
+src/pcluster/validators/slurm_settings_validator.py
+src/pcluster/validators/tags_validators.py
 src/pcluster/validators/utils.py
 src/pcluster3_config_converter/__init__.py
 src/pcluster3_config_converter/pcluster3_config_converter.py
```

### Comparing `aws-parallelcluster-3.5.1/src/aws_parallelcluster.egg-info/requires.txt` & `aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 aws-cdk.aws-logs!=1.153.0,~=1.137
 aws-cdk.aws-route53!=1.153.0,~=1.137
 aws-cdk.aws-ssm!=1.153.0,~=1.137
 aws-cdk.aws-sqs!=1.153.0,~=1.137
 aws-cdk.aws-cloudformation!=1.153.0,~=1.137
 werkzeug~=2.0
 connexion~=2.13.0
-flask~=2.0
+flask~=2.2.0
 jmespath~=0.10
 
 [awslambda]
 aws-lambda-powertools~=1.14
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/awslambda/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/awslambda/entrypoint.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/awslambda/serverless_wsgi.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/serverless_wsgi.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_instances_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_instances_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_logs_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/cluster_operations_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_operations_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/image_logs_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/controllers/image_operations_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_operations_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/converters.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/converters.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/encoder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/encoder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/errors.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/errors.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/flask_app.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/flask_app.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/ami_info.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/base_model_.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/build_image_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/build_image_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/change.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/change.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/cloud_formation_resource_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_resource_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/cloud_formation_stack_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_stack_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_configuration_structure.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_info_summary.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_instance.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/cluster_status_filtering_option.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/compute_fleet_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/config_validation_message.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/config_validation_message.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/conflict_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/conflict_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/create_cluster_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/create_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/delete_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/delete_image_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_cluster_instances_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_instances_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_compute_fleet_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/describe_image_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/dryrun_operation_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/dryrun_operation_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_ami_info.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_ami_info_summary.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_ami_state.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/ec2_instance.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/failure.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/failure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/get_cluster_log_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/get_cluster_stack_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/get_image_log_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/get_image_stack_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/image_build_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_build_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/image_builder_image_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_builder_image_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/image_configuration_structure.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/image_info_summary.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/image_status_filtering_option.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/instance_state.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/instance_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/internal_service_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/internal_service_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/limit_exceeded_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/limit_exceeded_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/list_cluster_log_streams_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_cluster_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/list_clusters_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_clusters_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/list_image_log_streams_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_image_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/list_images_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/list_official_images_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_official_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/log_event.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/log_stream.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_stream.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/metadata.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/metadata.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/node_type.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/node_type.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/not_found_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/not_found_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/requested_compute_fleet_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/requested_compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/scheduler.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/stack_event.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/stack_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/tag.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/tag.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/unauthorized_client_error_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/unauthorized_client_error_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/update_cluster_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/update_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/update_compute_fleet_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/update_compute_fleet_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/update_error.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_error.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/models/validation_level.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/validation_level.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/openapi/openapi.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/openapi.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openapi: 3.0.2
 info:
   description: ParallelCluster API
   title: ParallelCluster
-  version: 3.5.1
+  version: 3.6.0
 servers:
 - url: /
 # override: auth is defined the the API GW level
 # security:
 # - aws.auth.sigv4: []
 paths:
   /v3/clusters:
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/typing_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/typing_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/api/util.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/util.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/aws_api.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_api.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/aws_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,26 +33,36 @@
 
         If the stack doesn't exist it raises an exception.
         """
         self._stack_data = stack_data
         self._params = self._stack_data.get("Parameters", [])
         self.tags = self._stack_data.get("Tags", [])
         self.outputs = self._stack_data.get("Outputs", [])
+        self.__resources = None
 
     @property
     def id(self):
         """Return the id/arn of the stack."""
         return self._stack_data.get("StackId")
 
     @property
     def name(self):
         """Return the name of the stack."""
         return self._stack_data.get("StackName")
 
     @property
+    def resources(self):
+        """Return the resources of the stack."""
+        if not self.__resources:
+            from pcluster.aws.aws_api import AWSApi  # noqa: F401 pylint: disable=import-outside-toplevel
+
+            self.__resources = AWSApi.instance().cfn.describe_stack_resources(self.name)
+        return self.__resources
+
+    @property
     def status(self):
         """Return the status of the stack."""
         return self._stack_data.get("StackStatus")
 
     @property
     def status_reason(self):
         """Return the reason the stack is in its current status."""
@@ -86,14 +96,22 @@
 
         :param key_name: Parameter Key
         :return: ParameterValue if that parameter exists, otherwise None
         """
         param_value = next((par["ParameterValue"] for par in self._params if par["ParameterKey"] == key_name), None)
         return None if param_value is None else param_value.strip()
 
+    def get_resource_physical_id(self, resource_logical_id: str):
+        """Return the resource information."""
+        resource = self.resources.get(resource_logical_id)
+        if resource:
+            return resource["PhysicalResourceId"]
+        else:
+            return None
+
 
 class InstanceInfo:
     """Object to store Instance information, initialized with a describe_instances call."""
 
     def __init__(self, instance_data: dict):
         self._instance_data = instance_data
         self._tags = self._instance_data.get("Tags", [])
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/batch.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/batch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/cfn.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/cfn.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,51 +12,66 @@
 import logging
 
 from botocore.exceptions import ClientError
 
 from pcluster.aws.aws_resources import StackInfo
 from pcluster.aws.common import AWSClientError, AWSExceptionHandler, Boto3Client, StackNotFoundError
 from pcluster.constants import PCLUSTER_IMAGE_ID_TAG, PCLUSTER_VERSION_TAG
+from pcluster.utils import remove_none_values
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CfnClient(Boto3Client):
     """Implement CFN Boto3 client."""
 
     def __init__(self):
         super().__init__("cloudformation")
 
     @AWSExceptionHandler.handle_client_exception
-    def create_stack(self, stack_name: str, disable_rollback: bool, tags: list, template_body: str):
+    def create_stack(
+        self, stack_name: str, disable_rollback: bool, tags: list, template_body: str, parameters: list = None
+    ):
         """Create CFN stack by using the given template."""
+        optional_args = {
+            "Tags": tags,
+            "Parameters": parameters,
+        }
+        optional_args_with_value = remove_none_values(optional_args)
         return self._client.create_stack(
             StackName=stack_name,
             TemplateBody=template_body,
             Capabilities=["CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"],
             DisableRollback=disable_rollback,
-            Tags=tags,
+            **optional_args_with_value,
         )
 
     @AWSExceptionHandler.handle_client_exception
     def create_stack_from_url(
         self,
         stack_name: str,
         disable_rollback: bool,
         tags: list,
         template_url: str,
         capabilities: str = "CAPABILITY_IAM",
+        parameters: list = None,
     ):
         """Create CFN stack by using the given template url."""
+        optional_args = {
+            "Tags": tags,
+            "Parameters": parameters,
+        }
+        optional_args_with_value = remove_none_values(optional_args)
+
         return self._client.create_stack(
             StackName=stack_name,
             TemplateURL=template_url,
             Capabilities=[capabilities, "CAPABILITY_NAMED_IAM"],
             DisableRollback=disable_rollback,
-            Tags=tags,
+            **optional_args_with_value,
         )
 
     @AWSExceptionHandler.handle_client_exception
     def delete_stack(self, stack_name: str):
         """Delete CFN stack."""
         return self._client.delete_stack(StackName=stack_name)
 
@@ -67,27 +82,27 @@
             StackName=stack_name,
             TemplateBody=json.dumps(updated_template, indent=2),  # Indent so it looks nice in the console
             Parameters=params,
             Capabilities=["CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"],
         )
 
     @AWSExceptionHandler.handle_client_exception
-    def update_stack_from_url(self, stack_name: str, template_url: str, tags: list = None):
+    def update_stack_from_url(self, stack_name: str, template_url: str, tags: list = None, parameters: list = None):
         """Update CFN stack by using the given template url."""
-        if tags is None:
-            return self._client.update_stack(
-                StackName=stack_name,
-                TemplateURL=template_url,
-                Capabilities=["CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"],
-            )
+        optional_args = {
+            "Tags": tags,
+            "Parameters": parameters,
+        }
+        optional_args_with_value = remove_none_values(optional_args)
+
         return self._client.update_stack(
             StackName=stack_name,
             TemplateURL=template_url,
             Capabilities=["CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"],
-            Tags=tags,
+            **optional_args_with_value,
         )
 
     @AWSExceptionHandler.handle_client_exception
     @AWSExceptionHandler.retry_on_boto3_throttling
     def describe_stack(self, stack_name: str):
         """Get information for the given stack."""
         try:
@@ -144,14 +159,20 @@
             return self._client.describe_stack_resource(StackName=stack_name, LogicalResourceId=logic_resource_id)
         except Exception:
             raise AWSClientError(
                 function_name="describe_stack_resource", message=f"No resource {logic_resource_id} found."
             )
 
     @AWSExceptionHandler.handle_client_exception
+    def describe_stack_resources(self, stack_name: str):
+        """Get stack resources information."""
+        response = self._client.describe_stack_resources(StackName=stack_name).get("StackResources")
+        return {resource["LogicalResourceId"]: resource for resource in response}  # Build dictionary for better query.
+
+    @AWSExceptionHandler.handle_client_exception
     def get_imagebuilder_stacks(self, next_token=None):
         """List existing imagebuilder stacks."""
         return self._list_parentless_stacks_with_tag(PCLUSTER_IMAGE_ID_TAG, next_token)
 
     def _list_parentless_stacks_with_tag(self, tag, next_token=None):
         describe_stacks_kwargs = {}
         if next_token:
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/dynamo.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/dynamo.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/ec2.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             return subnets[0].get("VpcId")
         raise AWSClientError(function_name="describe_subnets", message=f"Subnet {subnet_id} not found")
 
     @AWSExceptionHandler.handle_client_exception
     @Cache.cached
     def get_subnet_cidr(self, subnet_id):
         """Return cidr block  of the given subnet."""
-        subnets = self._client.describe_subnets(SubnetIds=[subnet_id]).get("Subnets")
+        subnets = self.describe_subnets([subnet_id])
         if subnets:
             return subnets[0].get("CidrBlock")
         raise AWSClientError(function_name="describe_subnets", message=f"Subnet {subnet_id} not found")
 
     @AWSExceptionHandler.handle_client_exception
     @Cache.cached
     def describe_image(self, ami_id):
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/efs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/efs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/fsx.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/fsx.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/iam.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/iam.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/imagebuilder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/kms.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/kms.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/logs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/resource_groups.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/resource_groups.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/route53.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/route53.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/s3.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/s3_resource.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3_resource.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/secretsmanager.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/ssm.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/aws/sts.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/sts.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/cluster_logs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/commands.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/command.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/command.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/easyconfig.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/easyconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     placement_group_exists,
     prompt,
     prompt_iterable,
 )
 from pcluster.constants import (
     DEFAULT_MAX_COUNT,
     DEFAULT_MIN_COUNT,
-    MAX_NUMBER_OF_COMPUTE_RESOURCES,
+    MAX_COMPUTE_RESOURCES_PER_QUEUE,
+    MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER,
     MAX_NUMBER_OF_QUEUES,
     SUPPORTED_SCHEDULERS,
 )
 from pcluster.utils import error, get_supported_os_for_scheduler
 from pcluster.validators.cluster_validators import NameValidator
 
 LOGGER = logging.getLogger(__name__)
@@ -164,15 +165,15 @@
     if scheduler == "awsbatch":
         number_of_queues = 1
         size_name = "vCPU"
     else:
         number_of_queues = int(
             prompt(
                 "Number of queues",
-                lambda x: str(x).isdigit() and int(x) >= 1 and int(x) <= MAX_NUMBER_OF_QUEUES,
+                lambda x: str(x).isdigit() and 1 <= int(x) <= MAX_NUMBER_OF_QUEUES,
                 default_value=1,
             )
         )
         size_name = "instance count"
 
     queues = []
     queue_names = []
@@ -191,18 +192,21 @@
                 f"Error: The name {queue_name} cannot be used for multiple queues. Please insert a different queue "
                 "name."
             )
 
         if scheduler == "awsbatch":
             number_of_compute_resources = 1
         else:
+            queue_limit = min(
+                (MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER / number_of_queues), MAX_COMPUTE_RESOURCES_PER_QUEUE
+            )
             number_of_compute_resources = int(
                 prompt(
                     f"Number of compute resources for {queue_name}",
-                    validator=lambda x: str(x).isdigit() and int(x) >= 1 and int(x) <= MAX_NUMBER_OF_COMPUTE_RESOURCES,
+                    validator=lambda x, q=queue_limit: str(x).isdigit() and 1 <= int(x) <= q,
                     default_value=1,
                 )
             )
         compute_resources = []
         efa_enabled_in_queue = False
         for compute_resource_index in range(number_of_compute_resources):
             efa_enabled_in_compute_resource = False
@@ -357,15 +361,25 @@
             qualified_compute_subnets = _filter_subnets_offering_instance_types(subnet_list, compute_instance_types)
         else:
             # Special case of awsbatch, where compute instance type is not specified
             qualified_compute_subnets = subnet_list
         if (
             not qualified_head_node_subnets
             or not qualified_compute_subnets
-            or (prompt("Automate Subnet creation? (y/n)", lambda x: x in ("y", "n"), default_value="y") == "y")
+            or (
+                prompt(
+                    "The creation of a public and private subnet combination will result in\n"
+                    "charges for NAT gateway creation that are not covered under the free tier.\n"
+                    "Please refer to https://aws.amazon.com/vpc/pricing/ for more details.\n"
+                    "Automate Subnet creation? (y/n)",
+                    lambda x: x in ("y", "n"),
+                    default_value="y",
+                )
+                == "y"
+            )
         ):
             # Start auto subnets creation in the absence of qualified subnets.
             # Otherwise, user selects between manual and automate subnets creation
             if not qualified_head_node_subnets or not qualified_compute_subnets:
                 print("There are no qualified subnets. Starting automatic creation of subnets...")
             vpc_parameters.update(
                 automate_subnet_creation(
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/networking.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/networking.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/subnet_computation.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/subnet_computation.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/configure/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/dcv_connect.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         except Exception as e:
             attempts -= 1
             if not attempts:
                 raise e
 
             LOGGER.debug("%s, retrying in %s seconds..", e, wait)
             time.sleep(wait)
+    return None
 
 
 class DcvConnectCommand(CliCommand):
     """Implement pcluster dcv connect command."""
 
     # CLI
     name = "dcv-connect"
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/dcv_util.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 from pcluster.constants import SUPPORTED_OSES
 
 
 def get_supported_dcv_os(architecture):
     """Return a list of all the operating system supported by DCV."""
     architectures_dict = {
         "x86_64": SUPPORTED_OSES,
-        "arm64": ["ubuntu1804", "alinux2", "centos7"],
+        "arm64": ["ubuntu1804", "alinux2", "centos7", "rhel8"],
     }
     return architectures_dict.get(architecture, [])
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/image_logs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/image_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/ssh.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/commands/version.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/entrypoint.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/exceptions.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/logger.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/logger.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/middleware.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/cli/model.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/model.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/config/cluster_config.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/cluster_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,33 +27,38 @@
 from pcluster.config.common import Imds as TopLevelImds
 from pcluster.config.common import Resource
 from pcluster.constants import (
     CIDR_ALL_IPS,
     CW_DASHBOARD_ENABLED_DEFAULT,
     CW_LOGS_ENABLED_DEFAULT,
     CW_LOGS_RETENTION_DAYS_DEFAULT,
+    CW_LOGS_ROTATION_ENABLED_DEFAULT,
     DEFAULT_EPHEMERAL_DIR,
     DEFAULT_MAX_COUNT,
     DEFAULT_MIN_COUNT,
     DELETE_POLICY,
+    DETAILED_MONITORING_ENABLED_DEFAULT,
     EBS_VOLUME_SIZE_DEFAULT,
     EBS_VOLUME_TYPE_DEFAULT,
     EBS_VOLUME_TYPE_DEFAULT_US_ISO,
     EBS_VOLUME_TYPE_IOPS_DEFAULT,
     LUSTRE,
+    MAX_COMPUTE_RESOURCES_PER_QUEUE,
     MAX_EBS_COUNT,
     MAX_EXISTING_STORAGE_COUNT,
     MAX_NEW_STORAGE_COUNT,
-    MAX_NUMBER_OF_COMPUTE_RESOURCES,
+    MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER,
     MAX_NUMBER_OF_QUEUES,
     NODE_BOOTSTRAP_TIMEOUT,
     ONTAP,
     OPENZFS,
     SCHEDULER_PLUGIN_INTERFACE_VERSION,
     SCHEDULER_PLUGIN_INTERFACE_VERSION_LOW_RANGE,
+    SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES,
+    SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES,
     SUPPORTED_OSES,
     Feature,
 )
 from pcluster.utils import (
     get_attr,
     get_installed_version,
     get_partition,
@@ -90,27 +95,29 @@
     HostedZoneValidator,
     InstanceArchitectureCompatibilityValidator,
     IntelHpcArchitectureValidator,
     IntelHpcOsValidator,
     ManagedFsxMultiAzValidator,
     MaxCountValidator,
     MixedSecurityGroupOverwriteValidator,
+    MultiNetworkInterfacesInstancesValidator,
     NameValidator,
     NumberOfStorageValidator,
     OverlappingMountDirValidator,
     RegionValidator,
+    RootVolumeEncryptionConsistencyValidator,
     RootVolumeSizeValidator,
     SchedulableMemoryValidator,
     SchedulerOsValidator,
     SchedulerValidator,
     SharedStorageMountDirValidator,
     SharedStorageNameValidator,
     UnmanagedFsxMultiAzValidator,
 )
-from pcluster.validators.common import ValidatorContext
+from pcluster.validators.common import ValidatorContext, get_async_timed_validator_type_for
 from pcluster.validators.database_validators import DatabaseUriValidator
 from pcluster.validators.directory_service_validators import (
     AdditionalSssdConfigsValidator,
     DomainAddrValidator,
     DomainNameValidator,
     LdapTlsReqCertValidator,
     PasswordSecretArnValidator,
@@ -161,14 +168,15 @@
     InstancesAllocationStrategyValidator,
     InstancesCPUValidator,
     InstancesEFAValidator,
     InstancesMemorySchedulingValidator,
     InstancesNetworkingValidator,
 )
 from pcluster.validators.kms_validators import KmsKeyIdEncryptedValidator, KmsKeyValidator
+from pcluster.validators.monitoring_validators import DetailedMonitoringValidator, LogRotationValidator
 from pcluster.validators.networking_validators import (
     ElasticIpValidator,
     MultiAzPlacementGroupValidator,
     QueueSubnetsValidator,
     SecurityGroupsValidator,
     SingleInstanceTypeSubnetValidator,
     SubnetsValidator,
@@ -184,14 +192,22 @@
     PluginInterfaceVersionValidator,
     SchedulerPluginOsArchitectureValidator,
     SchedulerPluginRegionValidator,
     SudoPrivilegesValidator,
     SupportedVersionsValidator,
     UserNameValidator,
 )
+from pcluster.validators.slurm_settings_validator import (
+    SLURM_SETTINGS_DENY_LIST,
+    CustomSlurmNodeNamesValidator,
+    CustomSlurmSettingLevel,
+    CustomSlurmSettingsIncludeFileOnlyValidator,
+    CustomSlurmSettingsValidator,
+)
+from pcluster.validators.tags_validators import ComputeResourceTagsValidator
 
 LOGGER = logging.getLogger(__name__)
 
 # pylint: disable=C0302
 
 # ---------------------- Storage ---------------------- #
 
@@ -749,41 +765,72 @@
 
     def __init__(self, enabled: bool = None, gdr_support: bool = None, **kwargs):
         super().__init__(**kwargs)
         self.enabled = enabled
         self.gdr_support = Resource.init_param(gdr_support, default=False)
 
 
+# ---------------------- Health Checks ---------------------- #
+
+
+class GpuHealthCheck(Resource):
+    """Represent the configuration for the GPU Health Check."""
+
+    def __init__(self, enabled: bool = None, **kwargs):
+        super().__init__(**kwargs)
+        self.enabled = enabled
+
+
+class HealthChecks(Resource):
+    """Represent the health checks configuration."""
+
+    def __init__(self, gpu: GpuHealthCheck = None, **kwargs):
+        super().__init__(**kwargs)
+        self.gpu = gpu or GpuHealthCheck(implied=True)
+
+
 # ---------------------- Monitoring ---------------------- #
 
 
 class CloudWatchLogs(Resource):
     """Represent the CloudWatch configuration in Logs."""
 
     def __init__(self, enabled: bool = None, retention_in_days: int = None, deletion_policy: str = None, **kwargs):
         super().__init__(**kwargs)
         self.enabled = Resource.init_param(enabled, default=CW_LOGS_ENABLED_DEFAULT)
         self.retention_in_days = Resource.init_param(retention_in_days, default=CW_LOGS_RETENTION_DAYS_DEFAULT)
         self.deletion_policy = Resource.init_param(deletion_policy, default="Retain")
 
 
+class LogRotation(Resource):
+    """Represent the Rotation configuration in Logs."""
+
+    def __init__(self, enabled: bool = None, **kwargs):
+        super().__init__(**kwargs)
+        self.enabled = Resource.init_param(enabled, default=CW_LOGS_ROTATION_ENABLED_DEFAULT)
+
+
 class CloudWatchDashboards(Resource):
     """Represent the CloudWatch Dashboard."""
 
     def __init__(self, enabled: bool = None, **kwargs):
         super().__init__(**kwargs)
         self.enabled = Resource.init_param(enabled, default=CW_DASHBOARD_ENABLED_DEFAULT)
 
 
 class Logs(Resource):
     """Represent the CloudWatch Logs configuration."""
 
-    def __init__(self, cloud_watch: CloudWatchLogs = None, **kwargs):
+    def __init__(self, cloud_watch: CloudWatchLogs = None, rotation: LogRotation = None, **kwargs):
         super().__init__(**kwargs)
         self.cloud_watch = cloud_watch or CloudWatchLogs(implied=True)
+        self.rotation = rotation or LogRotation(implied=True)
+
+    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
+        self._register_validator(LogRotationValidator, log=self)
 
 
 class Dashboards(Resource):
     """Represent the Dashboards configuration."""
 
     def __init__(self, cloud_watch: CloudWatchDashboards = None, **kwargs):
         super().__init__(**kwargs)
@@ -791,18 +838,21 @@
 
 
 class Monitoring(Resource):
     """Represent the Monitoring configuration."""
 
     def __init__(self, detailed_monitoring: bool = None, logs: Logs = None, dashboards: Dashboards = None, **kwargs):
         super().__init__(**kwargs)
-        self.detailed_monitoring = Resource.init_param(detailed_monitoring, default=False)
+        self.detailed_monitoring = Resource.init_param(detailed_monitoring, default=DETAILED_MONITORING_ENABLED_DEFAULT)
         self.logs = logs or Logs(implied=True)
         self.dashboards = dashboards or Dashboards(implied=True)
 
+    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
+        self._register_validator(DetailedMonitoringValidator, is_detailed_monitoring_enabled=self.detailed_monitoring)
+
 
 # ---------------------- Others ---------------------- #
 
 
 class Tag(BaseTag):
     """Represent the Tag configuration."""
 
@@ -1081,33 +1131,33 @@
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         if self.custom_ami:
             self._register_validator(CustomAmiTagValidator, custom_ami=self.custom_ami)
 
 
 class CustomAction(Resource):
-    """Represent a custom action resource."""
+    """Represent a custom action script resource."""
 
     def __init__(self, script: str, args: List[str] = None):
         super().__init__()
         self.script = Resource.init_param(script)
         self.args = Resource.init_param(args)
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        self._register_validator(UrlValidator, url=self.script)
+        self._register_validator(get_async_timed_validator_type_for(UrlValidator), url=self.script, timeout=5)
 
 
 class CustomActions(Resource):
     """Represent a custom action resource."""
 
     def __init__(
         self,
-        on_node_start: CustomAction = None,
-        on_node_configured: CustomAction = None,
-        on_node_updated: CustomAction = None,
+        on_node_start=None,
+        on_node_configured=None,
+        on_node_updated=None,
     ):
         super().__init__()
         self.on_node_start = Resource.init_param(on_node_start)
         self.on_node_configured = Resource.init_param(on_node_configured)
         self.on_node_updated = Resource.init_param(on_node_updated)
 
 
@@ -1273,14 +1323,16 @@
         self.cluster_template_body = None
         self.source_config = None
         self.config_version = ""
         self.original_config_version = ""
         self._official_ami = None
         self.imds = imds or TopLevelImds(implied="v1.0")
         self.deployment_settings = deployment_settings
+        self.managed_head_node_security_group = None
+        self.managed_compute_security_group = None
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         self._register_validator(RegionValidator, region=self.region)
         self._register_validator(ClusterNameValidator, name=self.cluster_name, scheduling=self.scheduling)
         self._register_validator(
             ArchitectureOsValidator,
             os=self.image.os,
@@ -1304,15 +1356,15 @@
         )
         self._register_storage_validators()
         self._register_validator(
             HeadNodeLaunchTemplateValidator,
             head_node=self.head_node,
             os=self.image.os,
             ami_id=self.head_node_ami,
-            tags=self.get_cluster_tags(),
+            tags=self.get_tags(),
             imds_support=self.imds.imds_support,
         )
         if self.head_node.dcv:
             self._register_validator(FeatureRegionValidator, feature=Feature.DCV, region=self.region)
             self._register_validator(
                 DcvValidator,
                 instance_type=self.head_node.instance_type,
@@ -1406,23 +1458,23 @@
                 elif isinstance(storage, SharedEfs):
                     if storage.file_system_id:
                         existing_storage_count["efs"] += 1
                         self._register_validator(
                             EfsIdValidator,
                             efs_id=storage.file_system_id,
                             avail_zones_mapping=self.availability_zones_subnets_mapping,
-                            are_all_security_groups_customized=self.are_all_security_groups_customized,
+                            security_groups_by_nodes=self.security_groups_by_nodes,
                         )
                     else:
                         new_storage_count["efs"] += 1
             self._register_validator(
                 ExistingFsxNetworkingValidator,
                 file_system_ids=list(existing_fsx),
-                head_node_subnet_id=self.head_node.networking.subnet_id,
-                are_all_security_groups_customized=self.are_all_security_groups_customized,
+                subnet_ids=[self.head_node.networking.subnet_id] + self.compute_subnet_ids,
+                security_groups_by_nodes=self.security_groups_by_nodes,
             )
 
             self._validate_max_storage_count(ebs_count, existing_storage_count, new_storage_count)
             self._validate_new_storage_multiple_subnets(
                 self.scheduling.queues, self.compute_subnet_ids, new_storage_count
             )
 
@@ -1629,39 +1681,70 @@
         return (
             self.monitoring.logs.cloud_watch.enabled
             if self.monitoring and self.monitoring.logs and self.monitoring.logs.cloud_watch
             else False
         )
 
     @property
+    def is_log_rotation_enabled(self):
+        """Return True if log rotation is enabled."""
+        return (
+            self.monitoring.logs.rotation.enabled
+            if self.monitoring and self.monitoring.logs and self.monitoring.logs.rotation
+            else False
+        )
+
+    @property
     def is_cw_dashboard_enabled(self):
         """Return True if CloudWatch Dashboard is enabled."""
         return (
             self.monitoring.dashboards.cloud_watch.enabled
             if self.monitoring and self.monitoring.dashboards and self.monitoring.dashboards.cloud_watch
             else False
         )
 
     @property
+    def is_detailed_monitoring_enabled(self):
+        """Return True if Detailed Monitoring is enabled."""
+        return self.monitoring.detailed_monitoring
+
+    @property
     def is_dcv_enabled(self):
         """Return True if DCV is enabled."""
         return self.head_node.dcv and self.head_node.dcv.enabled
 
     @property
-    def are_all_security_groups_customized(self):
-        """Return True if all head node and queues have (additional) security groups specified."""
+    def security_groups_by_nodes(self):
+        """
+        Return Security groups by nodes.
+
+        The result is a set of frozenset,
+        e.g. {frozenset(security groups for head node), frozenset(security groups for queue 1), ...}
+        """
         head_node_networking = self.head_node.networking
-        if not (head_node_networking.security_groups or head_node_networking.additional_security_groups):
-            return False
+        security_groups_for_head_node = set()
+        if head_node_networking.security_groups:
+            security_groups_for_head_node.update(set(head_node_networking.security_groups))
+        else:
+            security_groups_for_head_node.add(self.managed_head_node_security_group)
+        if head_node_networking.additional_security_groups:
+            security_groups_for_head_node.update(set(head_node_networking.additional_security_groups))
+        security_groups_for_all_nodes = {frozenset(security_groups_for_head_node)}
         for queue in self.scheduling.queues:
             queue_networking = queue.networking
             if isinstance(queue_networking, _QueueNetworking):
-                if not (queue_networking.security_groups or queue_networking.additional_security_groups):
-                    return False
-        return True
+                security_groups_for_compute_node = set()
+                if queue_networking.security_groups:
+                    security_groups_for_compute_node.update(set(queue_networking.security_groups))
+                else:
+                    security_groups_for_compute_node.add(self.managed_compute_security_group)
+                if queue_networking.additional_security_groups:
+                    security_groups_for_compute_node.update(set(queue_networking.additional_security_groups))
+                security_groups_for_all_nodes.add(frozenset(security_groups_for_compute_node))
+        return security_groups_for_all_nodes
 
     @property
     def extra_chef_attributes(self):
         """Return extra chef attributes."""
         return (
             self.dev_settings.cookbook.extra_chef_attributes
             if self.dev_settings and self.dev_settings.cookbook and self.dev_settings.cookbook.extra_chef_attributes
@@ -1702,18 +1785,22 @@
         self._official_ami = value
 
     @property
     def lambda_functions_vpc_config(self):
         """Return the vpc config of the PCluster Lambda Functions or None."""
         return self.deployment_settings.lambda_functions_vpc_config if self.deployment_settings else None
 
-    def get_cluster_tags(self):
+    def get_tags(self):
         """Return tags configured in the cluster configuration."""
         return self.tags
 
+    def get_instance_types_data(self) -> dict:
+        """Get instance type infos for all instance types used in the configuration file."""
+        return {}
+
 
 class AwsBatchComputeResource(BaseComputeResource):
     """Represent the AwsBatch Compute Resource."""
 
     def __init__(
         self,
         instance_types: List[str] = None,
@@ -1821,14 +1908,17 @@
         min_count: int = None,
         spot_price: float = None,
         efa: Efa = None,
         disable_simultaneous_multithreading: bool = None,
         schedulable_memory: int = None,
         capacity_reservation_target: CapacityReservationTarget = None,
         networking: SlurmComputeResourceNetworking = None,
+        health_checks: HealthChecks = None,
+        custom_slurm_settings: Dict = None,
+        tags: List[Tag] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.max_count = Resource.init_param(max_count, default=DEFAULT_MAX_COUNT)
         self.min_count = Resource.init_param(min_count, default=DEFAULT_MIN_COUNT)
         self.spot_price = Resource.init_param(spot_price)
         self.disable_simultaneous_multithreading = Resource.init_param(
@@ -1836,14 +1926,17 @@
         )
         self.efa = efa or Efa(enabled=False, implied=True)
         self.schedulable_memory = Resource.init_param(schedulable_memory)
         self.capacity_reservation_target = capacity_reservation_target
         self._instance_types_with_instance_storage = []
         self._instance_type_info_map = {}
         self.networking = networking or SlurmComputeResourceNetworking(implied=True)
+        self.health_checks = health_checks or HealthChecks(implied=True)
+        self.custom_slurm_settings = Resource.init_param(custom_slurm_settings, default={})
+        self.tags = tags
 
     @staticmethod
     def fetch_instance_type_info(instance_type) -> InstanceTypeInfo:
         """Return instance type information."""
         return AWSApi.instance().ec2.get_instance_type_info(instance_type)
 
     @property
@@ -1886,27 +1979,35 @@
         )
 
     @property
     @abstractmethod
     def instance_types(self) -> List[str]:
         pass
 
+    def get_tags(self):
+        """Return tags configured in the slurm compute resource configuration."""
+        return self.tags
+
 
 class FlexibleInstanceType(Resource):
     """Represent an instance type listed in the Instances of a ComputeResources."""
 
     def __init__(self, instance_type: str, **kwargs):
         super().__init__(**kwargs)
         self.instance_type = Resource.init_param(instance_type)
 
 
 class SlurmFlexibleComputeResource(_BaseSlurmComputeResource):
     """Represents a Slurm Compute Resource with Multiple Instance Types."""
 
-    def __init__(self, instances: List[FlexibleInstanceType], **kwargs):
+    def __init__(
+        self,
+        instances: List[FlexibleInstanceType],
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         self.instances = Resource.init_param(instances)
 
     @property
     def instance_types(self) -> List[str]:
         """Return list of instance type names in this compute resource."""
         return [
@@ -1935,15 +2036,19 @@
                     least_max_nics = max_nics
         return least_max_nics
 
 
 class SlurmComputeResource(_BaseSlurmComputeResource):
     """Represents a Slurm Compute Resource with a Single Instance Type."""
 
-    def __init__(self, instance_type, **kwargs):
+    def __init__(
+        self,
+        instance_type,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         self.instance_type = Resource.init_param(instance_type)
         self.__instance_type_info = None
 
     @property
     def instance_types(self) -> List[str]:
         """List of instance types under this compute resource."""
@@ -2046,14 +2151,18 @@
             return None
 
     @property
     def multi_az_enabled(self):
         """Return true if more than one AZ are defined in the queue Networking section."""
         return len(self.networking.az_list) > 1
 
+    def get_tags(self):
+        """Return tags configured in the queue configuration."""
+        return None
+
     def get_managed_placement_group_keys(self) -> List[str]:
         managed_placement_group_keys = []
         for compute_resource in self.compute_resources:
             placement_group_setting = self.get_placement_group_settings_for_compute_resource(compute_resource)
             if placement_group_setting.get("is_managed"):
                 managed_placement_group_keys.append(placement_group_setting.get("key"))
         return managed_placement_group_keys
@@ -2124,17 +2233,23 @@
 
 class SlurmQueue(_CommonQueue):
     """Represents a Slurm Queue that has Compute Resources with both Single and Multiple Instance Types."""
 
     def __init__(
         self,
         allocation_strategy: str = None,
+        custom_slurm_settings: Dict = None,
+        health_checks: HealthChecks = None,
+        tags: List[Tag] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
+        self.health_checks = health_checks or HealthChecks(implied=True)
+        self.custom_slurm_settings = Resource.init_param(custom_slurm_settings, default={})
+        self.tags = tags
         if any(
             isinstance(compute_resource, SlurmFlexibleComputeResource) for compute_resource in self.compute_resources
         ):
             self.allocation_strategy = (
                 AllocationStrategy[to_snake_case(allocation_strategy).upper()]
                 if allocation_strategy
                 else AllocationStrategy.LOWEST_PRICE
@@ -2152,39 +2267,50 @@
     def instance_types_with_instance_storage(self):
         """Return a set of instance types in the queue that have instance store."""
         result = set()
         for compute_resource in self.compute_resources:
             result.update(compute_resource.instance_types_with_instance_storage)
         return result
 
+    def get_tags(self):
+        """Return tags configured in the slurm queue configuration."""
+        return self.tags
+
     def _register_validators(self, context: ValidatorContext = None):
         super()._register_validators(context)
         self._register_validator(
             DuplicateNameValidator,
             name_list=[compute_resource.name for compute_resource in self.compute_resources],
             resource_name="Compute resource",
         )
         self._register_validator(
             MaxCountValidator,
             resources_length=len(self.compute_resources),
-            max_length=MAX_NUMBER_OF_COMPUTE_RESOURCES,
-            resource_name="ComputeResources",
+            max_length=MAX_COMPUTE_RESOURCES_PER_QUEUE,
+            resource_name="ComputeResources per Queue",
         )
         self._register_validator(
             QueueSubnetsValidator,
             queue_name=self.name,
             subnet_ids=self.networking.subnet_ids,
             az_subnet_ids_mapping=self.networking.az_subnet_ids_mapping,
         )
         if any(isinstance(compute_resource, SlurmComputeResource) for compute_resource in self.compute_resources):
             self._register_validator(
                 SingleInstanceTypeSubnetValidator,
                 queue_name=self.name,
                 subnet_ids=self.networking.subnet_ids,
             )
+        if self.custom_slurm_settings:
+            self._register_validator(
+                CustomSlurmSettingsValidator,
+                custom_settings=[self.custom_slurm_settings],
+                deny_list=SLURM_SETTINGS_DENY_LIST["Queue"]["Global"],
+                settings_level=CustomSlurmSettingLevel.QUEUE,
+            )
         for compute_resource in self.compute_resources:
             self._register_validator(
                 EfaSecurityGroupValidator,
                 efa_enabled=compute_resource.efa.enabled,
                 security_groups=self.networking.security_groups,
                 additional_security_groups=self.networking.additional_security_groups,
             )
@@ -2194,14 +2320,21 @@
                 placement_group_key=self.get_placement_group_settings_for_compute_resource(compute_resource).get("key"),
                 placement_group_disabled=self.get_chosen_placement_group_setting_for_compute_resource(
                     compute_resource
                 ).enabled
                 is False,
                 multi_az_enabled=self.multi_az_enabled,
             )
+            if compute_resource.custom_slurm_settings:
+                self._register_validator(
+                    CustomSlurmSettingsValidator,
+                    custom_settings=[compute_resource.custom_slurm_settings],
+                    deny_list=SLURM_SETTINGS_DENY_LIST["ComputeResource"]["Global"],
+                    settings_level=CustomSlurmSettingLevel.COMPUTE_RESOURCE,
+                )
             for instance_type in compute_resource.instance_types:
                 self._register_validator(
                     CapacityTypeValidator,
                     capacity_type=self.capacity_type,
                     instance_type=instance_type,
                 )
 
@@ -2252,24 +2385,53 @@
     def __init__(
         self,
         scaledown_idletime: int = None,
         dns: Dns = None,
         queue_update_strategy: str = None,
         enable_memory_based_scheduling: bool = None,
         database: Database = None,
+        custom_slurm_settings: List[Dict] = None,
+        custom_slurm_settings_include_file: str = None,
         **kwargs,
     ):
         super().__init__()
         self.scaledown_idletime = Resource.init_param(scaledown_idletime, default=10)
         self.dns = dns or Dns(implied=True)
         self.queue_update_strategy = Resource.init_param(
             queue_update_strategy, default=QueueUpdateStrategy.COMPUTE_FLEET_STOP.value
         )
         self.enable_memory_based_scheduling = Resource.init_param(enable_memory_based_scheduling, default=False)
         self.database = database
+        self.custom_slurm_settings = Resource.init_param(custom_slurm_settings)
+        self.custom_slurm_settings_include_file = Resource.init_param(custom_slurm_settings_include_file)
+
+    def _register_validators(self, context: ValidatorContext = None):
+        super()._register_validators(context)
+        if self.custom_slurm_settings:  # if not empty register validator
+            self._register_validator(
+                CustomSlurmSettingsValidator,
+                custom_settings=self.custom_slurm_settings,
+                deny_list=SLURM_SETTINGS_DENY_LIST["SlurmConf"]["Global"],
+                settings_level=CustomSlurmSettingLevel.SLURM_CONF,
+            )
+            self._register_validator(CustomSlurmNodeNamesValidator, custom_settings=self.custom_slurm_settings)
+            if self.database:
+                self._register_validator(
+                    CustomSlurmSettingsValidator,
+                    custom_settings=self.custom_slurm_settings,
+                    deny_list=SLURM_SETTINGS_DENY_LIST["SlurmConf"]["Accounting"],
+                    settings_level=CustomSlurmSettingLevel.SLURM_CONF,
+                )
+        if self.custom_slurm_settings_include_file:
+            self._register_validator(UrlValidator, url=self.custom_slurm_settings_include_file)
+            self._register_validator(
+                CustomSlurmSettingsIncludeFileOnlyValidator,
+                custom_settings=self.custom_slurm_settings,
+                include_file_url=self.custom_slurm_settings_include_file,
+            )
 
 
 class QueueUpdateStrategy(Enum):
     """Enum to identify the update strategy supported by the queue."""
 
     DRAIN = "DRAIN"
     COMPUTE_FLEET_STOP = "COMPUTE_FLEET_STOP"
@@ -2286,19 +2448,31 @@
         self.settings = settings or SlurmSettings(implied=True)
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         self._register_validator(
             DuplicateNameValidator, name_list=[queue.name for queue in self.queues], resource_name="Queue"
         )
         self._register_validator(
+            RootVolumeEncryptionConsistencyValidator,
+            encryption_settings=[
+                (queue.name, queue.compute_settings.local_storage.root_volume.encrypted) for queue in self.queues
+            ],
+        )
+        self._register_validator(
             MaxCountValidator,
             resources_length=len(self.queues),
             max_length=MAX_NUMBER_OF_QUEUES,
             resource_name="SlurmQueues",
         )
+        self._register_validator(
+            MaxCountValidator,
+            resources_length=sum(len(queue.compute_resources) for queue in self.queues),
+            max_length=MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER,
+            resource_name="ComputeResources per Cluster",
+        )
 
 
 class SchedulerPluginQueue(_CommonQueue):
     """Represent the Scheduler Plugin queue."""
 
     def __init__(
         self,
@@ -2312,14 +2486,20 @@
         super()._register_validators(context)
         self._register_validator(
             DuplicateNameValidator,
             name_list=[compute_resource.name for compute_resource in self.compute_resources],
             resource_name="Compute resource",
         )
         self._register_validator(
+            MaxCountValidator,
+            resources_length=len(self.compute_resources),
+            max_length=SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES,
+            resource_name="ComputeResources per Queue",
+        )
+        self._register_validator(
             QueueSubnetsValidator,
             queue_name=self.name,
             subnet_ids=self.networking.subnet_ids,
             az_subnet_ids_mapping=self.networking.az_subnet_ids_mapping,
         )
         if any(isinstance(compute_resource, SlurmComputeResource) for compute_resource in self.compute_resources):
             self._register_validator(
@@ -2373,23 +2553,23 @@
 
 
 class SchedulerPluginQueueConstraints(Resource):
     """Represent the Queue Constraints for a Scheduler Plugin."""
 
     def __init__(self, max_count: int = None, **kwargs):
         super().__init__(**kwargs)
-        self.max_count = Resource.init_param(max_count, default=MAX_NUMBER_OF_QUEUES)
+        self.max_count = Resource.init_param(max_count, default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES)
 
 
 class SchedulerPluginComputeResourceConstraints(Resource):
     """Represent the Compute Resource Constraints for a Scheduler Plugin."""
 
     def __init__(self, max_count: int = None, **kwargs):
         super().__init__(**kwargs)
-        self.max_count = Resource.init_param(max_count, default=MAX_NUMBER_OF_COMPUTE_RESOURCES)
+        self.max_count = Resource.init_param(max_count, default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES)
 
 
 class SchedulerPluginRequirements(Resource):
     """Represent the Requirements for a Scheduler Plugin."""
 
     def __init__(
         self,
@@ -2652,47 +2832,49 @@
         )
         self._register_validator(
             MaxCountValidator,
             resources_length=len(self.queues),
             max_length=get_attr(
                 self.settings.scheduler_definition,
                 "requirements.queue_constraints.max_count",
-                default=MAX_NUMBER_OF_QUEUES,
+                default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES,
             ),
             resource_name="SchedulerQueues",
         )
         for queue in self.queues:
             self._register_validator(
                 MaxCountValidator,
                 resources_length=len(queue.compute_resources),
                 max_length=get_attr(
                     self.settings.scheduler_definition,
                     "requirements.compute_resource_constraints.max_count",
-                    default=MAX_NUMBER_OF_COMPUTE_RESOURCES,
+                    default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES,
                 ),
                 resource_name="ComputeResources",
             )
 
 
 class CommonSchedulerClusterConfig(BaseClusterConfig):
     """Represent the common Cluster configuration between Slurm Config and Scheduler Plugin Config."""
 
     def _register_validators(self, context: ValidatorContext = None):
         super()._register_validators(context)
         checked_images = []
-        for queue in self.scheduling.queues:
+        for index, queue in enumerate(self.scheduling.queues):
             queue_image = self.image_dict[queue.name]
-            self._register_validator(
-                ComputeResourceLaunchTemplateValidator,
-                queue=queue,
-                ami_id=queue_image,
-                os=self.image.os,
-                tags=self.get_cluster_tags(),
-                imds_support=self.imds.imds_support,
-            )
+            if index == 0:
+                # Execute LaunchTemplateValidator only for the first queue
+                self._register_validator(
+                    ComputeResourceLaunchTemplateValidator,
+                    queue=queue,
+                    ami_id=queue_image,
+                    os=self.image.os,
+                    tags=self.get_tags(),
+                    imds_support=self.imds.imds_support,
+                )
             ami_volume_size = AWSApi.instance().ec2.describe_image(queue_image).volume_size
             root_volume = queue.compute_settings.local_storage.root_volume
             root_volume_size = root_volume.size
             if root_volume_size is None:  # If root volume size is not specified, it will be the size of the AMI.
                 root_volume_size = ami_volume_size
             self._register_validator(
                 RootVolumeSizeValidator,
@@ -2807,14 +2989,22 @@
             capacity_reservation_ids.update(
                 AWSApi.instance().resource_groups.get_capacity_reservation_ids_from_group_resources(
                     capacity_reservation_resource_group_arn
                 )
             )
         return list(capacity_reservation_ids)
 
+    @property
+    def has_custom_actions_in_queue(self):
+        """Return True if any queues have custom scripts."""
+        for queue in self.scheduling.queues:
+            if queue.custom_actions:
+                return True
+        return False
+
 
 class SchedulerPluginClusterConfig(CommonSchedulerClusterConfig):
     """Represent the full Scheduler Plugin Cluster configuration."""
 
     def __init__(self, cluster_name: str, scheduling: SchedulerPluginScheduling, **kwargs):
         super().__init__(cluster_name, **kwargs)
         self.scheduling = scheduling
@@ -2835,15 +3025,15 @@
         result[instance_type_info.instance_type()] = instance_type_info.instance_type_data
         for queue in self.scheduling.queues:
             for compute_resource in queue.compute_resources:
                 instance_type_info = compute_resource.instance_type_info
                 result[instance_type_info.instance_type()] = instance_type_info.instance_type_data
         return result
 
-    def get_cluster_tags(self):
+    def get_tags(self):
         """Return tags configured in the root of the cluster config and under scheduler definition."""
         return (self.tags if self.tags else []) + get_attr(
             self.scheduling, "settings.scheduler_definition.tags", default=[]
         )
 
     def _register_validators(self, context: ValidatorContext = None):
         super()._register_validators(context)
@@ -2916,14 +3106,15 @@
                 HostedZoneValidator,
                 hosted_zone_id=self.scheduling.settings.dns.hosted_zone_id,
                 cluster_vpc=self.vpc_id,
                 cluster_name=self.cluster_name,
             )
 
         instance_types_data = self.get_instance_types_data()
+        self._register_validator(MultiNetworkInterfacesInstancesValidator, queues=self.scheduling.queues)
         for queue in self.scheduling.queues:
             for compute_resource in queue.compute_resources:
                 if self.scheduling.settings.enable_memory_based_scheduling:
                     for instance_type in compute_resource.instance_types:
                         self._register_validator(
                             InstanceTypeMemoryInfoValidator,
                             instance_type=instance_type,
@@ -2960,14 +3151,22 @@
                         InstancesEFAValidator,
                         InstancesNetworkingValidator,
                         InstancesAllocationStrategyValidator,
                         InstancesMemorySchedulingValidator,
                     ]
                     for validator in flexible_instance_types_validators:
                         self._register_validator(validator, **validator_args)
+                self._register_validator(
+                    ComputeResourceTagsValidator,
+                    queue_name=queue.name,
+                    compute_resource_name=compute_resource.name,
+                    cluster_tags=self.get_tags(),
+                    queue_tags=queue.get_tags(),
+                    compute_resource_tags=compute_resource.get_tags(),
+                )
 
     @property
     def image_dict(self):
         """Return image dict of queues, key is queue name, value is image id."""
         if self.__image_dict:
             return self.__image_dict
         self.__image_dict = {}
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/config/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # This module contains all the classes representing the Resources objects.
 # These objects are obtained from the configuration file through a conversion based on the Schema classes.
 #
+import asyncio
+import itertools
 import json
 import logging
 from abc import ABC, abstractmethod
 from typing import List, Set
 
-from pcluster.validators.common import FailureLevel, ValidationResult, Validator, ValidatorContext
+from pcluster.validators.common import AsyncValidator, FailureLevel, ValidationResult, Validator, ValidatorContext
 from pcluster.validators.iam_validators import AdditionalIamPolicyValidator
 from pcluster.validators.networking_validators import LambdaFunctionsVpcConfigValidator
 from pcluster.validators.s3_validators import UrlValidator
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -118,14 +120,15 @@
 
         def __repr__(self):
             return repr(self.value)
 
     def __init__(self, implied: bool = False):
         # Parameters registry
         self.__params = {}
+        self._validation_futures = []
         self._validation_failures: List[ValidationResult] = []
         self._validators: List = []
         self.implied = implied
 
     @property
     def params(self):
         """Return the params registry for this Resource."""
@@ -163,63 +166,124 @@
         super().__setattr__(key, value)
 
     @staticmethod
     def init_param(value, default=None, update_policy=None):
         """Create a resource attribute backed by a Configuration Parameter."""
         return Resource.Param(value, default=default, update_policy=update_policy)
 
-    def _validator_execute(self, validator_class, validator_args, suppressors):
+    @staticmethod
+    def _validator_execute(validator_class, validator_args, suppressors, validation_executor):
         validator = validator_class()
+
         if any(suppressor.suppress_validator(validator) for suppressor in (suppressors or [])):
             LOGGER.debug("Suppressing validator %s", validator_class.__name__)
-            return []
+            return None
+
         LOGGER.debug("Executing validator %s", validator_class.__name__)
+        return validation_executor(validator_args, validator)
+
+    @staticmethod
+    def _validator_execute_sync(validator_args, validator):
         try:
             return validator.execute(**validator_args)
         except Exception as e:
+            LOGGER.debug("Validator %s unexpected failure: %s", validator.type, e)
             return [ValidationResult(str(e), FailureLevel.ERROR, validator.type)]
 
+    @staticmethod
+    def _validator_execute_async(validator_args, validator):
+        return validator.execute_async(**validator_args)
+
+    def _await_async_validators(self):
+        # here could be a good spot to add a cascading timeout for the async validators
+        # if they are taking too long to execute for a resource and its children since the use of
+        # get_async_timed_validator_type_for allows to decorate only on single validator at a time and
+        # does not cascade to child resources
+        return list(
+            itertools.chain.from_iterable(
+                asyncio.get_event_loop().run_until_complete(asyncio.gather(*self._validation_futures))
+            )
+        )
+
     def _nested_resources(self):
         nested_resources = []
         for _, value in self.__dict__.items():
             if isinstance(value, Resource):
                 nested_resources.append(value)
             if isinstance(value, list) and value:
                 nested_resources.extend(item for item in value if isinstance(item, Resource))
         return nested_resources
 
     def validate(
-        self, suppressors: List[ValidatorSuppressor] = None, context: ValidatorContext = None
-    ) -> List[ValidationResult]:
-        """Execute registered validators."""
-        # Cleanup failures and validators
+        self, suppressors: List[ValidatorSuppressor] = None, context: ValidatorContext = None, nested: bool = False
+    ):
+        """
+        Execute registered validators.
+
+        The "nested" parameter is used only for internal recursive calls to distinguish those from the top level
+        one where the async validators results should be awaited for.
+        """
+        # this validation logic is a responsibility that could be completely separated from the resource tree
+        # also until we need to support both sync and async validation this logic will be unnecessarily complex
+        # embracing async validation completely is possible and will greatly simplify this
+        self._validation_futures.clear()
         self._validation_failures.clear()
 
+        try:
+            self._validate_nested_resources(context, suppressors)
+            self._validate_self(context, suppressors)
+        finally:
+            if nested:
+                result = self._validation_failures, self._validation_futures.copy()
+            else:
+                self._validation_failures.extend(self._await_async_validators())
+                result = self._validation_failures
+            self._validation_futures.clear()
+
+        return result
+
+    def _validate_nested_resources(self, context, suppressors):
         # Call validators for nested resources
         for nested_resource in self._nested_resources():
-            self._validation_failures.extend(nested_resource.validate(suppressors, context))
+            failures, futures = nested_resource.validate(suppressors, context, nested=True)
+            self._validation_futures.extend(futures)
+            self._validation_failures.extend(failures)
 
-        # Update validators to be executed according to current status of the model and order by priority
+    def _validate_self(self, context, suppressors):
         self._validators.clear()
         self._register_validators(context)
         for validator in self._validators:
-            self._validation_failures.extend(self._validator_execute(*validator, suppressors))
-
-        return self._validation_failures
+            if issubclass(validator[0], AsyncValidator):
+                result = self._validator_execute(*validator, suppressors, self._validator_execute_async)
+                if result:
+                    self._validation_futures.extend([result])
+            else:
+                self._validation_failures.extend(
+                    self._validator_execute(*validator, suppressors, self._validator_execute_sync) or []
+                )
 
     def _register_validators(self, context: ValidatorContext = None):
         """
-        Execute validators.
+        Register all the validators that contribute to ensure that the resource parameters are valid.
 
-        Method to be implemented in Resources.
+        Method to be implemented in Resource subclasses that need to register validators by invoking the internal
+        _register_validator method.
+        :param context:
+        :return:
         """
         pass
 
     def _register_validator(self, validator_class, **validator_args):
-        """Execute the validator."""
+        """Add a validator with the specified arguments.
+
+        The validator will be executed according to the current status of the model and ordered by priority.
+        :param validator_class: Validator class to be executed
+        :param validator_args: Arguments to be passed to the validator
+        :return:
+        """
         self._validators.append((validator_class, validator_args))
 
     def __repr__(self):
         """Return a human readable representation of the Resource object."""
         return "<{name}({attributes})>".format(
             name=self.__class__.__name__,
             attributes=",".join(f"{attr}={repr(value)}" for attr, value in self.__dict__.items()),
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/config/config_patch.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/config_patch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/config/imagebuilder_config.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/imagebuilder_config.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/config/update_policy.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/update_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,16 +416,16 @@
 # Checks resize of max_count
 UpdatePolicy.MAX_COUNT = UpdatePolicy(
     name="MAX_COUNT",
     level=1,
     fail_reason=lambda change, patch: "Shrinking a queue requires the compute fleet to be stopped first",
     action_needed=UpdatePolicy.ACTIONS_NEEDED["pcluster_stop"],
     condition_checker=lambda change, patch: not patch.cluster.has_running_capacity()
-    or (change.new_value if change.new_value is not None else DEFAULT_MAX_COUNT)
-    >= (change.old_value if change.old_value is not None else DEFAULT_MAX_COUNT),
+    or (int(change.new_value) if change.new_value is not None else DEFAULT_MAX_COUNT)
+    >= (int(change.old_value) if change.old_value is not None else DEFAULT_MAX_COUNT),
 )
 
 # Update supported only with all compute nodes down or with replacement policy set different from COMPUTE_FLEET_STOP
 UpdatePolicy.QUEUE_UPDATE_STRATEGY = UpdatePolicy(
     name="QUEUE_UPDATE_STRATEGY",
     level=5,
     fail_reason=fail_reason_queue_update_strategy,
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/constants.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 PCLUSTER_NAME_REGEX = r"^([a-zA-Z][a-zA-Z0-9-]{0,%d})$"
 PCLUSTER_ISSUES_LINK = "https://github.com/aws/aws-parallelcluster/issues"
 
 CIDR_ALL_IPS = "0.0.0.0/0"
 
 SUPPORTED_SCHEDULERS = ["slurm", "awsbatch"]
 SCHEDULERS_SUPPORTING_IMDS_SECURED = ["slurm", "plugin"]
-SUPPORTED_OSES = ["alinux2", "centos7", "ubuntu1804", "ubuntu2004"]
+SUPPORTED_OSES = ["alinux2", "centos7", "ubuntu1804", "ubuntu2004", "rhel8"]
 SUPPORTED_OSES_FOR_SCHEDULER = {"slurm": SUPPORTED_OSES, "plugin": SUPPORTED_OSES, "awsbatch": ["alinux2"]}
 DELETE_POLICY = "Delete"
 RETAIN_POLICY = "Retain"
 DELETION_POLICIES = [DELETE_POLICY, RETAIN_POLICY]
 DELETION_POLICIES_WITH_SNAPSHOT = DELETION_POLICIES + ["Snapshot"]
 SUPPORTED_ARCHITECTURES = ["x86_64", "arm64"]
 SUPPORTED_OSES_FOR_ARCHITECTURE = {"x86_64": SUPPORTED_OSES, "arm64": SUPPORTED_OSES}
@@ -36,21 +36,23 @@
 AWSBATCH = "awsbatch"
 
 OS_MAPPING = {
     "centos7": {"user": "centos", "root-device": "/dev/sda1"},
     "alinux2": {"user": "ec2-user", "root-device": "/dev/xvda"},
     "ubuntu1804": {"user": "ubuntu", "root-device": "/dev/sda1"},
     "ubuntu2004": {"user": "ubuntu", "root-device": "/dev/sda1"},
+    "rhel8": {"user": "ec2-user", "root-device": "/dev/sda1"},
 }
 
 OS_TO_IMAGE_NAME_PART_MAP = {
     "alinux2": "amzn2-hvm",
     "centos7": "centos7-hvm",
     "ubuntu1804": "ubuntu-1804-lts-hvm",
     "ubuntu2004": "ubuntu-2004-lts-hvm",
+    "rhel8": "rhel8-hvm",
 }
 
 IMAGE_NAME_PART_TO_OS_MAP = {value: key for key, value in OS_TO_IMAGE_NAME_PART_MAP.items()}
 
 # Describe the list of requirements to be satisfied by the Pcluster AWS Batch CLI to manage the cluster.
 # It must be in the form <package-name><comparison-operator><version>
 # It can contain multiple items separated by a colon.
@@ -77,45 +79,57 @@
     LUSTRE: {"tcp": [988]},
     # OpenZFS Security group: https://docs.aws.amazon.com/fsx/latest/OpenZFSGuide/limit-access-security-groups.html
     OPENZFS: {"tcp": [111, 2049, 20001, 20002, 20003], "udp": [111, 2049, 20001, 20002, 20003]},
     # Ontap Security group: https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/limit-access-security-groups.html
     ONTAP: {"tcp": [111, 635, 2049, 4046], "udp": [111, 635, 2049, 4046]},
 }
 
+EFS_PORT = 2049
+
 EBS_VOLUME_TYPE_IOPS_DEFAULT = {
     "io1": 100,
     "io2": 100,
     "gp3": 3000,
 }
 EBS_VOLUME_SIZE_DEFAULT = 35
 EBS_VOLUME_TYPE_DEFAULT = "gp3"
 EBS_VOLUME_TYPE_DEFAULT_US_ISO = "gp2"
 
 DEFAULT_MAX_COUNT = 10
 DEFAULT_MIN_COUNT = 0
-MAX_NUMBER_OF_QUEUES = 10
-MAX_NUMBER_OF_COMPUTE_RESOURCES = 5
+MAX_NUMBER_OF_QUEUES = 100
+SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES = 10
+SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES = 5
+MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER = 150  # Based on API timeout limitations
+MAX_COMPUTE_RESOURCES_PER_DEPLOYMENT_WAVE = 150  # Maximum compute resources that can be deployed at the same time
+MAX_COMPUTE_RESOURCES_PER_QUEUE = 40  # Ensures that each queue will share the same stack as its compute resources
 
 MAX_EBS_COUNT = 5
 MAX_NEW_STORAGE_COUNT = {"efs": 1, "fsx": 1, "raid": 1}
 MAX_EXISTING_STORAGE_COUNT = {"efs": 20, "fsx": 20, "raid": 0}
 
 COOKBOOK_PACKAGES_VERSIONS = {
-    "parallelcluster": "3.5.1",
-    "cookbook": "aws-parallelcluster-cookbook-3.5.1",
+    "parallelcluster": "3.6.0b1",
+    "cookbook": "aws-parallelcluster-cookbook-3.6.0b1",
     "chef": "17.2.29",
     "berkshelf": "7.2.0",
     "ami": "dev",
 }
 
 CW_DASHBOARD_ENABLED_DEFAULT = True
 CW_LOGS_ENABLED_DEFAULT = True
-CW_LOGS_RETENTION_DAYS_DEFAULT = 14
+CW_LOGS_ROTATION_ENABLED_DEFAULT = True
+CW_LOGS_RETENTION_DAYS_DEFAULT = 180
 CW_LOGS_CFN_PARAM_NAME = "ClusterCWLogGroup"
 CW_LOG_GROUP_NAME_PREFIX = "/aws/parallelcluster/"
+CW_ALARM_PERIOD_DEFAULT = 60
+CW_ALARM_PERCENT_THRESHOLD_DEFAULT = 90
+CW_ALARM_EVALUATION_PERIODS_DEFAULT = 1
+CW_ALARM_DATAPOINTS_TO_ALARM_DEFAULT = 1
+DETAILED_MONITORING_ENABLED_DEFAULT = False
 
 STACK_EVENTS_LOG_STREAM_NAME_FORMAT = "{}-cfn-events"
 
 PCLUSTER_IMAGE_NAME_REGEX = r"^[-_A-Za-z0-9{][-_A-Za-z0-9\s:{}\.]+[-_A-Za-z0-9}]$"
 PCLUSTER_IMAGE_ID_REGEX = r"^([a-zA-Z][a-zA-Z0-9-]{0,127})$"
 
 PCLUSTER_SLURM_DYNAMODB_PREFIX = "parallelcluster-slurm-"
@@ -288,7 +302,9 @@
     Operation.DESCRIBE_IMAGE: ["us-iso"],
     Operation.LIST_IMAGES: ["us-iso"],
     Operation.EXPORT_IMAGE_LOGS: ["us-iso"],
     Operation.GET_IMAGE_LOG_EVENTS: ["us-iso"],
     Operation.GET_IMAGE_STACK_EVENTS: ["us-iso"],
     Operation.LIST_IMAGE_LOG_STREAMS: ["us-iso"],
 }
+
+MAX_TAGS_COUNT = 40  # Tags are limited to 50, reserve some tags for parallelcluster specified tags
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/imagebuilder_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/imagebuilder_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/launch_template_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/launch_template_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/lib/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/lib/lib.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/lib/lib.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/models/cluster.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from jinja2 import BaseLoader
 from jinja2.sandbox import SandboxedEnvironment
 from marshmallow import ValidationError
 
 from pcluster.api.models import Metadata
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.common import AWSClientError, BadRequestError, LimitExceededError, StackNotFoundError, get_region
-from pcluster.config.cluster_config import BaseClusterConfig, SchedulerPluginScheduling, SlurmScheduling, Tag
+from pcluster.config.cluster_config import BaseClusterConfig, SchedulerPluginScheduling, Tag
 from pcluster.config.common import ValidatorSuppressor
 from pcluster.config.config_patch import ConfigPatch
 from pcluster.constants import (
     PCLUSTER_CLUSTER_NAME_TAG,
     PCLUSTER_NODE_TYPE_TAG,
     PCLUSTER_QUEUE_NAME_TAG,
     PCLUSTER_S3_ARTIFACTS_DICT,
@@ -365,44 +365,88 @@
             self._add_tags()
             self._generate_artifact_dir()
             artifact_dir_generated = True
             self._upload_config()
             LOGGER.info("Generation and upload completed successfully")
 
             # Create template if not provided by the user
+            assets_metadata = None
             if not (self.config.dev_settings and self.config.dev_settings.cluster_template):
-                self.template_body = CDKTemplateBuilder().build_cluster_template(
+                self.template_body, assets_metadata = CDKTemplateBuilder().build_cluster_template(
                     cluster_config=self.config, bucket=self.bucket, stack_name=self.stack_name
                 )
 
             LOGGER.info("Uploading cluster artifacts...")
             # upload cluster artifacts and generated template
             self._upload_artifacts()
             LOGGER.info("Upload of cluster artifacts completed successfully")
 
             LOGGER.info("Creating stack named: %s", self.stack_name)
+            asset_parameters = self._generate_asset_parameters(assets_metadata)
             creation_result = AWSApi.instance().cfn.create_stack_from_url(
                 stack_name=self.stack_name,
                 template_url=self.bucket.get_cfn_template_url(
                     template_name=PCLUSTER_S3_ARTIFACTS_DICT.get("template_name")
                 ),
                 disable_rollback=disable_rollback,
                 tags=self._get_cfn_tags(),
+                parameters=[
+                    parameter_key_value
+                    for asset_parameter in asset_parameters
+                    for parameter_key_value in asset_parameter
+                    if asset_parameters
+                ],
             )
 
             return creation_result.get("StackId"), suppressed_validation_failures
 
         except ConfigValidationError as e:
             raise e
         except Exception as e:
             if not creation_result and artifact_dir_generated:
                 # Cleanup S3 artifacts if stack is not created yet
                 self.bucket.delete_s3_artifacts()
             raise _cluster_error_mapper(e, str(e))
 
+    @staticmethod
+    def _generate_asset_parameters(assets_metadata):
+        """
+        Create cloud formation template parameters for assets.
+
+        CDK adds 3 parameters to the root stack after running a synthesis.
+        1. ArtifactHash (256-Hash of the asset - useful when running `cdk deploy` only, not relevant otherwise)
+        2. S3Bucket (S3 Bucket where asset is stored)
+        3. S3VersionKey (S3 object key and version of the asset in the form "key||version")
+        """
+        return (
+            [
+                (
+                    {
+                        "ParameterKey": asset_metadata["hash_parameter"]["key"],
+                        "ParameterValue": asset_metadata["hash_parameter"]["value"],
+                    },
+                    {
+                        "ParameterKey": asset_metadata["s3_bucket_parameter"]["key"],
+                        "ParameterValue": asset_metadata["s3_bucket_parameter"]["value"],
+                    },
+                    # CDK builds the TemplateURL parameter of the NestedStack in the Root Template by concatenating
+                    # the AssetParameter S3 Bucket, Object and Version
+                    # The S3 Object and Version are passed as a string "ObjectKey||Version"
+                    # In this case we don't need to specify a version, hence we pass "ObjectKey||"
+                    {
+                        "ParameterKey": asset_metadata["s3_object_key_parameter"]["key"],
+                        "ParameterValue": f"{asset_metadata['s3_object_key_parameter']['value']}||",
+                    },
+                )
+                for asset_metadata in assets_metadata
+            ]
+            if assets_metadata
+            else []
+        )
+
     def _load_config(self, cluster_config: dict) -> BaseClusterConfig:
         """Load the config and catch / translate any errors that occur during loading."""
         try:
             return ClusterSchema(cluster_name=self.name).load(cluster_config)
         except ValidationError as e:
             # syntactic failure
             data = str(sorted(e.messages.items()) if isinstance(e.messages, dict) else e)
@@ -436,14 +480,17 @@
         cluster_config_dict = parse_config(config_text or self.source_config_text)
 
         try:
             LOGGER.info("Validating cluster configuration...")
             Cluster._load_additional_instance_type_data(cluster_config_dict)
             config = self._load_config(cluster_config_dict)
             config.official_ami = self.__official_ami
+            if context.during_update:
+                config.managed_head_node_security_group = self.stack.get_resource_physical_id("HeadNodeSecurityGroup")
+                config.managed_compute_security_group = self.stack.get_resource_physical_id("ComputeSecurityGroup")
 
             validation_failures = config.validate(validator_suppressors, context)
             if any(f.level.value >= FailureLevel(validation_failure_level).value for f in validation_failures):
                 raise ConfigValidationError("Invalid cluster configuration.", validation_failures=validation_failures)
             LOGGER.info("Validation succeeded.")
         except ConfigValidationError as e:
             raise e
@@ -526,21 +573,20 @@
                     custom_artifacts_name=PCLUSTER_S3_ARTIFACTS_DICT.get("scheduler_resources_name"),
                 )
 
             # Upload template
             if self.template_body:
                 self.bucket.upload_cfn_template(self.template_body, PCLUSTER_S3_ARTIFACTS_DICT.get("template_name"))
 
-            if isinstance(self.config.scheduling, (SlurmScheduling, SchedulerPluginScheduling)):
-                # upload instance types data
-                self.bucket.upload_config(
-                    self.config.get_instance_types_data(),
-                    PCLUSTER_S3_ARTIFACTS_DICT.get("instance_types_data_name"),
-                    format=S3FileFormat.JSON,
-                )
+            # upload instance types data
+            self.bucket.upload_config(
+                self.config.get_instance_types_data(),
+                PCLUSTER_S3_ARTIFACTS_DICT.get("instance_types_data_name"),
+                format=S3FileFormat.JSON,
+            )
 
             if isinstance(self.config.scheduling, SchedulerPluginScheduling):
                 self._render_and_upload_scheduler_plugin_template()
             LOGGER.info("Cluster artifacts uploaded correctly.")
         except BadRequestClusterActionError:
             raise
         except Exception as e:
@@ -847,15 +893,15 @@
         """Validate a cluster update request."""
         self._validate_cluster_exists()
         self._validate_stack_status_not_in_progress()
         target_config, ignored_validation_failures = self._validate_and_parse_config(
             validator_suppressors=validator_suppressors,
             validation_failure_level=validation_failure_level,
             config_text=target_source_config,
-            context=ValidatorContext(head_node_instance_id=self.head_node_instance.id),
+            context=ValidatorContext(head_node_instance_id=self.head_node_instance.id, during_update=True),
         )
         changes = self._validate_patch(force, target_config)
 
         self._validate_scheduling_update(changes, target_config)
 
         if dry_run and isinstance(self.config.scheduling, SchedulerPluginScheduling):
             self._render_and_upload_scheduler_plugin_template(dry_run=dry_run)
@@ -906,32 +952,41 @@
             self.__source_config_text = target_source_config
 
             self._add_tags()
             self._upload_config()
             self._upload_change_set(changes)
 
             # Create template if not provided by the user
+            assets_metadata = None
             if not (self.config.dev_settings and self.config.dev_settings.cluster_template):
-                self.template_body = CDKTemplateBuilder().build_cluster_template(
+                self.template_body, assets_metadata = CDKTemplateBuilder().build_cluster_template(
                     cluster_config=self.config,
                     bucket=self.bucket,
                     stack_name=self.stack_name,
                     log_group_name=self.stack.log_group_name,
                 )
 
             # upload cluster artifacts and generated template
             self._upload_artifacts()
 
+            asset_parameters = self._generate_asset_parameters(assets_metadata)
+
             LOGGER.info("Updating stack named: %s", self.stack_name)
             AWSApi.instance().cfn.update_stack_from_url(
                 stack_name=self.stack_name,
                 template_url=self.bucket.get_cfn_template_url(
                     template_name=PCLUSTER_S3_ARTIFACTS_DICT.get("template_name")
                 ),
                 tags=self._get_cfn_tags(),
+                parameters=[
+                    parameter_key_value
+                    for asset_parameter in asset_parameters
+                    for parameter_key_value in asset_parameter
+                    if asset_parameters
+                ],
             )
 
             self.__stack = ClusterStack(AWSApi.instance().cfn.describe_stack(self.stack_name))
             LOGGER.debug("StackId: %s", self.stack.id)
             LOGGER.info("Status: %s", self.stack.status)
 
             return changes, ignored_validation_failures
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/models/cluster_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/models/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/models/compute_fleet_status_manager.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/compute_fleet_status_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/models/imagebuilder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/models/imagebuilder_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/models/s3_bucket.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/s3_bucket.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 
 
 class S3FileFormat(Enum):
     """Define S3 file format."""
 
     YAML = "yaml"
     JSON = "json"
+    MINIFIED_JSON = "min.json"
     TEXT = "text"
 
 
 class S3FileType(Enum):
     """Define S3 file types."""
 
+    ASSETS = "assets"
     CONFIGS = "configs"
     TEMPLATES = "templates"
     CUSTOM_RESOURCES = "custom_resources"
 
 
 class S3Bucket:
     """Represent the s3 bucket configuration."""
@@ -194,22 +196,28 @@
         """Check bucket is configured successfully or not by bootstrapped file."""
         AWSApi.instance().s3.head_object(
             bucket_name=self.name, object_name="/".join([self._root_directory, self._bootstrapped_file_name])
         )
 
     def upload_config(self, config, config_name, format=S3FileFormat.YAML):
         """Upload config file to S3 bucket."""
-        return self._upload_file(file_type=S3FileType.CONFIGS, content=config, file_name=config_name, format=format)
+        return self.upload_file(file_type=S3FileType.CONFIGS, content=config, file_name=config_name, format=format)
 
     def upload_cfn_template(self, template_body, template_name, format=S3FileFormat.YAML):
         """Upload cloudformation template to S3 bucket."""
-        return self._upload_file(
+        return self.upload_file(
             file_type=S3FileType.TEMPLATES, content=template_body, file_name=template_name, format=format
         )
 
+    def upload_cfn_asset(self, asset_file_content, asset_name: str, format=S3FileFormat.YAML):
+        """Upload cloudformation assets to S3 bucket."""
+        return self.upload_file(
+            file_type=S3FileType.ASSETS, content=asset_file_content, file_name=asset_name, format=format
+        )
+
     def upload_resources(self, resource_dir, custom_artifacts_name):
         """
         Upload custom resources to S3 bucket.
 
         :param resource_dir: resource directory containing the resources to upload.
         :param custom_artifacts_name: custom_artifacts_name for zipped dir
         """
@@ -258,35 +266,21 @@
 
     def get_resource_url(self, resource_name):
         """Get custom resource http url from S3 bucket."""
         return self._get_file_url(file_type=S3FileType.CUSTOM_RESOURCES, file_name=resource_name)
 
     # --------------------------------------- S3 private functions --------------------------------------- #
 
-    def _upload_file(self, content, file_name, file_type, format=S3FileFormat.YAML):
+    def upload_file(self, content, file_name, file_type, format=S3FileFormat.YAML):
         """Upload file to S3 bucket."""
-        if format == S3FileFormat.YAML:
-            result = AWSApi.instance().s3.put_object(
-                bucket_name=self.name,
-                body=yaml.dump(content),
-                key=self.get_object_key(file_type, file_name),
-            )
-        elif format == S3FileFormat.JSON:
-            result = AWSApi.instance().s3.put_object(
-                bucket_name=self.name,
-                body=json.dumps(content),
-                key=self.get_object_key(file_type, file_name),
-            )
-        else:
-            result = AWSApi.instance().s3.put_object(
-                bucket_name=self.name,
-                body=content,
-                key=self.get_object_key(file_type, file_name),
-            )
-        return result
+        return AWSApi.instance().s3.put_object(
+            bucket_name=self.name,
+            body=format_content(content, format),
+            key=self.get_object_key(file_type, file_name),
+        )
 
     def _get_file(self, file_name, file_type, version_id=None, format=S3FileFormat.YAML):
         """Get file from S3 bucket."""
         result = AWSApi.instance().s3.get_object(
             bucket_name=self.name, key=self.get_object_key(file_type, file_name), version_id=version_id
         )
 
@@ -414,7 +408,26 @@
     :param expiration: Time in seconds for the presigned URL to remain valid
     :return: Presigned URL as string
     """
     s3_uri_info = parse_bucket_url(s3_uri)
     return AWSApi.instance().s3.create_presigned_url(
         s3_uri_info["bucket_name"], s3_uri_info["object_key"], expiration=expiration
     )
+
+
+def format_content(content, s3_file_format: S3FileFormat):
+    """
+    Return content formatted by the given S3 File Format.
+
+    If format is not in the S3FileFormat Enum, it returns the content without any formatting
+    :param content: Object representing the content to be formatted
+    :param s3_file_format: S3FileFormat to use for the output
+    :return:
+    """
+    if s3_file_format == S3FileFormat.YAML:
+        return yaml.dump(content)
+    elif s3_file_format == S3FileFormat.JSON:
+        return json.dumps(content)
+    elif s3_file_format == S3FileFormat.MINIFIED_JSON:
+        return json.dumps(content, separators=(",", ":"))
+    else:
+        return content
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/networking/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/networking/vpc_factory.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/networking/vpc_factory.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/alinux2/Dockerfile` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/alinux2/Dockerfile`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/build-docker-images.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/build-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/buildspec.yml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/buildspec.yml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/batch/docker/upload-docker-images.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/upload-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/compute_node/user_data.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/compute_node/user_data.sh`

 * *Files 6% similar despite different names*

```diff
@@ -67,24 +67,21 @@
 write_files:
   - path: /tmp/dna.json
     permissions: '0644'
     owner: root:root
     content: |
       {
         "cluster": {
+          "cluster_name": "${ClusterName}",
           "stack_name": "${AWS::StackName}",
           "stack_arn": "${AWS::StackId}",
           "enable_efa": "${EnableEfa}",
           "raid_shared_dir": "${RAIDSharedDir}",
           "raid_type": "${RAIDType}",
           "base_os": "${BaseOS}",
-          "preinstall": "${PreInstallScript}",
-          "preinstall_args": "${PreInstallArgs}",
-          "postinstall": "${PostInstallScript}",
-          "postinstall_args": "${PostInstallArgs}",
           "region": "${AWS::Region}",
           "efs_fs_ids": "${EFSIds}",
           "efs_shared_dirs": "${EFSSharedDirs}",
           "efs_encryption_in_transits": "${EFSEncryptionInTransits}",
           "efs_iam_authorizations": "${EFSIamAuthorizations}",
           "fsx_fs_ids": "${FSXIds}",
           "fsx_mount_names": "${FSXMountNames}",
@@ -100,14 +97,15 @@
           "log_group_name": "${LogGroupName}",
           "dns_domain": "${ClusterDNSDomain}",
           "hosted_zone": "${ClusterHostedZone}",
           "node_type": "ComputeFleet",
           "cluster_user": "${OSUser}",
           "enable_intel_hpc_platform": "${IntelHPCPlatform}",
           "cw_logging_enabled": "${CWLoggingEnabled}",
+          "log_rotation_enabled": "${LogRotationEnabled}",
           "scheduler_queue_name": "${QueueName}",
           "scheduler_compute_resource_name": "${ComputeResourceName}",
           "enable_efa_gdr": "${EnableEfaGdr}",
           "custom_node_package": "${CustomNodePackage}",
           "custom_awsbatchcli_package": "${CustomAwsBatchCliPackage}",
           "use_private_hostname": "${UsePrivateHostname}",
           "head_node_private_ip": "${HeadNodePrivateIp}",
@@ -183,15 +181,17 @@
       export parallelcluster_version=aws-parallelcluster-${ParallelClusterVersion}
       export cookbook_version=${CookbookVersion}
       export chef_version=${ChefVersion}
       export berkshelf_version=${BerkshelfVersion}
       if [ -f /opt/parallelcluster/.bootstrapped ]; then
         installed_version=$(cat /opt/parallelcluster/.bootstrapped)
         if [ "${!cookbook_version}" != "${!installed_version}" ]; then
-          error_exit "This AMI was created with ${!installed_version}, but is trying to be used with ${!cookbook_version}. Please either use an AMI created with ${!cookbook_version} or change your ParallelCluster to ${!installed_version}"
+          cookbook_version_number=$(echo ${!cookbook_version} | awk -F- '{print $NF}')
+          installed_version_number=$(echo ${!installed_version} | awk -F- '{print $NF}')
+          error_exit "This AMI was created with ParallelCluster ${!installed_version_number}, but is trying to be used with ParallelCluster ${!cookbook_version_number}. Please either use an AMI created with ParallelCluster ${!cookbook_version_number} or change your ParallelCluster to ${!installed_version_number}"
         fi
       else
         error_exit "This AMI was not baked by ParallelCluster. Please use pcluster build-image command to create an AMI by providing your AMI as parent image."
       fi
       if [ "${!custom_cookbook}" != "NONE" ]; then
         curl --retry 3 -v -L -o /etc/chef/aws-parallelcluster-cookbook.tgz ${!cookbook_url}
         vendor_cookbook
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/head_node/user_data.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/head_node/user_data.sh`

 * *Files 4% similar despite different names*

```diff
@@ -124,15 +124,17 @@
 export parallelcluster_version=aws-parallelcluster-${ParallelClusterVersion}
 export cookbook_version=${CookbookVersion}
 export chef_version=${ChefVersion}
 export berkshelf_version=${BerkshelfVersion}
 if [ -f /opt/parallelcluster/.bootstrapped ]; then
   installed_version=$(cat /opt/parallelcluster/.bootstrapped)
   if [ "${!cookbook_version}" != "${!installed_version}" ]; then
-    error_exit "This AMI was created with ${!installed_version}, but is trying to be used with ${!cookbook_version}. Please either use an AMI created with ${!cookbook_version} or change your ParallelCluster to ${!installed_version}"
+    cookbook_version_number=$(echo ${!cookbook_version} | awk -F- '{print $NF}')
+    installed_version_number=$(echo ${!installed_version} | awk -F- '{print $NF}')
+    error_exit "This AMI was created with ${!installed_version_number}, but is trying to be used with ${!cookbook_version_number}. Please either use an AMI created with ${!cookbook_version_number} or change your ParallelCluster to ${!installed_version_number}"
   fi
 else
   error_exit "This AMI was not baked by ParallelCluster. Please use pcluster build-image command to create an AMI by providing your AMI as parent image."
 fi
 if [ "${!custom_cookbook}" != "NONE" ]; then
   curl --retry 3 -v -L -o /etc/chef/aws-parallelcluster-cookbook.tgz ${!cookbook_url}
   vendor_cookbook
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/custom_script.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/custom_script.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
           commands:
             - |
               set -v
               CINC_URL="https://${AWS::Region}-aws-parallelcluster.s3.${AWS::Region}.${AWS::URLSuffix}/archives/cinc/cinc-install-1.1.0.sh"
               [ -n "${CfnParamCincInstaller}" ] && CINC_URL="${CfnParamCincInstaller}"
               echo "${!CINC_URL}"
 
-      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.18.04 | ubuntu.20.04
+      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.18.04 | ubuntu.20.04 | rhel.8.7
       - name: OperatingSystemRelease
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               FILE=/etc/os-release
@@ -86,14 +86,16 @@
                 OS='alinux2'
               elif [ `echo "${!RELEASE}" | grep '^centos\.7'` ]; then
                 OS='centos7'
               elif [ `echo "${!RELEASE}" | grep '^ubuntu\.18'` ]; then
                 OS='ubuntu1804'
               elif [ `echo "${!RELEASE}" | grep '^ubuntu\.20'` ]; then
                 OS='ubuntu2004'
+              elif [ `echo "${!RELEASE}" | grep '^rhel\.8'` ]; then
+                OS='rhel8'
               else
                 echo "Operating System '${!RELEASE}' is not supported. Failing build."
                 exit {{ FailExitCode }}
               fi
 
               echo ${!OS}
 
@@ -102,15 +104,15 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
                set -v
                OS='{{ build.OperatingSystemName.outputs.stdout }}'
 
-               if [ `echo "${!OS}" | grep -E '^(alinux|centos)'` ]; then
+               if [ `echo "${!OS}" | grep -E '^(alinux|centos|rhel)'` ]; then
                  PLATFORM='RHEL'
                elif [ `echo "${!OS}" | grep -E '^ubuntu'` ]; then
                  PLATFORM='DEBIAN'
                fi
 
                echo ${!PLATFORM}
 
@@ -140,23 +142,23 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               if [ ${CfnParamUpdateOsAndReboot} == false ]; then
                 RELEASE='{{ build.OperatingSystemRelease.outputs.stdout }}'
-                if [ `echo "${!RELEASE}" | grep -Ev '^(amzn|centos|ubuntu)'` ]; then
+                if [ `echo "${!RELEASE}" | grep -Ev '^(amzn|centos|ubuntu|rhel)'` ]; then
                   echo "This component does not support '${!RELEASE}'. Failing build."
                   exit {{ FailExitCode }}
                 fi
 
-                # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu1804, Ubuntu2004 and Centos7
+                # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu1804, Ubuntu2004, Centos7 and RHEL8
                 ARCH=$(uname -m)
                 if [[ `echo ${!ARCH}` == 'aarch64' ]]; then
-                  if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.18\.04|ubuntu\.20\.04)'` ]; then
+                  if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.18\.04|ubuntu\.20\.04|rhel\.8)'` ]; then
                     echo "This component does not support '${!RELEASE}' on ARM64 CPUs. Failing build."
                     exit {{ FailExitCode }}
                   fi
                 fi
               fi
 
       # Install prerequisite OS packages
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
                 OS='alinux2'
               elif [ $(echo "${RELEASE}" | grep '^centos\.7') ]; then
                 OS='centos7'
               elif [ $(echo "${RELEASE}" | grep '^ubuntu\.18') ]; then
                 OS='ubuntu1804'
               elif [ $(echo "${RELEASE}" | grep '^ubuntu\.20') ]; then
                 OS='ubuntu2004'
+              elif [ $(echo "${RELEASE}" | grep '^rhel\.8') ]; then
+                OS='rhel8'
               fi
 
               echo ${OS}
 
       - name: ParallelClusterTag
         action: ExecuteBash
         inputs:
@@ -64,15 +66,15 @@
             - |
               set -v
 
               # Install AWS CLI
               which aws
               if [[ $? -ne 0 ]]; then
                 echo "Installing unzip"
-                if [[ "{{ test.OperatingSystemName.outputs.stdout }}" =~ ^(centos7|alinux) ]]; then
+                if [[ "{{ test.OperatingSystemName.outputs.stdout }}" =~ ^(centos7|alinux|rhel) ]]; then
                   yum -y install unzip
                 elif [[ "{{ test.OperatingSystemName.outputs.stdout }}" =~ ^ubuntu ]]; then
                   apt-get -y install unzip
                 fi
                 echo "Installing AWS CLI"
                 curl --retry 3 -L -o /tmp/awscliv2.zip "https://awscli.amazonaws.com/awscli-exe-linux-$(uname -m).zip"
                 cd /tmp/ && unzip awscliv2.zip
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,16 @@
                 OS='alinux2'
               elif [ `echo "${RELEASE}" | grep '^centos\.7'` ]; then
                 OS='centos7'
               elif [ `echo "${RELEASE}" | grep '^ubuntu\.18'` ]; then
                 OS='ubuntu1804'
               elif [ `echo "${RELEASE}" | grep '^ubuntu\.20'` ]; then
                 OS='ubuntu2004'
+              elif [ `echo "${RELEASE}" | grep '^rhel\.8'` ]; then
+                OS='rhel8'
               else
                 echo "Operating System '${RELEASE}' is not supported. Failing build." && exit 1
               fi
 
               echo ${OS}
 
       ### versions ###
@@ -140,14 +142,16 @@
         inputs:
           commands:
             - |
               set -vx
               OS="{{ test.OperatingSystemName.outputs.stdout }}"
               if [[ ${OS} =~ ^alinux ]]; then
                 username="ec2-user"
+              elif [[ ${OS} =~ ^rhel ]]; then
+                username="ec2-user"
               elif [[ ${OS} =~ ^centos ]]; then
                 username="centos"
               elif [[ ${OS} =~ ^ubuntu ]]; then
                 username="ubuntu"
               fi
               export PATH="/usr/local/bin:/usr/bin/:${PATH}"
 
@@ -173,19 +177,21 @@
               echo "Checking virtualenv python version..."
               {{ test.CookbookVirtualenvPath.outputs.stdout }}/bin/python -V | grep {{ test.PythonVersion.outputs.stdout }}
               [[ $? -ne 0 ]] && echo "Check cookbook virtualenv python version failed" && exit 1
 
               {{ test.NodeVirtualenvPath.outputs.stdout }}/bin/python -V | grep {{ test.PythonVersion.outputs.stdout }}
               [[ $? -ne 0 ]] && echo "Check node virtualenv python version failed" && exit 1
 
-              {{ test.SchedulerPluginVirtualenvPath.outputs.stdout }}/bin/python -V | grep {{ test.SchedulerPluginPythonVersion.outputs.stdout }}
-              [[ $? -ne 0 ]] && echo "Check scheduler plugin virtualenv python version failed" && exit 1
-              su -l pcluster-scheduler-plugin -c "which python" | grep envs/scheduler_plugin_virtualenv/bin/python
-              [[ $? -ne 0 ]] && echo "Check scheduler plugin virtualenv python path failed" && exit 1
-
+              if [[ {{ test.OperatingSystemName.outputs.stdout }} != 'rhel8' ]]; then
+                {{ test.SchedulerPluginVirtualenvPath.outputs.stdout }}/bin/python -V | grep {{ test.SchedulerPluginPythonVersion.outputs.stdout }}
+                [[ $? -ne 0 ]] && echo "Check scheduler plugin virtualenv python version failed" && exit 1
+                su -l pcluster-scheduler-plugin -c "which python" | grep envs/scheduler_plugin_virtualenv/bin/python
+                [[ $? -ne 0 ]] && echo "Check scheduler plugin virtualenv python path failed" && exit 1
+              fi
+              
               echo "Virtualenv test passed"
 
       - name: Pip
         action: ExecuteBash
         inputs:
           commands:
             - |
@@ -264,19 +270,21 @@
 
       - name: SchedulerPluginEventHandlerScript
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -vx
-              Script=/usr/local/sbin/invoke-scheduler-plugin-event-handler.sh
-              if [ -x ${Script} ]; then
-                echo "Scheduler plugin handler script '${Script}' is executable."
-              else
-                echo "Scheduler plugin handler script '${Script}' is not executable." && exit 1
+              if [[ {{ test.OperatingSystemName.outputs.stdout }} != 'rhel8' ]]; then
+                Script=/usr/local/sbin/invoke-scheduler-plugin-event-handler.sh
+                if [ -x ${Script} ]; then
+                  echo "Scheduler plugin handler script '${Script}' is executable."
+                else
+                  echo "Scheduler plugin handler script '${Script}' is not executable." && exit 1
+                fi
               fi
 
       - name: Log4jPatcher
         action: ExecuteBash
         inputs:
           commands:
             - |
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,16 @@
                 OS='alinux2'
               elif [ `echo "${RELEASE}" | grep '^centos\.7'` ]; then
                 OS='centos7'
               elif [ `echo "${RELEASE}" | grep '^ubuntu\.18'` ]; then
                 OS='ubuntu1804'
               elif [ `echo "${RELEASE}" | grep '^ubuntu\.20'` ]; then
                 OS='ubuntu2004'
+              elif [ `echo "${RELEASE}" | grep '^rhel\.8'` ]; then
+                OS='rhel8'
               else
                 echo "Operating System '${RELEASE}' is not supported. Failing build." && exit 1
               fi
 
               echo ${OS}
 
       # Get input base AMI Architecture
@@ -73,15 +75,15 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               OS='{{ validate.OperatingSystemName.outputs.stdout }}'
 
-              if [ `echo "${OS}" | grep -E '^(alinux|centos)'` ]; then
+              if [ `echo "${OS}" | grep -E '^(alinux|centos|rhel)'` ]; then
                 PLATFORM='RHEL'
               elif [ `echo "${OS}" | grep -E '^ubuntu'` ]; then
                 PLATFORM='DEBIAN'
               fi
 
               echo ${PLATFORM}
 
@@ -100,41 +102,41 @@
       ### conditions ###
       - name: IntelMPISupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} != 'arm64' ]] && echo "true" || echo "false"
+              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} != 'arm64' && {{ validate.OperatingSystemName.outputs.stdout }} != 'rhel8' ]] && echo "true" || echo "false"
 
       - name: ArmPLSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' ]] && echo "true" || echo "false"
+              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' && {{ validate.OperatingSystemName.outputs.stdout }} != 'rhel8' ]] && echo "true" || echo "false"
 
       - name: FabricManagerSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' ]] && echo "false" || echo "true"
+              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' || {{ validate.OperatingSystemName.outputs.stdout }} == 'rhel8' ]] && echo "false" || echo "true"
 
       - name: LustreSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               ARCHITECTURE='{{ validate.OperatingSystemArchitecture.outputs.stdout }}'
               OS='{{ validate.OperatingSystemName.outputs.stdout }}'
-              if [ ${ARCHITECTURE} == 'arm64' ] && [[ ${OS} =~ ^(ubuntu(18|20)04|alinux2)$ ]] || [ ${ARCHITECTURE} == 'x86_64' ]; then
+              if [ ${ARCHITECTURE} == 'arm64' ] && [[ ${OS} =~ ^(ubuntu(18|20)04|alinux2|rhel8)$ ]] || [ ${ARCHITECTURE} == 'x86_64' ]; then
                 echo "true"
               else
                 echo "false"
               fi
 
       ### versions ###
       - name: MungeVersion
@@ -281,15 +283,15 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -vx
               PLATFORM='{{ validate.PlatformName.outputs.stdout }}'
 
-              if [ {{ validate.NvidiaEnabled.outputs.stdout }} == "no" ]; then
+              if [[ {{ validate.NvidiaEnabled.outputs.stdout }} == 'no' || {{ validate.OperatingSystemName.outputs.stdout }} == 'rhel8' ]]; then
                 echo "Nvidia recipe not enabled, skipping." && exit 0
               fi
               if [ {{ validate.HasGPU.outputs.stdout }} == "false" ]; then
                 echo "No GPU detected, skipping." && exit 0
               fi
 
               driver_ver="{{ validate.NvidiaDriverVersion.outputs.stdout }}"
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   - FailExitCode:
       type: string
       value: 1
 
 phases:
   - name: build
     steps:
-      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.18.04
+      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.18.04 | ubuntu.20.04 | rhel.8.7
       - name: OperatingSystemRelease
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               FILE=/etc/os-release
@@ -39,14 +39,16 @@
                 OS='alinux2'
               elif [ `echo "${!RELEASE}" | grep '^centos\.7'` ]; then
                 OS='centos7'
               elif [ `echo "${!RELEASE}" | grep '^ubuntu\.18'` ]; then
                 OS='ubuntu1804'
               elif [ `echo "${!RELEASE}" | grep '^ubuntu\.20'` ]; then
                 OS='ubuntu2004'
+              elif [ `echo "${!RELEASE}" | grep '^rhel\.8'` ]; then
+                OS='rhel8'
               else
                 echo "Operating System '${!RELEASE}' is not supported. Failing build."
                 exit {{ FailExitCode }}
               fi
 
               echo ${!OS}
 
@@ -55,15 +57,15 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
                set -v
                OS='{{ build.OperatingSystemName.outputs.stdout }}'
 
-               if [ `echo "${!OS}" | grep -E '^(alinux|centos)'` ]; then
+               if [ `echo "${!OS}" | grep -E '^(alinux|centos|rhel)'` ]; then
                  PLATFORM='RHEL'
                elif [ `echo "${!OS}" | grep -E '^ubuntu'` ]; then
                  PLATFORM='DEBIAN'
                fi
 
                echo ${!PLATFORM}
 
@@ -71,23 +73,23 @@
       - name: IsOperatingSystemSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               RELEASE='{{ build.OperatingSystemRelease.outputs.stdout }}'
-              if [ `echo "${!RELEASE}" | grep -Ev '^(amzn|centos|ubuntu)'` ]; then
+              if [ `echo "${!RELEASE}" | grep -Ev '^(amzn|centos|ubuntu|rhel)'` ]; then
                 echo "This component does not support '${!RELEASE}'. Failing build."
                 exit {{ FailExitCode }}
               fi
 
-              # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu1804, Ubuntu2004 and Centos7
+              # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu1804, Ubuntu2004, Centos7 and RHEL 8
               ARCH=$(uname -m)
               if [[ `echo ${!ARCH}` == 'aarch64' ]]; then
-                if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.18\.04|ubuntu\.20\.04)'` ]; then
+                if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.18\.04|ubuntu\.20\.04|rhel\.8)'` ]; then
                   echo "This component does not support '${!RELEASE}' on ARM64 CPUs. Failing build."
                   exit {{ FailExitCode }}
                 fi
               fi
 
       - name: DisableNouveau
         action: ExecuteBash
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/schemas/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/schemas/cluster_schema.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/cluster_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,22 +51,25 @@
     DirectoryService,
     Dns,
     Efa,
     EphemeralVolume,
     ExistingFsxOntap,
     ExistingFsxOpenZfs,
     FlexibleInstanceType,
+    GpuHealthCheck,
     HeadNode,
     HeadNodeImage,
     HeadNodeNetworking,
+    HealthChecks,
     Iam,
     Image,
     Imds,
     IntelSoftware,
     LocalStorage,
+    LogRotation,
     Logs,
     Monitoring,
     PlacementGroup,
     Proxy,
     QueueImage,
     QueueUpdateStrategy,
     Raid,
@@ -106,14 +109,15 @@
     SlurmQueueNetworking,
     SlurmScheduling,
     SlurmSettings,
     Ssh,
     SudoerConfiguration,
     Timeouts,
 )
+from pcluster.config.common import BaseTag
 from pcluster.config.update_policy import UpdatePolicy
 from pcluster.constants import (
     DELETION_POLICIES,
     DELETION_POLICIES_WITH_SNAPSHOT,
     FSX_LUSTRE,
     FSX_ONTAP,
     FSX_OPENZFS,
@@ -128,15 +132,20 @@
 from pcluster.schemas.common_schema import (
     AdditionalIamPolicySchema,
     BaseDevSettingsSchema,
     BaseSchema,
     DeploymentSettingsSchema,
 )
 from pcluster.schemas.common_schema import ImdsSchema as TopLevelImdsSchema
-from pcluster.schemas.common_schema import TagSchema, get_field_validator, validate_no_reserved_tag
+from pcluster.schemas.common_schema import (
+    TagSchema,
+    get_field_validator,
+    validate_no_duplicate_tag,
+    validate_no_reserved_tag,
+)
 from pcluster.utils import yaml_load
 from pcluster.validators.cluster_validators import EFS_MESSAGES, FSX_MESSAGES
 
 # pylint: disable=C0302
 
 
 LOGGER = logging.getLogger(__name__)
@@ -754,14 +763,25 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return CloudWatchLogs(**data)
 
 
+class RotationSchema(BaseSchema):
+    """Represent the schema of the Log Rotation section."""
+
+    enabled = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return LogRotation(**data)
+
+
 class CloudWatchDashboardsSchema(BaseSchema):
     """Represent the schema of the CloudWatchDashboards section."""
 
     enabled = fields.Bool(metadata={"update_policy": UpdatePolicy.SUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
@@ -769,14 +789,15 @@
         return CloudWatchDashboards(**data)
 
 
 class LogsSchema(BaseSchema):
     """Represent the schema of the Logs section."""
 
     cloud_watch = fields.Nested(CloudWatchLogsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
+    rotation = fields.Nested(RotationSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return Logs(**data)
 
 
@@ -790,15 +811,15 @@
         """Generate resource."""
         return Dashboards(**data)
 
 
 class MonitoringSchema(BaseSchema):
     """Represent the schema of the Monitoring section."""
 
-    detailed_monitoring = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
+    detailed_monitoring = fields.Bool(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
     logs = fields.Nested(LogsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     dashboards = fields.Nested(DashboardsSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return Monitoring(**data)
@@ -1002,14 +1023,39 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return ClusterDevSettings(**data)
 
 
+# ---------------------- Health Checks ---------------------- #
+
+
+class GpuHealthCheckSchema(BaseSchema):
+    """Represent the schema of gpu health check."""
+
+    enabled = fields.Bool(metadata={"update_policy": UpdatePolicy.SUPPORTED})
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return GpuHealthCheck(**data)
+
+
+class HealthChecksSchema(BaseSchema):
+    """Represent the HealthChecks schema."""
+
+    gpu = fields.Nested(GpuHealthCheckSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return HealthChecks(**data)
+
+
 # ---------------------- Node and Cluster Schema ---------------------- #
 
 
 class ImageSchema(BaseSchema):
     """Represent the schema of the Image."""
 
     os = fields.Str(
@@ -1050,74 +1096,96 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return QueueImage(**data)
 
 
-class HeadNodeCustomActionSchema(BaseSchema):
-    """Represent the schema of the custom action."""
+class OneOrManyCustomActionField(fields.Nested):
+    """Custom Marshmallow filed to handle backward compatible single script custom actions."""
 
-    script = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    args = fields.List(fields.Str(), metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
+    def __init__(self, **kwargs):
+        schema = self._build_dynamic_schema_class(
+            kwargs.get("metadata", {}).get("update_policy", UpdatePolicy.UNSUPPORTED)
+        )
+        super().__init__(schema, **kwargs)
 
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return CustomAction(**data)
+    @staticmethod
+    def _build_dynamic_schema_class(update_policy):
+        class_name = f"CustomActionScriptSchema{update_policy.name}"
+        if class_name not in globals():
+            schema_class_type = type(
+                class_name,
+                (CustomActionScriptSchemaBase,),
+                {
+                    "script": fields.Str(required=True, metadata={"update_policy": update_policy}),
+                    "args": fields.List(fields.Str(), metadata={"update_policy": update_policy}),
+                },
+            )
+            globals()[class_name] = schema_class_type
+        else:
+            schema_class_type = globals()[class_name]
+        return schema_class_type
 
+    def _deserialize(self, value, attr, data, **kwargs):
+        if "Script" in value and "Sequence" in value:
+            raise ValidationError("Both Script and Sequence fields are provided. Only one is allowed.")
+
+        if "Script" in value:
+            return super()._deserialize(value, attr, data, **kwargs)
+
+        if "Sequence" in value:
+            sequence = value["Sequence"]
+            if not isinstance(sequence, list):
+                raise ValidationError("Invalid input type for Sequence, expected list.")
+            res = []
+            for item in sequence:
+                res.append(super()._deserialize(item, attr, data, **kwargs))
+            return res
+
+        raise ValidationError("Either Script or Sequence field must be provided.")
+
+    def _serialize(self, nested_obj, attr, obj, **kwargs):
+        if isinstance(nested_obj, list):
+            nested_serialized = []
+            for item in nested_obj:
+                nested_serialized.append(super()._serialize(item, attr, obj, **kwargs))
+            res = {"Sequence": nested_serialized}
+        else:
+            res = super()._serialize(nested_obj, attr, obj, **kwargs)
+        return res
 
-class HeadNodeUpdatableCustomActionSchema(BaseSchema):
-    """Represent the schema of an updatable custom action."""
 
-    script = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.SUPPORTED})
-    args = fields.List(fields.Str(), metadata={"update_policy": UpdatePolicy.SUPPORTED})
+class CustomActionScriptSchemaBase(BaseSchema):
+    """Represent the schema of the custom action script that cannot be updated."""
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return CustomAction(**data)
 
 
-class HeadNodeCustomActionsSchema(BaseSchema):
-    """Represent the schema for all available custom actions."""
+class QueueCustomActionsSchema(BaseSchema):
+    """Represent the schema for all available custom actions in the queues."""
 
-    on_node_start = fields.Nested(HeadNodeCustomActionSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    on_node_configured = fields.Nested(HeadNodeCustomActionSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    on_node_updated = fields.Nested(
-        HeadNodeUpdatableCustomActionSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED}
-    )
+    on_node_start = OneOrManyCustomActionField(metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY})
+    on_node_configured = OneOrManyCustomActionField(metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return CustomActions(**data)
 
 
-class QueueCustomActionSchema(BaseSchema):
-    """Represent the schema of the custom action."""
-
-    script = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY})
-    args = fields.List(fields.Str(), metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return CustomAction(**data)
-
+class HeadNodeCustomActionsSchema(BaseSchema):
+    """Represent the schema for all available custom actions in the head node."""
 
-class QueueCustomActionsSchema(BaseSchema):
-    """Represent the schema for all available custom actions."""
-
-    on_node_start = fields.Nested(
-        QueueCustomActionSchema, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY}
-    )
-    on_node_configured = fields.Nested(
-        QueueCustomActionSchema, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY}
-    )
+    on_node_start = OneOrManyCustomActionField(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
+    on_node_configured = OneOrManyCustomActionField(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
+    on_node_updated = OneOrManyCustomActionField(metadata={"update_policy": UpdatePolicy.SUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return CustomActions(**data)
 
 
@@ -1169,14 +1237,34 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return SlurmComputeResourceNetworking(**data)
 
 
+class QueueTagSchema(BaseSchema):
+    """Represent the schema of Tag section."""
+
+    key = fields.Str(
+        required=True,
+        validate=validate.Length(max=128),
+        metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY},
+    )
+    value = fields.Str(
+        required=True,
+        validate=validate.Length(max=256),
+        metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY},
+    )
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return BaseTag(**data)
+
+
 class SlurmComputeResourceSchema(_ComputeResourceSchema):
     """Represent the schema of the Slurm ComputeResource."""
 
     instance_type = fields.Str(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
     instances = fields.Nested(
         InstanceTypeSchema,
         many=True,
@@ -1192,14 +1280,19 @@
     schedulable_memory = fields.Int(metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY})
     capacity_reservation_target = fields.Nested(
         CapacityReservationTargetSchema, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY}
     )
     networking = fields.Nested(
         SlurmComputeResourceNetworkingSchema, metadata={"update_policy": UpdatePolicy.MANAGED_PLACEMENT_GROUP}
     )
+    health_checks = fields.Nested(HealthChecksSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    custom_slurm_settings = fields.Dict(metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    tags = fields.Nested(
+        QueueTagSchema, many=True, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY, "update_key": "Key"}
+    )
 
     @validates_schema
     def no_coexist_instance_type_flexibility(self, data, **kwargs):
         """Validate that 'instance_type' and 'instances' do not co-exist."""
         if self.fields_coexist(
             data,
             ["instance_type", "instances"],
@@ -1217,14 +1310,20 @@
             if instance_type_name in instance_types:
                 raise ValidationError(
                     f"Duplicate instance type ({instance_type_name}) detected. Instances should not have "
                     f"duplicate instance types. "
                 )
             instance_types.add(instance_type_name)
 
+    @validates("tags")
+    def validate_tags(self, tags):
+        """Validate tags."""
+        validate_no_reserved_tag(tags)
+        validate_no_duplicate_tag(tags)
+
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         if data.get("instances"):
             return SlurmFlexibleComputeResource(**data)
         return SlurmComputeResource(**data)
 
@@ -1315,20 +1414,31 @@
         SlurmComputeResourceSchema,
         many=True,
         metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP_ON_REMOVE, "update_key": "Name"},
     )
     networking = fields.Nested(
         SlurmQueueNetworkingSchema, required=True, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY}
     )
+    health_checks = fields.Nested(HealthChecksSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    custom_slurm_settings = fields.Dict(metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    tags = fields.Nested(
+        QueueTagSchema, many=True, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY, "update_key": "Key"}
+    )
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return SlurmQueue(**data)
 
+    @validates("tags")
+    def validate_tags(self, tags):
+        """Validate tags."""
+        validate_no_reserved_tag(tags)
+        validate_no_duplicate_tag(tags)
+
 
 class AwsBatchQueueSchema(BaseQueueSchema):
     """Represent the schema of a Batch Queue."""
 
     compute_resources = fields.Nested(
         AwsBatchComputeResourceSchema,
         many=True,
@@ -1401,14 +1511,16 @@
     dns = fields.Nested(DnsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     queue_update_strategy = fields.Str(
         validate=validate.OneOf([strategy.value for strategy in QueueUpdateStrategy]),
         metadata={"update_policy": UpdatePolicy.IGNORED},
     )
     enable_memory_based_scheduling = fields.Bool(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
     database = fields.Nested(DatabaseSchema, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
+    custom_slurm_settings = fields.List(fields.Dict, metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    custom_slurm_settings_include_file = fields.Str(metadata={"update_policy": UpdatePolicy.SUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return SlurmSettings(**data)
 
 
@@ -1975,15 +2087,15 @@
         many=True,
         metadata={
             "update_policy": UpdatePolicy(UpdatePolicy.SHARED_STORAGE_UPDATE_POLICY),
             "update_key": "Name",
         },
     )
 
-    monitoring = fields.Nested(MonitoringSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    monitoring = fields.Nested(MonitoringSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     additional_packages = fields.Nested(AdditionalPackagesSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     tags = fields.Nested(
         TagSchema, many=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED, "update_key": "Key"}
     )
     iam = fields.Nested(ClusterIamSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     directory_service = fields.Nested(
         DirectoryServiceSchema, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP}
@@ -1999,14 +2111,15 @@
         super().__init__()
         self.cluster_name = cluster_name
 
     @validates("tags")
     def validate_tags(self, tags):
         """Validate tags."""
         validate_no_reserved_tag(tags)
+        validate_no_duplicate_tag(tags)
 
     @validates_schema
     def no_settings_for_batch(self, data, **kwargs):
         """Ensure IntelSoftware and DirectoryService section is not included when AWS Batch is the scheduler."""
         scheduling = data.get("scheduling")
         head_node = data.get("head_node")
         if scheduling and scheduling.scheduler == "awsbatch":
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/schemas/common_schema.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/common_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,21 +45,42 @@
         json.loads(data)
     except ValueError:
         return False
     return True
 
 
 def validate_no_reserved_tag(tags):
-    """Validate there is no tag with reserved prefix."""
+    """
+    Validate there is no tag with reserved prefix.
+
+    If one tag in the config has a boolean value, tags will be a list of dict.
+    If all of them are strings, we'll have a list of BaseTag objects.
+    """
     if tags:
         for tag in tags:
-            if tag.key.startswith(PCLUSTER_PREFIX):
+            if isinstance(tag, BaseTag):
+                tag_key = tag.key
+            else:
+                tag_key = tag.get("key", "")
+            if tag_key.startswith(PCLUSTER_PREFIX):
                 raise ValidationError(message=f"The tag key prefix '{PCLUSTER_PREFIX}' is reserved and cannot be used.")
 
 
+def validate_no_duplicate_tag(tags):
+    """Validate there is no duplicate tag keys in the same tag section."""
+    all_tags = set()
+    for tag in tags:
+        tag_key = tag.key
+        if tag_key in all_tags:
+            raise ValidationError(
+                f"Duplicate tag key ({tag_key}) detected. Tags keys should be unique within the Tags section."
+            )
+        all_tags.add(tag_key)
+
+
 def get_field_validator(field_name):
     allowed_values = ALLOWED_VALUES[field_name]
     return validate.OneOf(allowed_values) if isinstance(allowed_values, list) else validate.Regexp(allowed_values)
 
 
 class BaseSchema(Schema):
     """Represent a base schema, containing all the features required by all the Schema classes."""
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/schemas/imagebuilder_schema.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/imagebuilder_schema.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/awsbatch_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/awsbatch_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,17 +563,17 @@
                         value=self.config.image.os,
                     ),
                     codebuild.CfnProject.EnvironmentVariableProperty(
                         name="NOTIFICATION_URL",
                         value=self._docker_build_wait_condition_handle.ref,
                     ),
                 ],
-                image="aws/codebuild/amazonlinux2-aarch64-standard:1.0"
+                image="aws/codebuild/amazonlinux2-aarch64-standard:2.0"
                 if self._condition_use_arm_code_build_image()
-                else "aws/codebuild/amazonlinux2-x86_64-standard:3.0",
+                else "aws/codebuild/amazonlinux2-x86_64-standard:4.0",
                 type="ARM_CONTAINER" if self._condition_use_arm_code_build_image() else "LINUX_CONTAINER",
                 privileged_mode=True,
             ),
             name=f"pcluster-{self.stack_name}-build-docker-images-project",
             service_role=self._code_build_role.attr_arn,
             source=codebuild.CfnProject.SourceProperty(
                 location=f"{self.bucket.name}/{self.bucket.artifact_directory}"
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/cdk_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # This module contains all the classes required to convert a Cluster into a CFN template by using CDK.
 #
-
 import logging
 import os
 import tempfile
 
 from pcluster.config.cluster_config import BaseClusterConfig
 from pcluster.config.imagebuilder_config import ImageBuilderConfig
 from pcluster.models.s3_bucket import S3Bucket
+from pcluster.templates.cdk_artifacts_manager import CDKArtifactsManager
 from pcluster.utils import load_yaml_dict
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CDKTemplateBuilder:
     """Create the template, starting from the given resources."""
@@ -35,23 +35,27 @@
         LOGGER.info("Importing CDK...")
         from aws_cdk.core import App  # pylint: disable=C0415
 
         from pcluster.templates.cluster_stack import ClusterCdkStack  # pylint: disable=C0415
 
         LOGGER.info("CDK import completed successfully")
         LOGGER.info("Starting CDK template generation...")
-        with tempfile.TemporaryDirectory() as tempdir:
+        with tempfile.TemporaryDirectory() as cloud_assembly_dir:
             output_file = str(stack_name)
-            app = App(outdir=str(tempdir))
+            app = App(outdir=str(cloud_assembly_dir))
             ClusterCdkStack(app, output_file, stack_name, cluster_config, bucket, log_group_name)
-            app.synth()
-            generated_template = load_yaml_dict(os.path.join(tempdir, f"{output_file}.template.json"))
-        LOGGER.info("CDK template generation completed successfully")
 
-        return generated_template
+            cloud_assembly = app.synth()
+            LOGGER.info("CDK template generation completed successfully")
+
+            cdk_artifacts_manager = CDKArtifactsManager(cloud_assembly)
+            assets_metadata = cdk_artifacts_manager.upload_assets(bucket=bucket)
+            generated_template = cdk_artifacts_manager.get_template_body()
+
+        return generated_template, assets_metadata
 
     @staticmethod
     def build_imagebuilder_template(image_config: ImageBuilderConfig, image_id: str, bucket: S3Bucket):
         """Build template for the given imagebuilder and return as output in Yaml format."""
         from aws_cdk.core import App  # pylint: disable=C0415
 
         from pcluster.templates.imagebuilder_stack import ImageBuilderCdkStack  # pylint: disable=C0415
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/cdk_builder_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 import pkg_resources
 from aws_cdk import aws_ec2 as ec2
 from aws_cdk import aws_iam as iam
 from aws_cdk import aws_lambda as awslambda
 from aws_cdk import aws_logs as logs
 from aws_cdk.aws_iam import ManagedPolicy, PermissionsBoundary
-from aws_cdk.core import Arn, CfnDeletionPolicy, CfnTag, Construct, Fn, Stack
+from aws_cdk.core import Arn, ArnFormat, CfnDeletionPolicy, CfnTag, Construct, Fn, Stack
 
 from pcluster.config.cluster_config import (
     BaseClusterConfig,
     BaseComputeResource,
     BaseQueue,
     HeadNode,
     SharedStorageType,
     SlurmClusterConfig,
+    SlurmComputeResource,
     SlurmQueue,
 )
 from pcluster.constants import (
     COOKBOOK_PACKAGES_VERSIONS,
     CW_LOGS_RETENTION_DAYS_DEFAULT,
     IAM_ROLE_PATH,
     LAMBDA_VPC_ACCESS_MANAGED_POLICY,
@@ -141,18 +142,18 @@
 
 def get_cluster_tags(stack_name: str, raw_dict: bool = False):
     """Return a list of cluster tags to be used for all the resources."""
     tags = {PCLUSTER_CLUSTER_NAME_TAG: stack_name}
     return tags if raw_dict else dict_to_cfn_tags(tags)
 
 
-def get_custom_tags(config: BaseClusterConfig, raw_dict: bool = False):
+def get_custom_tags(config: Union[BaseClusterConfig, SlurmQueue, SlurmComputeResource], raw_dict: bool = False):
     """Return a list of tags set by the user."""
-    cluster_tags = config.get_cluster_tags()
-    tags = {tag.key: tag.value for tag in cluster_tags} if cluster_tags else {}
+    custom_tags = config.get_tags()
+    tags = {tag.key: tag.value for tag in custom_tags} if custom_tags else {}
     return tags if raw_dict else dict_to_cfn_tags(tags)
 
 
 def get_default_instance_tags(
     stack_name: str,
     config: BaseClusterConfig,
     node: Union[HeadNode, BaseComputeResource],
@@ -306,14 +307,18 @@
 def apply_permissions_boundary(boundary, scope):
     """Apply a permissions boundary to all IAM roles defined in the scope."""
     if boundary:
         boundary = ManagedPolicy.from_managed_policy_arn(scope, "Boundary", boundary)
         PermissionsBoundary.of(scope).apply(boundary)
 
 
+def scheduler_is_slurm(config: BaseClusterConfig):
+    return config.scheduling.scheduler == "slurm"
+
+
 def generate_launch_template_version_cfn_parameter_hash(queue, compute_resource):
     """
     Generate 16 characters hash for compute fleet launch template version cfn parameter.
 
     :param queue
     :param compute_resource
     :return: 16 chars string e.g. 2238a84ac8a74529
@@ -748,15 +753,17 @@
                                         )
                                     ],
                                 ),
                             ]
                         )
 
         if self._config.directory_service:
-            password_secret_arn = Arn.parse(self._config.directory_service.password_secret_arn)
+            password_secret_arn = Arn.split(
+                self._config.directory_service.password_secret_arn, ArnFormat.COLON_RESOURCE_NAME
+            )
             policy.append(
                 iam.PolicyStatement(
                     sid="AllowGettingDirectorySecretValue",
                     actions=[
                         "secretsmanager:GetSecretValue"
                         if password_secret_arn.service == "secretsmanager"
                         else "ssm:GetParameter"
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/cluster_stack.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cluster_stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,72 +13,68 @@
 
 #
 # This module contains all the classes required to convert a Cluster into a CFN template by using CDK.
 #
 import json
 from collections import defaultdict, namedtuple
 from datetime import datetime
-from typing import Dict, List, Union
+from typing import Union
 
 from aws_cdk import aws_cloudformation as cfn
+from aws_cdk import aws_cloudwatch as cloudwatch
 from aws_cdk import aws_dynamodb as dynamomdb
 from aws_cdk import aws_ec2 as ec2
 from aws_cdk import aws_efs as efs
 from aws_cdk import aws_fsx as fsx
 from aws_cdk import aws_iam as iam
-from aws_cdk import aws_lambda as awslambda
 from aws_cdk import aws_logs as logs
 from aws_cdk.core import (
-    CfnCustomResource,
     CfnDeletionPolicy,
     CfnOutput,
     CfnParameter,
-    CfnResource,
     CfnStack,
     CfnTag,
     Construct,
     CustomResource,
+    Duration,
     Fn,
     Stack,
 )
 
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.common import AWSClientError
 from pcluster.config.cluster_config import (
     AwsBatchClusterConfig,
     BaseSharedFsx,
     ExistingFsxOntap,
     ExistingFsxOpenZfs,
-    SchedulerPluginQueue,
     SharedEbs,
     SharedEfs,
     SharedFsxLustre,
     SharedStorageType,
     SlurmClusterConfig,
-    SlurmComputeResource,
-    SlurmQueue,
 )
 from pcluster.constants import (
+    CW_ALARM_DATAPOINTS_TO_ALARM_DEFAULT,
+    CW_ALARM_EVALUATION_PERIODS_DEFAULT,
+    CW_ALARM_PERCENT_THRESHOLD_DEFAULT,
+    CW_ALARM_PERIOD_DEFAULT,
     CW_LOG_GROUP_NAME_PREFIX,
     CW_LOGS_CFN_PARAM_NAME,
     DEFAULT_EPHEMERAL_DIR,
     LUSTRE,
     NODE_BOOTSTRAP_TIMEOUT,
     OS_MAPPING,
-    PCLUSTER_CLUSTER_NAME_TAG,
-    PCLUSTER_COMPUTE_RESOURCE_NAME_TAG,
     PCLUSTER_DYNAMODB_PREFIX,
-    PCLUSTER_QUEUE_NAME_TAG,
     PCLUSTER_S3_ARTIFACTS_DICT,
 )
 from pcluster.models.s3_bucket import S3Bucket
 from pcluster.templates.awsbatch_builder import AwsBatchConstruct
 from pcluster.templates.cdk_builder_utils import (
     CdkLaunchTemplateBuilder,
-    ComputeNodeIamResources,
     HeadNodeIamResources,
     PclusterLambdaConstruct,
     add_lambda_cfn_role,
     apply_permissions_boundary,
     convert_deletion_policy,
     create_hash_suffix,
     generate_launch_template_version_cfn_parameter_hash,
@@ -87,23 +83,23 @@
     get_common_user_data_env,
     get_custom_tags,
     get_default_instance_tags,
     get_default_volume_tags,
     get_directory_service_dna_json_for_head_node,
     get_lambda_log_group_prefix,
     get_log_group_deletion_policy,
-    get_queue_security_groups_full,
     get_shared_storage_ids_by_type,
     get_slurm_specific_dna_json_for_head_node,
     get_user_data_content,
     to_comma_separated_string,
 )
+from pcluster.templates.compute_fleet_stack import ComputeFleetConstruct
 from pcluster.templates.cw_dashboard_builder import CWDashboardConstruct
 from pcluster.templates.slurm_builder import SlurmConstruct
-from pcluster.utils import get_attr, get_http_tokens_setting, get_service_endpoint, join_shell_args
+from pcluster.utils import get_attr, get_http_tokens_setting, get_service_endpoint
 
 StorageInfo = namedtuple("StorageInfo", ["id", "config"])
 
 
 class ClusterCdkStack:
     """Create the CloudFormation stack template for the Cluster."""
 
@@ -179,15 +175,15 @@
         """
         Generate compute fleet role names.
 
         Return a comma separate string for compute fleet role names cfn parameter
         in Scheduler Plugin cfn substack template.
         """
         role_list = []
-        for _, instance_role in self._managed_compute_instance_roles.items():
+        for _, instance_role in self.compute_fleet_resources.managed_compute_instance_roles.items():
             if instance_role is None:
                 continue
             role_list.append(instance_role)
         return ",".join([instance_role.ref for instance_role in role_list])
 
     # -- Parameters -------------------------------------------------------------------------------------------------- #
 
@@ -293,14 +289,53 @@
                 scope=self.stack,
                 id="PclusterDashboard",
                 stack_name=self.stack.stack_name,
                 cluster_config=self.config,
                 head_node_instance=self.head_node_instance,
                 shared_storage_infos=self.shared_storage_infos,
                 cw_log_group_name=self.log_group.log_group_name if self.config.is_cw_logging_enabled else None,
+                cw_log_group=self.log_group,
+            )
+
+            self._add_alarms()
+
+    def _add_alarms(self):
+        self.alarms = []
+
+        metrics_for_alarms = {
+            "Mem": cloudwatch.Metric(
+                namespace="CWAgent",
+                metric_name="mem_used_percent",
+                dimensions_map={"InstanceId": self.head_node_instance.ref},
+                statistic="Maximum",
+                period=Duration.seconds(CW_ALARM_PERIOD_DEFAULT),
+            ),
+            "Disk": cloudwatch.Metric(
+                namespace="CWAgent",
+                metric_name="disk_used_percent",
+                dimensions_map={"InstanceId": self.head_node_instance.ref, "path": "/"},
+                statistic="Maximum",
+                period=Duration.seconds(CW_ALARM_PERIOD_DEFAULT),
+            ),
+        }
+
+        for metric_key, metric in metrics_for_alarms.items():
+            alarm_id = f"HeadNode{metric_key}Alarm"
+            alarm_name = f"{self.stack.stack_name}_{metric_key}Alarm_HeadNode"
+            self.alarms.append(
+                cloudwatch.Alarm(
+                    scope=self.stack,
+                    id=alarm_id,
+                    metric=metric,
+                    evaluation_periods=CW_ALARM_EVALUATION_PERIODS_DEFAULT,
+                    threshold=CW_ALARM_PERCENT_THRESHOLD_DEFAULT,
+                    alarm_name=alarm_name,
+                    comparison_operator=cloudwatch.ComparisonOperator.GREATER_THAN_THRESHOLD,
+                    datapoints_to_alarm=CW_ALARM_DATAPOINTS_TO_ALARM_DEFAULT,
+                )
             )
 
     def _add_iam_resources(self):
         head_node_iam_resources = HeadNodeIamResources(
             self.stack,
             "HeadNodeIamResources",
             self.config,
@@ -308,29 +343,14 @@
             self.shared_storage_infos,
             "HeadNode",
             self.bucket,
         )
         self._head_node_instance_profile = head_node_iam_resources.instance_profile
         self._managed_head_node_instance_role = head_node_iam_resources.instance_role
 
-        if not self._condition_is_batch():
-            iam_resources = {}
-            for queue in self.config.scheduling.queues:
-                iam_resources[queue.name] = ComputeNodeIamResources(
-                    self.stack,
-                    f"ComputeNodeIamResources{queue.name}",
-                    self.config,
-                    queue,
-                    self.shared_storage_infos,
-                    queue.name,
-                )
-
-            self._compute_instance_profiles = {k: v.instance_profile for k, v in iam_resources.items()}
-            self._managed_compute_instance_roles = {k: v.instance_role for k, v in iam_resources.items()}
-
     def _add_cluster_log_group(self):
         log_group = logs.CfnLogGroup(
             self.stack,
             "CloudWatchLogGroup",
             log_group_name=self.log_group_name,
             retention_in_days=get_cloud_watch_logs_retention_days(self.config),
         )
@@ -344,15 +364,14 @@
             self.scheduler_resources = SlurmConstruct(
                 scope=self.stack,
                 id="Slurm",
                 stack_name=self._stack_name,
                 cluster_config=self.config,
                 bucket=self.bucket,
                 managed_head_node_instance_role=self._managed_head_node_instance_role,
-                managed_compute_instance_roles=self._managed_compute_instance_roles,
                 cleanup_lambda_role=cleanup_lambda_role,  # None if provided by the user
                 cleanup_lambda=cleanup_lambda,
             )
         if not self._condition_is_batch():
             _dynamodb_table_status = dynamomdb.CfnTable(
                 self.stack,
                 "DynamoDBTable",
@@ -375,18 +394,18 @@
                 log_group=self.log_group,
                 cleanup_lambda=cleanup_lambda,
                 cleanup_lambda_role=cleanup_lambda_role,
                 compute_security_group=self._compute_security_group,
                 shared_storage_infos=self.shared_storage_infos,
                 shared_storage_mount_dirs=self.shared_storage_mount_dirs,
                 shared_storage_attributes=self.shared_storage_attributes,
-                compute_node_instance_profiles=self._compute_instance_profiles,
                 cluster_hosted_zone=self.scheduler_resources.cluster_hosted_zone if self.scheduler_resources else None,
                 dynamodb_table=self.scheduler_resources.dynamodb_table if self.scheduler_resources else None,
                 head_eni=self._head_eni,
+                slurm_construct=self.scheduler_resources,
             )
         self._add_scheduler_plugin_substack()
 
     def _add_cleanup_resources_lambda(self):
         """Create Lambda cleanup resources function and its role."""
         cleanup_resources_lambda_role = None
         if self._condition_create_lambda_iam_role():
@@ -957,19 +976,14 @@
                 ],
             ),
         )
 
         # Metadata
         head_node_launch_template.add_metadata("Comment", "AWS ParallelCluster Head Node")
         # CloudFormation::Init metadata
-        pre_install_action, post_install_action, post_update_action = (None, None, None)
-        if head_node.custom_actions:
-            pre_install_action = head_node.custom_actions.on_node_start
-            post_install_action = head_node.custom_actions.on_node_configured
-            post_update_action = head_node.custom_actions.on_node_updated
 
         dna_json = json.dumps(
             {
                 "cluster": {
                     "stack_name": self._stack_name,
                     "stack_arn": self.stack.stack_id,
                     "scheduler_plugin_substack_arn": self.scheduler_plugin_stack.ref
@@ -979,26 +993,14 @@
                     "raid_shared_dir": to_comma_separated_string(
                         self.shared_storage_mount_dirs[SharedStorageType.RAID]
                     ),
                     "raid_type": to_comma_separated_string(
                         self.shared_storage_attributes[SharedStorageType.RAID]["Type"]
                     ),
                     "base_os": self.config.image.os,
-                    "preinstall": pre_install_action.script if pre_install_action else "NONE",
-                    "preinstall_args": join_shell_args(pre_install_action.args)
-                    if pre_install_action and pre_install_action.args
-                    else "NONE",
-                    "postinstall": post_install_action.script if post_install_action else "NONE",
-                    "postinstall_args": join_shell_args(post_install_action.args)
-                    if post_install_action and post_install_action.args
-                    else "NONE",
-                    "postupdate": post_update_action.script if post_update_action else "NONE",
-                    "postupdate_args": join_shell_args(post_update_action.args)
-                    if post_update_action and post_update_action.args
-                    else "NONE",
                     "region": self.stack.region,
                     "efs_fs_ids": get_shared_storage_ids_by_type(self.shared_storage_infos, SharedStorageType.EFS),
                     "efs_shared_dirs": to_comma_separated_string(self.shared_storage_mount_dirs[SharedStorageType.EFS]),
                     "efs_encryption_in_transits": to_comma_separated_string(
                         self.shared_storage_attributes[SharedStorageType.EFS]["EncryptionInTransits"],
                         use_lower_case=True,
                     ),
@@ -1032,14 +1034,15 @@
                     "log_group_name": self.log_group.log_group_name
                     if self.config.monitoring.logs.cloud_watch.enabled
                     else "NONE",
                     "dcv_enabled": "head_node" if self.config.is_dcv_enabled else "false",
                     "dcv_port": head_node.dcv.port if head_node.dcv else "NONE",
                     "enable_intel_hpc_platform": "true" if self.config.is_intel_hpc_platform_enabled else "false",
                     "cw_logging_enabled": "true" if self.config.is_cw_logging_enabled else "false",
+                    "log_rotation_enabled": "true" if self.config.is_log_rotation_enabled else "false",
                     "cluster_s3_bucket": self.bucket.name,
                     "cluster_config_s3_key": "{0}/configs/{1}".format(
                         self.bucket.artifact_directory, PCLUSTER_S3_ARTIFACTS_DICT.get("config_name")
                     ),
                     "cluster_config_version": self.config.config_version,
                     "change_set_s3_key": f"{self.bucket.artifact_directory}/configs/"
                     f"{PCLUSTER_S3_ARTIFACTS_DICT.get('change_set_name')}",
@@ -1273,17 +1276,17 @@
         return head_node_instance
 
     def _get_launch_templates_config(self):
         if not self.compute_fleet_resources:
             return None
 
         lt_config = {"Queues": {}}
-        for queue, compute_resouces in self.compute_fleet_resources.compute_launch_templates.items():
+        for queue, compute_resources in self.compute_fleet_resources.launch_templates.items():
             lt_config["Queues"][queue] = {"ComputeResources": {}}
-            for compute_resource, launch_template in compute_resouces.items():
+            for compute_resource, launch_template in compute_resources.items():
                 lt_config["Queues"][queue]["ComputeResources"][compute_resource] = {
                     "LaunchTemplate": {"Id": launch_template.ref, "Version": launch_template.attr_latest_version_number}
                 }
 
         return lt_config
 
     def _add_scheduler_plugin_substack(self):
@@ -1367,333 +1370,7 @@
 
         CfnOutput(
             self.stack,
             "HeadNodePrivateDnsName",
             description="Private DNS name of the head node",
             value=self.head_node_instance.attr_private_dns_name,
         )
-
-
-class ComputeFleetConstruct(Construct):
-    """Construct defining compute fleet specific resources."""
-
-    def __init__(
-        self,
-        scope: Construct,
-        id: str,
-        cluster_config: SlurmClusterConfig,
-        log_group: logs.CfnLogGroup,
-        cleanup_lambda: awslambda.CfnFunction,
-        cleanup_lambda_role: iam.CfnRole,
-        compute_security_group: ec2.CfnSecurityGroup,
-        shared_storage_infos: Dict,
-        shared_storage_mount_dirs: Dict,
-        shared_storage_attributes: Dict,
-        compute_node_instance_profiles: Dict[str, str],
-        cluster_hosted_zone,
-        dynamodb_table,
-        head_eni,
-    ):
-        super().__init__(scope, id)
-        self._cleanup_lambda = cleanup_lambda
-        self._cleanup_lambda_role = cleanup_lambda_role
-        self._compute_security_group = compute_security_group
-        self._config = cluster_config
-        self._shared_storage_infos = shared_storage_infos
-        self._shared_storage_mount_dirs = shared_storage_mount_dirs
-        self._shared_storage_attributes = shared_storage_attributes
-        self._log_group = log_group
-        self._cluster_hosted_zone = cluster_hosted_zone
-        self._dynamodb_table = dynamodb_table
-        self._compute_node_instance_profiles = compute_node_instance_profiles
-        self._head_eni = head_eni
-        self._launch_template_builder = CdkLaunchTemplateBuilder()
-        self._add_resources()
-
-    # -- Utility methods --------------------------------------------------------------------------------------------- #
-
-    @property
-    def stack_name(self):
-        """Name of the CFN stack."""
-        return Stack.of(self).stack_name
-
-    # -- Resources --------------------------------------------------------------------------------------------------- #
-
-    def _add_resources(self):
-        managed_placement_groups = self._add_placement_groups()
-        self.compute_launch_templates = self._add_launch_templates(
-            managed_placement_groups, self._compute_node_instance_profiles
-        )
-        custom_resource_deps = list(managed_placement_groups.values())
-        if self._compute_security_group:
-            custom_resource_deps.append(self._compute_security_group)
-        self._add_cleanup_custom_resource(dependencies=custom_resource_deps)
-
-    def _add_cleanup_custom_resource(self, dependencies: List[CfnResource]):
-        terminate_compute_fleet_custom_resource = CfnCustomResource(
-            self,
-            "TerminateComputeFleetCustomResource",
-            service_token=self._cleanup_lambda.attr_arn,
-        )
-        terminate_compute_fleet_custom_resource.add_property_override("StackName", self.stack_name)
-        terminate_compute_fleet_custom_resource.add_property_override("Action", "TERMINATE_EC2_INSTANCES")
-        for dep in dependencies:
-            terminate_compute_fleet_custom_resource.add_depends_on(dep)
-
-        if self._cleanup_lambda_role:
-            self._add_policies_to_cleanup_resources_lambda_role()
-
-    def _add_policies_to_cleanup_resources_lambda_role(self):
-        self._cleanup_lambda_role.policies[0].policy_document.add_statements(
-            iam.PolicyStatement(
-                actions=["ec2:DescribeInstances"],
-                resources=["*"],
-                effect=iam.Effect.ALLOW,
-                sid="DescribeInstances",
-            ),
-            iam.PolicyStatement(
-                actions=["ec2:TerminateInstances"],
-                resources=["*"],
-                effect=iam.Effect.ALLOW,
-                conditions={"StringEquals": {f"ec2:ResourceTag/{PCLUSTER_CLUSTER_NAME_TAG}": self.stack_name}},
-                sid="FleetTerminatePolicy",
-            ),
-        )
-
-    def _add_placement_groups(self) -> Dict[str, ec2.CfnPlacementGroup]:
-        managed_placement_groups = {}
-        for queue in self._config.scheduling.queues:
-            for key in queue.get_managed_placement_group_keys():
-                managed_placement_groups[key] = ec2.CfnPlacementGroup(
-                    self,
-                    f"PlacementGroup{create_hash_suffix(key)}",
-                    strategy="cluster",
-                )
-        return managed_placement_groups
-
-    @staticmethod
-    def _get_placement_group_for_compute_resource(queue, managed_placement_groups, compute_resource) -> str:
-        placement_group_settings = queue.get_placement_group_settings_for_compute_resource(compute_resource)
-        placement_group_key = placement_group_settings.get("key")
-        managed = placement_group_settings.get("is_managed")
-        return managed_placement_groups[placement_group_key].ref if managed else placement_group_key
-
-    def _add_launch_templates(self, managed_placement_groups, instance_profiles):
-        compute_launch_templates = {}
-        for queue in self._config.scheduling.queues:
-            compute_launch_templates[queue.name] = {}
-            queue_lt_security_groups = get_queue_security_groups_full(self._compute_security_group, queue)
-            queue_pre_install_action, queue_post_install_action = (None, None)
-            if queue.custom_actions:
-                queue_pre_install_action = queue.custom_actions.on_node_start
-                queue_post_install_action = queue.custom_actions.on_node_configured
-
-            for resource in queue.compute_resources:
-                compute_launch_templates[queue.name][resource.name] = self._add_compute_resource_launch_template(
-                    queue,
-                    resource,
-                    queue_pre_install_action,
-                    queue_post_install_action,
-                    queue_lt_security_groups,
-                    self._get_placement_group_for_compute_resource(queue, managed_placement_groups, resource),
-                    instance_profiles,
-                )
-        return compute_launch_templates
-
-    def _add_compute_resource_launch_template(
-        self,
-        queue,
-        compute_resource,
-        queue_pre_install_action,
-        queue_post_install_action,
-        queue_lt_security_groups,
-        placement_group,
-        instance_profiles,
-    ):
-        # LT network interfaces
-        compute_lt_nw_interfaces = [
-            ec2.CfnLaunchTemplate.NetworkInterfaceProperty(
-                device_index=0,
-                associate_public_ip_address=queue.networking.assign_public_ip
-                if compute_resource.max_network_interface_count == 1
-                else None,  # parameter not supported for instance types with multiple network interfaces
-                interface_type="efa" if compute_resource.efa and compute_resource.efa.enabled else None,
-                groups=queue_lt_security_groups,
-                subnet_id=queue.networking.subnet_ids[0]
-                if isinstance(compute_resource, SlurmComputeResource)
-                else None,
-            )
-        ]
-
-        for network_interface_index in range(1, compute_resource.max_network_interface_count):
-            compute_lt_nw_interfaces.append(
-                ec2.CfnLaunchTemplate.NetworkInterfaceProperty(
-                    device_index=0,
-                    network_card_index=network_interface_index,
-                    interface_type="efa" if compute_resource.efa and compute_resource.efa.enabled else None,
-                    groups=queue_lt_security_groups,
-                    subnet_id=queue.networking.subnet_ids[0]
-                    if isinstance(compute_resource, SlurmComputeResource)
-                    else None,
-                )
-            )
-
-        conditional_template_properties = {}
-        if compute_resource.is_ebs_optimized:
-            conditional_template_properties.update({"ebs_optimized": True})
-        if isinstance(compute_resource, SlurmComputeResource):
-            conditional_template_properties.update({"instance_type": compute_resource.instance_type})
-
-        return ec2.CfnLaunchTemplate(
-            self,
-            f"LaunchTemplate{create_hash_suffix(queue.name + compute_resource.name)}",
-            launch_template_name=f"{self.stack_name}-{queue.name}-{compute_resource.name}",
-            launch_template_data=ec2.CfnLaunchTemplate.LaunchTemplateDataProperty(
-                block_device_mappings=self._launch_template_builder.get_block_device_mappings(
-                    queue.compute_settings.local_storage.root_volume, self._config.image.os
-                ),
-                # key_name=,
-                network_interfaces=compute_lt_nw_interfaces,
-                placement=ec2.CfnLaunchTemplate.PlacementProperty(group_name=placement_group),
-                image_id=self._config.image_dict[queue.name],
-                iam_instance_profile=ec2.CfnLaunchTemplate.IamInstanceProfileProperty(
-                    name=instance_profiles[queue.name]
-                ),
-                instance_market_options=self._launch_template_builder.get_instance_market_options(
-                    queue, compute_resource
-                ),
-                instance_initiated_shutdown_behavior="terminate",
-                capacity_reservation_specification=self._launch_template_builder.get_capacity_reservation(
-                    queue,
-                    compute_resource,
-                ),
-                metadata_options=ec2.CfnLaunchTemplate.MetadataOptionsProperty(
-                    http_tokens=get_http_tokens_setting(self._config.imds.imds_support)
-                ),
-                user_data=Fn.base64(
-                    Fn.sub(
-                        get_user_data_content("../resources/compute_node/user_data.sh"),
-                        {
-                            **{
-                                "EnableEfa": "efa" if compute_resource.efa and compute_resource.efa.enabled else "NONE",
-                                "RAIDSharedDir": to_comma_separated_string(
-                                    self._shared_storage_mount_dirs[SharedStorageType.RAID]
-                                ),
-                                "RAIDType": to_comma_separated_string(
-                                    self._shared_storage_attributes[SharedStorageType.RAID]["Type"]
-                                ),
-                                "DisableMultiThreadingManually": "true"
-                                if compute_resource.disable_simultaneous_multithreading_manually
-                                else "false",
-                                "BaseOS": self._config.image.os,
-                                "PreInstallScript": queue_pre_install_action.script
-                                if queue_pre_install_action
-                                else "NONE",
-                                "PreInstallArgs": join_shell_args(queue_pre_install_action.args)
-                                if queue_pre_install_action and queue_pre_install_action.args
-                                else "NONE",
-                                "PostInstallScript": queue_post_install_action.script
-                                if queue_post_install_action
-                                else "NONE",
-                                "PostInstallArgs": join_shell_args(queue_post_install_action.args)
-                                if queue_post_install_action and queue_post_install_action.args
-                                else "NONE",
-                                "EFSIds": get_shared_storage_ids_by_type(
-                                    self._shared_storage_infos, SharedStorageType.EFS
-                                ),
-                                "EFSSharedDirs": to_comma_separated_string(
-                                    self._shared_storage_mount_dirs[SharedStorageType.EFS]
-                                ),
-                                "EFSEncryptionInTransits": to_comma_separated_string(
-                                    self._shared_storage_attributes[SharedStorageType.EFS]["EncryptionInTransits"],
-                                    use_lower_case=True,
-                                ),
-                                "EFSIamAuthorizations": to_comma_separated_string(
-                                    self._shared_storage_attributes[SharedStorageType.EFS]["IamAuthorizations"],
-                                    use_lower_case=True,
-                                ),
-                                "FSXIds": get_shared_storage_ids_by_type(
-                                    self._shared_storage_infos, SharedStorageType.FSX
-                                ),
-                                "FSXMountNames": to_comma_separated_string(
-                                    self._shared_storage_attributes[SharedStorageType.FSX]["MountNames"]
-                                ),
-                                "FSXDNSNames": to_comma_separated_string(
-                                    self._shared_storage_attributes[SharedStorageType.FSX]["DNSNames"]
-                                ),
-                                "FSXVolumeJunctionPaths": to_comma_separated_string(
-                                    self._shared_storage_attributes[SharedStorageType.FSX]["VolumeJunctionPaths"]
-                                ),
-                                "FSXFileSystemTypes": to_comma_separated_string(
-                                    self._shared_storage_attributes[SharedStorageType.FSX]["FileSystemTypes"]
-                                ),
-                                "FSXSharedDirs": to_comma_separated_string(
-                                    self._shared_storage_mount_dirs[SharedStorageType.FSX]
-                                ),
-                                "Scheduler": self._config.scheduling.scheduler,
-                                "EphemeralDir": queue.compute_settings.local_storage.ephemeral_volume.mount_dir
-                                if isinstance(queue, (SlurmQueue, SchedulerPluginQueue))
-                                and queue.compute_settings.local_storage.ephemeral_volume
-                                else DEFAULT_EPHEMERAL_DIR,
-                                "EbsSharedDirs": to_comma_separated_string(
-                                    self._shared_storage_mount_dirs[SharedStorageType.EBS]
-                                ),
-                                "ClusterDNSDomain": str(self._cluster_hosted_zone.name)
-                                if self._cluster_hosted_zone
-                                else "",
-                                "ClusterHostedZone": str(self._cluster_hosted_zone.ref)
-                                if self._cluster_hosted_zone
-                                else "",
-                                "OSUser": OS_MAPPING[self._config.image.os]["user"],
-                                "SlurmDynamoDBTable": self._dynamodb_table.ref if self._dynamodb_table else "NONE",
-                                "LogGroupName": self._log_group.log_group_name
-                                if self._config.monitoring.logs.cloud_watch.enabled
-                                else "NONE",
-                                "IntelHPCPlatform": "true" if self._config.is_intel_hpc_platform_enabled else "false",
-                                "CWLoggingEnabled": "true" if self._config.is_cw_logging_enabled else "false",
-                                "QueueName": queue.name,
-                                "ComputeResourceName": compute_resource.name,
-                                "EnableEfaGdr": "compute"
-                                if compute_resource.efa and compute_resource.efa.gdr_support
-                                else "NONE",
-                                "CustomNodePackage": self._config.custom_node_package or "",
-                                "CustomAwsBatchCliPackage": self._config.custom_aws_batch_cli_package or "",
-                                "ExtraJson": self._config.extra_chef_attributes,
-                                "UsePrivateHostname": str(
-                                    get_attr(self._config, "scheduling.settings.dns.use_ec2_hostnames", default=False)
-                                ).lower(),
-                                "HeadNodePrivateIp": self._head_eni.attr_primary_private_ip_address,
-                                "DirectoryServiceEnabled": str(self._config.directory_service is not None).lower(),
-                                "Timeout": str(
-                                    get_attr(
-                                        self._config,
-                                        "dev_settings.timeouts.compute_node_bootstrap_timeout",
-                                        NODE_BOOTSTRAP_TIMEOUT,
-                                    )
-                                ),
-                            },
-                            **get_common_user_data_env(queue, self._config),
-                        },
-                    )
-                ),
-                monitoring=ec2.CfnLaunchTemplate.MonitoringProperty(enabled=False),
-                tag_specifications=[
-                    ec2.CfnLaunchTemplate.TagSpecificationProperty(
-                        resource_type="instance",
-                        tags=get_default_instance_tags(
-                            self.stack_name, self._config, compute_resource, "Compute", self._shared_storage_infos
-                        )
-                        + [CfnTag(key=PCLUSTER_QUEUE_NAME_TAG, value=queue.name)]
-                        + [CfnTag(key=PCLUSTER_COMPUTE_RESOURCE_NAME_TAG, value=compute_resource.name)]
-                        + get_custom_tags(self._config),
-                    ),
-                    ec2.CfnLaunchTemplate.TagSpecificationProperty(
-                        resource_type="volume",
-                        tags=get_default_volume_tags(self.stack_name, "Compute")
-                        + [CfnTag(key=PCLUSTER_QUEUE_NAME_TAG, value=queue.name)]
-                        + [CfnTag(key=PCLUSTER_COMPUTE_RESOURCE_NAME_TAG, value=compute_resource.name)]
-                        + get_custom_tags(self._config),
-                    ),
-                ],
-                **conditional_template_properties,
-            ),
-        )
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/cw_dashboard_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cw_dashboard_builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,64 +5,78 @@
 #
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict, namedtuple
+from typing import Iterable
 
 from aws_cdk import aws_cloudwatch as cloudwatch
 from aws_cdk import aws_ec2 as ec2
-from aws_cdk.core import Construct, Stack
+from aws_cdk import aws_logs as logs
+from aws_cdk.core import Construct, Duration, Stack
 
 from pcluster.config.cluster_config import BaseClusterConfig, SharedFsxLustre, SharedStorageType
 
 MAX_WIDTH = 24
 
 
 class Coord:
     """Create coordinates for locating cloudwatch graphs."""
 
     def __init__(self, x_value: int, y_value: int):
         self.x_value = x_value
         self.y_value = y_value
 
 
-_PclusterMetric = namedtuple("_PclusterMetric", ["title", "metrics", "supported_vol_types"])
+_PclusterMetric = namedtuple(
+    "_PclusterMetric", ["title", "metrics", "supported_vol_types", "namespace", "additional_dimensions"]
+)
+_CustomMetricFilter = namedtuple(
+    "_CustomMetricFilter",
+    ["metric_name", "filter_pattern", "metric_value", "metric_statistic", "metric_unit"],
+    defaults=("Sum", "Count"),
+)
 _Filter = namedtuple("new_filter", ["pattern", "param"])
 _CWLogWidget = namedtuple(
     "_CWLogWidget",
     ["title", "conditions", "fields", "filters", "sort", "limit"],
 )
+_HealthMetric = namedtuple(
+    "_ErrorMetric", ["title", "metric_filters", "left_y_axis", "left_annotations"], defaults=(None, None)
+)
 
 
-def new_pcluster_metric(title=None, metrics=None, supported_vol_types=None):
-    return _PclusterMetric(title, metrics, supported_vol_types)
+def new_pcluster_metric(title=None, metrics=None, supported_vol_types=None, namespace=None, additional_dimensions=None):
+    return _PclusterMetric(title, metrics, supported_vol_types, namespace, additional_dimensions)
 
 
 class CWDashboardConstruct(Construct):
     """Create the resources required when creating cloudwatch dashboard."""
 
     def __init__(
         self,
         scope: Construct,
         stack_name: str,
         id: str,
         cluster_config: BaseClusterConfig,
         head_node_instance: ec2.CfnInstance,
         shared_storage_infos: dict,
         cw_log_group_name: str,
+        cw_log_group: logs.CfnLogGroup,
     ):
         super().__init__(scope, id)
         self.stack_scope = scope
         self.stack_name = stack_name
         self.config = cluster_config
         self.head_node_instance = head_node_instance
         self.shared_storage_infos = shared_storage_infos
         self.cw_log_group_name = cw_log_group_name
+        self.cw_log_group = cw_log_group
 
         self.dashboard_name = self.stack_name + "-" + self._stack_region
         self.coord = Coord(x_value=0, y_value=0)
         self.graph_width = 6
         self.graph_height = 6
         self.logs_width = MAX_WIDTH
         self.logs_height = 6
@@ -127,16 +141,18 @@
         if len(self.shared_storage_infos[SharedStorageType.EFS]) > 0:
             self._add_efs_metrics_graphs()
 
         # Add FSx metrics graphs
         if len(self.shared_storage_infos[SharedStorageType.FSX]) > 0:
             self._add_fsx_metrics_graphs()
 
-        # Head Node logs, if CW Logs are enabled
+        # Head Node logs add custom metrics if cw_log and metrics are enabled
         if self.config.is_cw_logging_enabled:
+            if self.config.scheduling.scheduler == "slurm":
+                self._add_custom_health_metrics()
             self._add_cw_log()
 
     def _update_coord(self, d_x, d_y):
         """Calculate coordinates for the new graph."""
         self.coord.x_value = self.coord.x_value + d_x
         x_value = self.coord.x_value + d_x
         if x_value > MAX_WIDTH:  # updates both x and y values
@@ -166,32 +182,35 @@
     def _add_text_widget(self, markdown):
         """Add the textwidget to the cloudwatch dashboard and update coordinates."""
         text_widget = cloudwatch.TextWidget(markdown="\n" + markdown + "\n", height=1, width=MAX_WIDTH)
         text_widget.position(x=self.coord.x_value, y=self.coord.y_value)
         self.cloudwatch_dashboard.add_widgets(text_widget)
         self._update_coord_after_section(d_y=1)
 
-    def _generate_graph_widget(self, title, metric_list):
+    def _generate_graph_widget(self, title, metric_list, **widget_kwargs):
         """Generate a graph widget and update the coordinates."""
         widget = cloudwatch.GraphWidget(
             title=title,
             left=metric_list,
             region=self._stack_region,
             width=self.graph_width,
             height=self.graph_height,
+            **widget_kwargs,
         )
         widget.position(x=self.coord.x_value, y=self.coord.y_value)
         self._update_coord(self.graph_width, self.graph_height)
         return widget
 
-    def _generate_ec2_metrics_list(self, metrics):
+    def _generate_metrics_list(self, metrics_param):
         metric_list = []
-        for metric in metrics:
+        dimensions_map = {"InstanceId": self.head_node_instance.ref}
+        dimensions_map.update(metrics_param.additional_dimensions if metrics_param.additional_dimensions else {})
+        for metric in metrics_param.metrics:
             cloudwatch_metric = cloudwatch.Metric(
-                namespace="AWS/EC2", metric_name=metric, dimensions_map={"InstanceId": self.head_node_instance.ref}
+                namespace=metrics_param.namespace, metric_name=metric, dimensions_map=dimensions_map
             )
             metric_list.append(cloudwatch_metric)
         return metric_list
 
     def _add_conditional_storage_widgets(
         self,
         conditional_metrics,
@@ -214,14 +233,204 @@
                     metric_list.append(cloudwatch_metric)
 
             if len(metric_list) > 0:  # Add the metrics only if there exist support volumes for it
                 graph_widget = self._generate_graph_widget(metric_condition_params.title, metric_list)
                 widgets_list.append(graph_widget)
         return widgets_list
 
+    def _add_custom_pcluster_metric_filter(
+        self, metric_name, filter_pattern, custom_namespace, metric_value, metric_unit=None
+    ):
+        """Adding custom metric filter from named tuple."""
+        metric_filter = logs.CfnMetricFilter(
+            scope=self.stack_scope,
+            id=metric_name + " Filter",
+            filter_pattern=filter_pattern,
+            log_group_name=self.cw_log_group_name,
+            metric_transformations=[
+                logs.CfnMetricFilter.MetricTransformationProperty(
+                    metric_namespace=custom_namespace,
+                    metric_name=metric_name,
+                    metric_value=metric_value,
+                    unit=metric_unit,
+                    dimensions=[
+                        logs.CfnMetricFilter.DimensionProperty(
+                            key="ClusterName",
+                            value="$.cluster-name",
+                        ),
+                    ],
+                )
+            ],
+        )
+        metric_filter.add_depends_on(self.cw_log_group)
+        return metric_filter
+
+    def _add_custom_health_metrics(self):
+        """Create custom health metric filters and outputs to cloudwatch graph."""
+
+        def _generate_metric_filter_pattern(event_type, failure_type=None):
+            if failure_type:
+                return (
+                    f"{{ $.event-type = {event_type} && $.detail.failure-type = {failure_type} && "
+                    '$.scheduler = "slurm" }'
+                )
+            else:
+                return f'{{ $.event-type = {event_type} && $.scheduler = "slurm" }}'
+
+        metric_value = "$.detail.count"
+        launch_failure_event_type = "node-launch-failure-count"
+        jobs_not_starting_errors = [
+            _CustomMetricFilter(
+                metric_name="IamPolicyErrors",
+                filter_pattern=_generate_metric_filter_pattern(launch_failure_event_type, "iam-policy-errors"),
+                metric_value=metric_value,
+            ),
+            _CustomMetricFilter(
+                metric_name="VcpuLimitErrors",
+                filter_pattern=_generate_metric_filter_pattern(launch_failure_event_type, "vcpu-limit-failures"),
+                metric_value=metric_value,
+            ),
+            _CustomMetricFilter(
+                metric_name="VolumeLimitErrors",
+                filter_pattern=_generate_metric_filter_pattern(launch_failure_event_type, "volume-limit-failures"),
+                metric_value=metric_value,
+            ),
+            _CustomMetricFilter(
+                metric_name="InsufficientCapacityErrors",
+                filter_pattern=_generate_metric_filter_pattern(launch_failure_event_type, "ice-failures"),
+                metric_value=metric_value,
+            ),
+            _CustomMetricFilter(
+                metric_name="OtherInstanceLaunchFailures",
+                filter_pattern=_generate_metric_filter_pattern(launch_failure_event_type, "other-failures"),
+                metric_value=metric_value,
+            ),
+        ]
+
+        compute_node_events = [
+            _CustomMetricFilter(
+                metric_name="InstanceBootstrapTimeoutErrors",
+                filter_pattern='{ $.event-type = "protected-mode-error-count" && '
+                '($.detail.failure-type = "static-replacement-timeout-error" || '
+                '$.detail.failure-type = "dynamic-resume-timeout-error" ) && '
+                '$.scheduler = "slurm" }',
+                metric_value=metric_value,
+            ),
+            _CustomMetricFilter(
+                metric_name="EC2HealthCheckErrors",
+                filter_pattern=_generate_metric_filter_pattern("nodes-failing-health-check-count", "ec2_health_check"),
+                metric_value=metric_value,
+            ),
+            _CustomMetricFilter(
+                metric_name="ScheduledEventHealthCheckErrors",
+                filter_pattern=_generate_metric_filter_pattern(
+                    "nodes-failing-health-check-count", "scheduled_event_health_check"
+                ),
+                metric_value=metric_value,
+            ),
+            _CustomMetricFilter(
+                metric_name="NoCorrespondingInstanceErrors",
+                filter_pattern=_generate_metric_filter_pattern("invalid-backing-instance-count"),
+                metric_value=metric_value,
+            ),
+            # Use text matching here because it comes from slurmctld.log
+            _CustomMetricFilter(
+                metric_name="SlurmNodeNotRespondingErrors",
+                filter_pattern=_generate_metric_filter_pattern("node-not-responding-down-count"),
+                metric_value=metric_value,
+            ),
+        ]
+
+        cluster_health_metrics = [
+            _HealthMetric(
+                "Instance Provisioning Errors",
+                jobs_not_starting_errors,
+                left_y_axis=cloudwatch.YAxisProps(min=0.0),
+            ),
+            _HealthMetric(
+                "Unhealthy Instance Errors",
+                compute_node_events,
+                left_y_axis=cloudwatch.YAxisProps(min=0.0),
+            ),
+        ]
+        if self.config.has_custom_actions_in_queue:
+            custom_action_errors = [
+                _CustomMetricFilter(
+                    metric_name="OnNodeStartDownloadErrors",
+                    filter_pattern='{ $.event-type = "custom-action-error" && $.scheduler = "slurm" && '
+                    '$.detail.action = "OnNodeStart" && $.detail.stage = "downloading"}',
+                    metric_value="1",
+                ),
+                _CustomMetricFilter(
+                    metric_name="OnNodeStartRunErrors",
+                    filter_pattern='{ $.event-type = "custom-action-error" && $.scheduler = "slurm" && '
+                    '$.detail.action = "OnNodeStart" && $.detail.stage = "executing"}',
+                    metric_value="1",
+                ),
+                _CustomMetricFilter(
+                    metric_name="OnNodeConfiguredDownloadErrors",
+                    filter_pattern='{ $.event-type = "custom-action-error" && $.scheduler = "slurm" && '
+                    '$.detail.action = "OnNodeConfigured" && $.detail.stage = "downloading"}',
+                    metric_value="1",
+                ),
+                _CustomMetricFilter(
+                    metric_name="OnNodeConfiguredRunErrors",
+                    filter_pattern='{ $.event-type = "custom-action-error" && $.scheduler = "slurm" && '
+                    '$.detail.action = "OnNodeConfigured" && $.detail.stage = "executing"}',
+                    metric_value="1",
+                ),
+            ]
+
+            cluster_health_metrics.append(
+                _HealthMetric(
+                    "Custom Action Errors",
+                    custom_action_errors,
+                    left_y_axis=cloudwatch.YAxisProps(min=0.0),
+                )
+            )
+
+        cluster_health_metrics.append(
+            _HealthMetric(
+                "Compute Fleet Idle Time",
+                [
+                    _CustomMetricFilter(
+                        metric_name="MaxDynamicNodeIdleTime",
+                        filter_pattern='{ $.event-type = "compute-node-idle-time" && $.scheduler = "slurm" && '
+                        '$.detail.node-type = "dynamic"}',
+                        metric_value="$.detail.longest-idle-time",
+                        metric_statistic="max",
+                        metric_unit="Seconds",
+                    ),
+                ],
+                left_y_axis=cloudwatch.YAxisProps(min=0.0),
+                left_annotations=[
+                    cloudwatch.HorizontalAnnotation(
+                        value=self.config.scheduling.settings.scaledown_idletime * 60,
+                        color=cloudwatch.Color.GREEN,
+                        fill=cloudwatch.Shading.BELOW,
+                        visible=True,
+                    ),
+                    cloudwatch.HorizontalAnnotation(
+                        value=self.config.scheduling.settings.scaledown_idletime * 60,
+                        label="Idle Time Scaledown",
+                        color=cloudwatch.Color.BLUE,
+                        fill=cloudwatch.Shading.ABOVE,
+                        visible=True,
+                    ),
+                ],
+            )
+        )
+
+        self._add_text_widget("# Cluster Health Metrics")
+        self._add_health_metrics_graph_widgets(cluster_health_metrics)
+        self._add_text_widget(
+            "General [Troubleshooting Resources]"
+            "(https://docs.aws.amazon.com/parallelcluster/latest/ug/troubleshooting.html)"
+        )
+
     def _add_storage_widgets(self, metrics, storages_list, namespace, dimension_name):
         widgets_list = []
         for metrics_param in metrics:
             metric_list = []
             for metric in metrics_param.metrics:
                 for storage in storages_list:
                     cloudwatch_metric = cloudwatch.Metric(
@@ -285,29 +494,47 @@
             widgets_list.append(self._generate_graph_widget(title, metric_list))
         return widgets_list
 
     def _add_head_node_instance_metrics_graphs(self):
         # Create a text widget for subtitle "Head Node Instance Metrics"
         self._add_text_widget("## Head Node Instance Metrics")
 
-        # EC2 metrics graph for head node instance
+        # EC2 metrics for graph for head node instance
         ec2_metrics = [
-            new_pcluster_metric(title="CPU Utilization", metrics=["CPUUtilization"]),
-            new_pcluster_metric(title="Network Packets In/Out", metrics=["NetworkPacketsIn", "NetworkPacketsOut"]),
-            new_pcluster_metric(title="Network In and Out", metrics=["NetworkIn", "NetworkOut"]),
-            new_pcluster_metric(title="Disk Read/Write Bytes", metrics=["DiskReadBytes", "DiskWriteBytes"]),
-            new_pcluster_metric(title="Disk Read/Write Ops", metrics=["DiskReadOps", "DiskWriteOps"]),
+            new_pcluster_metric(title="CPU Utilization", metrics=["CPUUtilization"], namespace="AWS/EC2"),
+            new_pcluster_metric(
+                title="Network Packets In/Out", metrics=["NetworkPacketsIn", "NetworkPacketsOut"], namespace="AWS/EC2"
+            ),
+            new_pcluster_metric(title="Network In and Out", metrics=["NetworkIn", "NetworkOut"], namespace="AWS/EC2"),
+            new_pcluster_metric(
+                title="Disk Read/Write Bytes", metrics=["DiskReadBytes", "DiskWriteBytes"], namespace="AWS/EC2"
+            ),
+            new_pcluster_metric(
+                title="Disk Read/Write Ops", metrics=["DiskReadOps", "DiskWriteOps"], namespace="AWS/EC2"
+            ),
         ]
 
-        # Create EC2 metrics graphs and update coordinates
+        # CW Agent metrics for graph for head node instance
+        cwagent_metrics = [
+            new_pcluster_metric(
+                title="Disk Used Percent",
+                metrics=["disk_used_percent"],
+                namespace="CWAgent",
+                additional_dimensions={"path": "/"},
+            ),
+            new_pcluster_metric(title="Memory Used Percent", metrics=["mem_used_percent"], namespace="CWAgent"),
+        ]
+
+        # Create graphs for EC2 metrics and CW Agent metrics and update coordinates
         widgets_list = []
-        for metrics_param in ec2_metrics:
-            metrics_list = self._generate_ec2_metrics_list(metrics_param.metrics)
+        for metrics_param in ec2_metrics + cwagent_metrics:
+            metrics_list = self._generate_metrics_list(metrics_param)
             graph_widget = self._generate_graph_widget(metrics_param.title, metrics_list)
             widgets_list.append(graph_widget)
+
         self.cloudwatch_dashboard.add_widgets(*widgets_list)
         self._update_coord_after_section(self.graph_height)
 
     def _add_volume_metrics_graphs(self, title, storage_type, ebs_metrics, conditional_ebs_metrics):
         self._add_text_widget(title)
 
         # Get a list of volumes
@@ -374,15 +601,15 @@
             storages_list=fsx_volumes_list,
         )
         self.cloudwatch_dashboard.add_widgets(*widgets_list)
         self._update_coord_after_section(self.graph_height)
 
     def _add_cw_log(self):
         # Create a text widget for subtitle "Head Node Logs"
-        self._add_text_widget("## Head Node Logs")
+        self._add_text_widget("# Head Node Logs")
 
         dcv_enabled = self.config.is_dcv_enabled
         scheduler = self.config.scheduling.scheduler
         base_os = self.config.image.os
         head_private_ip = self.head_node_instance.attr_private_ip
 
         Condition = namedtuple("Condition", ["allowed_values", "param"])
@@ -460,15 +687,15 @@
                 ],
             ),
             SectionWidgets(
                 "System's logs",
                 [
                     self._new_cw_log_widget(
                         title="system-messages",
-                        conditions=[Condition(["alinux2", "centos7"], base_os)],
+                        conditions=[Condition(["alinux2", "centos7", "rhel8"], base_os)],
                         filters=[self._new_filter(pattern=f"{head_private_ip}.*system-messages")],
                     ),
                     self._new_cw_log_widget(
                         title="syslog",
                         conditions=[Condition(["ubuntu1804", "ubuntu2004"], base_os)],
                         filters=[self._new_filter(pattern=f"{head_private_ip}.*syslog")],
                     ),
@@ -530,7 +757,40 @@
             limit = 100
         return _CWLogWidget(title, conditions, fields, filters, sort, limit)
 
     def _new_filter(self, pattern=None, param=None):
         if param is None:
             param = "@logStream"
         return _Filter(pattern, param)
+
+    def _add_health_metrics_graph_widgets(self, cluster_health_metrics: Iterable[_HealthMetric]):
+        """Add cluster health metrics graph widgets."""
+        custom_namespace = "ParallelCluster"
+        widgets_list = []
+        for health_metric in cluster_health_metrics:
+            metric_list = []
+            for new_filter in health_metric.metric_filters:
+                self._add_custom_pcluster_metric_filter(
+                    metric_name=new_filter.metric_name,
+                    filter_pattern=new_filter.filter_pattern,
+                    custom_namespace=custom_namespace,
+                    metric_value=new_filter.metric_value,
+                    metric_unit=new_filter.metric_unit,
+                )
+                cloudwatch_metric = cloudwatch.Metric(
+                    namespace=custom_namespace,
+                    metric_name=new_filter.metric_name,
+                    period=Duration.minutes(1),
+                    statistic=new_filter.metric_statistic,
+                    dimensions_map={"ClusterName": self.config.cluster_name},
+                )
+                metric_list.append(cloudwatch_metric)
+            graph_widget = self._generate_graph_widget(
+                health_metric.title,
+                metric_list,
+                left_y_axis=health_metric.left_y_axis,
+                left_annotations=health_metric.left_annotations,
+            )
+            widgets_list.append(graph_widget)
+
+        self.cloudwatch_dashboard.add_widgets(*widgets_list)
+        self._update_coord_after_section(self.graph_height)
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/imagebuilder_stack.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/imagebuilder_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,14 +573,15 @@
     ):
         # ImageBuilderInfrastructureConfiguration
         infrastructure_configuration_resource = imagebuilder.CfnInfrastructureConfiguration(
             self,
             "InfrastructureConfiguration",
             name=self._build_resource_name(IMAGEBUILDER_RESOURCE_NAME_PREFIX),
             tags=build_tags,
+            resource_tags=build_tags,
             instance_profile_name=instance_profile_name or Fn.ref("InstanceProfile"),
             terminate_instance_on_failure=self.config.dev_settings.terminate_instance_on_failure
             if self.config.dev_settings and self.config.dev_settings.terminate_instance_on_failure is not None
             else True,
             instance_types=[self.config.build.instance_type],
             security_group_ids=self.config.build.security_group_ids,
             subnet_id=self.config.build.subnet_id,
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/import_cdk.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/import_cdk.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/templates/slurm_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/slurm_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,25 @@
         self,
         scope: Construct,
         id: str,
         stack_name: str,
         cluster_config: SlurmClusterConfig,
         bucket: S3Bucket,
         managed_head_node_instance_role: iam.CfnRole,
-        managed_compute_instance_roles: Dict[str, iam.CfnRole],
         cleanup_lambda_role: iam.CfnRole,
         cleanup_lambda: awslambda.CfnFunction,
     ):
         super().__init__(scope, id)
         self.stack_scope = scope
         self.stack_name = stack_name
         self.config = cluster_config
         self.bucket = bucket
         self.cleanup_lambda_role = cleanup_lambda_role
         self.cleanup_lambda = cleanup_lambda
         self.managed_head_node_instance_role = managed_head_node_instance_role
-        self.managed_compute_instance_roles = managed_compute_instance_roles
 
         self._add_parameters()
         self._add_resources()
 
     # -- Utility methods --------------------------------------------------------------------------------------------- #
 
     @property
@@ -97,26 +95,32 @@
 
     # -- Resources --------------------------------------------------------------------------------------------------- #
 
     def _add_resources(self):
         # DynamoDB to store cluster states
         self._add_dynamodb_table()
 
-        # Add Slurm Policies to new instances roles
         if self.managed_head_node_instance_role:
             self._add_policies_to_head_node_role("HeadNode", self.managed_head_node_instance_role.ref)
-        for queue_name, role in self.managed_compute_instance_roles.items():
-            if role:
-                self._add_policies_to_compute_node_role(queue_name, role.ref)
 
         self.cluster_hosted_zone = None
         if not self._condition_disable_cluster_dns():
             self.cluster_hosted_zone = self._add_private_hosted_zone()
 
-    def _add_policies_to_compute_node_role(self, node_name, role):
+    def register_policies_with_role(self, scope, managed_compute_instance_roles: Dict[str, iam.CfnRole]):
+        """
+        Associate the Slurm Policies to the compute node roles.
+
+        The Slurm Policies specify permissions for accessing Route53 and DynamoDB resources.
+        """
+        for queue_name, role in managed_compute_instance_roles.items():
+            if role:
+                self._add_policies_to_compute_node_role(scope, queue_name, role.ref)
+
+    def _add_policies_to_compute_node_role(self, scope, node_name, role):
         suffix = create_hash_suffix(node_name)
         _, policy_name = add_cluster_iam_resource_prefix(
             self.config.cluster_name, self.config, "parallelcluster-slurm-compute", iam_type="AWS::IAM::Policy"
         )
         policy_statements = [
             {
                 "sid": "SlurmDynamoDBTableQuery",
@@ -131,15 +135,15 @@
                         resource=f"table/{PCLUSTER_SLURM_DYNAMODB_PREFIX}{self.stack_name}/index/*",
                     ),
                 ],
             },
         ]
 
         iam.CfnPolicy(
-            self.stack_scope,
+            scope,
             f"SlurmPolicies{suffix}",
             policy_name=policy_name or "parallelcluster-slurm-compute",
             policy_document=iam.PolicyDocument(
                 statements=[iam.PolicyStatement(**statement) for statement in policy_statements]
             ),
             roles=[role],
         )
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 # the License. A copy of the License is located at
 #
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
+import asyncio
 import datetime
+import functools
 import itertools
 import json
 import logging
 import os
 import random
 import re
 import string
 import sys
 import time
 import zipfile
+from concurrent.futures import ThreadPoolExecutor
 from io import BytesIO
 from shlex import quote
-from typing import NoReturn
+from typing import Callable, NoReturn
 from urllib.parse import urlparse
 
 import dateutil.parser
 import pkg_resources
 import yaml
 from yaml import SafeLoader
 from yaml.constructor import ConstructorError
@@ -404,7 +407,132 @@
     """Get http tokens settings for supported IMDS version."""
     return "required" if imds_support == "v2.0" else "optional"
 
 
 def remove_none_values(original_dictionary):
     """Return a dictionary without entries with None value."""
     return {key: value for key, value in original_dictionary.items() if value is not None}
+
+
+def batch_by_property_callback(items, property_callback: Callable[..., int], batch_size):
+    """
+    Group a list of items into batches based on a property of each item and the specified `batch_size`.
+
+    The property of each item is obtained using the property_callback function. This way the caller of
+    `batch_by_property_size` defines which property to use for each item.
+    Example: (With batch_size of 2 and property_callback=lambda item: len(item.property))
+        [
+            Item(property=["test-1", "test-2"]),
+            Item(property=["test-3"]),
+            Item(property=["test-4"]),
+        ] --> [ [Item(property=["test-1", "test-2"])], [Item(property=["test-3"]), Item(property=["test-4"])] ]
+    :param items: list of items to organize into batches
+    :param property_callback: a callback function that returns the property(size) to use for batching
+    :param batch_size: maximum size of each batch
+    :return: batches of items as a list
+    """
+    # Avoid batching if total property count is already less than or equal to the batch_size
+    if sum(property_callback(item) for item in items) < batch_size:
+        yield items
+        return
+
+    batch_total_property_value, current_batch = 0, []
+    for item_index, item in enumerate(items):
+        property_value = property_callback(item)
+        if property_callback(item) > batch_size:
+            raise ValueError(
+                f"{item.__class__} property callback value of {property_value} is larger than "
+                f"the batch size ({batch_size}))"
+            )
+
+        if batch_total_property_value + property_value > batch_size:
+            yield current_batch
+            batch_total_property_value, current_batch = property_value, [item]
+        else:
+            batch_total_property_value += property_value
+            current_batch.append(item)
+        if item_index == len(items) - 1:
+            # If on the last time, yield the batch
+            yield current_batch
+
+
+class AsyncUtils:
+    """Utility class for async functions."""
+
+    @staticmethod
+    def async_retry(stop_max_attempt_number=5, wait_fixed=1, retry_on_exception=None):
+        """
+        Decorate an async coroutine function to retry its execution when an exception is risen.
+
+        :param stop_max_attempt_number: Max number of retries.
+        :param wait_fixed: Wait time (in seconds) between retries.
+        :param retry_on_exception: Exception to retry on.
+        :return:
+        """
+        if retry_on_exception is None:
+            retry_on_exception = (Exception,)
+
+        def decorator(func):
+            @functools.wraps(func)
+            async def wrapper(*args, **kwargs):
+                attempt = 0
+                result = None
+                while attempt <= stop_max_attempt_number:
+                    try:
+                        result = await func(*args, **kwargs)
+                        break
+                    except retry_on_exception as err:
+                        if attempt < stop_max_attempt_number:
+                            attempt += 1
+                            await asyncio.sleep(wait_fixed)
+                        else:
+                            raise err
+                return result
+
+            return wrapper
+
+        return decorator
+
+    @staticmethod
+    def async_timeout_cache(timeout=10):
+        """
+        Decorate a function to cache the result of a call for a given time period.
+
+        :param timeout: Timeout in seconds.
+        :return:
+        """
+
+        def decorator(func):
+            _cache = {}
+
+            @functools.wraps(func)
+            async def wrapper(*args, **kwargs):
+                cache_key = (func.__name__, args[1:], frozenset(kwargs.items()))
+                current_time = time.time()
+
+                if cache_key not in _cache or (_cache[cache_key][1] < current_time):
+                    _cache[cache_key] = (asyncio.ensure_future(func(*args, **kwargs)), current_time + timeout)
+
+                return await _cache[cache_key][0]
+
+            return wrapper
+
+        return decorator
+
+    _thread_pool_executor: ThreadPoolExecutor = ThreadPoolExecutor()
+
+    @staticmethod
+    def async_from_sync(func):
+        """
+        Convert a synchronous function to an async one.
+
+        :param func:
+        :return:
+        """
+
+        @functools.wraps(func)
+        async def wrapper(self, *args, **kwargs):
+            return await asyncio.get_event_loop().run_in_executor(
+                AsyncUtils._thread_pool_executor, lambda: func(self, *args, **kwargs)
+            )
+
+        return wrapper
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/awsbatch_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/awsbatch_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/cluster_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/cluster_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 import math
 import re
 from collections import defaultdict
 from enum import Enum
-from ipaddress import ip_network
+from ipaddress import collapse_addresses, ip_network
 from itertools import combinations, product
 from typing import List
 
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.aws_resources import InstanceTypeInfo
 from pcluster.aws.common import AWSClientError
 from pcluster.cli.commands.dcv_util import get_supported_dcv_os
 from pcluster.constants import (
     CIDR_ALL_IPS,
     DELETE_POLICY,
+    EFS_PORT,
     FSX_PORTS,
     PCLUSTER_IMAGE_BUILD_STATUS_TAG,
     PCLUSTER_NAME_MAX_LENGTH,
     PCLUSTER_NAME_MAX_LENGTH_SLURM_ACCOUNTING,
     PCLUSTER_NAME_REGEX,
     PCLUSTER_TAG_VALUE_REGEX,
     PCLUSTER_VERSION_TAG,
@@ -56,15 +57,15 @@
     "errors": {
         "ignored_param_with_efs_fs_id": "{efs_param} cannot be specified when an existing EFS file system is used.",
     }
 }
 
 FSX_SUPPORTED_ARCHITECTURES_OSES = {
     "x86_64": SUPPORTED_OSES,
-    "arm64": ["ubuntu1804", "ubuntu2004", "alinux2", "centos7"],
+    "arm64": SUPPORTED_OSES,
 }
 
 FSX_MESSAGES = {
     "errors": {
         "unsupported_os": "On {architecture} instance types, FSx Lustre can be used with one of the following operating"
         " systems: {supported_oses}. Please double check the os configuration.",
         "unsupported_architecture": "FSx Lustre can be used only with instance types and AMIs that support these "
@@ -166,16 +167,16 @@
                     f" change your ParallelCluster to {tags_dict[PCLUSTER_VERSION_TAG]}"
                 ),
                 FailureLevel.ERROR,
             )
         elif PCLUSTER_IMAGE_BUILD_STATUS_TAG not in tags_dict:
             self._add_failure(
                 (
-                    "The custom AMI did not pass the tests in image builder. "
-                    "Cluster created from this AMI may have unexpected behaviors."
+                    "Unable to retrieve custom AMI build status. "
+                    "Please check build-image CloudFormation stack for details."
                 ),
                 FailureLevel.ERROR,
             )
 
 
 class ComputeResourceSizeValidator(Validator):
     """
@@ -413,50 +414,95 @@
                 FailureLevel.ERROR,
             )
 
 
 # --------------- Storage validators --------------- #
 
 
-def _check_in_out_access(security_groups_ids, port, is_cidr_optional, protocol="tcp"):
+def _is_access_allowed(security_groups_ids, subnets, port, security_groups_by_nodes, protocol="tcp"):
     """
     Verify given list of security groups to check if they allow in and out access on the given port.
 
     :param security_groups_ids: list of security groups to verify
     :param port: port to verify
-    :param is_cidr_optional: if it is True, don't enforce check on CIDR.
+    :param security_groups_by_nodes: all security groups from cluster. This is a set of frozen sets.
+    Each frozen set contains sg combination of a queue.
     :param protocol: the IP protocol to be checked.
     :return: True if both in and out access are allowed
     :raise: ClientError if a given security group doesn't exist
     """
     in_access = False
     out_access = False
+    src_ip_ranges = []
+    dst_ip_ranges = []
+    src_security_groups = set()
+    dst_security_groups = set()
 
     for sec_group in AWSApi.instance().ec2.describe_security_groups(security_groups_ids):
         # Check all inbound rules
         for rule in sec_group.get("IpPermissions"):
-            if _check_sg_rules_for_port(rule, port, protocol):
-                if is_cidr_optional or rule.get("IpRanges") or rule.get("PrefixListIds"):
-                    in_access = True
-                    break
+            if in_access:
+                break
+            if _is_port_allowed_by_sg_rule(rule, port, protocol):
+                in_access = _populate_allowed_src_or_dst(rule, src_ip_ranges, src_security_groups)
 
         # Check all outbound rules
         for rule in sec_group.get("IpPermissionsEgress"):
-            if _check_sg_rules_for_port(rule, port, protocol):
-                if is_cidr_optional or rule.get("IpRanges") or rule.get("PrefixListIds"):
-                    out_access = True
-                    break
+            if out_access:
+                break
+            if _is_port_allowed_by_sg_rule(rule, port, protocol):
+                out_access = _populate_allowed_src_or_dst(rule, dst_ip_ranges, dst_security_groups)
 
         if in_access and out_access:
             return True
-
+    # If in_access or out_access is still False, check allowed ip ranges and security groups.
+    # The in_access or out_access could only have been true, if previous logics had found prefix list in SG rules.
+    # Rules of ip ranges have to be checked at the end because the union of all ip ranges may cover the subnets,
+    # even when individual ip ranges do not cover the subnets. The same reason applies to allowed security groups.
+    in_access = in_access or _are_ip_ranges_and_sg_accessible(
+        security_groups_by_nodes, src_ip_ranges, src_security_groups, subnets
+    )
+    out_access = out_access or _are_ip_ranges_and_sg_accessible(
+        security_groups_by_nodes, dst_ip_ranges, dst_security_groups, subnets
+    )
+    return in_access and out_access
+
+
+def _are_ip_ranges_and_sg_accessible(security_groups_by_nodes, allowed_ip_ranges, allowed_security_groups, subnets):
+    # For all cluster nodes, at least one of the security groups attached need to be in the UserIdGroupPairs.
+    return all(
+        node_security_groups & allowed_security_groups for node_security_groups in security_groups_by_nodes
+    ) or _are_subnets_covered_by_cidrs(allowed_ip_ranges, subnets)
+
+
+def _populate_allowed_src_or_dst(rule, ip_ranges, allowed_security_groups):
+    """
+    Collect Ip ranges or security groups allowed by the rule.
+
+    :param rule: A rule of a security group
+    :param ip_ranges: A list of ip ranges.
+    :param allowed_security_groups: A list of allowed security group.
+    :return: True if we can determine the current rule allows connection.
+    False if it does not allow connection or cannot be determined.
+    """
+    if rule.get("PrefixListIds"):
+        return True  # Always assume prefix list is properly set for code simplicity
+    elif rule.get("IpRanges"):
+        ip_ranges.extend(rule.get("IpRanges"))
+        return False  # Ip Ranges have to be checked later. Return False because the rule allowance is not determined.
+    elif rule.get("UserIdGroupPairs"):
+        allowed_security_groups.update(
+            {user_id_group_pair.get("GroupId") for user_id_group_pair in rule.get("UserIdGroupPairs")}
+        )
+        # Security groups have to be checked later. Return False because the rule allowance is not determined.
+        return False
     return False
 
 
-def _check_sg_rules_for_port(rule, port_to_check, protocol):
+def _is_port_allowed_by_sg_rule(rule, port_to_check, protocol):
     """
     Verify if the security group rule accepts connections on the given port.
 
     :param rule: The rule to check
     :param port_to_check: The port to check
     :param protocol: the IP protocol to be checked.
     :return: True if the rule accepts connection, False otherwise
@@ -479,14 +525,31 @@
 
     if (ip_protocol in expected_protocol) and (from_port <= port_to_check <= to_port):
         return True
 
     return False
 
 
+def _are_subnets_covered_by_cidrs(ip_ranges, subnets):
+    """Verify given list of security groups to check if they allow in and out access on cluster subnet CIDRs."""
+    # Collapse ip ranges for better performance and correctness
+    collapsed_ip_ranges = list(collapse_addresses([ip_network(ip_range["CidrIp"]) for ip_range in ip_ranges]))
+
+    for subnet in subnets:
+        subnet_cidr = ip_network(AWSApi.instance().ec2.get_subnet_cidr(subnet))
+        covered = False
+        for ip_range in collapsed_ip_ranges:
+            if ip_range.supernet_of(subnet_cidr):
+                covered = True
+                break
+        if not covered:
+            return False
+    return True
+
+
 class ExistingFsxNetworkingValidator(Validator):
     """
     FSx networking validator.
 
     Validate file system mount point according to the head node subnet.
     The reason to have this structure is to make boto3 calls as few as possible.
     """
@@ -500,35 +563,31 @@
             network_interfaces_data = {}
             for network_interface in response:
                 network_interfaces_data[network_interface["NetworkInterfaceId"]] = network_interface
             return network_interfaces_data
         else:
             return {}
 
-    def _validate(self, file_system_ids, head_node_subnet_id, are_all_security_groups_customized):
+    def _validate(self, file_system_ids, subnet_ids, security_groups_by_nodes):
         try:
-            # Check to see if there is any existing mt on the fs
             file_systems = AWSApi.instance().fsx.get_file_systems_info(file_system_ids)
-
-            vpc_id = AWSApi.instance().ec2.get_subnet_vpc(head_node_subnet_id)
-
-            network_interfaces_data = self._describe_network_interfaces(file_systems)
-
-            self._check_file_systems(are_all_security_groups_customized, file_systems, network_interfaces_data, vpc_id)
+            self._check_file_systems(security_groups_by_nodes, file_systems, subnet_ids)
         except AWSClientError as e:
             self._add_failure(str(e), FailureLevel.ERROR)
 
-    def _check_file_systems(self, are_all_security_groups_customized, file_systems, network_interfaces_data, vpc_id):
+    def _check_file_systems(self, security_groups_by_nodes, file_systems, subnet_ids):
+        vpc_id = AWSApi.instance().ec2.get_subnet_vpc(subnet_ids[0])
+        network_interfaces_data = self._describe_network_interfaces(file_systems)
         for file_system in file_systems:
             # Check to see if fs is in the same VPC as the stack
             file_system_id = file_system.file_system_id
             if file_system.vpc_id != vpc_id:
                 self._add_failure(
                     "Currently only support using FSx file system that is in the same VPC as the cluster. "
-                    "The file system provided is in {0}.".format(file_system.vpc_id),
+                    f"The file system {file_system_id} is in {file_system.vpc_id}.",
                     FailureLevel.ERROR,
                 )
 
             # If there is an existing mt in the az, check the inbound and outbound rules of the security groups
             network_interface_ids = file_system.network_interface_ids
             if not network_interface_ids:
                 self._add_failure(
@@ -541,37 +600,38 @@
                 for network_interface_id in network_interface_ids:
                     network_interface_responses.append(network_interfaces_data[network_interface_id])
 
                 network_interfaces = [ni for ni in network_interface_responses if ni.get("VpcId") == vpc_id]
 
                 for protocol, ports in FSX_PORTS[file_system.file_system_type].items():
                     missing_ports = self._get_missing_ports(
-                        are_all_security_groups_customized, network_interfaces, ports, protocol
+                        security_groups_by_nodes, subnet_ids, network_interfaces, ports, protocol
                     )
 
                     if missing_ports:
                         self._add_failure(
                             f"The current security group settings on file system '{file_system_id}' does not"
                             " satisfy mounting requirement. The file system must be associated to a security group"
                             f" that allows inbound and outbound {protocol.upper()} traffic through ports {ports}. "
                             f"Missing ports: {missing_ports}",
                             FailureLevel.ERROR,
                         )
 
-    def _get_missing_ports(self, are_all_security_groups_customized, network_interfaces, ports, protocol):
+    def _get_missing_ports(self, security_groups_by_nodes, subnet_ids, network_interfaces, ports, protocol):
         missing_ports = []
         for port in ports:
             fs_access = False
             for network_interface in network_interfaces:
                 # Get list of security group IDs
                 sg_ids = [sg.get("GroupId") for sg in network_interface.get("Groups")]
-                if _check_in_out_access(
+                if _is_access_allowed(
                     sg_ids,
+                    subnet_ids,
                     port=port,
-                    is_cidr_optional=are_all_security_groups_customized,
+                    security_groups_by_nodes=security_groups_by_nodes,
                     protocol=protocol,
                 ):
                     fs_access = True
                     break
             if not fs_access:
                 missing_ports.append(port)
         return missing_ports
@@ -739,15 +799,15 @@
 class EfsIdValidator(Validator):  # TODO add tests
     """
     EFS id validator.
 
     Validate if there are existing mount target in the cluster (head and computes) availability zone
     """
 
-    def _validate(self, efs_id, avail_zones_mapping: dict, are_all_security_groups_customized):
+    def _validate(self, efs_id, avail_zones_mapping: dict, security_groups_by_nodes):
         availability_zones = avail_zones_mapping.keys()
         if len(availability_zones) > 1 and not AWSApi.instance().efs.is_efs_standard(efs_id):
             self._add_failure(
                 f"Cluster has subnets located in different availability zones but EFS ({efs_id}) uses OneZone EFS "
                 "storage class which works within a single Availability Zone. Please use subnets located in one "
                 "Availability Zone or use a standard storage class EFS.",
                 FailureLevel.ERROR,
@@ -756,73 +816,37 @@
         avail_zones_missing_mount_target_for_efs_standard = []
         for avail_zone, subnets in avail_zones_mapping.items():
             head_node_target_id = AWSApi.instance().efs.get_efs_mount_target_id(efs_id, avail_zone)
             # If there is an existing mt in the az, need to check the inbound and outbound rules of the security groups
             if head_node_target_id:
                 # Get list of security group IDs of the mount target
                 sg_ids = AWSApi.instance().efs.get_efs_mount_target_security_groups(head_node_target_id)
-                if not _check_in_out_access(sg_ids, port=2049, is_cidr_optional=are_all_security_groups_customized):
+                if not _is_access_allowed(
+                    sg_ids, subnets, port=EFS_PORT, security_groups_by_nodes=security_groups_by_nodes
+                ):
                     self._add_failure(
                         "There is an existing Mount Target {0} in the Availability Zone {1} for EFS {2}, "
                         "but it does not have a security group that allows inbound and outbound rules to support NFS. "
                         "Please modify the Mount Target's security group, to allow traffic on port 2049.".format(
                             head_node_target_id, avail_zone, efs_id
                         ),
                         FailureLevel.ERROR,
                     )
-                if not are_all_security_groups_customized:
-                    self._check_cidrs_cover_subnets(head_node_target_id, avail_zone, sg_ids, efs_id, subnets)
             else:
                 if AWSApi.instance().efs.is_efs_standard(efs_id):
                     avail_zones_missing_mount_target_for_efs_standard.append(avail_zone)
         if avail_zones_missing_mount_target_for_efs_standard:
             self._add_failure(
                 "There is no existing Mount Target for EFS '{0}' in these Availability Zones: '{1}'. "
                 "Please create an EFS Mount Target for those availability zones.".format(
                     efs_id, avail_zones_missing_mount_target_for_efs_standard
                 ),
                 FailureLevel.ERROR,
             )
 
-    def _check_subnet_access(self, security_groups_ids, subnet_cidr, access_type):
-        permission = "IpPermissions" if access_type == "in" else "IpPermissionsEgress"
-        access = False
-        for sec_group in security_groups_ids:
-            for rule in sec_group.get(permission):
-                if rule.get("PrefixListIds"):
-                    access = True
-                    break
-                if rule.get("IpRanges"):
-                    for ip_range in rule.get("IpRanges"):
-                        if ip_network(ip_range.get("CidrIp")).supernet_of(subnet_cidr):
-                            access = True
-                            break
-        return access
-
-    def _check_cidrs_cover_subnets(self, head_node_target_id, avail_zone, security_groups_ids, efs_id, subnets):
-        """Verify given list of security groups to check if they allow in and out access on cluster subnet CIDRs."""
-        security_groups_ids = AWSApi.instance().ec2.describe_security_groups(security_groups_ids)
-        for subnet in subnets:
-            subnet_cidr = ip_network(AWSApi.instance().ec2.get_subnet_cidr(subnet))
-            in_access, out_access = self._check_subnet_access(
-                security_groups_ids, subnet_cidr, "in"
-            ), self._check_subnet_access(security_groups_ids, subnet_cidr, "out")
-
-            if not in_access or not out_access:
-                self._add_failure(
-                    "There is an existing Mount Target {0} in the Availability Zone {1} for EFS {2}, "
-                    "but it does not have a security group that allows inbound and outbound rules to allow traffic of "
-                    "subnet {3}. Please modify the Mount Target's security group, to allow traffic on subnet.".format(
-                        head_node_target_id, avail_zone, efs_id, subnet
-                    ),
-                    FailureLevel.WARNING,
-                )
-
-        return False
-
 
 class SharedStorageNameValidator(Validator):
     """
     Shared storage name validator.
 
     Validate if the provided name for the shared storage complies with the acceptable pattern.
     Since the storage name is used as a tag, the provided name must comply with the tag pattern.
@@ -1380,7 +1404,63 @@
             "CapacityReservationTarget": remove_none_values(
                 {
                     "CapacityReservationId": cr_target.capacity_reservation_id,
                     "CapacityReservationResourceGroupArn": cr_target.capacity_reservation_resource_group_arn,
                 }
             )
         }
+
+
+class RootVolumeEncryptionConsistencyValidator(Validator):
+    """Verify consistency on the Encryption parameter of all the specified RootVolumes of the queues."""
+
+    def _validate(self, encryption_settings: list):
+        reference_queue_name, reference_root_volume_encryption = encryption_settings.pop(0)
+        for queue in encryption_settings:
+            queue_name, root_volume_encryption = queue
+            if reference_root_volume_encryption != root_volume_encryption:
+                self._add_failure(
+                    f"The Encryption parameter of the root volume of the queue {queue_name} is not consistent "
+                    f"with the value set for the queue {reference_queue_name}, and may cause a problem in case "
+                    f"of Service Control Policies (SCPs) enforcing encryption.",
+                    FailureLevel.WARNING,
+                )
+
+
+class MultiNetworkInterfacesInstancesValidator(Validator):
+    """Verify that queues with multi nic compute resources don't auto-assign public IPs or contain subnets that do."""
+
+    def _validate(self, queues):
+        multi_nic_queues = [
+            queue
+            for queue in queues
+            for compute_resource in queue.compute_resources
+            if compute_resource.max_network_interface_count > 1
+        ]
+
+        all_subnets_with_public_ips = {
+            subnet.get("SubnetId")
+            for subnet in AWSApi.instance().ec2.describe_subnets(
+                {subnet_id for queue in multi_nic_queues for subnet_id in queue.networking.subnet_ids}
+            )
+            if subnet.get("MapPublicIpOnLaunch")
+        }
+
+        for queue in multi_nic_queues:
+            if queue.networking.assign_public_ip:
+                self._add_failure(
+                    f"The queue {queue.name} contains an instance type with multiple network interfaces however the "
+                    f"AssignPublicIp value is set to true. AWS public IPs can only be assigned to instances launched "
+                    f"with a single network interface.",
+                    FailureLevel.ERROR,
+                )
+
+            queue_subnets_with_public_ips = sorted(
+                [subnet_id for subnet_id in queue.networking.subnet_ids if subnet_id in all_subnets_with_public_ips]
+            )
+            if queue_subnets_with_public_ips:
+                self._add_failure(
+                    f"The queue {queue.name} contains an instance type with multiple network interfaces however the "
+                    f"subnets {queue_subnets_with_public_ips} is configured to automatically assign public IPs. AWS "
+                    f"public IPs can only be assigned to instances launched with a single network interface.",
+                    FailureLevel.ERROR,
+                )
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/database_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/database_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/directory_service_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/directory_service_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 from urllib.parse import urlparse
 
-from aws_cdk.core import Arn
+from aws_cdk.core import Arn, ArnFormat
 
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.common import AWSClientError
 from pcluster.constants import DIRECTORY_SERVICE_RESERVED_SETTINGS
 from pcluster.validators.common import FailureLevel, Validator
 
 
@@ -80,15 +80,15 @@
 
         In particular, the ARN should be one of the following resources:
          1. a readable secret in AWS Secrets Manager, which is supported in all regions but us-isob-east-1.
          2. a readable parameter in SSM Parameter Store, which is supported only in us-isob-east-1.
         """
         try:
             # We only require the secret to exist; we do not validate its content.
-            arn_components = Arn.parse(password_secret_arn)
+            arn_components = Arn.split(password_secret_arn, ArnFormat.COLON_RESOURCE_NAME)
             service, resource = arn_components.service, arn_components.resource
             if service == "secretsmanager" and resource == "secret" and region != "us-isob-east-1":
                 AWSApi.instance().secretsmanager.describe_secret(password_secret_arn)
             elif service == "ssm" and resource == "parameter" and region == "us-isob-east-1":
                 parameter_name = arn_components.resource_name
                 AWSApi.instance().ssm.get_parameter(parameter_name)
             else:
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/ebs_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/ebs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/ec2_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/ec2_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/efs_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/efs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/feature_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/feature_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/fsx_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/fsx_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/iam_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/iam_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/imagebuilder_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/imagebuilder_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/instances_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/instances_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/kms_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/kms_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/networking_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/networking_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/s3_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/s3_validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 import re
-import time
 from urllib.error import HTTPError, URLError
 from urllib.request import urlopen
 
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.common import AWSClientError
-from pcluster.utils import get_url_scheme
-from pcluster.validators.common import FailureLevel, Validator
+from pcluster.utils import AsyncUtils, get_url_scheme
+from pcluster.validators.common import AsyncValidator, FailureLevel, Validator
 from pcluster.validators.utils import get_bucket_name_from_s3_url
 
 
-class UrlValidator(Validator):
+class UrlValidator(AsyncValidator):
     """
     Url Validator.
 
     Validate given url with s3 or https prefix.
+    Validation is cached across instances to avoid repeated calls to the same urls.
     """
 
-    def _validate(
+    @AsyncUtils.async_timeout_cache(timeout=10)
+    async def _validate_async(
+        self,
+        url,
+        fail_on_https_error: bool = False,
+        fail_on_s3_error: bool = False,
+        expected_bucket_owner: str = None,
+    ):
+        try:
+            await self._validate_async_internal(
+                url,
+                fail_on_https_error=fail_on_https_error,
+                fail_on_s3_error=fail_on_s3_error,
+                expected_bucket_owner=expected_bucket_owner,
+            )
+        except ConnectionError as err:
+            self._add_failure(f"The url '{url}' causes ConnectionError: {err}.", FailureLevel.WARNING)
+
+    @AsyncUtils.async_retry(stop_max_attempt_number=3, wait_fixed=1, retry_on_exception=ConnectionError)
+    async def _validate_async_internal(
         self,
         url,
-        retries=3,
         fail_on_https_error: bool = False,
         fail_on_s3_error: bool = False,
         expected_bucket_owner: str = None,
     ):
         scheme = get_url_scheme(url)
         if scheme in ["https", "s3"]:
-            try:
-                if scheme == "s3":
-                    self._validate_s3_uri(
-                        url, fail_on_error=fail_on_s3_error, expected_bucket_owner=expected_bucket_owner
-                    )
-                else:
-                    if expected_bucket_owner:
-                        self._add_failure("S3BucketOwner can only be specified with S3 URL", FailureLevel.ERROR)
-                    self._validate_https_uri(url, fail_on_error=fail_on_https_error)
-            except ConnectionError as e:
-                if retries > 0:
-                    time.sleep(5)
-                    self._validate(url, retries=retries - 1)
-                else:
-                    self._add_failure(f"The url '{url}' causes ConnectionError: {e}.", FailureLevel.WARNING)
+            if scheme == "s3":
+                _async_validate_s3_uri = AsyncUtils.async_from_sync(self._validate_s3_uri)
+                await _async_validate_s3_uri(
+                    url, fail_on_error=fail_on_s3_error, expected_bucket_owner=expected_bucket_owner
+                )
+            else:
+                if expected_bucket_owner:
+                    self._add_failure("S3BucketOwner can only be specified with S3 URL", FailureLevel.ERROR)
+                _async_validate_https_uri = AsyncUtils.async_from_sync(self._validate_https_uri)
+                await _async_validate_https_uri(url, fail_on_error=fail_on_https_error)
 
         else:
             self._add_failure(
                 f"The value '{url}' is not a valid URL, choose URL with 'https' or 's3' prefix.",
                 FailureLevel.ERROR,
             )
```

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/scheduler_plugin_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/scheduler_plugin_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster/validators/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster3_config_converter/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.5.1/src/pcluster3_config_converter/pcluster3_config_converter.py` & `aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/pcluster3_config_converter.py`

 * *Files identical despite different names*

