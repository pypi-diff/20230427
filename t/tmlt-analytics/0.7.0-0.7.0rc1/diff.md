# Comparing `tmp/tmlt_analytics-0.7.0.tar.gz` & `tmp/tmlt_analytics-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_analytics-0.7.0.tar", max compression
+gzip compressed data, was "tmlt_analytics-0.7.0rc1.tar", max compression
```

## Comparing `tmlt_analytics-0.7.0.tar` & `tmlt_analytics-0.7.0rc1.tar`

### file list

```diff
@@ -1,165 +1,159 @@
--rw-r--r--   0        0        0    15769 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/LICENSE
--rw-r--r--   0        0        0    20138 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/LICENSE.docs
--rw-r--r--   0        0        0      121 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/NOTICE
--rw-r--r--   0        0        0     2597 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/README.md
--rw-r--r--   0        0        0      951 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/_templates/package-name.html
--rw-r--r--   0        0        0     6705 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/conf.py
--rw-r--r--   0        0        0     1602 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/bigquery/bigquery-setup.rst
--rw-r--r--   0        0        0     3022 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/bigquery/docker-image.rst
--rw-r--r--   0        0        0     1237 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/bigquery/index.rst
--rw-r--r--   0        0        0     6303 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/bigquery/inputs-outputs.rst
--rw-r--r--   0        0        0     5770 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/bigquery/parameters.rst
--rw-r--r--   0        0        0     4763 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/bigquery/running-the-program.rst
--rw-r--r--   0        0        0     1716 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/bigquery/setup.rst
--rw-r--r--   0        0        0      314 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/index.rst
--rw-r--r--   0        0        0     4960 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/installation.rst
--rw-r--r--   0        0        0     2735 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/howto-guides/troubleshooting.rst
--rw-r--r--   0        0        0   118378 2023-04-27 18:13:47.698994 tmlt_analytics-0.7.0/doc/images/api_diagram.svg
--rw-r--r--   0        0        0    85925 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_age_at_joining.png
--rw-r--r--   0        0        0    27267 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_attacker_certainty.png
--rw-r--r--   0        0        0    41645 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_average_age_by_edu.png
--rw-r--r--   0        0        0    34101 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_books_by_unique_members.png
--rw-r--r--   0        0        0   104926 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_counts_age_gender.png
--rw-r--r--   0        0        0    34006 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_counts_different_eps.png
--rw-r--r--   0        0        0    25097 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_counts_edu+sex.png
--rw-r--r--   0        0        0    13993 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_counts_education.png
--rw-r--r--   0        0        0    41034 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_error_vs_partition_age_edu.png
--rw-r--r--   0        0        0    59042 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_favorite_genres.png
--rw-r--r--   0        0        0    14310 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_filters_education.png
--rw-r--r--   0        0        0    30330 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_genres_by_age.png
--rw-r--r--   0        0        0    14782 2023-04-27 18:13:47.702994 tmlt_analytics-0.7.0/doc/images/chart_quantiles_education.png
--rw-r--r--   0        0        0    20853 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/chart_senior_counts_1.png
--rw-r--r--   0        0        0    21067 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/chart_senior_counts_2.png
--rw-r--r--   0        0        0    29335 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/chart_teen_edu_counts.png
--rw-r--r--   0        0        0    20226 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/chart_younger_age_counts.png
--rw-r--r--   0        0        0    29155 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/clamping_bounds_averages.png
--rw-r--r--   0        0        0     9416 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/clamping_bounds_schema.png
--rw-r--r--   0        0        0    18639 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/flat_map_row_example.svg
--rw-r--r--   0        0        0    23590 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/flow_chart_truncation.svg
--rw-r--r--   0        0        0    14685 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/histogram_books_borrowed.png
--rw-r--r--   0        0        0     1844 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/index_api.svg
--rw-r--r--   0        0        0      609 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/index_howto_guides.svg
--rw-r--r--   0        0        0     1196 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/index_more.svg
--rw-r--r--   0        0        0      604 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1371 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    23369 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/intuitive_noise_visualization.png
--rw-r--r--   0        0        0    30903 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/logo.png
--rw-r--r--   0        0        0    54373 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/private_join_example.svg
--rw-r--r--   0        0        0    35838 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/private_join_tables.svg
--rw-r--r--   0        0        0    32227 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/images/public_join_example_zips.svg
--rw-r--r--   0        0        0     5569 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/index.rst
--rw-r--r--   0        0        0      662 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/intersphinx_mapping.json
--rw-r--r--   0        0        0     3169 2023-04-27 18:13:47.706994 tmlt_analytics-0.7.0/doc/privacy-policy.rst
--rw-r--r--   0        0        0     2024 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3440 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/templates/python/module.rst
--rw-r--r--   0        0        0      396 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/topic-guides/index.rst
--rw-r--r--   0        0        0    11697 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/topic-guides/nulls-nans-infinities.rst
--rw-r--r--   0        0        0     8608 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/topic-guides/privacy-budgets.rst
--rw-r--r--   0        0        0     6595 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/topic-guides/privacy-promise.rst
--rw-r--r--   0        0        0     7726 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0    10617 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/topic-guides/understanding-sensitivity.rst
--rw-r--r--   0        0        0     8462 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/topic-guides/working-with-sessions.rst
--rw-r--r--   0        0        0     9124 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/clamping-bounds.rst
--rw-r--r--   0        0        0     7246 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/first-steps.rst
--rw-r--r--   0        0        0    18802 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/groupby-queries.rst
--rw-r--r--   0        0        0      430 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/index.rst
--rw-r--r--   0        0        0    12394 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/more-with-privacy-ids.rst
--rw-r--r--   0        0        0     8475 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/privacy-budget-basics.rst
--rw-r--r--   0        0        0    13656 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/privacy-id-basics.rst
--rw-r--r--   0        0        0    16226 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/doc/tutorials/simple-transformations.rst
--rw-r--r--   0        0        0     4789 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/examples/interactive_evaluation.ipynb
--rw-r--r--   0        0        0     5459 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/examples/private_join.ipynb
--rw-r--r--   0        0        0     6570 2023-04-27 18:13:47.710994 tmlt_analytics-0.7.0/examples/zcdp_puredp_switching.ipynb
--rw-r--r--   0        0        0     4464 2023-04-27 18:14:22.867258 tmlt_analytics-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/__init__.py
--rw-r--r--   0        0        0     6976 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/conftest.py
--rw-r--r--   0        0        0      115 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/__init__.py
--rw-r--r--   0        0        0      108 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/__init__.py
--rw-r--r--   0        0        0     4265 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/conftest.py
--rw-r--r--   0        0        0      151 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/ids/__init__.py
--rw-r--r--   0        0        0    15227 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/ids/test_constraint_propagation.py
--rw-r--r--   0        0        0     6531 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/ids/test_count_distinct_optimization.py
--rw-r--r--   0        0        0    21707 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/ids/test_l0_linf_truncation.py
--rw-r--r--   0        0        0    13996 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/ids/test_l1_truncation.py
--rw-r--r--   0        0        0     4011 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/ids/test_partition.py
--rw-r--r--   0        0        0      143 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/mixed/__init__.py
--rw-r--r--   0        0        0     5087 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/mixed/test_mixed_session.py
--rw-r--r--   0        0        0      152 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/rows/__init__.py
--rw-r--r--   0        0        0    25557 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/rows/conftest.py
--rw-r--r--   0        0        0    40599 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/rows/test_add_max_rows.py
--rw-r--r--   0        0        0     6134 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/rows/test_add_max_rows_in_max_groups.py
--rw-r--r--   0        0        0    13790 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/rows/test_add_max_rows_infs_nulls.py
--rw-r--r--   0        0        0     7754 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/rows/test_invalid.py
--rw-r--r--   0        0        0     2212 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/system/session/test_invalid_constraints.py
--rw-r--r--   0        0        0      108 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/__init__.py
--rw-r--r--   0        0        0      298 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    75163 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/test_measurement_visitor.py
--rw-r--r--   0        0        0    54429 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/test_output_schema_visitor.py
--rw-r--r--   0        0        0      107 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/__init__.py
--rw-r--r--   0        0        0    17843 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/conftest.py
--rw-r--r--   0        0        0    24159 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
--rw-r--r--   0        0        0    36757 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
--rw-r--r--   0        0        0     7610 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
--rw-r--r--   0        0        0    14086 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_binning_spec.py
--rw-r--r--   0        0        0     2301 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_catalog.py
--rw-r--r--   0        0        0      657 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_cleanup.py
--rw-r--r--   0        0        0     5285 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_constraints.py
--rw-r--r--   0        0        0    21191 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_keyset.py
--rw-r--r--   0        0        0    13993 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_neighboring_relations.py
--rw-r--r--   0        0        0     3058 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_noise_info.py
--rw-r--r--   0        0        0     5865 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_privacy_budget.py
--rw-r--r--   0        0        0     5420 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0     3011 2023-04-27 18:13:47.714994 tmlt_analytics-0.7.0/test/unit/test_protected_change.py
--rw-r--r--   0        0        0    40864 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_query_builder.py
--rw-r--r--   0        0        0    63485 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_query_expr_compiler.py
--rw-r--r--   0        0        0    16715 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_query_expression.py
--rw-r--r--   0        0        0     4904 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_query_expression_visitor.py
--rw-r--r--   0        0        0     2172 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_schema.py
--rw-r--r--   0        0        0    13538 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_schema_conversion.py
--rw-r--r--   0        0        0    84468 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_session.py
--rw-r--r--   0        0        0     1604 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_table_identifiers.py
--rw-r--r--   0        0        0     5371 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_transformation_utils.py
--rw-r--r--   0        0        0      792 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_truncation_strategy.py
--rw-r--r--   0        0        0      518 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test/unit/test_utils.py
--rw-r--r--   0        0        0       37 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/test_requirements.txt
--rw-r--r--   0        0        0      222 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/__init__.py
--rw-r--r--   0        0        0     3666 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_catalog.py
--rw-r--r--   0        0        0     3555 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_coerce_spark_schema.py
--rw-r--r--   0        0        0    16188 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_neighboring_relation.py
--rw-r--r--   0        0        0     6110 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_neighboring_relation_visitor.py
--rw-r--r--   0        0        0     5428 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_noise_info.py
--rw-r--r--   0        0        0     2289 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0      184 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/__init__.py
--rw-r--r--   0        0        0     9786 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_compiler.py
--rw-r--r--   0        0        0     7694 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
--rw-r--r--   0        0        0    38844 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
--rw-r--r--   0        0        0    46296 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
--rw-r--r--   0        0        0    59768 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
--rw-r--r--   0        0        0    12796 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_schema.py
--rw-r--r--   0        0        0     1250 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_table_identifier.py
--rw-r--r--   0        0        0     3979 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_table_reference.py
--rw-r--r--   0        0        0    10147 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/_transformation_utils.py
--rw-r--r--   0        0        0    11663 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/binning_spec.py
--rw-r--r--   0        0        0      306 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/cleanup.py
--rw-r--r--   0        0        0      458 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/constraints/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/constraints/_base.py
--rw-r--r--   0        0        0      735 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/constraints/_simplify.py
--rw-r--r--   0        0        0    12819 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/constraints/_truncation.py
--rw-r--r--   0        0        0    11850 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/keyset.py
--rw-r--r--   0        0        0     7155 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/privacy_budget.py
--rw-r--r--   0        0        0     5497 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/protected_change.py
--rw-r--r--   0        0        0        0 2023-04-27 18:13:47.718994 tmlt_analytics-0.7.0/tmlt/analytics/py.typed
--rw-r--r--   0        0        0   126865 2023-04-27 18:13:47.722994 tmlt_analytics-0.7.0/tmlt/analytics/query_builder.py
--rw-r--r--   0        0        0    41097 2023-04-27 18:13:47.722994 tmlt_analytics-0.7.0/tmlt/analytics/query_expr.py
--rw-r--r--   0        0        0    72573 2023-04-27 18:13:47.722994 tmlt_analytics-0.7.0/tmlt/analytics/session.py
--rw-r--r--   0        0        0     3031 2023-04-27 18:13:47.722994 tmlt_analytics-0.7.0/tmlt/analytics/truncation_strategy.py
--rw-r--r--   0        0        0     4772 2023-04-27 18:13:47.722994 tmlt_analytics-0.7.0/tmlt/analytics/utils.py
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0/setup.py
--rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    13178 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0    20138 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/LICENSE.docs
+-rw-r--r--   0        0        0      121 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/NOTICE
+-rw-r--r--   0        0        0     2597 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/README.md
+-rw-r--r--   0        0        0      951 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/package-name.html
+-rw-r--r--   0        0        0     1108 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/citing.rst
+-rw-r--r--   0        0        0      201 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/index.rst
+-rw-r--r--   0        0        0      670 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/license.rst
+-rw-r--r--   0        0        0     3159 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/privacy_policy.rst
+-rw-r--r--   0        0        0     6764 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/conf.py
+-rw-r--r--   0        0        0   118378 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/api_diagram.svg
+-rw-r--r--   0        0        0    85925 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_age_at_joining.png
+-rw-r--r--   0        0        0    27267 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_attacker_certainty.png
+-rw-r--r--   0        0        0    41645 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_average_age_by_edu.png
+-rw-r--r--   0        0        0    34101 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_books_by_unique_members.png
+-rw-r--r--   0        0        0   104926 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_age_gender.png
+-rw-r--r--   0        0        0    34006 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_different_eps.png
+-rw-r--r--   0        0        0    25097 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_edu+sex.png
+-rw-r--r--   0        0        0    13993 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_education.png
+-rw-r--r--   0        0        0    41034 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_error_vs_partition_age_edu.png
+-rw-r--r--   0        0        0    59042 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_favorite_genres.png
+-rw-r--r--   0        0        0    14310 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_filters_education.png
+-rw-r--r--   0        0        0    30330 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_genres_by_age.png
+-rw-r--r--   0        0        0    14782 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_quantiles_education.png
+-rw-r--r--   0        0        0    20853 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_1.png
+-rw-r--r--   0        0        0    21067 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_2.png
+-rw-r--r--   0        0        0    29335 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/chart_teen_edu_counts.png
+-rw-r--r--   0        0        0    20226 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/chart_younger_age_counts.png
+-rw-r--r--   0        0        0    29155 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_averages.png
+-rw-r--r--   0        0        0     9416 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_schema.png
+-rw-r--r--   0        0        0    23590 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/flow_chart_truncation.svg
+-rw-r--r--   0        0        0    14685 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/histogram_books_borrowed.png
+-rw-r--r--   0        0        0     1844 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_api.svg
+-rw-r--r--   0        0        0     1196 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_more.svg
+-rw-r--r--   0        0        0      604 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1371 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    30903 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/logo.png
+-rw-r--r--   0        0        0     3971 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/index.rst
+-rw-r--r--   0        0        0     4960 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/installation.rst
+-rw-r--r--   0        0        0      662 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/intersphinx_mapping.json
+-rw-r--r--   0        0        0     2024 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3440 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/templates/python/module.rst
+-rw-r--r--   0        0        0     1602 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/bigquery-setup.rst
+-rw-r--r--   0        0        0     3022 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/docker-image.rst
+-rw-r--r--   0        0        0     1237 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/index.rst
+-rw-r--r--   0        0        0     6303 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/inputs-outputs.rst
+-rw-r--r--   0        0        0     5770 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/parameters.rst
+-rw-r--r--   0        0        0     4763 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/running-the-program.rst
+-rw-r--r--   0        0        0     1716 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/setup.rst
+-rw-r--r--   0        0        0      405 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0    11697 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/nulls-nans-infinities.rst
+-rw-r--r--   0        0        0     8608 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-budgets.rst
+-rw-r--r--   0        0        0     6595 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-promise.rst
+-rw-r--r--   0        0        0     7726 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0     2735 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/troubleshooting.rst
+-rw-r--r--   0        0        0     8462 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/working-with-sessions.rst
+-rw-r--r--   0        0        0     9124 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/clamping-bounds.rst
+-rw-r--r--   0        0        0     7246 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/first-steps.rst
+-rw-r--r--   0        0        0    18802 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/groupby-queries.rst
+-rw-r--r--   0        0        0      430 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/index.rst
+-rw-r--r--   0        0        0    11634 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/more-with-privacy-ids.rst
+-rw-r--r--   0        0        0     7732 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-budget-basics.rst
+-rw-r--r--   0        0        0    11302 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-id-basics.rst
+-rw-r--r--   0        0        0    16226 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/simple-transformations.rst
+-rw-r--r--   0        0        0     4789 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/interactive_evaluation.ipynb
+-rw-r--r--   0        0        0     5459 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/private_join.ipynb
+-rw-r--r--   0        0        0     6570 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/zcdp_puredp_switching.ipynb
+-rw-r--r--   0        0        0     4469 2023-04-17 23:55:55.706036 tmlt_analytics-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/__init__.py
+-rw-r--r--   0        0        0     6976 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/conftest.py
+-rw-r--r--   0        0        0      115 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/__init__.py
+-rw-r--r--   0        0        0     4265 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/conftest.py
+-rw-r--r--   0        0        0      151 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/__init__.py
+-rw-r--r--   0        0        0    15227 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_constraint_propagation.py
+-rw-r--r--   0        0        0    21707 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l0_linf_truncation.py
+-rw-r--r--   0        0        0    14517 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l1_truncation.py
+-rw-r--r--   0        0        0     4011 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_partition.py
+-rw-r--r--   0        0        0      143 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/mixed/__init__.py
+-rw-r--r--   0        0        0     5087 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/mixed/test_mixed_session.py
+-rw-r--r--   0        0        0      152 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/__init__.py
+-rw-r--r--   0        0        0    25557 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/conftest.py
+-rw-r--r--   0        0        0    38557 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows.py
+-rw-r--r--   0        0        0     6134 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_in_max_groups.py
+-rw-r--r--   0        0        0    13790 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_infs_nulls.py
+-rw-r--r--   0        0        0     7754 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_invalid.py
+-rw-r--r--   0        0        0     2212 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/test_invalid_constraints.py
+-rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/__init__.py
+-rw-r--r--   0        0        0      298 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    75163 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_measurement_visitor.py
+-rw-r--r--   0        0        0    54429 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_output_schema_visitor.py
+-rw-r--r--   0        0        0      107 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/__init__.py
+-rw-r--r--   0        0        0    17843 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/conftest.py
+-rw-r--r--   0        0        0    24159 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
+-rw-r--r--   0        0        0    36757 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
+-rw-r--r--   0        0        0     7610 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
+-rw-r--r--   0        0        0    14086 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_binning_spec.py
+-rw-r--r--   0        0        0     2301 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_catalog.py
+-rw-r--r--   0        0        0      657 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_cleanup.py
+-rw-r--r--   0        0        0     5285 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_constraints.py
+-rw-r--r--   0        0        0    21191 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_keyset.py
+-rw-r--r--   0        0        0    13993 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_neighboring_relations.py
+-rw-r--r--   0        0        0     3058 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_noise_info.py
+-rw-r--r--   0        0        0     5865 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget.py
+-rw-r--r--   0        0        0     5420 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0     3011 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_protected_change.py
+-rw-r--r--   0        0        0    40864 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_builder.py
+-rw-r--r--   0        0        0    63485 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expr_compiler.py
+-rw-r--r--   0        0        0    16715 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expression.py
+-rw-r--r--   0        0        0     4904 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expression_visitor.py
+-rw-r--r--   0        0        0     2172 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_schema.py
+-rw-r--r--   0        0        0    13538 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_schema_conversion.py
+-rw-r--r--   0        0        0    84468 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_session.py
+-rw-r--r--   0        0        0     1604 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_table_identifiers.py
+-rw-r--r--   0        0        0     5371 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_transformation_utils.py
+-rw-r--r--   0        0        0      792 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_truncation_strategy.py
+-rw-r--r--   0        0        0      518 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_utils.py
+-rw-r--r--   0        0        0       37 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test_requirements.txt
+-rw-r--r--   0        0        0      222 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/__init__.py
+-rw-r--r--   0        0        0     3666 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_catalog.py
+-rw-r--r--   0        0        0     3555 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_coerce_spark_schema.py
+-rw-r--r--   0        0        0    16188 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation.py
+-rw-r--r--   0        0        0     6110 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation_visitor.py
+-rw-r--r--   0        0        0     5428 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_noise_info.py
+-rw-r--r--   0        0        0     2289 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0      184 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0     9786 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_compiler.py
+-rw-r--r--   0        0        0     7694 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
+-rw-r--r--   0        0        0    34784 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
+-rw-r--r--   0        0        0    46272 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
+-rw-r--r--   0        0        0    59768 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
+-rw-r--r--   0        0        0    12656 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_schema.py
+-rw-r--r--   0        0        0     1250 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_identifier.py
+-rw-r--r--   0        0        0     3979 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_reference.py
+-rw-r--r--   0        0        0    10147 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_transformation_utils.py
+-rw-r--r--   0        0        0    11663 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/binning_spec.py
+-rw-r--r--   0        0        0      306 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/cleanup.py
+-rw-r--r--   0        0        0      288 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_base.py
+-rw-r--r--   0        0        0      735 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_simplify.py
+-rw-r--r--   0        0        0    12819 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_truncation.py
+-rw-r--r--   0        0        0    11850 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/keyset.py
+-rw-r--r--   0        0        0     7155 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/privacy_budget.py
+-rw-r--r--   0        0        0     5471 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/protected_change.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/py.typed
+-rw-r--r--   0        0        0   126388 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/query_builder.py
+-rw-r--r--   0        0        0    41097 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/query_expr.py
+-rw-r--r--   0        0        0    72500 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/session.py
+-rw-r--r--   0        0        0     3031 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/truncation_strategy.py
+-rw-r--r--   0        0        0     4772 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/utils.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0rc1/setup.py
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0rc1/PKG-INFO
```

### Comparing `tmlt_analytics-0.7.0/CHANGELOG.rst` & `tmlt_analytics-0.7.0rc1/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,41 @@
 .. _analytics-changelog:
 
 Changelog
 =========
 
-0.7.0 - 2023-04-27
-------------------
-
-This release adds support for *privacy identifiers*:
-Tumult Analytics can now protect input tables in which the differential privacy guarantee needs to hide the presence of arbitrarily many rows sharing the same value in a particular column.
-For example, this may be used to protect each user of a service when every row in a table is associated with a user ID.
-
-Privacy identifiers are set up using the new :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change.
-A number of features have been added to the API to support this, including alternative behaviors for various query transformations when working with IDs and the new concept of :mod:`~tmlt.analytics.constraints`.
-To get started with these features, take a look at the new :ref:`Working with privacy IDs <Working with privacy IDs>` and :ref:`Doing more with privacy IDs <Advanced IDs features>` tutorials.
+Unreleased
+----------
 
 Added
 ~~~~~
-- A new :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change has been added, which protects the addition or removal of all rows with the same value in a specified column.
-  See the documentation for :class:`~tmlt.analytics.protected_change.AddRowsWithID` and the :ref:`Doing more with privacy IDs <Advanced IDs features>` tutorial for more information.
-
-  - When creating a Session with :class:`~tmlt.analytics.protected_change.AddRowsWithID` using a :class:`Session.Builder<tmlt.analytics.session.Session.Builder>`, you must use the new :meth:`~tmlt.analytics.session.Session.Builder.with_id_space` method to specify the identifier space(s) of tables using this protected change.
-  - When creating a Session with :meth:`Session.from_dataframe()<tmlt.analytics.session.Session.from_dataframe>`, specifying an ID space is not necessary.
+- Added MaxRowsPerGroupPerID contraint, which limits the number of rows each unique (ID, grouping column value) pair may appear in.
+- Added MaxGroupsPerID constraint, which limits the number of unique grouping column values associated with each unique ID.
+- Added a new :class:`tmlt.analytics.protected_change.AddRowsWithID` class, which protects the addition or removal of all rows with the same value in a specified column.
+  When creating a session with AddRowsWithID for multiple tables, you must use the new :meth:`Session.Builder.with_id_space <tmlt.analytics.session.Session.Builder.with_id_space>` method to specify the identifier space(s) of the tables.
+  See the documentation for :class:`tmlt.analytics.protected_change.AddRowsWithID` for more information.
+- Added a new method, :meth:`tmlt.analytics.session.Session.describe`, which describes a session, query, or table.
 
-- :class:`~tmlt.analytics.query_builder.QueryBuilder` has a new method, :meth:`~tmlt.analytics.query_builder.QueryBuilder.enforce`, for enforcing constraints on a table.
-  Types for representing these constraints are located in the new :mod:`tmlt.analytics.constraints` module.
-- A new method, :meth:`Session.describe()<tmlt.analytics.session.Session.describe>`, has been added to provide a summary of the tables in a :class:`~tmlt.analytics.session.Session`, or of a single table or the output of a query.
 
 Changed
 ~~~~~~~
-- :meth:`QueryBuilder.join_private()<tmlt.analytics.query_builder.QueryBuilder.join_private>` now accepts the name of a private table as ``right_operand``.
-  For example, ``QueryBuilder("table").join_private("foo")`` is equivalent to ``QueryBuilder("table").join_private(QueryBuilder("foo"))``.
-- The ``max_num_rows`` parameter to :meth:`QueryBuilder.flat_map()<tmlt.analytics.query_builder.QueryBuilder.flat_map>` is now optional when applied to tables with an :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change.
-- *Backwards-incompatible*: The parameters to :meth:`QueryBuilder.flat_map()<tmlt.analytics.query_builder.QueryBuilder.flat_map>` have been reordered, moving ``max_num_rows`` to be the last parameter.
-- *Backwards-incompatible*: The lower and upper bounds for quantile, sum, average, variance, and standard deviation queries can no longer be equal to one another.
-  The lower bound must now be strictly less than the upper bound.
-- *Backwards-incompatible*: Renamed :meth:`QueryBuilder.filter()<tmlt.analytics.query_builder.QueryBuilder.filter>` ``predicate`` argument to ``condition``.
-- *Backwards-incompatible*: Renamed :class:`~tmlt.analytics.query_expr.Filter` query expression ``predicate`` property to ``condition``.
-- *Backwards-incompatible*: Renamed :meth:`KeySet.filter()<tmlt.analytics.keyset.KeySet.filter>` ``expr`` argument to ``condition``.
-
-Deprecated
-~~~~~~~~~~
-- The ``stability`` and ``grouping_column`` parameters to :class:`Session.from_dataframe()<tmlt.analytics.session.Session.from_dataframe>` and :class:`Session.Builder.with_private_dataframe()<tmlt.analytics.session.Session.Builder.with_private_dataframe>` are deprecated, and will be removed in a future release.
-  The ``protected_change`` parameter should be used instead, and will become required.
-
-Removed
-~~~~~~~
-- The ``attr_name`` parameter to :class:`Session.partition_and_create()<tmlt.analytics.session.Session.partition_and_create>`, which was deprecated in version 0.5.0, has been removed.
+- Argument ``max_num_rows`` of ``QueryBuilder.flat_map`` is now optional for tables with a :class:`tmlt.analytics.protected_change.AddRowsWithID` protected change.
+- *Backwards-incompatible*: Argument ``max_num_rows`` is now the last parameter specified for ``QueryBuilder.flat_map``.
+- *Backwards-incompatible*: Analytics no longer allows users to set lower bounds equal to upper bounds for quantile, sum, average, variance, and standard deviation queries. Now, the lower bound must be strictly less than the upper bound.
+- *Backwards-incompatible*: Renamed ``QueryBuilder.filter`` argument from "predicate" to "condition".
+- *Backwards-incompatible*: Renamed ``query_expr.Filter`` property from "predicate" to "condition".
+- *Backwards-incompatible*: Renamed ``KeySet.filter`` argument from "expr" to "condition".
+- ``QueryBuilder.join_private`` now accepts a string as a ``right_operand``. ``QueryBuilder("table").join_private("foo")`` is equivalent to ``QueryBuilder("table").join_private(QueryBuilder("foo"))``.
+- *Backwards-incompatible*: Removed the ``attr_name`` argument from ``Session.partition_and_create``.
 
 Fixed
 ~~~~~
-- :meth:`Session.add_public_datafame()<tmlt.analytics.session.Session.add_public_dataframe>` used to allow creation of a public table with the same name as an existing public table, which was neither intended nor fully supported by some :class:`~tmlt.analytics.session.Session` methods.
-  It now raises a ``ValueError`` in this case.
-- Some query patterns on tables containing nulls could cause grouped aggregations to produce the wrong set of group keys in their output.
-  This no longer happens.
-- In certain unusual cases, join transformations could erroneously drop rows containing nulls in columns that were not being joined on.
-  These rows are no longer dropped.
+
+- ``Session.add_public_datafame`` used to allow creation of a public table with the same name as an existing private table, even though doing so is disallowed elsewhere and is not fully supported by some ``Session`` methods.
+  It now raises a ``ValueError`` when this happens, like it already did when there was a name conflict with an existing public table.
 
 0.6.1 - 2022-12-07
 ------------------
 
 This is a maintenance release which introduces a number of documentation improvements, but has no publicly-visible API changes.
 
 0.6.0 - 2022-12-06
```

### Comparing `tmlt_analytics-0.7.0/LICENSE` & `tmlt_analytics-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/LICENSE.docs` & `tmlt_analytics-0.7.0rc1/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/README.md` & `tmlt_analytics-0.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/_static/css/custom.css` & `tmlt_analytics-0.7.0rc1/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/_static/favicon.ico` & `tmlt_analytics-0.7.0rc1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/_static/js/version-banner.js` & `tmlt_analytics-0.7.0rc1/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/_static/logo.png` & `tmlt_analytics-0.7.0rc1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/conf.py` & `tmlt_analytics-0.7.0rc1/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ci_tag = os.getenv("CI_COMMIT_TAG")
 ci_branch = os.getenv("CI_COMMIT_BRANCH")
 
 version = ci_tag or ci_branch or "HEAD"
 commit_hash = os.getenv("CI_COMMIT_SHORT_SHA") or "unknown version"
 build_time = datetime.datetime.utcnow().isoformat(sep=" ", timespec="minutes")
 
+linkcheck_mode_url_prefix = os.getenv("BASE_URL_OVERRIDE")
 # Linkcheck will complain that these anchors don't exist,
 # even though the link works.
 linkcheck_ignore = [
     "https://colab.research.google.com/drive/18J_UrHAKJf52RMRxi4OOpk59dV9tvKxO#offline=true&sandboxMode=true"
 ]
 
 # Sphinx configuration
```

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/bigquery/bigquery-setup.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/bigquery-setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/bigquery/docker-image.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/docker-image.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/bigquery/index.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/bigquery/inputs-outputs.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/inputs-outputs.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/bigquery/parameters.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/parameters.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/bigquery/running-the-program.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/running-the-program.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/bigquery/setup.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/installation.rst` & `tmlt_analytics-0.7.0rc1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/howto-guides/troubleshooting.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/api_diagram.svg` & `tmlt_analytics-0.7.0rc1/doc/images/api_diagram.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_age_at_joining.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_age_at_joining.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_attacker_certainty.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_attacker_certainty.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_average_age_by_edu.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_average_age_by_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_books_by_unique_members.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_books_by_unique_members.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_counts_age_gender.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_age_gender.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_counts_different_eps.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_different_eps.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_counts_edu+sex.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_edu+sex.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_counts_education.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_error_vs_partition_age_edu.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_error_vs_partition_age_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_favorite_genres.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_favorite_genres.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_filters_education.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_filters_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_genres_by_age.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_genres_by_age.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_quantiles_education.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_quantiles_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_senior_counts_1.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_1.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_senior_counts_2.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_2.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_teen_edu_counts.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_teen_edu_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/chart_younger_age_counts.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_younger_age_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/clamping_bounds_averages.png` & `tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_averages.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/clamping_bounds_schema.png` & `tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_schema.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/flow_chart_truncation.svg` & `tmlt_analytics-0.7.0rc1/doc/images/flow_chart_truncation.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/histogram_books_borrowed.png` & `tmlt_analytics-0.7.0rc1/doc/images/histogram_books_borrowed.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/index_api.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/index_howto_guides.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_topic_guides.svg`

 * *Files 24% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
 00000020: 662d 3822 3f3e 0d0a 0d0a 3c21 444f 4354  f-8"?>....<!DOCT
 00000030: 5950 4520 7376 6720 5055 424c 4943 2022  YPE svg PUBLIC "
 00000040: 2d2f 2f57 3343 2f2f 4454 4420 5356 4720  -//W3C//DTD SVG 
 00000050: 312e 312f 2f45 4e22 2022 6874 7470 3a2f  1.1//EN" "http:/
 00000060: 2f77 7777 2e77 332e 6f72 672f 4772 6170  /www.w3.org/Grap
 00000070: 6869 6373 2f53 5647 2f31 2e31 2f44 5444  hics/SVG/1.1/DTD
-00000080: 2f73 7667 3131 2e64 7464 223e 0d0a 3c21  /svg11.dtd">..<!
-00000090: 2d2d 2055 706c 6f61 6465 6420 746f 3a20  -- Uploaded to: 
-000000a0: 5356 4720 5265 706f 2c20 7777 772e 7376  SVG Repo, www.sv
-000000b0: 6772 6570 6f2e 636f 6d2c 2047 656e 6572  grepo.com, Gener
-000000c0: 6174 6f72 3a20 5356 4720 5265 706f 204d  ator: SVG Repo M
-000000d0: 6978 6572 2054 6f6f 6c73 202d 2d3e 0a3c  ixer Tools -->.<
-000000e0: 7376 6720 7769 6474 683d 2238 3030 7078  svg width="800px
-000000f0: 2220 6865 6967 6874 3d22 3830 3070 7822  " height="800px"
-00000100: 2076 6965 7742 6f78 3d22 3020 3020 3332   viewBox="0 0 32
-00000110: 2033 3222 2076 6572 7369 6f6e 3d22 312e   32" version="1.
-00000120: 3122 2078 6d6c 6e73 3d22 6874 7470 3a2f  1" xmlns="http:/
-00000130: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
-00000140: 2f73 7667 2220 786d 6c6e 733a 786c 696e  /svg" xmlns:xlin
-00000150: 6b3d 2268 7474 703a 2f2f 7777 772e 7733  k="http://www.w3
-00000160: 2e6f 7267 2f31 3939 392f 786c 696e 6b22  .org/1999/xlink"
-00000170: 3e0d 0a3c 6720 6964 3d22 6963 6f6d 6f6f  >..<g id="icomoo
-00000180: 6e2d 6967 6e6f 7265 223e 0d0a 3c2f 673e  n-ignore">..</g>
-00000190: 0d0a 3c70 6174 6820 643d 224d 3138 2e37  ..<path d="M18.7
-000001a0: 3236 2033 2e37 3733 6c2d 312e 3337 3520  26 3.773l-1.375 
-000001b0: 3131 2e31 3668 362e 3038 386c 2d31 302e  11.16h6.088l-10.
-000001c0: 3136 3520 3133 2e32 3933 2031 2e33 3736  165 13.293 1.376
-000001d0: 2d31 312e 3136 682d 362e 3038 386c 3130  -11.16h-6.088l10
-000001e0: 2e31 3635 2d31 332e 3239 337a 4d32 302e  .165-13.293zM20.
-000001f0: 3236 3520 302e 3030 366c 2d31 332e 3836  265 0.006l-13.86
-00000200: 3120 3138 2e31 3236 6837 2e30 3430 6c2d  1 18.126h7.040l-
-00000210: 312e 3730 3920 3133 2e38 3631 2031 332e  1.709 13.861 13.
-00000220: 3836 312d 3138 2e31 3236 682d 372e 3034  861-18.126h-7.04
-00000230: 306c 312e 3730 392d 3133 2e38 3631 7a22  0l1.709-13.861z"
-00000240: 2066 696c 6c3d 2223 3030 3030 3030 223e   fill="#000000">
-00000250: 0a0d 3c2f 7061 7468 3e0d 0a3c 2f73 7667  ..</path>..</svg
-00000260: 3e                                       >
+00000080: 2f73 7667 3131 2e64 7464 223e 0d0a 3c73  /svg11.dtd">..<s
+00000090: 7667 2077 6964 7468 3d22 3332 7078 2220  vg width="32px" 
+000000a0: 6865 6967 6874 3d22 3332 7078 2220 7669  height="32px" vi
+000000b0: 6577 426f 783d 2230 2030 2033 3220 3332  ewBox="0 0 32 32
+000000c0: 2220 7665 7273 696f 6e3d 2231 2e31 2220  " version="1.1" 
+000000d0: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+000000e0: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
+000000f0: 6722 2078 6d6c 6e73 3a78 6c69 6e6b 3d22  g" xmlns:xlink="
+00000100: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00000110: 672f 3139 3939 2f78 6c69 6e6b 223e 0d0a  g/1999/xlink">..
+00000120: 3c67 2069 643d 2269 636f 6d6f 6f6e 2d69  <g id="icomoon-i
+00000130: 676e 6f72 6522 3e0d 0a3c 2f67 3e0d 0a3c  gnore">..</g>..<
+00000140: 7061 7468 2064 3d22 4d33 312e 3531 3420  path d="M31.514 
+00000150: 3131 2e31 3737 6c2d 3135 2e35 3134 2d37  11.177l-15.514-7
+00000160: 2e34 3637 2d31 352e 3531 3420 372e 3436  .467-15.514 7.46
+00000170: 3720 322e 3138 3620 312e 3331 3876 3131  7 2.186 1.318v11
+00000180: 2e35 3239 6831 2e30 3636 762d 3130 2e38  .529h1.066v-10.8
+00000190: 3836 6c33 2e31 3939 2031 2e39 3239 7631  86l3.199 1.929v1
+000001a0: 332e 3232 3368 3138 2e31 3236 762d 3133  3.223h18.126v-13
+000001b0: 2e32 3139 6c36 2e34 3531 2d33 2e38 3934  .219l6.451-3.894
+000001c0: 7a4d 3136 2034 2e38 3933 6c31 332e 3237  zM16 4.893l13.27
+000001d0: 3520 362e 3339 2d31 332e 3236 3720 382e  5 6.39-13.267 8.
+000001e0: 3030 382d 3133 2e32 3832 2d38 2e30 3039  008-13.282-8.009
+000001f0: 2031 332e 3237 342d 362e 3339 7a4d 3233   13.274-6.39zM23
+00000200: 2e39 3937 2032 372e 3232 3468 2d31 352e  .997 27.224h-15.
+00000210: 3939 3476 2d31 312e 3531 346c 382e 3030  994v-11.514l8.00
+00000220: 3520 342e 3832 3720 372e 3938 392d 342e  5 4.827 7.989-4.
+00000230: 3832 3376 3131 2e35 317a 2220 6669 6c6c  823v11.51z" fill
+00000240: 3d22 2330 3030 3030 3022 3e3c 2f70 6174  ="#000000"></pat
+00000250: 683e 0d0a 3c2f 7376 673e 0d0a            h>..</svg>..
```

### Comparing `tmlt_analytics-0.7.0/doc/images/index_more.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/index_tutorials.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/images/logo.png` & `tmlt_analytics-0.7.0rc1/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/intersphinx_mapping.json` & `tmlt_analytics-0.7.0rc1/doc/intersphinx_mapping.json`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/privacy-policy.rst` & `tmlt_analytics-0.7.0rc1/doc/additional-resources/privacy_policy.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-:orphan:
-
-.. _privacy-policy:
+.. _privacy_policy:
 
 Privacy Policy
 ==============
 
 Effective Date: Aug 26th, 2022
 
 Welcome
```

### Comparing `tmlt_analytics-0.7.0/doc/templates/python/class.rst` & `tmlt_analytics-0.7.0rc1/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/templates/python/module.rst` & `tmlt_analytics-0.7.0rc1/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/topic-guides/nulls-nans-infinities.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/nulls-nans-infinities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/topic-guides/privacy-budgets.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-budgets.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/topic-guides/privacy-promise.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-promise.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 A :class:`~tmlt.analytics.session.Session` is initialized with:
 
 * one or more private tables (containing data you wish to query in a differentially
   private way), each associated to a :mod:`protected change<tmlt.analytics.protected_change>`;
 * zero or more public tables (containing data that does not require privacy
   protection, but may be used as auxiliary input to your computation);
 * a privacy definition along with its associated privacy parameters (e.g.
-  tutorials use `PureDPBudget`, corresponding to pure differential privacy, and
+  tutorials use `PureDBBudget`, corresponding to pure differential privacy, and
   Tumult Analytics also supports zero-concentrated differential privacy).
 
 After initialization, the Session guarantees that the answers returned by
 calling :meth:`~tmlt.analytics.session.Session.evaluate` to evaluate queries
 satisfy the corresponding privacy definition with respect to the private data,
 using the specified parameters. For example, a Session initialized with
 :code:`PureDPBudget(1)` provides :math:`{\varepsilon}`-differential privacy with
```

### Comparing `tmlt_analytics-0.7.0/doc/topic-guides/spark.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/topic-guides/working-with-sessions.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/working-with-sessions.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/tutorials/clamping-bounds.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/clamping-bounds.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/tutorials/first-steps.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/first-steps.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/tutorials/groupby-queries.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/groupby-queries.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/doc/tutorials/more-with-privacy-ids.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/more-with-privacy-ids.rst`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Initializing a Session with multiple IDs tables
 -----------------------------------------------
 
 Notice that both of the dataframes we’ve loaded share a common
 identifier: the ID associated with each library member. Our goal is to
 construct a :class:`Session<tmlt.analytics.session.Session>` that
 protects the addition or removal of arbitrarily many rows that share the
-same ID, *in both tables*. To do so, we have to use the
+same ID, *in both tables*. To do so, we have to use the 
 :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change
 again, but we also have to indicate that both tables share the same *ID space*.
 This is done as follows.
 
 .. testcode::
 
     budget = PureDPBudget(float("inf")) # infinite budget for the session
@@ -94,15 +94,15 @@
     Private dataframes: ['members', 'checkouts']
 
 The
 :meth:`Session.Builder.with_id_space<tmlt.analytics.session.Session.Builder.with_id_space>`
 method and the :class:`AddRowsWithID<tmlt.analytics.protected_change.AddRowsWithID>`
 protected change work together to accomplish our desired notion of privacy.
 
-- The ``with_id_space`` function defines our ID space, ``member_id_space``. This is
+- The ``with_primary_id`` function defines our ID space, ``member_id_space``. This is
   how we indicate that the same person is associated with the same ID in both tables.
 
 - This ID space is then specified to ``AddRowsWithID``’s ``identifier``
   parameter, while the ``id_column`` parameter indicates
   which column in the dataframe contains the IDs.
 
 With this information, the resulting Session now protects each library member
@@ -121,15 +121,15 @@
 - First, since each book in the checkouts table can be
   associated with more than one genre, we will expand this
   table to break out each genre for a book into a separate row.
 
 - Second, we will join the expanded checkouts data with the library
   members data, using the members ID as a join key.
 
-- Finally, we will group the joined table by age group and genres, and obtain
+- Finally, we will group the joined table by age group and genres, and obtain 
   counts by genres.
 
 Flat maps
 ~~~~~~~~~
 
 First, let's expand the checkout dataframe to
 associate each book to its genres, with each genre on its own separate row. To do this,
@@ -205,42 +205,14 @@
     print(f"Private dataframes: {session.private_sources}")
 
 .. testoutput::
     :options: +NORMALIZE_WHITESPACE
 
     Private dataframes: ['checkouts_joined', 'checkouts_single_genre', 'members', 'checkouts']
 
-Let's inspect the result of the join to make sure it looks right:
-
-.. testcode::
-
-    session.describe("checkouts_joined")
-
-.. testoutput::
-    :options: +NORMALIZE_WHITESPACE
-
-    Columns:
-	- 'member_id'         INTEGER, ID column (in ID space member_id_space)
-	- 'checkout_date'     TIMESTAMP
-	- 'title'             VARCHAR
-	- 'author'            VARCHAR
-	- 'isbn'              VARCHAR
-	- 'publication_date'  INTEGER
-	- 'publisher'         VARCHAR
-	- 'genres'            VARCHAR
-	- 'genre'             VARCHAR
-	- 'name'              VARCHAR
-	- 'age'               INTEGER
-	- 'gender'            VARCHAR
-	- 'education_level'   VARCHAR
-	- 'zip_code'          VARCHAR
-	- 'books_borrowed'    INTEGER
-	- 'favorite_genres'   VARCHAR
-	- 'date_joined'       TIMESTAMP
-
 Using :meth:`~tmlt.analytics.query_builder.QueryBuilder.join_private` on two private tables in the same ID space works seamlessly as long as the ID
 columns are part of the join and have the same name in both tables. Like with
 :meth:`~tmlt.analytics.query_builder.QueryBuilder.flat_map`, no truncation is necessary.
 
 Computing the statistic
 ~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -333,8 +305,8 @@
 
 - Data preparation is generally more convenient when using privacy IDs, because you
   don't need to worry about truncating your data (when performing e.g. flat maps or
   joins) until immediately before aggregation.
 
 - Truncation as a last step before aggregation can lead to better utility. Plus,
   if you want to compute multiple aggregations, you might also want to use different
-  truncation parameters for each.
+  truncation parameters for each.
```

### Comparing `tmlt_analytics-0.7.0/doc/tutorials/privacy-budget-basics.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-budget-basics.rst`

 * *Files 9% similar despite different names*

```diff
@@ -78,38 +78,14 @@
    session = Session.from_dataframe(
        privacy_budget=budget,
        source_id="members",
        dataframe=members_df,
        protected_change=AddOneRow(),
    )
 
-Let's check that we initialized the Session as intended using the
-:meth:`describe<tmlt.analytics.session.Session.describe>` method:
-
-.. testcode::
-
-   session.describe()
-
-.. testoutput::
-   :options: +NORMALIZE_WHITESPACE
-
-   The session has a remaining privacy budget of PureDPBudget(epsilon=2.5).
-   The following private tables are available:
-   Table 'members' (no constraints):
-      Columns:
-         - 'id'               INTEGER
-         - 'name'             VARCHAR
-         - 'age'              INTEGER
-         - 'gender'           VARCHAR
-         - 'education_level'  VARCHAR
-         - 'zip_code'         VARCHAR
-         - 'books_borrowed'   INTEGER
-         - 'favorite_genres'  VARCHAR
-         - 'date_joined'      TIMESTAMP
-
 Initializing a Session with a finite privacy budget gives a simple interface
 promise: all queries evaluated on this Session, *taken together*, will provide
 differentially private results with at most ``epsilon=2.5``. This parameter
 measures the potential privacy *loss*: a lower epsilon gives a stricter limit on
 the privacy loss, and therefore a higher level of protection. Here, the
 corresponding interface promise is a *privacy guarantee*: it enforces a minimum
 level of protection on the private data. For more information about this promise
```

### Comparing `tmlt_analytics-0.7.0/doc/tutorials/privacy-id-basics.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-id-basics.rst`

 * *Files 10% similar despite different names*

```diff
@@ -82,38 +82,15 @@
         budget,
         "checkouts",
         checkouts_df,
         protected_change=AddRowsWithID(id_column="member_id"),
     )
 
 Initializing our Session like this protects members of our library,
-regardless of how many books they've checked out. Let's take a look at our Session:
-
-.. testcode::
-
-    session.describe()
-
-.. testoutput::
-    :options: +NORMALIZE_WHITESPACE
-
-    The session has a remaining privacy budget of PureDPBudget(epsilon=inf).
-    The following private tables are available:
-    Table 'checkouts' (no constraints):
-        Columns:
-            - 'checkout_date'     TIMESTAMP
-            - 'member_id'         INTEGER, ID column (in ID space default_id_space)
-            - 'title'             VARCHAR
-            - 'author'            VARCHAR
-            - 'isbn'              VARCHAR
-            - 'publication_date'  INTEGER
-            - 'publisher'         VARCHAR
-            - 'genres'            VARCHAR
-
-We can see that our Session has a single table, ``checkouts``, with 7 columns, and that
-the 'member_id' column is marked as our ID column.
+regardless of how many books they've checked out.
 
 A simple query with privacy IDs
 -------------------------------
 
 Let's find out what the most popular books in our library are! We can do this
 by counting how many times each book has been checked out.
 
@@ -178,14 +155,15 @@
     |...|...|...|...|
     |...|...|...|...|
     |...|...|...|...|
     |...|...|...|...|
     |...|...|...|...|
     +--------------------+--------------------+----------+-----+
 
+
 .. code-block::
 
     +--------------------+--------------------+----------+-----+
     |               title|              author|      isbn|count|
     +--------------------+--------------------+----------+-----+
     |Comfort Me with A...|         Ruth Reichl|0375758739| 3787|
     |       The Alchemist|Paulo Coelho/Alan...|0061122416| 2441|
@@ -193,45 +171,43 @@
     |     Eat  Pray  Love|   Elizabeth Gilbert|0143038419| 2071|
     |The Tipping Point...|    Malcolm Gladwell|0316346624| 1884|
     +--------------------+--------------------+----------+-----+
 
 With this additional step limiting the maximum contribution of each privacy ID,
 we are now able to run the query and find the five most popular books. This
 step is also called *truncation*: we dropped (or *truncated*) some of the data
-to enforce the desired constraint.
+to enforce the desired constraint. 
 
 More constraints
 ----------------
 
 Limiting the number of rows per privacy ID is not the only way to truncate the
 data and perform queries with privacy IDs. Another option is to limit the
 number of *groups* that each ID can appear in, and limit the number of
 *rows per group* that a single privacy ID can contribute. Let's see an example
 by computing how many patrons have checked out each of our top five books.
 
 For this query, we will combine two constraints to truncate our data:
 
-* :class:`~tmlt.analytics.constraints.MaxGroupsPerID`: limiting the number of
-  groups (here, distinct books) that any library patron can contribute to; and
-* :class:`~tmlt.analytics.constraints.MaxRowsPerGroupPerID`: limiting the number
-  of rows that any library patron can provide for each group.
-
-We will limit each patron to 5 groups (we only consider the 5 most popular
-books) and have patrons only appear once per group (we don't want to count the
-same patron twice for the same book).
+* :class:`~tmlt.analytics.constraints.MaxGroupsPerID`: limiting
+  the number of groups (here, distinct books) that any library patron can contribute to
+* :class:`~tmlt.analytics.constraints.MaxRowsPerGroupPerID`:
+  limiting the number of rows that any library patron can provide for each group.
+
+We will limit each patron to 5 groups (we only consider the 5 most popular books) and have
+patrons only appear once per group (we don't want to count the same patron twice for the same book).
 
 Then, we will create a keyset from our top 5 books and perform a count query:
 
 .. testcode::
 
     top_five_keyset = KeySet.from_dataframe(
         top_five.select("title", "author", "isbn"),
     )
-    count_distinct_query = (
-        QueryBuilder("checkouts")
+    count_distinct_query = (QueryBuilder("checkouts")
         .enforce(MaxGroupsPerID("isbn", 5))
         .enforce(MaxRowsPerGroupPerID("isbn", 1))
         .groupby(top_five_keyset)
         .count()
     )
     result = session.evaluate(count_distinct_query, PureDPBudget(1.5))
     result.show()
@@ -258,60 +234,15 @@
     |Comfort Me with A...|         Ruth Reichl|0375758739|  481|
     |     Eat  Pray  Love|   Elizabeth Gilbert|0143038419|  658|
     |       The Alchemist|Paulo Coelho/Alan...|0061122416|  777|
     |The Devil in the ...|Erik Larson/Tony ...|0739303406|  657|
     |The Tipping Point...|    Malcolm Gladwell|0316346624|  549|
     +--------------------+--------------------+----------+-----+
 
-We could also express this query using
-:meth:`~tmlt.analytics.query_builder.QueryBuilder.count_distinct`: limiting each
-ID to a single row per library member (per ISBN) is the same as counting
-distinct IDs.
-
-.. testcode::
-
-    top_five_keyset = KeySet.from_dataframe(top_five.select("isbn"))
-    count_distinct_query = (
-        QueryBuilder("checkouts")
-        .enforce(MaxGroupsPerID("isbn", 5))
-        .groupby(top_five_keyset)
-        .count_distinct(["member_id"], name="count")
-    )
-    result = session.evaluate(
-        count_distinct_query, PureDPBudget(1.5)
-    ).join(  # Add title/author back to result
-        top_five.select("title", "author", "isbn"), on=["isbn"], how="left"
-    ).select(  # Reorder dataframe columns
-        "title", "author", "isbn", "count"
-    )
-
-.. testcode::
-    :hide:
-
-    result.show()
-
-.. testoutput::
-    :hide:
-    :options: +NORMALIZE_WHITESPACE
-
-    +--------------------+--------------------+----------+-----+
-    |               title|              author|      isbn|count|
-    +--------------------+--------------------+----------+-----+
-    |...|...|...|...|
-    |...|...|...|...|
-    |...|...|...|...|
-    |...|...|...|...|
-    |...|...|...|...|
-    +--------------------+--------------------+----------+-----+
-
-When using `count_distinct` on the ID column, we no longer need to specify the
-`MaxRowsPerGroupPerID` constraint: Tumult Analytics understands that each ID can
-contribute at most once per group.
-
-We can then display the results as a graph:
+We can display this data as a graph:
 
 .. code-block::
 
     import matplotlib.pyplot as plt
     import seaborn as sns
 
     sns.set_theme(style="whitegrid")
@@ -322,29 +253,26 @@
             return row["title"]
         return row["title"][:12] + "..."
 
     data_to_plot["short_title"] = data_to_plot.apply(
         lambda row: shorten_title(row), axis=1
     )
 
-    g = sns.barplot(x="title", y="count", data=data_to_plot, color="#1f77b4")
-    g.set_xticklabels(
-        data_to_plot["short_title"], rotation=45, horizontalalignment="right"
-    )
+    g = sns.barplot(x="short_title", y="count", data=data_to_plot, color="#1f77b4")
+    g.set_xticklabels(g.get_xticklabels(), rotation=45, horizontalalignment="right")
     plt.title("How many members have checked out popular books")
     plt.xlabel("Book Title")
     plt.ylabel("Members")
     plt.tight_layout()
     plt.show()
 
 .. image:: ../images/chart_books_by_unique_members.png
    :alt: A bar chart plotting the number of unique library members who have checked out each book. The most popular book (The Alchemist) has been checked out by about 750 people; each book after that has been checked out by fewer people, with the last book (Comfort Me With...) having been checked out by just under 500 people.
    :align: center
 
-.. _flow-chart-truncation:
 
 Summary
 -------
 
 We've seen that when using privacy IDs, we need to truncate the data to limit
 how much each privacy ID can contribute to the final statistic. There are two
 ways of doing so: using :class:`~tmlt.analytics.constraints.MaxRowsPerID`,
```

### Comparing `tmlt_analytics-0.7.0/doc/tutorials/simple-transformations.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/simple-transformations.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/examples/interactive_evaluation.ipynb` & `tmlt_analytics-0.7.0rc1/examples/interactive_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/examples/private_join.ipynb` & `tmlt_analytics-0.7.0rc1/examples/private_join.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/examples/zcdp_puredp_switching.ipynb` & `tmlt_analytics-0.7.0rc1/examples/zcdp_puredp_switching.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/pyproject.toml` & `tmlt_analytics-0.7.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 homepage = "https://www.tmlt.dev/"
 repository = "https://gitlab.com/tumult-labs/analytics"
 documentation = "https://docs.tmlt.dev/analytics/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.7.0"
+version = "0.7.0-rc.1"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Education",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
```

### Comparing `tmlt_analytics-0.7.0/test/conftest.py` & `tmlt_analytics-0.7.0rc1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/conftest.py` & `tmlt_analytics-0.7.0rc1/test/system/session/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/ids/test_constraint_propagation.py` & `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/ids/test_l0_linf_truncation.py` & `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l0_linf_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/ids/test_l1_truncation.py` & `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l1_truncation.py`

 * *Files 6% similar despite different names*

```diff
@@ -290,14 +290,17 @@
 @pytest.mark.parametrize("session", [INF_BUDGET], indirect=True, ids=["puredp"])
 @pytest.mark.parametrize(
     "query,expected_noise",
     [
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count(), [1]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count(), [2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count(), [5]),
+        (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count_distinct(["id"]), [1]),
+        (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count_distinct(["id"]), [2]),
+        (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count_distinct(["id"]), [5]),
         # Two aggregations, a sum and a count, each with half the budget
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 10), [10, 2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 10), [50, 10]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 20), [20, 2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 20), [100, 10]),
     ],
 )
@@ -313,14 +316,17 @@
 @pytest.mark.parametrize("session", [INF_BUDGET_ZCDP], indirect=True, ids=["zcdp"])
 @pytest.mark.parametrize(
     "query,expected_noise",
     [
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count(), [0.5]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count(), [2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count(), [12.5]),
+        (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count_distinct(["id"]), [0.5]),
+        (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count_distinct(["id"]), [2]),
+        (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count_distinct(["id"]), [12.5]),
         # Two aggregations, a sum and a count, each with half the budget
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 10), [25, 1]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 10), [625, 25]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 20), [100, 1]),
         (
             QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 20),
             [2500, 25],
```

### Comparing `tmlt_analytics-0.7.0/test/system/session/ids/test_partition.py` & `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_partition.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/mixed/test_mixed_session.py` & `tmlt_analytics-0.7.0rc1/test/system/session/mixed/test_mixed_session.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/rows/conftest.py` & `tmlt_analytics-0.7.0rc1/test/system/session/rows/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/rows/test_add_max_rows.py` & `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows.py`

 * *Files 6% similar despite different names*

```diff
@@ -953,66 +953,14 @@
         assert len(list(spark.sparkContext._jsc.sc().getRDDStorageInfo())) == 2
         # Delete views
         session.delete_view("view1")
         assert len(list(spark.sparkContext._jsc.sc().getRDDStorageInfo())) == 1
         session.delete_view("view2")
         assert len(list(spark.sparkContext._jsc.sc().getRDDStorageInfo())) == 0
 
-    # regression test for #2491
-    def test_filter_regression(self, spark) -> None:
-        """Regression tests for issue 2491.
-
-        This issue caused incorrect results when joining a dataframe with
-        another dataframe derived from the first (in this case, a KeySet
-        derived from the private data).
-        """
-        sdf = spark.createDataFrame(
-            pd.DataFrame(
-                [["0", 1, 100000], ["1", 0, 20000], ["1", 2, 20000]],
-                columns=["A", "B", "X"],
-            )
-        )
-        total_budget = 10
-        session = Session.from_dataframe(
-            privacy_budget=PureDPBudget(total_budget),
-            source_id="private",
-            dataframe=sdf,
-            protected_change=AddOneRow(),
-        )
-
-        all_keys = KeySet.from_dataframe(sdf)
-        keyset = all_keys["A", "B"]
-        budget_per_query = PureDPBudget(total_budget / 3)
-        expected_a_b = pd.DataFrame([["0", 1], ["1", 0], ["1", 2]], columns=["A", "B"])
-
-        count_query = QueryBuilder("private").filter("B == 2").groupby(keyset).count()
-        count_result = session.evaluate(count_query, budget_per_query)
-        count_a_b = count_result.select("A", "B")
-        assert_frame_equal_with_sort(count_a_b.toPandas(), expected_a_b)
-
-        median_query = (
-            QueryBuilder("private")
-            .filter("B == 2")
-            .groupby(keyset)
-            .median("X", 0, 10 ** 6, "dp_median")
-        )
-        median_result = session.evaluate(median_query, budget_per_query)
-        median_a_b = median_result.select("A", "B")
-        assert_frame_equal_with_sort(median_a_b.toPandas(), expected_a_b)
-
-        average_query = (
-            QueryBuilder("private")
-            .filter("B == 2")
-            .groupby(keyset)
-            .average("X", 0, 10 ** 6, "dp_average")
-        )
-        average_result = session.evaluate(average_query, budget_per_query)
-        average_a_b = average_result.select("A", "B")
-        assert_frame_equal_with_sort(average_a_b.toPandas(), expected_a_b)
-
     def test_grouping_noninteger_stability(self, spark) -> None:
         """Test that zCDP grouping_column and non-integer stabilities work."""
         grouped_df = spark.createDataFrame(
             pd.DataFrame({"id": [7, 7, 8, 9], "group": [0, 1, 0, 1]})
         )
         ks = KeySet.from_dict({"group": [0, 1]})
         query = QueryBuilder("id").groupby(ks).count()
```

### Comparing `tmlt_analytics-0.7.0/test/system/session/rows/test_add_max_rows_in_max_groups.py` & `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_in_max_groups.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/rows/test_add_max_rows_infs_nulls.py` & `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_infs_nulls.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/rows/test_invalid.py` & `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_invalid.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/system/session/test_invalid_constraints.py` & `tmlt_analytics-0.7.0rc1/test/system/session/test_invalid_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/query_expr_compiler/test_measurement_visitor.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_measurement_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/query_expr_compiler/test_output_schema_visitor.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_output_schema_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/conftest.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_binning_spec.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_binning_spec.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_catalog.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_cleanup.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_constraints.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_keyset.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_neighboring_relations.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_neighboring_relations.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_noise_info.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_noise_info.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_privacy_budget.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_protected_change.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_query_builder.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_query_expr_compiler.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_expr_compiler.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_query_expression.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_expression.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_query_expression_visitor.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_expression_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_schema.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_schema_conversion.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_schema_conversion.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_session.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_table_identifiers.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_table_identifiers.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_transformation_utils.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_truncation_strategy.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/test/unit/test_utils.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_catalog.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_coerce_spark_schema.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_coerce_spark_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_neighboring_relation.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_neighboring_relation_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_noise_info.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_noise_info.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_compiler.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_compiler.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 )
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
     DropNullAndNan,
-    EnforceConstraint,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
     GroupByCountDistinct,
     GroupByQuantile,
@@ -163,98 +162,14 @@
         raise AssertionError(
             f"Constraints {constraints} are not a combination for which a stability "
             "can be computed. This is probably a bug; please let us know about it "
             "so we can fix it!"
         )
 
 
-def _generate_constrained_count_distinct(
-    query: GroupByCountDistinct, schema: Schema, constraints: List[Constraint]
-) -> Optional[GroupByCount]:
-    """Return a more optimal query for the given count-distinct, if one exists.
-
-    This method handles inferring additional constraints on a
-    GroupByCountDistinct query and using those constraints to generate more
-    optimal queries. This is possible in two cases, both on IDs tables:
-
-    - Only the ID column is being counted, and no groupby is performed. When
-      this happens, each ID can contribute at most once to the resulting count,
-      equivalent to a ``MaxRowsPerID(1)`` constraint.
-
-    - Only the ID column is being counted, and the result is grouped on exactly
-      one column which has a MaxGroupsPerID constraint on it. In this case, each
-      ID can contribute at most once to the count of each group, equivalent to a
-      ``MaxRowsPerGroupPerID(other_column, 1)`` constraint.
-
-    In both of these cases, a performance optimization is also possible: because
-    enforcing the constraints drops all but one of the rows per ID in the first
-    case or per (ID, group) value pair in the second, a normal count query will
-    produce the same result and should run faster because it doesn't need to
-    handle deduplicating the values.
-    """
-    columns_to_count = set(query.columns_to_count or schema.columns)
-    groupby_columns = query.groupby_keys.dataframe().columns
-
-    # For non-IDs cases or cases where columns other than the ID column must be
-    # distinct, there's no optimization to make.
-    if schema.id_column is None or columns_to_count != {schema.id_column}:
-        return None
-
-    mechanism = (
-        CountMechanism.DEFAULT
-        if query.mechanism == CountDistinctMechanism.DEFAULT
-        else CountMechanism.LAPLACE
-        if query.mechanism == CountDistinctMechanism.LAPLACE
-        else CountMechanism.GAUSSIAN
-        if query.mechanism == CountDistinctMechanism.GAUSSIAN
-        else None
-    )
-    if mechanism is None:
-        raise AssertionError(
-            f"Unknown mechanism {query.mechanism}. This is probably a bug; "
-            "please let us know about it so we can fix it!"
-        )
-
-    if not groupby_columns:
-        # No groupby is performed; this is equivalent to a MaxRowsPerID(1)
-        # constraint on the table.
-        return GroupByCount(
-            EnforceConstraint(query.child, MaxRowsPerID(1)),
-            groupby_keys=query.groupby_keys,
-            output_column=query.output_column,
-            mechanism=mechanism,
-        )
-    elif len(groupby_columns) == 1:
-        # A groupby on exactly one column is performed; if that column has a
-        # MaxGroupsPerID constraint, then this is equivalent to a
-        # MaxRowsPerGroupsPerID(grouping_column, 1) constraint.
-        grouping_column = groupby_columns[0]
-        constraint = next(
-            (
-                c
-                for c in constraints
-                if isinstance(c, MaxGroupsPerID)
-                and c.grouping_column == grouping_column
-            ),
-            None,
-        )
-        if constraint is not None:
-            return GroupByCount(
-                EnforceConstraint(
-                    query.child, MaxRowsPerGroupPerID(constraint.grouping_column, 1)
-                ),
-                groupby_keys=query.groupby_keys,
-                output_column=query.output_column,
-                mechanism=mechanism,
-            )
-
-    # If none of the above cases are true, no optimization is possible.
-    return None
-
-
 class MeasurementVisitor(QueryExprVisitor):
     """A visitor to create a measurement from a query expression."""
 
     def __init__(
         self,
         per_query_privacy_budget: sp.Expr,
         stability: Any,
@@ -637,35 +552,19 @@
             count_column=query.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
     def visit_groupby_count_distinct(self, query: GroupByCountDistinct) -> Measurement:
         """Create a measurement from a GroupByCountDistinct query expression."""
-        mechanism = self._pick_noise_for_count(query)
-        (
-            child_transformation,
-            child_ref,
-            child_constraints,
-        ) = self._visit_child_transformation(query.child, mechanism)
-        constrained_query = _generate_constrained_count_distinct(
-            query,
-            query.child.accept(OutputSchemaVisitor(self.catalog)),
-            child_constraints,
-        )
-        if constrained_query is not None:
-            return constrained_query.accept(self)
-
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_count_distinct(query)
-
+        mechanism = self._pick_noise_for_count(query)
         child_transformation, child_ref = self._truncate_table(
-            child_transformation,
-            child_ref,
-            child_constraints,
+            *self._visit_child_transformation(query.child, mechanism),
             grouping_columns=query.groupby_keys.dataframe().columns,
         )
         transformation = get_table_from_ref(child_transformation, child_ref)
 
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
@@ -676,15 +575,15 @@
         # If not counting all columns, drop the ones that are neither counted
         # nor grouped on.
         if query.columns_to_count:
             groupby_columns = list(query.groupby_keys.schema().keys())
             transformation |= SelectTransformation(
                 transformation.output_domain,
                 transformation.output_metric,
-                list(set(query.columns_to_count + groupby_columns)),
+                query.columns_to_count + groupby_columns,
             )
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
```

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,14 @@
             **{
                 query.output_column: ColumnDescriptor(
                     output_column_type, allow_null=False
                 )
             },
         },
         grouping_column=None,
-        id_column=None,
     )
     return output_schema
 
 
 class OutputSchemaVisitor(QueryExprVisitor):
     """A visitor to get the output schema of a query expression."""
```

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_schema.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,19 +165,14 @@
                     column_type=ColumnType[ty],
                     allow_null=default_allow_null,
                     allow_nan=default_allow_nan,
                     allow_inf=default_allow_inf,
                 )
 
     @property
-    def columns(self):
-        """Return the names of the columns in the schema."""
-        return self._column_descs.keys()
-
-    @property
     def column_descs(self) -> Dict[str, ColumnDescriptor]:
         """Returns a mapping from column name to column descriptor."""
         return dict(self._column_descs)
 
     @property
     def column_types(self) -> Dict[str, str]:
         """Returns a mapping from column name to column type."""
```

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_table_identifier.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_identifier.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_table_reference.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_reference.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/_transformation_utils.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/binning_spec.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/binning_spec.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/constraints/_base.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class Constraint(ABC):
     """A known, enforceable fact about a table.
 
     Constraints provide information about the contents of a table to help
     produce differentially-private results. For example, a constraint might say
     that each ID in a table corresponds to no more than two rows in that table
     (the :class:`~tmlt.analytics.constraints.MaxRowsPerID`
-    constraint). Constraints are applied via the :meth:`QueryBuilder.enforce()
+    constraint). Constraints are applied via the :meth:`QueryBuilder.enforce
     <tmlt.analytics.query_builder.QueryBuilder.enforce>` method.
 
     This class is a base class for all constraints, and cannot be used directly.
     """
 
     @abstractmethod
     def _enforce(
```

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/constraints/_simplify.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_simplify.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/constraints/_truncation.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/keyset.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/privacy_budget.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/protected_change.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/protected_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
     id_column: str
     """The name of the column containing the identifier."""
 
     id_space: str = "default_id_space"
     """The identifier space of the rows that may be added or removed. If not specified,
     a default will be assigned when using this protected change with
-    :class:`Session.from_dataframe()<tmlt.analytics.session.Session.from_dataframe>`."""
+    :class:`tmlt.analytics.session.Session.from_dataframe`."""
 
     def __post_init__(self):
         """Validate attributes."""
         check_type("id_space", self.id_space, str)
         if self.id_space == "":
             raise ValueError("identifier must be non-empty")
         check_type("id_column", self.id_column, str)
```

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/query_builder.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/query_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -281,24 +281,23 @@
         The current query can also join with a named private table (represented
         as a string).
 
         This operation is a natural join, with the same behavior and requirements as
         :func:`join_public`.
 
         For operations on tables with a
-        :class:`~tmlt.analytics.protected_change.ProtectedChange` that protects
-        adding or removing rows (e.g.
-        :class:`~tmlt.analytics.protected_change.AddMaxRows`), there is a key
-        difference: before the join is performed, each table is *truncated*
-        based on the corresponding
+        :class:`tmlt.analytics.protected_change.ProtectedChange` that protects adding or
+        removing rows (e.g., :class:`~tmlt.analytics.protected_change.AddMaxRows`),
+        there is a key difference: before the join is performed, each table is
+        *truncated* based on the corresponding
         :class:`~tmlt.analytics.truncation_strategy.TruncationStrategy`.
 
         In contrast, operations on tables with a
-        :class:`~tmlt.analytics.protected_change.AddRowsWithID`
-        :class:`~tmlt.analytics.protected_change.ProtectedChange` do not require a
+        :class:`tmlt.analytics.protected_change.AddRowsWithID`
+        :class:`tmlt.analytics.protected_change.ProtectedChange` do not require a
         :class:`~tmlt.analytics.truncation_strategy.TruncationStrategy`, as no
         truncation is necessary while performing the join.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
@@ -995,15 +994,15 @@
                 This function should return a dictionary, which should always
                 have the same keys regardless of input, and the values in that
                 dictionary should match the column type specified in
                 ``new_column_types``. The function should not have any side effects
                 (in particular, f cannot raise exceptions).
             new_column_types: Mapping from column names to types, for new columns
                 produced by f. Using
-                :class:`~tmlt.analytics.query_builder.ColumnDescriptor`
+                :class:`tmlt.analytics.query_builder.ColumnDescriptor`
                 is preferred.
             augment: If True, add new columns to the existing dataframe (so new
                      schema = old schema + schema_new_columns).
                      If False, make the new dataframe with schema = schema_new_columns
         """
         self._query_expr = Map(
             child=self._query_expr,
@@ -1030,16 +1029,16 @@
         """Updates the current query to apply a flat map.
 
         If you provide only a ColumnType for the new column types, Analytics
         assumes that all new columns created may contain null values (and that
         DECIMAL columns may contain NaN or infinite values).
 
         Operations on tables with a
-        :class:`~tmlt.analytics.protected_change.AddRowsWithID`
-        :class:`~tmlt.analytics.protected_change.ProtectedChange` do not require a
+        :class:`tmlt.analytics.protected_change.AddRowsWithID`
+        :class:`tmlt.analytics.protected_change.ProtectedChange` do not require a
         ``max_num_rows`` argument, since it is not necessary to impose a limit on
         the number of new rows.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
@@ -1105,29 +1104,29 @@
                 The function's input is a dictionary matching a column name to
                 its value for that row.
                 This function should return a list of dictionaries.
                 Those dictionaries should always
                 have the same keys regardless of input, and the values in those
                 dictionaries should match the column type specified in
                 ``new_column_types``. The function should not have any side effects
-                (in particular, ``f`` must not raise exceptions).
+                (in particular, f cannot raise exceptions).
             new_column_types: Mapping from column names to types, for new columns
-                produced by ``f``. Using
-                :class:`~tmlt.analytics.query_builder.ColumnDescriptor`
+                produced by f. Using
+                :class:`tmlt.analytics.query_builder.ColumnDescriptor`
                 is preferred.
             augment: If True, add new columns to the existing dataframe (so new
                      schema = old schema + schema_new_columns).
                      If False, make the new dataframe with schema = schema_new_columns
             grouping: Whether this produces a new column that we want to groupby.
                 If True, this requires that any groupby aggregations following this
                 query include the new column as a groupby column. Only one new column
                 is supported, and the new column must have distinct values for each
                 input row.
-            max_num_rows: The enforced limit on the number of rows from each ``f(row)``.
-                If ``f`` produces more rows than this, only the first ``max_num_rows``
+            max_num_rows: The enforced limit on the number of rows from each f(row).
+                If f produces more rows than this, only the first ``max_num_rows``
                 rows will be in the output.
         """
         grouping_column: Optional[str]
         if grouping:
             if len(new_column_types) != 1:
                 raise ValueError(
                     "new_column_types contains "
@@ -1323,17 +1322,14 @@
 
     def enforce(self, constraint: Constraint) -> "QueryBuilder":
         """Enforce a :mod:`~tmlt.analytics.constraints.Constraint` on the current table.
 
         This method can be used to enforce constraints on the current table. See
         the :mod:`~tmlt.analytics.constraints` module for information about the
         available constraints and what they are used for.
-
-        Args:
-            constraint: The constraint to enforce.
         """
         self._query_expr = EnforceConstraint(self._query_expr, constraint, options={})
         return self
 
     def groupby(self, keys: KeySet) -> "GroupedQueryBuilder":
         """Groups the query by the given set of keys, returning a GroupedQueryBuilder.
 
@@ -1535,15 +1531,15 @@
             ... )
             >>> answer.toPandas()
                count
             0      3
 
         Args:
             name: Name for the resulting aggregation column. Defaults to "count".
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).count(name=name, mechanism=mechanism)
 
     def count_distinct(
         self,
         columns: Optional[List[str]] = None,
@@ -1618,15 +1614,15 @@
 
         Args:
             columns: Columns in which to count distinct values. If none are provided,
                 the query will count every distinct row.
             name: Name for the resulting aggregation column. Defaults to
                 "count_distinct" if no columns are provided, or
                 "count_distinct(A, B, C)" if the provided columns are A, B, and C.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
             cols: Deprecated; use ``columns`` instead.
         """
         return self.groupby(KeySet.from_dict({})).count_distinct(
             columns=columns, name=name, mechanism=mechanism, cols=cols
         )
 
@@ -1637,18 +1633,19 @@
         low: float,
         high: float,
         name: Optional[str] = None,
     ) -> QueryExpr:
         """Returns a quantile query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
+
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1708,18 +1705,18 @@
 
     def min(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a minimum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1777,18 +1774,18 @@
 
     def max(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a maximum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1846,18 +1843,18 @@
 
     def median(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a median value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1921,18 +1918,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: SumMechanism = SumMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a sum query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -1987,15 +1984,15 @@
         Args:
             column: The column to compute the sum over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_sum"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).sum(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
     def average(
@@ -2005,18 +2002,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: AverageMechanism = AverageMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns an average query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2071,15 +2068,15 @@
         Args:
             column: The column to compute the average over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_average"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).average(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
     def variance(
@@ -2089,18 +2086,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: VarianceMechanism = VarianceMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a variance query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2155,15 +2152,15 @@
         Args:
             column: The column to compute the variance over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_variance"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).variance(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
     def stdev(
@@ -2173,18 +2170,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: StdevMechanism = StdevMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a standard deviation query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~drop_null_and_nan` query will be performed first. If the
-            column being measured contains infinite values, a
-            :meth:`~drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2239,15 +2236,15 @@
         Args:
             column: The column to compute the stdev over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_stdev"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).stdev(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
 
@@ -2323,15 +2320,15 @@
             >>> answer.sort("A").toPandas()
                A  count
             0  0      1
             1  1      2
 
         Args:
             name: Name for the resulting aggregation column. Defaults to "count".
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = "count"
         query_expr = GroupByCount(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -2399,15 +2396,15 @@
 
         Args:
             columns: Columns in which to count distinct values. If none are provided,
                 the query will count every distinct row.
             name: Name for the resulting aggregation column. Defaults to
                 "count_distinct" if no columns are provided, or
                 "count_distinct(A, B, C)" if the provided columns are A, B, and C.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
             cols: Deprecated; use ``columns`` instead.
         """
         if cols is not None:
             warnings.warn(
                 "The `cols` argument is deprecated; use `columns` instead",
                 DeprecationWarning,
@@ -2442,18 +2439,18 @@
         low: float,
         high: float,
         name: Optional[str] = None,
     ) -> QueryExpr:
         """Returns a quantile query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2524,18 +2521,18 @@
 
     def min(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a minimum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2599,18 +2596,18 @@
 
     def max(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a maximum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2674,18 +2671,18 @@
 
     def median(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a median value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2751,18 +2748,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: SumMechanism = SumMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a sum query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a ``drop_null_and_nan`` query will be performed first. If the column being
+            measured contains infinite values, a ``drop_infinity`` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2819,15 +2816,15 @@
         Args:
             column: The column to compute the sum over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_sum"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_sum"
         query_expr = GroupByBoundedSum(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -2846,18 +2843,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: AverageMechanism = AverageMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns an average query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a `drop_null_and_nan` query will be performed first. If the column being
+            measured contains infinite values, a `drop_infinity` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2914,15 +2911,15 @@
         Args:
             column: The column to compute the average over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_average"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_average"
         query_expr = GroupByBoundedAverage(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -2941,18 +2938,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: VarianceMechanism = VarianceMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a variance query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a `drop_null_and_nan` query will be performed first. If the column being
+            measured contains infinite values, a `drop_infinity` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -3009,15 +3006,15 @@
         Args:
             column: The column to compute the variance over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_variance"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_variance"
         query_expr = GroupByBoundedVariance(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -3036,18 +3033,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: StdevMechanism = StdevMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a standard deviation query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values, a
-            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
-            first. If the column being measured contains infinite values, a
-            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
+            If the column being measured contains NaN or null values,
+            a `drop_null_and_nan` query will be performed first. If the column being
+            measured contains infinite values, a `drop_infinity` query will be
+            performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -3104,15 +3101,15 @@
         Args:
             column: The column to compute the stdev over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_stdev"``.
-            mechanism: Choice of noise mechanism. By default, the framework
+            mechanism: Choice of noise mechanism. By DEFAULT, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_stdev"
         query_expr = GroupByBoundedSTDEV(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
```

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/query_expr.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/query_expr.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/session.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,17 +238,17 @@
             :data:`SUPPORTED_SPARK_TYPES` for information about which types are
             supported.
 
             Args:
                 source_id: Source id for the private source dataframe.
                 dataframe: Private source dataframe to perform queries on,
                     corresponding to the ``source_id``.
-                stability: Deprecated: use ``protected_change`` instead, see
+                stability: Use ``protected_change`` instead, see
                     :ref:`changelog<changelog#protected-change>`.
-                grouping_column: Deprecated: use ``protected_change`` instead, see
+                grouping_column: Use ``protected_change`` instead, see
                     :ref:`changelog<changelog#protected-change>`.
                 protected_change: A
                     :class:`~tmlt.analytics.protected_change.ProtectedChange`
                     specifying what changes to the input data the resulting
                     :class:`Session` should protect.
             """
             _assert_is_identifier(source_id)
@@ -269,14 +269,17 @@
                         " protected_change."
                     )
                 self._private_sources[source_id] = _PrivateSourceTuple(
                     dataframe, protected_change, domain
                 )
                 return self
 
+            # TODO(#2722): All paths through the below need deprecation
+            #     warnings, for either the use of stability/grouping_column or
+            #     the assumption of AddOneRow() if no stability is specified.
             if stability is None:
                 warn(
                     "Using a default for protected_change is deprecated. Future"
                     " code should explicitly specify protected_change=AddOneRow()",
                     DeprecationWarning,
                 )
                 if grouping_column is None:
@@ -339,24 +342,22 @@
             if source_id in self._private_sources or source_id in self._public_sources:
                 raise ValueError(f"Duplicate source id: '{source_id}'")
             dataframe = coerce_spark_schema_or_fail(dataframe)
             self._public_sources[source_id] = dataframe
             return self
 
         def with_id_space(self, id_space: str) -> "Session.Builder":
-            """Creates an identifier space for the session.
+            """Sets the identifier space for the session.
 
-            This defines a space of identifiers that map 1-to-1 to the
-            identifiers being protected by a table with the
-            :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected
-            change. Any table with such a protected change must be a member of
-            some identifier space.
+            This defines the space of identifiers that map 1-to-1 to the identifiers
+            being protected. Any IDs table must have exactly one column containing
+            those identifiers.
 
             Args:
-                id_space: The name of the identifier space.
+                id_space: The identifier space for the session.
             """
             _assert_is_identifier(id_space)
             if id_space in self._id_spaces:
                 raise ValueError(
                     f"This Builder already has an ID space of the name: {id_space}."
                 )
             self._id_spaces.append(id_space)
@@ -479,17 +480,17 @@
             {'A': 'VARCHAR', 'B': 'INTEGER', 'X': 'INTEGER'}
 
         Args:
             privacy_budget: The total privacy budget allocated to this session.
             source_id: The source id for the private source dataframe.
             dataframe: The private source dataframe to perform queries on,
                 corresponding to the `source_id`.
-            stability: Deprecated: use ``protected_change`` instead, see
+            stability: Use ``protected_change`` instead, see
                 :ref:`changelog<changelog#protected-change>`
-            grouping_column: Deprecated: use ``protected_change`` instead, see
+            grouping_column: Use ``protected_change`` instead, see
                 :ref:`changelog<changelog#protected-change>`
             protected_change: A
                 :class:`~tmlt.analytics.protected_change.ProtectedChange`
                 specifying what changes to the input data the resulting
                 :class:`Session` should protect.
         """
         # pylint: enable=line-too-long
@@ -644,126 +645,14 @@
             raise AssertionError(
                 "Session accountant's input metric has an incorrect type. This is "
                 "probably a bug; please let us know about it so we can "
                 "fix it!"
             )
         return self._accountant.input_metric
 
-    def describe(
-        self, obj: Optional[Union[QueryExpr, QueryBuilder, str]] = None
-    ) -> None:
-        """Describe a Session, table, or query.
-
-        If ``obj`` is not specified, ``session.describe()`` will describe the
-        Session and all of the tables it contains.
-
-        If ``obj`` is a :class:`~tmlt.analytics.query_builder.QueryBuilder` or
-        :class:`~tmlt.analytics.query_expr.QueryExpr`, ``session.describe(obj)``
-        will describe the table that would result from that query if it were
-        applied to the Session.
-
-        If ``obj`` is a string, ``session.describe(obj)`` will describe the table
-        with that name. This is a shorthand for
-        ``session.describe(QueryBuilder(obj))``.
-
-        Args:
-            obj: The table or query to be described, or None to describe the
-                whole Session.
-        """
-        if obj is None:
-            self._describe_self()
-        elif isinstance(obj, QueryExpr):
-            self._describe_query(obj)
-        elif isinstance(obj, QueryBuilder):
-            self._describe_query(obj.query_expr)
-        elif isinstance(obj, str):
-            self._describe_query(QueryBuilder(obj).query_expr)
-        else:
-            assert_never(obj)
-
-    def _describe_self(self) -> None:
-        """Describe the current state of this session."""
-        out = []
-        state = self._accountant.state
-        if state == PrivacyAccountantState.ACTIVE:
-            # Don't add anything to output if the session is active
-            pass
-        elif state == PrivacyAccountantState.RETIRED:
-            out.append("This session has been stopped, and can no longer be used.")
-        elif state == PrivacyAccountantState.WAITING_FOR_CHILDREN:
-            out.append(
-                "This session is waiting for its children (created with"
-                " `partition_and_create`) to finish."
-            )
-        elif state == PrivacyAccountantState.WAITING_FOR_SIBLING:
-            out.append(
-                "This session is waiting for its sibling(s) (created with"
-                " `partition_and_create`) to finish."
-            )
-        else:
-            raise AssertionError(
-                f"Unrecognized accountant state {out}. This is probably a bug; please"
-                " let us know about it so we can fix it!"
-            )
-        budget: PrivacyBudget = self.remaining_privacy_budget
-        out.append(f"The session has a remaining privacy budget of {budget}.")
-        if len(self._catalog.tables) == 0:
-            out.append("The session has no tables available.")
-        else:
-            public_table_descs = []
-            private_table_descs = []
-            for name, table in self._catalog.tables.items():
-                column_strs = ["\t" + e for e in _describe_schema(table.schema)]
-                columns_desc = "\n".join(column_strs)
-                if isinstance(table, PublicTable):
-                    table_desc = f"Public table '{name}':\n" + columns_desc
-                    public_table_descs.append(table_desc)
-                elif isinstance(table, PrivateTable):
-                    table_desc = f"Table '{name}':\n"
-                    table_desc += columns_desc
-
-                    constraints: Optional[
-                        List[Constraint]
-                    ] = self._table_constraints.get(NamedTable(name))
-                    if not constraints:
-                        table_desc = (
-                            f"Table '{name}' (no constraints):\n" + columns_desc
-                        )
-                    else:
-                        table_desc = (
-                            f"Table '{name}':\n" + columns_desc + "\n\tConstraints:\n"
-                        )
-                        constraints_strs = [f"\t\t- {e}" for e in constraints]
-                        table_desc += "\n".join(constraints_strs)
-
-                    private_table_descs.append(table_desc)
-                else:
-                    raise AssertionError(
-                        f"Table {name} has an unrecognized type: {type(table)}. This is"
-                        " probably a bug; please let us know about it so we can"
-                        " fix it!"
-                    )
-            if len(private_table_descs) != 0:
-                out.append(
-                    "The following private tables are available:\n"
-                    + "\n".join(private_table_descs)
-                )
-            if len(public_table_descs) != 0:
-                out.append(
-                    "The following public tables are available:\n"
-                    + "\n".join(public_table_descs)
-                )
-        print("\n".join(out))
-
-    def _describe_query(self, query: QueryExpr):
-        """Describe the output schema of a query and the constraints on it."""
-        schema = self._compiler.query_schema(query, self._catalog)
-        out = _describe_schema(schema)
-        print("\n".join(out))
-
     @typechecked
     def get_schema(self, source_id: str) -> Schema:
         """Returns the schema for any data source.
 
         This includes information on whether the columns are nullable.
 
         Args:
@@ -1286,19 +1175,17 @@
         source_id: str,
         privacy_budget: PrivacyBudget,
         column: Optional[str] = None,
         splits: Optional[Union[Dict[str, str], Dict[str, int]]] = None,
     ) -> Dict[str, "Session"]:
         """Returns new sessions from a partition mapped to split name/``source_id``.
 
-        The type of privacy budget that you use must match the type your Session
-        was initialized with (i.e., you cannot use a
-        :class:`~tmlt.analytics.privacy_budget.RhoZCDPBudget` to partition your
-        Session if the Session was created using a
-        :class:`~tmlt.analytics.privacy_budget.PureDPBudget`, and vice versa).
+        The type of privacy budget that you use must match the type your Session was
+        initialized with (i.e., you cannot use a RhoZCDPBudget to partition your
+        Session if the Session was created using a PureDPBudget, and vice versa).
 
         The sessions returned must be used in the order that they were created.
         Using this session again or calling stop() will stop all partition sessions.
 
         ..
             >>> # Get data
             >>> spark = SparkSession.builder.getOrCreate()
@@ -1662,14 +1549,125 @@
             )
         self._accountant.force_activate()
 
     def stop(self) -> None:
         """Close out this session, allowing other sessions to become active."""
         self._accountant.retire()
 
+    def describe(self, x: Optional[Union[QueryExpr, QueryBuilder, str]] = None) -> None:
+        """Describe this session, or a query, or a table.
+
+        If ``x`` is ``None``, ``session._describe(x)`` will describe the session.
+
+        If ``x`` is a
+        :class:`~tmlt.analytics.query_expr.QueryExpr`,
+        ``session._describe(x)`` will describe
+        the schema resulting from that query expression.
+
+        If x is a
+        :class:`~tmlt.analytics.query_builder.QueryBuilder`,
+        ``session._describe(x) will describe the query constructed by the
+        query builder. This is equivalent to calling
+        ``session._describe(x.query_expr)``.
+
+        If x is a string, x is assumed to be a table name. In this case,
+        ``session._describe(x)`` is equivalent to
+        ``session._describe(QueryBuilder(x))``.
+        """
+        if x is None:
+            self._describe_self()
+        elif isinstance(x, QueryExpr):
+            self._describe_query(x)
+        elif isinstance(x, QueryBuilder):
+            self._describe_query(x.query_expr)
+        elif isinstance(x, str):
+            self._describe_query(QueryBuilder(x).query_expr)
+        else:
+            assert_never(x)
+
+    def _describe_self(self) -> None:
+        """Describe the current state of this session."""
+        out = []
+        state = self._accountant.state
+        if state == PrivacyAccountantState.ACTIVE:
+            # Don't add anything to output if the session is active
+            pass
+        elif state == PrivacyAccountantState.RETIRED:
+            out.append("This session has been stopped, and can no longer be used.")
+        elif state == PrivacyAccountantState.WAITING_FOR_CHILDREN:
+            out.append(
+                "This session is waiting for its children (created with"
+                " `partition_and_create`) to finish."
+            )
+        elif state == PrivacyAccountantState.WAITING_FOR_SIBLING:
+            out.append(
+                "This session is waiting for its sibling(s) (created with"
+                " `partition_and_create`) to finish."
+            )
+        else:
+            raise AssertionError(
+                f"Unrecognized accountant state {out}. This is probably a bug; please"
+                " let us know about it so we can fix it!"
+            )
+        budget: PrivacyBudget = self.remaining_privacy_budget
+        out.append(f"The session has a remaining privacy budget of {budget}.")
+        if len(self._catalog.tables) == 0:
+            out.append("The session has no tables available.")
+        else:
+            public_table_descs = []
+            private_table_descs = []
+            for name, table in self._catalog.tables.items():
+                column_strs = ["\t" + e for e in _describe_schema(table.schema)]
+                columns_desc = "\n".join(column_strs)
+                if isinstance(table, PublicTable):
+                    table_desc = f"Public table '{name}':\n" + columns_desc
+                    public_table_descs.append(table_desc)
+                elif isinstance(table, PrivateTable):
+                    table_desc = f"Table '{name}':\n"
+                    table_desc += columns_desc
+
+                    constraints: Optional[
+                        List[Constraint]
+                    ] = self._table_constraints.get(NamedTable(name))
+                    if not constraints:
+                        table_desc = (
+                            f"Table '{name}' (no constraints):\n" + columns_desc
+                        )
+                    else:
+                        table_desc = (
+                            f"Table '{name}':\n" + columns_desc + "\n\tConstraints:\n"
+                        )
+                        constraints_strs = [f"\t\t- {e}" for e in constraints]
+                        table_desc += "\n".join(constraints_strs)
+
+                    private_table_descs.append(table_desc)
+                else:
+                    raise AssertionError(
+                        f"Table {name} has an unrecognized type: {type(table)}. This is"
+                        " probably a bug; please let us know about it so we can"
+                        " fix it!"
+                    )
+            if len(private_table_descs) != 0:
+                out.append(
+                    "The following private tables are available:\n"
+                    + "\n".join(private_table_descs)
+                )
+            if len(public_table_descs) != 0:
+                out.append(
+                    "The following public tables are available:\n"
+                    + "\n".join(public_table_descs)
+                )
+        print("\n".join(out))
+
+    def _describe_query(self, query: QueryExpr):
+        """Describe the output schema of a query and the constraints on it."""
+        schema = self._compiler.query_schema(query, self._catalog)
+        out = _describe_schema(schema)
+        print("\n".join(out))
+
 
 def _assert_is_identifier(source_id: str):
     """Checks that the ``source_id`` is a valid Python identifier.
 
     Args:
         source_id: The name of the dataframe or transformation.
     """
```

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/truncation_strategy.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/tmlt/analytics/utils.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0/setup.py` & `tmlt_analytics-0.7.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sympy>=1.8,<1.10',
  'tmlt.core>=0.9.0,<0.10.0',
  'typeguard>=2.12.1,<2.13.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'tmlt-analytics',
-    'version': '0.7.0',
+    'version': '0.7.0rc1',
     'description': "Tumult's differential privacy analytics API",
     'long_description': '# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions/concerns, please [create an issue](https://gitlab.com/tumult-labs/analytics/-/issues) or reach out to us on [Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\n## Contributing\n\nWe are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nThe Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nThe Tumult Platform documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.tmlt.dev/',
```

### Comparing `tmlt_analytics-0.7.0/PKG-INFO` & `tmlt_analytics-0.7.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-analytics
-Version: 0.7.0
+Version: 0.7.0rc1
 Summary: Tumult's differential privacy analytics API
 Home-page: https://www.tmlt.dev/
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.10.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

