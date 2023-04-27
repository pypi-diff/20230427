# Comparing `tmp/cockroachdb_cloud_client-0.1.1.tar.gz` & `tmp/cockroachdb_cloud_client-2022.9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cockroachdb_cloud_client-0.1.1.tar", max compression
+gzip compressed data, was "cockroachdb_cloud_client-2022.9.20.tar", max compression
```

## Comparing `cockroachdb_cloud_client-0.1.1.tar` & `cockroachdb_cloud_client-2022.9.20.tar`

### file list

```diff
@@ -1,206 +1,126 @@
--rw-r--r--   0        0        0    35149 2022-10-11 13:07:34.312971 cockroachdb_cloud_client-0.1.1/LICENSE
--rw-r--r--   0        0        0     1688 2022-11-22 12:37:40.364530 cockroachdb_cloud_client-0.1.1/README.md
--rw-r--r--   0        0        0      165 2023-04-27 16:45:02.986973 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/__init__.py
--rw-r--r--   0        0        0       47 2023-04-27 16:45:00.649181 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 16:45:00.664450 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/__init__.py
--rw-r--r--   0        0        0     5754 2023-04-27 16:45:03.175423 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_add_allowlist_entry.py
--rw-r--r--   0        0        0     7354 2023-04-27 16:45:03.189476 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_add_egress_rule.py
--rw-r--r--   0        0        0     7515 2023-04-27 16:45:03.204333 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_add_user_to_role.py
--rw-r--r--   0        0        0     5472 2023-04-27 16:45:03.196081 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_cluster.py
--rw-r--r--   0        0        0     5816 2023-04-27 16:45:03.207735 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_database.py
--rw-r--r--   0        0        0     5017 2023-04-27 16:45:03.189359 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_private_endpoint_services.py
--rw-r--r--   0        0        0     5892 2023-04-27 16:45:03.226181 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_sql_user.py
--rw-r--r--   0        0        0     5443 2023-04-27 16:45:03.230289 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_allowlist_entry.py
--rw-r--r--   0        0        0     4813 2023-04-27 16:45:03.223643 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_client_ca_cert.py
--rw-r--r--   0        0        0     5064 2023-04-27 16:45:03.236232 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_cloud_watch_metric_export.py
--rw-r--r--   0        0        0     4682 2023-04-27 16:45:03.237628 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_cluster.py
--rw-r--r--   0        0        0     4882 2023-04-27 16:45:03.243914 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_database.py
--rw-r--r--   0        0        0     5049 2023-04-27 16:45:03.252091 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_datadog_metric_export.py
--rw-r--r--   0        0        0     6080 2023-04-27 16:45:03.285415 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_egress_rule.py
--rw-r--r--   0        0        0     4916 2023-04-27 16:45:03.263867 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_log_export.py
--rw-r--r--   0        0        0     4870 2023-04-27 16:45:03.271402 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_sql_user.py
--rw-r--r--   0        0        0     6196 2023-04-27 16:45:03.311414 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_edit_database.py
--rw-r--r--   0        0        0     5955 2023-04-27 16:45:03.317707 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_edit_database_2.py
--rw-r--r--   0        0        0     7113 2023-04-27 16:45:03.315540 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_edit_egress_rule.py
--rw-r--r--   0        0        0     6950 2023-04-27 16:45:03.320888 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_enable_cloud_watch_metric_export.py
--rw-r--r--   0        0        0     6758 2023-04-27 16:45:03.326820 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_enable_cmek_spec.py
--rw-r--r--   0        0        0     6511 2023-04-27 16:45:03.329518 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_enable_datadog_metric_export.py
--rw-r--r--   0        0        0     6907 2023-04-27 16:45:03.352245 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_enable_log_export.py
--rw-r--r--   0        0        0     5547 2023-04-27 16:45:03.335719 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_all_roles_for_user.py
--rw-r--r--   0        0        0     4846 2023-04-27 16:45:03.345986 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_client_ca_cert.py
--rw-r--r--   0        0        0     5050 2023-04-27 16:45:03.344840 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_cloud_watch_metric_export_info.py
--rw-r--r--   0        0        0     4695 2023-04-27 16:45:03.358958 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_cluster.py
--rw-r--r--   0        0        0     4814 2023-04-27 16:45:03.360885 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_cmek_cluster_info.py
--rw-r--r--   0        0        0     7389 2023-04-27 16:45:03.420297 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_connection_string.py
--rw-r--r--   0        0        0     4995 2023-04-27 16:45:03.375843 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_datadog_metric_export_info.py
--rw-r--r--   0        0        0     5179 2023-04-27 16:45:03.388753 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_egress_rule.py
--rw-r--r--   0        0        0     4707 2023-04-27 16:45:03.398085 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_invoice.py
--rw-r--r--   0        0        0     4901 2023-04-27 16:45:03.421181 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_log_export_info.py
--rw-r--r--   0        0        0     4375 2023-04-27 16:45:03.421296 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_organization_info.py
--rw-r--r--   0        0        0     5041 2023-04-27 16:45:03.440540 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_person_users_by_email.py
--rw-r--r--   0        0        0     9589 2023-04-27 16:45:03.533884 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_allowlist_entries.py
--rw-r--r--   0        0        0    11141 2023-04-27 16:45:03.576675 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_available_regions.py
--rw-r--r--   0        0        0     4990 2023-04-27 16:45:03.433905 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_aws_endpoint_connections.py
--rw-r--r--   0        0        0    10001 2023-04-27 16:45:03.562027 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_cluster_nodes.py
--rw-r--r--   0        0        0     9589 2023-04-27 16:45:03.562625 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_clusters.py
--rw-r--r--   0        0        0     9336 2023-04-27 16:45:03.565787 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_databases.py
--rw-r--r--   0        0        0     9400 2023-04-27 16:45:03.564731 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_egress_rules.py
--rw-r--r--   0        0        0     4629 2023-04-27 16:45:03.466492 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_invoices.py
--rw-r--r--   0        0        0     9285 2023-04-27 16:45:03.562857 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_major_cluster_versions.py
--rw-r--r--   0        0        0     5564 2023-04-27 16:45:03.490885 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_private_endpoint_services.py
--rw-r--r--   0        0        0     9232 2023-04-27 16:45:03.596652 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_role_grants.py
--rw-r--r--   0        0        0     9197 2023-04-27 16:45:03.606683 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_sql_users.py
--rw-r--r--   0        0        0     7647 2023-04-27 16:45:03.571703 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_remove_user_from_role.py
--rw-r--r--   0        0        0     7581 2023-04-27 16:45:03.569893 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_set_aws_endpoint_connection_state.py
--rw-r--r--   0        0        0     6070 2023-04-27 16:45:03.557466 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_set_client_ca_cert.py
--rw-r--r--   0        0        0     6741 2023-04-27 16:45:03.574118 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_set_egress_traffic_policy.py
--rw-r--r--   0        0        0     6804 2023-04-27 16:45:03.579575 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_set_roles_for_user.py
--rw-r--r--   0        0        0     6149 2023-04-27 16:45:03.606702 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_client_ca_cert.py
--rw-r--r--   0        0        0     8564 2023-04-27 16:45:03.623616 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cluster.py
--rw-r--r--   0        0        0     6833 2023-04-27 16:45:03.640189 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cmek_spec.py
--rw-r--r--   0        0        0     5991 2023-04-27 16:45:03.674035 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cmek_status.py
--rw-r--r--   0        0        0     6277 2023-04-27 16:45:03.684854 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_sql_user_password.py
--rw-r--r--   0        0        0     2817 2023-04-27 16:45:03.625674 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/client.py
--rw-r--r--   0        0        0      470 2023-04-27 16:45:03.572854 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/errors.py
--rw-r--r--   0        0        0    15911 2023-04-27 16:45:01.931166 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/__init__.py
--rw-r--r--   0        0        0     2089 2023-04-27 16:45:03.627595 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/add_egress_rule_response.py
--rw-r--r--   0        0        0     2223 2023-04-27 16:45:03.646624 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/allowlist_entry.py
--rw-r--r--   0        0        0     5433 2023-04-27 16:45:03.621351 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/any_.py
--rw-r--r--   0        0        0     2957 2023-04-27 16:45:03.637232 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/aws_endpoint_connection.py
--rw-r--r--   0        0        0      356 2023-04-27 16:45:01.826539 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/aws_endpoint_connection_status_type.py
--rw-r--r--   0        0        0     2127 2023-04-27 16:45:03.634759 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/aws_endpoint_connections.py
--rw-r--r--   0        0        0     2413 2023-04-27 16:45:03.633326 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/aws_private_link_service_detail.py
--rw-r--r--   0        0        0     1857 2023-04-27 16:45:03.636541 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/built_in_role.py
--rw-r--r--   0        0        0     2747 2023-04-27 16:45:03.660462 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/client_ca_cert_info.py
--rw-r--r--   0        0        0      215 2023-04-27 16:45:02.084793 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/client_ca_cert_status.py
--rw-r--r--   0        0        0     2422 2023-04-27 16:45:03.669773 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cloud_provider_region.py
--rw-r--r--   0        0        0      154 2023-04-27 16:45:01.734296 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cloud_provider_type.py
--rw-r--r--   0        0        0     3623 2023-04-27 16:45:03.711416 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cloud_watch_metric_export_info.py
--rw-r--r--   0        0        0    11940 2023-04-27 16:45:03.846065 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster.py
--rw-r--r--   0        0        0     3021 2023-04-27 16:45:03.713944 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_config.py
--rw-r--r--   0        0        0     2037 2023-04-27 16:45:03.677493 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_major_version.py
--rw-r--r--   0        0        0      225 2023-04-27 16:45:01.821895 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_major_version_support_status_type.py
--rw-r--r--   0        0        0      257 2023-04-27 16:45:01.993182 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_state_type.py
--rw-r--r--   0        0        0     1630 2023-04-27 16:45:02.065857 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_status_type.py
--rw-r--r--   0        0        0      345 2023-04-27 16:45:01.943577 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_upgrade_status_type.py
--rw-r--r--   0        0        0     5102 2023-04-27 16:45:03.726870 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_cluster_info.py
--rw-r--r--   0        0        0      145 2023-04-27 16:45:01.751300 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_customer_action.py
--rw-r--r--   0        0        0     6828 2023-04-27 16:45:03.773892 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_key_info.py
--rw-r--r--   0        0        0     2957 2023-04-27 16:45:03.719884 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_key_specification.py
--rw-r--r--   0        0        0      238 2023-04-27 16:45:01.731925 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_key_type_enumerates_types_of_customer_managed_keys.py
--rw-r--r--   0        0        0     5326 2023-04-27 16:45:03.735125 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_region_info.py
--rw-r--r--   0        0        0     2778 2023-04-27 16:45:03.716024 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_region_specification.py
--rw-r--r--   0        0        0      441 2023-04-27 16:45:01.755824 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_status.py
--rw-r--r--   0        0        0     2037 2023-04-27 16:45:03.704531 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_add_allowlist_entry_2_allowlist_entry.py
--rw-r--r--   0        0        0     4204 2023-04-27 16:45:03.742077 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_add_egress_rule_add_egress_rule_request.py
--rw-r--r--   0        0        0      202 2023-04-27 16:45:02.041095 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_add_user_to_role_resource_type.py
--rw-r--r--   0        0        0      526 2023-04-27 16:45:02.110149 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_add_user_to_role_role_name.py
--rw-r--r--   0        0        0     1615 2023-04-27 16:45:03.702960 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_create_database_create_database_request.py
--rw-r--r--   0        0        0     1820 2023-04-27 16:45:03.723568 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_create_sql_user_create_sql_user_request.py
--rw-r--r--   0        0        0     1836 2023-04-27 16:45:03.730301 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_edit_database_2_update_database_request.py
--rw-r--r--   0        0        0     1686 2023-04-27 16:45:03.726123 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_edit_database_update_database_request.py
--rw-r--r--   0        0        0     4169 2023-04-27 16:45:03.785216 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_edit_egress_rule_edit_egress_rule_request.py
--rw-r--r--   0        0        0     2854 2023-04-27 16:45:03.752980 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_enable_cloud_watch_metric_export_enable_cloud_watch_metric_export_request.py
--rw-r--r--   0        0        0     2527 2023-04-27 16:45:03.757601 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_enable_cmek_spec_cmek_cluster_specification.py
--rw-r--r--   0        0        0     2054 2023-04-27 16:45:03.756233 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_enable_datadog_metric_export_enable_datadog_metric_export_request.py
--rw-r--r--   0        0        0     4808 2023-04-27 16:45:03.818309 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_enable_log_export_enable_log_export_request.py
--rw-r--r--   0        0        0      200 2023-04-27 16:45:01.868671 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_get_connection_string_os.py
--rw-r--r--   0        0        0      192 2023-04-27 16:45:01.899848 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_allowlist_entries_pagination_sort_order.py
--rw-r--r--   0        0        0      192 2023-04-27 16:45:02.053518 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_available_regions_pagination_sort_order.py
--rw-r--r--   0        0        0      179 2023-04-27 16:45:01.922938 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_available_regions_provider.py
--rw-r--r--   0        0        0      188 2023-04-27 16:45:01.902728 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_cluster_nodes_pagination_sort_order.py
--rw-r--r--   0        0        0      184 2023-04-27 16:45:01.968036 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_clusters_pagination_sort_order.py
--rw-r--r--   0        0        0      185 2023-04-27 16:45:02.030275 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_databases_pagination_sort_order.py
--rw-r--r--   0        0        0      187 2023-04-27 16:45:01.793476 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_egress_rules_pagination_sort_order.py
--rw-r--r--   0        0        0      196 2023-04-27 16:45:02.018464 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_major_cluster_versions_pagination_sort_order.py
--rw-r--r--   0        0        0      186 2023-04-27 16:45:01.933505 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_role_grants_pagination_sort_order.py
--rw-r--r--   0        0        0      184 2023-04-27 16:45:02.120434 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_list_sql_users_pagination_sort_order.py
--rw-r--r--   0        0        0      207 2023-04-27 16:45:01.919051 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_remove_user_from_role_resource_type.py
--rw-r--r--   0        0        0      531 2023-04-27 16:45:01.938130 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_remove_user_from_role_role_name.py
--rw-r--r--   0        0        0     2150 2023-04-27 16:45:03.775317 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_aws_endpoint_connection_state_set_aws_endpoint_connection_state_request.py
--rw-r--r--   0        0        0     1745 2023-04-27 16:45:03.772253 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_client_ca_cert_set_client_ca_cert_request.py
--rw-r--r--   0        0        0     1345 2023-04-27 16:45:03.766516 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_egress_traffic_policy_response_200.py
--rw-r--r--   0        0        0     2453 2023-04-27 16:45:03.779922 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_egress_traffic_policy_set_egress_traffic_policy_request.py
--rw-r--r--   0        0        0     2082 2023-04-27 16:45:03.784246 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_roles_for_user_json_body.py
--rw-r--r--   0        0        0     2044 2023-04-27 16:45:03.798854 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_allowlist_entry_allowlist_entry.py
--rw-r--r--   0        0        0     1871 2023-04-27 16:45:03.774369 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_client_ca_cert_update_client_ca_cert_request.py
--rw-r--r--   0        0        0     2527 2023-04-27 16:45:03.801358 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_spec_cmek_cluster_specification.py
--rw-r--r--   0        0        0     1885 2023-04-27 16:45:03.788448 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_status_update_cmek_status_request.py
--rw-r--r--   0        0        0     1740 2023-04-27 16:45:03.808830 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_sql_user_password_update_sql_user_password_request.py
--rw-r--r--   0        0        0     2541 2023-04-27 16:45:03.826195 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/create_cluster_request.py
--rw-r--r--   0        0        0     3293 2023-04-27 16:45:03.853940 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/create_cluster_specification.py
--rw-r--r--   0        0        0     2456 2023-04-27 16:45:03.838427 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/currency_amount.py
--rw-r--r--   0        0        0      179 2023-04-27 16:45:01.888877 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/currency_type.py
--rw-r--r--   0        0        0     1677 2023-04-27 16:45:03.834576 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/database.py
--rw-r--r--   0        0        0     3078 2023-04-27 16:45:03.872507 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/datadog_metric_export_info.py
--rw-r--r--   0        0        0      208 2023-04-27 16:45:01.940484 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/datadog_site_type.py
--rw-r--r--   0        0        0     4772 2023-04-27 16:45:03.869865 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_cluster_create_specification.py
--rw-r--r--   0        0        0     1524 2023-04-27 16:45:03.826475 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_cluster_create_specification_region_nodes.py
--rw-r--r--   0        0        0     5068 2023-04-27 16:45:03.899212 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_cluster_update_specification.py
--rw-r--r--   0        0        0     1524 2023-04-27 16:45:03.835423 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_cluster_update_specification_region_nodes.py
--rw-r--r--   0        0        0     2862 2023-04-27 16:45:03.858682 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_hardware_config.py
--rw-r--r--   0        0        0     2819 2023-04-27 16:45:03.864559 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_hardware_create_specification.py
--rw-r--r--   0        0        0     3255 2023-04-27 16:45:03.882497 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_hardware_update_specification.py
--rw-r--r--   0        0        0     2241 2023-04-27 16:45:03.854724 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_machine_type_specification.py
--rw-r--r--   0        0        0     2101 2023-04-27 16:45:03.873628 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/delete_egress_rule_response.py
--rw-r--r--   0        0        0     2229 2023-04-27 16:45:03.882629 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/delete_metric_export_response.py
--rw-r--r--   0        0        0     2094 2023-04-27 16:45:03.888035 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/edit_egress_rule_response.py
--rw-r--r--   0        0        0     4973 2023-04-27 16:45:03.968932 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/egress_rule.py
--rw-r--r--   0        0        0      268 2023-04-27 16:45:02.125849 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/egress_traffic_policy_type.py
--rw-r--r--   0        0        0     2408 2023-04-27 16:45:03.904372 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_all_roles_for_user_response_contains_a_representation_of_all_roles_a_given_user_has.py
--rw-r--r--   0        0        0     2809 2023-04-27 16:45:03.909598 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_connection_string_response.py
--rw-r--r--   0        0        0     1363 2023-04-27 16:45:03.878055 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_connection_string_response_params.py
--rw-r--r--   0        0        0     1711 2023-04-27 16:45:03.895298 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_egress_rule_response.py
--rw-r--r--   0        0        0     2352 2023-04-27 16:45:03.926423 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_person_users_by_email_response.py
--rw-r--r--   0        0        0     5820 2023-04-27 16:45:03.974825 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/invoice.py
--rw-r--r--   0        0        0     1791 2023-04-27 16:45:03.912660 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/invoice_adjustment.py
--rw-r--r--   0        0        0     3690 2023-04-27 16:45:03.968910 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/invoice_item.py
--rw-r--r--   0        0        0     3305 2023-04-27 16:45:03.968985 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/keyset_pagination_request.py
--rw-r--r--   0        0        0     1886 2023-04-27 16:45:03.928504 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/keyset_pagination_response.py
--rw-r--r--   0        0        0     2664 2023-04-27 16:45:03.968924 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/line_item.py
--rw-r--r--   0        0        0     3173 2023-04-27 16:45:03.968944 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_allowlist_entries_response.py
--rw-r--r--   0        0        0     2952 2023-04-27 16:45:03.968964 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_available_regions_response.py
--rw-r--r--   0        0        0     2779 2023-04-27 16:45:03.968955 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_cluster_nodes_response.py
--rw-r--r--   0        0        0     2843 2023-04-27 16:45:03.968964 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_clusters_response.py
--rw-r--r--   0        0        0     2877 2023-04-27 16:45:03.985014 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_databases_response.py
--rw-r--r--   0        0        0     3144 2023-04-27 16:45:03.985396 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_egress_rules_response.py
--rw-r--r--   0        0        0     1947 2023-04-27 16:45:03.968917 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_invoices_response.py
--rw-r--r--   0        0        0     2997 2023-04-27 16:45:04.002729 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_major_cluster_versions_response.py
--rw-r--r--   0        0        0     3224 2023-04-27 16:45:04.017818 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_role_grants_response_contains_a_representation_of_all_roles.py
--rw-r--r--   0        0        0     2782 2023-04-27 16:45:04.014337 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_sql_users_response.py
--rw-r--r--   0        0        0     5516 2023-04-27 16:45:04.078680 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/log_export_cluster_info.py
--rw-r--r--   0        0        0     5293 2023-04-27 16:45:04.083026 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/log_export_cluster_specification.py
--rw-r--r--   0        0        0     3805 2023-04-27 16:45:04.059125 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/log_export_group.py
--rw-r--r--   0        0        0      298 2023-04-27 16:45:01.957507 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/log_export_status.py
--rw-r--r--   0        0        0      200 2023-04-27 16:45:02.020983 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/log_export_type.py
--rw-r--r--   0        0        0      213 2023-04-27 16:45:02.105796 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/log_level_type.py
--rw-r--r--   0        0        0      259 2023-04-27 16:45:01.831213 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/metric_export_status_type.py
--rw-r--r--   0        0        0      172 2023-04-27 16:45:02.010044 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/network_visibility_type.py
--rw-r--r--   0        0        0     1788 2023-04-27 16:45:04.053095 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/node.py
--rw-r--r--   0        0        0      165 2023-04-27 16:45:01.774290 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/node_status_type.py
--rw-r--r--   0        0        0      184 2023-04-27 16:45:01.857933 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/operating_system_type.py
--rw-r--r--   0        0        0     1936 2023-04-27 16:45:04.034325 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/organization.py
--rw-r--r--   0        0        0      515 2023-04-27 16:45:01.783108 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/organization_user_role_type.py
--rw-r--r--   0        0        0     1843 2023-04-27 16:45:04.028101 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/person_user_info_contains_information_about_a_person.py
--rw-r--r--   0        0        0      193 2023-04-27 16:45:01.985102 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/plan_type.py
--rw-r--r--   0        0        0     2805 2023-04-27 16:45:04.057860 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/private_endpoint_service.py
--rw-r--r--   0        0        0      289 2023-04-27 16:45:01.787407 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/private_endpoint_service_status_type.py
--rw-r--r--   0        0        0     2087 2023-04-27 16:45:04.048219 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/private_endpoint_services.py
--rw-r--r--   0        0        0      177 2023-04-27 16:45:01.859806 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/quantity_unit_type.py
--rw-r--r--   0        0        0     2890 2023-04-27 16:45:04.066337 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/region.py
--rw-r--r--   0        0        0     1686 2023-04-27 16:45:04.065192 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/resource.py
--rw-r--r--   0        0        0      179 2023-04-27 16:45:01.864048 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/resource_type_type.py
--rw-r--r--   0        0        0     2938 2023-04-27 16:45:04.072873 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/serverless_cluster_config.py
--rw-r--r--   0        0        0     3685 2023-04-27 16:45:04.080820 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/serverless_cluster_create_specification.py
--rw-r--r--   0        0        0     2702 2023-04-27 16:45:04.076099 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/serverless_cluster_update_specification.py
--rw-r--r--   0        0        0      193 2023-04-27 16:45:01.775948 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/set_aws_endpoint_connection_status_type.py
--rw-r--r--   0        0        0      148 2023-04-27 16:45:01.753655 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/sort_order.py
--rw-r--r--   0        0        0     1334 2023-04-27 16:45:04.065162 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/sql_user.py
--rw-r--r--   0        0        0     2520 2023-04-27 16:45:04.088444 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/status.py
--rw-r--r--   0        0        0     5726 2023-04-27 16:45:04.105392 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/update_cluster_specification.py
--rw-r--r--   0        0        0     2509 2023-04-27 16:45:04.078072 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/usage_limits.py
--rw-r--r--   0        0        0     2125 2023-04-27 16:45:04.087066 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/user_role_grants.py
--rw-r--r--   0        0        0       25 2023-04-27 16:45:00.466480 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/py.typed
--rw-r--r--   0        0        0      974 2023-04-27 16:45:04.073520 cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/types.py
--rw-r--r--   0        0        0      964 2023-04-27 16:44:56.134007 cockroachdb_cloud_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 cockroachdb_cloud_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-11 13:07:34.312971 cockroachdb_cloud_client-2022.9.20/LICENSE
+-rw-r--r--   0        0        0     3717 2022-10-11 13:19:07.741689 cockroachdb_cloud_client-2022.9.20/README.md
+-rw-r--r--   0        0        0      109 2022-10-11 13:22:53.342325 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-10-11 13:22:53.498619 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-11 13:22:53.518688 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/__init__.py
+-rw-r--r--   0        0        0     4443 2022-10-11 13:22:55.644368 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_add_allowlist_entry.py
+-rw-r--r--   0        0        0     4161 2022-10-11 13:22:55.652948 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_cluster.py
+-rw-r--r--   0        0        0     4505 2022-10-11 13:22:55.657741 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_database.py
+-rw-r--r--   0        0        0     4674 2022-10-11 13:22:55.681957 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_private_endpoint_services.py
+-rw-r--r--   0        0        0     4581 2022-10-11 13:22:55.689701 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_sql_user.py
+-rw-r--r--   0        0        0     4132 2022-10-11 13:22:55.732937 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_allowlist_entry.py
+-rw-r--r--   0        0        0     3371 2022-10-11 13:22:55.761214 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_cluster.py
+-rw-r--r--   0        0        0     3571 2022-10-11 13:22:55.756898 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_database.py
+-rw-r--r--   0        0        0     3401 2022-10-11 13:22:55.757044 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_log_export.py
+-rw-r--r--   0        0        0     3559 2022-10-11 13:22:55.770192 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_sql_user.py
+-rw-r--r--   0        0        0     4500 2022-10-11 13:22:55.766698 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_edit_database.py
+-rw-r--r--   0        0        0     5439 2022-10-11 13:22:55.762812 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_enable_cmek_spec.py
+-rw-r--r--   0        0        0     4368 2022-10-11 13:22:55.771969 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_enable_log_export.py
+-rw-r--r--   0        0        0     3384 2022-10-11 13:22:55.756239 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_cluster.py
+-rw-r--r--   0        0        0     3503 2022-10-11 13:22:55.778677 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_cmek_cluster_info.py
+-rw-r--r--   0        0        0     3396 2022-10-11 13:22:55.762864 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_invoice.py
+-rw-r--r--   0        0        0     3398 2022-10-11 13:22:55.744959 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_log_export_info.py
+-rw-r--r--   0        0        0     8278 2022-10-11 13:22:55.847583 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_allowlist_entries.py
+-rw-r--r--   0        0        0     9830 2022-10-11 13:22:55.886534 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_available_regions.py
+-rw-r--r--   0        0        0     3679 2022-10-11 13:22:55.799424 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_aws_endpoint_connections.py
+-rw-r--r--   0        0        0     8690 2022-10-11 13:22:55.920740 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_cluster_nodes.py
+-rw-r--r--   0        0        0     8278 2022-10-11 13:22:55.945252 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_clusters.py
+-rw-r--r--   0        0        0     8025 2022-10-11 13:22:55.966494 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_databases.py
+-rw-r--r--   0        0        0     3366 2022-10-11 13:22:55.859861 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_invoices.py
+-rw-r--r--   0        0        0     3697 2022-10-11 13:22:55.857707 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_private_endpoint_services.py
+-rw-r--r--   0        0        0     7886 2022-10-11 13:22:55.962783 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_sql_users.py
+-rw-r--r--   0        0        0     5802 2022-10-11 13:22:55.898687 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_set_aws_endpoint_connection_state.py
+-rw-r--r--   0        0        0     5301 2022-10-11 13:22:55.923174 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cluster.py
+-rw-r--r--   0        0        0     5514 2022-10-11 13:22:55.881565 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cmek_spec.py
+-rw-r--r--   0        0        0     4680 2022-10-11 13:22:55.893644 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cmek_status.py
+-rw-r--r--   0        0        0     4966 2022-10-11 13:22:55.892300 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_sql_user_password.py
+-rw-r--r--   0        0        0     1821 2022-10-11 13:22:55.842114 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/client.py
+-rw-r--r--   0        0        0     6019 2022-10-11 13:22:54.752567 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/__init__.py
+-rw-r--r--   0        0        0     2223 2022-10-11 13:22:55.869441 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/allowlist_entry.py
+-rw-r--r--   0        0        0     5409 2022-10-11 13:22:55.865913 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/any_.py
+-rw-r--r--   0        0        0      153 2022-10-11 13:22:54.858809 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/api_cloud_provider.py
+-rw-r--r--   0        0        0     2987 2022-10-11 13:22:55.923507 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/aws_endpoint_connection.py
+-rw-r--r--   0        0        0      496 2022-10-11 13:22:54.641625 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/aws_endpoint_connection_status.py
+-rw-r--r--   0        0        0     2009 2022-10-11 13:22:55.941976 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/aws_endpoint_connections.py
+-rw-r--r--   0        0        0     2408 2022-10-11 13:22:55.931003 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/aws_private_link_service_detail.py
+-rw-r--r--   0        0        0     2370 2022-10-11 13:22:55.948900 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cloud_provider_region.py
+-rw-r--r--   0        0        0     7528 2022-10-11 13:22:56.105088 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cluster.py
+-rw-r--r--   0        0        0     2693 2022-10-11 13:22:55.958548 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cluster_config.py
+-rw-r--r--   0        0        0      257 2022-10-11 13:22:54.785600 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cluster_state_type.py
+-rw-r--r--   0        0        0     1290 2022-10-11 13:22:54.830811 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cluster_status_type.py
+-rw-r--r--   0        0        0     4943 2022-10-11 13:22:55.994055 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_cluster_info.py
+-rw-r--r--   0        0        0      145 2022-10-11 13:22:54.645399 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_customer_action.py
+-rw-r--r--   0        0        0     6467 2022-10-11 13:22:56.065530 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_key_info.py
+-rw-r--r--   0        0        0     2728 2022-10-11 13:22:56.000304 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_key_specification.py
+-rw-r--r--   0        0        0      176 2022-10-11 13:22:54.774650 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_key_type.py
+-rw-r--r--   0        0        0     5173 2022-10-11 13:22:56.028525 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_region_info.py
+-rw-r--r--   0        0        0     2587 2022-10-11 13:22:56.011517 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_region_specification.py
+-rw-r--r--   0        0        0      441 2022-10-11 13:22:54.650080 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_status.py
+-rw-r--r--   0        0        0     2037 2022-10-11 13:22:55.999706 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_add_allowlist_entry_2_allowlist_entry.py
+-rw-r--r--   0        0        0     1615 2022-10-11 13:22:55.984243 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_create_database_create_database_request.py
+-rw-r--r--   0        0        0     1366 2022-10-11 13:22:55.978580 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_create_private_endpoint_services_json_body.py
+-rw-r--r--   0        0        0     1820 2022-10-11 13:22:56.019379 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_create_sql_user_create_sql_user_request.py
+-rw-r--r--   0        0        0     1795 2022-10-11 13:22:55.996109 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_edit_database_update_database_request.py
+-rw-r--r--   0        0        0     2406 2022-10-11 13:22:56.017225 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_enable_cmek_spec_cmek_cluster_specification.py
+-rw-r--r--   0        0        0     3099 2022-10-11 13:22:56.070061 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_enable_log_export_enable_log_export_request.py
+-rw-r--r--   0        0        0      192 2022-10-11 13:22:54.733648 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_list_allowlist_entries_pagination_sort_order.py
+-rw-r--r--   0        0        0      192 2022-10-11 13:22:54.819567 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_list_available_regions_pagination_sort_order.py
+-rw-r--r--   0        0        0      179 2022-10-11 13:22:54.746676 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_list_available_regions_provider.py
+-rw-r--r--   0        0        0      188 2022-10-11 13:22:54.735998 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_list_cluster_nodes_pagination_sort_order.py
+-rw-r--r--   0        0        0      184 2022-10-11 13:22:54.772358 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_list_clusters_pagination_sort_order.py
+-rw-r--r--   0        0        0      185 2022-10-11 13:22:54.808224 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_list_databases_pagination_sort_order.py
+-rw-r--r--   0        0        0      184 2022-10-11 13:22:54.866303 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_list_sql_users_pagination_sort_order.py
+-rw-r--r--   0        0        0     2166 2022-10-11 13:22:56.053632 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_set_aws_endpoint_connection_state_json_body.py
+-rw-r--r--   0        0        0     2044 2022-10-11 13:22:56.046252 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_allowlist_entry_allowlist_entry.py
+-rw-r--r--   0        0        0     2406 2022-10-11 13:22:56.035163 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_spec_cmek_cluster_specification.py
+-rw-r--r--   0        0        0     1885 2022-10-11 13:22:56.038805 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_status_update_cmek_status_request.py
+-rw-r--r--   0        0        0     1740 2022-10-11 13:22:56.073362 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_sql_user_password_update_sql_user_password_request.py
+-rw-r--r--   0        0        0     2409 2022-10-11 13:22:56.111997 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/create_cluster_request.py
+-rw-r--r--   0        0        0     2913 2022-10-11 13:22:56.130705 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/create_cluster_specification.py
+-rw-r--r--   0        0        0      175 2022-10-11 13:22:54.835751 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/currency.py
+-rw-r--r--   0        0        0     2169 2022-10-11 13:22:56.086018 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/currency_amount.py
+-rw-r--r--   0        0        0     1677 2022-10-11 13:22:56.070994 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/database.py
+-rw-r--r--   0        0        0     2954 2022-10-11 13:22:56.087520 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_cluster_create_specification.py
+-rw-r--r--   0        0        0     1525 2022-10-11 13:22:56.069722 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_cluster_create_specification_region_nodes.py
+-rw-r--r--   0        0        0     4533 2022-10-11 13:22:56.167654 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_cluster_update_specification.py
+-rw-r--r--   0        0        0     1525 2022-10-11 13:22:56.079458 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_cluster_update_specification_region_nodes.py
+-rw-r--r--   0        0        0     2856 2022-10-11 13:22:56.131437 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_hardware_config.py
+-rw-r--r--   0        0        0     2675 2022-10-11 13:22:56.148929 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_hardware_create_specification.py
+-rw-r--r--   0        0        0     3045 2022-10-11 13:22:56.182585 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_hardware_update_specification.py
+-rw-r--r--   0        0        0     2238 2022-10-11 13:22:56.165101 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_machine_type_specification.py
+-rw-r--r--   0        0        0     4368 2022-10-11 13:22:56.237883 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/invoice.py
+-rw-r--r--   0        0        0     3446 2022-10-11 13:22:56.207945 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/invoice_item.py
+-rw-r--r--   0        0        0     3108 2022-10-11 13:22:56.220016 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/keyset_pagination_request.py
+-rw-r--r--   0        0        0     1886 2022-10-11 13:22:56.175651 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/keyset_pagination_response.py
+-rw-r--r--   0        0        0     2651 2022-10-11 13:22:56.154789 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/line_item.py
+-rw-r--r--   0        0        0     2920 2022-10-11 13:22:56.223544 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_allowlist_entries_response.py
+-rw-r--r--   0        0        0     2688 2022-10-11 13:22:56.229355 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_available_regions_response.py
+-rw-r--r--   0        0        0     2547 2022-10-11 13:22:56.230083 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_cluster_nodes_response.py
+-rw-r--r--   0        0        0     2605 2022-10-11 13:22:56.208968 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_clusters_response.py
+-rw-r--r--   0        0        0     2637 2022-10-11 13:22:56.214610 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_databases_response.py
+-rw-r--r--   0        0        0     1858 2022-10-11 13:22:56.222098 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_invoices_response.py
+-rw-r--r--   0        0        0     2543 2022-10-11 13:22:56.242567 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_sql_users_response.py
+-rw-r--r--   0        0        0     5153 2022-10-11 13:22:56.279998 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/log_export_cluster_info.py
+-rw-r--r--   0        0        0     3262 2022-10-11 13:22:56.250016 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/log_export_cluster_specification.py
+-rw-r--r--   0        0        0      298 2022-10-11 13:22:54.763492 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/log_export_status.py
+-rw-r--r--   0        0        0      200 2022-10-11 13:22:54.803680 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/log_export_type.py
+-rw-r--r--   0        0        0     1767 2022-10-11 13:22:56.246467 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/node.py
+-rw-r--r--   0        0        0      161 2022-10-11 13:22:54.828080 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/node_status.py
+-rw-r--r--   0        0        0      189 2022-10-11 13:22:54.657770 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/plan.py
+-rw-r--r--   0        0        0     2759 2022-10-11 13:22:56.257462 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/private_endpoint_service.py
+-rw-r--r--   0        0        0     1967 2022-10-11 13:22:56.250128 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/private_endpoint_services.py
+-rw-r--r--   0        0        0      513 2022-10-11 13:22:54.643633 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/private_endpoints.py
+-rw-r--r--   0        0        0      177 2022-10-11 13:22:54.714453 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/quantity_unit_type.py
+-rw-r--r--   0        0        0     1907 2022-10-11 13:22:56.262181 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/region.py
+-rw-r--r--   0        0        0     1749 2022-10-11 13:22:56.263053 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/serverless_cluster_config.py
+-rw-r--r--   0        0        0     1934 2022-10-11 13:22:56.267556 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/serverless_cluster_create_specification.py
+-rw-r--r--   0        0        0     1555 2022-10-11 13:22:56.258517 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/serverless_cluster_update_specification.py
+-rw-r--r--   0        0        0      148 2022-10-11 13:22:54.647733 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/sort_order.py
+-rw-r--r--   0        0        0     1334 2022-10-11 13:22:56.266481 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/sql_user.py
+-rw-r--r--   0        0        0     2398 2022-10-11 13:22:56.286225 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/status.py
+-rw-r--r--   0        0        0     3061 2022-10-11 13:22:56.286569 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/update_cluster_specification.py
+-rw-r--r--   0        0        0       25 2022-10-11 13:22:53.342556 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/py.typed
+-rw-r--r--   0        0        0      939 2022-10-11 13:22:56.264237 cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/types.py
+-rw-r--r--   0        0        0      724 2022-10-11 13:55:16.348242 cockroachdb_cloud_client-2022.9.20/pyproject.toml
+-rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 cockroachdb_cloud_client-2022.9.20/setup.py
+-rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 cockroachdb_cloud_client-2022.9.20/PKG-INFO
```

### Comparing `cockroachdb_cloud_client-0.1.1/LICENSE` & `cockroachdb_cloud_client-2022.9.20/LICENSE`

 * *Files identical despite different names*

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_add_allowlist_entry.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cmek_spec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,181 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.allowlist_entry import AllowlistEntry
+from ...models.cmek_cluster_info import CMEKClusterInfo
+from ...models.cockroach_cloud_update_cmek_spec_cmek_cluster_specification import (
+    CockroachCloudUpdateCMEKSpecCMEKClusterSpecification,
+)
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
-    json_body: AllowlistEntry,
+    json_body: CockroachCloudUpdateCMEKSpecCMEKClusterSpecification,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/networking/allowlist".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/cmek".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "post",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[AllowlistEntry, Any]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = AllowlistEntry.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, CMEKClusterInfo]]:
+    if response.status_code == 200:
+        response_200 = CMEKClusterInfo.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[AllowlistEntry, Any]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, CMEKClusterInfo]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
-    json_body: AllowlistEntry,
-) -> Response[Union[AllowlistEntry, Any]]:
-    """Add a new CIDR address to the IP allowlist
+    json_body: CockroachCloudUpdateCMEKSpecCMEKClusterSpecification,
+) -> Response[Union[Any, CMEKClusterInfo]]:
+    """Enable or update the CMEK spec for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'name':
-            'Example', 'sql': True, 'ui': True}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Response[Union[AllowlistEntry, Any]]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
-    json_body: AllowlistEntry,
-) -> Optional[Union[AllowlistEntry, Any]]:
-    """Add a new CIDR address to the IP allowlist
+    json_body: CockroachCloudUpdateCMEKSpecCMEKClusterSpecification,
+) -> Optional[Union[Any, CMEKClusterInfo]]:
+    """Enable or update the CMEK spec for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'name':
-            'Example', 'sql': True, 'ui': True}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Union[AllowlistEntry, Any]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
-    json_body: AllowlistEntry,
-) -> Response[Union[AllowlistEntry, Any]]:
-    """Add a new CIDR address to the IP allowlist
+    json_body: CockroachCloudUpdateCMEKSpecCMEKClusterSpecification,
+) -> Response[Union[Any, CMEKClusterInfo]]:
+    """Enable or update the CMEK spec for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'name':
-            'Example', 'sql': True, 'ui': True}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Response[Union[AllowlistEntry, Any]]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
-    json_body: AllowlistEntry,
-) -> Optional[Union[AllowlistEntry, Any]]:
-    """Add a new CIDR address to the IP allowlist
+    json_body: CockroachCloudUpdateCMEKSpecCMEKClusterSpecification,
+) -> Optional[Union[Any, CMEKClusterInfo]]:
+    """Enable or update the CMEK spec for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'name':
-            'Example', 'sql': True, 'ui': True}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Union[AllowlistEntry, Any]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
             json_body=json_body,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_cluster.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
 from ...models.cluster import Cluster
 from ...models.create_cluster_request import CreateClusterRequest
 from ...types import Response
 
 
 def _get_kwargs(
@@ -24,158 +22,138 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, Cluster]]:
-    if response.status_code == HTTPStatus.OK:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Cluster]]:
+    if response.status_code == 200:
         response_200 = Cluster.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, Cluster]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Cluster]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     json_body: CreateClusterRequest,
 ) -> Response[Union[Any, Cluster]]:
-    """Create and initialize a new cluster
+    """Create and initialize a new cluster.
 
     Args:
         json_body (CreateClusterRequest):  Example: {'name': 'test-cluster', 'provider': 'GCP',
             'spec': {'serverless': {'regions': ['us-central1'], 'spend_limit': 0}}}.
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, Cluster]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
     json_body: CreateClusterRequest,
 ) -> Optional[Union[Any, Cluster]]:
-    """Create and initialize a new cluster
+    """Create and initialize a new cluster.
 
     Args:
         json_body (CreateClusterRequest):  Example: {'name': 'test-cluster', 'provider': 'GCP',
             'spec': {'serverless': {'regions': ['us-central1'], 'spend_limit': 0}}}.
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, Cluster]
+        Response[Union[Any, Cluster]]
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
     json_body: CreateClusterRequest,
 ) -> Response[Union[Any, Cluster]]:
-    """Create and initialize a new cluster
+    """Create and initialize a new cluster.
 
     Args:
         json_body (CreateClusterRequest):  Example: {'name': 'test-cluster', 'provider': 'GCP',
             'spec': {'serverless': {'regions': ['us-central1'], 'spend_limit': 0}}}.
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, Cluster]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
     json_body: CreateClusterRequest,
 ) -> Optional[Union[Any, Cluster]]:
-    """Create and initialize a new cluster
+    """Create and initialize a new cluster.
 
     Args:
         json_body (CreateClusterRequest):  Example: {'name': 'test-cluster', 'provider': 'GCP',
             'spec': {'serverless': {'regions': ['us-central1'], 'spend_limit': 0}}}.
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, Cluster]
+        Response[Union[Any, Cluster]]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
         )
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_database.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_set_aws_endpoint_connection_state.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,197 +1,194 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cockroach_cloud_create_database_create_database_request import (
-    CockroachCloudCreateDatabaseCreateDatabaseRequest,
+from ...models.aws_endpoint_connection import AwsEndpointConnection
+from ...models.cockroach_cloud_set_aws_endpoint_connection_state_json_body import (
+    CockroachCloudSetAwsEndpointConnectionStateJsonBody,
 )
-from ...models.database import Database
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
+    endpoint_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
+    json_body: CockroachCloudSetAwsEndpointConnectionStateJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/databases".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/networking/aws-endpoint-connections/{endpoint_id}".format(
+        client.base_url, cluster_id=cluster_id, endpoint_id=endpoint_id
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "post",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, Database]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Database.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, AwsEndpointConnection]]:
+    if response.status_code == 200:
+        response_200 = AwsEndpointConnection.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, Database]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, AwsEndpointConnection]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
+    endpoint_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
-) -> Response[Union[Any, Database]]:
-    """Create a new database
+    json_body: CockroachCloudSetAwsEndpointConnectionStateJsonBody,
+) -> Response[Union[Any, AwsEndpointConnection]]:
+    """Sets the AWS Endpoint Connection state based on what is passed in the body: accepted or rejected.
+    The \"status\" in the returned proto does not reflect the latest post-update status, but rather
+    the status before the state is transitioned.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
-            'example_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        endpoint_id (str):
+        json_body (CockroachCloudSetAwsEndpointConnectionStateJsonBody):
 
     Returns:
-        Response[Union[Any, Database]]
+        Response[Union[Any, AwsEndpointConnection]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
+        endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
+    endpoint_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
-) -> Optional[Union[Any, Database]]:
-    """Create a new database
+    json_body: CockroachCloudSetAwsEndpointConnectionStateJsonBody,
+) -> Optional[Union[Any, AwsEndpointConnection]]:
+    """Sets the AWS Endpoint Connection state based on what is passed in the body: accepted or rejected.
+    The \"status\" in the returned proto does not reflect the latest post-update status, but rather
+    the status before the state is transitioned.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
-            'example_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        endpoint_id (str):
+        json_body (CockroachCloudSetAwsEndpointConnectionStateJsonBody):
 
     Returns:
-        Union[Any, Database]
+        Response[Union[Any, AwsEndpointConnection]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
+        endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
+    endpoint_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
-) -> Response[Union[Any, Database]]:
-    """Create a new database
+    json_body: CockroachCloudSetAwsEndpointConnectionStateJsonBody,
+) -> Response[Union[Any, AwsEndpointConnection]]:
+    """Sets the AWS Endpoint Connection state based on what is passed in the body: accepted or rejected.
+    The \"status\" in the returned proto does not reflect the latest post-update status, but rather
+    the status before the state is transitioned.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
-            'example_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        endpoint_id (str):
+        json_body (CockroachCloudSetAwsEndpointConnectionStateJsonBody):
 
     Returns:
-        Response[Union[Any, Database]]
+        Response[Union[Any, AwsEndpointConnection]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
+        endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
+    endpoint_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
-) -> Optional[Union[Any, Database]]:
-    """Create a new database
+    json_body: CockroachCloudSetAwsEndpointConnectionStateJsonBody,
+) -> Optional[Union[Any, AwsEndpointConnection]]:
+    """Sets the AWS Endpoint Connection state based on what is passed in the body: accepted or rejected.
+    The \"status\" in the returned proto does not reflect the latest post-update status, but rather
+    the status before the state is transitioned.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
-            'example_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        endpoint_id (str):
+        json_body (CockroachCloudSetAwsEndpointConnectionStateJsonBody):
 
     Returns:
-        Union[Any, Database]
+        Response[Union[Any, AwsEndpointConnection]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
+            endpoint_id=endpoint_id,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_private_endpoint_services.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_private_endpoint_services.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,173 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
+from ...models.cockroach_cloud_create_private_endpoint_services_json_body import (
+    CockroachCloudCreatePrivateEndpointServicesJsonBody,
+)
 from ...models.private_endpoint_services import PrivateEndpointServices
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudCreatePrivateEndpointServicesJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/clusters/{cluster_id}/networking/private-endpoint-services".format(
         client.base_url, cluster_id=cluster_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, PrivateEndpointServices]]:
-    if response.status_code == HTTPStatus.OK:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, PrivateEndpointServices]]:
+    if response.status_code == 200:
         response_200 = PrivateEndpointServices.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, PrivateEndpointServices]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, PrivateEndpointServices]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudCreatePrivateEndpointServicesJsonBody,
 ) -> Response[Union[Any, PrivateEndpointServices]]:
-    """Creates all PrivateEndpointServices for a given cluster
+    """Creates all PrivateEndpointServices for a given cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreatePrivateEndpointServicesJsonBody):
 
     Returns:
         Response[Union[Any, PrivateEndpointServices]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudCreatePrivateEndpointServicesJsonBody,
 ) -> Optional[Union[Any, PrivateEndpointServices]]:
-    """Creates all PrivateEndpointServices for a given cluster
+    """Creates all PrivateEndpointServices for a given cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreatePrivateEndpointServicesJsonBody):
 
     Returns:
-        Union[Any, PrivateEndpointServices]
+        Response[Union[Any, PrivateEndpointServices]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudCreatePrivateEndpointServicesJsonBody,
 ) -> Response[Union[Any, PrivateEndpointServices]]:
-    """Creates all PrivateEndpointServices for a given cluster
+    """Creates all PrivateEndpointServices for a given cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreatePrivateEndpointServicesJsonBody):
 
     Returns:
         Response[Union[Any, PrivateEndpointServices]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudCreatePrivateEndpointServicesJsonBody,
 ) -> Optional[Union[Any, PrivateEndpointServices]]:
-    """Creates all PrivateEndpointServices for a given cluster
+    """Creates all PrivateEndpointServices for a given cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreatePrivateEndpointServicesJsonBody):
 
     Returns:
-        Union[Any, PrivateEndpointServices]
+        Response[Union[Any, PrivateEndpointServices]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_sql_user.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_enable_cmek_spec.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,195 +1,181 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cockroach_cloud_create_sql_user_create_sql_user_request import (
-    CockroachCloudCreateSQLUserCreateSQLUserRequest,
+from ...models.cmek_cluster_info import CMEKClusterInfo
+from ...models.cockroach_cloud_enable_cmek_spec_cmek_cluster_specification import (
+    CockroachCloudEnableCMEKSpecCMEKClusterSpecification,
 )
-from ...models.sql_user import SQLUser
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
+    json_body: CockroachCloudEnableCMEKSpecCMEKClusterSpecification,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/sql-users".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/cmek".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, SQLUser]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = SQLUser.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, CMEKClusterInfo]]:
+    if response.status_code == 200:
+        response_200 = CMEKClusterInfo.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, SQLUser]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, CMEKClusterInfo]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
-) -> Response[Union[Any, SQLUser]]:
-    """Create a new SQL user
+    json_body: CockroachCloudEnableCMEKSpecCMEKClusterSpecification,
+) -> Response[Union[Any, CMEKClusterInfo]]:
+    """Enable CMEK for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
-            'example_username', 'password': 'example_password'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEnableCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Response[Union[Any, SQLUser]]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
-) -> Optional[Union[Any, SQLUser]]:
-    """Create a new SQL user
+    json_body: CockroachCloudEnableCMEKSpecCMEKClusterSpecification,
+) -> Optional[Union[Any, CMEKClusterInfo]]:
+    """Enable CMEK for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
-            'example_username', 'password': 'example_password'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEnableCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Union[Any, SQLUser]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
-) -> Response[Union[Any, SQLUser]]:
-    """Create a new SQL user
+    json_body: CockroachCloudEnableCMEKSpecCMEKClusterSpecification,
+) -> Response[Union[Any, CMEKClusterInfo]]:
+    """Enable CMEK for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
-            'example_username', 'password': 'example_password'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEnableCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Response[Union[Any, SQLUser]]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
-    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
-) -> Optional[Union[Any, SQLUser]]:
-    """Create a new SQL user
+    json_body: CockroachCloudEnableCMEKSpecCMEKClusterSpecification,
+) -> Optional[Union[Any, CMEKClusterInfo]]:
+    """Enable CMEK for a cluster.
 
     Args:
         cluster_id (str):
-        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
-            'example_username', 'password': 'example_password'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEnableCMEKSpecCMEKClusterSpecification):  Example:
+            {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri':
+            'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key', 'auth_principal':
+            'arn:aws:iam::account:role/role-name-with-path'}}]}.
 
     Returns:
-        Union[Any, SQLUser]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
             json_body=json_body,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_allowlist_entry.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_allowlist_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
 from ...models.allowlist_entry import AllowlistEntry
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
@@ -25,71 +23,63 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[AllowlistEntry, Any]]:
-    if response.status_code == HTTPStatus.OK:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[AllowlistEntry, Any]]:
+    if response.status_code == 200:
         response_200 = AllowlistEntry.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[AllowlistEntry, Any]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[AllowlistEntry, Any]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     cidr_ip: str,
     cidr_mask: int,
     *,
     client: Client,
 ) -> Response[Union[AllowlistEntry, Any]]:
-    """Delete an IP allowlist entry
+    """Delete an IP allowlist entry.
 
     Args:
         cluster_id (str):
         cidr_ip (str):
         cidr_mask (int):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[AllowlistEntry, Any]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         cidr_ip=cidr_ip,
@@ -98,37 +88,33 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     cidr_ip: str,
     cidr_mask: int,
     *,
     client: Client,
 ) -> Optional[Union[AllowlistEntry, Any]]:
-    """Delete an IP allowlist entry
+    """Delete an IP allowlist entry.
 
     Args:
         cluster_id (str):
         cidr_ip (str):
         cidr_mask (int):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[AllowlistEntry, Any]
+        Response[Union[AllowlistEntry, Any]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         cidr_ip=cidr_ip,
         cidr_mask=cidr_mask,
         client=client,
@@ -138,62 +124,54 @@
 async def asyncio_detailed(
     cluster_id: str,
     cidr_ip: str,
     cidr_mask: int,
     *,
     client: Client,
 ) -> Response[Union[AllowlistEntry, Any]]:
-    """Delete an IP allowlist entry
+    """Delete an IP allowlist entry.
 
     Args:
         cluster_id (str):
         cidr_ip (str):
         cidr_mask (int):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[AllowlistEntry, Any]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         cidr_ip=cidr_ip,
         cidr_mask=cidr_mask,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     cidr_ip: str,
     cidr_mask: int,
     *,
     client: Client,
 ) -> Optional[Union[AllowlistEntry, Any]]:
-    """Delete an IP allowlist entry
+    """Delete an IP allowlist entry.
 
     Args:
         cluster_id (str):
         cidr_ip (str):
         cidr_mask (int):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[AllowlistEntry, Any]
+        Response[Union[AllowlistEntry, Any]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             cidr_ip=cidr_ip,
             cidr_mask=cidr_mask,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_client_ca_cert.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cluster.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,174 +1,192 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.client_ca_cert_info import ClientCACertInfo
-from ...types import Response
+from ...models.cluster import Cluster
+from ...models.update_cluster_specification import UpdateClusterSpecification
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
+    json_body: UpdateClusterSpecification,
+    field_mask: Union[Unset, None, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/client-ca-cert".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    params: Dict[str, Any] = {}
+    params["field_mask"] = field_mask
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "delete",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
+        "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ClientCACertInfo]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = ClientCACertInfo.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Cluster]]:
+    if response.status_code == 200:
+        response_200 = Cluster.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ClientCACertInfo]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Cluster]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ClientCACertInfo]]:
-    """Delete Client CA Cert for a cluster
+    json_body: UpdateClusterSpecification,
+    field_mask: Union[Unset, None, str] = UNSET,
+) -> Response[Union[Any, Cluster]]:
+    """Scale or edit a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        field_mask (Union[Unset, None, str]):
+        json_body (UpdateClusterSpecification):  Example: {'dedicated': {'region_nodes': {'us-
+            west1': 3, 'us-central1': 5}, 'hardware': {'machine_type': 'n2-standard-8'}}}.
 
     Returns:
-        Response[Union[Any, ClientCACertInfo]]
+        Response[Union[Any, Cluster]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
+        field_mask=field_mask,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ClientCACertInfo]]:
-    """Delete Client CA Cert for a cluster
+    json_body: UpdateClusterSpecification,
+    field_mask: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[Any, Cluster]]:
+    """Scale or edit a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        field_mask (Union[Unset, None, str]):
+        json_body (UpdateClusterSpecification):  Example: {'dedicated': {'region_nodes': {'us-
+            west1': 3, 'us-central1': 5}, 'hardware': {'machine_type': 'n2-standard-8'}}}.
 
     Returns:
-        Union[Any, ClientCACertInfo]
+        Response[Union[Any, Cluster]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
+        field_mask=field_mask,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, ClientCACertInfo]]:
-    """Delete Client CA Cert for a cluster
+    json_body: UpdateClusterSpecification,
+    field_mask: Union[Unset, None, str] = UNSET,
+) -> Response[Union[Any, Cluster]]:
+    """Scale or edit a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        field_mask (Union[Unset, None, str]):
+        json_body (UpdateClusterSpecification):  Example: {'dedicated': {'region_nodes': {'us-
+            west1': 3, 'us-central1': 5}, 'hardware': {'machine_type': 'n2-standard-8'}}}.
 
     Returns:
-        Response[Union[Any, ClientCACertInfo]]
+        Response[Union[Any, Cluster]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
+        field_mask=field_mask,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, ClientCACertInfo]]:
-    """Delete Client CA Cert for a cluster
+    json_body: UpdateClusterSpecification,
+    field_mask: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[Any, Cluster]]:
+    """Scale or edit a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        field_mask (Union[Unset, None, str]):
+        json_body (UpdateClusterSpecification):  Example: {'dedicated': {'region_nodes': {'us-
+            west1': 3, 'us-central1': 5}, 'hardware': {'machine_type': 'n2-standard-8'}}}.
 
     Returns:
-        Union[Any, ClientCACertInfo]
+        Response[Union[Any, Cluster]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
+            json_body=json_body,
+            field_mask=field_mask,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_cluster.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,175 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cluster import Cluster
+from ...models.cockroach_cloud_create_database_create_database_request import (
+    CockroachCloudCreateDatabaseCreateDatabaseRequest,
+)
+from ...models.database import Database
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/databases".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "delete",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, Cluster]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Cluster.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Database]]:
+    if response.status_code == 200:
+        response_200 = Database.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, Cluster]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Database]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Cluster]]:
-    """Delete a cluster and all of its data
+    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
+) -> Response[Union[Any, Database]]:
+    """Create a new database.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
+            'example_database_name'}.
 
     Returns:
-        Response[Union[Any, Cluster]]
+        Response[Union[Any, Database]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Cluster]]:
-    """Delete a cluster and all of its data
+    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
+) -> Optional[Union[Any, Database]]:
+    """Create a new database.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
+            'example_database_name'}.
 
     Returns:
-        Union[Any, Cluster]
+        Response[Union[Any, Database]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Cluster]]:
-    """Delete a cluster and all of its data
+    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
+) -> Response[Union[Any, Database]]:
+    """Create a new database.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
+            'example_database_name'}.
 
     Returns:
-        Response[Union[Any, Cluster]]
+        Response[Union[Any, Database]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Cluster]]:
-    """Delete a cluster and all of its data
+    json_body: CockroachCloudCreateDatabaseCreateDatabaseRequest,
+) -> Optional[Union[Any, Database]]:
+    """Create a new database.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateDatabaseCreateDatabaseRequest):  Example: {'name':
+            'example_database_name'}.
 
     Returns:
-        Union[Any, Cluster]
+        Response[Union[Any, Database]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_delete_database.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_edit_database.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,175 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
+from ...models.cockroach_cloud_edit_database_update_database_request import (
+    CockroachCloudEditDatabaseUpdateDatabaseRequest,
+)
 from ...models.database import Database
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
-    name: str,
     *,
     client: Client,
+    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/databases/{name}".format(client.base_url, cluster_id=cluster_id, name=name)
+    url = "{}/api/v1/clusters/{cluster_id}/databases".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "delete",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, Database]]:
-    if response.status_code == HTTPStatus.OK:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Database]]:
+    if response.status_code == 200:
         response_200 = Database.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, Database]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Database]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
-    name: str,
     *,
     client: Client,
+    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
 ) -> Response[Union[Any, Database]]:
-    """Delete a database
+    """Update a database.
 
     Args:
         cluster_id (str):
-        name (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'new_name':
+            'example_new_database_name'}.
 
     Returns:
         Response[Union[Any, Database]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
-        name=name,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
-    name: str,
     *,
     client: Client,
+    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
 ) -> Optional[Union[Any, Database]]:
-    """Delete a database
+    """Update a database.
 
     Args:
         cluster_id (str):
-        name (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'new_name':
+            'example_new_database_name'}.
 
     Returns:
-        Union[Any, Database]
+        Response[Union[Any, Database]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
-        name=name,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
-    name: str,
     *,
     client: Client,
+    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
 ) -> Response[Union[Any, Database]]:
-    """Delete a database
+    """Update a database.
 
     Args:
         cluster_id (str):
-        name (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'new_name':
+            'example_new_database_name'}.
 
     Returns:
         Response[Union[Any, Database]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
-        name=name,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
-    name: str,
     *,
     client: Client,
+    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
 ) -> Optional[Union[Any, Database]]:
-    """Delete a database
+    """Update a database.
 
     Args:
         cluster_id (str):
-        name (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'new_name':
+            'example_new_database_name'}.
 
     Returns:
-        Union[Any, Database]
+        Response[Union[Any, Database]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
-            name=name,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_edit_database.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_sql_user_password.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,140 +1,128 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cockroach_cloud_edit_database_update_database_request import (
-    CockroachCloudEditDatabaseUpdateDatabaseRequest,
+from ...models.cockroach_cloud_update_sql_user_password_update_sql_user_password_request import (
+    CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest,
 )
-from ...models.database import Database
+from ...models.sql_user import SQLUser
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     name: str,
     *,
     client: Client,
-    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
+    json_body: CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/databases/{name}".format(client.base_url, cluster_id=cluster_id, name=name)
+    url = "{}/api/v1/clusters/{cluster_id}/sql-users/{name}/password".format(
+        client.base_url, cluster_id=cluster_id, name=name
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "patch",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, Database]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Database.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, SQLUser]]:
+    if response.status_code == 200:
+        response_200 = SQLUser.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, Database]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, SQLUser]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     name: str,
     *,
     client: Client,
-    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
-) -> Response[Union[Any, Database]]:
-    """Update a database
+    json_body: CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest,
+) -> Response[Union[Any, SQLUser]]:
+    """Update a SQL user's password.
 
     Args:
         cluster_id (str):
         name (str):
-        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'name':
-            'example_database_name', 'new_name': 'example_new_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest):  Example:
+            {'password': 'example_new_password'}.
 
     Returns:
-        Response[Union[Any, Database]]
+        Response[Union[Any, SQLUser]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         name=name,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     name: str,
     *,
     client: Client,
-    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
-) -> Optional[Union[Any, Database]]:
-    """Update a database
+    json_body: CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest,
+) -> Optional[Union[Any, SQLUser]]:
+    """Update a SQL user's password.
 
     Args:
         cluster_id (str):
         name (str):
-        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'name':
-            'example_database_name', 'new_name': 'example_new_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest):  Example:
+            {'password': 'example_new_password'}.
 
     Returns:
-        Union[Any, Database]
+        Response[Union[Any, SQLUser]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         name=name,
         client=client,
         json_body=json_body,
@@ -142,66 +130,58 @@
 
 
 async def asyncio_detailed(
     cluster_id: str,
     name: str,
     *,
     client: Client,
-    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
-) -> Response[Union[Any, Database]]:
-    """Update a database
+    json_body: CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest,
+) -> Response[Union[Any, SQLUser]]:
+    """Update a SQL user's password.
 
     Args:
         cluster_id (str):
         name (str):
-        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'name':
-            'example_database_name', 'new_name': 'example_new_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest):  Example:
+            {'password': 'example_new_password'}.
 
     Returns:
-        Response[Union[Any, Database]]
+        Response[Union[Any, SQLUser]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         name=name,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     name: str,
     *,
     client: Client,
-    json_body: CockroachCloudEditDatabaseUpdateDatabaseRequest,
-) -> Optional[Union[Any, Database]]:
-    """Update a database
+    json_body: CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest,
+) -> Optional[Union[Any, SQLUser]]:
+    """Update a SQL user's password.
 
     Args:
         cluster_id (str):
         name (str):
-        json_body (CockroachCloudEditDatabaseUpdateDatabaseRequest):  Example: {'name':
-            'example_database_name', 'new_name': 'example_new_database_name'}.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest):  Example:
+            {'password': 'example_new_password'}.
 
     Returns:
-        Union[Any, Database]
+        Response[Union[Any, SQLUser]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             name=name,
             client=client,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_cluster.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_create_sql_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,174 +1,175 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cluster import Cluster
+from ...models.cockroach_cloud_create_sql_user_create_sql_user_request import (
+    CockroachCloudCreateSQLUserCreateSQLUserRequest,
+)
+from ...models.sql_user import SQLUser
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/sql-users".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, Cluster]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Cluster.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, SQLUser]]:
+    if response.status_code == 200:
+        response_200 = SQLUser.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, Cluster]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, SQLUser]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Cluster]]:
-    """Get extended information about a cluster
+    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
+) -> Response[Union[Any, SQLUser]]:
+    """Create a new SQL user.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
+            'example_username', 'password': 'example_password'}.
 
     Returns:
-        Response[Union[Any, Cluster]]
+        Response[Union[Any, SQLUser]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Cluster]]:
-    """Get extended information about a cluster
+    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
+) -> Optional[Union[Any, SQLUser]]:
+    """Create a new SQL user.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
+            'example_username', 'password': 'example_password'}.
 
     Returns:
-        Union[Any, Cluster]
+        Response[Union[Any, SQLUser]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, Cluster]]:
-    """Get extended information about a cluster
+    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
+) -> Response[Union[Any, SQLUser]]:
+    """Create a new SQL user.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
+            'example_username', 'password': 'example_password'}.
 
     Returns:
-        Response[Union[Any, Cluster]]
+        Response[Union[Any, SQLUser]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Cluster]]:
-    """Get extended information about a cluster
+    json_body: CockroachCloudCreateSQLUserCreateSQLUserRequest,
+) -> Optional[Union[Any, SQLUser]]:
+    """Create a new SQL user.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudCreateSQLUserCreateSQLUserRequest):  Example: {'name':
+            'example_username', 'password': 'example_password'}.
 
     Returns:
-        Union[Any, Cluster]
+        Response[Union[Any, SQLUser]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_cmek_cluster_info.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_add_allowlist_entry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,174 +1,172 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cmek_cluster_info import CMEKClusterInfo
+from ...models.allowlist_entry import AllowlistEntry
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
+    json_body: AllowlistEntry,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/cmek".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/networking/allowlist".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, CMEKClusterInfo]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = CMEKClusterInfo.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[AllowlistEntry, Any]]:
+    if response.status_code == 200:
+        response_200 = AllowlistEntry.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, CMEKClusterInfo]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[AllowlistEntry, Any]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, CMEKClusterInfo]]:
-    """Get CMEK-related information for a cluster
+    json_body: AllowlistEntry,
+) -> Response[Union[AllowlistEntry, Any]]:
+    """Add a new CIDR address to the IP allowlist.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'ui':
+            True, 'sql': True, 'name': 'Example'}.
 
     Returns:
-        Response[Union[Any, CMEKClusterInfo]]
+        Response[Union[AllowlistEntry, Any]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, CMEKClusterInfo]]:
-    """Get CMEK-related information for a cluster
+    json_body: AllowlistEntry,
+) -> Optional[Union[AllowlistEntry, Any]]:
+    """Add a new CIDR address to the IP allowlist.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'ui':
+            True, 'sql': True, 'name': 'Example'}.
 
     Returns:
-        Union[Any, CMEKClusterInfo]
+        Response[Union[AllowlistEntry, Any]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, CMEKClusterInfo]]:
-    """Get CMEK-related information for a cluster
+    json_body: AllowlistEntry,
+) -> Response[Union[AllowlistEntry, Any]]:
+    """Add a new CIDR address to the IP allowlist.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'ui':
+            True, 'sql': True, 'name': 'Example'}.
 
     Returns:
-        Response[Union[Any, CMEKClusterInfo]]
+        Response[Union[AllowlistEntry, Any]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, CMEKClusterInfo]]:
-    """Get CMEK-related information for a cluster
+    json_body: AllowlistEntry,
+) -> Optional[Union[AllowlistEntry, Any]]:
+    """Add a new CIDR address to the IP allowlist.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (AllowlistEntry):  Example: {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'ui':
+            True, 'sql': True, 'name': 'Example'}.
 
     Returns:
-        Union[Any, CMEKClusterInfo]
+        Response[Union[AllowlistEntry, Any]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_get_datadog_metric_export_info.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_update_cmek_status.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,174 +1,175 @@
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.datadog_metric_export_info import DatadogMetricExportInfo
+from ...models.cmek_cluster_info import CMEKClusterInfo
+from ...models.cockroach_cloud_update_cmek_status_update_cmek_status_request import (
+    CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest,
+)
 from ...types import Response
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
+    json_body: CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/metricexport/datadog".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/cmek".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "get",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, DatadogMetricExportInfo]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = DatadogMetricExportInfo.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, CMEKClusterInfo]]:
+    if response.status_code == 200:
+        response_200 = CMEKClusterInfo.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, DatadogMetricExportInfo]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, CMEKClusterInfo]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, DatadogMetricExportInfo]]:
-    """Get the Datadog Metric Export configuration for a cluster
+    json_body: CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest,
+) -> Response[Union[Any, CMEKClusterInfo]]:
+    """Update the CMEK-related status for a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest):  Example: {'action':
+            'REVOKE'}.
 
     Returns:
-        Response[Union[Any, DatadogMetricExportInfo]]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, DatadogMetricExportInfo]]:
-    """Get the Datadog Metric Export configuration for a cluster
+    json_body: CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest,
+) -> Optional[Union[Any, CMEKClusterInfo]]:
+    """Update the CMEK-related status for a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest):  Example: {'action':
+            'REVOKE'}.
 
     Returns:
-        Union[Any, DatadogMetricExportInfo]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
-) -> Response[Union[Any, DatadogMetricExportInfo]]:
-    """Get the Datadog Metric Export configuration for a cluster
+    json_body: CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest,
+) -> Response[Union[Any, CMEKClusterInfo]]:
+    """Update the CMEK-related status for a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest):  Example: {'action':
+            'REVOKE'}.
 
     Returns:
-        Response[Union[Any, DatadogMetricExportInfo]]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
-) -> Optional[Union[Any, DatadogMetricExportInfo]]:
-    """Get the Datadog Metric Export configuration for a cluster
+    json_body: CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest,
+) -> Optional[Union[Any, CMEKClusterInfo]]:
+    """Update the CMEK-related status for a cluster.
 
     Args:
         cluster_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        json_body (CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest):  Example: {'action':
+            'REVOKE'}.
 
     Returns:
-        Union[Any, DatadogMetricExportInfo]
+        Response[Union[Any, CMEKClusterInfo]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_allowlist_entries.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_allowlist_entries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import datetime
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
 from ...models.cockroach_cloud_list_allowlist_entries_pagination_sort_order import (
     CockroachCloudListAllowlistEntriesPaginationSortOrder,
 )
 from ...models.list_allowlist_entries_response import ListAllowlistEntriesResponse
 from ...types import UNSET, Response, Unset
 
@@ -48,79 +46,71 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ListAllowlistEntriesResponse]]:
-    if response.status_code == HTTPStatus.OK:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ListAllowlistEntriesResponse]]:
+    if response.status_code == 200:
         response_200 = ListAllowlistEntriesResponse.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ListAllowlistEntriesResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, ListAllowlistEntriesResponse]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAllowlistEntriesPaginationSortOrder] = UNSET,
 ) -> Response[Union[Any, ListAllowlistEntriesResponse]]:
-    """Get the IP allowlist and propagation status for a cluster
+    """Get the IP allowlist and propagation status for a cluster.
 
      Sort order: CIDR address
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAllowlistEntriesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, ListAllowlistEntriesResponse]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
@@ -131,44 +121,40 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAllowlistEntriesPaginationSortOrder] = UNSET,
 ) -> Optional[Union[Any, ListAllowlistEntriesResponse]]:
-    """Get the IP allowlist and propagation status for a cluster
+    """Get the IP allowlist and propagation status for a cluster.
 
      Sort order: CIDR address
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAllowlistEntriesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, ListAllowlistEntriesResponse]
+        Response[Union[Any, ListAllowlistEntriesResponse]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
@@ -182,30 +168,26 @@
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAllowlistEntriesPaginationSortOrder] = UNSET,
 ) -> Response[Union[Any, ListAllowlistEntriesResponse]]:
-    """Get the IP allowlist and propagation status for a cluster
+    """Get the IP allowlist and propagation status for a cluster.
 
      Sort order: CIDR address
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAllowlistEntriesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, ListAllowlistEntriesResponse]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
@@ -214,44 +196,40 @@
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAllowlistEntriesPaginationSortOrder] = UNSET,
 ) -> Optional[Union[Any, ListAllowlistEntriesResponse]]:
-    """Get the IP allowlist and propagation status for a cluster
+    """Get the IP allowlist and propagation status for a cluster.
 
      Sort order: CIDR address
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAllowlistEntriesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, ListAllowlistEntriesResponse]
+        Response[Union[Any, ListAllowlistEntriesResponse]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
             pagination_page=pagination_page,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_available_regions.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_available_regions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import datetime
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
 from ...models.cockroach_cloud_list_available_regions_pagination_sort_order import (
     CockroachCloudListAvailableRegionsPaginationSortOrder,
 )
 from ...models.cockroach_cloud_list_available_regions_provider import CockroachCloudListAvailableRegionsProvider
 from ...models.list_available_regions_response import ListAvailableRegionsResponse
 from ...types import UNSET, Response, Unset
@@ -58,81 +56,73 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ListAvailableRegionsResponse]]:
-    if response.status_code == HTTPStatus.OK:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ListAvailableRegionsResponse]]:
+    if response.status_code == 200:
         response_200 = ListAvailableRegionsResponse.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ListAvailableRegionsResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, ListAvailableRegionsResponse]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     provider: Union[Unset, None, CockroachCloudListAvailableRegionsProvider] = UNSET,
     serverless: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAvailableRegionsPaginationSortOrder] = UNSET,
 ) -> Response[Union[Any, ListAvailableRegionsResponse]]:
-    """List the regions available for new clusters and nodes
+    """List the regions available for new clusters and nodes.
 
      Sort order: Distance (based on client IP address)
 
     Args:
         provider (Union[Unset, None, CockroachCloudListAvailableRegionsProvider]):
         serverless (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAvailableRegionsPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, ListAvailableRegionsResponse]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         provider=provider,
@@ -144,46 +134,42 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
     provider: Union[Unset, None, CockroachCloudListAvailableRegionsProvider] = UNSET,
     serverless: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAvailableRegionsPaginationSortOrder] = UNSET,
 ) -> Optional[Union[Any, ListAvailableRegionsResponse]]:
-    """List the regions available for new clusters and nodes
+    """List the regions available for new clusters and nodes.
 
      Sort order: Distance (based on client IP address)
 
     Args:
         provider (Union[Unset, None, CockroachCloudListAvailableRegionsProvider]):
         serverless (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAvailableRegionsPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, ListAvailableRegionsResponse]
+        Response[Union[Any, ListAvailableRegionsResponse]]
     """
 
     return sync_detailed(
         client=client,
         provider=provider,
         serverless=serverless,
         pagination_page=pagination_page,
@@ -199,31 +185,27 @@
     provider: Union[Unset, None, CockroachCloudListAvailableRegionsProvider] = UNSET,
     serverless: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAvailableRegionsPaginationSortOrder] = UNSET,
 ) -> Response[Union[Any, ListAvailableRegionsResponse]]:
-    """List the regions available for new clusters and nodes
+    """List the regions available for new clusters and nodes.
 
      Sort order: Distance (based on client IP address)
 
     Args:
         provider (Union[Unset, None, CockroachCloudListAvailableRegionsProvider]):
         serverless (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAvailableRegionsPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, ListAvailableRegionsResponse]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         provider=provider,
@@ -233,46 +215,42 @@
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
     provider: Union[Unset, None, CockroachCloudListAvailableRegionsProvider] = UNSET,
     serverless: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListAvailableRegionsPaginationSortOrder] = UNSET,
 ) -> Optional[Union[Any, ListAvailableRegionsResponse]]:
-    """List the regions available for new clusters and nodes
+    """List the regions available for new clusters and nodes.
 
      Sort order: Distance (based on client IP address)
 
     Args:
         provider (Union[Unset, None, CockroachCloudListAvailableRegionsProvider]):
         serverless (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListAvailableRegionsPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, ListAvailableRegionsResponse]
+        Response[Union[Any, ListAvailableRegionsResponse]]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             provider=provider,
             serverless=serverless,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_clusters.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_sql_users.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 import datetime
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cockroach_cloud_list_clusters_pagination_sort_order import CockroachCloudListClustersPaginationSortOrder
-from ...models.list_clusters_response import ListClustersResponse
+from ...models.cockroach_cloud_list_sql_users_pagination_sort_order import CockroachCloudListSQLUsersPaginationSortOrder
+from ...models.list_sql_users_response import ListSQLUsersResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
+    cluster_id: str,
     *,
     client: Client,
-    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
+    pagination_sort_order: Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters".format(client.base_url)
+    url = "{}/api/v1/clusters/{cluster_id}/sql-users".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["show_inactive"] = show_inactive
-
     params["pagination.page"] = pagination_page
 
     params["pagination.limit"] = pagination_limit
 
     json_pagination_as_of_time: Union[Unset, None, str] = UNSET
     if not isinstance(pagination_as_of_time, Unset):
         json_pagination_as_of_time = pagination_as_of_time.isoformat() if pagination_as_of_time else None
@@ -48,211 +44,191 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ListClustersResponse]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = ListClustersResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ListSQLUsersResponse]]:
+    if response.status_code == 200:
+        response_200 = ListSQLUsersResponse.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ListClustersResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, ListSQLUsersResponse]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    cluster_id: str,
     *,
     client: Client,
-    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
-) -> Response[Union[Any, ListClustersResponse]]:
-    """List clusters owned by an organization
+    pagination_sort_order: Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder] = UNSET,
+) -> Response[Union[Any, ListSQLUsersResponse]]:
+    """List SQL users for a cluster.
 
-     Sort order: Cluster name
+     Sort order: Username
 
     Args:
-        show_inactive (Union[Unset, None, bool]):  Default: True.
+        cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder]):
 
     Returns:
-        Response[Union[Any, ListClustersResponse]]
+        Response[Union[Any, ListSQLUsersResponse]]
     """
 
     kwargs = _get_kwargs(
+        cluster_id=cluster_id,
         client=client,
-        show_inactive=show_inactive,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
+    cluster_id: str,
     *,
     client: Client,
-    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
-) -> Optional[Union[Any, ListClustersResponse]]:
-    """List clusters owned by an organization
+    pagination_sort_order: Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder] = UNSET,
+) -> Optional[Union[Any, ListSQLUsersResponse]]:
+    """List SQL users for a cluster.
 
-     Sort order: Cluster name
+     Sort order: Username
 
     Args:
-        show_inactive (Union[Unset, None, bool]):  Default: True.
+        cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder]):
 
     Returns:
-        Union[Any, ListClustersResponse]
+        Response[Union[Any, ListSQLUsersResponse]]
     """
 
     return sync_detailed(
+        cluster_id=cluster_id,
         client=client,
-        show_inactive=show_inactive,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     ).parsed
 
 
 async def asyncio_detailed(
+    cluster_id: str,
     *,
     client: Client,
-    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
-) -> Response[Union[Any, ListClustersResponse]]:
-    """List clusters owned by an organization
+    pagination_sort_order: Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder] = UNSET,
+) -> Response[Union[Any, ListSQLUsersResponse]]:
+    """List SQL users for a cluster.
 
-     Sort order: Cluster name
+     Sort order: Username
 
     Args:
-        show_inactive (Union[Unset, None, bool]):  Default: True.
+        cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder]):
 
     Returns:
-        Response[Union[Any, ListClustersResponse]]
+        Response[Union[Any, ListSQLUsersResponse]]
     """
 
     kwargs = _get_kwargs(
+        cluster_id=cluster_id,
         client=client,
-        show_inactive=show_inactive,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
+    cluster_id: str,
     *,
     client: Client,
-    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
-) -> Optional[Union[Any, ListClustersResponse]]:
-    """List clusters owned by an organization
+    pagination_sort_order: Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder] = UNSET,
+) -> Optional[Union[Any, ListSQLUsersResponse]]:
+    """List SQL users for a cluster.
 
-     Sort order: Cluster name
+     Sort order: Username
 
     Args:
-        show_inactive (Union[Unset, None, bool]):  Default: True.
+        cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListSQLUsersPaginationSortOrder]):
 
     Returns:
-        Union[Any, ListClustersResponse]
+        Response[Union[Any, ListSQLUsersResponse]]
     """
 
     return (
         await asyncio_detailed(
+            cluster_id=cluster_id,
             client=client,
-            show_inactive=show_inactive,
             pagination_page=pagination_page,
             pagination_limit=pagination_limit,
             pagination_as_of_time=pagination_as_of_time,
             pagination_sort_order=pagination_sort_order,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_databases.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_databases.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import datetime
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
 from ...models.cockroach_cloud_list_databases_pagination_sort_order import (
     CockroachCloudListDatabasesPaginationSortOrder,
 )
 from ...models.list_databases_response import ListDatabasesResponse
 from ...types import UNSET, Response, Unset
 
@@ -48,79 +46,71 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ListDatabasesResponse]]:
-    if response.status_code == HTTPStatus.OK:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ListDatabasesResponse]]:
+    if response.status_code == 200:
         response_200 = ListDatabasesResponse.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ListDatabasesResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, ListDatabasesResponse]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListDatabasesPaginationSortOrder] = UNSET,
 ) -> Response[Union[Any, ListDatabasesResponse]]:
-    """List databases for a cluster
+    """List databases for a cluster.
 
      Sort order: Database name ascending
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListDatabasesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, ListDatabasesResponse]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
@@ -131,44 +121,40 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListDatabasesPaginationSortOrder] = UNSET,
 ) -> Optional[Union[Any, ListDatabasesResponse]]:
-    """List databases for a cluster
+    """List databases for a cluster.
 
      Sort order: Database name ascending
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListDatabasesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, ListDatabasesResponse]
+        Response[Union[Any, ListDatabasesResponse]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
@@ -182,30 +168,26 @@
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListDatabasesPaginationSortOrder] = UNSET,
 ) -> Response[Union[Any, ListDatabasesResponse]]:
-    """List databases for a cluster
+    """List databases for a cluster.
 
      Sort order: Database name ascending
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListDatabasesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
         Response[Union[Any, ListDatabasesResponse]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
@@ -214,44 +196,40 @@
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
     pagination_sort_order: Union[Unset, None, CockroachCloudListDatabasesPaginationSortOrder] = UNSET,
 ) -> Optional[Union[Any, ListDatabasesResponse]]:
-    """List databases for a cluster
+    """List databases for a cluster.
 
      Sort order: Database name ascending
 
     Args:
         cluster_id (str):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
             CockroachCloudListDatabasesPaginationSortOrder]):
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
     Returns:
-        Union[Any, ListDatabasesResponse]
+        Response[Union[Any, ListDatabasesResponse]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
             pagination_page=pagination_page,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_egress_rules.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_cluster_nodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import datetime
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cockroach_cloud_list_egress_rules_pagination_sort_order import (
-    CockroachCloudListEgressRulesPaginationSortOrder,
+from ...models.cockroach_cloud_list_cluster_nodes_pagination_sort_order import (
+    CockroachCloudListClusterNodesPaginationSortOrder,
 )
-from ...models.list_egress_rules_response import ListEgressRulesResponse
+from ...models.list_cluster_nodes_response import ListClusterNodesResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     cluster_id: str,
     *,
     client: Client,
+    region_name: Union[Unset, None, str] = UNSET,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListEgressRulesPaginationSortOrder] = UNSET,
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClusterNodesPaginationSortOrder] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/clusters/{cluster_id}/networking/egress-rules".format(client.base_url, cluster_id=cluster_id)
+    url = "{}/api/v1/clusters/{cluster_id}/nodes".format(client.base_url, cluster_id=cluster_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
+    params["region_name"] = region_name
+
     params["pagination.page"] = pagination_page
 
     params["pagination.limit"] = pagination_limit
 
     json_pagination_as_of_time: Union[Unset, None, str] = UNSET
     if not isinstance(pagination_as_of_time, Unset):
         json_pagination_as_of_time = pagination_as_of_time.isoformat() if pagination_as_of_time else None
@@ -48,215 +49,207 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ListEgressRulesResponse]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = ListEgressRulesResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ListClusterNodesResponse]]:
+    if response.status_code == 200:
+        response_200 = ListClusterNodesResponse.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ListEgressRulesResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, ListClusterNodesResponse]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     cluster_id: str,
     *,
     client: Client,
+    region_name: Union[Unset, None, str] = UNSET,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListEgressRulesPaginationSortOrder] = UNSET,
-) -> Response[Union[Any, ListEgressRulesResponse]]:
-    """List all egress rules associates with a cluster
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClusterNodesPaginationSortOrder] = UNSET,
+) -> Response[Union[Any, ListClusterNodesResponse]]:
+    """List nodes for a cluster.
 
-     Sort order: Name
+     Sort order: Region name, node name
 
     Args:
         cluster_id (str):
+        region_name (Union[Unset, None, str]):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
-            CockroachCloudListEgressRulesPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+            CockroachCloudListClusterNodesPaginationSortOrder]):
 
     Returns:
-        Response[Union[Any, ListEgressRulesResponse]]
+        Response[Union[Any, ListClusterNodesResponse]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        region_name=region_name,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     cluster_id: str,
     *,
     client: Client,
+    region_name: Union[Unset, None, str] = UNSET,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListEgressRulesPaginationSortOrder] = UNSET,
-) -> Optional[Union[Any, ListEgressRulesResponse]]:
-    """List all egress rules associates with a cluster
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClusterNodesPaginationSortOrder] = UNSET,
+) -> Optional[Union[Any, ListClusterNodesResponse]]:
+    """List nodes for a cluster.
 
-     Sort order: Name
+     Sort order: Region name, node name
 
     Args:
         cluster_id (str):
+        region_name (Union[Unset, None, str]):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
-            CockroachCloudListEgressRulesPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+            CockroachCloudListClusterNodesPaginationSortOrder]):
 
     Returns:
-        Union[Any, ListEgressRulesResponse]
+        Response[Union[Any, ListClusterNodesResponse]]
     """
 
     return sync_detailed(
         cluster_id=cluster_id,
         client=client,
+        region_name=region_name,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     ).parsed
 
 
 async def asyncio_detailed(
     cluster_id: str,
     *,
     client: Client,
+    region_name: Union[Unset, None, str] = UNSET,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListEgressRulesPaginationSortOrder] = UNSET,
-) -> Response[Union[Any, ListEgressRulesResponse]]:
-    """List all egress rules associates with a cluster
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClusterNodesPaginationSortOrder] = UNSET,
+) -> Response[Union[Any, ListClusterNodesResponse]]:
+    """List nodes for a cluster.
 
-     Sort order: Name
+     Sort order: Region name, node name
 
     Args:
         cluster_id (str):
+        region_name (Union[Unset, None, str]):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
-            CockroachCloudListEgressRulesPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+            CockroachCloudListClusterNodesPaginationSortOrder]):
 
     Returns:
-        Response[Union[Any, ListEgressRulesResponse]]
+        Response[Union[Any, ListClusterNodesResponse]]
     """
 
     kwargs = _get_kwargs(
         cluster_id=cluster_id,
         client=client,
+        region_name=region_name,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     cluster_id: str,
     *,
     client: Client,
+    region_name: Union[Unset, None, str] = UNSET,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListEgressRulesPaginationSortOrder] = UNSET,
-) -> Optional[Union[Any, ListEgressRulesResponse]]:
-    """List all egress rules associates with a cluster
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClusterNodesPaginationSortOrder] = UNSET,
+) -> Optional[Union[Any, ListClusterNodesResponse]]:
+    """List nodes for a cluster.
 
-     Sort order: Name
+     Sort order: Region name, node name
 
     Args:
         cluster_id (str):
+        region_name (Union[Unset, None, str]):
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
         pagination_sort_order (Union[Unset, None,
-            CockroachCloudListEgressRulesPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+            CockroachCloudListClusterNodesPaginationSortOrder]):
 
     Returns:
-        Union[Any, ListEgressRulesResponse]
+        Response[Union[Any, ListClusterNodesResponse]]
     """
 
     return (
         await asyncio_detailed(
             cluster_id=cluster_id,
             client=client,
+            region_name=region_name,
             pagination_page=pagination_page,
             pagination_limit=pagination_limit,
             pagination_as_of_time=pagination_as_of_time,
             pagination_sort_order=pagination_sort_order,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_role_grants.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/api/cockroach_cloud/cockroach_cloud_list_clusters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import datetime
-from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ... import errors
 from ...client import Client
-from ...models.cockroach_cloud_list_role_grants_pagination_sort_order import (
-    CockroachCloudListRoleGrantsPaginationSortOrder,
-)
-from ...models.list_role_grants_response_contains_a_representation_of_all_roles import (
-    ListRoleGrantsResponseContainsARepresentationOfAllRoles,
-)
+from ...models.cockroach_cloud_list_clusters_pagination_sort_order import CockroachCloudListClustersPaginationSortOrder
+from ...models.list_clusters_response import ListClustersResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: Client,
+    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListRoleGrantsPaginationSortOrder] = UNSET,
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/roles".format(client.base_url)
+    url = "{}/api/v1/clusters".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
+    params["show_inactive"] = show_inactive
+
     params["pagination.page"] = pagination_page
 
     params["pagination.limit"] = pagination_limit
 
     json_pagination_as_of_time: Union[Unset, None, str] = UNSET
     if not isinstance(pagination_as_of_time, Unset):
         json_pagination_as_of_time = pagination_as_of_time.isoformat() if pagination_as_of_time else None
@@ -49,199 +46,191 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = ListRoleGrantsResponseContainsARepresentationOfAllRoles.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ListClustersResponse]]:
+    if response.status_code == 200:
+        response_200 = ListClustersResponse.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
+    if response.status_code == 400:
         response_400 = cast(Any, response.json())
         return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
+    if response.status_code == 401:
         response_401 = cast(Any, response.json())
         return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
+    if response.status_code == 403:
         response_403 = cast(Any, response.json())
         return response_403
-    if response.status_code == HTTPStatus.NOT_FOUND:
+    if response.status_code == 404:
         response_404 = cast(Any, response.json())
         return response_404
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+    if response.status_code == 500:
         response_500 = cast(Any, response.json())
         return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    return None
 
 
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, ListClustersResponse]]:
     return Response(
-        status_code=HTTPStatus(response.status_code),
+        status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
+    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListRoleGrantsPaginationSortOrder] = UNSET,
-) -> Response[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]:
-    """Lists all RoleGrants
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
+) -> Response[Union[Any, ListClustersResponse]]:
+    """List clusters owned by an organization.
+
+     Sort order: Cluster name
 
     Args:
+        show_inactive (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None,
-            CockroachCloudListRoleGrantsPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
 
     Returns:
-        Response[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]
+        Response[Union[Any, ListClustersResponse]]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        show_inactive=show_inactive,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
+    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListRoleGrantsPaginationSortOrder] = UNSET,
-) -> Optional[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]:
-    """Lists all RoleGrants
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
+) -> Optional[Union[Any, ListClustersResponse]]:
+    """List clusters owned by an organization.
+
+     Sort order: Cluster name
 
     Args:
+        show_inactive (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None,
-            CockroachCloudListRoleGrantsPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
 
     Returns:
-        Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]
+        Response[Union[Any, ListClustersResponse]]
     """
 
     return sync_detailed(
         client=client,
+        show_inactive=show_inactive,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
+    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListRoleGrantsPaginationSortOrder] = UNSET,
-) -> Response[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]:
-    """Lists all RoleGrants
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
+) -> Response[Union[Any, ListClustersResponse]]:
+    """List clusters owned by an organization.
+
+     Sort order: Cluster name
 
     Args:
+        show_inactive (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None,
-            CockroachCloudListRoleGrantsPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
 
     Returns:
-        Response[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]
+        Response[Union[Any, ListClustersResponse]]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        show_inactive=show_inactive,
         pagination_page=pagination_page,
         pagination_limit=pagination_limit,
         pagination_as_of_time=pagination_as_of_time,
         pagination_sort_order=pagination_sort_order,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
+    show_inactive: Union[Unset, None, bool] = True,
     pagination_page: Union[Unset, None, str] = UNSET,
     pagination_limit: Union[Unset, None, int] = UNSET,
     pagination_as_of_time: Union[Unset, None, datetime.datetime] = UNSET,
-    pagination_sort_order: Union[Unset, None, CockroachCloudListRoleGrantsPaginationSortOrder] = UNSET,
-) -> Optional[Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]]:
-    """Lists all RoleGrants
+    pagination_sort_order: Union[Unset, None, CockroachCloudListClustersPaginationSortOrder] = UNSET,
+) -> Optional[Union[Any, ListClustersResponse]]:
+    """List clusters owned by an organization.
+
+     Sort order: Cluster name
 
     Args:
+        show_inactive (Union[Unset, None, bool]):  Default: True.
         pagination_page (Union[Unset, None, str]):
         pagination_limit (Union[Unset, None, int]):
         pagination_as_of_time (Union[Unset, None, datetime.datetime]):
-        pagination_sort_order (Union[Unset, None,
-            CockroachCloudListRoleGrantsPaginationSortOrder]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+        pagination_sort_order (Union[Unset, None, CockroachCloudListClustersPaginationSortOrder]):
 
     Returns:
-        Union[Any, ListRoleGrantsResponseContainsARepresentationOfAllRoles]
+        Response[Union[Any, ListClustersResponse]]
     """
 
     return (
         await asyncio_detailed(
             client=client,
+            show_inactive=show_inactive,
             pagination_page=pagination_page,
             pagination_limit=pagination_limit,
             pagination_as_of_time=pagination_as_of_time,
             pagination_sort_order=pagination_sort_order,
         )
     ).parsed
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/add_egress_rule_response.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/allowlist_entry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,82 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.egress_rule import EgressRule
-
-
-T = TypeVar("T", bound="AddEgressRuleResponse")
+T = TypeVar("T", bound="AllowlistEntry")
 
 
 @attr.s(auto_attribs=True)
-class AddEgressRuleResponse:
-    """AddEgressRuleResponse is the response message of the AddEgressRule RPC.
+class AllowlistEntry:
+    """
+    Example:
+        {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'ui': True, 'sql': True, 'name': 'Example'}
 
     Attributes:
-        rule (Union[Unset, EgressRule]): EgressRule represents a network egress rule.
+        cidr_ip (str):
+        cidr_mask (int):
+        ui (bool):
+        sql (bool):
+        name (Union[Unset, str]):
     """
 
-    rule: Union[Unset, "EgressRule"] = UNSET
+    cidr_ip: str
+    cidr_mask: int
+    ui: bool
+    sql: bool
+    name: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        rule: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.rule, Unset):
-            rule = self.rule.to_dict()
+        cidr_ip = self.cidr_ip
+        cidr_mask = self.cidr_mask
+        ui = self.ui
+        sql = self.sql
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if rule is not UNSET:
-            field_dict["Rule"] = rule
+        field_dict.update(
+            {
+                "cidr_ip": cidr_ip,
+                "cidr_mask": cidr_mask,
+                "ui": ui,
+                "sql": sql,
+            }
+        )
+        if name is not UNSET:
+            field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.egress_rule import EgressRule
-
         d = src_dict.copy()
-        _rule = d.pop("Rule", UNSET)
-        rule: Union[Unset, EgressRule]
-        if _rule is None:
-            rule = None
-        if isinstance(_rule, Unset):
-            rule = UNSET
-        else:
-            rule = EgressRule.from_dict(_rule)
+        cidr_ip = d.pop("cidr_ip")
+
+        cidr_mask = d.pop("cidr_mask")
+
+        ui = d.pop("ui")
+
+        sql = d.pop("sql")
+
+        name = d.pop("name", UNSET)
 
-        add_egress_rule_response = cls(
-            rule=rule,
+        allowlist_entry = cls(
+            cidr_ip=cidr_ip,
+            cidr_mask=cidr_mask,
+            ui=ui,
+            sql=sql,
+            name=name,
         )
 
-        add_egress_rule_response.additional_properties = d
-        return add_egress_rule_response
+        allowlist_entry.additional_properties = d
+        return allowlist_entry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/allowlist_entry.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_add_allowlist_entry_2_allowlist_entry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,68 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AllowlistEntry")
+T = TypeVar("T", bound="CockroachCloudAddAllowlistEntry2AllowlistEntry")
 
 
 @attr.s(auto_attribs=True)
-class AllowlistEntry:
+class CockroachCloudAddAllowlistEntry2AllowlistEntry:
     """
     Example:
-        {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'name': 'Example', 'sql': True, 'ui': True}
+        {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'ui': True, 'sql': True, 'name': 'Example'}
 
     Attributes:
-        cidr_ip (str):
-        cidr_mask (int):
-        sql (bool):
         ui (bool):
+        sql (bool):
         name (Union[Unset, str]):
     """
 
-    cidr_ip: str
-    cidr_mask: int
-    sql: bool
     ui: bool
+    sql: bool
     name: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cidr_ip = self.cidr_ip
-        cidr_mask = self.cidr_mask
-        sql = self.sql
         ui = self.ui
+        sql = self.sql
         name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "cidr_ip": cidr_ip,
-                "cidr_mask": cidr_mask,
-                "sql": sql,
                 "ui": ui,
+                "sql": sql,
             }
         )
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cidr_ip = d.pop("cidr_ip")
-
-        cidr_mask = d.pop("cidr_mask")
+        ui = d.pop("ui")
 
         sql = d.pop("sql")
 
-        ui = d.pop("ui")
-
         name = d.pop("name", UNSET)
 
-        allowlist_entry = cls(
-            cidr_ip=cidr_ip,
-            cidr_mask=cidr_mask,
-            sql=sql,
+        cockroach_cloud_add_allowlist_entry_2_allowlist_entry = cls(
             ui=ui,
+            sql=sql,
             name=name,
         )
 
-        allowlist_entry.additional_properties = d
-        return allowlist_entry
+        cockroach_cloud_add_allowlist_entry_2_allowlist_entry.additional_properties = d
+        return cockroach_cloud_add_allowlist_entry_2_allowlist_entry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/any_.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/any_.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,46 +30,43 @@
         Foo foo = ...;
         Any any = Any.pack(foo);
         ...
         if (any.is(Foo.class)) {
           foo = any.unpack(Foo.class);
         }
 
-    Example 3: Pack and unpack a message in Python.
+     Example 3: Pack and unpack a message in Python.
 
         foo = Foo(...)
         any = Any()
         any.Pack(foo)
         ...
         if any.Is(Foo.DESCRIPTOR):
           any.Unpack(foo)
           ...
 
-    Example 4: Pack and unpack a message in Go
+     Example 4: Pack and unpack a message in Go
 
          foo := &pb.Foo{...}
-         any, err := anypb.New(foo)
-         if err != nil {
-           ...
-         }
+         any, err := ptypes.MarshalAny(foo)
          ...
          foo := &pb.Foo{}
-         if err := any.UnmarshalTo(foo); err != nil {
+         if err := ptypes.UnmarshalAny(any, foo); err != nil {
            ...
          }
 
     The pack methods provided by protobuf library will by default use
     'type.googleapis.com/full.type.name' as the type URL and the unpack
     methods only use the fully qualified type name after the last '/'
     in the type URL, for example "foo.bar.com/x/y.z" will yield type
     name "y.z".
 
 
     JSON
-
+    ====
     The JSON representation of an `Any` value uses the regular
     representation of the deserialized, embedded message, with an
     additional field `@type` which contains the type URL. Example:
 
         package google.profile;
         message Person {
           string first_name = 1;
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/aws_endpoint_connection.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/aws_endpoint_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.aws_endpoint_connection_status_type import AWSEndpointConnectionStatusType
-from ..models.cloud_provider_type import CloudProviderType
+from ..models.api_cloud_provider import ApiCloudProvider
+from ..models.aws_endpoint_connection_status import AWSEndpointConnectionStatus
 
 T = TypeVar("T", bound="AwsEndpointConnection")
 
 
 @attr.s(auto_attribs=True)
 class AwsEndpointConnection:
     """
     Attributes:
-        cloud_provider (CloudProviderType):  - GCP: The Google Cloud Platform cloud provider.
+        region_name (str): RegionName is the cloud provider region name (i.e. us-east-1).
+        cloud_provider (ApiCloudProvider):  - GCP: The Google Cloud Platform cloud provider.
              - AWS: The Amazon Web Services cloud provider.
-        endpoint_id (str): endpoint_id is the client side of the PrivateLink connection.
-        region_name (str): region_name is the cloud provider region name (i.e. us-east-1).
-        service_id (str): service_id is the server side of the PrivateLink
+        status (AWSEndpointConnectionStatus): The statuses map to the statuses returned by the AWS API.
+        endpoint_id (str): EndpointID is the client side of the PrivateLink connection.
+        service_id (str): ServiceID is the server side of the PrivateLink
             connection. This is the same as AWSPrivateLinkEndpoint.service_id.
-        status (AWSEndpointConnectionStatusType):
     """
 
-    cloud_provider: CloudProviderType
-    endpoint_id: str
     region_name: str
+    cloud_provider: ApiCloudProvider
+    status: AWSEndpointConnectionStatus
+    endpoint_id: str
     service_id: str
-    status: AWSEndpointConnectionStatusType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        region_name = self.region_name
         cloud_provider = self.cloud_provider.value
 
+        status = self.status.value
+
         endpoint_id = self.endpoint_id
-        region_name = self.region_name
         service_id = self.service_id
-        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "region_name": region_name,
                 "cloud_provider": cloud_provider,
+                "status": status,
                 "endpoint_id": endpoint_id,
-                "region_name": region_name,
                 "service_id": service_id,
-                "status": status,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cloud_provider = CloudProviderType(d.pop("cloud_provider"))
+        region_name = d.pop("region_name")
 
-        endpoint_id = d.pop("endpoint_id")
+        cloud_provider = ApiCloudProvider(d.pop("cloud_provider"))
 
-        region_name = d.pop("region_name")
+        status = AWSEndpointConnectionStatus(d.pop("status"))
 
-        service_id = d.pop("service_id")
+        endpoint_id = d.pop("endpoint_id")
 
-        status = AWSEndpointConnectionStatusType(d.pop("status"))
+        service_id = d.pop("service_id")
 
         aws_endpoint_connection = cls(
+            region_name=region_name,
             cloud_provider=cloud_provider,
+            status=status,
             endpoint_id=endpoint_id,
-            region_name=region_name,
             service_id=service_id,
-            status=status,
         )
 
         aws_endpoint_connection.additional_properties = d
         return aws_endpoint_connection
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/aws_endpoint_connections.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/aws_endpoint_connections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.aws_endpoint_connection import AwsEndpointConnection
-
+from ..models.aws_endpoint_connection import AwsEndpointConnection
 
 T = TypeVar("T", bound="AwsEndpointConnections")
 
 
 @attr.s(auto_attribs=True)
 class AwsEndpointConnections:
     """
     Attributes:
-        connections (List['AwsEndpointConnection']): Connections is a list of private endpoints.
+        connections (List[AwsEndpointConnection]): Connections is a list of private endpoints.
     """
 
-    connections: List["AwsEndpointConnection"]
+    connections: List[AwsEndpointConnection]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         connections = []
         for connections_item_data in self.connections:
             connections_item = connections_item_data.to_dict()
 
@@ -34,16 +32,14 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.aws_endpoint_connection import AwsEndpointConnection
-
         d = src_dict.copy()
         connections = []
         _connections = d.pop("connections")
         for connections_item_data in _connections:
             connections_item = AwsEndpointConnection.from_dict(connections_item_data)
 
             connections.append(connections_item)
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/aws_private_link_service_detail.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/aws_private_link_service_detail.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,58 +5,57 @@
 T = TypeVar("T", bound="AWSPrivateLinkServiceDetail")
 
 
 @attr.s(auto_attribs=True)
 class AWSPrivateLinkServiceDetail:
     """
     Attributes:
-        availability_zone_ids (List[str]): availability_zone_ids are the identifiers for the availability zones
-            that the service is available in.
-        service_id (str): service_id is the server side of the PrivateLink
+        service_name (str): ServiceName is the AWS service name customers use to create endpoints on their end.
+        service_id (str): ServiceID is the server side of the PrivateLink
             connection. This is the same as AWSPrivateLinkEndpoint.service_id.
-        service_name (str): service_name is the AWS service name customers use to create endpoints
-            on their end.
+        availability_zone_ids (List[str]): AvailabilityZoneIDs are the identifiers for the availability zones that the
+            service
+            is available in.
     """
 
-    availability_zone_ids: List[str]
-    service_id: str
     service_name: str
+    service_id: str
+    availability_zone_ids: List[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        availability_zone_ids = self.availability_zone_ids
-
-        service_id = self.service_id
         service_name = self.service_name
+        service_id = self.service_id
+        availability_zone_ids = self.availability_zone_ids
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "availability_zone_ids": availability_zone_ids,
-                "service_id": service_id,
                 "service_name": service_name,
+                "service_id": service_id,
+                "availability_zone_ids": availability_zone_ids,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        availability_zone_ids = cast(List[str], d.pop("availability_zone_ids"))
+        service_name = d.pop("service_name")
 
         service_id = d.pop("service_id")
 
-        service_name = d.pop("service_name")
+        availability_zone_ids = cast(List[str], d.pop("availability_zone_ids"))
 
         aws_private_link_service_detail = cls(
-            availability_zone_ids=availability_zone_ids,
-            service_id=service_id,
             service_name=service_name,
+            service_id=service_id,
+            availability_zone_ids=availability_zone_ids,
         )
 
         aws_private_link_service_detail.additional_properties = d
         return aws_private_link_service_detail
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/built_in_role.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/serverless_cluster_create_specification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,58 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
-from ..models.organization_user_role_type import OrganizationUserRoleType
-
-if TYPE_CHECKING:
-    from ..models.resource import Resource
-
-
-T = TypeVar("T", bound="BuiltInRole")
+T = TypeVar("T", bound="ServerlessClusterCreateSpecification")
 
 
 @attr.s(auto_attribs=True)
-class BuiltInRole:
+class ServerlessClusterCreateSpecification:
     """
     Attributes:
-        name (OrganizationUserRoleType):
-        resource (Resource):
+        regions (List[str]): Region values should match the cloud provider's zone code.
+            For example, for Oregon, set region_name to "us-west2" for
+            GCP and "us-west-2" for AWS.
+        spend_limit (int):
     """
 
-    name: OrganizationUserRoleType
-    resource: "Resource"
+    regions: List[str]
+    spend_limit: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name.value
+        regions = self.regions
 
-        resource = self.resource.to_dict()
+        spend_limit = self.spend_limit
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "name": name,
-                "resource": resource,
+                "regions": regions,
+                "spend_limit": spend_limit,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.resource import Resource
-
         d = src_dict.copy()
-        name = OrganizationUserRoleType(d.pop("name"))
+        regions = cast(List[str], d.pop("regions"))
 
-        resource = Resource.from_dict(d.pop("resource"))
+        spend_limit = d.pop("spend_limit")
 
-        built_in_role = cls(
-            name=name,
-            resource=resource,
+        serverless_cluster_create_specification = cls(
+            regions=regions,
+            spend_limit=spend_limit,
         )
 
-        built_in_role.additional_properties = d
-        return built_in_role
+        serverless_cluster_create_specification.additional_properties = d
+        return serverless_cluster_create_specification
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cloud_provider_region.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cloud_provider_region.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.cloud_provider_type import CloudProviderType
+from ..models.api_cloud_provider import ApiCloudProvider
 
 T = TypeVar("T", bound="CloudProviderRegion")
 
 
 @attr.s(auto_attribs=True)
 class CloudProviderRegion:
     """
     Attributes:
-        distance (float): Distance in miles, based on client IP address.
-        location (str):
         name (str):
-        provider (CloudProviderType):  - GCP: The Google Cloud Platform cloud provider.
+        location (str):
+        provider (ApiCloudProvider):  - GCP: The Google Cloud Platform cloud provider.
              - AWS: The Amazon Web Services cloud provider.
         serverless (bool):
+        distance (float):
     """
 
-    distance: float
-    location: str
     name: str
-    provider: CloudProviderType
+    location: str
+    provider: ApiCloudProvider
     serverless: bool
+    distance: float
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        distance = self.distance
-        location = self.location
         name = self.name
+        location = self.location
         provider = self.provider.value
 
         serverless = self.serverless
+        distance = self.distance
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "distance": distance,
-                "location": location,
                 "name": name,
+                "location": location,
                 "provider": provider,
                 "serverless": serverless,
+                "distance": distance,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        distance = d.pop("distance")
+        name = d.pop("name")
 
         location = d.pop("location")
 
-        name = d.pop("name")
-
-        provider = CloudProviderType(d.pop("provider"))
+        provider = ApiCloudProvider(d.pop("provider"))
 
         serverless = d.pop("serverless")
 
+        distance = d.pop("distance")
+
         cloud_provider_region = cls(
-            distance=distance,
-            location=location,
             name=name,
+            location=location,
             provider=provider,
             serverless=serverless,
+            distance=distance,
         )
 
         cloud_provider_region.additional_properties = d
         return cloud_provider_region
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cloud_watch_metric_export_info.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/log_export_cluster_specification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,82 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.metric_export_status_type import MetricExportStatusType
+from ..models.log_export_type import LogExportType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CloudWatchMetricExportInfo")
+T = TypeVar("T", bound="LogExportClusterSpecification")
 
 
 @attr.s(auto_attribs=True)
-class CloudWatchMetricExportInfo:
-    """
-    Attributes:
-        cluster_id (str):
-        role_arn (str): role_arn is the IAM role used to upload metric segments to the
-            target AWS account.
-        log_group_name (Union[Unset, str]): log_group_name is the customized log group name.
-        status (Union[Unset, MetricExportStatusType]):
-        target_region (Union[Unset, str]): target_region specifies the specific AWS region that the metrics will
-            be exported to.
-        user_message (Union[Unset, str]):
+class LogExportClusterSpecification:
+    """LogExportClusterSpecification contains all the data necessary to
+    configure log export for an individual cluster. Users would supply
+    this data via the API and also receive it back when inspecting the
+    state of their log export configuration.
+
+        Attributes:
+            type (Union[Unset, LogExportType]): LogExportType encodes the cloud selection that we're exporting to
+                along with the cloud logging platform. Currently, each cloud has a
+                single logging platform.
+            log_name (Union[Unset, str]): log_name is an identifier for the logs in the customer's log sink.
+            auth_principal (Union[Unset, str]): auth_principal is either the AWS Role ARN that identifies a role
+                that the cluster account can assume to write to CloudWatch or the
+                GCP Project ID that the cluster service account has permissions to
+                write to for cloud logging.
     """
 
-    cluster_id: str
-    role_arn: str
-    log_group_name: Union[Unset, str] = UNSET
-    status: Union[Unset, MetricExportStatusType] = UNSET
-    target_region: Union[Unset, str] = UNSET
-    user_message: Union[Unset, str] = UNSET
+    type: Union[Unset, LogExportType] = UNSET
+    log_name: Union[Unset, str] = UNSET
+    auth_principal: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cluster_id = self.cluster_id
-        role_arn = self.role_arn
-        log_group_name = self.log_group_name
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        type: Union[Unset, str] = UNSET
+        if not isinstance(self.type, Unset):
+            type = self.type.value
 
-        target_region = self.target_region
-        user_message = self.user_message
+        log_name = self.log_name
+        auth_principal = self.auth_principal
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "cluster_id": cluster_id,
-                "role_arn": role_arn,
-            }
-        )
-        if log_group_name is not UNSET:
-            field_dict["log_group_name"] = log_group_name
-        if status is not UNSET:
-            field_dict["status"] = status
-        if target_region is not UNSET:
-            field_dict["target_region"] = target_region
-        if user_message is not UNSET:
-            field_dict["user_message"] = user_message
+        field_dict.update({})
+        if type is not UNSET:
+            field_dict["type"] = type
+        if log_name is not UNSET:
+            field_dict["log_name"] = log_name
+        if auth_principal is not UNSET:
+            field_dict["auth_principal"] = auth_principal
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cluster_id = d.pop("cluster_id")
-
-        role_arn = d.pop("role_arn")
-
-        log_group_name = d.pop("log_group_name", UNSET)
-
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, MetricExportStatusType]
-        if _status is None:
-            status = None
-        if isinstance(_status, Unset):
-            status = UNSET
+        _type = d.pop("type", UNSET)
+        type: Union[Unset, LogExportType]
+        if isinstance(_type, Unset):
+            type = UNSET
         else:
-            status = MetricExportStatusType(_status)
+            type = LogExportType(_type)
 
-        target_region = d.pop("target_region", UNSET)
+        log_name = d.pop("log_name", UNSET)
 
-        user_message = d.pop("user_message", UNSET)
+        auth_principal = d.pop("auth_principal", UNSET)
 
-        cloud_watch_metric_export_info = cls(
-            cluster_id=cluster_id,
-            role_arn=role_arn,
-            log_group_name=log_group_name,
-            status=status,
-            target_region=target_region,
-            user_message=user_message,
+        log_export_cluster_specification = cls(
+            type=type,
+            log_name=log_name,
+            auth_principal=auth_principal,
         )
 
-        cloud_watch_metric_export_info.additional_properties = d
-        return cloud_watch_metric_export_info
+        log_export_cluster_specification.additional_properties = d
+        return log_export_cluster_specification
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_config.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cluster_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.dedicated_hardware_config import DedicatedHardwareConfig
+from ..models.serverless_cluster_config import ServerlessClusterConfig
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.dedicated_hardware_config import DedicatedHardwareConfig
-    from ..models.serverless_cluster_config import ServerlessClusterConfig
-
-
 T = TypeVar("T", bound="ClusterConfig")
 
 
 @attr.s(auto_attribs=True)
 class ClusterConfig:
     """
     Attributes:
         dedicated (Union[Unset, DedicatedHardwareConfig]):
         serverless (Union[Unset, ServerlessClusterConfig]):
     """
 
-    dedicated: Union[Unset, "DedicatedHardwareConfig"] = UNSET
-    serverless: Union[Unset, "ServerlessClusterConfig"] = UNSET
+    dedicated: Union[Unset, DedicatedHardwareConfig] = UNSET
+    serverless: Union[Unset, ServerlessClusterConfig] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         dedicated: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.dedicated, Unset):
             dedicated = self.dedicated.to_dict()
 
@@ -41,31 +38,24 @@
         if serverless is not UNSET:
             field_dict["serverless"] = serverless
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dedicated_hardware_config import DedicatedHardwareConfig
-        from ..models.serverless_cluster_config import ServerlessClusterConfig
-
         d = src_dict.copy()
         _dedicated = d.pop("dedicated", UNSET)
         dedicated: Union[Unset, DedicatedHardwareConfig]
-        if _dedicated is None:
-            dedicated = None
         if isinstance(_dedicated, Unset):
             dedicated = UNSET
         else:
             dedicated = DedicatedHardwareConfig.from_dict(_dedicated)
 
         _serverless = d.pop("serverless", UNSET)
         serverless: Union[Unset, ServerlessClusterConfig]
-        if _serverless is None:
-            serverless = None
         if isinstance(_serverless, Unset):
             serverless = UNSET
         else:
             serverless = ServerlessClusterConfig.from_dict(_serverless)
 
         cluster_config = cls(
             dedicated=dedicated,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_major_version.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_cluster_update_specification_region_nodes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.cluster_major_version_support_status_type import ClusterMajorVersionSupportStatusType
-
-T = TypeVar("T", bound="ClusterMajorVersion")
+T = TypeVar("T", bound="DedicatedClusterUpdateSpecificationRegionNodes")
 
 
 @attr.s(auto_attribs=True)
-class ClusterMajorVersion:
-    """For more information about CockroachDB cluster version support, see
-    https://www.cockroachlabs.com/docs/releases/release-support-policy.html
-
-        Attributes:
-            support_status (ClusterMajorVersionSupportStatusType):
-            version (str):
+class DedicatedClusterUpdateSpecificationRegionNodes:
+    """Region keys should match the cloud provider's zone code.
+    For example, for Oregon, set region_name to "us-west2" for
+    GCP and "us-west-2" for AWS. Values represent the node count.
+
     """
 
-    support_status: ClusterMajorVersionSupportStatusType
-    version: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, int] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        support_status = self.support_status.value
-
-        version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "support_status": support_status,
-                "version": version,
-            }
-        )
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        support_status = ClusterMajorVersionSupportStatusType(d.pop("support_status"))
-
-        version = d.pop("version")
-
-        cluster_major_version = cls(
-            support_status=support_status,
-            version=version,
-        )
+        dedicated_cluster_update_specification_region_nodes = cls()
 
-        cluster_major_version.additional_properties = d
-        return cluster_major_version
+        dedicated_cluster_update_specification_region_nodes.additional_properties = d
+        return dedicated_cluster_update_specification_region_nodes
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> Any:
+    def __getitem__(self, key: str) -> int:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, key: str, value: int) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cluster_status_type.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cluster_status_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 from enum import Enum
 
 
 class ClusterStatusType(str, Enum):
-    CRDB_CLUSTER_DISRUPTION_FAILED = "CRDB_CLUSTER_DISRUPTION_FAILED"
-    CRDB_CLUSTER_DISRUPTION_RUNNING = "CRDB_CLUSTER_DISRUPTION_RUNNING"
-    CRDB_CMEK_OPERATION_FAILED = "CRDB_CMEK_OPERATION_FAILED"
-    CRDB_CMEK_OPERATION_RUNNING = "CRDB_CMEK_OPERATION_RUNNING"
-    CRDB_CUSTOM_CLIENT_CA_FAILED = "CRDB_CUSTOM_CLIENT_CA_FAILED"
-    CRDB_CUSTOM_CLIENT_CA_RUNNING = "CRDB_CUSTOM_CLIENT_CA_RUNNING"
-    CRDB_EDIT_CLUSTER_FAILED = "CRDB_EDIT_CLUSTER_FAILED"
-    CRDB_EDIT_CLUSTER_RUNNING = "CRDB_EDIT_CLUSTER_RUNNING"
-    CRDB_INSTANCE_UPDATE_FAILED = "CRDB_INSTANCE_UPDATE_FAILED"
-    CRDB_INSTANCE_UPDATE_RUNNING = "CRDB_INSTANCE_UPDATE_RUNNING"
-    CRDB_LOG_EXPORT_OPERATION_FAILED = "CRDB_LOG_EXPORT_OPERATION_FAILED"
-    CRDB_LOG_EXPORT_OPERATION_RUNNING = "CRDB_LOG_EXPORT_OPERATION_RUNNING"
-    CRDB_MAJOR_ROLLBACK_FAILED = "CRDB_MAJOR_ROLLBACK_FAILED"
-    CRDB_MAJOR_ROLLBACK_RUNNING = "CRDB_MAJOR_ROLLBACK_RUNNING"
-    CRDB_MAJOR_UPGRADE_FAILED = "CRDB_MAJOR_UPGRADE_FAILED"
+    CLUSTER_STATUS_UNSPECIFIED = "CLUSTER_STATUS_UNSPECIFIED"
     CRDB_MAJOR_UPGRADE_RUNNING = "CRDB_MAJOR_UPGRADE_RUNNING"
-    CRDB_PATCH_FAILED = "CRDB_PATCH_FAILED"
+    CRDB_MAJOR_UPGRADE_FAILED = "CRDB_MAJOR_UPGRADE_FAILED"
+    CRDB_MAJOR_ROLLBACK_RUNNING = "CRDB_MAJOR_ROLLBACK_RUNNING"
+    CRDB_MAJOR_ROLLBACK_FAILED = "CRDB_MAJOR_ROLLBACK_FAILED"
     CRDB_PATCH_RUNNING = "CRDB_PATCH_RUNNING"
-    CRDB_REPAVE_FAILED = "CRDB_REPAVE_FAILED"
-    CRDB_REPAVE_RUNNING = "CRDB_REPAVE_RUNNING"
-    CRDB_SCALE_FAILED = "CRDB_SCALE_FAILED"
+    CRDB_PATCH_FAILED = "CRDB_PATCH_FAILED"
     CRDB_SCALE_RUNNING = "CRDB_SCALE_RUNNING"
+    CRDB_SCALE_FAILED = "CRDB_SCALE_FAILED"
     MAINTENANCE_RUNNING = "MAINTENANCE_RUNNING"
-    TENANT_RESTORE_FAILED = "TENANT_RESTORE_FAILED"
+    CRDB_INSTANCE_UPDATE_RUNNING = "CRDB_INSTANCE_UPDATE_RUNNING"
+    CRDB_INSTANCE_UPDATE_FAILED = "CRDB_INSTANCE_UPDATE_FAILED"
+    CRDB_EDIT_CLUSTER_RUNNING = "CRDB_EDIT_CLUSTER_RUNNING"
+    CRDB_EDIT_CLUSTER_FAILED = "CRDB_EDIT_CLUSTER_FAILED"
+    CRDB_CMEK_OPERATION_RUNNING = "CRDB_CMEK_OPERATION_RUNNING"
+    CRDB_CMEK_OPERATION_FAILED = "CRDB_CMEK_OPERATION_FAILED"
     TENANT_RESTORE_RUNNING = "TENANT_RESTORE_RUNNING"
-    UNSPECIFIED = "UNSPECIFIED"
+    TENANT_RESTORE_FAILED = "TENANT_RESTORE_FAILED"
+    CRDB_LOG_EXPORT_OPERATION_RUNNING = "CRDB_LOG_EXPORT_OPERATION_RUNNING"
+    CRDB_LOG_EXPORT_OPERATION_FAILED = "CRDB_LOG_EXPORT_OPERATION_FAILED"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_cluster_info.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_cluster_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.cmek_region_info import CMEKRegionInfo
 from ..models.cmek_status import CMEKStatus
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cmek_region_info import CMEKRegionInfo
-
-
 T = TypeVar("T", bound="CMEKClusterInfo")
 
 
 @attr.s(auto_attribs=True)
 class CMEKClusterInfo:
     """CMEKClusterInfo contains the status of CMEK across an entire cluster,
     including within each one its regions.
 
         Attributes:
-            region_infos (Union[Unset, List['CMEKRegionInfo']]):
             status (Union[Unset, CMEKStatus]): CMEKStatus describes the current status of CMEK for an entire CRDB cluster
                 or a CMEK key within a region.
 
                  - UNKNOWN_STATUS: UNKNOWN should never be used; if it is used, it indicates a bug.
                  - DISABLED: DISABLED corresponds to the state of a cluster or region-level key when
                 CMEK has finished being disabled. By default, CMEK will be disabled for
                 new clusters.
@@ -43,67 +39,64 @@
                 a failure to update from one CMEK spec to another.
                  - REVOKED: REVOKED corresponds to the state of a cluster or region-level key when the
                 customer has revoked CockroachLab's permissions for their key.
                  - REVOKING: REVOKING corresponds to the state of a cluster or region-level key when
                 CMEK is in the process of being revoked.
                  - REVOKE_FAILED: REVOKE_FAILED corresponds to the state of a cluster or region-level key
                 when CMEK has failed to be revoked.
+            region_infos (Union[Unset, List[CMEKRegionInfo]]):
     """
 
-    region_infos: Union[Unset, List["CMEKRegionInfo"]] = UNSET
     status: Union[Unset, CMEKStatus] = UNSET
+    region_infos: Union[Unset, List[CMEKRegionInfo]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
+
         region_infos: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.region_infos, Unset):
             region_infos = []
             for region_infos_item_data in self.region_infos:
                 region_infos_item = region_infos_item_data.to_dict()
 
                 region_infos.append(region_infos_item)
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if region_infos is not UNSET:
-            field_dict["region_infos"] = region_infos
         if status is not UNSET:
             field_dict["status"] = status
+        if region_infos is not UNSET:
+            field_dict["region_infos"] = region_infos
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cmek_region_info import CMEKRegionInfo
-
         d = src_dict.copy()
-        region_infos = []
-        _region_infos = d.pop("region_infos", UNSET)
-        for region_infos_item_data in _region_infos or []:
-            region_infos_item = CMEKRegionInfo.from_dict(region_infos_item_data)
-
-            region_infos.append(region_infos_item)
-
         _status = d.pop("status", UNSET)
         status: Union[Unset, CMEKStatus]
-        if _status is None:
-            status = None
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CMEKStatus(_status)
 
+        region_infos = []
+        _region_infos = d.pop("region_infos", UNSET)
+        for region_infos_item_data in _region_infos or []:
+            region_infos_item = CMEKRegionInfo.from_dict(region_infos_item_data)
+
+            region_infos.append(region_infos_item)
+
         cmek_cluster_info = cls(
-            region_infos=region_infos,
             status=status,
+            region_infos=region_infos,
         )
 
         cmek_cluster_info.additional_properties = d
         return cmek_cluster_info
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_key_info.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_key_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.cmek_key_specification import CMEKKeySpecification
 from ..models.cmek_status import CMEKStatus
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cmek_key_specification import CMEKKeySpecification
-
-
 T = TypeVar("T", bound="CMEKKeyInfo")
 
 
 @attr.s(auto_attribs=True)
 class CMEKKeyInfo:
     """CMEKKeyInfo contains the status of a customer-provided key alongside the
     specification.
 
         Attributes:
-            created_at (Union[Unset, datetime.datetime]):
-            spec (Union[Unset, CMEKKeySpecification]): CMEKKeySpecification contains all the details necessary to use a
-                customer-provided
-                encryption key.
-
-                This involves the type/location of the key and the principal to authenticate as
-                when accessing it.
             status (Union[Unset, CMEKStatus]): CMEKStatus describes the current status of CMEK for an entire CRDB cluster
                 or a CMEK key within a region.
 
                  - UNKNOWN_STATUS: UNKNOWN should never be used; if it is used, it indicates a bug.
                  - DISABLED: DISABLED corresponds to the state of a cluster or region-level key when
                 CMEK has finished being disabled. By default, CMEK will be disabled for
                 new clusters.
@@ -51,109 +41,103 @@
                 a failure to update from one CMEK spec to another.
                  - REVOKED: REVOKED corresponds to the state of a cluster or region-level key when the
                 customer has revoked CockroachLab's permissions for their key.
                  - REVOKING: REVOKING corresponds to the state of a cluster or region-level key when
                 CMEK is in the process of being revoked.
                  - REVOKE_FAILED: REVOKE_FAILED corresponds to the state of a cluster or region-level key
                 when CMEK has failed to be revoked.
-            updated_at (Union[Unset, datetime.datetime]):
             user_message (Union[Unset, str]):
+            spec (Union[Unset, CMEKKeySpecification]): CMEKKeySpecification contains all the details necessary to use a
+                customer-provided
+                encryption key. This involves the type/location of the key and the principal
+                to authenticate as when accessing it.
+            created_at (Union[Unset, datetime.datetime]):
+            updated_at (Union[Unset, datetime.datetime]):
     """
 
-    created_at: Union[Unset, datetime.datetime] = UNSET
-    spec: Union[Unset, "CMEKKeySpecification"] = UNSET
     status: Union[Unset, CMEKStatus] = UNSET
-    updated_at: Union[Unset, datetime.datetime] = UNSET
     user_message: Union[Unset, str] = UNSET
+    spec: Union[Unset, CMEKKeySpecification] = UNSET
+    created_at: Union[Unset, datetime.datetime] = UNSET
+    updated_at: Union[Unset, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        created_at: Union[Unset, str] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat()
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
 
+        user_message = self.user_message
         spec: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.spec, Unset):
             spec = self.spec.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        created_at: Union[Unset, str] = UNSET
+        if not isinstance(self.created_at, Unset):
+            created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        user_message = self.user_message
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if spec is not UNSET:
-            field_dict["spec"] = spec
         if status is not UNSET:
             field_dict["status"] = status
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
         if user_message is not UNSET:
             field_dict["user_message"] = user_message
+        if spec is not UNSET:
+            field_dict["spec"] = spec
+        if created_at is not UNSET:
+            field_dict["created_at"] = created_at
+        if updated_at is not UNSET:
+            field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cmek_key_specification import CMEKKeySpecification
-
         d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
-        created_at: Union[Unset, datetime.datetime]
-        if _created_at is None:
-            created_at = None
-        if isinstance(_created_at, Unset):
-            created_at = UNSET
+        _status = d.pop("status", UNSET)
+        status: Union[Unset, CMEKStatus]
+        if isinstance(_status, Unset):
+            status = UNSET
         else:
-            created_at = isoparse(_created_at)
+            status = CMEKStatus(_status)
+
+        user_message = d.pop("user_message", UNSET)
 
         _spec = d.pop("spec", UNSET)
         spec: Union[Unset, CMEKKeySpecification]
-        if _spec is None:
-            spec = None
         if isinstance(_spec, Unset):
             spec = UNSET
         else:
             spec = CMEKKeySpecification.from_dict(_spec)
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, CMEKStatus]
-        if _status is None:
-            status = None
-        if isinstance(_status, Unset):
-            status = UNSET
+        _created_at = d.pop("created_at", UNSET)
+        created_at: Union[Unset, datetime.datetime]
+        if isinstance(_created_at, Unset):
+            created_at = UNSET
         else:
-            status = CMEKStatus(_status)
+            created_at = isoparse(_created_at)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
-        if _updated_at is None:
-            updated_at = None
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        user_message = d.pop("user_message", UNSET)
-
         cmek_key_info = cls(
-            created_at=created_at,
-            spec=spec,
             status=status,
-            updated_at=updated_at,
             user_message=user_message,
+            spec=spec,
+            created_at=created_at,
+            updated_at=updated_at,
         )
 
         cmek_key_info.additional_properties = d
         return cmek_key_info
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_key_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_enable_log_export_enable_log_export_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.cmek_key_type_enumerates_types_of_customer_managed_keys import (
-    CMEKKeyTypeEnumeratesTypesOfCustomerManagedKeys,
-)
+from ..models.log_export_type import LogExportType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CMEKKeySpecification")
+T = TypeVar("T", bound="CockroachCloudEnableLogExportEnableLogExportRequest")
 
 
 @attr.s(auto_attribs=True)
-class CMEKKeySpecification:
-    """CMEKKeySpecification contains all the details necessary to use a customer-provided
-    encryption key.
-
-    This involves the type/location of the key and the principal to authenticate as
-    when accessing it.
-
-        Attributes:
-            auth_principal (Union[Unset, str]):
-            type (Union[Unset, CMEKKeyTypeEnumeratesTypesOfCustomerManagedKeys]): - UNKNOWN_KEY_TYPE: UNKNOWN should never
-                be used; if it is used, it indicates a bug.
-            uri (Union[Unset, str]):
+class CockroachCloudEnableLogExportEnableLogExportRequest:
+    """
+    Attributes:
+        type (Union[Unset, LogExportType]): LogExportType encodes the cloud selection that we're exporting to
+            along with the cloud logging platform. Currently, each cloud has a
+            single logging platform.
+        log_name (Union[Unset, str]): log_name is an identifier for the logs in the customer's log sink.
+        auth_principal (Union[Unset, str]): auth_principal is either the AWS Role ARN that identifies a role
+            that the cluster account can assume to write to CloudWatch or the
+            GCP Project ID that the cluster service account has permissions to
+            write to for cloud logging.
     """
 
+    type: Union[Unset, LogExportType] = UNSET
+    log_name: Union[Unset, str] = UNSET
     auth_principal: Union[Unset, str] = UNSET
-    type: Union[Unset, CMEKKeyTypeEnumeratesTypesOfCustomerManagedKeys] = UNSET
-    uri: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        auth_principal = self.auth_principal
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
             type = self.type.value
 
-        uri = self.uri
+        log_name = self.log_name
+        auth_principal = self.auth_principal
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if auth_principal is not UNSET:
-            field_dict["auth_principal"] = auth_principal
         if type is not UNSET:
             field_dict["type"] = type
-        if uri is not UNSET:
-            field_dict["uri"] = uri
+        if log_name is not UNSET:
+            field_dict["log_name"] = log_name
+        if auth_principal is not UNSET:
+            field_dict["auth_principal"] = auth_principal
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        auth_principal = d.pop("auth_principal", UNSET)
-
         _type = d.pop("type", UNSET)
-        type: Union[Unset, CMEKKeyTypeEnumeratesTypesOfCustomerManagedKeys]
-        if _type is None:
-            type = None
+        type: Union[Unset, LogExportType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = CMEKKeyTypeEnumeratesTypesOfCustomerManagedKeys(_type)
+            type = LogExportType(_type)
 
-        uri = d.pop("uri", UNSET)
+        log_name = d.pop("log_name", UNSET)
 
-        cmek_key_specification = cls(
-            auth_principal=auth_principal,
+        auth_principal = d.pop("auth_principal", UNSET)
+
+        cockroach_cloud_enable_log_export_enable_log_export_request = cls(
             type=type,
-            uri=uri,
+            log_name=log_name,
+            auth_principal=auth_principal,
         )
 
-        cmek_key_specification.additional_properties = d
-        return cmek_key_specification
+        cockroach_cloud_enable_log_export_enable_log_export_request.additional_properties = d
+        return cockroach_cloud_enable_log_export_enable_log_export_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_region_info.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_region_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.cmek_key_info import CMEKKeyInfo
 from ..models.cmek_status import CMEKStatus
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cmek_key_info import CMEKKeyInfo
-
-
 T = TypeVar("T", bound="CMEKRegionInfo")
 
 
 @attr.s(auto_attribs=True)
 class CMEKRegionInfo:
-    """CMEKRegionInfo contains the status of CMEK within a region.
-
-    This includes current and past key specifications used within the region,
-    as well as the status of those specifications
+    """CMEKRegionInfo contains the status of CMEK within a region. This includes
+    current and past key specifications used within the region, as well as the
+    status of those specifications.
 
         Attributes:
-            key_infos (Union[Unset, List['CMEKKeyInfo']]):
             region (Union[Unset, str]):
             status (Union[Unset, CMEKStatus]): CMEKStatus describes the current status of CMEK for an entire CRDB cluster
                 or a CMEK key within a region.
 
                  - UNKNOWN_STATUS: UNKNOWN should never be used; if it is used, it indicates a bug.
                  - DISABLED: DISABLED corresponds to the state of a cluster or region-level key when
                 CMEK has finished being disabled. By default, CMEK will be disabled for
@@ -46,74 +41,71 @@
                 a failure to update from one CMEK spec to another.
                  - REVOKED: REVOKED corresponds to the state of a cluster or region-level key when the
                 customer has revoked CockroachLab's permissions for their key.
                  - REVOKING: REVOKING corresponds to the state of a cluster or region-level key when
                 CMEK is in the process of being revoked.
                  - REVOKE_FAILED: REVOKE_FAILED corresponds to the state of a cluster or region-level key
                 when CMEK has failed to be revoked.
+            key_infos (Union[Unset, List[CMEKKeyInfo]]):
     """
 
-    key_infos: Union[Unset, List["CMEKKeyInfo"]] = UNSET
     region: Union[Unset, str] = UNSET
     status: Union[Unset, CMEKStatus] = UNSET
+    key_infos: Union[Unset, List[CMEKKeyInfo]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        region = self.region
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
+
         key_infos: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.key_infos, Unset):
             key_infos = []
             for key_infos_item_data in self.key_infos:
                 key_infos_item = key_infos_item_data.to_dict()
 
                 key_infos.append(key_infos_item)
 
-        region = self.region
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if key_infos is not UNSET:
-            field_dict["key_infos"] = key_infos
         if region is not UNSET:
             field_dict["region"] = region
         if status is not UNSET:
             field_dict["status"] = status
+        if key_infos is not UNSET:
+            field_dict["key_infos"] = key_infos
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cmek_key_info import CMEKKeyInfo
-
         d = src_dict.copy()
-        key_infos = []
-        _key_infos = d.pop("key_infos", UNSET)
-        for key_infos_item_data in _key_infos or []:
-            key_infos_item = CMEKKeyInfo.from_dict(key_infos_item_data)
-
-            key_infos.append(key_infos_item)
-
         region = d.pop("region", UNSET)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, CMEKStatus]
-        if _status is None:
-            status = None
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CMEKStatus(_status)
 
+        key_infos = []
+        _key_infos = d.pop("key_infos", UNSET)
+        for key_infos_item_data in _key_infos or []:
+            key_infos_item = CMEKKeyInfo.from_dict(key_infos_item_data)
+
+            key_infos.append(key_infos_item)
+
         cmek_region_info = cls(
-            key_infos=key_infos,
             region=region,
             status=status,
+            key_infos=key_infos,
         )
 
         cmek_region_info.additional_properties = d
         return cmek_region_info
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cmek_region_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_region_specification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,65 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.cmek_key_specification import CMEKKeySpecification
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cmek_key_specification import CMEKKeySpecification
-
-
 T = TypeVar("T", bound="CMEKRegionSpecification")
 
 
 @attr.s(auto_attribs=True)
 class CMEKRegionSpecification:
     """CMEKRegionSpecification declares the customer-provided key specification that
     should be used in a given region.
 
         Attributes:
+            region (Union[Unset, str]):
             key_spec (Union[Unset, CMEKKeySpecification]): CMEKKeySpecification contains all the details necessary to use a
                 customer-provided
-                encryption key.
-
-                This involves the type/location of the key and the principal to authenticate as
-                when accessing it.
-            region (Union[Unset, str]):
+                encryption key. This involves the type/location of the key and the principal
+                to authenticate as when accessing it.
     """
 
-    key_spec: Union[Unset, "CMEKKeySpecification"] = UNSET
     region: Union[Unset, str] = UNSET
+    key_spec: Union[Unset, CMEKKeySpecification] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        region = self.region
         key_spec: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.key_spec, Unset):
             key_spec = self.key_spec.to_dict()
 
-        region = self.region
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if key_spec is not UNSET:
-            field_dict["key_spec"] = key_spec
         if region is not UNSET:
             field_dict["region"] = region
+        if key_spec is not UNSET:
+            field_dict["key_spec"] = key_spec
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cmek_key_specification import CMEKKeySpecification
-
         d = src_dict.copy()
+        region = d.pop("region", UNSET)
+
         _key_spec = d.pop("key_spec", UNSET)
         key_spec: Union[Unset, CMEKKeySpecification]
-        if _key_spec is None:
-            key_spec = None
         if isinstance(_key_spec, Unset):
             key_spec = UNSET
         else:
             key_spec = CMEKKeySpecification.from_dict(_key_spec)
 
-        region = d.pop("region", UNSET)
-
         cmek_region_specification = cls(
-            key_spec=key_spec,
             region=region,
+            key_spec=key_spec,
         )
 
         cmek_region_specification.additional_properties = d
         return cmek_region_specification
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_add_allowlist_entry_2_allowlist_entry.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_allowlist_entry_allowlist_entry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CockroachCloudAddAllowlistEntry2AllowlistEntry")
+T = TypeVar("T", bound="CockroachCloudUpdateAllowlistEntryAllowlistEntry")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudAddAllowlistEntry2AllowlistEntry:
+class CockroachCloudUpdateAllowlistEntryAllowlistEntry:
     """
     Example:
-        {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'name': 'Example', 'sql': True, 'ui': True}
+        {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'ui': True, 'sql': True, 'name': 'Example'}
 
     Attributes:
-        sql (bool):
         ui (bool):
+        sql (bool):
         name (Union[Unset, str]):
     """
 
-    sql: bool
     ui: bool
+    sql: bool
     name: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        sql = self.sql
         ui = self.ui
+        sql = self.sql
         name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "sql": sql,
                 "ui": ui,
+                "sql": sql,
             }
         )
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        sql = d.pop("sql")
-
         ui = d.pop("ui")
 
+        sql = d.pop("sql")
+
         name = d.pop("name", UNSET)
 
-        cockroach_cloud_add_allowlist_entry_2_allowlist_entry = cls(
-            sql=sql,
+        cockroach_cloud_update_allowlist_entry_allowlist_entry = cls(
             ui=ui,
+            sql=sql,
             name=name,
         )
 
-        cockroach_cloud_add_allowlist_entry_2_allowlist_entry.additional_properties = d
-        return cockroach_cloud_add_allowlist_entry_2_allowlist_entry
+        cockroach_cloud_update_allowlist_entry_allowlist_entry.additional_properties = d
+        return cockroach_cloud_update_allowlist_entry_allowlist_entry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_create_database_create_database_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_create_database_create_database_request.py`

 * *Files identical despite different names*

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_create_sql_user_create_sql_user_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_create_sql_user_create_sql_user_request.py`

 * *Files identical despite different names*

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_edit_database_2_update_database_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_edit_database_update_database_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CockroachCloudEditDatabase2UpdateDatabaseRequest")
+T = TypeVar("T", bound="CockroachCloudEditDatabaseUpdateDatabaseRequest")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudEditDatabase2UpdateDatabaseRequest:
+class CockroachCloudEditDatabaseUpdateDatabaseRequest:
     """
     Example:
-        {'name': 'example_database_name', 'new_name': 'example_new_database_name'}
+        {'new_name': 'example_new_database_name'}
 
     Attributes:
         name (str):
         new_name (str):
     """
 
     name: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         new_name = d.pop("new_name")
 
-        cockroach_cloud_edit_database_2_update_database_request = cls(
+        cockroach_cloud_edit_database_update_database_request = cls(
             name=name,
             new_name=new_name,
         )
 
-        cockroach_cloud_edit_database_2_update_database_request.additional_properties = d
-        return cockroach_cloud_edit_database_2_update_database_request
+        cockroach_cloud_edit_database_update_database_request.additional_properties = d
+        return cockroach_cloud_edit_database_update_database_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_edit_database_update_database_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_cluster_create_specification_region_nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CockroachCloudEditDatabaseUpdateDatabaseRequest")
+T = TypeVar("T", bound="DedicatedClusterCreateSpecificationRegionNodes")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudEditDatabaseUpdateDatabaseRequest:
-    """
-    Example:
-        {'name': 'example_database_name', 'new_name': 'example_new_database_name'}
+class DedicatedClusterCreateSpecificationRegionNodes:
+    """Region keys should match the cloud provider's zone code.
+    For example, for Oregon, set region_name to "us-west2" for
+    GCP and "us-west-2" for AWS. Values represent the node count.
 
-    Attributes:
-        new_name (str):
     """
 
-    new_name: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, int] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        new_name = self.new_name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "new_name": new_name,
-            }
-        )
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        new_name = d.pop("new_name")
-
-        cockroach_cloud_edit_database_update_database_request = cls(
-            new_name=new_name,
-        )
+        dedicated_cluster_create_specification_region_nodes = cls()
 
-        cockroach_cloud_edit_database_update_database_request.additional_properties = d
-        return cockroach_cloud_edit_database_update_database_request
+        dedicated_cluster_create_specification_region_nodes.additional_properties = d
+        return dedicated_cluster_create_specification_region_nodes
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> Any:
+    def __getitem__(self, key: str) -> int:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, key: str, value: int) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_enable_cloud_watch_metric_export_enable_cloud_watch_metric_export_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_available_regions_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,77 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.cloud_provider_region import CloudProviderRegion
+from ..models.keyset_pagination_response import KeysetPaginationResponse
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CockroachCloudEnableCloudWatchMetricExportEnableCloudWatchMetricExportRequest")
+T = TypeVar("T", bound="ListAvailableRegionsResponse")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudEnableCloudWatchMetricExportEnableCloudWatchMetricExportRequest:
+class ListAvailableRegionsResponse:
     """
-    Example:
-        {'log_group_name': 'example', 'role_arn': 'arn:aws:iam::account:role/ExampleRole', 'target_region': 'us-east-1'}
-
     Attributes:
-        role_arn (str): role_arn is the IAM role used to upload metric segments to the
-            target AWS account.
-        log_group_name (Union[Unset, str]): log_group_name is the customized log group name.
-        target_region (Union[Unset, str]): target_region specifies the specific AWS region that the metrics will
-            be exported to.
+        regions (List[CloudProviderRegion]):
+        pagination (Union[Unset, KeysetPaginationResponse]):
     """
 
-    role_arn: str
-    log_group_name: Union[Unset, str] = UNSET
-    target_region: Union[Unset, str] = UNSET
+    regions: List[CloudProviderRegion]
+    pagination: Union[Unset, KeysetPaginationResponse] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        role_arn = self.role_arn
-        log_group_name = self.log_group_name
-        target_region = self.target_region
+        regions = []
+        for regions_item_data in self.regions:
+            regions_item = regions_item_data.to_dict()
+
+            regions.append(regions_item)
+
+        pagination: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.pagination, Unset):
+            pagination = self.pagination.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "role_arn": role_arn,
+                "regions": regions,
             }
         )
-        if log_group_name is not UNSET:
-            field_dict["log_group_name"] = log_group_name
-        if target_region is not UNSET:
-            field_dict["target_region"] = target_region
+        if pagination is not UNSET:
+            field_dict["pagination"] = pagination
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        role_arn = d.pop("role_arn")
-
-        log_group_name = d.pop("log_group_name", UNSET)
-
-        target_region = d.pop("target_region", UNSET)
-
-        cockroach_cloud_enable_cloud_watch_metric_export_enable_cloud_watch_metric_export_request = cls(
-            role_arn=role_arn,
-            log_group_name=log_group_name,
-            target_region=target_region,
+        regions = []
+        _regions = d.pop("regions")
+        for regions_item_data in _regions:
+            regions_item = CloudProviderRegion.from_dict(regions_item_data)
+
+            regions.append(regions_item)
+
+        _pagination = d.pop("pagination", UNSET)
+        pagination: Union[Unset, KeysetPaginationResponse]
+        if isinstance(_pagination, Unset):
+            pagination = UNSET
+        else:
+            pagination = KeysetPaginationResponse.from_dict(_pagination)
+
+        list_available_regions_response = cls(
+            regions=regions,
+            pagination=pagination,
         )
 
-        cockroach_cloud_enable_cloud_watch_metric_export_enable_cloud_watch_metric_export_request.additional_properties = (
-            d
-        )
-        return cockroach_cloud_enable_cloud_watch_metric_export_enable_cloud_watch_metric_export_request
+        list_available_regions_response.additional_properties = d
+        return list_available_regions_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_enable_cmek_spec_cmek_cluster_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_enable_cmek_spec_cmek_cluster_specification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.cmek_region_specification import CMEKRegionSpecification
-
+from ..models.cmek_region_specification import CMEKRegionSpecification
 
 T = TypeVar("T", bound="CockroachCloudEnableCMEKSpecCMEKClusterSpecification")
 
 
 @attr.s(auto_attribs=True)
 class CockroachCloudEnableCMEKSpecCMEKClusterSpecification:
     """
     Example:
-        {'region_specs': [{'key_spec': {'auth_principal': 'arn:aws:iam::account:role/role-name-with-path', 'type':
-            'AWS_KMS', 'uri': 'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key'}, 'region': 'us-central1'}]}
+        {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri': 'arn:aws:kms:us-
+            west-2:111122223333:key/id-of-kms-key', 'auth_principal': 'arn:aws:iam::account:role/role-name-with-path'}}]}
 
     Attributes:
-        region_specs (List['CMEKRegionSpecification']):
+        region_specs (List[CMEKRegionSpecification]):
     """
 
-    region_specs: List["CMEKRegionSpecification"]
+    region_specs: List[CMEKRegionSpecification]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         region_specs = []
         for region_specs_item_data in self.region_specs:
             region_specs_item = region_specs_item_data.to_dict()
 
@@ -38,16 +36,14 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cmek_region_specification import CMEKRegionSpecification
-
         d = src_dict.copy()
         region_specs = []
         _region_specs = d.pop("region_specs")
         for region_specs_item_data in _region_specs:
             region_specs_item = CMEKRegionSpecification.from_dict(region_specs_item_data)
 
             region_specs.append(region_specs_item)
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_enable_datadog_metric_export_enable_datadog_metric_export_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_status_update_cmek_status_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.datadog_site_type import DatadogSiteType
+from ..models.cmek_customer_action import CMEKCustomerAction
 
-T = TypeVar("T", bound="CockroachCloudEnableDatadogMetricExportEnableDatadogMetricExportRequest")
+T = TypeVar("T", bound="CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudEnableDatadogMetricExportEnableDatadogMetricExportRequest:
+class CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest:
     """
     Example:
-        {'api_key': 'datadog_api_key', 'site': 'US1'}
+        {'action': 'REVOKE'}
 
     Attributes:
-        api_key (str): api_key is a Datadog API key.
-        site (DatadogSiteType):
+        action (CMEKCustomerAction): CMEKCustomerAction enumerates the actions a customer can take on a cluster
+            that has been enabled for CMEK.
     """
 
-    api_key: str
-    site: DatadogSiteType
+    action: CMEKCustomerAction
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        api_key = self.api_key
-        site = self.site.value
+        action = self.action.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "api_key": api_key,
-                "site": site,
+                "action": action,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        api_key = d.pop("api_key")
+        action = CMEKCustomerAction(d.pop("action"))
 
-        site = DatadogSiteType(d.pop("site"))
-
-        cockroach_cloud_enable_datadog_metric_export_enable_datadog_metric_export_request = cls(
-            api_key=api_key,
-            site=site,
+        cockroach_cloud_update_cmek_status_update_cmek_status_request = cls(
+            action=action,
         )
 
-        cockroach_cloud_enable_datadog_metric_export_enable_datadog_metric_export_request.additional_properties = d
-        return cockroach_cloud_enable_datadog_metric_export_enable_datadog_metric_export_request
+        cockroach_cloud_update_cmek_status_update_cmek_status_request.additional_properties = d
+        return cockroach_cloud_update_cmek_status_update_cmek_status_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_aws_endpoint_connection_state_set_aws_endpoint_connection_state_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_set_aws_endpoint_connection_state_json_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.set_aws_endpoint_connection_status_type import SetAWSEndpointConnectionStatusType
+from ..models.aws_endpoint_connection_status import AWSEndpointConnectionStatus
+from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CockroachCloudSetAwsEndpointConnectionStateSetAwsEndpointConnectionStateRequest")
+T = TypeVar("T", bound="CockroachCloudSetAwsEndpointConnectionStateJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudSetAwsEndpointConnectionStateSetAwsEndpointConnectionStateRequest:
+class CockroachCloudSetAwsEndpointConnectionStateJsonBody:
     """
-    Example:
-        {'status': 'AVAILABLE'}
-
     Attributes:
-        status (SetAWSEndpointConnectionStatusType):  - AVAILABLE: accept/verify the connection on the service side.
-             - REJECTED: reject the connection on the service side.
+        status (Union[Unset, AWSEndpointConnectionStatus]): The statuses map to the statuses returned by the AWS API.
     """
 
-    status: SetAWSEndpointConnectionStatusType
+    status: Union[Unset, AWSEndpointConnectionStatus] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        status = self.status.value
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "status": status,
-            }
-        )
+        field_dict.update({})
+        if status is not UNSET:
+            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        status = SetAWSEndpointConnectionStatusType(d.pop("status"))
+        _status = d.pop("status", UNSET)
+        status: Union[Unset, AWSEndpointConnectionStatus]
+        if isinstance(_status, Unset):
+            status = UNSET
+        else:
+            status = AWSEndpointConnectionStatus(_status)
 
-        cockroach_cloud_set_aws_endpoint_connection_state_set_aws_endpoint_connection_state_request = cls(
+        cockroach_cloud_set_aws_endpoint_connection_state_json_body = cls(
             status=status,
         )
 
-        cockroach_cloud_set_aws_endpoint_connection_state_set_aws_endpoint_connection_state_request.additional_properties = (
-            d
-        )
-        return cockroach_cloud_set_aws_endpoint_connection_state_set_aws_endpoint_connection_state_request
+        cockroach_cloud_set_aws_endpoint_connection_state_json_body.additional_properties = d
+        return cockroach_cloud_set_aws_endpoint_connection_state_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_client_ca_cert_set_client_ca_cert_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_create_private_endpoint_services_json_body.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,35 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CockroachCloudSetClientCACertSetClientCACertRequest")
+T = TypeVar("T", bound="CockroachCloudCreatePrivateEndpointServicesJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudSetClientCACertSetClientCACertRequest:
-    """
-    Example:
-        {'x509_pem_cert': '-----BEGIN CERTIFICATE-----...'}
-
-    Attributes:
-        x509_pem_cert (str):
-    """
+class CockroachCloudCreatePrivateEndpointServicesJsonBody:
+    """ """
 
-    x509_pem_cert: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        x509_pem_cert = self.x509_pem_cert
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "x509_pem_cert": x509_pem_cert,
-            }
-        )
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        x509_pem_cert = d.pop("x509_pem_cert")
+        cockroach_cloud_create_private_endpoint_services_json_body = cls()
 
-        cockroach_cloud_set_client_ca_cert_set_client_ca_cert_request = cls(
-            x509_pem_cert=x509_pem_cert,
-        )
-
-        cockroach_cloud_set_client_ca_cert_set_client_ca_cert_request.additional_properties = d
-        return cockroach_cloud_set_client_ca_cert_set_client_ca_cert_request
+        cockroach_cloud_create_private_endpoint_services_json_body.additional_properties = d
+        return cockroach_cloud_create_private_endpoint_services_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_egress_traffic_policy_response_200.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CockroachCloudSetEgressTrafficPolicyResponse200")
+from ..models.node_status import NodeStatus
 
+T = TypeVar("T", bound="Node")
 
-@attr.s(auto_attribs=True)
-class CockroachCloudSetEgressTrafficPolicyResponse200:
-    """ """
 
+@attr.s(auto_attribs=True)
+class Node:
+    """
+    Attributes:
+        name (str):
+        region_name (str):
+        status (NodeStatus):
+    """
+
+    name: str
+    region_name: str
+    status: NodeStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        name = self.name
+        region_name = self.region_name
+        status = self.status.value
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "name": name,
+                "region_name": region_name,
+                "status": status,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cockroach_cloud_set_egress_traffic_policy_response_200 = cls()
+        name = d.pop("name")
+
+        region_name = d.pop("region_name")
+
+        status = NodeStatus(d.pop("status"))
+
+        node = cls(
+            name=name,
+            region_name=region_name,
+            status=status,
+        )
 
-        cockroach_cloud_set_egress_traffic_policy_response_200.additional_properties = d
-        return cockroach_cloud_set_egress_traffic_policy_response_200
+        node.additional_properties = d
+        return node
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_egress_traffic_policy_set_egress_traffic_policy_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cmek_key_specification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,78 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.cmek_key_type import CMEKKeyType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CockroachCloudSetEgressTrafficPolicySetEgressTrafficPolicyRequest")
+T = TypeVar("T", bound="CMEKKeySpecification")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudSetEgressTrafficPolicySetEgressTrafficPolicyRequest:
-    """SetEgressTrafficPolicyRequest is the input for the SetEgressTrafficPolicy RPC.
-
-    Attributes:
-        allow_all (bool): allow_all, if true results in unrestricted egress traffic. If false, egress
-            traffic is set to default-deny and is managed via the Egress Rule
-            Management API.
-        idempotency_key (Union[Unset, str]): idempotency_key uniquely identifies this request. If not set, it will be
-            set by the server.
+class CMEKKeySpecification:
+    """CMEKKeySpecification contains all the details necessary to use a customer-provided
+    encryption key. This involves the type/location of the key and the principal
+    to authenticate as when accessing it.
+
+        Attributes:
+            type (Union[Unset, CMEKKeyType]): CMEKKeyType enumerates types of customer-managed keys.
+
+                 - UNKNOWN_KEY_TYPE: UNKNOWN should never be used; if it is used, it indicates a bug.
+            uri (Union[Unset, str]):
+            auth_principal (Union[Unset, str]):
     """
 
-    allow_all: bool
-    idempotency_key: Union[Unset, str] = UNSET
+    type: Union[Unset, CMEKKeyType] = UNSET
+    uri: Union[Unset, str] = UNSET
+    auth_principal: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        allow_all = self.allow_all
-        idempotency_key = self.idempotency_key
+        type: Union[Unset, str] = UNSET
+        if not isinstance(self.type, Unset):
+            type = self.type.value
+
+        uri = self.uri
+        auth_principal = self.auth_principal
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "allow_all": allow_all,
-            }
-        )
-        if idempotency_key is not UNSET:
-            field_dict["idempotency_key"] = idempotency_key
+        field_dict.update({})
+        if type is not UNSET:
+            field_dict["type"] = type
+        if uri is not UNSET:
+            field_dict["uri"] = uri
+        if auth_principal is not UNSET:
+            field_dict["auth_principal"] = auth_principal
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        allow_all = d.pop("allow_all")
-
-        idempotency_key = d.pop("idempotency_key", UNSET)
-
-        cockroach_cloud_set_egress_traffic_policy_set_egress_traffic_policy_request = cls(
-            allow_all=allow_all,
-            idempotency_key=idempotency_key,
+        _type = d.pop("type", UNSET)
+        type: Union[Unset, CMEKKeyType]
+        if isinstance(_type, Unset):
+            type = UNSET
+        else:
+            type = CMEKKeyType(_type)
+
+        uri = d.pop("uri", UNSET)
+
+        auth_principal = d.pop("auth_principal", UNSET)
+
+        cmek_key_specification = cls(
+            type=type,
+            uri=uri,
+            auth_principal=auth_principal,
         )
 
-        cockroach_cloud_set_egress_traffic_policy_set_egress_traffic_policy_request.additional_properties = d
-        return cockroach_cloud_set_egress_traffic_policy_set_egress_traffic_policy_request
+        cmek_key_specification.additional_properties = d
+        return cmek_key_specification
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_set_roles_for_user_json_body.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_sql_user_password_update_sql_user_password_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,51 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.built_in_role import BuiltInRole
-
-
-T = TypeVar("T", bound="CockroachCloudSetRolesForUserJsonBody")
+T = TypeVar("T", bound="CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudSetRolesForUserJsonBody:
+class CockroachCloudUpdateSQLUserPasswordUpdateSQLUserPasswordRequest:
     """
     Example:
-        [{'name': 'CLUSTER_ADMIN', 'resource': {'id': 'example_cluster_id', 'type': 'CLUSTER'}}]
+        {'password': 'example_new_password'}
 
     Attributes:
-        roles (List['BuiltInRole']):
+        password (str):
     """
 
-    roles: List["BuiltInRole"]
+    password: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        roles = []
-        for roles_item_data in self.roles:
-            roles_item = roles_item_data.to_dict()
-
-            roles.append(roles_item)
+        password = self.password
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "roles": roles,
+                "password": password,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.built_in_role import BuiltInRole
-
         d = src_dict.copy()
-        roles = []
-        _roles = d.pop("roles")
-        for roles_item_data in _roles:
-            roles_item = BuiltInRole.from_dict(roles_item_data)
-
-            roles.append(roles_item)
+        password = d.pop("password")
 
-        cockroach_cloud_set_roles_for_user_json_body = cls(
-            roles=roles,
+        cockroach_cloud_update_sql_user_password_update_sql_user_password_request = cls(
+            password=password,
         )
 
-        cockroach_cloud_set_roles_for_user_json_body.additional_properties = d
-        return cockroach_cloud_set_roles_for_user_json_body
+        cockroach_cloud_update_sql_user_password_update_sql_user_password_request.additional_properties = d
+        return cockroach_cloud_update_sql_user_password_update_sql_user_password_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_allowlist_entry_allowlist_entry.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/keyset_pagination_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,56 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CockroachCloudUpdateAllowlistEntryAllowlistEntry")
+T = TypeVar("T", bound="KeysetPaginationResponse")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudUpdateAllowlistEntryAllowlistEntry:
+class KeysetPaginationResponse:
     """
-    Example:
-        {'cidr_ip': '192.168.1.1', 'cidr_mask': 32, 'name': 'Example', 'sql': True, 'ui': True}
-
     Attributes:
-        sql (bool):
-        ui (bool):
-        name (Union[Unset, str]):
+        next_page (Union[Unset, str]):
+        previous_page (Union[Unset, str]):
     """
 
-    sql: bool
-    ui: bool
-    name: Union[Unset, str] = UNSET
+    next_page: Union[Unset, str] = UNSET
+    previous_page: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        sql = self.sql
-        ui = self.ui
-        name = self.name
+        next_page = self.next_page
+        previous_page = self.previous_page
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "sql": sql,
-                "ui": ui,
-            }
-        )
-        if name is not UNSET:
-            field_dict["name"] = name
+        field_dict.update({})
+        if next_page is not UNSET:
+            field_dict["next_page"] = next_page
+        if previous_page is not UNSET:
+            field_dict["previous_page"] = previous_page
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        sql = d.pop("sql")
-
-        ui = d.pop("ui")
+        next_page = d.pop("next_page", UNSET)
 
-        name = d.pop("name", UNSET)
+        previous_page = d.pop("previous_page", UNSET)
 
-        cockroach_cloud_update_allowlist_entry_allowlist_entry = cls(
-            sql=sql,
-            ui=ui,
-            name=name,
+        keyset_pagination_response = cls(
+            next_page=next_page,
+            previous_page=previous_page,
         )
 
-        cockroach_cloud_update_allowlist_entry_allowlist_entry.additional_properties = d
-        return cockroach_cloud_update_allowlist_entry_allowlist_entry
+        keyset_pagination_response.additional_properties = d
+        return keyset_pagination_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_spec_cmek_cluster_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_spec_cmek_cluster_specification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.cmek_region_specification import CMEKRegionSpecification
-
+from ..models.cmek_region_specification import CMEKRegionSpecification
 
 T = TypeVar("T", bound="CockroachCloudUpdateCMEKSpecCMEKClusterSpecification")
 
 
 @attr.s(auto_attribs=True)
 class CockroachCloudUpdateCMEKSpecCMEKClusterSpecification:
     """
     Example:
-        {'region_specs': [{'key_spec': {'auth_principal': 'arn:aws:iam::account:role/role-name-with-path', 'type':
-            'AWS_KMS', 'uri': 'arn:aws:kms:us-west-2:111122223333:key/id-of-kms-key'}, 'region': 'us-central1'}]}
+        {'region_specs': [{'region': 'us-central1', 'key_spec': {'type': 'AWS_KMS', 'uri': 'arn:aws:kms:us-
+            west-2:111122223333:key/id-of-kms-key', 'auth_principal': 'arn:aws:iam::account:role/role-name-with-path'}}]}
 
     Attributes:
-        region_specs (List['CMEKRegionSpecification']):
+        region_specs (List[CMEKRegionSpecification]):
     """
 
-    region_specs: List["CMEKRegionSpecification"]
+    region_specs: List[CMEKRegionSpecification]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         region_specs = []
         for region_specs_item_data in self.region_specs:
             region_specs_item = region_specs_item_data.to_dict()
 
@@ -38,16 +36,14 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cmek_region_specification import CMEKRegionSpecification
-
         d = src_dict.copy()
         region_specs = []
         _region_specs = d.pop("region_specs")
         for region_specs_item_data in _region_specs:
             region_specs_item = CMEKRegionSpecification.from_dict(region_specs_item_data)
 
             region_specs.append(region_specs_item)
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/cockroach_cloud_update_cmek_status_update_cmek_status_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/create_cluster_specification.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,73 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.cmek_customer_action import CMEKCustomerAction
+from ..models.dedicated_cluster_create_specification import DedicatedClusterCreateSpecification
+from ..models.serverless_cluster_create_specification import ServerlessClusterCreateSpecification
+from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest")
+T = TypeVar("T", bound="CreateClusterSpecification")
 
 
 @attr.s(auto_attribs=True)
-class CockroachCloudUpdateCMEKStatusUpdateCMEKStatusRequest:
+class CreateClusterSpecification:
     """
-    Example:
-        {'action': 'REVOKE'}
-
     Attributes:
-        action (CMEKCustomerAction): CMEKCustomerAction enumerates the actions a customer can take on a cluster
-            that has been enabled for CMEK.
+        dedicated (Union[Unset, DedicatedClusterCreateSpecification]):
+        serverless (Union[Unset, ServerlessClusterCreateSpecification]):
     """
 
-    action: CMEKCustomerAction
+    dedicated: Union[Unset, DedicatedClusterCreateSpecification] = UNSET
+    serverless: Union[Unset, ServerlessClusterCreateSpecification] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        action = self.action.value
+        dedicated: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.dedicated, Unset):
+            dedicated = self.dedicated.to_dict()
+
+        serverless: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.serverless, Unset):
+            serverless = self.serverless.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "action": action,
-            }
-        )
+        field_dict.update({})
+        if dedicated is not UNSET:
+            field_dict["dedicated"] = dedicated
+        if serverless is not UNSET:
+            field_dict["serverless"] = serverless
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        action = CMEKCustomerAction(d.pop("action"))
-
-        cockroach_cloud_update_cmek_status_update_cmek_status_request = cls(
-            action=action,
+        _dedicated = d.pop("dedicated", UNSET)
+        dedicated: Union[Unset, DedicatedClusterCreateSpecification]
+        if isinstance(_dedicated, Unset):
+            dedicated = UNSET
+        else:
+            dedicated = DedicatedClusterCreateSpecification.from_dict(_dedicated)
+
+        _serverless = d.pop("serverless", UNSET)
+        serverless: Union[Unset, ServerlessClusterCreateSpecification]
+        if isinstance(_serverless, Unset):
+            serverless = UNSET
+        else:
+            serverless = ServerlessClusterCreateSpecification.from_dict(_serverless)
+
+        create_cluster_specification = cls(
+            dedicated=dedicated,
+            serverless=serverless,
         )
 
-        cockroach_cloud_update_cmek_status_update_cmek_status_request.additional_properties = d
-        return cockroach_cloud_update_cmek_status_update_cmek_status_request
+        create_cluster_specification.additional_properties = d
+        return create_cluster_specification
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/create_cluster_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/create_cluster_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.cloud_provider_type import CloudProviderType
-
-if TYPE_CHECKING:
-    from ..models.create_cluster_specification import CreateClusterSpecification
-
+from ..models.api_cloud_provider import ApiCloudProvider
+from ..models.create_cluster_specification import CreateClusterSpecification
 
 T = TypeVar("T", bound="CreateClusterRequest")
 
 
 @attr.s(auto_attribs=True)
 class CreateClusterRequest:
     """
     Example:
         {'name': 'test-cluster', 'provider': 'GCP', 'spec': {'serverless': {'regions': ['us-central1'], 'spend_limit':
             0}}}
 
     Attributes:
         name (str): Name must be 6-20 characters in length and can include numbers,
             lowercase letters, and dashes (but no leading or trailing dashes).
-        provider (CloudProviderType):  - GCP: The Google Cloud Platform cloud provider.
+        provider (ApiCloudProvider):  - GCP: The Google Cloud Platform cloud provider.
              - AWS: The Amazon Web Services cloud provider.
         spec (CreateClusterSpecification):
     """
 
     name: str
-    provider: CloudProviderType
-    spec: "CreateClusterSpecification"
+    provider: ApiCloudProvider
+    spec: CreateClusterSpecification
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         provider = self.provider.value
 
         spec = self.spec.to_dict()
@@ -47,20 +44,18 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.create_cluster_specification import CreateClusterSpecification
-
         d = src_dict.copy()
         name = d.pop("name")
 
-        provider = CloudProviderType(d.pop("provider"))
+        provider = ApiCloudProvider(d.pop("provider"))
 
         spec = CreateClusterSpecification.from_dict(d.pop("spec"))
 
         create_cluster_request = cls(
             name=name,
             provider=provider,
             spec=spec,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/create_cluster_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_clusters_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,77 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.cluster import Cluster
+from ..models.keyset_pagination_response import KeysetPaginationResponse
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.dedicated_cluster_create_specification import DedicatedClusterCreateSpecification
-    from ..models.serverless_cluster_create_specification import ServerlessClusterCreateSpecification
-
-
-T = TypeVar("T", bound="CreateClusterSpecification")
+T = TypeVar("T", bound="ListClustersResponse")
 
 
 @attr.s(auto_attribs=True)
-class CreateClusterSpecification:
+class ListClustersResponse:
     """
     Attributes:
-        dedicated (Union[Unset, DedicatedClusterCreateSpecification]):
-        serverless (Union[Unset, ServerlessClusterCreateSpecification]):
+        clusters (List[Cluster]):
+        pagination (Union[Unset, KeysetPaginationResponse]):
     """
 
-    dedicated: Union[Unset, "DedicatedClusterCreateSpecification"] = UNSET
-    serverless: Union[Unset, "ServerlessClusterCreateSpecification"] = UNSET
+    clusters: List[Cluster]
+    pagination: Union[Unset, KeysetPaginationResponse] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        dedicated: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.dedicated, Unset):
-            dedicated = self.dedicated.to_dict()
-
-        serverless: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.serverless, Unset):
-            serverless = self.serverless.to_dict()
+        clusters = []
+        for clusters_item_data in self.clusters:
+            clusters_item = clusters_item_data.to_dict()
+
+            clusters.append(clusters_item)
+
+        pagination: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.pagination, Unset):
+            pagination = self.pagination.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if dedicated is not UNSET:
-            field_dict["dedicated"] = dedicated
-        if serverless is not UNSET:
-            field_dict["serverless"] = serverless
+        field_dict.update(
+            {
+                "clusters": clusters,
+            }
+        )
+        if pagination is not UNSET:
+            field_dict["pagination"] = pagination
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dedicated_cluster_create_specification import DedicatedClusterCreateSpecification
-        from ..models.serverless_cluster_create_specification import ServerlessClusterCreateSpecification
-
         d = src_dict.copy()
-        _dedicated = d.pop("dedicated", UNSET)
-        dedicated: Union[Unset, DedicatedClusterCreateSpecification]
-        if _dedicated is None:
-            dedicated = None
-        if isinstance(_dedicated, Unset):
-            dedicated = UNSET
-        else:
-            dedicated = DedicatedClusterCreateSpecification.from_dict(_dedicated)
-
-        _serverless = d.pop("serverless", UNSET)
-        serverless: Union[Unset, ServerlessClusterCreateSpecification]
-        if _serverless is None:
-            serverless = None
-        if isinstance(_serverless, Unset):
-            serverless = UNSET
+        clusters = []
+        _clusters = d.pop("clusters")
+        for clusters_item_data in _clusters:
+            clusters_item = Cluster.from_dict(clusters_item_data)
+
+            clusters.append(clusters_item)
+
+        _pagination = d.pop("pagination", UNSET)
+        pagination: Union[Unset, KeysetPaginationResponse]
+        if isinstance(_pagination, Unset):
+            pagination = UNSET
         else:
-            serverless = ServerlessClusterCreateSpecification.from_dict(_serverless)
+            pagination = KeysetPaginationResponse.from_dict(_pagination)
 
-        create_cluster_specification = cls(
-            dedicated=dedicated,
-            serverless=serverless,
+        list_clusters_response = cls(
+            clusters=clusters,
+            pagination=pagination,
         )
 
-        create_cluster_specification.additional_properties = d
-        return create_cluster_specification
+        list_clusters_response.additional_properties = d
+        return list_clusters_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/currency_amount.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/currency_amount.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.currency_type import CurrencyType
+from ..models.currency import Currency
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CurrencyAmount")
 
 
 @attr.s(auto_attribs=True)
 class CurrencyAmount:
     """
     Attributes:
-        amount (Union[Unset, float]): amount is the quantity of currency. Internally, currency amounts are tracked
-            and stored using an arbitrary-precision decimal representation, but are serialized
-            as 64-bit floating point numbers. There may be minor rounding discrepancies
-            when parsed as a 32-bit float.
-        currency (Union[Unset, CurrencyType]):
+        amount (Union[Unset, float]): Amount is the quantity of currency.
+        currency (Union[Unset, Currency]): Currency is the set of currencies supported in CockroachCloud.
     """
 
     amount: Union[Unset, float] = UNSET
-    currency: Union[Unset, CurrencyType] = UNSET
+    currency: Union[Unset, Currency] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         amount = self.amount
         currency: Union[Unset, str] = UNSET
         if not isinstance(self.currency, Unset):
             currency = self.currency.value
@@ -41,21 +38,19 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         amount = d.pop("amount", UNSET)
 
         _currency = d.pop("currency", UNSET)
-        currency: Union[Unset, CurrencyType]
-        if _currency is None:
-            currency = None
+        currency: Union[Unset, Currency]
         if isinstance(_currency, Unset):
             currency = UNSET
         else:
-            currency = CurrencyType(_currency)
+            currency = Currency(_currency)
 
         currency_amount = cls(
             amount=amount,
             currency=currency,
         )
 
         currency_amount.additional_properties = d
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/database.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/database.py`

 * *Files identical despite different names*

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/datadog_metric_export_info.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_machine_type_specification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,58 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.datadog_site_type import DatadogSiteType
-from ..models.metric_export_status_type import MetricExportStatusType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DatadogMetricExportInfo")
+T = TypeVar("T", bound="DedicatedMachineTypeSpecification")
 
 
 @attr.s(auto_attribs=True)
-class DatadogMetricExportInfo:
+class DedicatedMachineTypeSpecification:
     """
     Attributes:
-        cluster_id (str):
-        site (DatadogSiteType):
-        api_key (Union[Unset, str]): api_key is the last 4 digits of a Datadog API key.
-        status (Union[Unset, MetricExportStatusType]):
-        user_message (Union[Unset, str]):
+        machine_type (Union[Unset, str]): MachineType is the machine type identifier within the given cloud
+            provider, ex. m5.xlarge, n2-standard-4.
+        num_virtual_cpus (Union[Unset, int]): NumVirtualCPUs may be used to automatically select a machine type
+            according to the desired number of vCPUs.
     """
 
-    cluster_id: str
-    site: DatadogSiteType
-    api_key: Union[Unset, str] = UNSET
-    status: Union[Unset, MetricExportStatusType] = UNSET
-    user_message: Union[Unset, str] = UNSET
+    machine_type: Union[Unset, str] = UNSET
+    num_virtual_cpus: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cluster_id = self.cluster_id
-        site = self.site.value
-
-        api_key = self.api_key
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
-
-        user_message = self.user_message
+        machine_type = self.machine_type
+        num_virtual_cpus = self.num_virtual_cpus
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "cluster_id": cluster_id,
-                "site": site,
-            }
-        )
-        if api_key is not UNSET:
-            field_dict["api_key"] = api_key
-        if status is not UNSET:
-            field_dict["status"] = status
-        if user_message is not UNSET:
-            field_dict["user_message"] = user_message
+        field_dict.update({})
+        if machine_type is not UNSET:
+            field_dict["machine_type"] = machine_type
+        if num_virtual_cpus is not UNSET:
+            field_dict["num_virtual_cpus"] = num_virtual_cpus
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cluster_id = d.pop("cluster_id")
-
-        site = DatadogSiteType(d.pop("site"))
+        machine_type = d.pop("machine_type", UNSET)
 
-        api_key = d.pop("api_key", UNSET)
+        num_virtual_cpus = d.pop("num_virtual_cpus", UNSET)
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, MetricExportStatusType]
-        if _status is None:
-            status = None
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = MetricExportStatusType(_status)
-
-        user_message = d.pop("user_message", UNSET)
-
-        datadog_metric_export_info = cls(
-            cluster_id=cluster_id,
-            site=site,
-            api_key=api_key,
-            status=status,
-            user_message=user_message,
+        dedicated_machine_type_specification = cls(
+            machine_type=machine_type,
+            num_virtual_cpus=num_virtual_cpus,
         )
 
-        datadog_metric_export_info.additional_properties = d
-        return datadog_metric_export_info
+        dedicated_machine_type_specification.additional_properties = d
+        return dedicated_machine_type_specification
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_cluster_create_specification_region_nodes.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/status.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,85 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-T = TypeVar("T", bound="DedicatedClusterCreateSpecificationRegionNodes")
+from ..models.any_ import Any
+from ..types import UNSET, Unset
 
+T = TypeVar("T", bound="Status")
 
-@attr.s(auto_attribs=True)
-class DedicatedClusterCreateSpecificationRegionNodes:
-    """Region keys should match the cloud provider's zone code.
-    For example, for Oregon, set region_name to "us-west2" for
-    GCP and "us-west-2" for AWS. Values represent the node count.
 
+@attr.s(auto_attribs=True)
+class Status:
+    """
+    Attributes:
+        code (Union[Unset, int]):
+        message (Union[Unset, str]):
+        details (Union[Unset, List[Any]]):
     """
 
-    additional_properties: Dict[str, int] = attr.ib(init=False, factory=dict)
+    code: Union[Unset, int] = UNSET
+    message: Union[Unset, str] = UNSET
+    details: Union[Unset, List[Any]] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        code = self.code
+        message = self.message
+        details: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.details, Unset):
+            details = []
+            for details_item_data in self.details:
+                details_item = details_item_data.to_dict()
+
+                details.append(details_item)
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
+        if code is not UNSET:
+            field_dict["code"] = code
+        if message is not UNSET:
+            field_dict["message"] = message
+        if details is not UNSET:
+            field_dict["details"] = details
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        dedicated_cluster_create_specification_region_nodes = cls()
+        code = d.pop("code", UNSET)
+
+        message = d.pop("message", UNSET)
+
+        details = []
+        _details = d.pop("details", UNSET)
+        for details_item_data in _details or []:
+            details_item = Any.from_dict(details_item_data)
+
+            details.append(details_item)
+
+        status = cls(
+            code=code,
+            message=message,
+            details=details,
+        )
 
-        dedicated_cluster_create_specification_region_nodes.additional_properties = d
-        return dedicated_cluster_create_specification_region_nodes
+        status.additional_properties = d
+        return status
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> int:
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: int) -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_cluster_update_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_cluster_update_specification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,96 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.cmek_region_specification import CMEKRegionSpecification
+from ..models.dedicated_cluster_update_specification_region_nodes import DedicatedClusterUpdateSpecificationRegionNodes
+from ..models.dedicated_hardware_update_specification import DedicatedHardwareUpdateSpecification
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cmek_region_specification import CMEKRegionSpecification
-    from ..models.dedicated_cluster_update_specification_region_nodes import (
-        DedicatedClusterUpdateSpecificationRegionNodes,
-    )
-    from ..models.dedicated_hardware_update_specification import DedicatedHardwareUpdateSpecification
-
-
 T = TypeVar("T", bound="DedicatedClusterUpdateSpecification")
 
 
 @attr.s(auto_attribs=True)
 class DedicatedClusterUpdateSpecification:
     """
     Attributes:
-        cmek_region_specs (Union[Unset, List['CMEKRegionSpecification']]): This field should contain the CMEK specs for
-            newly added regions. If a
-            CMEK spec is provided for an existing region, the request is invalid and
-            will fail.
-        hardware (Union[Unset, DedicatedHardwareUpdateSpecification]):
         region_nodes (Union[Unset, DedicatedClusterUpdateSpecificationRegionNodes]): Region keys should match the cloud
             provider's zone code.
             For example, for Oregon, set region_name to "us-west2" for
             GCP and "us-west-2" for AWS. Values represent the node count.
+        hardware (Union[Unset, DedicatedHardwareUpdateSpecification]):
+        cmek_region_specs (Union[Unset, List[CMEKRegionSpecification]]): This field should contain the CMEK specs for
+            newly added regions. If a
+            CMEK spec is provided for an existing region, the request is invalid and
+            will fail.
     """
 
-    cmek_region_specs: Union[Unset, List["CMEKRegionSpecification"]] = UNSET
-    hardware: Union[Unset, "DedicatedHardwareUpdateSpecification"] = UNSET
-    region_nodes: Union[Unset, "DedicatedClusterUpdateSpecificationRegionNodes"] = UNSET
+    region_nodes: Union[Unset, DedicatedClusterUpdateSpecificationRegionNodes] = UNSET
+    hardware: Union[Unset, DedicatedHardwareUpdateSpecification] = UNSET
+    cmek_region_specs: Union[Unset, List[CMEKRegionSpecification]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        region_nodes: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.region_nodes, Unset):
+            region_nodes = self.region_nodes.to_dict()
+
+        hardware: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.hardware, Unset):
+            hardware = self.hardware.to_dict()
+
         cmek_region_specs: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.cmek_region_specs, Unset):
             cmek_region_specs = []
             for cmek_region_specs_item_data in self.cmek_region_specs:
                 cmek_region_specs_item = cmek_region_specs_item_data.to_dict()
 
                 cmek_region_specs.append(cmek_region_specs_item)
 
-        hardware: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.hardware, Unset):
-            hardware = self.hardware.to_dict()
-
-        region_nodes: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.region_nodes, Unset):
-            region_nodes = self.region_nodes.to_dict()
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if cmek_region_specs is not UNSET:
-            field_dict["cmek_region_specs"] = cmek_region_specs
-        if hardware is not UNSET:
-            field_dict["hardware"] = hardware
         if region_nodes is not UNSET:
             field_dict["region_nodes"] = region_nodes
+        if hardware is not UNSET:
+            field_dict["hardware"] = hardware
+        if cmek_region_specs is not UNSET:
+            field_dict["cmek_region_specs"] = cmek_region_specs
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cmek_region_specification import CMEKRegionSpecification
-        from ..models.dedicated_cluster_update_specification_region_nodes import (
-            DedicatedClusterUpdateSpecificationRegionNodes,
-        )
-        from ..models.dedicated_hardware_update_specification import DedicatedHardwareUpdateSpecification
-
         d = src_dict.copy()
-        cmek_region_specs = []
-        _cmek_region_specs = d.pop("cmek_region_specs", UNSET)
-        for cmek_region_specs_item_data in _cmek_region_specs or []:
-            cmek_region_specs_item = CMEKRegionSpecification.from_dict(cmek_region_specs_item_data)
-
-            cmek_region_specs.append(cmek_region_specs_item)
+        _region_nodes = d.pop("region_nodes", UNSET)
+        region_nodes: Union[Unset, DedicatedClusterUpdateSpecificationRegionNodes]
+        if isinstance(_region_nodes, Unset):
+            region_nodes = UNSET
+        else:
+            region_nodes = DedicatedClusterUpdateSpecificationRegionNodes.from_dict(_region_nodes)
 
         _hardware = d.pop("hardware", UNSET)
         hardware: Union[Unset, DedicatedHardwareUpdateSpecification]
-        if _hardware is None:
-            hardware = None
         if isinstance(_hardware, Unset):
             hardware = UNSET
         else:
             hardware = DedicatedHardwareUpdateSpecification.from_dict(_hardware)
 
-        _region_nodes = d.pop("region_nodes", UNSET)
-        region_nodes: Union[Unset, DedicatedClusterUpdateSpecificationRegionNodes]
-        if _region_nodes is None:
-            region_nodes = None
-        if isinstance(_region_nodes, Unset):
-            region_nodes = UNSET
-        else:
-            region_nodes = DedicatedClusterUpdateSpecificationRegionNodes.from_dict(_region_nodes)
+        cmek_region_specs = []
+        _cmek_region_specs = d.pop("cmek_region_specs", UNSET)
+        for cmek_region_specs_item_data in _cmek_region_specs or []:
+            cmek_region_specs_item = CMEKRegionSpecification.from_dict(cmek_region_specs_item_data)
+
+            cmek_region_specs.append(cmek_region_specs_item)
 
         dedicated_cluster_update_specification = cls(
-            cmek_region_specs=cmek_region_specs,
-            hardware=hardware,
             region_nodes=region_nodes,
+            hardware=hardware,
+            cmek_region_specs=cmek_region_specs,
         )
 
         dedicated_cluster_update_specification.additional_properties = d
         return dedicated_cluster_update_specification
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_cluster_update_specification_region_nodes.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/serverless_cluster_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="DedicatedClusterUpdateSpecificationRegionNodes")
+T = TypeVar("T", bound="ServerlessClusterConfig")
 
 
 @attr.s(auto_attribs=True)
-class DedicatedClusterUpdateSpecificationRegionNodes:
-    """Region keys should match the cloud provider's zone code.
-    For example, for Oregon, set region_name to "us-west2" for
-    GCP and "us-west-2" for AWS. Values represent the node count.
-
+class ServerlessClusterConfig:
+    """
+    Attributes:
+        spend_limit (int): Spend limit in US cents.
+        routing_id (str): Used to build a connection string.
     """
 
-    additional_properties: Dict[str, int] = attr.ib(init=False, factory=dict)
+    spend_limit: int
+    routing_id: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        spend_limit = self.spend_limit
+        routing_id = self.routing_id
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "spend_limit": spend_limit,
+                "routing_id": routing_id,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        dedicated_cluster_update_specification_region_nodes = cls()
+        spend_limit = d.pop("spend_limit")
+
+        routing_id = d.pop("routing_id")
+
+        serverless_cluster_config = cls(
+            spend_limit=spend_limit,
+            routing_id=routing_id,
+        )
 
-        dedicated_cluster_update_specification_region_nodes.additional_properties = d
-        return dedicated_cluster_update_specification_region_nodes
+        serverless_cluster_config.additional_properties = d
+        return serverless_cluster_config
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> int:
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: int) -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_hardware_config.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_hardware_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,71 +5,71 @@
 T = TypeVar("T", bound="DedicatedHardwareConfig")
 
 
 @attr.s(auto_attribs=True)
 class DedicatedHardwareConfig:
     """
     Attributes:
-        disk_iops (int): disk_iops is the number of disk I/O operations per second that are
+        machine_type (str): MachineType is the machine type identifier within the given cloud
+            provider, ex. m5.xlarge, n2-standard-4.
+        num_virtual_cpus (int): NumVirtualCPUs is the number of virtual CPUs per node in the cluster.
+        storage_gib (int): StorageGiB is the number of storage GiB per node in the cluster.
+        memory_gib (float): MemoryGiB is the memory GiB per node in the cluster.
+        disk_iops (int): DiskIOPs is the number of disk I/O operations per second that are
             permitted on each node in the cluster. Zero indicates the cloud
             provider-specific default.
-        machine_type (str): machine_type is the machine type identifier within the given cloud
-            provider, ex. m5.xlarge, n2-standard-4.
-        memory_gib (float): memory_gib is the memory GiB per node in the cluster.
-        num_virtual_cpus (int): num_virtual_cpus is the number of virtual CPUs per node in the cluster.
-        storage_gib (int): storage_gib is the number of storage GiB per node in the cluster.
     """
 
-    disk_iops: int
     machine_type: str
-    memory_gib: float
     num_virtual_cpus: int
     storage_gib: int
+    memory_gib: float
+    disk_iops: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        disk_iops = self.disk_iops
         machine_type = self.machine_type
-        memory_gib = self.memory_gib
         num_virtual_cpus = self.num_virtual_cpus
         storage_gib = self.storage_gib
+        memory_gib = self.memory_gib
+        disk_iops = self.disk_iops
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "disk_iops": disk_iops,
                 "machine_type": machine_type,
-                "memory_gib": memory_gib,
                 "num_virtual_cpus": num_virtual_cpus,
                 "storage_gib": storage_gib,
+                "memory_gib": memory_gib,
+                "disk_iops": disk_iops,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        disk_iops = d.pop("disk_iops")
-
         machine_type = d.pop("machine_type")
 
-        memory_gib = d.pop("memory_gib")
-
         num_virtual_cpus = d.pop("num_virtual_cpus")
 
         storage_gib = d.pop("storage_gib")
 
+        memory_gib = d.pop("memory_gib")
+
+        disk_iops = d.pop("disk_iops")
+
         dedicated_hardware_config = cls(
-            disk_iops=disk_iops,
             machine_type=machine_type,
-            memory_gib=memory_gib,
             num_virtual_cpus=num_virtual_cpus,
             storage_gib=storage_gib,
+            memory_gib=memory_gib,
+            disk_iops=disk_iops,
         )
 
         dedicated_hardware_config.additional_properties = d
         return dedicated_hardware_config
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_hardware_create_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_hardware_create_specification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.dedicated_machine_type_specification import DedicatedMachineTypeSpecification
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.dedicated_machine_type_specification import DedicatedMachineTypeSpecification
-
-
 T = TypeVar("T", bound="DedicatedHardwareCreateSpecification")
 
 
 @attr.s(auto_attribs=True)
 class DedicatedHardwareCreateSpecification:
     """
     Attributes:
         machine_spec (DedicatedMachineTypeSpecification):
-        storage_gib (int): storage_gib is the number of storage GiB per node in the cluster.
+        storage_gib (int): StorageGiB is the number of storage GiB per node in the cluster.
             Zero indicates default to the lowest storage GiB available given machine specs.
-        disk_iops (Union[Unset, int]): disk_iops is the number of disk I/O operations per second that are
+        disk_iops (Union[Unset, int]): DiskIOPs is the number of disk I/O operations per second that are
             permitted on each node in the cluster. Zero indicates the cloud
             provider-specific default. Only available for AWS clusters.
     """
 
-    machine_spec: "DedicatedMachineTypeSpecification"
+    machine_spec: DedicatedMachineTypeSpecification
     storage_gib: int
     disk_iops: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         machine_spec = self.machine_spec.to_dict()
 
@@ -45,16 +42,14 @@
         if disk_iops is not UNSET:
             field_dict["disk_iops"] = disk_iops
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dedicated_machine_type_specification import DedicatedMachineTypeSpecification
-
         d = src_dict.copy()
         machine_spec = DedicatedMachineTypeSpecification.from_dict(d.pop("machine_spec"))
 
         storage_gib = d.pop("storage_gib")
 
         disk_iops = d.pop("disk_iops", UNSET)
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/dedicated_hardware_update_specification.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/dedicated_hardware_update_specification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,71 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.dedicated_machine_type_specification import DedicatedMachineTypeSpecification
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.dedicated_machine_type_specification import DedicatedMachineTypeSpecification
-
-
 T = TypeVar("T", bound="DedicatedHardwareUpdateSpecification")
 
 
 @attr.s(auto_attribs=True)
 class DedicatedHardwareUpdateSpecification:
     """
     Attributes:
-        disk_iops (Union[Unset, int]): disk_iops is the number of disk I/O operations per second that are
+        machine_spec (Union[Unset, DedicatedMachineTypeSpecification]):
+        storage_gib (Union[Unset, int]): StorageGiB is the number of storage GiB per node in the cluster.
+        disk_iops (Union[Unset, int]): DiskIOPs is the number of disk I/O operations per second that are
             permitted on each node in the cluster. Zero indicates the cloud
             provider-specific default. Only available for AWS clusters.
-        machine_spec (Union[Unset, DedicatedMachineTypeSpecification]):
-        storage_gib (Union[Unset, int]): storage_gib is the number of storage GiB per node in the cluster.
     """
 
-    disk_iops: Union[Unset, int] = UNSET
-    machine_spec: Union[Unset, "DedicatedMachineTypeSpecification"] = UNSET
+    machine_spec: Union[Unset, DedicatedMachineTypeSpecification] = UNSET
     storage_gib: Union[Unset, int] = UNSET
+    disk_iops: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        disk_iops = self.disk_iops
         machine_spec: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.machine_spec, Unset):
             machine_spec = self.machine_spec.to_dict()
 
         storage_gib = self.storage_gib
+        disk_iops = self.disk_iops
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if disk_iops is not UNSET:
-            field_dict["disk_iops"] = disk_iops
         if machine_spec is not UNSET:
             field_dict["machine_spec"] = machine_spec
         if storage_gib is not UNSET:
             field_dict["storage_gib"] = storage_gib
+        if disk_iops is not UNSET:
+            field_dict["disk_iops"] = disk_iops
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dedicated_machine_type_specification import DedicatedMachineTypeSpecification
-
         d = src_dict.copy()
-        disk_iops = d.pop("disk_iops", UNSET)
-
         _machine_spec = d.pop("machine_spec", UNSET)
         machine_spec: Union[Unset, DedicatedMachineTypeSpecification]
-        if _machine_spec is None:
-            machine_spec = None
         if isinstance(_machine_spec, Unset):
             machine_spec = UNSET
         else:
             machine_spec = DedicatedMachineTypeSpecification.from_dict(_machine_spec)
 
         storage_gib = d.pop("storage_gib", UNSET)
 
+        disk_iops = d.pop("disk_iops", UNSET)
+
         dedicated_hardware_update_specification = cls(
-            disk_iops=disk_iops,
             machine_spec=machine_spec,
             storage_gib=storage_gib,
+            disk_iops=disk_iops,
         )
 
         dedicated_hardware_update_specification.additional_properties = d
         return dedicated_hardware_update_specification
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/delete_metric_export_response.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/update_cluster_specification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.metric_export_status_type import MetricExportStatusType
+from ..models.dedicated_cluster_update_specification import DedicatedClusterUpdateSpecification
+from ..models.serverless_cluster_update_specification import ServerlessClusterUpdateSpecification
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DeleteMetricExportResponse")
+T = TypeVar("T", bound="UpdateClusterSpecification")
 
 
 @attr.s(auto_attribs=True)
-class DeleteMetricExportResponse:
+class UpdateClusterSpecification:
     """
+    Example:
+        {'dedicated': {'region_nodes': {'us-west1': 3, 'us-central1': 5}, 'hardware': {'machine_type':
+            'n2-standard-8'}}}
+
     Attributes:
-        cluster_id (str):
-        status (Union[Unset, MetricExportStatusType]):
+        dedicated (Union[Unset, DedicatedClusterUpdateSpecification]):
+        serverless (Union[Unset, ServerlessClusterUpdateSpecification]):
     """
 
-    cluster_id: str
-    status: Union[Unset, MetricExportStatusType] = UNSET
+    dedicated: Union[Unset, DedicatedClusterUpdateSpecification] = UNSET
+    serverless: Union[Unset, ServerlessClusterUpdateSpecification] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cluster_id = self.cluster_id
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        dedicated: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.dedicated, Unset):
+            dedicated = self.dedicated.to_dict()
+
+        serverless: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.serverless, Unset):
+            serverless = self.serverless.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "cluster_id": cluster_id,
-            }
-        )
-        if status is not UNSET:
-            field_dict["status"] = status
+        field_dict.update({})
+        if dedicated is not UNSET:
+            field_dict["dedicated"] = dedicated
+        if serverless is not UNSET:
+            field_dict["serverless"] = serverless
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cluster_id = d.pop("cluster_id")
+        _dedicated = d.pop("dedicated", UNSET)
+        dedicated: Union[Unset, DedicatedClusterUpdateSpecification]
+        if isinstance(_dedicated, Unset):
+            dedicated = UNSET
+        else:
+            dedicated = DedicatedClusterUpdateSpecification.from_dict(_dedicated)
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, MetricExportStatusType]
-        if _status is None:
-            status = None
-        if isinstance(_status, Unset):
-            status = UNSET
+        _serverless = d.pop("serverless", UNSET)
+        serverless: Union[Unset, ServerlessClusterUpdateSpecification]
+        if isinstance(_serverless, Unset):
+            serverless = UNSET
         else:
-            status = MetricExportStatusType(_status)
+            serverless = ServerlessClusterUpdateSpecification.from_dict(_serverless)
 
-        delete_metric_export_response = cls(
-            cluster_id=cluster_id,
-            status=status,
+        update_cluster_specification = cls(
+            dedicated=dedicated,
+            serverless=serverless,
         )
 
-        delete_metric_export_response.additional_properties = d
-        return delete_metric_export_response
+        update_cluster_specification.additional_properties = d
+        return update_cluster_specification
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/egress_rule.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/log_export_cluster_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,147 +1,132 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.log_export_cluster_specification import LogExportClusterSpecification
+from ..models.log_export_status import LogExportStatus
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="EgressRule")
+T = TypeVar("T", bound="LogExportClusterInfo")
 
 
 @attr.s(auto_attribs=True)
-class EgressRule:
-    """EgressRule represents a network egress rule.
-
-    Attributes:
-        cluster_id (str): cluster_id identifies the cluster to which this egress rule applies.
-        crl_managed (bool): crl_managed indicates this egress rule is managed by CockroachDB Cloud
-            services. This field is set by the server.
-        description (str): description is a longer that serves to document the rules purpose.
-        destination (str): destination is the endpoint (or subnetwork if CIDR) to which traffic is
-            allowed.
-        id (str): id uniquely identifies this egress rule.
-        name (str): name is the name of the egress rule.
-        state (str): state indicates the state of the egress rule.
-        type (str): type classifies the destination field. Valid types include: "FQDN",
-            "CIDR".
-        created_at (Union[Unset, datetime.datetime]): created_at is the time at which the time at which the egress rule
-            was
-            created.
-        paths (Union[Unset, List[str]]): paths are the allowed URL paths. Only valid if Type="FQDN".
-        ports (Union[Unset, List[int]]): ports are the allowed ports for TCP protocol. If Empty, all ports are
-            allowed.
+class LogExportClusterInfo:
+    """LogExportClusterInfo contains a package of information that fully
+    describes both the intended state of the log export configuration for
+    a specific cluster but also some metadata around its deployment
+    status, any error messages, and some timestamps.
+
+        Attributes:
+            cluster_id (Union[Unset, str]):
+            status (Union[Unset, LogExportStatus]): LogExportStatus encodes the possible states that a configuration can
+                be in as it is created, deployed, and disabled.
+            user_message (Union[Unset, str]):
+            spec (Union[Unset, LogExportClusterSpecification]): LogExportClusterSpecification contains all the data
+                necessary to
+                configure log export for an individual cluster. Users would supply
+                this data via the API and also receive it back when inspecting the
+                state of their log export configuration.
+            created_at (Union[Unset, datetime.datetime]):
+            updated_at (Union[Unset, datetime.datetime]):
     """
 
-    cluster_id: str
-    crl_managed: bool
-    description: str
-    destination: str
-    id: str
-    name: str
-    state: str
-    type: str
+    cluster_id: Union[Unset, str] = UNSET
+    status: Union[Unset, LogExportStatus] = UNSET
+    user_message: Union[Unset, str] = UNSET
+    spec: Union[Unset, LogExportClusterSpecification] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
-    paths: Union[Unset, List[str]] = UNSET
-    ports: Union[Unset, List[int]] = UNSET
+    updated_at: Union[Unset, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         cluster_id = self.cluster_id
-        crl_managed = self.crl_managed
-        description = self.description
-        destination = self.destination
-        id = self.id
-        name = self.name
-        state = self.state
-        type = self.type
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
+
+        user_message = self.user_message
+        spec: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.spec, Unset):
+            spec = self.spec.to_dict()
+
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
-        paths: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.paths, Unset):
-            paths = self.paths
-
-        ports: Union[Unset, List[int]] = UNSET
-        if not isinstance(self.ports, Unset):
-            ports = self.ports
+        updated_at: Union[Unset, str] = UNSET
+        if not isinstance(self.updated_at, Unset):
+            updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "cluster_id": cluster_id,
-                "crl_managed": crl_managed,
-                "description": description,
-                "destination": destination,
-                "id": id,
-                "name": name,
-                "state": state,
-                "type": type,
-            }
-        )
+        field_dict.update({})
+        if cluster_id is not UNSET:
+            field_dict["cluster_id"] = cluster_id
+        if status is not UNSET:
+            field_dict["status"] = status
+        if user_message is not UNSET:
+            field_dict["user_message"] = user_message
+        if spec is not UNSET:
+            field_dict["spec"] = spec
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
-        if paths is not UNSET:
-            field_dict["paths"] = paths
-        if ports is not UNSET:
-            field_dict["ports"] = ports
+        if updated_at is not UNSET:
+            field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cluster_id = d.pop("cluster_id")
-
-        crl_managed = d.pop("crl_managed")
-
-        description = d.pop("description")
-
-        destination = d.pop("destination")
+        cluster_id = d.pop("cluster_id", UNSET)
 
-        id = d.pop("id")
-
-        name = d.pop("name")
+        _status = d.pop("status", UNSET)
+        status: Union[Unset, LogExportStatus]
+        if isinstance(_status, Unset):
+            status = UNSET
+        else:
+            status = LogExportStatus(_status)
 
-        state = d.pop("state")
+        user_message = d.pop("user_message", UNSET)
 
-        type = d.pop("type")
+        _spec = d.pop("spec", UNSET)
+        spec: Union[Unset, LogExportClusterSpecification]
+        if isinstance(_spec, Unset):
+            spec = UNSET
+        else:
+            spec = LogExportClusterSpecification.from_dict(_spec)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
-        if _created_at is None:
-            created_at = None
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        paths = cast(List[str], d.pop("paths", UNSET))
-
-        ports = cast(List[int], d.pop("ports", UNSET))
+        _updated_at = d.pop("updated_at", UNSET)
+        updated_at: Union[Unset, datetime.datetime]
+        if isinstance(_updated_at, Unset):
+            updated_at = UNSET
+        else:
+            updated_at = isoparse(_updated_at)
 
-        egress_rule = cls(
+        log_export_cluster_info = cls(
             cluster_id=cluster_id,
-            crl_managed=crl_managed,
-            description=description,
-            destination=destination,
-            id=id,
-            name=name,
-            state=state,
-            type=type,
+            status=status,
+            user_message=user_message,
+            spec=spec,
             created_at=created_at,
-            paths=paths,
-            ports=ports,
+            updated_at=updated_at,
         )
 
-        egress_rule.additional_properties = d
-        return egress_rule
+        log_export_cluster_info.additional_properties = d
+        return log_export_cluster_info
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_connection_string_response_params.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/sql_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="GetConnectionStringResponseParams")
+T = TypeVar("T", bound="SQLUser")
 
 
 @attr.s(auto_attribs=True)
-class GetConnectionStringResponseParams:
-    """params contains a list of individual key parameters for generating nonstandard connection strings."""
+class SQLUser:
+    """
+    Attributes:
+        name (str):
+    """
 
-    additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
+    name: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        name = self.name
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "name": name,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        get_connection_string_response_params = cls()
+        name = d.pop("name")
+
+        sql_user = cls(
+            name=name,
+        )
 
-        get_connection_string_response_params.additional_properties = d
-        return get_connection_string_response_params
+        sql_user.additional_properties = d
+        return sql_user
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> str:
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: str) -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_egress_rule_response.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_invoices_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.egress_rule import EgressRule
+from ..models.invoice import Invoice
 
-
-T = TypeVar("T", bound="GetEgressRuleResponse")
+T = TypeVar("T", bound="ListInvoicesResponse")
 
 
 @attr.s(auto_attribs=True)
-class GetEgressRuleResponse:
-    """GetEgressRuleResponse is the response message to the GetEgressRule RPC.
-
+class ListInvoicesResponse:
+    """
     Attributes:
-        rule (EgressRule): EgressRule represents a network egress rule.
+        invoices (List[Invoice]): Invoices are sorted by PeriodStart time.
     """
 
-    rule: "EgressRule"
+    invoices: List[Invoice]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        rule = self.rule.to_dict()
+        invoices = []
+        for invoices_item_data in self.invoices:
+            invoices_item = invoices_item_data.to_dict()
+
+            invoices.append(invoices_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "rule": rule,
+                "invoices": invoices,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.egress_rule import EgressRule
-
         d = src_dict.copy()
-        rule = EgressRule.from_dict(d.pop("rule"))
+        invoices = []
+        _invoices = d.pop("invoices")
+        for invoices_item_data in _invoices:
+            invoices_item = Invoice.from_dict(invoices_item_data)
+
+            invoices.append(invoices_item)
 
-        get_egress_rule_response = cls(
-            rule=rule,
+        list_invoices_response = cls(
+            invoices=invoices,
         )
 
-        get_egress_rule_response.additional_properties = d
-        return get_egress_rule_response
+        list_invoices_response.additional_properties = d
+        return list_invoices_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/get_person_users_by_email_response.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_sql_users_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,77 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.keyset_pagination_response import KeysetPaginationResponse
+from ..models.sql_user import SQLUser
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.person_user_info_contains_information_about_a_person import (
-        PersonUserInfoContainsInformationAboutAPerson,
-    )
-
-
-T = TypeVar("T", bound="GetPersonUsersByEmailResponse")
+T = TypeVar("T", bound="ListSQLUsersResponse")
 
 
 @attr.s(auto_attribs=True)
-class GetPersonUsersByEmailResponse:
+class ListSQLUsersResponse:
     """
     Attributes:
-        user (Union[Unset, PersonUserInfoContainsInformationAboutAPerson]):
+        users (List[SQLUser]):
+        pagination (Union[Unset, KeysetPaginationResponse]):
     """
 
-    user: Union[Unset, "PersonUserInfoContainsInformationAboutAPerson"] = UNSET
+    users: List[SQLUser]
+    pagination: Union[Unset, KeysetPaginationResponse] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        user: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.user, Unset):
-            user = self.user.to_dict()
+        users = []
+        for users_item_data in self.users:
+            users_item = users_item_data.to_dict()
+
+            users.append(users_item)
+
+        pagination: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.pagination, Unset):
+            pagination = self.pagination.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if user is not UNSET:
-            field_dict["user"] = user
+        field_dict.update(
+            {
+                "users": users,
+            }
+        )
+        if pagination is not UNSET:
+            field_dict["pagination"] = pagination
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.person_user_info_contains_information_about_a_person import (
-            PersonUserInfoContainsInformationAboutAPerson,
-        )
-
         d = src_dict.copy()
-        _user = d.pop("user", UNSET)
-        user: Union[Unset, PersonUserInfoContainsInformationAboutAPerson]
-        if _user is None:
-            user = None
-        if isinstance(_user, Unset):
-            user = UNSET
+        users = []
+        _users = d.pop("users")
+        for users_item_data in _users:
+            users_item = SQLUser.from_dict(users_item_data)
+
+            users.append(users_item)
+
+        _pagination = d.pop("pagination", UNSET)
+        pagination: Union[Unset, KeysetPaginationResponse]
+        if isinstance(_pagination, Unset):
+            pagination = UNSET
         else:
-            user = PersonUserInfoContainsInformationAboutAPerson.from_dict(_user)
+            pagination = KeysetPaginationResponse.from_dict(_pagination)
 
-        get_person_users_by_email_response = cls(
-            user=user,
+        list_sql_users_response = cls(
+            users=users,
+            pagination=pagination,
         )
 
-        get_person_users_by_email_response.additional_properties = d
-        return get_person_users_by_email_response
+        list_sql_users_response.additional_properties = d
+        return list_sql_users_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/invoice.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/invoice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,119 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 from dateutil.parser import isoparse
 
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.currency_amount import CurrencyAmount
-    from ..models.invoice_adjustment import InvoiceAdjustment
-    from ..models.invoice_item import InvoiceItem
-
+from ..models.currency_amount import CurrencyAmount
+from ..models.invoice_item import InvoiceItem
 
 T = TypeVar("T", bound="Invoice")
 
 
 @attr.s(auto_attribs=True)
 class Invoice:
     """Invoice message represents the details and the total charges associated with
     one billing period, which starts at the beginning of the month and ends at
-    the beginning of the next month.
-
-    The message also includes details about each invoice item.
+    the beginning of the next month. The message also includes details about each
+    invoice item.
 
         Attributes:
-            balances (List['CurrencyAmount']): balances are the amounts of currency left at the time of the invoice.
-            invoice_id (str): invoice_id is the unique ID representing the invoice.
-            invoice_items (List['InvoiceItem']): invoice_items are sorted by the cluster name.
-            period_end (datetime.datetime): period_end is the end of the billing period (exclusive).
-            period_start (datetime.datetime): period_start is the start of the billing period (inclusive).
-            totals (List['CurrencyAmount']): totals is a list of the total amounts per currency.
-            adjustments (Union[Unset, List['InvoiceAdjustment']]): adjustments is a list of credits or costs that adjust the
-                value of the
-                invoice (e.g. a Serverless Free Credit or Premium Support adjustment).
-                Unlike line items, adjustments are not tied to a particular cluster.
+            invoice_id (str): InvoiceID is the unique ID representing the invoice.
+            totals (List[CurrencyAmount]): Totals is a list of the total amounts per currency.
+            period_start (datetime.datetime): PeriodStart is the start of the billing period (inclusive).
+            period_end (datetime.datetime): PeriodEnd is the end of the billing period (exclusive).
+            invoice_items (List[InvoiceItem]): InvoiceItems are sorted by the cluster name.
+            balances (List[CurrencyAmount]): Balances are the amounts of currency left at the time of the invoice.
     """
 
-    balances: List["CurrencyAmount"]
     invoice_id: str
-    invoice_items: List["InvoiceItem"]
-    period_end: datetime.datetime
+    totals: List[CurrencyAmount]
     period_start: datetime.datetime
-    totals: List["CurrencyAmount"]
-    adjustments: Union[Unset, List["InvoiceAdjustment"]] = UNSET
+    period_end: datetime.datetime
+    invoice_items: List[InvoiceItem]
+    balances: List[CurrencyAmount]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        balances = []
-        for balances_item_data in self.balances:
-            balances_item = balances_item_data.to_dict()
+        invoice_id = self.invoice_id
+        totals = []
+        for totals_item_data in self.totals:
+            totals_item = totals_item_data.to_dict()
 
-            balances.append(balances_item)
+            totals.append(totals_item)
+
+        period_start = self.period_start.isoformat()
+
+        period_end = self.period_end.isoformat()
 
-        invoice_id = self.invoice_id
         invoice_items = []
         for invoice_items_item_data in self.invoice_items:
             invoice_items_item = invoice_items_item_data.to_dict()
 
             invoice_items.append(invoice_items_item)
 
-        period_end = self.period_end.isoformat()
-
-        period_start = self.period_start.isoformat()
-
-        totals = []
-        for totals_item_data in self.totals:
-            totals_item = totals_item_data.to_dict()
-
-            totals.append(totals_item)
-
-        adjustments: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.adjustments, Unset):
-            adjustments = []
-            for adjustments_item_data in self.adjustments:
-                adjustments_item = adjustments_item_data.to_dict()
+        balances = []
+        for balances_item_data in self.balances:
+            balances_item = balances_item_data.to_dict()
 
-                adjustments.append(adjustments_item)
+            balances.append(balances_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "balances": balances,
                 "invoice_id": invoice_id,
-                "invoice_items": invoice_items,
-                "period_end": period_end,
-                "period_start": period_start,
                 "totals": totals,
+                "period_start": period_start,
+                "period_end": period_end,
+                "invoice_items": invoice_items,
+                "balances": balances,
             }
         )
-        if adjustments is not UNSET:
-            field_dict["adjustments"] = adjustments
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.currency_amount import CurrencyAmount
-        from ..models.invoice_adjustment import InvoiceAdjustment
-        from ..models.invoice_item import InvoiceItem
-
         d = src_dict.copy()
-        balances = []
-        _balances = d.pop("balances")
-        for balances_item_data in _balances:
-            balances_item = CurrencyAmount.from_dict(balances_item_data)
+        invoice_id = d.pop("invoice_id")
 
-            balances.append(balances_item)
+        totals = []
+        _totals = d.pop("totals")
+        for totals_item_data in _totals:
+            totals_item = CurrencyAmount.from_dict(totals_item_data)
 
-        invoice_id = d.pop("invoice_id")
+            totals.append(totals_item)
+
+        period_start = isoparse(d.pop("period_start"))
+
+        period_end = isoparse(d.pop("period_end"))
 
         invoice_items = []
         _invoice_items = d.pop("invoice_items")
         for invoice_items_item_data in _invoice_items:
             invoice_items_item = InvoiceItem.from_dict(invoice_items_item_data)
 
             invoice_items.append(invoice_items_item)
 
-        period_end = isoparse(d.pop("period_end"))
-
-        period_start = isoparse(d.pop("period_start"))
-
-        totals = []
-        _totals = d.pop("totals")
-        for totals_item_data in _totals:
-            totals_item = CurrencyAmount.from_dict(totals_item_data)
-
-            totals.append(totals_item)
-
-        adjustments = []
-        _adjustments = d.pop("adjustments", UNSET)
-        for adjustments_item_data in _adjustments or []:
-            adjustments_item = InvoiceAdjustment.from_dict(adjustments_item_data)
+        balances = []
+        _balances = d.pop("balances")
+        for balances_item_data in _balances:
+            balances_item = CurrencyAmount.from_dict(balances_item_data)
 
-            adjustments.append(adjustments_item)
+            balances.append(balances_item)
 
         invoice = cls(
-            balances=balances,
             invoice_id=invoice_id,
-            invoice_items=invoice_items,
-            period_end=period_end,
-            period_start=period_start,
             totals=totals,
-            adjustments=adjustments,
+            period_start=period_start,
+            period_end=period_end,
+            invoice_items=invoice_items,
+            balances=balances,
         )
 
         invoice.additional_properties = d
         return invoice
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/invoice_item.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/invoice_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,88 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.cluster import Cluster
-    from ..models.currency_amount import CurrencyAmount
-    from ..models.line_item import LineItem
-
+from ..models.cluster import Cluster
+from ..models.currency_amount import CurrencyAmount
+from ..models.line_item import LineItem
 
 T = TypeVar("T", bound="InvoiceItem")
 
 
 @attr.s(auto_attribs=True)
 class InvoiceItem:
     """
     Attributes:
-        cluster (Cluster):  Example: {'account_id': '', 'cloud_provider': 'GCP', 'cockroach_version': 'v21.2.4',
-            'config': {'serverless': {'routing_id': 'example-cluster-1533', 'spend_limit': 0}}, 'created_at':
-            '2022-03-22T20:23:11.285067Z', 'creator_id': '7cde0cd9-0d8a-4008-8f90-45092ce8afc1', 'deleted_at': None, 'id':
-            '35c4abb2-bb66-46d7-afed-25ebef5ed2aa', 'name': 'example-cluster', 'operation_status':
-            'CLUSTER_STATUS_UNSPECIFIED', 'plan': 'SERVERLESS', 'regions': [{'name': 'us-central1', 'node_count': 0,
-            'sql_dns': 'free-tier7.gcp-us-central1.crdb.io', 'ui_dns': ''}], 'state': 'CREATED', 'updated_at':
-            '2022-03-22T20:23:11.879593Z', 'upgrade_status': 'USING_LATEST'}.
-        line_items (List['LineItem']): line_items contain all the relevant line items from the Metronome invoice.
-        totals (List['CurrencyAmount']): totals is a list of the total amounts of line items per currency.
+        cluster (Cluster):  Example: {'id': '35c4abb2-bb66-46d7-afed-25ebef5ed2aa', 'name': 'example-cluster',
+            'cockroach_version': 'v21.2.4', 'plan': 'SERVERLESS', 'cloud_provider': 'GCP', 'account_id': '', 'state':
+            'CREATED', 'creator_id': '7cde0cd9-0d8a-4008-8f90-45092ce8afc1', 'operation_status':
+            'CLUSTER_STATUS_UNSPECIFIED', 'config': {'serverless': {'spend_limit': 0, 'routing_id': 'example-
+            cluster-1533'}}, 'regions': [{'name': 'us-central1', 'sql_dns': 'free-tier7.gcp-us-central1.crdb.io', 'ui_dns':
+            '', 'node_count': 0}], 'created_at': '2022-03-22T20:23:11.285067Z', 'updated_at': '2022-03-22T20:23:11.879593Z',
+            'deleted_at': None}.
+        totals (List[CurrencyAmount]): Totals is a list of the total amounts of line items per currency.
+        line_items (List[LineItem]): LineItems contain all the relevant line items from the Metronome invoice.
     """
 
-    cluster: "Cluster"
-    line_items: List["LineItem"]
-    totals: List["CurrencyAmount"]
+    cluster: Cluster
+    totals: List[CurrencyAmount]
+    line_items: List[LineItem]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         cluster = self.cluster.to_dict()
 
-        line_items = []
-        for line_items_item_data in self.line_items:
-            line_items_item = line_items_item_data.to_dict()
-
-            line_items.append(line_items_item)
-
         totals = []
         for totals_item_data in self.totals:
             totals_item = totals_item_data.to_dict()
 
             totals.append(totals_item)
 
+        line_items = []
+        for line_items_item_data in self.line_items:
+            line_items_item = line_items_item_data.to_dict()
+
+            line_items.append(line_items_item)
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "cluster": cluster,
-                "line_items": line_items,
                 "totals": totals,
+                "line_items": line_items,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cluster import Cluster
-        from ..models.currency_amount import CurrencyAmount
-        from ..models.line_item import LineItem
-
         d = src_dict.copy()
         cluster = Cluster.from_dict(d.pop("cluster"))
 
-        line_items = []
-        _line_items = d.pop("line_items")
-        for line_items_item_data in _line_items:
-            line_items_item = LineItem.from_dict(line_items_item_data)
-
-            line_items.append(line_items_item)
-
         totals = []
         _totals = d.pop("totals")
         for totals_item_data in _totals:
             totals_item = CurrencyAmount.from_dict(totals_item_data)
 
             totals.append(totals_item)
 
+        line_items = []
+        _line_items = d.pop("line_items")
+        for line_items_item_data in _line_items:
+            line_items_item = LineItem.from_dict(line_items_item_data)
+
+            line_items.append(line_items_item)
+
         invoice_item = cls(
             cluster=cluster,
-            line_items=line_items,
             totals=totals,
+            line_items=line_items,
         )
 
         invoice_item.additional_properties = d
         return invoice_item
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/keyset_pagination_request.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/keyset_pagination_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,82 +10,76 @@
 T = TypeVar("T", bound="KeysetPaginationRequest")
 
 
 @attr.s(auto_attribs=True)
 class KeysetPaginationRequest:
     """
     Attributes:
-        as_of_time (Union[Unset, datetime.datetime]):
-        limit (Union[Unset, int]):
         page (Union[Unset, str]):
-        sort_order (Union[Unset, SortOrder]):  - ASC: Sort in ascending order. This is the default unless otherwise
-            specified.
-             - DESC: Sort in descending order.
+        limit (Union[Unset, int]):
+        as_of_time (Union[Unset, datetime.datetime]):
+        sort_order (Union[Unset, SortOrder]):  - DESC: Sort in descending order. The default order is ascending.
     """
 
-    as_of_time: Union[Unset, datetime.datetime] = UNSET
-    limit: Union[Unset, int] = UNSET
     page: Union[Unset, str] = UNSET
+    limit: Union[Unset, int] = UNSET
+    as_of_time: Union[Unset, datetime.datetime] = UNSET
     sort_order: Union[Unset, SortOrder] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        page = self.page
+        limit = self.limit
         as_of_time: Union[Unset, str] = UNSET
         if not isinstance(self.as_of_time, Unset):
             as_of_time = self.as_of_time.isoformat()
 
-        limit = self.limit
-        page = self.page
         sort_order: Union[Unset, str] = UNSET
         if not isinstance(self.sort_order, Unset):
             sort_order = self.sort_order.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if as_of_time is not UNSET:
-            field_dict["as_of_time"] = as_of_time
-        if limit is not UNSET:
-            field_dict["limit"] = limit
         if page is not UNSET:
             field_dict["page"] = page
+        if limit is not UNSET:
+            field_dict["limit"] = limit
+        if as_of_time is not UNSET:
+            field_dict["as_of_time"] = as_of_time
         if sort_order is not UNSET:
             field_dict["sort_order"] = sort_order
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        page = d.pop("page", UNSET)
+
+        limit = d.pop("limit", UNSET)
+
         _as_of_time = d.pop("as_of_time", UNSET)
         as_of_time: Union[Unset, datetime.datetime]
-        if _as_of_time is None:
-            as_of_time = None
         if isinstance(_as_of_time, Unset):
             as_of_time = UNSET
         else:
             as_of_time = isoparse(_as_of_time)
 
-        limit = d.pop("limit", UNSET)
-
-        page = d.pop("page", UNSET)
-
         _sort_order = d.pop("sort_order", UNSET)
         sort_order: Union[Unset, SortOrder]
-        if _sort_order is None:
-            sort_order = None
         if isinstance(_sort_order, Unset):
             sort_order = UNSET
         else:
             sort_order = SortOrder(_sort_order)
 
         keyset_pagination_request = cls(
-            as_of_time=as_of_time,
-            limit=limit,
             page=page,
+            limit=limit,
+            as_of_time=as_of_time,
             sort_order=sort_order,
         )
 
         keyset_pagination_request.additional_properties = d
         return keyset_pagination_request
 
     @property
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/line_item.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/line_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,77 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
+from ..models.currency_amount import CurrencyAmount
 from ..models.quantity_unit_type import QuantityUnitType
 
-if TYPE_CHECKING:
-    from ..models.currency_amount import CurrencyAmount
-
-
 T = TypeVar("T", bound="LineItem")
 
 
 @attr.s(auto_attribs=True)
 class LineItem:
     """
     Attributes:
-        description (str): description contains the details of the line item (i.e t3 micro).
-        quantity (float): quantity is the number of the specific line items used.
-        quantity_unit (QuantityUnitType):
+        description (str): Description contains the details of the line item (i.e t3 micro).
+        quantity (float): Quantity is the number of the specific line items used.
+        unit_cost (float): UnitCost is the cost per unit of line item.
         total (CurrencyAmount):
-        unit_cost (float): unit_cost is the cost per unit of line item.
+        quantity_unit (QuantityUnitType): Billing
+            QuantityUnitType is the unit type for a quantity of billing line item.
     """
 
     description: str
     quantity: float
-    quantity_unit: QuantityUnitType
-    total: "CurrencyAmount"
     unit_cost: float
+    total: CurrencyAmount
+    quantity_unit: QuantityUnitType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         description = self.description
         quantity = self.quantity
-        quantity_unit = self.quantity_unit.value
-
+        unit_cost = self.unit_cost
         total = self.total.to_dict()
 
-        unit_cost = self.unit_cost
+        quantity_unit = self.quantity_unit.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "description": description,
                 "quantity": quantity,
-                "quantity_unit": quantity_unit,
-                "total": total,
                 "unit_cost": unit_cost,
+                "total": total,
+                "quantity_unit": quantity_unit,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.currency_amount import CurrencyAmount
-
         d = src_dict.copy()
         description = d.pop("description")
 
         quantity = d.pop("quantity")
 
-        quantity_unit = QuantityUnitType(d.pop("quantity_unit"))
+        unit_cost = d.pop("unit_cost")
 
         total = CurrencyAmount.from_dict(d.pop("total"))
 
-        unit_cost = d.pop("unit_cost")
+        quantity_unit = QuantityUnitType(d.pop("quantity_unit"))
 
         line_item = cls(
             description=description,
             quantity=quantity,
-            quantity_unit=quantity_unit,
-            total=total,
             unit_cost=unit_cost,
+            total=total,
+            quantity_unit=quantity_unit,
         )
 
         line_item.additional_properties = d
         return line_item
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_allowlist_entries_response.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_allowlist_entries_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.allowlist_entry import AllowlistEntry
+from ..models.keyset_pagination_response import KeysetPaginationResponse
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.allowlist_entry import AllowlistEntry
-    from ..models.keyset_pagination_response import KeysetPaginationResponse
-
-
 T = TypeVar("T", bound="ListAllowlistEntriesResponse")
 
 
 @attr.s(auto_attribs=True)
 class ListAllowlistEntriesResponse:
     """
     Attributes:
-        allowlist (List['AllowlistEntry']):
+        allowlist (List[AllowlistEntry]):
         propagating (bool):
         pagination (Union[Unset, KeysetPaginationResponse]):
     """
 
-    allowlist: List["AllowlistEntry"]
+    allowlist: List[AllowlistEntry]
     propagating: bool
-    pagination: Union[Unset, "KeysetPaginationResponse"] = UNSET
+    pagination: Union[Unset, KeysetPaginationResponse] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         allowlist = []
         for allowlist_item_data in self.allowlist:
             allowlist_item = allowlist_item_data.to_dict()
 
@@ -49,31 +46,26 @@
         if pagination is not UNSET:
             field_dict["pagination"] = pagination
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.allowlist_entry import AllowlistEntry
-        from ..models.keyset_pagination_response import KeysetPaginationResponse
-
         d = src_dict.copy()
         allowlist = []
         _allowlist = d.pop("allowlist")
         for allowlist_item_data in _allowlist:
             allowlist_item = AllowlistEntry.from_dict(allowlist_item_data)
 
             allowlist.append(allowlist_item)
 
         propagating = d.pop("propagating")
 
         _pagination = d.pop("pagination", UNSET)
         pagination: Union[Unset, KeysetPaginationResponse]
-        if _pagination is None:
-            pagination = None
         if isinstance(_pagination, Unset):
             pagination = UNSET
         else:
             pagination = KeysetPaginationResponse.from_dict(_pagination)
 
         list_allowlist_entries_response = cls(
             allowlist=allowlist,
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_available_regions_response.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_cluster_nodes_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,77 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.keyset_pagination_response import KeysetPaginationResponse
+from ..models.node import Node
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cloud_provider_region import CloudProviderRegion
-    from ..models.keyset_pagination_response import KeysetPaginationResponse
-
-
-T = TypeVar("T", bound="ListAvailableRegionsResponse")
+T = TypeVar("T", bound="ListClusterNodesResponse")
 
 
 @attr.s(auto_attribs=True)
-class ListAvailableRegionsResponse:
+class ListClusterNodesResponse:
     """
     Attributes:
-        regions (List['CloudProviderRegion']):
+        nodes (List[Node]):
         pagination (Union[Unset, KeysetPaginationResponse]):
     """
 
-    regions: List["CloudProviderRegion"]
-    pagination: Union[Unset, "KeysetPaginationResponse"] = UNSET
+    nodes: List[Node]
+    pagination: Union[Unset, KeysetPaginationResponse] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        regions = []
-        for regions_item_data in self.regions:
-            regions_item = regions_item_data.to_dict()
+        nodes = []
+        for nodes_item_data in self.nodes:
+            nodes_item = nodes_item_data.to_dict()
 
-            regions.append(regions_item)
+            nodes.append(nodes_item)
 
         pagination: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.pagination, Unset):
             pagination = self.pagination.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "regions": regions,
+                "nodes": nodes,
             }
         )
         if pagination is not UNSET:
             field_dict["pagination"] = pagination
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cloud_provider_region import CloudProviderRegion
-        from ..models.keyset_pagination_response import KeysetPaginationResponse
-
         d = src_dict.copy()
-        regions = []
-        _regions = d.pop("regions")
-        for regions_item_data in _regions:
-            regions_item = CloudProviderRegion.from_dict(regions_item_data)
+        nodes = []
+        _nodes = d.pop("nodes")
+        for nodes_item_data in _nodes:
+            nodes_item = Node.from_dict(nodes_item_data)
 
-            regions.append(regions_item)
+            nodes.append(nodes_item)
 
         _pagination = d.pop("pagination", UNSET)
         pagination: Union[Unset, KeysetPaginationResponse]
-        if _pagination is None:
-            pagination = None
         if isinstance(_pagination, Unset):
             pagination = UNSET
         else:
             pagination = KeysetPaginationResponse.from_dict(_pagination)
 
-        list_available_regions_response = cls(
-            regions=regions,
+        list_cluster_nodes_response = cls(
+            nodes=nodes,
             pagination=pagination,
         )
 
-        list_available_regions_response.additional_properties = d
-        return list_available_regions_response
+        list_cluster_nodes_response.additional_properties = d
+        return list_cluster_nodes_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/list_clusters_response.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/list_databases_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,77 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.database import Database
+from ..models.keyset_pagination_response import KeysetPaginationResponse
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cluster import Cluster
-    from ..models.keyset_pagination_response import KeysetPaginationResponse
-
-
-T = TypeVar("T", bound="ListClustersResponse")
+T = TypeVar("T", bound="ListDatabasesResponse")
 
 
 @attr.s(auto_attribs=True)
-class ListClustersResponse:
+class ListDatabasesResponse:
     """
     Attributes:
-        clusters (List['Cluster']):
+        databases (List[Database]):
         pagination (Union[Unset, KeysetPaginationResponse]):
     """
 
-    clusters: List["Cluster"]
-    pagination: Union[Unset, "KeysetPaginationResponse"] = UNSET
+    databases: List[Database]
+    pagination: Union[Unset, KeysetPaginationResponse] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        clusters = []
-        for clusters_item_data in self.clusters:
-            clusters_item = clusters_item_data.to_dict()
+        databases = []
+        for databases_item_data in self.databases:
+            databases_item = databases_item_data.to_dict()
 
-            clusters.append(clusters_item)
+            databases.append(databases_item)
 
         pagination: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.pagination, Unset):
             pagination = self.pagination.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "clusters": clusters,
+                "databases": databases,
             }
         )
         if pagination is not UNSET:
             field_dict["pagination"] = pagination
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cluster import Cluster
-        from ..models.keyset_pagination_response import KeysetPaginationResponse
-
         d = src_dict.copy()
-        clusters = []
-        _clusters = d.pop("clusters")
-        for clusters_item_data in _clusters:
-            clusters_item = Cluster.from_dict(clusters_item_data)
+        databases = []
+        _databases = d.pop("databases")
+        for databases_item_data in _databases:
+            databases_item = Database.from_dict(databases_item_data)
 
-            clusters.append(clusters_item)
+            databases.append(databases_item)
 
         _pagination = d.pop("pagination", UNSET)
         pagination: Union[Unset, KeysetPaginationResponse]
-        if _pagination is None:
-            pagination = None
         if isinstance(_pagination, Unset):
             pagination = UNSET
         else:
             pagination = KeysetPaginationResponse.from_dict(_pagination)
 
-        list_clusters_response = cls(
-            clusters=clusters,
+        list_databases_response = cls(
+            databases=databases,
             pagination=pagination,
         )
 
-        list_clusters_response.additional_properties = d
-        return list_clusters_response
+        list_databases_response.additional_properties = d
+        return list_databases_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/node.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/region.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.node_status_type import NodeStatusType
-
-T = TypeVar("T", bound="Node")
+T = TypeVar("T", bound="Region")
 
 
 @attr.s(auto_attribs=True)
-class Node:
+class Region:
     """
     Attributes:
         name (str):
-        region_name (str):
-        status (NodeStatusType):
+        sql_dns (str):
+        ui_dns (str):
+        node_count (int): NodeCount will be 0 for serverless clusters.
     """
 
     name: str
-    region_name: str
-    status: NodeStatusType
+    sql_dns: str
+    ui_dns: str
+    node_count: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
-        region_name = self.region_name
-        status = self.status.value
+        sql_dns = self.sql_dns
+        ui_dns = self.ui_dns
+        node_count = self.node_count
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
-                "region_name": region_name,
-                "status": status,
+                "sql_dns": sql_dns,
+                "ui_dns": ui_dns,
+                "node_count": node_count,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
-        region_name = d.pop("region_name")
+        sql_dns = d.pop("sql_dns")
+
+        ui_dns = d.pop("ui_dns")
 
-        status = NodeStatusType(d.pop("status"))
+        node_count = d.pop("node_count")
 
-        node = cls(
+        region = cls(
             name=name,
-            region_name=region_name,
-            status=status,
+            sql_dns=sql_dns,
+            ui_dns=ui_dns,
+            node_count=node_count,
         )
 
-        node.additional_properties = d
-        return node
+        region.additional_properties = d
+        return region
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/private_endpoint_services.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/private_endpoint_services.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.private_endpoint_service import PrivateEndpointService
-
+from ..models.private_endpoint_service import PrivateEndpointService
 
 T = TypeVar("T", bound="PrivateEndpointServices")
 
 
 @attr.s(auto_attribs=True)
 class PrivateEndpointServices:
     """
     Attributes:
-        services (List['PrivateEndpointService']): services contains a list of all cluster related services.
+        services (List[PrivateEndpointService]): Services contains a list of all cluster related services.
     """
 
-    services: List["PrivateEndpointService"]
+    services: List[PrivateEndpointService]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         services = []
         for services_item_data in self.services:
             services_item = services_item_data.to_dict()
 
@@ -34,16 +32,14 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.private_endpoint_service import PrivateEndpointService
-
         d = src_dict.copy()
         services = []
         _services = d.pop("services")
         for services_item_data in _services:
             services_item = PrivateEndpointService.from_dict(services_item_data)
 
             services.append(services_item)
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/models/sql_user.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/models/serverless_cluster_update_specification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SQLUser")
+T = TypeVar("T", bound="ServerlessClusterUpdateSpecification")
 
 
 @attr.s(auto_attribs=True)
-class SQLUser:
+class ServerlessClusterUpdateSpecification:
     """
     Attributes:
-        name (str):
+        spend_limit (int):
     """
 
-    name: str
+    spend_limit: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
+        spend_limit = self.spend_limit
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "name": name,
+                "spend_limit": spend_limit,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
+        spend_limit = d.pop("spend_limit")
 
-        sql_user = cls(
-            name=name,
+        serverless_cluster_update_specification = cls(
+            spend_limit=spend_limit,
         )
 
-        sql_user.additional_properties = d
-        return sql_user
+        serverless_cluster_update_specification.additional_properties = d
+        return serverless_cluster_update_specification
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cockroachdb_cloud_client-0.1.1/cockroachdb_cloud_client/types.py` & `cockroachdb_cloud_client-2022.9.20/cockroachdb_cloud_client/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """ Contains some shared types for properties """
-from http import HTTPStatus
 from typing import BinaryIO, Generic, MutableMapping, Optional, Tuple, TypeVar
 
 import attr
 
 
 class Unset:
     def __bool__(self) -> bool:
@@ -31,14 +30,14 @@
 T = TypeVar("T")
 
 
 @attr.s(auto_attribs=True)
 class Response(Generic[T]):
     """A response from an endpoint"""
 
-    status_code: HTTPStatus
+    status_code: int
     content: bytes
     headers: MutableMapping[str, str]
     parsed: Optional[T]
 
 
 __all__ = ["File", "Response", "FileJsonType"]
```

### Comparing `cockroachdb_cloud_client-0.1.1/pyproject.toml` & `cockroachdb_cloud_client-2022.9.20/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 [tool.poetry]
 name = "cockroachdb_cloud_client"
-version = "0.1.1"
+version = "2022.09.20"
 description = "A client library for accessing CockroachDB Cloud API"
 
-authors = ['Fabio Ghirardello']
-homepage = "https://www.cockroachlabs.com/docs/api/cloud/v1.html#get-/api/v1/clusters"
-repository = "https://github.com/fabiog1901/cockroachdb_cloud_client"
-license = "GPL-3.0-or-later"
+authors = ['Cockroach Labs']
 
 readme = "README.md"
-
-documentation = "https://www.cockroachlabs.com/docs/"
-
 packages = [
     {include = "cockroachdb_cloud_client"},
 ]
 include = ["CHANGELOG.md", "cockroachdb_cloud_client/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

