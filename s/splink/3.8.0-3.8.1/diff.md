# Comparing `tmp/splink-3.8.0.tar.gz` & `tmp/splink-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.8.0.tar", max compression
+gzip compressed data, was "splink-3.8.1.tar", max compression
```

## Comparing `splink-3.8.0.tar` & `splink-3.8.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0     1076 2023-04-25 14:03:55.263020 splink-3.8.0/LICENSE
--rw-r--r--   0        0        0     8448 2023-04-25 14:03:55.263020 splink-3.8.0/README.md
--rw-r--r--   0        0        0     1451 2023-04-25 14:03:55.283021 splink-3.8.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-04-25 14:03:55.283021 splink-3.8.0/splink/__init__.py
--rw-r--r--   0        0        0    10852 2023-04-25 14:03:55.283021 splink-3.8.0/splink/accuracy.py
--rw-r--r--   0        0        0     4753 2023-04-25 14:03:55.283021 splink-3.8.0/splink/analyse_blocking.py
--rw-r--r--   0        0        0      461 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_base.py
--rw-r--r--   0        0        0     1672 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0     1015 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0    20569 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_linker.py
--rw-r--r--   0        0        0      350 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_transforms.py
--rw-r--r--   0        0        0     2904 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_utils.py
--rw-r--r--   0        0        0     2867 2023-04-25 14:03:55.283021 splink-3.8.0/splink/block_from_labels.py
--rw-r--r--   0        0        0     5965 2023-04-25 14:03:55.283021 splink-3.8.0/splink/blocking.py
--rw-r--r--   0        0        0    10627 2023-04-25 14:03:55.283021 splink-3.8.0/splink/charts.py
--rw-r--r--   0        0        0     9088 2023-04-25 14:03:55.283021 splink-3.8.0/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison.py
--rw-r--r--   0        0        0    25479 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level.py
--rw-r--r--   0        0        0     9013 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    25022 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    35793 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_library.py
--rw-r--r--   0        0        0     4315 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    23009 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16516 2023-04-25 14:03:55.287021 splink-3.8.0/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-04-25 14:03:55.287021 splink-3.8.0/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-04-25 14:03:55.287021 splink-3.8.0/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-04-25 14:03:55.287021 splink-3.8.0/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0      609 2023-04-25 14:03:55.287021 splink-3.8.0/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1332 2023-04-25 14:03:55.287021 splink-3.8.0/splink/dialect_base.py
--rw-r--r--   0        0        0     1332 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_base.py
--rw-r--r--   0        0        0     2369 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0     1823 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      543 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1750 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_helpers.py
--rw-r--r--   0        0        0     9974 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    17471 2023-04-25 14:03:55.287021 splink-3.8.0/splink/em_training_session.py
--rw-r--r--   0        0        0     5244 2023-04-25 14:03:55.287021 splink-3.8.0/splink/estimate_u.py
--rw-r--r--   0        0        0      144 2023-04-25 14:03:55.287021 splink-3.8.0/splink/exceptions.py
--rw-r--r--   0        0        0     6062 2023-04-25 14:03:55.287021 splink-3.8.0/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1558 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     2779 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     6737 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
--rw-r--r--   0        0        0     7747 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
--rw-r--r--   0        0        0     6298 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/compare_estimates.json
--rw-r--r--   0        0        0     2155 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json
--rw-r--r--   0        0        0      743 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/gamma_histogram.json
--rw-r--r--   0        0        0     1309 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/score_histogram.json
--rw-r--r--   0        0        0     5831 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0      977 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5766 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9159 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1734 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     1730 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1465 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1123 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1745 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     2645 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-04-25 14:03:55.291021 splink-3.8.0/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-04-25 14:03:55.291021 splink-3.8.0/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0    12871 2023-04-25 14:03:55.291021 splink-3.8.0/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-04-25 14:03:55.303022 splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     5486 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/templates/single_chart_template.txt
--rw-r--r--   0        0        0      195 2023-04-25 14:03:55.307022 splink-3.8.0/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-04-25 14:03:55.307022 splink-3.8.0/splink/input_column.py
--rw-r--r--   0        0        0   119034 2023-04-25 14:03:55.311022 splink-3.8.0/splink/linker.py
--rw-r--r--   0        0        0      300 2023-04-25 14:03:55.311022 splink-3.8.0/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-04-25 14:03:55.311022 splink-3.8.0/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-04-25 14:03:55.311022 splink-3.8.0/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-04-25 14:03:55.311022 splink-3.8.0/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-04-25 14:03:55.311022 splink-3.8.0/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-04-25 14:03:55.311022 splink-3.8.0/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-04-25 14:03:55.311022 splink-3.8.0/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     4386 2023-04-25 14:03:55.311022 splink-3.8.0/splink/misc.py
--rw-r--r--   0        0        0     2791 2023-04-25 14:03:55.311022 splink-3.8.0/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-04-25 14:03:55.311022 splink-3.8.0/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-04-25 14:03:55.311022 splink-3.8.0/splink/pipeline.py
--rw-r--r--   0        0        0     3205 2023-04-25 14:03:55.311022 splink-3.8.0/splink/predict.py
--rw-r--r--   0        0        0     8245 2023-04-25 14:03:55.311022 splink-3.8.0/splink/profile_data.py
--rw-r--r--   0        0        0    18517 2023-04-25 14:03:55.311022 splink-3.8.0/splink/settings.py
--rw-r--r--   0        0        0     1083 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/custom_spark_dialect.py
--rw-r--r--   0        0        0      473 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/jar_location.py
--rw-r--r--   0        0        0     1641 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_base.py
--rw-r--r--   0        0        0     2300 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0     1812 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      538 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0    22331 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4507 2023-04-25 14:03:55.311022 splink-3.8.0/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     3220 2023-04-25 14:03:55.311022 splink-3.8.0/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1181 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sql_transform.py
--rw-r--r--   0        0        0      147 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_base.py
--rw-r--r--   0        0        0     1109 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      379 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0     6052 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0     4453 2023-04-25 14:03:55.311022 splink-3.8.0/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-04-25 14:03:55.311022 splink-3.8.0/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1424 2023-04-25 14:03:55.311022 splink-3.8.0/splink/unlinkables.py
--rw-r--r--   0        0        0     2431 2023-04-25 14:03:55.311022 splink-3.8.0/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2326 2023-04-25 14:03:55.311022 splink-3.8.0/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-04-25 14:03:55.311022 splink-3.8.0/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 splink-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-27 19:35:50.176911 splink-3.8.1/LICENSE
+-rw-r--r--   0        0        0     8448 2023-04-27 19:35:50.176911 splink-3.8.1/README.md
+-rw-r--r--   0        0        0     1451 2023-04-27 19:35:50.204911 splink-3.8.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-04-27 19:35:50.204911 splink-3.8.1/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-04-27 19:35:50.204911 splink-3.8.1/splink/accuracy.py
+-rw-r--r--   0        0        0     4759 2023-04-27 19:35:50.204911 splink-3.8.1/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      461 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_base.py
+-rw-r--r--   0        0        0     1672 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0     1015 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0    20569 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0      350 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_transforms.py
+-rw-r--r--   0        0        0     2904 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_utils.py
+-rw-r--r--   0        0        0     2867 2023-04-27 19:35:50.204911 splink-3.8.1/splink/block_from_labels.py
+-rw-r--r--   0        0        0     5965 2023-04-27 19:35:50.204911 splink-3.8.1/splink/blocking.py
+-rw-r--r--   0        0        0    10627 2023-04-27 19:35:50.204911 splink-3.8.1/splink/charts.py
+-rw-r--r--   0        0        0     9088 2023-04-27 19:35:50.204911 splink-3.8.1/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison.py
+-rw-r--r--   0        0        0    25479 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level.py
+-rw-r--r--   0        0        0     9013 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    25022 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    35793 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_library.py
+-rw-r--r--   0        0        0     4315 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    23009 2023-04-27 19:35:50.208911 splink-3.8.1/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-04-27 19:35:50.208911 splink-3.8.1/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-04-27 19:35:50.208911 splink-3.8.1/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16516 2023-04-27 19:35:50.208911 splink-3.8.1/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-04-27 19:35:50.208911 splink-3.8.1/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-04-27 19:35:50.208911 splink-3.8.1/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-04-27 19:35:50.208911 splink-3.8.1/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0      609 2023-04-27 19:35:50.208911 splink-3.8.1/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1332 2023-04-27 19:35:50.208911 splink-3.8.1/splink/dialect_base.py
+-rw-r--r--   0        0        0     1332 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_base.py
+-rw-r--r--   0        0        0     2369 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0     1823 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      543 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1750 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_helpers.py
+-rw-r--r--   0        0        0     9974 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    17471 2023-04-27 19:35:50.208911 splink-3.8.1/splink/em_training_session.py
+-rw-r--r--   0        0        0     5244 2023-04-27 19:35:50.208911 splink-3.8.1/splink/estimate_u.py
+-rw-r--r--   0        0        0      144 2023-04-27 19:35:50.208911 splink-3.8.1/splink/exceptions.py
+-rw-r--r--   0        0        0     6062 2023-04-27 19:35:50.208911 splink-3.8.1/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1558 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     2779 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     6737 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
+-rw-r--r--   0        0        0     7747 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
+-rw-r--r--   0        0        0     6298 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/compare_estimates.json
+-rw-r--r--   0        0        0     2155 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json
+-rw-r--r--   0        0        0      743 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/gamma_histogram.json
+-rw-r--r--   0        0        0     1309 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/score_histogram.json
+-rw-r--r--   0        0        0     5831 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0      977 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5766 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9159 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1734 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     1730 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1465 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1123 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1745 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     2645 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-04-27 19:35:50.212911 splink-3.8.1/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-04-27 19:35:50.212911 splink-3.8.1/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0    12871 2023-04-27 19:35:50.212911 splink-3.8.1/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-04-27 19:35:50.224911 splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/templates/single_chart_template.txt
+-rw-r--r--   0        0        0      195 2023-04-27 19:35:50.228911 splink-3.8.1/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-04-27 19:35:50.232911 splink-3.8.1/splink/input_column.py
+-rw-r--r--   0        0        0   120307 2023-04-27 19:35:50.232911 splink-3.8.1/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-04-27 19:35:50.232911 splink-3.8.1/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-04-27 19:35:50.232911 splink-3.8.1/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-04-27 19:35:50.232911 splink-3.8.1/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-04-27 19:35:50.232911 splink-3.8.1/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-04-27 19:35:50.232911 splink-3.8.1/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-04-27 19:35:50.232911 splink-3.8.1/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-04-27 19:35:50.232911 splink-3.8.1/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     4548 2023-04-27 19:35:50.232911 splink-3.8.1/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-04-27 19:35:50.232911 splink-3.8.1/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-04-27 19:35:50.232911 splink-3.8.1/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-04-27 19:35:50.232911 splink-3.8.1/splink/pipeline.py
+-rw-r--r--   0        0        0     3205 2023-04-27 19:35:50.232911 splink-3.8.1/splink/predict.py
+-rw-r--r--   0        0        0     8245 2023-04-27 19:35:50.232911 splink-3.8.1/splink/profile_data.py
+-rw-r--r--   0        0        0    18694 2023-04-27 19:35:50.232911 splink-3.8.1/splink/settings.py
+-rw-r--r--   0        0        0     1083 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/custom_spark_dialect.py
+-rw-r--r--   0        0        0      473 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/jar_location.py
+-rw-r--r--   0        0        0     1641 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_base.py
+-rw-r--r--   0        0        0     2300 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0     1812 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      538 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0    22331 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4507 2023-04-27 19:35:50.232911 splink-3.8.1/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     3220 2023-04-27 19:35:50.232911 splink-3.8.1/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1181 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sql_transform.py
+-rw-r--r--   0        0        0      147 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_base.py
+-rw-r--r--   0        0        0     1109 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      379 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0     6052 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0     4453 2023-04-27 19:35:50.232911 splink-3.8.1/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-04-27 19:35:50.232911 splink-3.8.1/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1424 2023-04-27 19:35:50.232911 splink-3.8.1/splink/unlinkables.py
+-rw-r--r--   0        0        0     2431 2023-04-27 19:35:50.232911 splink-3.8.1/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-04-27 19:35:50.232911 splink-3.8.1/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-04-27 19:35:50.232911 splink-3.8.1/splink/waterfall_chart.py
+-rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 splink-3.8.1/PKG-INFO
```

### Comparing `splink-3.8.0/LICENSE` & `splink-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/README.md` & `splink-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/pyproject.toml` & `splink-3.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splink"
-version = "3.8.0"
+version = "3.8.1"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
```

### Comparing `splink-3.8.0/splink/accuracy.py` & `splink-3.8.1/splink/accuracy.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/analyse_blocking.py` & `splink-3.8.1/splink/analyse_blocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
             cl._level_dict["tf_adjustment_column"] = None
 
     concat = linker._initialise_df_concat(materialise=True)
 
     # Calculate the Cartesian Product
     if output_chart:
         # We only need the cartesian product if we want to output the chart view
-        if len(linker._input_tables_dict) == 1:
+
+        if settings_obj._link_type == "dedupe_only":
             group_by_statement = ""
         else:
             group_by_statement = "group by source_dataset"
 
         sql = f"""
             select count(*) as count
             from {concat.physical_name}
```

### Comparing `splink-3.8.0/splink/athena/athena_comparison_level_library.py` & `splink-3.8.1/splink/athena/athena_comparison_level_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/athena/athena_comparison_library.py` & `splink-3.8.1/splink/athena/athena_comparison_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/athena/athena_linker.py` & `splink-3.8.1/splink/athena/athena_linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/athena/athena_utils.py` & `splink-3.8.1/splink/athena/athena_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/block_from_labels.py` & `splink-3.8.1/splink/block_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/blocking.py` & `splink-3.8.1/splink/blocking.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/charts.py` & `splink-3.8.1/splink/charts.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/cluster_studio.py` & `splink-3.8.1/splink/cluster_studio.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison.py` & `splink-3.8.1/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_level.py` & `splink-3.8.1/splink/comparison_level.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_level_composition.py` & `splink-3.8.1/splink/comparison_level_composition.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_level_library.py` & `splink-3.8.1/splink/comparison_level_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_level_sql.py` & `splink-3.8.1/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_library.py` & `splink-3.8.1/splink/comparison_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_library_utils.py` & `splink-3.8.1/splink/comparison_library_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_template_library.py` & `splink-3.8.1/splink/comparison_template_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_vector_distribution.py` & `splink-3.8.1/splink/comparison_vector_distribution.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/comparison_vector_values.py` & `splink-3.8.1/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/connected_components.py` & `splink-3.8.1/splink/connected_components.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/convert_v2_to_v3.py` & `splink-3.8.1/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/databricks/enable_splink.py` & `splink-3.8.1/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/default_from_jsonschema.py` & `splink-3.8.1/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/dialect_base.py` & `splink-3.8.1/splink/dialect_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/duckdb/duckdb_base.py` & `splink-3.8.1/splink/duckdb/duckdb_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/duckdb/duckdb_comparison_level_library.py` & `splink-3.8.1/splink/duckdb/duckdb_comparison_level_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/duckdb/duckdb_comparison_library.py` & `splink-3.8.1/splink/duckdb/duckdb_comparison_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/duckdb/duckdb_comparison_template_library.py` & `splink-3.8.1/splink/duckdb/duckdb_comparison_template_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/duckdb/duckdb_helpers.py` & `splink-3.8.1/splink/duckdb/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/duckdb/duckdb_linker.py` & `splink-3.8.1/splink/duckdb/duckdb_linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/em_training_session.py` & `splink-3.8.1/splink/em_training_session.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/estimate_u.py` & `splink-3.8.1/splink/estimate_u.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/expectation_maximisation.py` & `splink-3.8.1/splink/expectation_maximisation.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.8.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/completeness.json` & `splink-3.8.1/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json` & `splink-3.8.1/splink/files/chart_defs/del/bayes_factor_history_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json` & `splink-3.8.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/del/compare_estimates.json` & `splink-3.8.1/splink/files/chart_defs/del/compare_estimates.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json` & `splink-3.8.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/del/gamma_histogram.json` & `splink-3.8.1/splink/files/chart_defs/del/gamma_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/del/score_histogram.json` & `splink-3.8.1/splink/files/chart_defs/del/score_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.8.1/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.8.1/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.8.1/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.8.1/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/missingness.json` & `splink-3.8.1/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.8.1/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/precision_recall.json` & `splink-3.8.1/splink/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-3.8.1/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/profile_data.json` & `splink-3.8.1/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/roc.json` & `splink-3.8.1/splink/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.8.1/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/external_js/vega-embed@6.20.2` & `splink-3.8.1/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/external_js/vega-lite@5.2.0` & `splink-3.8.1/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/external_js/vega@5.21.0` & `splink-3.8.1/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/settings_jsonschema.json` & `splink-3.8.1/splink/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.8.1/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/splink_cluster_studio/custom.css` & `splink-3.8.1/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/splink_comparison_viewer/custom.css` & `splink-3.8.1/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/splink_comparison_viewer/template.j2` & `splink-3.8.1/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.8.1/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/input_column.py` & `splink-3.8.1/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/linker.py` & `splink-3.8.1/splink/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 )
 from .match_weights_histogram import histogram_data
 from .misc import (
     ascii_uid,
     bayes_factor_to_prob,
     ensure_is_list,
     ensure_is_tuple,
+    find_unique_source_dataset,
     prob_to_bayes_factor,
 )
 from .missingness import completeness_data, missingness_data
 from .pipeline import SQLPipeline
 from .predict import predict_from_comparison_vectors_sqls
 from .profile_data import profile_columns
 from .settings import Settings
@@ -287,16 +288,15 @@
             return None
 
         # Used throughout the scripts to feed our SQL
         if self._settings_obj._source_dataset_column_name_is_required:
             df_obj = next(iter(self._input_tables_dict.values()))
             columns = df_obj.columns_escaped
 
-            input_column = self._settings_obj._source_dataset_input_column
-            src_ds_col = InputColumn(input_column, self).name()
+            input_column, src_ds_col = self._settings_obj_._source_dataset_col
             return "__splink_source_dataset" if src_ds_col in columns else input_column
         else:
             return None
 
     @property
     def _two_dataset_link_only(self):
         # Two dataset link only join is a special case where an inner join of the
@@ -336,14 +336,43 @@
 
     @property
     def _infinity_expression(self):
         raise NotImplementedError(
             f"infinity sql expression not available for {type(self)}"
         )
 
+    @property
+    def _verify_link_only_job(self):
+
+        cache = self._intermediate_table_cache
+        if "__splink__df_concat_with_tf" not in cache:
+            return
+
+        if self._settings_obj._link_type == "link_only":
+            # if input datasets > 1 then skip
+            if len(self._input_tables_dict) > 1:
+                return
+
+            # else, check if source dataset column is populated...
+            src_ds = self._source_dataset_column_name
+            if src_ds == "__splink_source_dataset":
+                _, src_ds = self._settings_obj_._source_dataset_col
+
+            sql = find_unique_source_dataset(src_ds)
+            self._enqueue_sql(sql, "source_ds_distinct")
+            src_ds_distinct = self._execute_sql_pipeline(
+                [cache["__splink__df_concat_with_tf"]]
+            )
+            if len(src_ds_distinct.as_record_dict()) == 1:
+                raise SplinkException(
+                    "if `link_type` is `link_only`, it should have at least two "
+                    "input dataframes, or one dataframe with a `source_dataset` "
+                    "column outlining which dataset each record belongs to."
+                )
+
     def _register_input_tables(self, input_tables, input_aliases, accepted_df_dtypes):
         # 'homogenised' means all entries are strings representing tables
         homogenised_tables = []
         homogenised_aliases = []
         accepted_df_dtypes = ensure_is_tuple(accepted_df_dtypes)
 
         for i, (table, alias) in enumerate(zip(input_tables, input_aliases)):
@@ -423,14 +452,18 @@
             for sql in sqls:
                 self._enqueue_sql(sql["sql"], sql["output_table_name"])
 
             if materialise:
                 nodes_with_tf = self._execute_sql_pipeline()
                 cache["__splink__df_concat_with_tf"] = nodes_with_tf
 
+        # verify the link job
+        if self._settings_obj_ is not None:
+            self._verify_link_only_job
+
         return nodes_with_tf
 
     def _table_to_splink_dataframe(
         self, templated_name, physical_name
     ) -> SplinkDataFrame:
         """Create a SplinkDataframe from a table in the underlying database called
         `physical_name`.
```

### Comparing `splink-3.8.0/splink/lower_id_on_lhs.py` & `splink-3.8.1/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/m_from_labels.py` & `splink-3.8.1/splink/m_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/m_training.py` & `splink-3.8.1/splink/m_training.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/m_u_records_to_parameters.py` & `splink-3.8.1/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/match_key_analysis.py` & `splink-3.8.1/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/match_weights_histogram.py` & `splink-3.8.1/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/misc.py` & `splink-3.8.1/splink/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,7 +158,16 @@
     base_version = [v.zfill(10) for v in base_version]
 
     return this_version >= base_version
 
 
 def ascii_uid(len):
     return "".join(random.choices(string.ascii_letters + string.digits, k=len))
+
+
+def find_unique_source_dataset(src_ds):
+    sql = f"""
+        select distinct {src_ds} as src
+        from __splink__df_concat_with_tf
+    """
+
+    return sql
```

### Comparing `splink-3.8.0/splink/missingness.py` & `splink-3.8.1/splink/missingness.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/parse_sql.py` & `splink-3.8.1/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/pipeline.py` & `splink-3.8.1/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/predict.py` & `splink-3.8.1/splink/predict.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/profile_data.py` & `splink-3.8.1/splink/profile_data.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/settings.py` & `splink-3.8.1/splink/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,19 @@
         if self._source_dataset_column_name_is_required:
             s_else_d = self._from_settings_dict_else_default
             return s_else_d("source_dataset_column_name")
         else:
             return None
 
     @property
+    def _source_dataset_col(self):
+        input_column = self._source_dataset_input_column
+        return (input_column, InputColumn(input_column, self).name())
+
+    @property
     def _unique_id_input_columns(self) -> list[InputColumn]:
         cols = []
 
         if self._source_dataset_column_name_is_required:
             col = InputColumn(
                 self._source_dataset_input_column,
                 settings_obj=self,
```

### Comparing `splink-3.8.0/splink/spark/custom_spark_dialect.py` & `splink-3.8.1/splink/spark/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/spark/spark_base.py` & `splink-3.8.1/splink/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/spark/spark_comparison_level_library.py` & `splink-3.8.1/splink/spark/spark_comparison_level_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/spark/spark_comparison_library.py` & `splink-3.8.1/splink/spark/spark_comparison_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/spark/spark_comparison_template_library.py` & `splink-3.8.1/splink/spark/spark_comparison_template_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/spark/spark_linker.py` & `splink-3.8.1/splink/spark/spark_linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/splink_comparison_viewer.py` & `splink-3.8.1/splink/splink_comparison_viewer.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/splink_dataframe.py` & `splink-3.8.1/splink/splink_dataframe.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/sql_transform.py` & `splink-3.8.1/splink/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/sqlite/sqlite_comparison_level_library.py` & `splink-3.8.1/splink/sqlite/sqlite_comparison_level_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/sqlite/sqlite_linker.py` & `splink-3.8.1/splink/sqlite/sqlite_linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/term_frequencies.py` & `splink-3.8.1/splink/term_frequencies.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/unique_id_concat.py` & `splink-3.8.1/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/unlinkables.py` & `splink-3.8.1/splink/unlinkables.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/validate_jsonschema.py` & `splink-3.8.1/splink/validate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/vertically_concatenate.py` & `splink-3.8.1/splink/vertically_concatenate.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/splink/waterfall_chart.py` & `splink-3.8.1/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.0/PKG-INFO` & `splink-3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.8.0
+Version: 3.8.1
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

