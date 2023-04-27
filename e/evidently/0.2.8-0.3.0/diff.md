# Comparing `tmp/evidently-0.2.8.tar.gz` & `tmp/evidently-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evidently-0.2.8.tar", last modified: Wed Mar 29 22:02:09 2023, max compression
+gzip compressed data, was "evidently-0.3.0.tar", last modified: Wed Apr 12 10:10:18 2023, max compression
```

## Comparing `evidently-0.2.8.tar` & `evidently-0.3.0.tar`

### file list

```diff
@@ -1,311 +1,205 @@
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.521744 evidently-0.2.8/
--rw-r--r--   0 emelidral   (501) staff       (20)      389 2023-03-29 22:02:09.521857 evidently-0.2.8/PKG-INFO
--rw-r--r--   0 emelidral   (501) staff       (20)     1373 2023-01-26 16:57:34.912306 evidently-0.2.8/setup.cfg
--rw-r--r--   0 emelidral   (501) staff       (20)     2039 2023-03-22 11:45:39.927356 evidently-0.2.8/setup.py
--rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-02-09 17:20:42.839338 evidently-0.2.8/setupbase.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.471783 evidently-0.2.8/src/
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.475648 evidently-0.2.8/src/evidently/
--rw-r--r--   0 emelidral   (501) staff       (20)      256 2022-09-27 21:22:07.984106 evidently-0.2.8/src/evidently/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7126 2023-01-26 16:57:34.912699 evidently-0.2.8/src/evidently/__main__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      162 2022-09-27 21:22:07.984507 evidently-0.2.8/src/evidently/_config.py
--rw-r--r--   0 emelidral   (501) staff       (20)      111 2023-03-29 21:59:17.449087 evidently-0.2.8/src/evidently/_version.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.477458 evidently-0.2.8/src/evidently/analyzers/
--rw-r--r--   0 emelidral   (501) staff       (20)       80 2022-11-16 10:53:30.690356 evidently-0.2.8/src/evidently/analyzers/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1002 2023-03-22 11:45:39.927526 evidently-0.2.8/src/evidently/analyzers/base_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5406 2023-01-26 16:57:34.913084 evidently-0.2.8/src/evidently/analyzers/cat_target_drift_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4790 2023-03-22 11:45:39.927699 evidently-0.2.8/src/evidently/analyzers/classification_performance_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1633 2023-01-26 16:57:34.914245 evidently-0.2.8/src/evidently/analyzers/data_drift_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5856 2023-02-17 14:41:03.890478 evidently-0.2.8/src/evidently/analyzers/data_quality_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5039 2023-01-26 16:57:34.915559 evidently-0.2.8/src/evidently/analyzers/num_target_drift_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16573 2023-01-26 16:57:34.915789 evidently-0.2.8/src/evidently/analyzers/prob_classification_performance_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)      971 2023-01-26 16:57:34.915962 evidently-0.2.8/src/evidently/analyzers/prob_distribution_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2643 2023-01-26 16:57:34.916168 evidently-0.2.8/src/evidently/analyzers/regression_performance_analyzer.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9963 2023-03-22 11:45:39.927982 evidently-0.2.8/src/evidently/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.478713 evidently-0.2.8/src/evidently/calculations/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-09-05 08:44:13.921228 evidently-0.2.8/src/evidently/calculations/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-03-22 11:45:39.928161 evidently-0.2.8/src/evidently/calculations/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)    15897 2023-03-29 20:31:40.150243 evidently-0.2.8/src/evidently/calculations/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2662 2022-11-16 10:53:30.690642 evidently-0.2.8/src/evidently/calculations/data_integration.py
--rw-r--r--   0 emelidral   (501) staff       (20)    31373 2023-03-22 11:45:39.928526 evidently-0.2.8/src/evidently/calculations/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-03-22 11:45:39.928719 evidently-0.2.8/src/evidently/calculations/regression_performance.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.482789 evidently-0.2.8/src/evidently/calculations/stattests/
--rw-r--r--   0 emelidral   (501) staff       (20)     1184 2023-03-03 10:18:49.587082 evidently-0.2.8/src/evidently/calculations/stattests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1337 2023-02-17 14:41:03.892721 evidently-0.2.8/src/evidently/calculations/stattests/anderson_darling_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1741 2022-11-23 07:36:22.485327 evidently-0.2.8/src/evidently/calculations/stattests/chisquare_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5295 2022-11-23 07:36:22.486075 evidently-0.2.8/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1533 2022-11-23 07:36:22.487597 evidently-0.2.8/src/evidently/calculations/stattests/energy_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2108 2022-11-23 07:36:22.488270 evidently-0.2.8/src/evidently/calculations/stattests/epps_singleton_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2592 2022-11-23 07:36:22.488846 evidently-0.2.8/src/evidently/calculations/stattests/fisher_exact_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-03-22 11:45:39.928885 evidently-0.2.8/src/evidently/calculations/stattests/g_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2983 2022-11-23 07:36:22.489903 evidently-0.2.8/src/evidently/calculations/stattests/hellinger_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-02-17 14:41:03.892982 evidently-0.2.8/src/evidently/calculations/stattests/jensenshannon.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1899 2022-11-23 07:36:22.491278 evidently-0.2.8/src/evidently/calculations/stattests/kl_div.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1545 2022-11-23 07:36:22.491685 evidently-0.2.8/src/evidently/calculations/stattests/ks_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1732 2023-03-22 11:45:39.928991 evidently-0.2.8/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4434 2022-12-07 18:36:44.762459 evidently-0.2.8/src/evidently/calculations/stattests/mmd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-03-22 11:45:39.929179 evidently-0.2.8/src/evidently/calculations/stattests/psi.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4586 2023-01-26 16:57:34.919333 evidently-0.2.8/src/evidently/calculations/stattests/registry.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1490 2022-11-23 07:36:22.492511 evidently-0.2.8/src/evidently/calculations/stattests/t_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)      743 2023-01-26 16:57:34.919431 evidently-0.2.8/src/evidently/calculations/stattests/text_content_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2746 2022-11-23 07:36:22.492693 evidently-0.2.8/src/evidently/calculations/stattests/tvd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-03-22 11:45:39.929302 evidently-0.2.8/src/evidently/calculations/stattests/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1832 2022-11-23 07:36:22.493430 evidently-0.2.8/src/evidently/calculations/stattests/wasserstein_distance_norm.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-02-17 14:41:03.893247 evidently-0.2.8/src/evidently/calculations/stattests/z_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-02-17 14:41:03.893517 evidently-0.2.8/src/evidently/calculations/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)      194 2023-03-22 11:45:39.929381 evidently-0.2.8/src/evidently/core.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.483163 evidently-0.2.8/src/evidently/dashboard/
--rw-r--r--   0 emelidral   (501) staff       (20)      154 2022-11-16 10:53:30.693498 evidently-0.2.8/src/evidently/dashboard/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6358 2023-01-26 16:57:34.920550 evidently-0.2.8/src/evidently/dashboard/dashboard.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.484868 evidently-0.2.8/src/evidently/dashboard/tabs/
--rw-r--r--   0 emelidral   (501) staff       (20)      449 2022-09-27 21:22:07.989782 evidently-0.2.8/src/evidently/dashboard/tabs/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2594 2022-10-11 19:17:03.958180 evidently-0.2.8/src/evidently/dashboard/tabs/base_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)      993 2022-10-11 19:17:03.943277 evidently-0.2.8/src/evidently/dashboard/tabs/cat_target_drift_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2101 2022-10-11 19:17:03.953212 evidently-0.2.8/src/evidently/dashboard/tabs/classification_performance_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)      323 2022-09-27 21:22:07.990449 evidently-0.2.8/src/evidently/dashboard/tabs/data_drift_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)      708 2022-10-11 19:17:03.961813 evidently-0.2.8/src/evidently/dashboard/tabs/data_quality_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1138 2022-10-11 19:17:03.973444 evidently-0.2.8/src/evidently/dashboard/tabs/num_target_drift_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3945 2022-10-11 19:17:03.992871 evidently-0.2.8/src/evidently/dashboard/tabs/prob_classification_performance_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4024 2022-10-11 19:17:03.991542 evidently-0.2.8/src/evidently/dashboard/tabs/regression_performance_tab.py
--rw-r--r--   0 emelidral   (501) staff       (20)      869 2022-09-27 21:22:07.991167 evidently-0.2.8/src/evidently/dashboard/tabs/widget_gallery_tab.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.493158 evidently-0.2.8/src/evidently/dashboard/widgets/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-01-24 12:25:45.652411 evidently-0.2.8/src/evidently/dashboard/widgets/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1288 2022-09-27 21:22:07.991292 evidently-0.2.8/src/evidently/dashboard/widgets/bar_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3348 2022-10-11 19:17:04.022582 evidently-0.2.8/src/evidently/dashboard/widgets/cat_output_drift_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11666 2022-10-11 19:17:04.054073 evidently-0.2.8/src/evidently/dashboard/widgets/cat_target_pred_feature_table_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2797 2022-10-11 19:17:04.007377 evidently-0.2.8/src/evidently/dashboard/widgets/class_conf_matrix_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9747 2022-10-11 19:17:04.068052 evidently-0.2.8/src/evidently/dashboard/widgets/class_confusion_based_feature_distr_table_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3133 2022-10-11 19:17:04.034803 evidently-0.2.8/src/evidently/dashboard/widgets/class_metrics_matrix_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2702 2022-10-11 19:17:04.025311 evidently-0.2.8/src/evidently/dashboard/widgets/class_quality_metrics_bar_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3102 2022-10-11 19:17:04.047825 evidently-0.2.8/src/evidently/dashboard/widgets/class_support_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1322 2022-10-11 19:17:04.032616 evidently-0.2.8/src/evidently/dashboard/widgets/class_target_name_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)      811 2022-10-11 19:17:04.046592 evidently-0.2.8/src/evidently/dashboard/widgets/counter_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13020 2023-03-22 11:45:39.929543 evidently-0.2.8/src/evidently/dashboard/widgets/data_drift_table_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8578 2022-10-26 16:56:38.334604 evidently-0.2.8/src/evidently/dashboard/widgets/data_quality_correlations.py
--rw-r--r--   0 emelidral   (501) staff       (20)    33747 2022-10-26 16:56:38.334818 evidently-0.2.8/src/evidently/dashboard/widgets/data_quality_features_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5158 2022-10-11 19:17:04.086567 evidently-0.2.8/src/evidently/dashboard/widgets/data_quality_summary_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12214 2022-10-11 19:17:04.165311 evidently-0.2.8/src/evidently/dashboard/widgets/expandable_list_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2990 2023-03-22 11:45:39.929651 evidently-0.2.8/src/evidently/dashboard/widgets/num_output_corr_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4361 2022-10-11 19:17:04.100956 evidently-0.2.8/src/evidently/dashboard/widgets/num_output_drift_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5734 2022-10-11 19:17:04.133216 evidently-0.2.8/src/evidently/dashboard/widgets/num_output_values_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5017 2022-10-11 19:17:04.125420 evidently-0.2.8/src/evidently/dashboard/widgets/num_target_pred_feature_table_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1789 2022-10-11 19:17:04.096413 evidently-0.2.8/src/evidently/dashboard/widgets/percent_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2916 2022-10-11 19:17:04.124635 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_conf_matrix_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)    15799 2022-10-11 19:17:04.216810 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_confusion_based_feature_distr_table_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3167 2022-10-11 19:17:04.149464 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_metrics_matrix_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4868 2022-10-11 19:17:04.194202 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_pr_curve_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6742 2022-10-11 19:17:04.240091 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_pr_table_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3671 2022-10-11 19:17:04.179323 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_pred_distr_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4194 2022-10-11 19:17:04.220781 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_prediction_cloud_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2614 2022-10-11 19:17:04.213767 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_quality_metrics_bar_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5287 2022-10-11 19:17:04.193271 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_roc_curve_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2951 2022-10-11 19:17:04.208376 evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_support_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4177 2022-10-11 19:17:04.261334 evidently-0.2.8/src/evidently/dashboard/widgets/reg_abs_perc_error_in_time_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5111 2022-10-11 19:17:04.235429 evidently-0.2.8/src/evidently/dashboard/widgets/reg_colored_pred_vs_actual_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3186 2022-10-11 19:17:04.259419 evidently-0.2.8/src/evidently/dashboard/widgets/reg_error_distr_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3919 2022-10-11 19:17:04.252800 evidently-0.2.8/src/evidently/dashboard/widgets/reg_error_in_time_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3720 2022-10-11 19:17:04.279363 evidently-0.2.8/src/evidently/dashboard/widgets/reg_error_normality_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4260 2022-10-11 19:17:04.255115 evidently-0.2.8/src/evidently/dashboard/widgets/reg_pred_and_actual_in_time_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3099 2022-10-11 19:17:04.265920 evidently-0.2.8/src/evidently/dashboard/widgets/reg_pred_vs_actual_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2643 2022-10-11 19:17:04.265687 evidently-0.2.8/src/evidently/dashboard/widgets/reg_quality_metrics_bar_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3145 2022-10-11 19:17:04.275492 evidently-0.2.8/src/evidently/dashboard/widgets/reg_underperform_metrics_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)    20453 2022-10-11 19:17:04.417502 evidently-0.2.8/src/evidently/dashboard/widgets/reg_underperform_segments_table_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3196 2022-10-11 19:17:04.286685 evidently-0.2.8/src/evidently/dashboard/widgets/target_name_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2571 2022-10-11 19:17:04.287259 evidently-0.2.8/src/evidently/dashboard/widgets/test_suite_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)      755 2022-09-05 08:44:13.936391 evidently-0.2.8/src/evidently/dashboard/widgets/text_widget.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1303 2022-09-05 08:44:13.936527 evidently-0.2.8/src/evidently/dashboard/widgets/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)      767 2022-09-05 08:44:13.936678 evidently-0.2.8/src/evidently/dashboard/widgets/widget.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.494017 evidently-0.2.8/src/evidently/descriptors/
--rw-r--r--   0 emelidral   (501) staff       (20)      249 2023-03-03 10:18:49.587277 evidently-0.2.8/src/evidently/descriptors/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-03-03 10:18:49.587546 evidently-0.2.8/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      582 2023-03-03 10:18:49.587773 evidently-0.2.8/src/evidently/descriptors/oov_words_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-03-03 10:18:49.587947 evidently-0.2.8/src/evidently/descriptors/text_length_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      776 2023-03-03 10:18:49.588219 evidently-0.2.8/src/evidently/descriptors/trigger_words_presence_descriptor.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.495059 evidently-0.2.8/src/evidently/features/
--rw-r--r--   0 emelidral   (501) staff       (20)     1682 2023-03-22 11:45:39.929863 evidently-0.2.8/src/evidently/features/OOV_words_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-01-26 16:57:34.920717 evidently-0.2.8/src/evidently/features/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1789 2023-03-03 10:18:49.588650 evidently-0.2.8/src/evidently/features/generated_features.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1095 2023-03-22 11:45:39.930042 evidently-0.2.8/src/evidently/features/non_letter_character_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)      966 2023-03-22 11:45:39.930218 evidently-0.2.8/src/evidently/features/text_length_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2121 2023-03-22 11:45:39.930398 evidently-0.2.8/src/evidently/features/trigger_words_presence_feature.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.496415 evidently-0.2.8/src/evidently/metric_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-01-26 16:57:34.921642 evidently-0.2.8/src/evidently/metric_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-03-22 11:45:39.930512 evidently-0.2.8/src/evidently/metric_preset/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3973 2023-03-22 11:45:39.930623 evidently-0.2.8/src/evidently/metric_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-03-22 11:45:39.930734 evidently-0.2.8/src/evidently/metric_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-03-22 11:45:39.930844 evidently-0.2.8/src/evidently/metric_preset/metric_preset.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-03-22 11:45:39.930961 evidently-0.2.8/src/evidently/metric_preset/regression_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-03-22 11:45:39.931079 evidently-0.2.8/src/evidently/metric_preset/target_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-03-22 11:45:39.931192 evidently-0.2.8/src/evidently/metric_preset/text_overview.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7346 2023-03-22 11:45:39.931279 evidently-0.2.8/src/evidently/metric_results.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.496907 evidently-0.2.8/src/evidently/metrics/
--rw-r--r--   0 emelidral   (501) staff       (20)     3674 2023-01-26 16:57:34.922937 evidently-0.2.8/src/evidently/metrics/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-01-26 16:57:34.924969 evidently-0.2.8/src/evidently/metrics/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.499367 evidently-0.2.8/src/evidently/metrics/classification_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-10-20 11:05:23.165249 evidently-0.2.8/src/evidently/metrics/classification_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2994 2023-03-22 11:45:39.931417 evidently-0.2.8/src/evidently/metrics/classification_performance/base_classification_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2890 2023-03-22 11:45:39.931553 evidently-0.2.8/src/evidently/metrics/classification_performance/class_balance_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4298 2023-03-29 20:31:40.150718 evidently-0.2.8/src/evidently/metrics/classification_performance/class_separation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11993 2023-03-22 11:45:39.931813 evidently-0.2.8/src/evidently/metrics/classification_performance/classification_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5193 2023-03-22 11:45:39.931942 evidently-0.2.8/src/evidently/metrics/classification_performance/classification_quality_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3312 2023-03-22 11:45:39.932081 evidently-0.2.8/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1549 2023-03-22 14:23:20.688288 evidently-0.2.8/src/evidently/metrics/classification_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4483 2023-03-22 11:45:39.932259 evidently-0.2.8/src/evidently/metrics/classification_performance/pr_curve_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6020 2023-03-29 20:31:40.151266 evidently-0.2.8/src/evidently/metrics/classification_performance/pr_table_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5884 2023-03-22 11:45:39.934756 evidently-0.2.8/src/evidently/metrics/classification_performance/probability_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7321 2023-03-22 11:45:39.935396 evidently-0.2.8/src/evidently/metrics/classification_performance/quality_by_class_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16891 2023-03-29 20:31:40.151693 evidently-0.2.8/src/evidently/metrics/classification_performance/quality_by_feature_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4425 2023-03-22 11:45:39.935836 evidently-0.2.8/src/evidently/metrics/classification_performance/roc_curve_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.500700 evidently-0.2.8/src/evidently/metrics/data_drift/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-10-05 12:35:40.104966 evidently-0.2.8/src/evidently/metrics/data_drift/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16581 2023-03-22 11:45:39.936148 evidently-0.2.8/src/evidently/metrics/data_drift/column_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6888 2023-03-22 11:45:39.936335 evidently-0.2.8/src/evidently/metrics/data_drift/column_value_plot.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12269 2023-03-22 11:45:39.936471 evidently-0.2.8/src/evidently/metrics/data_drift/data_drift_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4682 2023-03-22 11:45:39.936640 evidently-0.2.8/src/evidently/metrics/data_drift/dataset_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13290 2023-03-29 20:31:40.152337 evidently-0.2.8/src/evidently/metrics/data_drift/target_by_features_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10000 2023-03-22 11:45:39.937034 evidently-0.2.8/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11228 2023-03-22 11:45:39.937190 evidently-0.2.8/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.501734 evidently-0.2.8/src/evidently/metrics/data_integrity/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-10-05 12:35:40.105318 evidently-0.2.8/src/evidently/metrics/data_integrity/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8402 2023-03-22 11:45:39.937340 evidently-0.2.8/src/evidently/metrics/data_integrity/column_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7199 2023-03-22 11:45:39.937461 evidently-0.2.8/src/evidently/metrics/data_integrity/column_regexp_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    30445 2023-03-22 11:45:39.937733 evidently-0.2.8/src/evidently/metrics/data_integrity/column_summary_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12513 2023-03-22 11:45:39.937872 evidently-0.2.8/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8846 2023-03-22 11:45:39.938000 evidently-0.2.8/src/evidently/metrics/data_integrity/dataset_summary_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.503787 evidently-0.2.8/src/evidently/metrics/data_quality/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-10-21 23:32:00.070218 evidently-0.2.8/src/evidently/metrics/data_quality/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5359 2023-03-22 11:45:39.938138 evidently-0.2.8/src/evidently/metrics/data_quality/column_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3077 2023-03-22 11:45:39.938297 evidently-0.2.8/src/evidently/metrics/data_quality/column_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5946 2023-03-22 11:45:39.938411 evidently-0.2.8/src/evidently/metrics/data_quality/column_quantile_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6929 2023-03-22 11:45:39.938529 evidently-0.2.8/src/evidently/metrics/data_quality/column_value_list_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9392 2023-03-22 11:45:39.938653 evidently-0.2.8/src/evidently/metrics/data_quality/column_value_range_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4393 2023-03-22 11:45:39.938797 evidently-0.2.8/src/evidently/metrics/data_quality/conflict_prediction_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-03-22 11:45:39.938915 evidently-0.2.8/src/evidently/metrics/data_quality/conflict_target_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13989 2023-03-22 11:45:39.939045 evidently-0.2.8/src/evidently/metrics/data_quality/dataset_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2657 2023-03-22 11:45:39.939163 evidently-0.2.8/src/evidently/metrics/data_quality/stability_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7109 2023-03-22 11:45:39.939309 evidently-0.2.8/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5215 2023-03-22 11:45:39.939431 evidently-0.2.8/src/evidently/metrics/data_quality/text_descriptors_distribution.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.506345 evidently-0.2.8/src/evidently/metrics/regression_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-10-21 23:32:00.071803 evidently-0.2.8/src/evidently/metrics/regression_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4488 2023-03-22 11:45:39.939562 evidently-0.2.8/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)    28709 2023-03-29 20:31:40.153016 evidently-0.2.8/src/evidently/metrics/regression_performance/error_bias_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3936 2023-03-22 11:45:39.939889 evidently-0.2.8/src/evidently/metrics/regression_performance/error_distribution.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4145 2023-03-22 11:45:39.939993 evidently-0.2.8/src/evidently/metrics/regression_performance/error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6061 2023-03-22 11:45:39.940117 evidently-0.2.8/src/evidently/metrics/regression_performance/error_normality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1700 2023-03-22 11:45:39.940184 evidently-0.2.8/src/evidently/metrics/regression_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4214 2023-03-22 11:45:39.940304 evidently-0.2.8/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3821 2023-03-22 11:45:39.940414 evidently-0.2.8/src/evidently/metrics/regression_performance/predicted_vs_actual.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8427 2023-03-22 11:45:39.940543 evidently-0.2.8/src/evidently/metrics/regression_performance/regression_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12880 2023-03-22 11:45:39.940706 evidently-0.2.8/src/evidently/metrics/regression_performance/regression_performance_metrics.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12845 2023-03-22 11:45:39.940887 evidently-0.2.8/src/evidently/metrics/regression_performance/regression_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9113 2023-03-22 11:45:39.941008 evidently-0.2.8/src/evidently/metrics/regression_performance/top_error.py
--rw-r--r--   0 emelidral   (501) staff       (20)      628 2023-03-22 11:45:39.941080 evidently-0.2.8/src/evidently/metrics/regression_performance/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4594 2023-03-22 11:45:39.941151 evidently-0.2.8/src/evidently/metrics/regression_performance/visualization.py
--rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-03-22 11:45:39.941308 evidently-0.2.8/src/evidently/metrics/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.506859 evidently-0.2.8/src/evidently/model/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-01-24 12:25:45.654672 evidently-0.2.8/src/evidently/model/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-01-26 16:57:34.934661 evidently-0.2.8/src/evidently/model/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-01-26 16:57:34.934804 evidently-0.2.8/src/evidently/model/widget.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.507237 evidently-0.2.8/src/evidently/model_monitoring/
--rw-r--r--   0 emelidral   (501) staff       (20)      600 2022-11-16 10:53:30.698840 evidently-0.2.8/src/evidently/model_monitoring/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2360 2022-10-11 19:17:04.458303 evidently-0.2.8/src/evidently/model_monitoring/monitoring.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.508697 evidently-0.2.8/src/evidently/model_monitoring/monitors/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-01-24 12:25:45.654934 evidently-0.2.8/src/evidently/model_monitoring/monitors/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1710 2022-10-11 19:17:04.475265 evidently-0.2.8/src/evidently/model_monitoring/monitors/cat_target_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6825 2023-03-22 11:45:39.941447 evidently-0.2.8/src/evidently/model_monitoring/monitors/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1942 2022-10-11 19:17:04.468223 evidently-0.2.8/src/evidently/model_monitoring/monitors/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2255 2022-10-11 19:17:04.480766 evidently-0.2.8/src/evidently/model_monitoring/monitors/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3080 2023-03-22 11:45:39.941556 evidently-0.2.8/src/evidently/model_monitoring/monitors/num_target_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6978 2023-03-22 11:45:39.941650 evidently-0.2.8/src/evidently/model_monitoring/monitors/prob_classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5558 2022-10-11 19:17:04.527669 evidently-0.2.8/src/evidently/model_monitoring/monitors/regression_performance.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.509052 evidently-0.2.8/src/evidently/model_profile/
--rw-r--r--   0 emelidral   (501) staff       (20)      160 2022-11-16 10:53:30.699070 evidently-0.2.8/src/evidently/model_profile/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1557 2022-10-11 19:17:04.527254 evidently-0.2.8/src/evidently/model_profile/model_profile.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.510664 evidently-0.2.8/src/evidently/model_profile/sections/
--rw-r--r--   0 emelidral   (501) staff       (20)      628 2022-10-11 19:17:04.490716 evidently-0.2.8/src/evidently/model_profile/sections/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      992 2022-09-05 08:44:13.940638 evidently-0.2.8/src/evidently/model_profile/sections/base_profile_section.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1786 2023-03-22 11:45:39.941818 evidently-0.2.8/src/evidently/model_profile/sections/cat_target_drift_profile_section.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1959 2023-03-22 11:45:39.941921 evidently-0.2.8/src/evidently/model_profile/sections/classification_performance_profile_section.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2532 2023-03-22 11:45:39.942025 evidently-0.2.8/src/evidently/model_profile/sections/data_drift_profile_section.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2678 2023-03-22 11:45:39.942131 evidently-0.2.8/src/evidently/model_profile/sections/data_quality_profile_section.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1969 2023-03-22 11:45:39.942235 evidently-0.2.8/src/evidently/model_profile/sections/num_target_drift_profile_section.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2483 2023-03-22 11:45:39.942338 evidently-0.2.8/src/evidently/model_profile/sections/prob_classification_performance_profile_section.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2171 2023-03-22 11:45:39.942433 evidently-0.2.8/src/evidently/model_profile/sections/regression_performance_profile_section.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.510851 evidently-0.2.8/src/evidently/nbextension/
--rw-r--r--   0 emelidral   (501) staff       (20)      268 2022-10-11 19:17:04.544608 evidently-0.2.8/src/evidently/nbextension/__init__.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.511791 evidently-0.2.8/src/evidently/nbextension/static/
--rw-r--r--   0 emelidral   (501) staff       (20)      409 2022-04-11 19:01:19.562560 evidently-0.2.8/src/evidently/nbextension/static/extension.js
--rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-02-03 13:11:36.708110 evidently-0.2.8/src/evidently/nbextension/static/index.js
--rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-02-03 13:11:36.709545 evidently-0.2.8/src/evidently/nbextension/static/index.js.LICENSE.txt
--rw-r--r--   0 emelidral   (501) staff       (20) 19811245 2022-01-27 17:11:31.945741 evidently-0.2.8/src/evidently/nbextension/static/index.js.map
--rw-r--r--   0 emelidral   (501) staff       (20)    94648 2022-04-11 19:01:19.575769 evidently-0.2.8/src/evidently/nbextension/static/material-ui-icons.woff2
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.512546 evidently-0.2.8/src/evidently/options/
--rw-r--r--   0 emelidral   (501) staff       (20)      783 2022-10-03 16:45:53.883530 evidently-0.2.8/src/evidently/options/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3349 2023-01-26 16:57:34.935105 evidently-0.2.8/src/evidently/options/color_scheme.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8204 2023-01-26 16:57:34.935255 evidently-0.2.8/src/evidently/options/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-01-26 16:57:34.935629 evidently-0.2.8/src/evidently/options/quality_metrics.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.513376 evidently-0.2.8/src/evidently/pipeline/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-01-24 12:25:45.656008 evidently-0.2.8/src/evidently/pipeline/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1087 2023-03-22 11:45:39.942549 evidently-0.2.8/src/evidently/pipeline/column_mapping.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2256 2022-10-11 19:17:04.572907 evidently-0.2.8/src/evidently/pipeline/pipeline.py
--rw-r--r--   0 emelidral   (501) staff       (20)      905 2022-09-27 21:22:08.017066 evidently-0.2.8/src/evidently/pipeline/stage.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.513576 evidently-0.2.8/src/evidently/profile_sections/
--rw-r--r--   0 emelidral   (501) staff       (20)      295 2022-10-11 19:17:04.555142 evidently-0.2.8/src/evidently/profile_sections/__init__.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.514537 evidently-0.2.8/src/evidently/renderers/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-07-06 23:19:26.758582 evidently-0.2.8/src/evidently/renderers/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2780 2023-03-22 11:45:39.942696 evidently-0.2.8/src/evidently/renderers/base_renderer.py
--rw-r--r--   0 emelidral   (501) staff       (20)    27722 2023-03-22 11:45:39.942856 evidently-0.2.8/src/evidently/renderers/html_widgets.py
--rw-r--r--   0 emelidral   (501) staff       (20)      733 2022-11-22 14:22:49.518378 evidently-0.2.8/src/evidently/renderers/notebook_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-03-22 11:45:39.942972 evidently-0.2.8/src/evidently/renderers/render_utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.514889 evidently-0.2.8/src/evidently/report/
--rw-r--r--   0 emelidral   (501) staff       (20)       27 2022-09-05 08:44:13.944194 evidently-0.2.8/src/evidently/report/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6741 2023-03-22 11:45:39.943093 evidently-0.2.8/src/evidently/report/report.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.515761 evidently-0.2.8/src/evidently/runner/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-01-24 12:25:45.656210 evidently-0.2.8/src/evidently/runner/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2216 2023-01-26 16:57:34.936548 evidently-0.2.8/src/evidently/runner/dashboard_runner.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-01-26 16:57:34.936720 evidently-0.2.8/src/evidently/runner/loader.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2647 2023-01-26 16:57:34.936874 evidently-0.2.8/src/evidently/runner/profile_runner.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-01-26 16:57:34.937015 evidently-0.2.8/src/evidently/runner/runner.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.516260 evidently-0.2.8/src/evidently/suite/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2022-07-06 23:19:26.758822 evidently-0.2.8/src/evidently/suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12539 2023-03-22 11:45:39.943270 evidently-0.2.8/src/evidently/suite/base_suite.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-01-26 16:57:34.937343 evidently-0.2.8/src/evidently/suite/execution_graph.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.516430 evidently-0.2.8/src/evidently/tabs/
--rw-r--r--   0 emelidral   (501) staff       (20)      251 2022-10-11 19:17:04.604503 evidently-0.2.8/src/evidently/tabs/__init__.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.516764 evidently-0.2.8/src/evidently/telemetry/
--rw-r--r--   0 emelidral   (501) staff       (20)       36 2022-01-24 12:25:45.656546 evidently-0.2.8/src/evidently/telemetry/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1007 2022-09-05 08:44:13.950795 evidently-0.2.8/src/evidently/telemetry/sender.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.518406 evidently-0.2.8/src/evidently/test_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      859 2022-11-23 07:36:22.499291 evidently-0.2.8/src/evidently/test_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-03-22 11:45:39.943395 evidently-0.2.8/src/evidently/test_preset/classification_binary.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-03-22 11:45:39.943506 evidently-0.2.8/src/evidently/test_preset/classification_binary_topk.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-03-22 14:23:20.688438 evidently-0.2.8/src/evidently/test_preset/classification_multiclass.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6024 2023-03-22 11:45:39.943738 evidently-0.2.8/src/evidently/test_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-03-22 11:45:39.943842 evidently-0.2.8/src/evidently/test_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-03-22 11:45:39.943954 evidently-0.2.8/src/evidently/test_preset/data_stability.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5483 2023-03-22 11:45:39.944079 evidently-0.2.8/src/evidently/test_preset/no_target_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-03-22 11:45:39.944208 evidently-0.2.8/src/evidently/test_preset/regression.py
--rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-03-22 11:45:39.944310 evidently-0.2.8/src/evidently/test_preset/test_preset.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.518744 evidently-0.2.8/src/evidently/test_suite/
--rw-r--r--   0 emelidral   (501) staff       (20)       34 2022-07-06 23:19:26.759379 evidently-0.2.8/src/evidently/test_suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6938 2023-03-22 11:45:39.944456 evidently-0.2.8/src/evidently/test_suite/test_suite.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.520093 evidently-0.2.8/src/evidently/tests/
--rw-r--r--   0 emelidral   (501) staff       (20)     4410 2022-11-23 07:36:22.503518 evidently-0.2.8/src/evidently/tests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9384 2023-03-22 11:45:39.944572 evidently-0.2.8/src/evidently/tests/base_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)    27793 2023-03-22 11:45:39.944825 evidently-0.2.8/src/evidently/tests/classification_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    20108 2023-03-22 11:45:39.944978 evidently-0.2.8/src/evidently/tests/data_drift_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    47961 2023-03-22 11:45:39.945193 evidently-0.2.8/src/evidently/tests/data_integrity_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    61141 2023-03-22 11:45:39.945330 evidently-0.2.8/src/evidently/tests/data_quality_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    14045 2023-03-22 11:45:39.945475 evidently-0.2.8/src/evidently/tests/regression_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16360 2023-03-22 11:45:39.945608 evidently-0.2.8/src/evidently/tests/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.521530 evidently-0.2.8/src/evidently/utils/
--rw-r--r--   0 emelidral   (501) staff       (20)       40 2022-05-17 08:06:32.941958 evidently-0.2.8/src/evidently/utils/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-01-26 16:57:34.940229 evidently-0.2.8/src/evidently/utils/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8342 2023-03-03 10:18:49.593541 evidently-0.2.8/src/evidently/utils/data_drift_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8044 2023-03-22 11:45:39.945741 evidently-0.2.8/src/evidently/utils/data_operations.py
--rw-r--r--   0 emelidral   (501) staff       (20)    17061 2023-03-22 11:45:39.945901 evidently-0.2.8/src/evidently/utils/data_preprocessing.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-03-22 11:45:39.946033 evidently-0.2.8/src/evidently/utils/generators.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1465 2022-10-11 19:17:04.788874 evidently-0.2.8/src/evidently/utils/numpy_encoder.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2213 2022-10-21 23:32:00.078011 evidently-0.2.8/src/evidently/utils/types.py
--rw-r--r--   0 emelidral   (501) staff       (20)    23874 2023-03-22 11:45:39.946188 evidently-0.2.8/src/evidently/utils/visualizations.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-03-29 22:02:09.521706 evidently-0.2.8/src/evidently/widgets/
--rw-r--r--   0 emelidral   (501) staff       (20)      266 2022-10-11 19:17:04.790710 evidently-0.2.8/src/evidently/widgets/__init__.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.321893 evidently-0.3.0/
+-rw-r--r--   0 emelidral   (501) staff       (20)      373 2023-04-12 10:10:18.322016 evidently-0.3.0/PKG-INFO
+-rw-r--r--   0 emelidral   (501) staff       (20)     1447 2023-04-11 11:50:44.033151 evidently-0.3.0/setup.cfg
+-rw-r--r--   0 emelidral   (501) staff       (20)     2068 2023-04-11 11:50:44.033217 evidently-0.3.0/setup.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-04-11 11:50:44.033364 evidently-0.3.0/setupbase.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.289234 evidently-0.3.0/src/
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.292634 evidently-0.3.0/src/evidently/
+-rw-r--r--   0 emelidral   (501) staff       (20)      256 2023-04-11 11:50:44.033482 evidently-0.3.0/src/evidently/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2680 2023-04-11 17:10:42.502107 evidently-0.3.0/src/evidently/__main__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      162 2023-04-11 11:50:44.033618 evidently-0.3.0/src/evidently/_config.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      111 2023-04-12 10:07:31.233524 evidently-0.3.0/src/evidently/_version.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6886 2023-04-11 22:08:01.497073 evidently-0.3.0/src/evidently/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.294020 evidently-0.3.0/src/evidently/calculations/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.034605 evidently-0.3.0/src/evidently/calculations/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-04-11 11:50:44.034697 evidently-0.3.0/src/evidently/calculations/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16012 2023-04-11 11:50:44.034784 evidently-0.3.0/src/evidently/calculations/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2662 2023-04-11 11:50:44.034844 evidently-0.3.0/src/evidently/calculations/data_integration.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    31464 2023-04-11 11:50:44.034969 evidently-0.3.0/src/evidently/calculations/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-04-11 11:50:44.035061 evidently-0.3.0/src/evidently/calculations/regression_performance.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.298034 evidently-0.3.0/src/evidently/calculations/stattests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1184 2023-04-11 11:50:44.035148 evidently-0.3.0/src/evidently/calculations/stattests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1337 2023-04-11 11:50:44.035216 evidently-0.3.0/src/evidently/calculations/stattests/anderson_darling_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1741 2023-04-11 11:50:44.035280 evidently-0.3.0/src/evidently/calculations/stattests/chisquare_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5352 2023-04-11 11:50:44.035359 evidently-0.3.0/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1533 2023-04-11 11:50:44.035446 evidently-0.3.0/src/evidently/calculations/stattests/energy_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2108 2023-04-11 11:50:44.035531 evidently-0.3.0/src/evidently/calculations/stattests/epps_singleton_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2592 2023-04-11 11:50:44.035581 evidently-0.3.0/src/evidently/calculations/stattests/fisher_exact_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-04-11 11:50:44.035635 evidently-0.3.0/src/evidently/calculations/stattests/g_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2983 2023-04-11 11:50:44.035704 evidently-0.3.0/src/evidently/calculations/stattests/hellinger_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-04-11 11:50:44.035768 evidently-0.3.0/src/evidently/calculations/stattests/jensenshannon.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1899 2023-04-11 11:50:44.035819 evidently-0.3.0/src/evidently/calculations/stattests/kl_div.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1545 2023-04-11 11:50:44.035878 evidently-0.3.0/src/evidently/calculations/stattests/ks_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1732 2023-04-11 11:50:44.035946 evidently-0.3.0/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4683 2023-04-11 11:50:44.036014 evidently-0.3.0/src/evidently/calculations/stattests/mmd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-04-11 11:50:44.036061 evidently-0.3.0/src/evidently/calculations/stattests/psi.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4586 2023-04-11 11:50:44.036122 evidently-0.3.0/src/evidently/calculations/stattests/registry.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1490 2023-04-11 11:50:44.036213 evidently-0.3.0/src/evidently/calculations/stattests/t_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      743 2023-04-11 11:50:44.036270 evidently-0.3.0/src/evidently/calculations/stattests/text_content_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2746 2023-04-11 11:50:44.036327 evidently-0.3.0/src/evidently/calculations/stattests/tvd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-04-11 11:50:44.036404 evidently-0.3.0/src/evidently/calculations/stattests/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1832 2023-04-11 11:50:44.036454 evidently-0.3.0/src/evidently/calculations/stattests/wasserstein_distance_norm.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-04-11 11:50:44.036512 evidently-0.3.0/src/evidently/calculations/stattests/z_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.036630 evidently-0.3.0/src/evidently/calculations/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7042 2023-04-11 22:08:01.497774 evidently-0.3.0/src/evidently/core.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.298911 evidently-0.3.0/src/evidently/descriptors/
+-rw-r--r--   0 emelidral   (501) staff       (20)      249 2023-04-11 11:50:44.040731 evidently-0.3.0/src/evidently/descriptors/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-04-11 11:50:44.040789 evidently-0.3.0/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      582 2023-04-11 11:50:44.040840 evidently-0.3.0/src/evidently/descriptors/oov_words_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-04-11 11:50:44.040888 evidently-0.3.0/src/evidently/descriptors/text_length_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      776 2023-04-11 11:50:44.040933 evidently-0.3.0/src/evidently/descriptors/trigger_words_presence_descriptor.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.299951 evidently-0.3.0/src/evidently/features/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1682 2023-04-11 11:50:44.041013 evidently-0.3.0/src/evidently/features/OOV_words_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.041037 evidently-0.3.0/src/evidently/features/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1894 2023-04-11 11:50:44.041102 evidently-0.3.0/src/evidently/features/generated_features.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1095 2023-04-11 11:50:44.041157 evidently-0.3.0/src/evidently/features/non_letter_character_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      966 2023-04-11 11:50:44.041206 evidently-0.3.0/src/evidently/features/text_length_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2121 2023-04-11 11:50:44.041271 evidently-0.3.0/src/evidently/features/trigger_words_presence_feature.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.301404 evidently-0.3.0/src/evidently/metric_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-04-11 11:50:44.041350 evidently-0.3.0/src/evidently/metric_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-04-11 11:50:44.041407 evidently-0.3.0/src/evidently/metric_preset/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3973 2023-04-11 11:50:44.041471 evidently-0.3.0/src/evidently/metric_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-04-11 11:50:44.041535 evidently-0.3.0/src/evidently/metric_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-04-11 11:50:44.041591 evidently-0.3.0/src/evidently/metric_preset/metric_preset.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-04-11 11:50:44.041650 evidently-0.3.0/src/evidently/metric_preset/regression_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-04-11 11:50:44.041719 evidently-0.3.0/src/evidently/metric_preset/target_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-04-11 11:50:44.041776 evidently-0.3.0/src/evidently/metric_preset/text_overview.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7679 2023-04-11 22:08:01.498430 evidently-0.3.0/src/evidently/metric_results.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.301934 evidently-0.3.0/src/evidently/metrics/
+-rw-r--r--   0 emelidral   (501) staff       (20)     3737 2023-04-11 11:50:44.041950 evidently-0.3.0/src/evidently/metrics/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-04-11 11:50:44.042032 evidently-0.3.0/src/evidently/metrics/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.304405 evidently-0.3.0/src/evidently/metrics/classification_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.042092 evidently-0.3.0/src/evidently/metrics/classification_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2994 2023-04-11 11:50:44.042167 evidently-0.3.0/src/evidently/metrics/classification_performance/base_classification_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2890 2023-04-11 11:50:44.042230 evidently-0.3.0/src/evidently/metrics/classification_performance/class_balance_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4298 2023-04-11 11:50:44.042357 evidently-0.3.0/src/evidently/metrics/classification_performance/class_separation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11993 2023-04-11 11:50:44.042435 evidently-0.3.0/src/evidently/metrics/classification_performance/classification_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5193 2023-04-11 11:50:44.042500 evidently-0.3.0/src/evidently/metrics/classification_performance/classification_quality_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3312 2023-04-11 11:50:44.042564 evidently-0.3.0/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1534 2023-04-11 11:50:44.042621 evidently-0.3.0/src/evidently/metrics/classification_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4483 2023-04-11 11:50:44.042685 evidently-0.3.0/src/evidently/metrics/classification_performance/pr_curve_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6020 2023-04-11 11:50:44.042749 evidently-0.3.0/src/evidently/metrics/classification_performance/pr_table_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5959 2023-04-11 11:50:44.042828 evidently-0.3.0/src/evidently/metrics/classification_performance/probability_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7318 2023-04-11 11:50:44.042904 evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_class_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16900 2023-04-11 22:08:01.499197 evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_feature_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4425 2023-04-11 11:50:44.043054 evidently-0.3.0/src/evidently/metrics/classification_performance/roc_curve_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.306211 evidently-0.3.0/src/evidently/metrics/data_drift/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043120 evidently-0.3.0/src/evidently/metrics/data_drift/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16581 2023-04-11 11:50:44.043222 evidently-0.3.0/src/evidently/metrics/data_drift/column_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6963 2023-04-11 11:50:44.043309 evidently-0.3.0/src/evidently/metrics/data_drift/column_value_plot.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12269 2023-04-11 11:50:44.043396 evidently-0.3.0/src/evidently/metrics/data_drift/data_drift_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4682 2023-04-11 11:50:44.043500 evidently-0.3.0/src/evidently/metrics/data_drift/dataset_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10630 2023-04-11 11:50:44.043573 evidently-0.3.0/src/evidently/metrics/data_drift/embedding_drift_methods.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4469 2023-04-11 11:50:44.043645 evidently-0.3.0/src/evidently/metrics/data_drift/embeddings_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13290 2023-04-11 11:50:44.043698 evidently-0.3.0/src/evidently/metrics/data_drift/target_by_features_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10000 2023-04-11 11:50:44.043757 evidently-0.3.0/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11173 2023-04-11 11:50:44.043845 evidently-0.3.0/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.307315 evidently-0.3.0/src/evidently/metrics/data_integrity/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043904 evidently-0.3.0/src/evidently/metrics/data_integrity/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8345 2023-04-11 11:50:44.043991 evidently-0.3.0/src/evidently/metrics/data_integrity/column_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7142 2023-04-11 11:50:44.044068 evidently-0.3.0/src/evidently/metrics/data_integrity/column_regexp_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    30453 2023-04-11 11:50:44.044199 evidently-0.3.0/src/evidently/metrics/data_integrity/column_summary_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12456 2023-04-11 11:50:44.044306 evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8789 2023-04-11 11:50:44.044393 evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_summary_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.309456 evidently-0.3.0/src/evidently/metrics/data_quality/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.044472 evidently-0.3.0/src/evidently/metrics/data_quality/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5821 2023-04-11 11:50:44.044563 evidently-0.3.0/src/evidently/metrics/data_quality/column_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3054 2023-04-11 11:50:44.044629 evidently-0.3.0/src/evidently/metrics/data_quality/column_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5936 2023-04-11 11:50:44.044695 evidently-0.3.0/src/evidently/metrics/data_quality/column_quantile_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6872 2023-04-11 11:50:44.044766 evidently-0.3.0/src/evidently/metrics/data_quality/column_value_list_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8991 2023-04-11 11:50:44.044848 evidently-0.3.0/src/evidently/metrics/data_quality/column_value_range_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4336 2023-04-11 11:50:44.044913 evidently-0.3.0/src/evidently/metrics/data_quality/conflict_prediction_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-04-11 11:50:44.044975 evidently-0.3.0/src/evidently/metrics/data_quality/conflict_target_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13927 2023-04-11 11:50:44.045061 evidently-0.3.0/src/evidently/metrics/data_quality/dataset_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2657 2023-04-11 11:50:44.045118 evidently-0.3.0/src/evidently/metrics/data_quality/stability_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7248 2023-04-11 11:50:44.045194 evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5215 2023-04-11 11:50:44.045257 evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_distribution.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.312060 evidently-0.3.0/src/evidently/metrics/regression_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.045310 evidently-0.3.0/src/evidently/metrics/regression_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4488 2023-04-11 11:50:44.045377 evidently-0.3.0/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    28709 2023-04-11 11:50:44.045473 evidently-0.3.0/src/evidently/metrics/regression_performance/error_bias_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3936 2023-04-11 11:50:44.045565 evidently-0.3.0/src/evidently/metrics/regression_performance/error_distribution.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4145 2023-04-11 11:50:44.045610 evidently-0.3.0/src/evidently/metrics/regression_performance/error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6061 2023-04-11 11:50:44.045672 evidently-0.3.0/src/evidently/metrics/regression_performance/error_normality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1675 2023-04-11 11:50:44.045735 evidently-0.3.0/src/evidently/metrics/regression_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4214 2023-04-11 11:50:44.045783 evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3896 2023-04-11 11:50:44.045845 evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_vs_actual.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8427 2023-04-11 11:50:44.045914 evidently-0.3.0/src/evidently/metrics/regression_performance/regression_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12823 2023-04-11 11:50:44.045990 evidently-0.3.0/src/evidently/metrics/regression_performance/regression_performance_metrics.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12845 2023-04-11 11:50:44.046056 evidently-0.3.0/src/evidently/metrics/regression_performance/regression_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9131 2023-04-11 11:50:44.046126 evidently-0.3.0/src/evidently/metrics/regression_performance/top_error.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      628 2023-04-11 11:50:44.046174 evidently-0.3.0/src/evidently/metrics/regression_performance/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4630 2023-04-11 11:50:44.046235 evidently-0.3.0/src/evidently/metrics/regression_performance/visualization.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-04-11 11:50:44.046284 evidently-0.3.0/src/evidently/metrics/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.312534 evidently-0.3.0/src/evidently/model/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.046336 evidently-0.3.0/src/evidently/model/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-04-11 11:50:44.046390 evidently-0.3.0/src/evidently/model/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.046446 evidently-0.3.0/src/evidently/model/widget.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.312706 evidently-0.3.0/src/evidently/nbextension/
+-rw-r--r--   0 emelidral   (501) staff       (20)      195 2023-04-11 11:50:44.047775 evidently-0.3.0/src/evidently/nbextension/__init__.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.313401 evidently-0.3.0/src/evidently/nbextension/static/
+-rw-r--r--   0 emelidral   (501) staff       (20)      409 2023-04-11 11:50:44.047847 evidently-0.3.0/src/evidently/nbextension/static/extension.js
+-rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-04-11 11:50:44.055472 evidently-0.3.0/src/evidently/nbextension/static/index.js
+-rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-04-11 11:50:44.055652 evidently-0.3.0/src/evidently/nbextension/static/index.js.LICENSE.txt
+-rw-r--r--   0 emelidral   (501) staff       (20)    94648 2023-04-11 11:50:44.056026 evidently-0.3.0/src/evidently/nbextension/static/material-ui-icons.woff2
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.314070 evidently-0.3.0/src/evidently/options/
+-rw-r--r--   0 emelidral   (501) staff       (20)      783 2023-04-11 11:50:44.056118 evidently-0.3.0/src/evidently/options/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3349 2023-04-11 11:50:44.056178 evidently-0.3.0/src/evidently/options/color_scheme.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8204 2023-04-11 11:50:44.056254 evidently-0.3.0/src/evidently/options/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-04-11 11:50:44.056307 evidently-0.3.0/src/evidently/options/quality_metrics.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.314409 evidently-0.3.0/src/evidently/pipeline/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056358 evidently-0.3.0/src/evidently/pipeline/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1165 2023-04-11 11:50:44.056415 evidently-0.3.0/src/evidently/pipeline/column_mapping.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.315235 evidently-0.3.0/src/evidently/renderers/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056636 evidently-0.3.0/src/evidently/renderers/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3114 2023-04-11 11:50:44.056702 evidently-0.3.0/src/evidently/renderers/base_renderer.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    27722 2023-04-11 11:50:44.056806 evidently-0.3.0/src/evidently/renderers/html_widgets.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      733 2023-04-11 11:50:44.056873 evidently-0.3.0/src/evidently/renderers/notebook_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-04-11 11:50:44.056927 evidently-0.3.0/src/evidently/renderers/render_utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.315561 evidently-0.3.0/src/evidently/report/
+-rw-r--r--   0 emelidral   (501) staff       (20)       27 2023-04-11 11:50:44.057001 evidently-0.3.0/src/evidently/report/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7338 2023-04-11 11:50:44.057070 evidently-0.3.0/src/evidently/report/report.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.316049 evidently-0.3.0/src/evidently/runner/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057130 evidently-0.3.0/src/evidently/runner/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-04-11 11:50:44.057260 evidently-0.3.0/src/evidently/runner/loader.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-04-11 11:50:44.057381 evidently-0.3.0/src/evidently/runner/runner.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.316550 evidently-0.3.0/src/evidently/suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057438 evidently-0.3.0/src/evidently/suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13761 2023-04-11 11:50:44.057526 evidently-0.3.0/src/evidently/suite/base_suite.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-04-11 11:50:44.057593 evidently-0.3.0/src/evidently/suite/execution_graph.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.316876 evidently-0.3.0/src/evidently/telemetry/
+-rw-r--r--   0 emelidral   (501) staff       (20)       36 2023-04-11 11:50:44.057752 evidently-0.3.0/src/evidently/telemetry/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1007 2023-04-11 11:50:44.057808 evidently-0.3.0/src/evidently/telemetry/sender.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.318562 evidently-0.3.0/src/evidently/test_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      859 2023-04-11 11:50:44.057891 evidently-0.3.0/src/evidently/test_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-04-11 11:50:44.058127 evidently-0.3.0/src/evidently/test_preset/classification_binary.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-04-11 11:50:44.058178 evidently-0.3.0/src/evidently/test_preset/classification_binary_topk.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-04-11 11:50:44.058248 evidently-0.3.0/src/evidently/test_preset/classification_multiclass.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6024 2023-04-11 11:50:44.058298 evidently-0.3.0/src/evidently/test_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.058356 evidently-0.3.0/src/evidently/test_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-04-11 11:50:44.058402 evidently-0.3.0/src/evidently/test_preset/data_stability.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5483 2023-04-11 11:50:44.058454 evidently-0.3.0/src/evidently/test_preset/no_target_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-04-11 11:50:44.058506 evidently-0.3.0/src/evidently/test_preset/regression.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-04-11 11:50:44.058559 evidently-0.3.0/src/evidently/test_preset/test_preset.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.318904 evidently-0.3.0/src/evidently/test_suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)       34 2023-04-11 11:50:44.058625 evidently-0.3.0/src/evidently/test_suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7454 2023-04-11 11:50:44.058693 evidently-0.3.0/src/evidently/test_suite/test_suite.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.320259 evidently-0.3.0/src/evidently/tests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     4410 2023-04-11 11:50:44.058785 evidently-0.3.0/src/evidently/tests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11758 2023-04-11 11:50:44.058862 evidently-0.3.0/src/evidently/tests/base_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22752 2023-04-11 11:50:44.059177 evidently-0.3.0/src/evidently/tests/classification_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    19989 2023-04-11 11:50:44.059285 evidently-0.3.0/src/evidently/tests/data_drift_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    41950 2023-04-11 11:50:44.059392 evidently-0.3.0/src/evidently/tests/data_integrity_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    53163 2023-04-11 11:50:44.059500 evidently-0.3.0/src/evidently/tests/data_quality_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10930 2023-04-11 11:50:44.059579 evidently-0.3.0/src/evidently/tests/regression_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16360 2023-04-11 11:50:44.059661 evidently-0.3.0/src/evidently/tests/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.321850 evidently-0.3.0/src/evidently/utils/
+-rw-r--r--   0 emelidral   (501) staff       (20)       40 2023-04-11 11:50:44.059731 evidently-0.3.0/src/evidently/utils/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-04-11 11:50:44.059794 evidently-0.3.0/src/evidently/utils/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8342 2023-04-11 11:50:44.059864 evidently-0.3.0/src/evidently/utils/data_drift_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8133 2023-04-11 11:50:44.059931 evidently-0.3.0/src/evidently/utils/data_operations.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    20996 2023-04-11 11:50:44.060030 evidently-0.3.0/src/evidently/utils/data_preprocessing.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-04-11 11:50:44.060100 evidently-0.3.0/src/evidently/utils/generators.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1392 2023-04-11 22:08:01.499801 evidently-0.3.0/src/evidently/utils/numpy_encoder.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.060206 evidently-0.3.0/src/evidently/utils/types.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    25482 2023-04-11 11:50:44.060302 evidently-0.3.0/src/evidently/utils/visualizations.py
```

### Comparing `evidently-0.2.8/setup.cfg` & `evidently-0.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -17,22 +17,23 @@
     =src
 
 [options.packages.find]
 where = src
 
 
 [flake8]
-ignore = E501,F401,W503,W504
+ignore = E501,F401,W503,W504,E203
 max-line-length = 140
 per-file-ignores =
      src/evidently/tabs/__init__.py: F403
      src/evidently/profile_sections/__init__.py: F403
      src/evidently/widgets/__init__.py: F403
 
 [mypy]
+show_error_codes = True
 files = src/evidently
 python_version = 3.7
 
 [mypy-nltk.*]
 ignore_missing_imports = True
 
 [mypy-pandas.*]
@@ -46,14 +47,17 @@
 
 [mypy-sklearn.*]
 ignore_missing_imports = True
 
 [mypy-plotly.*]
 ignore_missing_imports = True
 
+[mypy-umap.*]
+ignore_missing_imports = True
+
 [mypy-IPython.*]
 ignore_missing_imports = True
 
 [tool:pytest]
 testpaths=tests
 python_classes=*Test
```

### Comparing `evidently-0.2.8/setup.py` & `evidently-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     install_requires=[
         "plotly>=5.5.0",
         "statsmodels>=0.12.2",
         "scikit-learn>=0.24.0",
         "pandas>=1.3.5",
         "numpy>=1.19.5",
         "nltk>=3.6.7",
+        "umap-learn>=0.5.3",
         "scipy>=1.5.4",
         "requests>=2.19.0",
         "PyYAML>=5.1",
         "pydantic<2",
     ],
     extras_require={
         "dev": [
```

### Comparing `evidently-0.2.8/setupbase.py` & `evidently-0.3.0/setupbase.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/analyzers/cat_target_drift_analyzer.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/probability_distribution_metric.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,158 @@
-#!/usr/bin/env python
-# coding: utf-8
-from dataclasses import dataclass
+import dataclasses
+from typing import Dict
+from typing import Iterable
+from typing import List
 from typing import Optional
-from typing import Sequence
 
+import numpy as np
 import pandas as pd
+from plotly import figure_factory as ff
 
-from evidently import ColumnMapping
-from evidently.analyzers.base_analyzer import Analyzer
-from evidently.analyzers.base_analyzer import BaseAnalyzerResult
-from evidently.calculations.data_drift import ColumnDataDriftMetrics
-from evidently.calculations.data_drift import ensure_prediction_column_is_string
-from evidently.calculations.data_drift import get_one_column_drift
-from evidently.calculations.data_quality import get_rows_count
-from evidently.options import DataDriftOptions
-from evidently.options import QualityMetricsOptions
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.calculations.classification_performance import get_prediction_data
+from evidently.core import IncludeTags
+from evidently.model.widget import BaseWidgetInfo
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import GraphData
+from evidently.renderers.html_widgets import WidgetSize
+from evidently.renderers.html_widgets import plotly_graph_tabs
 from evidently.utils.data_operations import process_columns
-from evidently.utils.data_operations import replace_infinity_values_to_nan
 
 
-@dataclass
-class CatTargetDriftAnalyzerResults(BaseAnalyzerResult):
-    """Class for all results of category target drift calculations"""
+class ClassificationProbDistributionResults(MetricResult):
+    class Config:
+        dict_include = False
+        pd_include = False
+        tags = {IncludeTags.Render}
 
-    target_metrics: Optional[ColumnDataDriftMetrics] = None
-    prediction_metrics: Optional[ColumnDataDriftMetrics] = None
-    reference_data_count: int = 0
-    current_data_count: int = 0
+    current_distribution: Optional[Dict[str, list]]  # todo use DistributionField?
+    reference_distribution: Optional[Dict[str, list]]
 
 
-class CatTargetDriftAnalyzer(Analyzer):
-    """Categorical target drift analyzer.
+class ClassificationProbDistribution(Metric[ClassificationProbDistributionResults]):
+    @staticmethod
+    def get_distribution(dataset: pd.DataFrame, target_name: str, prediction_labels: Iterable) -> Dict[str, list]:
+        result = {}
+        dataset.replace([np.inf, -np.inf], np.nan, inplace=True)
+        for label in prediction_labels:
+            result[label] = [
+                dataset[dataset[target_name] == label][label],
+                dataset[dataset[target_name] != label][label],
+            ]
 
-    Analyze categorical `target` and `prediction` distributions and provide calculations to the following questions:
-    Does the model target behave similarly to the past period? Do my model predictions still look the same?
+        return result
 
-    For reference see https://evidentlyai.com/blog/evidently-014-target-and-prediction-drift
-    """
+    def calculate(self, data: InputData) -> ClassificationProbDistributionResults:
+        columns = process_columns(data.current_data, data.column_mapping)
+        prediction = columns.utility_columns.prediction
+        target = columns.utility_columns.target
+
+        if target is None:
+            raise ValueError("Target column should be present")
+
+        if prediction is None:
+            raise ValueError("Prediction column should be present")
+
+        prediction_data = get_prediction_data(data.current_data, columns, data.column_mapping.pos_label)
+        if prediction_data.prediction_probas is None:
+            current_distribution = None
+            reference_distribution = None
+
+        else:
+            current_data_copy = data.current_data.copy()
+            for col in prediction_data.prediction_probas.columns:
+                current_data_copy[col] = prediction_data.prediction_probas[col]
 
-    @staticmethod
-    def get_results(analyzer_results) -> CatTargetDriftAnalyzerResults:
-        return analyzer_results[CatTargetDriftAnalyzer]
+            current_distribution = self.get_distribution(
+                current_data_copy, target, prediction_data.prediction_probas.columns
+            )
 
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-    ) -> CatTargetDriftAnalyzerResults:
-        """Calculate the target and prediction drifts.
-
-        With default options, uses a chi² test when number of labels is greater than 2.
-        Otherwise, uses a z-test.
-
-        Notes:
-            Be aware that any nan or infinity values will be dropped from the dataframes in place.
-
-            You can also provide a custom function that computes a statistic by adding special
-            `DataDriftOptions` object to the `option_provider` of the class.::
-
-                options = DataDriftOptions(cat_target_stattest_func=...)
-                analyzer.options_prover.add(options)
-
-            Such a function takes two arguments:::
-
-                def(reference_data: pd.Series, current_data: pd.Series):
-                   ...
-
-            and returns arbitrary number (like a p_value from the other tests ;-))
-        Args:
-            reference_data: usually the data which you used in training.
-            current_data: new, unseen data to which we compare the reference data.
-            column_mapping: a `ColumnMapping` object that contains references to the name of target and prediction
-                columns
-        Returns:
-            A dictionary that contains some meta information as well as `metrics` for either target or prediction
-            columns or both. The `*_drift` column in `metrics` contains a computed p_value from tests.
-        """
-        if reference_data is None:
-            raise ValueError("reference_data should be present")
-
-        if current_data is None:
-            raise ValueError("current_data should be present")
-
-        data_drift_options = self.options_provider.get(DataDriftOptions)
-        columns = process_columns(reference_data, column_mapping)
-        target_column = columns.utility_columns.target
-
-        if not isinstance(target_column, str) and isinstance(target_column, Sequence):
-            raise ValueError("target should not be a sequence")
-
-        classification_threshold = self.options_provider.get(QualityMetricsOptions).classification_threshold
-        prediction_column = ensure_prediction_column_is_string(
-            prediction_column=columns.utility_columns.prediction,
-            current_data=current_data,
-            reference_data=reference_data,
-            threshold=classification_threshold,
+            if data.reference_data is not None:
+                reference_data_copy = data.reference_data.copy()
+                for col in prediction_data.prediction_probas.columns:
+                    reference_data_copy[col] = prediction_data.prediction_probas[col]
+                reference_distribution = self.get_distribution(
+                    reference_data_copy, target, prediction_data.prediction_probas.columns
+                )
+
+            else:
+                reference_distribution = None
+
+        return ClassificationProbDistributionResults(
+            current_distribution=current_distribution,
+            reference_distribution=reference_distribution,
         )
 
-        result = CatTargetDriftAnalyzerResults(
-            columns=columns,
-            reference_data_count=get_rows_count(reference_data),
-            current_data_count=get_rows_count(current_data),
-        )
 
-        # consider replacing only values in target and prediction column
-        reference_data = replace_infinity_values_to_nan(reference_data)
-        current_data = replace_infinity_values_to_nan(current_data)
-
-        if target_column is not None:
-            result.target_metrics = get_one_column_drift(
-                current_data=current_data,
-                reference_data=reference_data,
-                column_name=target_column,
-                dataset_columns=columns,
-                options=data_drift_options,
-                column_type="cat",
-            )
-
-        if prediction_column is not None:
-            result.prediction_metrics = get_one_column_drift(
-                current_data=current_data,
-                reference_data=reference_data,
-                column_name=prediction_column,
-                dataset_columns=columns,
-                options=data_drift_options,
-                column_type="cat",
+@default_renderer(wrap_type=ClassificationProbDistribution)
+class ClassificationProbDistributionRenderer(MetricRenderer):
+    def _plot(self, distribution: Dict[str, list]):
+        # plot distributions
+        graphs = []
+
+        for label in distribution:
+            pred_distr = ff.create_distplot(
+                distribution[label],
+                [str(label), "other"],
+                colors=[
+                    self.color_options.primary_color,
+                    self.color_options.secondary_color,
+                ],
+                bin_size=0.05,
+                show_curve=False,
+                show_rug=True,
+            )
+
+            pred_distr.update_layout(
+                xaxis_title="Probability",
+                yaxis_title="Share",
+                legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1),
+            )
+            pred_distr_json = pred_distr.to_plotly_json()
+            graphs.append(
+                {
+                    "title": str(label),
+                    "data": pred_distr_json["data"],
+                    "layout": pred_distr_json["layout"],
+                }
+            )
+        return graphs
+
+    def render_html(self, obj: ClassificationProbDistribution) -> List[BaseWidgetInfo]:
+        metric_result = obj.get_result()
+        reference_distribution = metric_result.reference_distribution
+        current_distribution = metric_result.current_distribution
+        result = []
+        size = WidgetSize.FULL
+
+        if reference_distribution is not None:
+            size = WidgetSize.HALF
+
+        if current_distribution is not None:
+            result.append(
+                plotly_graph_tabs(
+                    title="Current: Probability Distribution",
+                    size=size,
+                    figures=[
+                        GraphData(graph["title"], graph["data"], graph["layout"])
+                        for graph in self._plot(current_distribution)
+                    ],
+                )
+            )
+
+        if reference_distribution is not None:
+            result.append(
+                plotly_graph_tabs(
+                    title="Reference: Probability Distribution",
+                    size=size,
+                    figures=[
+                        GraphData(graph["title"], graph["data"], graph["layout"])
+                        for graph in self._plot(reference_distribution)
+                    ],
+                )
             )
 
         return result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `evidently-0.2.8/src/evidently/analyzers/num_target_drift_analyzer.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/class_separation_metric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,91 @@
-from dataclasses import dataclass
+from typing import List
 from typing import Optional
-from typing import Sequence
 
+import numpy as np
 import pandas as pd
 
-from evidently import ColumnMapping
-from evidently.analyzers.base_analyzer import Analyzer
-from evidently.analyzers.base_analyzer import BaseAnalyzerResult
-from evidently.calculations.data_drift import ColumnDataDriftMetrics
-from evidently.calculations.data_drift import get_one_column_drift
-from evidently.calculations.data_quality import get_rows_count
-from evidently.options import DataDriftOptions
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.calculations.classification_performance import get_prediction_data
+from evidently.metric_results import ColumnScatter
+from evidently.metric_results import column_scatter_from_df
+from evidently.metric_results import df_from_column_scatter
+from evidently.model.widget import BaseWidgetInfo
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import TabData
+from evidently.renderers.html_widgets import get_class_separation_plot_data
+from evidently.renderers.html_widgets import header_text
+from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.data_operations import process_columns
 
 
-@dataclass
-class NumTargetDriftAnalyzerResults(BaseAnalyzerResult):
-    reference_data_count: int = 0
-    current_data_count: int = 0
-    target_metrics: Optional[ColumnDataDriftMetrics] = None
-    prediction_metrics: Optional[ColumnDataDriftMetrics] = None
-
-
-class NumTargetDriftAnalyzer(Analyzer):
-    """Numerical target drift analyzer.
-
-    Analyze numerical `target` and `prediction` distributions and provide calculations to the following questions:
-    Does the model target behave similarly to the past period? Do my model predictions still look the same?
-
-    For reference see https://evidentlyai.com/blog/evidently-014-target-and-prediction-drift
-    """
-
-    @staticmethod
-    def get_results(analyzer_results) -> NumTargetDriftAnalyzerResults:
-        return analyzer_results[NumTargetDriftAnalyzer]
-
-    def calculate(
-        self, reference_data: pd.DataFrame, current_data: Optional[pd.DataFrame], column_mapping: ColumnMapping
-    ) -> NumTargetDriftAnalyzerResults:
-        """Calculate the target and prediction drifts.
-
-        With default options, uses a two sample Kolmogorov-Smirnov test at a 0.95 confidence level.
-
-        Notes:
-            You can also provide a custom function that computes a statistic by adding special
-            `DataDriftOptions` object to the `option_provider` of the class.::
-
-                options = DataDriftOptions(num_target_stattest_func=...)
-                analyzer.options_prover.add(options)
-
-            Such a function takes two arguments:::
-
-                def(reference_data: pd.Series, current_data: pd.Series):
-                   ...
-
-            and returns arbitrary number (like a p_value from the other tests ;-))
-        Args:
-            reference_data: usually the data which you used in training.
-            current_data: new, unseen data to which we compare the reference data.
-            column_mapping: a `ColumnMapping` object that contains references to the name of target and prediction
-                columns
-        Returns:
-            A dictionary that contains some meta information as well as `metrics` for either target or prediction
-            columns or both. The `*_drift` column in `metrics` contains a computed p_value from tests.
-        Raises:
-            ValueError when target or predictions columns are not numerical.
-        """
-        if reference_data is None:
-            raise ValueError("reference_data should be present")
-
-        if current_data is None:
-            raise ValueError("current_data should be present")
-
-        if current_data is None:
-            raise ValueError("current_data should be present")
-
-        columns = process_columns(reference_data, column_mapping)
-        target_column = columns.utility_columns.target
-        prediction_column = columns.utility_columns.prediction
-
-        if not isinstance(target_column, str) and isinstance(columns.utility_columns.target, Sequence):
-            raise ValueError("target should not be a sequence")
-
-        if not isinstance(prediction_column, str) and isinstance(prediction_column, Sequence):
-            raise ValueError("prediction should not be a sequence")
-
-        if set(columns.num_feature_names) - set(current_data.columns):
+class ClassificationClassSeparationPlotResults(MetricResult):
+    class Config:
+        smart_union = True
+        dict_exclude_fields = {"current", "reference"}
+        pd_exclude_fields = {"current", "reference"}
+
+    target_name: str
+    current: Optional[ColumnScatter] = None
+    reference: Optional[ColumnScatter] = None
+
+
+class ClassificationClassSeparationPlot(Metric[ClassificationClassSeparationPlotResults]):
+    def calculate(self, data: InputData) -> ClassificationClassSeparationPlotResults:
+        dataset_columns = process_columns(data.current_data, data.column_mapping)
+        target_name = dataset_columns.utility_columns.target
+        prediction_name = dataset_columns.utility_columns.prediction
+        if target_name is None or prediction_name is None:
+            raise ValueError("The columns 'target' and 'prediction' columns should be present")
+        curr_predictions = get_prediction_data(data.current_data, dataset_columns, data.column_mapping.pos_label)
+        if curr_predictions.prediction_probas is None:
             raise ValueError(
-                f"Some numerical features in current data {current_data.columns}"
-                f"are not present in columns.num_feature_names"
+                "ClassificationClassSeparationPlot can be calculated only on binary probabilistic predictions"
             )
-
-        result = NumTargetDriftAnalyzerResults(
-            columns=columns,
-            reference_data_count=get_rows_count(reference_data),
-            current_data_count=get_rows_count(current_data),
+        current_plot = curr_predictions.prediction_probas.copy()
+        current_plot[target_name] = data.current_data[target_name]
+        reference_plot = None
+        if data.reference_data is not None:
+            ref_predictions = get_prediction_data(data.reference_data, dataset_columns, data.column_mapping.pos_label)
+            if ref_predictions.prediction_probas is None:
+                raise ValueError(
+                    "ClassificationClassSeparationPlot can be calculated only on binary probabilistic predictions"
+                )
+            reference_plot = ref_predictions.prediction_probas.copy()
+            reference_plot[target_name] = data.reference_data[target_name]
+        return ClassificationClassSeparationPlotResults(
+            current=column_scatter_from_df(current_plot, True),
+            reference=column_scatter_from_df(reference_plot, True),
+            target_name=target_name,
         )
-        data_drift_options = self.options_provider.get(DataDriftOptions)
 
-        if target_column is not None:
-            result.target_metrics = get_one_column_drift(
-                current_data=current_data,
-                reference_data=reference_data,
-                column_name=target_column,
-                dataset_columns=columns,
-                options=data_drift_options,
-                column_type="num",
-            )
-
-        if prediction_column is not None:
-            result.prediction_metrics = get_one_column_drift(
-                current_data=current_data,
-                reference_data=reference_data,
-                column_name=prediction_column,
-                dataset_columns=columns,
-                options=data_drift_options,
-                column_type="num",
-            )
 
-        return result
+@default_renderer(wrap_type=ClassificationClassSeparationPlot)
+class ClassificationClassSeparationPlotRenderer(MetricRenderer):
+    def render_html(self, obj: ClassificationClassSeparationPlot) -> List[BaseWidgetInfo]:
+        current_plot = obj.get_result().current
+        reference_plot = obj.get_result().reference
+        target_name = obj.get_result().target_name
+        if current_plot is None:
+            return []
+        # todo changing data here, consider doing this in calculation
+        current_df = df_from_column_scatter(current_plot)
+        current_df.replace([np.inf, -np.inf], np.nan, inplace=True)
+        reference_df = None
+        if reference_plot is not None:
+            reference_df = df_from_column_scatter(reference_plot)
+            reference_df.replace([np.inf, -np.inf], np.nan, inplace=True)
+
+        tab_data = get_class_separation_plot_data(
+            current_df,
+            reference_df,
+            target_name,
+            color_options=self.color_options,
+        )
+        tabs = [TabData(name, widget) for name, widget in tab_data]
+        return [
+            header_text(label="Class Separation Quality"),
+            widget_tabs(title="", tabs=tabs),
+        ]
```

### Comparing `evidently-0.2.8/src/evidently/analyzers/prob_classification_performance_analyzer.py` & `evidently-0.3.0/src/evidently/calculations/classification_performance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,333 +1,372 @@
-#!/usr/bin/env python
-# coding: utf-8
-from dataclasses import dataclass
+from typing import TYPE_CHECKING
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Sequence
 from typing import Union
 
 import numpy as np
 import pandas as pd
+from numpy import dtype
+from pandas.core.dtypes.common import is_float_dtype
+from pandas.core.dtypes.common import is_integer_dtype
+from pandas.core.dtypes.common import is_object_dtype
+from pandas.core.dtypes.common import is_string_dtype
 from sklearn import metrics
 
 from evidently import ColumnMapping
-from evidently.analyzers.base_analyzer import Analyzer
-from evidently.analyzers.base_analyzer import BaseAnalyzerResult
-from evidently.calculations.classification_performance import calculate_confusion_by_classes
-from evidently.options import QualityMetricsOptions
-from evidently.utils.data_operations import process_columns
-
-
-@dataclass
-class ConfusionMatrix:
-    labels: List[str]
-    values: list
-
-
-@dataclass
-class ProbClassificationPerformanceMetrics:
-    """Class for performance metrics values"""
-
-    accuracy: float
-    precision: float
-    recall: float
-    f1: float
-    roc_auc: float
-    log_loss: float
-    metrics_matrix: dict
-    confusion_matrix: ConfusionMatrix
-    confusion_by_classes: Dict[Union[str, int], Dict[str, int]]
-    roc_aucs: Optional[list] = None
-    roc_curve: Optional[dict] = None
-    pr_curve: Optional[dict] = None
-    pr_table: Optional[Union[dict, list]] = None
-
-
-@dataclass
-class ProbClassificationPerformanceAnalyzerResults(BaseAnalyzerResult):
-    quality_metrics_options: QualityMetricsOptions
-    reference_metrics: Optional[ProbClassificationPerformanceMetrics] = None
-    current_metrics: Optional[ProbClassificationPerformanceMetrics] = None
-
-
-class ProbClassificationPerformanceAnalyzer(Analyzer):
-    @staticmethod
-    def get_results(analyzer_results) -> ProbClassificationPerformanceAnalyzerResults:
-        return analyzer_results[ProbClassificationPerformanceAnalyzer]
-
-    def calculate(
-        self, reference_data: pd.DataFrame, current_data: Optional[pd.DataFrame], column_mapping: ColumnMapping
-    ) -> ProbClassificationPerformanceAnalyzerResults:
-        if reference_data is None:
-            raise ValueError("reference_data should be present")
-
-        columns = process_columns(reference_data, column_mapping)
-        target_column = columns.utility_columns.target
-        prediction_column = columns.utility_columns.prediction
-        quality_metrics_options = self.options_provider.get(QualityMetricsOptions)
-        result = ProbClassificationPerformanceAnalyzerResults(
-            columns=columns,
-            quality_metrics_options=quality_metrics_options,
-        )
-        classification_threshold = quality_metrics_options.classification_threshold
-
-        if target_column is not None and prediction_column is not None:
-            target_and_preds = [target_column]
-            if isinstance(prediction_column, str):
-                target_and_preds += [prediction_column]
-            else:
-                target_and_preds += prediction_column
-            reference_data.replace([np.inf, -np.inf], np.nan, inplace=True)
-            reference_data.dropna(axis=0, how="any", inplace=True, subset=target_and_preds)
-            binaraized_target = (reference_data[target_column].values.reshape(-1, 1) == prediction_column).astype(int)
-            array_prediction = reference_data[prediction_column].to_numpy()
-
-            if len(prediction_column) > 2:
-                prediction_ids = np.argmax(array_prediction, axis=-1)
-                prediction_labels = [prediction_column[x] for x in prediction_ids]
+from evidently.metric_results import Boxes
+from evidently.metric_results import ConfusionMatrix
+from evidently.metric_results import DatasetClassificationQuality
+from evidently.metric_results import DatasetColumns
+from evidently.metric_results import PredictionData
+from evidently.metric_results import RatesPlotData
+
+if TYPE_CHECKING:
+    pass
+
+
+def calculate_confusion_by_classes(
+    confusion_matrix: np.ndarray, class_names: Sequence[Union[str, int]]
+) -> Dict[Union[str, int], Dict[str, int]]:
+    """Calculate metrics:
+    - TP (true positive)
+    - TN (true negative)
+    - FP (false positive)
+    - FN (false negative)
+    for each class from confusion matrix.
+
+    Returns:
+        a dict like::
+
+            {
+                "class_1_name": {
+                    "tp": 1,
+                    "tn": 5,
+                    "fp": 0,
+                    "fn": 3,
+                },
+                "class_1_name": {
+                    "tp": 1,
+                    "tn": 5,
+                    "fp": 0,
+                    "fn": 3,
+                },
+            }
+    """
+    true_positive = np.diag(confusion_matrix)
+    false_positive = confusion_matrix.sum(axis=0) - np.diag(confusion_matrix)
+    false_negative = confusion_matrix.sum(axis=1) - np.diag(confusion_matrix)
+    true_negative = confusion_matrix.sum() - (false_positive + false_negative + true_positive)
+    confusion_by_classes = {}
+
+    for idx, class_name in enumerate(class_names):
+        confusion_by_classes[class_name] = {
+            "tp": true_positive[idx],
+            "tn": true_negative[idx],
+            "fp": false_positive[idx],
+            "fn": false_negative[idx],
+        }
+
+    return confusion_by_classes
+
+
+def k_probability_threshold(prediction_probas: pd.DataFrame, k: Union[int, float]) -> float:
+    probas = prediction_probas.iloc[:, 0].sort_values(ascending=False)
+    if isinstance(k, float):
+        if k < 0.0 or k > 1.0:
+            raise ValueError(f"K should be in range [0.0, 1.0] but was {k}")
+        return probas.iloc[max(int(np.ceil(k * prediction_probas.shape[0])) - 1, 0)]
+    if isinstance(k, int):
+        return probas.iloc[min(k, prediction_probas.shape[0] - 1)]
+    raise ValueError(f"K has unexpected type {type(k)}")
+
+
+def get_prediction_data(
+    data: pd.DataFrame, data_columns: DatasetColumns, pos_label: Optional[Union[str, int]], threshold: float = 0.5
+) -> PredictionData:
+    """Get predicted values and optional prediction probabilities from source data.
+    Also take into account a threshold value - if a probability is less than the value, do not take it into account.
+
+    Return and object with predicted values and an optional prediction probabilities.
+    """
+    # binary or multiclass classification
+    # for binary prediction_probas has column order [pos_label, neg_label]
+    # for multiclass classification return just values and probas
+    prediction = data_columns.utility_columns.prediction
+    target = data_columns.utility_columns.target
+    if isinstance(prediction, list) and len(prediction) > 2:
+        # list of columns with prediction probas, should be same as target labels
+        return PredictionData(
+            predictions=data[prediction].idxmax(axis=1),
+            prediction_probas=data[prediction],
+            labels=prediction,
+        )
 
-            else:
-                maper = {True: prediction_column[0], False: prediction_column[1]}
-                prediction_labels = (reference_data[prediction_column[0]] >= classification_threshold).map(maper)
+    if isinstance(prediction, str) and not is_float_dtype(data[prediction]) and target is not None:
+        # if prediction is not probas, get unique values from it and target
+        labels = np.union1d(data[target].unique(), data[prediction].unique()).tolist()
+        return PredictionData(
+            predictions=data[prediction],
+            prediction_probas=None,
+            labels=labels,
+        )
 
-            labels = sorted(set(reference_data[target_column]))
+    elif isinstance(prediction, str) and not is_float_dtype(data[prediction]) and target is None:
+        # if prediction is not probas, get unique values from it
+        labels = data[prediction].unique().tolist()
+
+    elif isinstance(prediction, str) and is_float_dtype(data[prediction]) and target is not None:
+        # if prediction is probas, get unique values from target only
+        labels = data[target].unique().tolist()
+
+    elif isinstance(prediction, list):
+        labels = prediction
+
+    # binary classification
+    # prediction in mapping is a list of two columns:
+    # one is positive value probabilities, second is negative value probabilities
+    if isinstance(prediction, list) and len(prediction) == 2:
+        pos_label = _check_pos_labels(pos_label, labels)
+        labels = pd.Series(labels)
+
+        # get negative label for binary classification
+        neg_label = labels[labels != pos_label].iloc[0]
+
+        predictions = threshold_probability_labels(data[prediction], pos_label, neg_label, threshold)
+        return PredictionData(
+            predictions=predictions,
+            prediction_probas=data[[pos_label, neg_label]],
+            labels=[pos_label, neg_label],
+        )
 
-            # calculate quality metrics
-            roc_auc = metrics.roc_auc_score(binaraized_target, array_prediction, average="macro")
-            log_loss = metrics.log_loss(binaraized_target, array_prediction)
-            accuracy_score = metrics.accuracy_score(reference_data[target_column], prediction_labels)
-            avg_precision = metrics.precision_score(reference_data[target_column], prediction_labels, average="macro")
-            avg_recall = metrics.recall_score(reference_data[target_column], prediction_labels, average="macro")
-            avg_f1 = metrics.f1_score(reference_data[target_column], prediction_labels, average="macro")
-
-            # calculate class support and metrics matrix
-            metrics_matrix = metrics.classification_report(
-                reference_data[target_column], prediction_labels, output_dict=True
+    # binary classification
+    # target is strings or other values, prediction is a string with positive label name, one column with probabilities
+    if (
+        isinstance(prediction, str)
+        and target is not None
+        and (is_string_dtype(data[target]) or is_object_dtype(data[target]))
+        and is_float_dtype(data[prediction])
+    ):
+        pos_label = _check_pos_labels(pos_label, labels)
+        if prediction not in labels:
+            raise ValueError(
+                "No prediction for the target labels were found. "
+                "Consider to rename columns with the prediction to match target labels."
             )
 
-            roc_aucs = None
-
-            if len(prediction_column) > 2:
-                roc_aucs = metrics.roc_auc_score(binaraized_target, array_prediction, average=None).tolist()
-
-            # calculate confusion matrix
-            conf_matrix = metrics.confusion_matrix(reference_data[target_column], prediction_labels)
-            confusion_by_classes = calculate_confusion_by_classes(conf_matrix, labels)
-
-            result.reference_metrics = ProbClassificationPerformanceMetrics(
-                accuracy=accuracy_score,
-                precision=avg_precision,
-                recall=avg_recall,
-                f1=avg_f1,
-                roc_auc=roc_auc,
-                log_loss=log_loss,
-                metrics_matrix=metrics_matrix,
-                confusion_matrix=ConfusionMatrix(labels=labels, values=conf_matrix.tolist()),
-                roc_aucs=roc_aucs,
-                confusion_by_classes=confusion_by_classes,
-            )
+        # get negative label for binary classification
+        labels = pd.Series(labels)
+        neg_label = labels[labels != pos_label].iloc[0]
+        if pos_label == prediction:
+            pos_preds = data[prediction]
+
+        else:
+            pos_preds = data[prediction].apply(lambda x: 1.0 - x)
+
+        prediction_probas = pd.DataFrame.from_dict(
+            {
+                pos_label: pos_preds,
+                neg_label: pos_preds.apply(lambda x: 1.0 - x),
+            }
+        )
+        predictions = threshold_probability_labels(prediction_probas, pos_label, neg_label, threshold)
+        return PredictionData(
+            predictions=predictions,
+            prediction_probas=prediction_probas,
+            labels=[pos_label, neg_label],
+        )
 
-            # calculate ROC and PR curves, PR table
-            if len(prediction_column) <= 2:
-                binaraized_target = pd.DataFrame(binaraized_target[:, 0])
-                binaraized_target.columns = ["target"]
-
-                fpr, tpr, thrs = metrics.roc_curve(binaraized_target, reference_data[prediction_column[0]])
-                result.reference_metrics.roc_curve = {"fpr": fpr.tolist(), "tpr": tpr.tolist(), "thrs": thrs.tolist()}
-
-                pr, rcl, thrs = metrics.precision_recall_curve(binaraized_target, reference_data[prediction_column[0]])
-                result.reference_metrics.pr_curve = {"pr": pr.tolist(), "rcl": rcl.tolist(), "thrs": thrs.tolist()}
-
-                pr_table = []
-                step_size = 0.05
-                binded = list(zip(binaraized_target["target"].tolist(), reference_data[prediction_column[0]].tolist()))
-                binded.sort(key=lambda item: item[1], reverse=True)
-                data_size = len(binded)
-                target_class_size = sum([x[0] for x in binded])
-                offset = max(round(data_size * step_size), 1)
-
-                for step in np.arange(offset, data_size + offset, offset):
-                    count = min(step, data_size)
-                    prob = round(binded[min(step, data_size - 1)][1], 2)
-                    top = round(100.0 * min(step, data_size) / data_size, 1)
-                    tp = sum([x[0] for x in binded[: min(step, data_size)]])
-                    fp = count - tp
-                    precision = round(100.0 * tp / count, 1)
-                    recall = round(100.0 * tp / target_class_size, 1)
-                    pr_table.append([top, int(count), prob, int(tp), int(fp), precision, recall])
+    # binary target and preds are numbers and prediction is a label
+    if not isinstance(prediction, list) and prediction in [0, 1, "0", "1"] and pos_label == 0:
+        if prediction in [0, "0"]:
+            pos_preds = data[prediction]
+        else:
+            pos_preds = data[prediction].apply(lambda x: 1.0 - x)
+        predictions = pos_preds.apply(lambda x: 0 if x >= threshold else 1)
+        prediction_probas = pd.DataFrame.from_dict(
+            {
+                0: pos_preds,
+                1: pos_preds.apply(lambda x: 1.0 - x),
+            }
+        )
+        return PredictionData(
+            predictions=predictions,
+            prediction_probas=prediction_probas,
+            labels=[0, 1],
+        )
 
-                result.reference_metrics.pr_table = pr_table
+    # binary target and preds are numbers
+    elif (
+        isinstance(prediction, str)
+        and target is not None
+        and is_integer_dtype(data[target].dtype)
+        and data[prediction].dtype == dtype("float")
+    ):
+        predictions = (data[prediction] >= threshold).astype(dtype("int64"))
+        prediction_probas = pd.DataFrame.from_dict(
+            {
+                1: data[prediction],
+                0: data[prediction].apply(lambda x: 1.0 - x),
+            }
+        )
+        return PredictionData(
+            predictions=predictions,
+            prediction_probas=prediction_probas,
+            labels=[1, 0],
+        )
 
+    # for other cases return just prediction values, probabilities are None by default
+    return PredictionData(
+        predictions=data[prediction],
+        prediction_probas=None,
+        labels=data[prediction].unique().tolist(),
+    )
+
+
+def _check_pos_labels(pos_label: Optional[Union[str, int]], labels: List[str]) -> Union[str, int]:
+    if pos_label is None:
+        raise ValueError("Undefined pos_label.")
+
+    if pos_label not in labels:
+        raise ValueError(f"Cannot find pos_label '{pos_label}' in labels {labels}")
+
+    return pos_label
+
+
+def threshold_probability_labels(
+    prediction_probas: pd.DataFrame, pos_label: Union[str, int], neg_label: Union[str, int], threshold: float
+) -> pd.Series:
+    """Get prediction values by probabilities with the threshold apply"""
+    return prediction_probas[pos_label].apply(lambda x: pos_label if x >= threshold else neg_label)
+
+
+STEP_SIZE = 0.05
+
+
+def calculate_pr_table(binded):
+    result = []
+    binded.sort(key=lambda item: item[1], reverse=True)
+    data_size = len(binded)
+    target_class_size = sum([x[0] for x in binded])
+    offset = max(round(data_size * STEP_SIZE), 1)
+
+    for step in np.arange(offset, data_size + offset, offset):
+        count = min(step, data_size)
+        prob = round(binded[min(step, data_size - 1)][1], 2)
+        top = round(100.0 * min(step, data_size) / data_size, 1)
+        tp = sum([x[0] for x in binded[: min(step, data_size)]])
+        fp = count - tp
+        precision = round(100.0 * tp / count, 1)
+        recall = round(100.0 * tp / target_class_size, 1)
+        result.append([top, int(count), prob, int(tp), int(fp), precision, recall])
+    return result
+
+
+def calculate_matrix(target: pd.Series, prediction: pd.Series, labels: List[Union[str, int]]) -> ConfusionMatrix:
+    sorted_labels = sorted(labels)
+    matrix = metrics.confusion_matrix(target, prediction, labels=sorted_labels)
+    return ConfusionMatrix(labels=sorted_labels, values=[row.tolist() for row in matrix])
+
+
+def collect_plot_data(prediction_probas: pd.DataFrame) -> Boxes:
+    res = {}
+    mins = []
+    lowers = []
+    means = []
+    uppers = []
+    maxs = []
+    for col in prediction_probas.columns:
+        mins.append(np.percentile(prediction_probas[col], 0))
+        lowers.append(np.percentile(prediction_probas[col], 25))
+        means.append(np.percentile(prediction_probas[col], 50))
+        uppers.append(np.percentile(prediction_probas[col], 75))
+        maxs.append(np.percentile(prediction_probas[col], 100))
+    res["mins"] = mins
+    res["lowers"] = lowers
+    res["means"] = means
+    res["uppers"] = uppers
+    res["maxs"] = maxs
+    return Boxes(mins=mins, lowers=lowers, means=means, uppers=uppers, maxs=maxs)
+
+
+def calculate_metrics(
+    column_mapping: ColumnMapping,
+    confusion_matrix: ConfusionMatrix,
+    target: pd.Series,
+    prediction: PredictionData,
+) -> "DatasetClassificationQuality":
+    if column_mapping.pos_label is not None:
+        pos_label = column_mapping.pos_label
+    else:
+        pos_label = 1
+    tpr = None
+    tnr = None
+    fpr = None
+    fnr = None
+    roc_auc = None
+    log_loss = None
+    rate_plots_data: Optional[RatesPlotData] = None
+    plot_data = None
+    if len(prediction.labels) == 2:
+        confusion_by_classes = calculate_confusion_by_classes(
+            np.array(confusion_matrix.values),
+            confusion_matrix.labels,
+        )
+        conf_by_pos_label = confusion_by_classes[pos_label]
+        precision = metrics.precision_score(target, prediction.predictions, pos_label=pos_label)
+        recall = metrics.recall_score(target, prediction.predictions, pos_label=pos_label)
+        f1 = metrics.f1_score(target, prediction.predictions, pos_label=pos_label)
+        tpr = conf_by_pos_label["tp"] / (conf_by_pos_label["tp"] + conf_by_pos_label["fn"])
+        tnr = conf_by_pos_label["tn"] / (conf_by_pos_label["tn"] + conf_by_pos_label["fp"])
+        fpr = conf_by_pos_label["fp"] / (conf_by_pos_label["fp"] + conf_by_pos_label["tn"])
+        fnr = conf_by_pos_label["fn"] / (conf_by_pos_label["fn"] + conf_by_pos_label["tp"])
+    else:
+        precision = metrics.precision_score(target, prediction.predictions, average="macro")
+        recall = metrics.recall_score(target, prediction.predictions, average="macro")
+        f1 = metrics.f1_score(target, prediction.predictions, average="macro")
+    if prediction.prediction_probas is not None:
+        binaraized_target = (
+            target.astype(str).values.reshape(-1, 1) == list(prediction.prediction_probas.columns.astype(str))
+        ).astype(int)
+        prediction_probas_array = prediction.prediction_probas.to_numpy()
+        roc_auc = metrics.roc_auc_score(binaraized_target, prediction_probas_array, average="macro")
+        log_loss = metrics.log_loss(binaraized_target, prediction_probas_array)
+        plot_data = collect_plot_data(prediction.prediction_probas)
+    if len(prediction.labels) == 2 and prediction.prediction_probas is not None:
+        fprs, tprs, thrs = metrics.roc_curve(target == pos_label, prediction.prediction_probas[pos_label])
+        df = pd.DataFrame(
+            {
+                "true": (target == pos_label).astype(int).values,
+                "preds": prediction.prediction_probas[pos_label].values,
+            }
+        )
+        tnrs = []
+        fnrs = []
+        for tr in thrs:
+            if tr < 1:
+                tn = df[(df.true == 0) & (df.preds < tr)].shape[0]
+                fn = df[(df.true == 1) & (df.preds < tr)].shape[0]
+                tp = df[(df.true == 1) & (df.preds >= tr)].shape[0]
+                fp = df[(df.true == 0) & (df.preds >= tr)].shape[0]
+                tnrs.append(tn / (tn + fp))
+                fnrs.append(fn / (fn + tp))
             else:
-                binaraized_target = pd.DataFrame(binaraized_target)
-                binaraized_target.columns = prediction_column
-
-                result.reference_metrics.roc_curve = {}
-                result.reference_metrics.pr_curve = {}
-                result.reference_metrics.pr_table = {}
-
-                for label in prediction_column:
-                    fpr, tpr, thrs = metrics.roc_curve(binaraized_target[label], reference_data[label])
-                    result.reference_metrics.roc_curve[label] = {
-                        "fpr": fpr.tolist(),
-                        "tpr": tpr.tolist(),
-                        "thrs": thrs.tolist(),
-                    }
-
-                    pr, rcl, thrs = metrics.precision_recall_curve(binaraized_target[label], reference_data[label])
-                    result.reference_metrics.pr_curve[label] = {
-                        "pr": pr.tolist(),
-                        "rcl": rcl.tolist(),
-                        "thrs": thrs.tolist(),
-                    }
-
-                    pr_table = []
-                    step_size = 0.05
-                    binded = list(zip(binaraized_target[label].tolist(), reference_data[label].tolist()))
-                    binded.sort(key=lambda item: item[1], reverse=True)
-                    data_size = len(binded)
-                    target_class_size = sum([x[0] for x in binded])
-                    offset = max(round(data_size * step_size), 1)
-
-                    for step in np.arange(offset, data_size + offset, offset):
-                        count = min(step, data_size)
-                        prob = round(binded[min(step, data_size - 1)][1], 2)
-                        top = round(100.0 * min(step, data_size) / data_size, 1)
-                        tp = sum([x[0] for x in binded[: min(step, data_size)]])
-                        fp = count - tp
-                        precision = round(100.0 * tp / count, 1)
-                        recall = round(100.0 * tp / target_class_size, 1)
-                        pr_table.append([top, int(count), prob, int(tp), int(fp), precision, recall])
-                    result.reference_metrics.pr_table[label] = pr_table
-
-            if current_data is not None:
-                current_data.replace([np.inf, -np.inf], np.nan, inplace=True)
-                current_data.dropna(axis=0, how="any", inplace=True, subset=target_and_preds)
-
-                binaraized_target = (current_data[target_column].values.reshape(-1, 1) == prediction_column).astype(int)
-
-                array_prediction = current_data[prediction_column].to_numpy()
-
-                if len(prediction_column) > 2:
-                    prediction_ids = np.argmax(array_prediction, axis=-1)
-                    prediction_labels = [prediction_column[x] for x in prediction_ids]
-
-                else:
-                    maper = {True: prediction_column[0], False: prediction_column[1]}
-                    prediction_labels = (current_data[prediction_column[0]] >= classification_threshold).map(maper)
-
-                # calculate quality metrics
-                roc_auc = metrics.roc_auc_score(binaraized_target, array_prediction, average="macro")
-                log_loss = metrics.log_loss(binaraized_target, array_prediction)
-                accuracy_score = metrics.accuracy_score(current_data[target_column], prediction_labels)
-                avg_precision = metrics.precision_score(current_data[target_column], prediction_labels, average="macro")
-                avg_recall = metrics.recall_score(current_data[target_column], prediction_labels, average="macro")
-                avg_f1 = metrics.f1_score(current_data[target_column], prediction_labels, average="macro")
-
-                # calculate class support and metrics matrix
-                metrics_matrix = metrics.classification_report(
-                    current_data[target_column], prediction_labels, output_dict=True
-                )
-
-                roc_aucs = None
-
-                if len(prediction_column) > 2:
-                    roc_aucs = metrics.roc_auc_score(binaraized_target, array_prediction, average=None).tolist()
-
-                # calculate confusion matrix
-                conf_matrix = metrics.confusion_matrix(current_data[target_column], prediction_labels)
-                # get TP, FP, TN, FN metrics for each class
-                confusion_by_classes = calculate_confusion_by_classes(conf_matrix, labels)
-
-                result.current_metrics = ProbClassificationPerformanceMetrics(
-                    accuracy=accuracy_score,
-                    precision=avg_precision,
-                    recall=avg_recall,
-                    f1=avg_f1,
-                    roc_auc=roc_auc,
-                    log_loss=log_loss,
-                    metrics_matrix=metrics_matrix,
-                    confusion_matrix=ConfusionMatrix(labels=labels, values=conf_matrix.tolist()),
-                    roc_aucs=roc_aucs,
-                    confusion_by_classes=confusion_by_classes,
-                )
-
-                # calculate ROC and PR curves, PR table
-                if len(prediction_column) <= 2:
-                    binaraized_target = pd.DataFrame(binaraized_target[:, 0])
-                    binaraized_target.columns = ["target"]
-
-                    fpr, tpr, thrs = metrics.roc_curve(binaraized_target, current_data[prediction_column[0]])
-                    result.current_metrics.roc_curve = {"fpr": fpr.tolist(), "tpr": tpr.tolist(), "thrs": thrs.tolist()}
-
-                    pr, rcl, thrs = metrics.precision_recall_curve(
-                        binaraized_target, current_data[prediction_column[0]]
-                    )
-                    result.current_metrics.pr_curve = {"pr": pr.tolist(), "rcl": rcl.tolist(), "thrs": thrs.tolist()}
-
-                    pr_table = []
-                    step_size = 0.05
-                    binded = list(
-                        zip(binaraized_target["target"].tolist(), current_data[prediction_column[0]].tolist())
-                    )
-                    binded.sort(key=lambda item: item[1], reverse=True)
-                    data_size = len(binded)
-                    target_class_size = sum([x[0] for x in binded])
-                    offset = max(round(data_size * step_size), 1)
-
-                    for step in np.arange(offset, data_size + offset, offset):
-                        count = min(step, data_size)
-                        prob = round(binded[min(step, data_size - 1)][1], 2)
-                        top = round(100.0 * min(step, data_size) / data_size, 1)
-                        tp = sum([x[0] for x in binded[: min(step, data_size)]])
-                        fp = count - tp
-                        precision = round(100.0 * tp / count, 1)
-                        recall = round(100.0 * tp / target_class_size, 1)
-                        pr_table.append([top, int(count), prob, int(tp), int(fp), precision, recall])
-
-                    result.current_metrics.pr_table = pr_table
-
-                else:
-                    binaraized_target = pd.DataFrame(binaraized_target)
-                    binaraized_target.columns = prediction_column
-
-                    result.current_metrics.roc_curve = {}
-                    result.current_metrics.pr_curve = {}
-                    result.current_metrics.pr_table = {}
-
-                    for label in prediction_column:
-                        fpr, tpr, thrs = metrics.roc_curve(binaraized_target[label], current_data[label])
-                        result.current_metrics.roc_curve[label] = {
-                            "fpr": fpr.tolist(),
-                            "tpr": tpr.tolist(),
-                            "thrs": thrs.tolist(),
-                        }
-
-                        pr, rcl, thrs = metrics.precision_recall_curve(binaraized_target[label], current_data[label])
-                        result.current_metrics.pr_curve[label] = {
-                            "pr": pr.tolist(),
-                            "rcl": rcl.tolist(),
-                            "thrs": thrs.tolist(),
-                        }
-
-                        pr_table = []
-                        step_size = 0.05
-                        binded = list(zip(binaraized_target[label].tolist(), current_data[label].tolist()))
-                        binded.sort(key=lambda item: item[1], reverse=True)
-                        data_size = len(binded)
-                        target_class_size = sum([x[0] for x in binded])
-                        offset = max(round(data_size * step_size), 1)
-
-                        for step in np.arange(offset, data_size + offset, offset):
-                            count = min(step, data_size)
-                            prob = round(binded[min(step, data_size - 1)][1], 2)
-                            top = round(100.0 * min(step, data_size) / data_size, 1)
-                            tp = sum([x[0] for x in binded[: min(step, data_size)]])
-                            fp = count - tp
-                            precision = round(100.0 * tp / count, 1)
-                            recall = round(100.0 * tp / target_class_size, 1)
-                            pr_table.append([top, int(count), prob, int(tp), int(fp), precision, recall])
-
-                        result.current_metrics.pr_table[label] = pr_table
-
-        return result
+                fnrs.append(1)
+                tnrs.append(1)
+        rate_plots_data = RatesPlotData(thrs=thrs.tolist(), tpr=tprs.tolist(), fpr=fprs.tolist(), fnr=fnrs, tnr=tnrs)
+
+    return DatasetClassificationQuality(
+        accuracy=metrics.accuracy_score(target, prediction.predictions),
+        precision=precision,
+        recall=recall,
+        f1=f1,
+        tpr=tpr,
+        tnr=tnr,
+        fpr=fpr,
+        fnr=fnr,
+        roc_auc=roc_auc,
+        log_loss=log_loss,
+        rate_plots_data=rate_plots_data,
+        plot_data=plot_data,
+    )
```

### Comparing `evidently-0.2.8/src/evidently/calculations/classification_performance.py` & `evidently-0.3.0/src/evidently/metrics/data_drift/target_by_features_table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,372 +1,331 @@
-from typing import TYPE_CHECKING
+import json
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Sequence
 from typing import Union
 
 import numpy as np
 import pandas as pd
-from numpy import dtype
-from pandas.core.dtypes.common import is_float_dtype
-from pandas.core.dtypes.common import is_integer_dtype
-from pandas.core.dtypes.common import is_object_dtype
-from pandas.core.dtypes.common import is_string_dtype
-from sklearn import metrics
-
-from evidently import ColumnMapping
-from evidently.metric_results import Boxes
-from evidently.metric_results import ConfusionMatrix
-from evidently.metric_results import DatasetClassificationQuality
-from evidently.metric_results import DatasetColumns
+import plotly.express as px
+import plotly.graph_objs as go
+from pandas.api.types import is_integer_dtype
+from pandas.api.types import is_string_dtype
+from plotly.subplots import make_subplots
+
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.calculations.classification_performance import get_prediction_data
+from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
+from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
+from evidently.features.text_length_feature import TextLength
 from evidently.metric_results import PredictionData
-from evidently.metric_results import RatesPlotData
+from evidently.metric_results import StatsByFeature
+from evidently.model.widget import AdditionalGraphInfo
+from evidently.model.widget import BaseWidgetInfo
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.utils.data_operations import process_columns
+from evidently.utils.data_preprocessing import DataDefinition
+
+
+class TargetByFeaturesTableResults(MetricResult):
+    class Config:
+        dict_include = False
+
+    current: StatsByFeature
+    reference: Optional[StatsByFeature]
+    target_name: Optional[str]
+    columns: List[str]
+    task: str
+
+
+class TargetByFeaturesTable(Metric[TargetByFeaturesTableResults]):
+    columns: Optional[List[str]]
+    text_features_gen: Optional[
+        Dict[
+            str,
+            Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]],
+        ]
+    ]
+
+    def __init__(self, columns: Optional[List[str]] = None):
+        self.columns = columns
+        self.text_features_gen = None
+
+    def required_features(self, data_definition: DataDefinition):
+        if len(data_definition.get_columns("text_features")) > 0:
+            text_cols = [col.column_name for col in data_definition.get_columns("text_features")]
+            text_features_gen = {}
+            text_features_gen_result = []
+            for col in text_cols:
+                col_dict: Dict[
+                    str,
+                    Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage],
+                ] = {}
+                col_dict[f"{col}: Text Length"] = TextLength(col)
+                col_dict[f"{col}: Non Letter Character %"] = NonLetterCharacterPercentage(col)
+                col_dict[f"{col}: OOV %"] = OOVWordsPercentage(col)
+
+                text_features_gen_result += [
+                    col_dict[f"{col}: Text Length"],
+                    col_dict[f"{col}: Non Letter Character %"],
+                    col_dict[f"{col}: OOV %"],
+                ]
+                text_features_gen[col] = col_dict
+            self.text_features_gen = text_features_gen
 
-if TYPE_CHECKING:
-    pass
-
-
-def calculate_confusion_by_classes(
-    confusion_matrix: np.ndarray, class_names: Sequence[Union[str, int]]
-) -> Dict[Union[str, int], Dict[str, int]]:
-    """Calculate metrics:
-    - TP (true positive)
-    - TN (true negative)
-    - FP (false positive)
-    - FN (false negative)
-    for each class from confusion matrix.
-
-    Returns:
-        a dict like::
-
-            {
-                "class_1_name": {
-                    "tp": 1,
-                    "tn": 5,
-                    "fp": 0,
-                    "fn": 3,
-                },
-                "class_1_name": {
-                    "tp": 1,
-                    "tn": 5,
-                    "fp": 0,
-                    "fn": 3,
-                },
-            }
-    """
-    true_positive = np.diag(confusion_matrix)
-    false_positive = confusion_matrix.sum(axis=0) - np.diag(confusion_matrix)
-    false_negative = confusion_matrix.sum(axis=1) - np.diag(confusion_matrix)
-    true_negative = confusion_matrix.sum() - (false_positive + false_negative + true_positive)
-    confusion_by_classes = {}
-
-    for idx, class_name in enumerate(class_names):
-        confusion_by_classes[class_name] = {
-            "tp": true_positive[idx],
-            "tn": true_negative[idx],
-            "fp": false_positive[idx],
-            "fn": false_negative[idx],
-        }
-
-    return confusion_by_classes
-
-
-def k_probability_threshold(prediction_probas: pd.DataFrame, k: Union[int, float]) -> float:
-    probas = prediction_probas.iloc[:, 0].sort_values(ascending=False)
-    if isinstance(k, float):
-        if k < 0.0 or k > 1.0:
-            raise ValueError(f"K should be in range [0.0, 1.0] but was {k}")
-        return probas.iloc[max(int(np.ceil(k * prediction_probas.shape[0])) - 1, 0)]
-    if isinstance(k, int):
-        return probas.iloc[min(k, prediction_probas.shape[0] - 1)]
-    raise ValueError(f"K has unexpected type {type(k)}")
-
-
-def get_prediction_data(
-    data: pd.DataFrame, data_columns: DatasetColumns, pos_label: Optional[Union[str, int]], threshold: float = 0.5
-) -> PredictionData:
-    """Get predicted values and optional prediction probabilities from source data.
-    Also take into account a threshold value - if a probability is less than the value, do not take it into account.
-
-    Return and object with predicted values and an optional prediction probabilities.
-    """
-    # binary or multiclass classification
-    # for binary prediction_probas has column order [pos_label, neg_label]
-    # for multiclass classification return just values and probas
-    prediction = data_columns.utility_columns.prediction
-    target = data_columns.utility_columns.target
-    if isinstance(prediction, list) and len(prediction) > 2:
-        # list of columns with prediction probas, should be same as target labels
-        return PredictionData(
-            predictions=data[prediction].idxmax(axis=1),
-            prediction_probas=data[prediction],
-            labels=prediction,
-        )
-
-    if isinstance(prediction, str) and not is_float_dtype(data[prediction]) and target is not None:
-        # if prediction is not probas, get unique values from it and target
-        labels = np.union1d(data[target].unique(), data[prediction].unique()).tolist()
-        return PredictionData(
-            predictions=data[prediction],
-            prediction_probas=None,
-            labels=labels,
-        )
+            return text_features_gen_result
+        else:
+            return []
 
-    elif isinstance(prediction, str) and not is_float_dtype(data[prediction]) and target is None:
-        # if prediction is not probas, get unique values from it
-        labels = data[prediction].unique().tolist()
-
-    elif isinstance(prediction, str) and is_float_dtype(data[prediction]) and target is not None:
-        # if prediction is probas, get unique values from target only
-        labels = data[target].unique().tolist()
-
-    elif isinstance(prediction, list):
-        labels = prediction
-
-    # binary classification
-    # prediction in mapping is a list of two columns:
-    # one is positive value probabilities, second is negative value probabilities
-    if isinstance(prediction, list) and len(prediction) == 2:
-        pos_label = _check_pos_labels(pos_label, labels)
-        labels = pd.Series(labels)
-
-        # get negative label for binary classification
-        neg_label = labels[labels != pos_label].iloc[0]
-
-        predictions = threshold_probability_labels(data[prediction], pos_label, neg_label, threshold)
-        return PredictionData(
-            predictions=predictions,
-            prediction_probas=data[[pos_label, neg_label]],
-            labels=[pos_label, neg_label],
-        )
+    def get_parameters(self) -> tuple:
+        return ()
 
-    # binary classification
-    # target is strings or other values, prediction is a string with positive label name, one column with probabilities
-    if (
-        isinstance(prediction, str)
-        and target is not None
-        and (is_string_dtype(data[target]) or is_object_dtype(data[target]))
-        and is_float_dtype(data[prediction])
-    ):
-        pos_label = _check_pos_labels(pos_label, labels)
-        if prediction not in labels:
-            raise ValueError(
-                "No prediction for the target labels were found. "
-                "Consider to rename columns with the prediction to match target labels."
+    def calculate(self, data: InputData) -> TargetByFeaturesTableResults:
+        dataset_columns = process_columns(data.current_data, data.column_mapping)
+        target_name = dataset_columns.utility_columns.target
+        prediction_name = dataset_columns.utility_columns.prediction
+        if target_name is None and prediction_name is None:
+            raise ValueError("The columns 'target' or 'prediction' should be present")
+        if data.reference_data is None:
+            raise ValueError("Reference data should be present")
+        curr_df = data.current_data.copy()
+        ref_df = data.reference_data.copy()
+        curr_predictions = None
+        ref_predictions = None
+        if prediction_name is not None:
+            curr_predictions = get_prediction_data(data.current_data, dataset_columns, data.column_mapping.pos_label)
+            ref_predictions = get_prediction_data(data.reference_data, dataset_columns, data.column_mapping.pos_label)
+
+        if self.columns is None:
+            columns = (
+                dataset_columns.num_feature_names
+                + dataset_columns.cat_feature_names
+                + dataset_columns.text_feature_names
             )
-
-        # get negative label for binary classification
-        labels = pd.Series(labels)
-        neg_label = labels[labels != pos_label].iloc[0]
-        if pos_label == prediction:
-            pos_preds = data[prediction]
-
         else:
-            pos_preds = data[prediction].apply(lambda x: 1.0 - x)
+            columns = list(
+                np.intersect1d(
+                    self.columns,
+                    (
+                        dataset_columns.num_feature_names
+                        + dataset_columns.cat_feature_names
+                        + dataset_columns.text_feature_names
+                    ),
+                )
+            )
+        if data.column_mapping.task is not None:
+            task = data.column_mapping.task
+        else:
+            if target_name is not None:
+                if curr_df[target_name].nunique() < 5 or is_string_dtype(curr_df[target_name]):
+                    task = "classification"
+                else:
+                    task = "regression"
+            elif curr_predictions is not None:
+                if is_string_dtype(curr_predictions.predictions) or (
+                    is_integer_dtype(curr_predictions.predictions) and curr_predictions.predictions.nunique() < 5
+                ):
+                    task = "classification"
+                else:
+                    task = "regression"
+            else:
+                raise ValueError("Task parameter of column_mapping should be specified")
+        # process text columns
+        if (
+            self.text_features_gen is not None
+            and len(np.intersect1d(list(self.text_features_gen.keys()), columns)) >= 1
+        ):
+            for col in np.intersect1d(list(self.text_features_gen.keys()), columns):
+                columns += list(self.text_features_gen[col].keys())
+                columns.remove(col)
+                curr_text_df = pd.concat(
+                    [data.get_current_column(x.feature_name()) for x in list(self.text_features_gen[col].values())],
+                    axis=1,
+                )
+                curr_text_df.columns = list(self.text_features_gen[col].keys())
+                curr_df = pd.concat(
+                    [
+                        curr_df.reset_index(drop=True),
+                        curr_text_df.reset_index(drop=True),
+                    ],
+                    axis=1,
+                )
+
+                if ref_df is not None:
+                    ref_text_df = pd.concat(
+                        [
+                            data.get_reference_column(x.feature_name())
+                            for x in list(self.text_features_gen[col].values())
+                        ],
+                        axis=1,
+                    )
+                    ref_text_df.columns = list(self.text_features_gen[col].keys())
+                    ref_df = pd.concat(
+                        [
+                            ref_df.reset_index(drop=True),
+                            ref_text_df.reset_index(drop=True),
+                        ],
+                        axis=1,
+                    )
+        table_columns = columns.copy()
+        if target_name is not None:
+            table_columns += [target_name]
+        if prediction_name is not None and isinstance(prediction_name, str):
+            table_columns += [prediction_name]
+        if prediction_name is not None and isinstance(prediction_name, list):
+            table_columns += prediction_name
+
+        return TargetByFeaturesTableResults(
+            current=StatsByFeature(
+                plot_data=curr_df[table_columns],
+                predictions=curr_predictions,
+            ),
+            reference=StatsByFeature(
+                plot_data=ref_df[table_columns],
+                predictions=ref_predictions,
+            ),
+            columns=columns,
+            target_name=target_name,
+            task=task,
+        )
+
+
+@default_renderer(wrap_type=TargetByFeaturesTable)
+class TargetByFeaturesTableRenderer(MetricRenderer):
+    def render_html(self, obj: TargetByFeaturesTable) -> List[BaseWidgetInfo]:
+        result = obj.get_result()
+        current_data = result.current.plot_data
+        # todo: better typing
+        assert current_data is not None
+        reference_data = result.reference.plot_data if result.reference is not None else None
+        target_name = result.target_name
+        curr_predictions = result.current.predictions
+        ref_predictions = result.reference.predictions if result.reference is not None else None
+        columns = result.columns
+        task = result.task
+        if curr_predictions is not None and ref_predictions is not None:
+            current_data["prediction_labels"] = curr_predictions.predictions.values
+            reference_data["prediction_labels"] = ref_predictions.predictions.values
+
+        additional_graphs_data = []
+        params_data = []
+
+        for feature_name in columns:
+            # add data for table in params
+            parts = []
+
+            if target_name is not None:
+                parts.append({"title": "Target", "id": feature_name + "_target_values"})
+                if task == "regression":
+                    target_fig = self._get_regression_fig(feature_name, target_name, current_data, reference_data)
+                else:
+                    target_fig = self._get_classification_fig(feature_name, target_name, current_data, reference_data)
+
+                target_fig_json = json.loads(target_fig.to_json())
+
+                additional_graphs_data.append(
+                    AdditionalGraphInfo(
+                        feature_name + "_target_values",
+                        {
+                            "data": target_fig_json["data"],
+                            "layout": target_fig_json["layout"],
+                        },
+                    )
+                )
+
+            if curr_predictions is not None:
+                parts.append({"title": "Prediction", "id": feature_name + "_prediction_values"})
+                if task == "regression":
+                    preds_fig = self._get_regression_fig(
+                        feature_name, "prediction_labels", current_data, reference_data
+                    )
+                else:
+                    preds_fig = self._get_classification_fig(
+                        feature_name, "prediction_labels", current_data, reference_data
+                    )
+                preds_fig_json = json.loads(preds_fig.to_json())
+
+                additional_graphs_data.append(
+                    AdditionalGraphInfo(
+                        feature_name + "_prediction_values",
+                        {
+                            "data": preds_fig_json["data"],
+                            "layout": preds_fig_json["layout"],
+                        },
+                    )
+                )
+
+            params_data.append(
+                {
+                    "details": {
+                        "parts": parts,
+                        "insights": [],
+                    },
+                    "f1": feature_name,
+                }
+            )
+        return [
+            BaseWidgetInfo(
+                title="Target (Prediction) Behavior By Feature",
+                type="big_table",
+                size=2,
+                params={
+                    "rowsPerPage": min(len(columns), 10),
+                    "columns": [{"title": "Feature", "field": "f1"}],
+                    "data": params_data,
+                },
+                additionalGraphs=additional_graphs_data,
+            )
+        ]
 
-        prediction_probas = pd.DataFrame.from_dict(
-            {
-                pos_label: pos_preds,
-                neg_label: pos_preds.apply(lambda x: 1.0 - x),
-            }
-        )
-        predictions = threshold_probability_labels(prediction_probas, pos_label, neg_label, threshold)
-        return PredictionData(
-            predictions=predictions,
-            prediction_probas=prediction_probas,
-            labels=[pos_label, neg_label],
-        )
+    def _get_regression_fig(self, feature_name: str, main_column: str, curr_data: pd.DataFrame, ref_data: pd.DataFrame):
+        fig = make_subplots(rows=1, cols=2, subplot_titles=("Current", "Reference"), shared_yaxes=True)
+        fig.add_trace(
+            go.Scattergl(
+                x=curr_data[feature_name],
+                y=curr_data[main_column],
+                mode="markers",
+                name="current",
+                marker=dict(size=6, color=self.color_options.primary_color),
+            ),
+            row=1,
+            col=1,
+        )
+
+        fig.add_trace(
+            go.Scatter(
+                x=ref_data[feature_name],
+                y=ref_data[main_column],
+                mode="markers",
+                name="reference",
+                marker=dict(size=6, color=self.color_options.secondary_color),
+            ),
+            row=1,
+            col=2,
+        )
+        fig.update_xaxes(title_text=feature_name, showgrid=True, row=1, col=1)
+        fig.update_xaxes(title_text=feature_name, showgrid=True, row=1, col=2)
+        fig.update_yaxes(title_text=main_column, showgrid=True, row=1, col=1)
 
-    # binary target and preds are numbers and prediction is a label
-    if not isinstance(prediction, list) and prediction in [0, 1, "0", "1"] and pos_label == 0:
-        if prediction in [0, "0"]:
-            pos_preds = data[prediction]
-        else:
-            pos_preds = data[prediction].apply(lambda x: 1.0 - x)
-        predictions = pos_preds.apply(lambda x: 0 if x >= threshold else 1)
-        prediction_probas = pd.DataFrame.from_dict(
-            {
-                0: pos_preds,
-                1: pos_preds.apply(lambda x: 1.0 - x),
-            }
-        )
-        return PredictionData(
-            predictions=predictions,
-            prediction_probas=prediction_probas,
-            labels=[0, 1],
-        )
+        return fig
 
-    # binary target and preds are numbers
-    elif (
-        isinstance(prediction, str)
-        and target is not None
-        and is_integer_dtype(data[target].dtype)
-        and data[prediction].dtype == dtype("float")
+    def _get_classification_fig(
+        self, feature_name: str, main_column: str, curr_data: pd.DataFrame, ref_data: pd.DataFrame
     ):
-        predictions = (data[prediction] >= threshold).astype(dtype("int64"))
-        prediction_probas = pd.DataFrame.from_dict(
-            {
-                1: data[prediction],
-                0: data[prediction].apply(lambda x: 1.0 - x),
-            }
-        )
-        return PredictionData(
-            predictions=predictions,
-            prediction_probas=prediction_probas,
-            labels=[1, 0],
+        curr = curr_data.copy()
+        ref = ref_data.copy()
+        ref["dataset"] = "Reference"
+        curr["dataset"] = "Current"
+        merged_data = pd.concat([ref, curr])
+        fig = px.histogram(
+            merged_data,
+            x=feature_name,
+            color=main_column,
+            facet_col="dataset",
+            barmode="overlay",
+            category_orders={"dataset": ["Current", "Reference"]},
         )
 
-    # for other cases return just prediction values, probabilities are None by default
-    return PredictionData(
-        predictions=data[prediction],
-        prediction_probas=None,
-        labels=data[prediction].unique().tolist(),
-    )
-
-
-def _check_pos_labels(pos_label: Optional[Union[str, int]], labels: List[str]) -> Union[str, int]:
-    if pos_label is None:
-        raise ValueError("Undefined pos_label.")
-
-    if pos_label not in labels:
-        raise ValueError(f"Cannot find pos_label '{pos_label}' in labels {labels}")
-
-    return pos_label
-
-
-def threshold_probability_labels(
-    prediction_probas: pd.DataFrame, pos_label: Union[str, int], neg_label: Union[str, int], threshold: float
-) -> pd.Series:
-    """Get prediction values by probabilities with the threshold apply"""
-    return prediction_probas[pos_label].apply(lambda x: pos_label if x >= threshold else neg_label)
-
-
-STEP_SIZE = 0.05
-
-
-def calculate_pr_table(binded):
-    result = []
-    binded.sort(key=lambda item: item[1], reverse=True)
-    data_size = len(binded)
-    target_class_size = sum([x[0] for x in binded])
-    offset = max(round(data_size * STEP_SIZE), 1)
-
-    for step in np.arange(offset, data_size + offset, offset):
-        count = min(step, data_size)
-        prob = round(binded[min(step, data_size - 1)][1], 2)
-        top = round(100.0 * min(step, data_size) / data_size, 1)
-        tp = sum([x[0] for x in binded[: min(step, data_size)]])
-        fp = count - tp
-        precision = round(100.0 * tp / count, 1)
-        recall = round(100.0 * tp / target_class_size, 1)
-        result.append([top, int(count), prob, int(tp), int(fp), precision, recall])
-    return result
-
-
-def calculate_matrix(target: pd.Series, prediction: pd.Series, labels: List[Union[str, int]]) -> ConfusionMatrix:
-    sorted_labels = sorted(labels)
-    matrix = metrics.confusion_matrix(target, prediction, labels=sorted_labels)
-    return ConfusionMatrix(labels=sorted_labels, values=[row.tolist() for row in matrix])
-
-
-def collect_plot_data(prediction_probas: pd.DataFrame) -> Boxes:
-    res = {}
-    mins = []
-    lowers = []
-    means = []
-    uppers = []
-    maxs = []
-    for col in prediction_probas.columns:
-        mins.append(np.percentile(prediction_probas[col], 0))
-        lowers.append(np.percentile(prediction_probas[col], 25))
-        means.append(np.percentile(prediction_probas[col], 50))
-        uppers.append(np.percentile(prediction_probas[col], 75))
-        maxs.append(np.percentile(prediction_probas[col], 100))
-    res["mins"] = mins
-    res["lowers"] = lowers
-    res["means"] = means
-    res["uppers"] = uppers
-    res["maxs"] = maxs
-    return Boxes(mins=mins, lowers=lowers, means=means, uppers=uppers, maxs=maxs)
-
-
-def calculate_metrics(
-    column_mapping: ColumnMapping,
-    confusion_matrix: ConfusionMatrix,
-    target: pd.Series,
-    prediction: PredictionData,
-) -> "DatasetClassificationQuality":
-    if column_mapping.pos_label is not None:
-        pos_label = column_mapping.pos_label
-    else:
-        pos_label = 1
-    tpr = None
-    tnr = None
-    fpr = None
-    fnr = None
-    roc_auc = None
-    log_loss = None
-    rate_plots_data: Optional[RatesPlotData] = None
-    plot_data = None
-    if len(prediction.labels) == 2:
-        confusion_by_classes = calculate_confusion_by_classes(
-            np.array(confusion_matrix.values),
-            confusion_matrix.labels,
-        )
-        conf_by_pos_label = confusion_by_classes[pos_label]
-        precision = metrics.precision_score(target, prediction.predictions, pos_label=pos_label)
-        recall = metrics.recall_score(target, prediction.predictions, pos_label=pos_label)
-        f1 = metrics.f1_score(target, prediction.predictions, pos_label=pos_label)
-        tpr = conf_by_pos_label["tp"] / (conf_by_pos_label["tp"] + conf_by_pos_label["fn"])
-        tnr = conf_by_pos_label["tn"] / (conf_by_pos_label["tn"] + conf_by_pos_label["fp"])
-        fpr = conf_by_pos_label["fp"] / (conf_by_pos_label["fp"] + conf_by_pos_label["tn"])
-        fnr = conf_by_pos_label["fn"] / (conf_by_pos_label["fn"] + conf_by_pos_label["tp"])
-    else:
-        precision = metrics.precision_score(target, prediction.predictions, average="macro")
-        recall = metrics.recall_score(target, prediction.predictions, average="macro")
-        f1 = metrics.f1_score(target, prediction.predictions, average="macro")
-    if prediction.prediction_probas is not None:
-        binaraized_target = (
-            target.astype(str).values.reshape(-1, 1) == list(prediction.prediction_probas.columns.astype(str))
-        ).astype(int)
-        prediction_probas_array = prediction.prediction_probas.to_numpy()
-        roc_auc = metrics.roc_auc_score(binaraized_target, prediction_probas_array, average="macro")
-        log_loss = metrics.log_loss(binaraized_target, prediction_probas_array)
-        plot_data = collect_plot_data(prediction.prediction_probas)
-    if len(prediction.labels) == 2 and prediction.prediction_probas is not None:
-        fprs, tprs, thrs = metrics.roc_curve(target == pos_label, prediction.prediction_probas[pos_label])
-        df = pd.DataFrame(
-            {
-                "true": (target == pos_label).astype(int).values,
-                "preds": prediction.prediction_probas[pos_label].values,
-            }
-        )
-        tnrs = []
-        fnrs = []
-        for tr in thrs:
-            if tr < 1:
-                tn = df[(df.true == 0) & (df.preds < tr)].shape[0]
-                fn = df[(df.true == 1) & (df.preds < tr)].shape[0]
-                tp = df[(df.true == 1) & (df.preds >= tr)].shape[0]
-                fp = df[(df.true == 0) & (df.preds >= tr)].shape[0]
-                tnrs.append(tn / (tn + fp))
-                fnrs.append(fn / (fn + tp))
-            else:
-                fnrs.append(1)
-                tnrs.append(1)
-        rate_plots_data = RatesPlotData(thrs=thrs.tolist(), tpr=tprs.tolist(), fpr=fprs.tolist(), fnr=fnrs, tnr=tnrs)
-
-    return DatasetClassificationQuality(
-        accuracy=metrics.accuracy_score(target, prediction.predictions),
-        precision=precision,
-        recall=recall,
-        f1=f1,
-        tpr=tpr,
-        tnr=tnr,
-        fpr=fpr,
-        fnr=fnr,
-        roc_auc=roc_auc,
-        log_loss=log_loss,
-        rate_plots_data=rate_plots_data,
-        plot_data=plot_data,
-    )
+        return fig
```

### Comparing `evidently-0.2.8/src/evidently/calculations/data_drift.py` & `evidently-0.3.0/src/evidently/calculations/data_drift.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,47 +7,47 @@
 from typing import Sequence
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import ColumnMetricResult
-from evidently.base_metric import MetricResultField
+from evidently.base_metric import MetricResult
 from evidently.calculations.stattests import get_stattest
 from evidently.core import ColumnType
+from evidently.core import IncludeTags
 from evidently.metric_results import DatasetColumns
 from evidently.metric_results import Distribution
 from evidently.metric_results import DistributionIncluded
 from evidently.metric_results import ScatterField
 from evidently.options import DataDriftOptions
 from evidently.utils.data_drift_utils import get_text_data_for_plots
 from evidently.utils.data_operations import recognize_column_type_
 from evidently.utils.types import Numeric
 from evidently.utils.visualizations import get_distribution_for_column
 
 Examples = List[str]
 Words = List[str]
 
 
-class DriftStatsField(MetricResultField):
+class DriftStatsField(MetricResult):
     class Config:
-        dict_include_fields = {"small_distribution"}
+        dict_exclude_fields = {"characteristic_examples", "characteristic_words", "correlations"}
+        # todo: after tests PR
+        field_tags = {k: {IncludeTags.Render} for k in dict_exclude_fields}
         pd_include = False
 
     distribution: Optional[Distribution]
     characteristic_examples: Optional[Examples]
     characteristic_words: Optional[Words]
     small_distribution: Optional[DistributionIncluded]
     correlations: Optional[Dict[str, float]]
 
 
 class ColumnDataDriftMetrics(ColumnMetricResult):
-    class Config:
-        dict_exclude_fields = {"scatter"}
-
     stattest_name: str
     stattest_threshold: Optional[float]
     drift_score: Numeric
     drift_detected: bool
 
     current: DriftStatsField
     reference: DriftStatsField
@@ -60,15 +60,15 @@
     """Dataset drift calculation results"""
 
     number_of_drifted_columns: int
     dataset_drift_score: float
     dataset_drift: bool
 
 
-class DatasetDriftMetrics(MetricResultField):
+class DatasetDriftMetrics(MetricResult):
     number_of_columns: int
     number_of_drifted_columns: int
     share_of_drifted_columns: float
     dataset_drift: bool
     drift_by_columns: Dict[str, ColumnDataDriftMetrics]
     options: DataDriftOptions
     dataset_columns: DatasetColumns
```

### Comparing `evidently-0.2.8/src/evidently/calculations/data_integration.py` & `evidently-0.3.0/src/evidently/calculations/data_integration.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/data_quality.py` & `evidently-0.3.0/src/evidently/calculations/data_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,16 +263,16 @@
 
     return result
 
 
 class DataQualityGetPlotData:
     def __init__(self) -> None:
         self.period_prefix: Optional[str] = None
-        self.curr: Optional[pd.Series] = None
-        self.ref: Optional[pd.Series] = None
+        self.curr: Optional[pd.DataFrame] = None
+        self.ref: Optional[pd.DataFrame] = None
 
     def calculate_main_plot(
         self,
         curr: pd.DataFrame,
         ref: Optional[pd.DataFrame],
         feature_name: str,
         feature_type: str,
@@ -708,57 +708,63 @@
     return ColumnCorrelations(
         column_name=column_name,
         kind="cramer_v",
         values=Distribution(x=result_x, y=result_y),
     )
 
 
-def calculate_category_column_correlations(
-    column_name: str, dataset: pd.DataFrame, columns: List[str]
-) -> Dict[str, ColumnCorrelations]:
+def calculate_category_correlation(
+    column_display_name: str,
+    column: pd.Series,
+    features: pd.DataFrame,
+) -> List[ColumnCorrelations]:
     """For category columns calculate cramer_v correlation"""
-    if dataset[column_name].empty:
-        return {}
+    if column.empty or features.empty:
+        return []
 
-    if not columns:
-        return {}
-
-    correlation = calculate_cramer_v_correlation(column_name, dataset, columns)
-
-    if pd.isnull(correlation.values.y).all():
-        return {}
-
-    else:
-        return {correlation.kind: correlation}
-
-
-def calculate_numerical_column_correlations(
-    column_name: str, dataset: pd.DataFrame, columns: List[str]
-) -> Dict[str, ColumnCorrelations]:
-    if dataset[column_name].empty or not columns:
-        return {}
+    result_x = []
+    result_y = []
 
-    if not columns:
-        return {}
+    for feature_name in features.columns:
+        result_x.append(feature_name)
+        result_y.append(_cramer_v(column, features[feature_name]))
+
+    return [
+        ColumnCorrelations(
+            column_name=column_display_name,
+            kind="cramer_v",
+            values=Distribution(x=result_x, y=result_y),
+        ),
+    ]
+
+
+def calculate_numerical_correlation(
+    column_display_name: str,
+    column: pd.Series,
+    features: pd.DataFrame,
+) -> List[ColumnCorrelations]:
+    if column.empty or features.empty:
+        return []
 
-    result: Dict[str, ColumnCorrelations] = {}
-    column = dataset[column_name]
+    result = []
 
     for kind in ["pearson", "spearman", "kendall"]:
         correlations_columns = []
         correlations_values = []
 
-        for other_column_name in columns:
+        for other_column_name in features.columns:
             correlations_columns.append(other_column_name)
-            correlations_values.append(column.corr(dataset[other_column_name], method=kind))
+            correlations_values.append(column.corr(features[other_column_name], method=kind))
 
-        result[kind] = ColumnCorrelations(
-            column_name=column_name,
-            kind=kind,
-            values=Distribution(x=correlations_columns, y=correlations_values),
+        result.append(
+            ColumnCorrelations(
+                column_name=column_display_name,
+                kind=kind,
+                values=Distribution(x=correlations_columns, y=correlations_values),
+            )
         )
 
     return result
 
 
 def calculate_column_distribution(column: pd.Series, column_type: str) -> ColumnDistribution:
     if column.empty:
```

### Comparing `evidently-0.2.8/src/evidently/calculations/regression_performance.py` & `evidently-0.3.0/src/evidently/calculations/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/__init__.py` & `evidently-0.3.0/src/evidently/calculations/stattests/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/anderson_darling_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/anderson_darling_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/chisquare_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/chisquare_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/cramer_von_mises_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/cramer_von_mises_stattest.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from scipy.special import kv
 from scipy.stats import rankdata
 
 from evidently.calculations.stattests.registry import StatTest
 from evidently.calculations.stattests.registry import register_stattest
 
 
-def _all_partitions(nx: int, ny: int) -> Generator[Tuple[int, int], None, None]:
+def _all_partitions(nx: int, ny: int) -> Generator[Tuple[np.ndarray, np.ndarray], None, None]:
     """
     Args:
         nx: int
         ny: int
     Return:
         None
     """
@@ -89,33 +89,33 @@
 def _cdf_cvm_inf(x: float) -> float:
     """Calculate the cdf of the Cramér-von Mises statistic
     Args:
         x: float
     Returns:
         tot: float
     """
-    x = np.asarray(x)
+    x_array = np.asarray(x)
 
     def term(x, k):
         u = np.exp(gammaln(k + 0.5) - gammaln(k + 1)) / (np.pi**1.5 * np.sqrt(x))
         y = 4 * k + 1
         q = y**2 / (16 * x)
         b = kv(0.25, q)
         return u * np.sqrt(y) * np.exp(-q) * b
 
-    tot = np.zeros_like(x, dtype="float")
-    cond = np.ones_like(x, dtype="bool")
+    tot = np.zeros_like(x_array, dtype="float")
+    cond = np.ones_like(x_array, dtype="bool")
     k = 0
     while np.any(cond):
-        z = term(x[cond], k)  # type: ignore
+        z = term(x_array[cond], k)  # type: ignore
         tot[cond] = tot[cond] + z
         cond[cond] = np.abs(z) >= 1e-7
         k += 1
 
-    return tot
+    return tot[0]
 
 
 def _cvm_2samp(x: np.ndarray, y: np.ndarray, method: str = "auto") -> CramerVonMisesResult:
     """Perform the two-sample Cramér-von Mises test
     Args:
         x : array_like
         y : array_like
@@ -167,15 +167,15 @@
         vt = vt / (45 * N**2 * 4 * k)  # type: ignore
 
         tn = 1 / 6 + (t - et) / np.sqrt(45 * vt)
 
         if tn < 0.003:
             p = 1.0
         else:
-            p = max(0, 1.0 - _cdf_cvm_inf(tn))
+            p = max(0.0, 1.0 - _cdf_cvm_inf(tn))
 
     return CramerVonMisesResult(statistic=t, pvalue=p)
 
 
 def _cramer_von_mises(
     reference_data: pd.Series,
     current_data: pd.Series,
@@ -188,15 +188,15 @@
         current_data: current data
         feature_type: feature type
         threshold: level of significance
     Returns:
         p_value: p-value
         test_result: whether the drift is detected
     """
-    res = _cvm_2samp(reference_data, current_data)
+    res = _cvm_2samp(reference_data.values, current_data.values)
     return res.pvalue, res.pvalue <= threshold
 
 
 cramer_von_mises = StatTest(
     name="cramer_von_mises",
     display_name="Cramer-Von-mises",
     func=_cramer_von_mises,
```

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/energy_distance.py` & `evidently-0.3.0/src/evidently/calculations/stattests/energy_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/epps_singleton_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/epps_singleton_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/fisher_exact_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/fisher_exact_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/g_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/g_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/hellinger_distance.py` & `evidently-0.3.0/src/evidently/calculations/stattests/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/jensenshannon.py` & `evidently-0.3.0/src/evidently/calculations/stattests/jensenshannon.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/kl_div.py` & `evidently-0.3.0/src/evidently/calculations/stattests/kl_div.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/ks_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/ks_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/mmd_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/mmd_stattest.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,24 @@
 def sigma_median(dist: np.ndarray) -> float:
     """Calculate the median sigma
     Args:
         dist: pairwise distance result
     Returns:
         sigma: the median sigma
     """
-    sigma = (0.5 * np.percentile(dist.flatten(), 50, interpolation="nearest")) ** 0.5
+    sigma = (
+        0.5
+        * np.percentile(
+            # error: No overload variant of "percentile" matches argument types
+            # "ndarray[Any, Any]", "int", "str"  [call-overload]
+            a=dist.flatten(),
+            q=50,
+            interpolation="nearest",  # type: ignore[call-overload]
+        )
+    ) ** 0.5
     if sigma == 0:
         return (0.5 * 1) ** 0.5
     return sigma
 
 
 def rbf(x: np.ndarray, y: np.ndarray, pass_sigma: Optional[float]) -> Tuple[np.ndarray, float]:
     """compute the RBF kernel
```

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/psi.py` & `evidently-0.3.0/src/evidently/calculations/stattests/psi.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/registry.py` & `evidently-0.3.0/src/evidently/calculations/stattests/registry.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/t_test.py` & `evidently-0.3.0/src/evidently/calculations/stattests/t_test.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/text_content_drift.py` & `evidently-0.3.0/src/evidently/calculations/stattests/text_content_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/tvd_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/tvd_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/utils.py` & `evidently-0.3.0/src/evidently/calculations/stattests/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/wasserstein_distance_norm.py` & `evidently-0.3.0/src/evidently/calculations/stattests/wasserstein_distance_norm.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/stattests/z_stattest.py` & `evidently-0.3.0/src/evidently/calculations/stattests/z_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/calculations/utils.py` & `evidently-0.3.0/src/evidently/calculations/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/cat_target_pred_feature_table_widget.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/regression_quality.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,294 +1,312 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-import json
+import dataclasses
+from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Union
 
+import numpy as np
 import pandas as pd
-import plotly.express as px
-
-from evidently import ColumnMapping
-from evidently.analyzers.cat_target_drift_analyzer import CatTargetDriftAnalyzer
-from evidently.dashboard.widgets.utils import CutQuantileTransformer
-from evidently.dashboard.widgets.widget import Widget
-from evidently.model.widget import AdditionalGraphInfo
+from sklearn.metrics import mean_absolute_error
+from sklearn.metrics import mean_absolute_percentage_error
+from sklearn.metrics import mean_squared_error
+from sklearn.metrics import r2_score
+
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.calculations.regression_performance import calculate_regression_performance
+from evidently.metric_results import DatasetColumns
+from evidently.metric_results import Histogram
+from evidently.metrics.regression_performance.objects import RegressionMetricScatter
+from evidently.metrics.regression_performance.objects import RegressionMetricsScatter
+from evidently.metrics.regression_performance.regression_performance_metrics import RegressionMetrics
+from evidently.metrics.regression_performance.utils import apply_func_to_binned_data
+from evidently.metrics.utils import make_target_bins_for_reg_plots
 from evidently.model.widget import BaseWidgetInfo
-from evidently.options import QualityMetricsOptions
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import CounterData
+from evidently.renderers.html_widgets import counter
+from evidently.renderers.html_widgets import header_text
+from evidently.utils.data_operations import process_columns
+from evidently.utils.visualizations import make_hist_for_cat_plot
+from evidently.utils.visualizations import make_hist_for_num_plot
+
+
+class MoreRegressionMetrics(RegressionMetrics):
+    error_std: float
+    abs_error_std: float
+    abs_perc_error_std: float
+
+
+class RegressionQualityMetricResults(MetricResult):
+    class Config:
+        dict_exclude_fields = {"hist_for_plot", "vals_for_plots", "me_hist_for_plot"}
+        pd_exclude_fields = {"hist_for_plot", "vals_for_plots", "me_hist_for_plot"}
+
+    columns: DatasetColumns
+    current: MoreRegressionMetrics
+    reference: Optional[MoreRegressionMetrics]
+    rmse_default: float
+    me_default_sigma: float
+    me_hist_for_plot: Histogram
+    mean_abs_error_default: float
+    mean_abs_perc_error_default: float
+    abs_error_max_default: float
+    error_normality: dict
+    hist_for_plot: Histogram
+    vals_for_plots: RegressionMetricsScatter
+    error_bias: Optional[dict] = None
+
+
+class RegressionQualityMetric(Metric[RegressionQualityMetricResults]):
+    def calculate(self, data: InputData) -> RegressionQualityMetricResults:
+        dataset_columns = process_columns(data.current_data, data.column_mapping)
+        target_name = dataset_columns.utility_columns.target
+        prediction_name = dataset_columns.utility_columns.prediction
+
+        if target_name is None or prediction_name is None:
+            raise ValueError("The columns 'target' and 'prediction' columns should be present")
+        if not isinstance(prediction_name, str):
+            raise ValueError("Expect one column for prediction. List of columns was provided.")
+        current_metrics = calculate_regression_performance(
+            dataset=data.current_data,
+            columns=dataset_columns,
+            error_bias_prefix="current_",
+        )
+        error_bias = current_metrics.error_bias
+        reference_metrics = None
 
+        if data.reference_data is not None:
+            ref_columns = process_columns(data.reference_data, data.column_mapping)
+            reference_metrics = calculate_regression_performance(
+                dataset=data.reference_data,
+                columns=ref_columns,
+                error_bias_prefix="ref_",
+            )
 
-class CatTargetPredFeatureTable(Widget):
-    @staticmethod
-    def _get_rows_per_page(columns) -> int:
-        return min(len(columns.num_feature_names) + len(columns.cat_feature_names), 10)
-
-    def analyzers(self):
-        return [CatTargetDriftAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-
-        results = CatTargetDriftAnalyzer.get_results(analyzers_results)
-        quality_metrics_options = self.options_provider.get(QualityMetricsOptions)
-        cut_quantile = quality_metrics_options.cut_quantile
-
-        if current_data is None:
-            raise ValueError("current_data should be present")
-
-        target_name = results.columns.utility_columns.target
-        prediction_name = None
-        if results.prediction_metrics:
-            prediction_name = results.prediction_metrics.column_name
-
-        if prediction_name is not None and target_name is not None:
-            additional_graphs_data = []
-            params_data = []
-            for feature_name in results.columns.get_all_features_list(
-                cat_before_num=False
-            ):
-                # add data for table in params
-                params_data.append(
-                    {
-                        "details": {
-                            "parts": [
-                                {
-                                    "title": "Target",
-                                    "id": feature_name + "_target_values",
-                                },
-                                {
-                                    "title": "Prediction",
-                                    "id": feature_name + "_prediction_values",
-                                },
-                            ],
-                            "insights": [],
-                        },
-                        "f1": feature_name,
-                    }
-                )
-
-                # create target plot
-                reference_data["dataset"] = "Reference"
-                current_data["dataset"] = "Current"
-                quantile = quality_metrics_options.get_cut_quantile(feature_name)
-                if cut_quantile and quantile is not None:
-                    side, q = quantile
-                    cqt = CutQuantileTransformer(side=side, q=q)
-                    cqt.fit(reference_data[feature_name])
-                    reference_data_to_plot = cqt.transform_df(
-                        reference_data, feature_name
-                    )
-                    current_data_to_plot = cqt.transform_df(current_data, feature_name)
-                else:
-                    reference_data_to_plot = reference_data
-                    current_data_to_plot = current_data
-                merged_data = pd.concat([reference_data_to_plot, current_data_to_plot])
-
-                target_fig = px.histogram(
-                    merged_data,
-                    x=feature_name,
-                    color=target_name,
-                    facet_col="dataset",
-                    barmode="overlay",
-                    category_orders={"dataset": ["Reference", "Current"]},
-                )
-
-                target_fig_json = json.loads(target_fig.to_json())
-
-                # create prediction plot
-                pred_fig = px.histogram(
-                    merged_data,
-                    x=feature_name,
-                    color=prediction_name,
-                    facet_col="dataset",
-                    barmode="overlay",
-                    category_orders={"dataset": ["Reference", "Current"]},
-                )
-
-                pred_fig_json = json.loads(pred_fig.to_json())
-
-                # write plot data in table as additional data
-                additional_graphs_data.append(
-                    AdditionalGraphInfo(
-                        feature_name + "_target_values",
-                        {
-                            "data": target_fig_json["data"],
-                            "layout": target_fig_json["layout"],
-                        },
-                    )
-                )
-
-                additional_graphs_data.append(
-                    AdditionalGraphInfo(
-                        feature_name + "_prediction_values",
-                        {
-                            "data": pred_fig_json["data"],
-                            "layout": pred_fig_json["layout"],
-                        },
-                    )
-                )
-
-            return BaseWidgetInfo(
-                title=self.title,
-                type="big_table",
-                size=2,
-                params={
-                    "rowsPerPage": self._get_rows_per_page(results.columns),
-                    "columns": [{"title": "Feature", "field": "f1"}],
-                    "data": params_data,
-                },
-                additionalGraphs=additional_graphs_data,
+            if reference_metrics is not None and reference_metrics.error_bias:
+                for feature_name, current_bias in reference_metrics.error_bias.items():
+                    if feature_name in error_bias:
+                        error_bias[feature_name].update(current_bias)
+
+                    else:
+                        error_bias[feature_name] = current_bias
+
+        r2_score_value = r2_score(
+            y_true=data.current_data[target_name],
+            y_pred=data.current_data[prediction_name],
+        )
+        rmse_score_value = mean_squared_error(
+            y_true=data.current_data[target_name],
+            y_pred=data.current_data[prediction_name],
+        )
+
+        # mae default values
+        dummy_preds = data.current_data[target_name].median()
+        mean_abs_error_default = mean_absolute_error(
+            y_true=data.current_data[target_name],
+            y_pred=[dummy_preds] * data.current_data.shape[0],
+        )
+        # rmse default values
+        rmse_ref = None
+        if data.reference_data is not None:
+            rmse_ref = mean_squared_error(
+                y_true=data.reference_data[target_name],
+                y_pred=data.reference_data[prediction_name],
+            )
+        dummy_preds = data.current_data[target_name].mean()
+        rmse_default = mean_squared_error(
+            y_true=data.current_data[target_name],
+            y_pred=[dummy_preds] * data.current_data.shape[0],
+        )
+        # mape default values
+        # optimal constant for mape
+        s = data.current_data[target_name]
+        inv_y = 1 / s[s != 0].values
+        w = inv_y / sum(inv_y)
+        idxs = np.argsort(w)
+        sorted_w = w[idxs]
+        sorted_w_cumsum = np.cumsum(sorted_w)
+        idx = np.where(sorted_w_cumsum > 0.5)[0][0]
+        pos = idxs[idx]
+        dummy_preds = s[s != 0].values[pos]
+
+        mean_abs_perc_error_default = (
+            mean_absolute_percentage_error(
+                y_true=data.current_data[target_name],
+                y_pred=[dummy_preds] * data.current_data.shape[0],
+            )
+            * 100
+        )
+        #  r2_score default values
+        r2_score_ref = None
+        if data.reference_data is not None:
+            r2_score_ref = r2_score(
+                y_true=data.reference_data[target_name],
+                y_pred=data.reference_data[prediction_name],
             )
+        # max error default values
+        abs_error_max_ref = None
+        mean_error_ref = None
+
+        if reference_metrics is not None:
+            abs_error_max_ref = reference_metrics.abs_error_max
+            mean_error_ref = reference_metrics.mean_error
+
+        y_true = data.current_data[target_name]
+        y_pred = data.current_data[prediction_name]
+        abs_error_max_default = np.abs(y_true - y_true.median()).max()
 
-        if target_name is not None:
-            additional_graphs_data = []
-            params_data = []
-
-            for feature_name in results.columns.get_all_features_list(
-                cat_before_num=False
-            ):
-                # add data for table in params
-                params_data.append(
-                    {
-                        "details": {
-                            "parts": [
-                                {
-                                    "title": "Target",
-                                    "id": feature_name + "_target_values",
-                                }
-                            ],
-                            "insights": [],
-                        },
-                        "f1": feature_name,
-                    }
-                )
-
-                # create target plot
-                # TO DO%: out pf the cycle
-                reference_data["dataset"] = "Reference"
-                current_data["dataset"] = "Current"
-                quantile = quality_metrics_options.get_cut_quantile(feature_name)
-                if cut_quantile and quantile is not None:
-                    side, q = quantile
-                    cqt = CutQuantileTransformer(side=side, q=q)
-                    cqt.fit(reference_data[feature_name])
-                    reference_data_to_plot = cqt.transform_df(
-                        reference_data, feature_name
-                    )
-                    current_data_to_plot = cqt.transform_df(current_data, feature_name)
-                else:
-                    reference_data_to_plot = reference_data
-                    current_data_to_plot = current_data
-                merged_data = pd.concat([reference_data_to_plot, current_data_to_plot])
-
-                target_fig = px.histogram(
-                    merged_data,
-                    x=feature_name,
-                    color=target_name,
-                    facet_col="dataset",
-                    barmode="overlay",
-                    category_orders={"dataset": ["Reference", "Current"]},
-                )
-
-                target_fig_json = json.loads(target_fig.to_json())
-
-                # write plot data in table as additional data
-                additional_graphs_data.append(
-                    AdditionalGraphInfo(
-                        feature_name + "_target_values",
-                        {
-                            "data": target_fig_json["data"],
-                            "layout": target_fig_json["layout"],
-                        },
-                    )
-                )
-
-            return BaseWidgetInfo(
-                title=self.title,
-                type="big_table",
-                size=2,
-                params={
-                    "rowsPerPage": self._get_rows_per_page(results.columns),
-                    "columns": [{"title": "Feature", "field": "f1"}],
-                    "data": params_data,
-                },
-                additionalGraphs=additional_graphs_data,
+        #  me default values
+        me_default_sigma = (y_pred - y_true).std()
+
+        # visualisation
+
+        df_target_binned = make_target_bins_for_reg_plots(
+            data.current_data, target_name, prediction_name, data.reference_data
+        )
+        curr_target_bins = df_target_binned.loc[df_target_binned.data == "curr", "target_binned"]
+        ref_target_bins = None
+        if data.reference_data is not None:
+            ref_target_bins = df_target_binned.loc[df_target_binned.data == "ref", "target_binned"]
+        hist_for_plot = make_hist_for_cat_plot(curr_target_bins, ref_target_bins)
+
+        vals_for_plots: Dict[str, RegressionMetricScatter] = {}
+
+        if data.reference_data is not None:
+            is_ref_data = True
+
+        else:
+            is_ref_data = False
+
+        for name, func in zip(
+            ["r2_score", "rmse", "mean_abs_error", "mean_abs_perc_error"],
+            [
+                r2_score,
+                mean_squared_error,
+                mean_absolute_error,
+                mean_absolute_percentage_error,
+            ],
+        ):
+            vals_for_plots[name] = apply_func_to_binned_data(
+                df_target_binned, func, target_name, prediction_name, is_ref_data
             )
-        if results.columns.utility_columns.prediction is not None:
-            additional_graphs_data = []
-            params_data = []
-            for feature_name in (
-                results.columns.num_feature_names + results.columns.cat_feature_names
-            ):
-                # add data for table in params
-                params_data.append(
-                    {
-                        "details": {
-                            "parts": [
-                                {
-                                    "title": "Prediction",
-                                    "id": feature_name + "_prediction_values",
-                                }
-                            ],
-                            "insights": [],
-                        },
-                        "f1": feature_name,
-                    }
-                )
-
-                # create target plot
-                reference_data["dataset"] = "Reference"
-                current_data["dataset"] = "Current"
-                quantile = quality_metrics_options.get_cut_quantile(feature_name)
-                if cut_quantile and quantile is not None:
-                    side, q = quantile
-                    cqt = CutQuantileTransformer(side=side, q=q)
-                    cqt.fit(reference_data[feature_name])
-                    reference_data_to_plot = cqt.transform_df(
-                        reference_data, feature_name
-                    )
-                    current_data_to_plot = cqt.transform_df(current_data, feature_name)
-                else:
-                    reference_data_to_plot = reference_data
-                    current_data_to_plot = current_data
-                merged_data = pd.concat([reference_data_to_plot, current_data_to_plot])
-
-                prediction_fig = px.histogram(
-                    merged_data,
-                    x=feature_name,
-                    barmode="overlay",
-                    color=results.columns.utility_columns.prediction,
-                    facet_col="dataset",
-                    category_orders={"dataset": ["Reference", "Current"]},
-                )
-
-                prediction_fig_json = json.loads(prediction_fig.to_json())
-
-                # write plot data in table as additional data
-                additional_graphs_data.append(
-                    AdditionalGraphInfo(
-                        feature_name + "_prediction_values",
-                        {
-                            "data": prediction_fig_json["data"],
-                            "layout": prediction_fig_json["layout"],
-                        },
-                    )
-                )
-
-            return BaseWidgetInfo(
-                title=self.title,
-                type="big_table",
-                size=2,
-                params={
-                    "rowsPerPage": self._get_rows_per_page(results.columns),
-                    "columns": [{"title": "Feature", "field": "f1"}],
-                    "data": params_data,
-                },
-                additionalGraphs=additional_graphs_data,
+
+        # me plot
+        err_curr = data.current_data[prediction_name] - data.current_data[target_name]
+        err_ref = None
+
+        if is_ref_data:
+            err_ref = data.reference_data[prediction_name] - data.reference_data[target_name]
+        me_hist_for_plot = make_hist_for_num_plot(err_curr, err_ref)
+
+        if r2_score_ref is not None:
+            r2_score_ref = float(r2_score_ref)
+
+        if rmse_ref is not None:
+            rmse_ref = float(rmse_ref)
+
+        underperformance_ref = None
+
+        if reference_metrics is not None:
+            underperformance_ref = reference_metrics.underperformance
+
+        reference = None
+        if reference_metrics is not None:
+            reference = MoreRegressionMetrics(
+                mean_error=mean_error_ref,
+                underperformance=underperformance_ref,
+                mean_abs_error=reference_metrics.mean_abs_error,
+                mean_abs_perc_error=reference_metrics.mean_abs_perc_error,
+                error_std=reference_metrics.error_std,
+                abs_error_std=reference_metrics.abs_error_std,
+                abs_perc_error_std=reference_metrics.abs_perc_error_std,
+                rmse=rmse_ref,
+                r2_score=r2_score_ref,
+                abs_error_max=abs_error_max_ref,
             )
-        raise ValueError(
-            f"Widget {self.title} require 'prediction' or 'target' columns not to be None"
+
+        return RegressionQualityMetricResults(
+            columns=dataset_columns,
+            current=MoreRegressionMetrics(
+                r2_score=r2_score_value,
+                rmse=rmse_score_value,
+                mean_error=current_metrics.mean_error,
+                mean_abs_error=current_metrics.mean_abs_error,
+                mean_abs_perc_error=current_metrics.mean_abs_perc_error,
+                abs_error_max=current_metrics.abs_error_max,
+                error_std=current_metrics.error_std,
+                abs_error_std=current_metrics.abs_error_std,
+                abs_perc_error_std=current_metrics.abs_perc_error_std,
+                underperformance=current_metrics.underperformance,
+            ),
+            reference=reference,
+            rmse_default=rmse_default,
+            me_default_sigma=me_default_sigma,
+            me_hist_for_plot=me_hist_for_plot,
+            mean_abs_error_default=mean_abs_error_default,
+            mean_abs_perc_error_default=mean_abs_perc_error_default,
+            abs_error_max_default=abs_error_max_default,
+            error_normality=current_metrics.error_normality,
+            hist_for_plot=hist_for_plot,
+            vals_for_plots=RegressionMetricsScatter(**vals_for_plots),
+            error_bias=error_bias,
         )
+
+
+@default_renderer(wrap_type=RegressionQualityMetric)
+class RegressionQualityMetricRenderer(MetricRenderer):
+    def render_html(self, obj: RegressionQualityMetric) -> List[BaseWidgetInfo]:
+        metric_result = obj.get_result()
+        target_name = metric_result.columns.utility_columns.target
+        result = [
+            header_text(label=f"Regression Model Performance. Target: '{target_name}’"),
+            counter(
+                title="Current: Model Quality (+/- std)",
+                counters=[
+                    CounterData(
+                        "ME",
+                        f"{round(metric_result.current.mean_error, 2)} ({round(metric_result.current.error_std, 2)})",
+                    ),
+                    CounterData(
+                        "MAE",
+                        f"{round(metric_result.current.mean_abs_error, 2)} ({round(metric_result.current.abs_error_std, 2)})",
+                    ),
+                    CounterData(
+                        "MAPE",
+                        (
+                            f"{round(metric_result.current.mean_abs_perc_error, 2)}"
+                            f" ({round(metric_result.current.abs_perc_error_std, 2)})"
+                        ),
+                    ),
+                ],
+            ),
+        ]
+        if metric_result.reference is not None:
+            result.append(
+                counter(
+                    title="Reference: Model Quality (+/- std)",
+                    counters=[
+                        CounterData(
+                            "ME",
+                            f"{round(metric_result.reference.mean_error, 2)} ({round(metric_result.reference.error_std, 2)})",
+                        ),
+                        CounterData(
+                            "MAE",
+                            (
+                                f"{round(metric_result.reference.mean_abs_error, 2)}"
+                                f" ({round(metric_result.reference.abs_error_std, 2)})"
+                            ),
+                        ),
+                        CounterData(
+                            "MAPE",
+                            (
+                                f"{round(metric_result.reference.mean_abs_perc_error, 2)}"
+                                f" ({round(metric_result.reference.abs_perc_error_std, 2)})"
+                            ),
+                        ),
+                    ],
+                ),
+            )
+        return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/class_quality_metrics_bar_widget.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/confusion_matrix_metric.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,79 @@
-#!/usr/bin/env python
-# coding: utf-8
+import dataclasses
+from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Union
 
-import pandas as pd
-
-from evidently import ColumnMapping
-from evidently.analyzers.classification_performance_analyzer import (
-    ClassificationPerformanceAnalyzer,
-)
-from evidently.dashboard.widgets.widget import Widget
+from evidently.base_metric import InputData
+from evidently.base_metric import MetricResult
+from evidently.calculations.classification_performance import calculate_matrix
+from evidently.metric_results import ConfusionMatrix
+from evidently.metrics.classification_performance.base_classification_metric import ThresholdClassificationMetric
 from evidently.model.widget import BaseWidgetInfo
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import header_text
+from evidently.renderers.html_widgets import plotly_figure
+from evidently.utils.visualizations import plot_conf_mtrx
+
+DEFAULT_THRESHOLD = 0.5
+
+
+class ClassificationConfusionMatrixResult(MetricResult):
+    current_matrix: ConfusionMatrix
+    reference_matrix: Optional[ConfusionMatrix]
+    target_names: Optional[Dict[Union[str, int], str]] = None
+
+
+class ClassificationConfusionMatrix(ThresholdClassificationMetric[ClassificationConfusionMatrixResult]):
+    probas_threshold: Optional[float]
+    k: Optional[Union[float, int]]
+
+    def __init__(self, probas_threshold: Optional[float] = None, k: Optional[Union[float, int]] = None):
+        super().__init__(probas_threshold=probas_threshold, k=k)
+
+    def calculate(self, data: InputData) -> ClassificationConfusionMatrixResult:
+        current_target_data, current_pred = self.get_target_prediction_data(data.current_data, data.column_mapping)
+        target_names = data.column_mapping.target_names
+        current_results = calculate_matrix(
+            current_target_data,
+            current_pred.predictions,
+            current_pred.labels,
+        )
 
-
-class ClassQualityMetricsBarWidget(Widget):
-    def __init__(self, title: str, dataset: str = "reference"):
-        super().__init__(title)
-        self.dataset = dataset  # reference or current
-
-    def analyzers(self):
-        return [ClassificationPerformanceAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-
-        results = ClassificationPerformanceAnalyzer.get_results(analyzers_results)
-        target_name = results.columns.utility_columns.target
-        prediction_name = results.columns.utility_columns.prediction
-
-        if target_name is None or prediction_name is None:
-            if self.dataset == "reference":
-                raise ValueError(
-                    f"Widget [{self.title}] requires 'target' and 'prediction' columns."
-                )
-            return None
-
-        if self.dataset == "current":
-            result_metrics = results.current_metrics
-
-        elif self.dataset == "reference":
-            result_metrics = results.reference_metrics
-
-            if not result_metrics:
-                raise ValueError(
-                    f"Widget [{self.title}] required 'reference' results from"
-                    f" {ClassificationPerformanceAnalyzer.__name__} but no data found"
-                )
-
-        else:
-            raise ValueError(
-                f"Widget [{self.title}] requires 'current' or 'reference' dataset value"
+        reference_results = None
+        if data.reference_data is not None:
+            ref_target_data, ref_pred = self.get_target_prediction_data(data.reference_data, data.column_mapping)
+
+            reference_results = calculate_matrix(
+                ref_target_data,
+                ref_pred.predictions,
+                ref_pred.labels,
             )
 
-        if result_metrics is None:
-            return None
-
-        # plot quality metrics bar
-        return BaseWidgetInfo(
-            title=self.title,
-            type="counter",
-            size=2,
-            params={
-                "counters": [
-                    {
-                        "value": str(round(result_metrics.accuracy, 3)),
-                        "label": "Accuracy",
-                    },
-                    {
-                        "value": str(round(result_metrics.precision, 3)),
-                        "label": "Precision",
-                    },
-                    {"value": str(round(result_metrics.recall, 3)), "label": "Recall"},
-                    {"value": str(round(result_metrics.f1, 3)), "label": "F1"},
-                ]
-            },
+        return ClassificationConfusionMatrixResult(
+            current_matrix=current_results,
+            reference_matrix=reference_results,
+            target_names=target_names,
         )
+
+
+@default_renderer(wrap_type=ClassificationConfusionMatrix)
+class ClassificationConfusionMatrixRenderer(MetricRenderer):
+    def render_html(self, obj: ClassificationConfusionMatrix) -> List[BaseWidgetInfo]:
+        metric_result = obj.get_result()
+        target_names = metric_result.target_names
+        curr_matrix = metric_result.current_matrix
+        ref_matrix = metric_result.reference_matrix
+        if target_names is not None:
+            curr_matrix.labels = [target_names[x] for x in curr_matrix.labels]
+            if ref_matrix is not None:
+                ref_matrix.labels = [target_names[x] for x in ref_matrix.labels]
+
+        fig = plot_conf_mtrx(curr_matrix, ref_matrix)
+        fig.for_each_xaxis(lambda axis: axis.update(title_text="Predicted Value"))
+        fig.update_layout(yaxis_title="Actual Value")
+        return [
+            header_text(label="Confusion Matrix"),
+            plotly_figure(figure=fig, title=""),
+        ]
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/data_drift_table_widget.py` & `evidently-0.3.0/src/evidently/metrics/data_drift/data_drift_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,353 +1,273 @@
-#!/usr/bin/env python
-# coding: utf-8
+from typing import Dict
 from typing import List
 from typing import Optional
 
-import numpy as np
-import pandas as pd
-import plotly.graph_objs as go
-
-from evidently import ColumnMapping
-from evidently.analyzers.data_drift_analyzer import DataDriftAnalyzer
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
 from evidently.calculations.data_drift import ColumnDataDriftMetrics
-from evidently.dashboard.widgets.utils import CutQuantileTransformer
-from evidently.dashboard.widgets.utils import fig_to_json
-from evidently.dashboard.widgets.widget import Widget
-from evidently.model.widget import AdditionalGraphInfo
+from evidently.calculations.data_drift import get_drift_for_columns
+from evidently.calculations.stattests import PossibleStatTestType
+from evidently.metric_results import DatasetColumns
 from evidently.model.widget import BaseWidgetInfo
-from evidently.options import ColorOptions
 from evidently.options import DataDriftOptions
-from evidently.options import QualityMetricsOptions
-
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import ColumnDefinition
+from evidently.renderers.html_widgets import ColumnType
+from evidently.renderers.html_widgets import RichTableDataRow
+from evidently.renderers.html_widgets import RowDetails
+from evidently.renderers.html_widgets import header_text
+from evidently.renderers.html_widgets import plotly_figure
+from evidently.renderers.html_widgets import rich_table_data
+from evidently.renderers.html_widgets import table_data
+from evidently.renderers.render_utils import get_distribution_plot_figure
+from evidently.utils.data_operations import process_columns
+from evidently.utils.visualizations import plot_scatter_for_data_drift
+
+
+class DataDriftTableResults(MetricResult):
+    class Config:
+        dict_exclude_fields = {"dataset_columns"}
+
+    number_of_columns: int
+    number_of_drifted_columns: int
+    share_of_drifted_columns: float
+    dataset_drift: bool
+    drift_by_columns: Dict[str, ColumnDataDriftMetrics]
+    dataset_columns: DatasetColumns
+
+
+class DataDriftTable(Metric[DataDriftTableResults]):
+    columns: Optional[List[str]]
+    options: DataDriftOptions
 
-def _generate_feature_params(name: str, data: ColumnDataDriftMetrics) -> dict:
-    if data.current.small_distribution is None or data.reference.small_distribution is None:
-        return {}
-
-    current_small_hist = data.current.small_distribution
-    ref_small_hist = data.reference.small_distribution
-    feature_type = data.column_type
-    drift_score = data.drift_score
-    distr_sim_test = "Detected" if data.drift_detected else "Not Detected"
-    parts = []
-
-    if data.column_type == "num":
-        parts.append({"title": "Data drift", "id": f"{name}_drift", "type": "widget"})
-
-    parts.append({"title": "Data distribution", "id": f"{name}_distr"})
-    return {
-        "details": {"parts": parts, "insights": []},
-        "f1": name,
-        "f6": feature_type,
-        "stattest_name": data.stattest_name,
-        "f3": {"x": list(ref_small_hist.x), "y": list(ref_small_hist.y)},
-        "f4": {"x": list(current_small_hist.x), "y": list(current_small_hist.y)},
-        "f2": distr_sim_test,
-        "f5": round(drift_score, 6),
-    }
-
-
-def _generate_additional_graph_num_feature(
-    name: str,
-    reference_data: pd.DataFrame,
-    current_data: pd.DataFrame,
-    date_column: Optional[str],
-    data_drift_options: DataDriftOptions,
-    quality_metrics_options: QualityMetricsOptions,
-    color_options: ColorOptions,
-) -> List[AdditionalGraphInfo]:
-    # plot distributions
-    conf_interval_n_sigmas = quality_metrics_options.conf_interval_n_sigmas
-    fig = go.Figure()
-    if data_drift_options.xbins and data_drift_options.xbins.get(name):
-        current_xbins = data_drift_options.xbins.get(name)
-        current_nbinsx = None
-    else:
-        current_xbins = None
-        current_nbinsx = data_drift_options.get_nbinsx(name)
-    quantiles = quality_metrics_options.get_cut_quantile(name)
-    if quantiles:
-        side, q = quantiles
-        cqt = CutQuantileTransformer(side=side, q=q)
-        cqt.fit(reference_data[name])
-        reference_data_to_plot = cqt.transform(reference_data[name])
-        current_data_to_plot = cqt.transform(current_data[name])
-    else:
-        reference_data_to_plot = reference_data[name]
-        current_data_to_plot = current_data[name]
-    fig.add_trace(
-        go.Histogram(
-            x=reference_data_to_plot,
-            marker_color=color_options.get_reference_data_color(),
-            opacity=0.6,
-            xbins=current_xbins,
-            nbinsx=current_nbinsx,
-            name="Reference",
-            histnorm="probability",
+    def __init__(
+        self,
+        columns: Optional[List[str]] = None,
+        stattest: Optional[PossibleStatTestType] = None,
+        cat_stattest: Optional[PossibleStatTestType] = None,
+        num_stattest: Optional[PossibleStatTestType] = None,
+        text_stattest: Optional[PossibleStatTestType] = None,
+        per_column_stattest: Optional[Dict[str, PossibleStatTestType]] = None,
+        stattest_threshold: Optional[float] = None,
+        cat_stattest_threshold: Optional[float] = None,
+        num_stattest_threshold: Optional[float] = None,
+        text_stattest_threshold: Optional[float] = None,
+        per_column_stattest_threshold: Optional[Dict[str, float]] = None,
+    ):
+        self.columns = columns
+        self.options = DataDriftOptions(
+            all_features_stattest=stattest,
+            cat_features_stattest=cat_stattest,
+            num_features_stattest=num_stattest,
+            text_features_stattest=text_stattest,
+            per_feature_stattest=per_column_stattest,
+            all_features_threshold=stattest_threshold,
+            cat_features_threshold=cat_stattest_threshold,
+            num_features_threshold=num_stattest_threshold,
+            text_features_threshold=text_stattest_threshold,
+            per_feature_threshold=per_column_stattest_threshold,
         )
-    )
 
-    fig.add_trace(
-        go.Histogram(
-            x=current_data_to_plot,
-            marker_color=color_options.get_current_data_color(),
-            opacity=0.6,
-            xbins=current_xbins,
-            nbinsx=current_nbinsx,
-            name="Current",
-            histnorm="probability",
-        )
-    )
-    fig.update_layout(
-        legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1),
-        xaxis_title=name,
-        yaxis_title="Share",
-    )
-
-    distr_figure = fig_to_json(fig)
-
-    # plot drift
-    reference_mean = np.mean(reference_data[name][np.isfinite(reference_data[name])])
-    reference_std = np.std(reference_data[name][np.isfinite(reference_data[name])], ddof=1)
-    x_title = "Timestamp" if date_column else "Index"
-
-    fig = go.Figure()
-
-    fig.add_trace(
-        go.Scattergl(
-            x=current_data[date_column] if date_column else current_data.index,
-            y=current_data[name],
-            mode="markers",
-            name="Current",
-            marker=dict(size=6, color=color_options.get_current_data_color()),
-        )
-    )
+    def get_parameters(self) -> tuple:
+        return None if self.columns is None else tuple(self.columns), self.options
 
-    if date_column:
-        # take the second value because of some plotly issues
-        x0 = current_data[date_column].sort_values().iloc[1]
-
-    else:
-        x0 = current_data.index.sort_values()[1]
-
-    fig.add_trace(
-        go.Scattergl(
-            x=[x0, x0],
-            y=[
-                reference_mean - conf_interval_n_sigmas * reference_std,
-                reference_mean + conf_interval_n_sigmas * reference_std,
-            ],
-            mode="markers",
-            name="Current",
-            marker=dict(size=0.01, color=color_options.non_visible_color, opacity=0.005),
-            showlegend=False,
+    def calculate(self, data: InputData) -> DataDriftTableResults:
+        if data.reference_data is None:
+            raise ValueError("Reference dataset should be present")
+
+        dataset_columns = process_columns(data.reference_data, data.column_mapping)
+        result = get_drift_for_columns(
+            current_data=data.current_data,
+            reference_data=data.reference_data,
+            data_drift_options=self.options,
+            dataset_columns=dataset_columns,
+            columns=self.columns,
+        )
+        return DataDriftTableResults(
+            number_of_columns=result.number_of_columns,
+            number_of_drifted_columns=result.number_of_drifted_columns,
+            share_of_drifted_columns=result.share_of_drifted_columns,
+            dataset_drift=result.dataset_drift,
+            drift_by_columns=result.drift_by_columns,
+            dataset_columns=result.dataset_columns,
         )
-    )
 
-    fig.update_layout(
-        xaxis_title=x_title,
-        yaxis_title=name,
-        showlegend=True,
-        legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1),
-        shapes=[
-            dict(
-                type="rect",
-                # x-reference is assigned to the x-values
-                xref="paper",
-                # y-reference is assigned to the plot paper [0,1]
-                yref="y",
-                x0=0,
-                y0=reference_mean - conf_interval_n_sigmas * reference_std,
-                x1=1,
-                y1=reference_mean + conf_interval_n_sigmas * reference_std,
-                fillcolor=color_options.fill_color,
-                opacity=0.5,
-                layer="below",
-                line_width=0,
-            ),
-            dict(
-                type="line",
-                name="Reference",
-                xref="paper",
-                yref="y",
-                x0=0,  # min(testset_agg_by_date.index),
-                y0=reference_mean,
-                x1=1,  # max(testset_agg_by_date.index),
-                y1=reference_mean,
-                line=dict(color=color_options.zero_line_color, width=3),
-            ),
-        ],
-    )
 
-    drift_figure = fig_to_json(fig)
+@default_renderer(wrap_type=DataDriftTable)
+class DataDriftTableRenderer(MetricRenderer):
+    def _generate_column_params(self, column_name: str, data: ColumnDataDriftMetrics) -> Optional[RichTableDataRow]:
+        details = RowDetails()
+        if data.column_type == "text":
+            if (
+                data.current.characteristic_examples is not None
+                and data.reference.characteristic_examples is not None
+                and data.current.characteristic_words is not None
+                and data.reference.characteristic_words is not None
+            ):
+                current_table_words = table_data(
+                    title="",
+                    column_names=["", ""],
+                    data=[[el, ""] for el in data.current.characteristic_words],
+                )
+                details.with_part("current: characteristic words", info=current_table_words)
+                reference_table_words = table_data(
+                    title="",
+                    column_names=["", ""],
+                    data=[[el, ""] for el in data.reference.characteristic_words],
+                )
+                details.with_part("reference: characteristic words", info=reference_table_words)
+                current_table_examples = table_data(
+                    title="",
+                    column_names=["", ""],
+                    data=[[el, ""] for el in data.current.characteristic_examples],
+                )
+                details.with_part("current: characteristic examples", info=current_table_examples)
+                reference_table_examples = table_data(
+                    title="",
+                    column_names=["", ""],
+                    data=[[el, ""] for el in data.reference.characteristic_examples],
+                )
+                details.with_part("reference: characteristic examples", info=reference_table_examples)
 
-    # add distributions data
-    return [
-        AdditionalGraphInfo(f"{name}_distr", {"data": distr_figure["data"], "layout": distr_figure["layout"]}),
-        AdditionalGraphInfo(
-            f"{name}_drift",
-            {
-                "title": "",
-                "size": 2,
-                "text": "",
-                "type": "big_graph",
-                "params": {"data": drift_figure["data"], "layout": drift_figure["layout"]},
-            },
-        ),
-    ]
-
-
-def _generate_additional_graph_cat_feature(
-    name: str, reference_data: pd.DataFrame, current_data: pd.DataFrame, color_options: ColorOptions
-) -> List[AdditionalGraphInfo]:
-    fig = go.Figure()
-    feature_ref_data = reference_data[name].dropna()
-    feature_cur_data = current_data[name].dropna()
-    reference_data_to_plot = list(reversed(list(map(list, zip(*feature_ref_data.value_counts().items())))))
-    current_data_to_plot = list(reversed(list(map(list, zip(*feature_cur_data.value_counts().items())))))
-    fig.add_trace(
-        go.Bar(
-            x=reference_data_to_plot[1],
-            y=reference_data_to_plot[0],
-            marker_color=color_options.get_reference_data_color(),
-            opacity=0.6,
-            name="Reference",
-        )
-    )
+            data_drift = "Detected" if data.drift_detected else "Not Detected"
 
-    fig.add_trace(
-        go.Bar(
-            x=current_data_to_plot[1],
-            y=current_data_to_plot[0],
-            marker_color=color_options.get_current_data_color(),
-            opacity=0.6,
-            name="Current",
-        )
-    )
-    fig.update_layout(
-        legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1),
-        xaxis_title=name,
-        yaxis_title="Share",
-    )
-
-    distr_figure = fig_to_json(fig)
-    return [AdditionalGraphInfo(f"{name}_distr", {"data": distr_figure["data"], "layout": distr_figure["layout"]})]
-
-
-class DataDriftTableWidget(Widget):
-    def analyzers(self):
-        return [DataDriftAnalyzer]
+            # tabs = [
+            #     TabData(title="Carent Dataset: characteristic WORDS", widget=current_table_words),
+            #     TabData(title="Reference Dataset: characteristic WORDS", widget=reference_table_words),
+            #     TabData(title="Carent Dataset: characteristic EXAMPLES", widget=current_table_examples),
+            #     TabData(title="Reference Dataset: characteristic EXAMPLES", widget=reference_table_examples),
+            # ]
+            return RichTableDataRow(
+                details=details,
+                fields={
+                    "column_name": column_name,
+                    "column_type": data.column_type,
+                    "stattest_name": data.stattest_name,
+                    # "reference_distribution": {},
+                    # "current_distribution": {},
+                    "data_drift": data_drift,
+                    "drift_score": round(data.drift_score, 6),
+                },
+            )
 
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-        color_options = self.options_provider.get(ColorOptions)
-        data_drift_results = DataDriftAnalyzer.get_results(analyzers_results)
-        all_features = data_drift_results.columns.get_all_features_list()
-        date_column = data_drift_results.columns.utility_columns.date
-        target_column = data_drift_results.columns.utility_columns.target
-        prediction_column = data_drift_results.columns.utility_columns.prediction
+        else:
+            if (
+                data.current.small_distribution is None
+                or data.reference.small_distribution is None
+                or data.current.distribution is None
+                or data.reference.distribution is None
+            ):
+                return None
+
+            current_small_hist = data.current.small_distribution
+            ref_small_hist = data.reference.small_distribution
+            data_drift = "Detected" if data.drift_detected else "Not Detected"
+            if data.column_type == "num" and data.scatter is not None:
+                scatter_fig = plot_scatter_for_data_drift(
+                    curr_y=data.scatter.scatter[data.column_name],
+                    curr_x=data.scatter.scatter[data.scatter.x_name],
+                    y0=data.scatter.plot_shape["y0"],
+                    y1=data.scatter.plot_shape["y1"],
+                    y_name=data.column_name,
+                    x_name=data.scatter.x_name,
+                    color_options=self.color_options,
+                )
+                scatter = plotly_figure(title="", figure=scatter_fig)
+                details.with_part("DATA DRIFT", info=scatter)
+            fig = get_distribution_plot_figure(
+                current_distribution=data.current.distribution,
+                reference_distribution=data.reference.distribution,
+                color_options=self.color_options,
+            )
+            distribution = plotly_figure(title="", figure=fig)
+            details.with_part("DATA DISTRIBUTION", info=distribution)
+            return RichTableDataRow(
+                details=details,
+                fields={
+                    "column_name": column_name,
+                    "column_type": data.column_type,
+                    "stattest_name": data.stattest_name,
+                    "reference_distribution": {
+                        "x": list(ref_small_hist.x),
+                        "y": list(ref_small_hist.y),
+                    },
+                    "current_distribution": {
+                        "x": list(current_small_hist.x),
+                        "y": list(current_small_hist.y),
+                    },
+                    "data_drift": data_drift,
+                    "drift_score": round(data.drift_score, 6),
+                },
+            )
 
-        if current_data is None:
-            raise ValueError("current_data should be present")
+    def render_html(self, obj: DataDriftTable) -> List[BaseWidgetInfo]:
+        results = obj.get_result()
+        color_options = self.color_options
+        target_column = results.dataset_columns.utility_columns.target
+        prediction_column = results.dataset_columns.utility_columns.prediction
 
         # set params data
         params_data = []
-        data_drift_options = self.options_provider.get(DataDriftOptions)
-        quality_metrics_options = self.options_provider.get(QualityMetricsOptions)
 
         # sort columns by drift score
-        df_for_sort = pd.DataFrame()
-        df_for_sort["features"] = all_features
-        df_for_sort["scores"] = [
-            data_drift_results.metrics.drift_by_columns[feature].drift_score for feature in all_features
-        ]
-        all_features = df_for_sort.sort_values("scores", ascending=False).features.tolist()
-        columns = []
-
+        all_columns = sorted(
+            results.drift_by_columns.keys(),
+            key=lambda x: results.drift_by_columns[x].drift_score,
+            reverse=True,
+        )
         # move target and prediction to the top of the table
-        if target_column:
+        columns = []
+        if target_column in all_columns:
             columns.append(target_column)
-
-            if target_column in all_features:
-                all_features.remove(target_column)
-
-        if prediction_column and isinstance(prediction_column, str):
+            all_columns.remove(target_column)
+        if isinstance(prediction_column, str) and prediction_column in all_columns:
             columns.append(prediction_column)
+            all_columns.remove(prediction_column)
 
-            if prediction_column in all_features:
-                all_features.remove(prediction_column)
+        columns = columns + all_columns
 
-        columns = columns + all_features
-
-        for feature_name in columns:
-            params_data.append(
-                _generate_feature_params(feature_name, data_drift_results.metrics.drift_by_columns[feature_name])
-            )
+        for column_name in columns:
+            column_params = self._generate_column_params(column_name, results.drift_by_columns[column_name])
 
-        # set additionalGraphs
-        additional_graphs_data = []
-        for feature_name in columns:
-            # plot distributions
-            if data_drift_results.metrics.drift_by_columns[feature_name].column_type == "num":
-                additional_graphs_data += _generate_additional_graph_num_feature(
-                    feature_name,
-                    reference_data,
-                    current_data,
-                    date_column,
-                    data_drift_options,
-                    quality_metrics_options,
-                    color_options,
-                )
-            elif data_drift_results.metrics.drift_by_columns[feature_name].column_type == "cat":
-                additional_graphs_data += _generate_additional_graph_cat_feature(
-                    feature_name, reference_data, current_data, color_options
-                )
-        n_drifted_features = data_drift_results.metrics.number_of_drifted_columns
-        dataset_drift = data_drift_results.metrics.dataset_drift
-        n_features = data_drift_results.metrics.number_of_columns
-        drift_share = data_drift_results.metrics.share_of_drifted_columns
-
-        title_prefix = (
-            f"Drift is detected for {drift_share * 100:.2f}% of features ({n_drifted_features}"
-            f" out of {n_features}). "
-        )
-        title_suffix = "Dataset Drift is detected." if dataset_drift else "Dataset Drift is NOT detected."
-
-        return BaseWidgetInfo(
-            title=title_prefix + title_suffix,
-            type="big_table",
-            details="",
-            alerts=[],
-            alertsPosition="row",
-            insights=[],
-            size=2,
-            params={
-                "rowsPerPage": min(n_features, 10),
-                "columns": [
-                    {"title": "Feature", "field": "f1"},
-                    {"title": "Type", "field": "f6"},
-                    {
-                        "title": "Reference Distribution",
-                        "field": "f3",
-                        "type": "histogram",
-                        "options": {"xField": "x", "yField": "y", "color": color_options.primary_color},
-                    },
-                    {
-                        "title": "Current Distribution",
-                        "field": "f4",
-                        "type": "histogram",
-                        "options": {"xField": "x", "yField": "y", "color": color_options.primary_color},
-                    },
-                    {"title": "Data Drift", "field": "f2"},
-                    {"title": "Stat Test", "field": "stattest_name"},
-                    {"title": "Drift Score", "field": "f5"},
+            if column_params is not None:
+                params_data.append(column_params)
+
+        drift_percents = round(results.share_of_drifted_columns * 100, 3)
+
+        return [
+            header_text(label="Data Drift Summary"),
+            rich_table_data(
+                title=f"Drift is detected for {drift_percents}% of columns "
+                f"({results.number_of_drifted_columns} out of {results.number_of_columns}).",
+                columns=[
+                    ColumnDefinition("Column", "column_name"),
+                    ColumnDefinition("Type", "column_type"),
+                    ColumnDefinition(
+                        "Reference Distribution",
+                        "reference_distribution",
+                        ColumnType.HISTOGRAM,
+                        options={
+                            "xField": "x",
+                            "yField": "y",
+                            "color": color_options.primary_color,
+                        },
+                    ),
+                    ColumnDefinition(
+                        "Current Distribution",
+                        "current_distribution",
+                        ColumnType.HISTOGRAM,
+                        options={
+                            "xField": "x",
+                            "yField": "y",
+                            "color": color_options.primary_color,
+                        },
+                    ),
+                    ColumnDefinition("Data Drift", "data_drift"),
+                    ColumnDefinition("Stat Test", "stattest_name"),
+                    ColumnDefinition("Drift Score", "drift_score"),
                 ],
-                "data": params_data,
-            },
-            additionalGraphs=additional_graphs_data,
-        )
+                data=params_data,
+            ),
+        ]
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/num_output_drift_widget.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/pr_curve_metric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,96 @@
-#!/usr/bin/env python
-# coding: utf-8
-
+import dataclasses
+from typing import List
 from typing import Optional
 
 import pandas as pd
-import plotly.figure_factory as ff
+from sklearn import metrics
 
-from evidently import ColumnMapping
-from evidently.analyzers.num_target_drift_analyzer import NumTargetDriftAnalyzer
-from evidently.dashboard.widgets.utils import CutQuantileTransformer
-from evidently.dashboard.widgets.utils import fig_to_json
-from evidently.dashboard.widgets.widget import Widget
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.calculations.classification_performance import get_prediction_data
+from evidently.metric_results import PRCurve
+from evidently.metric_results import PRCurveData
+from evidently.metric_results import PredictionData
 from evidently.model.widget import BaseWidgetInfo
-from evidently.options import ColorOptions
-from evidently.options import QualityMetricsOptions
-
-
-class NumOutputDriftWidget(Widget):
-    def __init__(self, title: str, kind: str = "target"):
-        super().__init__(title)
-        self.kind = kind  # target or prediction
-
-    def analyzers(self):
-        return [NumTargetDriftAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-        color_options = self.options_provider.get(ColorOptions)
-        results = NumTargetDriftAnalyzer.get_results(analyzers_results)
-        quality_metrics_options = self.options_provider.get(QualityMetricsOptions)
-        cut_quantile = quality_metrics_options.cut_quantile
-
-        if current_data is None:
-            raise ValueError("current_data should be present")
-
-        if self.kind == "target":
-            if results.columns.utility_columns.target is None:
-                return None
-
-            column_name = results.columns.utility_columns.target
-            metrics = results.target_metrics
-
-        elif self.kind == "prediction":
-            if results.columns.utility_columns.prediction is None:
-                return None
-
-            if not isinstance(results.columns.utility_columns.prediction, str):
-                raise ValueError(
-                    f"Widget [{self.title}] requires one str value for 'prediction' column"
-                )
-
-            column_name = results.columns.utility_columns.prediction
-            metrics = results.prediction_metrics
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import TabData
+from evidently.renderers.html_widgets import get_pr_rec_plot_data
+from evidently.renderers.html_widgets import header_text
+from evidently.renderers.html_widgets import widget_tabs
+from evidently.utils.data_operations import process_columns
+
+
+class ClassificationPRCurveResults(MetricResult):
+    current_pr_curve: Optional[PRCurve] = None
+    reference_pr_curve: Optional[PRCurve] = None
+
+
+class ClassificationPRCurve(Metric[ClassificationPRCurveResults]):
+    def calculate(self, data: InputData) -> ClassificationPRCurveResults:
+        dataset_columns = process_columns(data.current_data, data.column_mapping)
+        target_name = dataset_columns.utility_columns.target
+        prediction_name = dataset_columns.utility_columns.prediction
+        if target_name is None or prediction_name is None:
+            raise ValueError("The columns 'target' and 'prediction' columns should be present")
+        curr_predictions = get_prediction_data(data.current_data, dataset_columns, data.column_mapping.pos_label)
+        curr_pr_curve = self.calculate_metrics(data.current_data[target_name], curr_predictions)
+        ref_pr_curve = None
+        if data.reference_data is not None:
+            ref_predictions = get_prediction_data(data.reference_data, dataset_columns, data.column_mapping.pos_label)
+            ref_pr_curve = self.calculate_metrics(data.reference_data[target_name], ref_predictions)
+        return ClassificationPRCurveResults(
+            current_pr_curve=curr_pr_curve,
+            reference_pr_curve=ref_pr_curve,
+        )
 
-        else:
-            raise ValueError(
-                f"Widget [{self.title}] requires 'target' or 'prediction' kind parameter value"
+    def calculate_metrics(self, target_data: pd.Series, prediction: PredictionData) -> PRCurve:
+        labels = prediction.labels
+        if prediction.prediction_probas is None:
+            raise ValueError("PR Curve can be calculated only on binary probabilistic predictions")
+        binaraized_target = (target_data.values.reshape(-1, 1) == labels).astype(int)
+        pr_curve = {}
+        if len(labels) <= 2:
+            binaraized_target = pd.DataFrame(binaraized_target[:, 0])
+            binaraized_target.columns = ["target"]
+            pr, rcl, thrs = metrics.precision_recall_curve(binaraized_target, prediction.prediction_probas.iloc[:, 0])
+            pr_curve[prediction.prediction_probas.columns[0]] = PRCurveData(
+                pr=pr.tolist(),
+                rcl=rcl.tolist(),
+                thrs=thrs.tolist(),
             )
-
-        if metrics is None:
-            return None
-
-        # calculate output drift
-        stattest_name = metrics.stattest_name
-        drift_score = metrics.drift_score
-        drift_detected = metrics.drift_detected
-        output_sim_test = "detected" if drift_detected else "not detected"
-
-        # plot output distributions
-        quantile = quality_metrics_options.get_cut_quantile(column_name)
-        if cut_quantile and quantile is not None:
-            side, q = quantile
-            cqt = CutQuantileTransformer(side=side, q=q)
-            cqt.fit(reference_data[column_name])
-            reference_data_to_plot = cqt.transform(reference_data[column_name])
-            current_data_to_plot = cqt.transform(current_data[column_name])
         else:
-            reference_data_to_plot = reference_data[column_name]
-            current_data_to_plot = current_data[column_name]
-
-        output_distr = ff.create_distplot(
-            [reference_data_to_plot, current_data_to_plot],
-            ["Reference", "Current"],
-            colors=[
-                color_options.get_reference_data_color(),
-                color_options.get_current_data_color(),
-            ],
-            show_rug=True,
-        )
+            binaraized_target = pd.DataFrame(binaraized_target)
+            binaraized_target.columns = labels
+            for label in labels:
+
+                pr, rcl, thrs = metrics.precision_recall_curve(
+                    binaraized_target[label],
+                    prediction.prediction_probas[label],
+                )
 
-        output_distr.update_layout(
-            xaxis_title="Value",
-            yaxis_title="Share",
-            legend=dict(
-                orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1
-            ),
-        )
+                pr_curve[label] = PRCurveData(
+                    pr=pr.tolist(),
+                    rcl=rcl.tolist(),
+                    thrs=thrs.tolist(),
+                )
+        return pr_curve
 
-        # output_drift_json = json.loads(output_distr.to_json())
-        output_drift_json = fig_to_json(output_distr)
 
-        return BaseWidgetInfo(
-            title=f"{self.kind.title()} Drift: {output_sim_test},"
-            f" drift score={round(drift_score, 6)} ({stattest_name})",
-            type="big_graph",
-            details="",
-            alerts=[],
-            alertsPosition="row",
-            insights=[],
-            size=2,
-            params={
-                "data": output_drift_json["data"],
-                "layout": output_drift_json["layout"],
-            },
-            additionalGraphs=[],
-        )
+@default_renderer(wrap_type=ClassificationPRCurve)
+class ClassificationPRCurveRenderer(MetricRenderer):
+    def render_html(self, obj: ClassificationPRCurve) -> List[BaseWidgetInfo]:
+        current_pr_curve: Optional[PRCurve] = obj.get_result().current_pr_curve
+        reference_pr_curve: Optional[PRCurve] = obj.get_result().reference_pr_curve
+        if current_pr_curve is None:
+            return []
+
+        tab_data = get_pr_rec_plot_data(current_pr_curve, reference_pr_curve, color_options=self.color_options)
+        if len(tab_data) == 1:
+            return [header_text(label="Precision-Recall Curve"), tab_data[0][1]]
+        tabs = [TabData(name, widget) for name, widget in tab_data]
+        return [
+            header_text(label="Precision-Recall Curve"),
+            widget_tabs(title="", tabs=tabs),
+        ]
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/num_output_values_widget.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/error_normality.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,165 +1,138 @@
-#!/usr/bin/env python
-# coding: utf-8
-
+import dataclasses
 import json
+from typing import List
 from typing import Optional
+from typing import Union
 
 import numpy as np
-import pandas as pd
-import plotly.graph_objs as go
-
-from evidently import ColumnMapping
-from evidently.analyzers.num_target_drift_analyzer import NumTargetDriftAnalyzer
-from evidently.dashboard.widgets.widget import Widget
+from plotly import graph_objs as go
+from plotly.subplots import make_subplots
+from scipy.stats import probplot
+
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.metric_results import ScatterData
 from evidently.model.widget import BaseWidgetInfo
-from evidently.options import ColorOptions
-from evidently.options import QualityMetricsOptions
-
-
-class NumOutputValuesWidget(Widget):
-    def __init__(self, title: str, kind: str = "target"):
-        super().__init__(title)
-        self.title = title
-        self.kind = kind  # target or prediction
-
-    def analyzers(self):
-        return [NumTargetDriftAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-        color_options = self.options_provider.get(ColorOptions)
-        results = NumTargetDriftAnalyzer.get_results(analyzers_results)
-        quality_metrics_options = self.options_provider.get(QualityMetricsOptions)
-        conf_interval_n_sigmas = quality_metrics_options.conf_interval_n_sigmas
-
-        if current_data is None:
-            raise ValueError("current_data should be present")
-
-        if self.kind == "target":
-            if results.columns.utility_columns.target is None:
-                return None
-
-            column_name = results.columns.utility_columns.target
-
-        elif self.kind == "prediction":
-            if results.columns.utility_columns.prediction is None:
-                return None
-
-            if not isinstance(results.columns.utility_columns.prediction, str):
-                raise ValueError(
-                    f"Widget [{self.title}] requires one str value for 'prediction' column"
-                )
-
-            column_name = results.columns.utility_columns.prediction
-
-        else:
-            raise ValueError(
-                f"Widget [{self.title}] requires 'target' or 'prediction' kind parameter value"
-            )
-
-        utility_columns_date = results.columns.utility_columns.date
-        # plot values
-        reference_mean = np.mean(reference_data[column_name])
-        reference_std = np.std(reference_data[column_name], ddof=1)
-        x_title = "Timestamp" if utility_columns_date else "Index"
-
-        output_values = go.Figure()
-
-        output_values.add_trace(
-            go.Scattergl(
-                x=reference_data[utility_columns_date]
-                if utility_columns_date
-                else reference_data.index,
-                y=reference_data[column_name],
-                mode="markers",
-                name="Reference",
-                marker=dict(size=6, color=color_options.get_reference_data_color()),
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import header_text
+from evidently.utils.data_operations import process_columns
+
+
+class RegressionErrorNormalityResults(MetricResult):
+    class Config:
+        dict_exclude_fields = {"current_error", "reference_error"}
+        pd_exclude_fields = {"current_error", "reference_error"}
+
+    current_error: ScatterData
+    reference_error: Optional[ScatterData]
+
+
+class RegressionErrorNormality(Metric[RegressionErrorNormalityResults]):
+    def calculate(self, data: InputData) -> RegressionErrorNormalityResults:
+        dataset_columns = process_columns(data.current_data, data.column_mapping)
+        target_name = dataset_columns.utility_columns.target
+        prediction_name = dataset_columns.utility_columns.prediction
+        curr_df = data.current_data
+        ref_df = data.reference_data
+        if target_name is None or prediction_name is None:
+            raise ValueError("The columns 'target' and 'prediction' columns should be present")
+        if not isinstance(prediction_name, str):
+            raise ValueError("Expect one column for prediction. List of columns was provided.")
+        curr_df = self._make_df_for_plot(curr_df, target_name, prediction_name, None)
+        current_error = curr_df[prediction_name] - curr_df[target_name]
+        reference_error = None
+        if ref_df is not None:
+            ref_df = self._make_df_for_plot(ref_df, target_name, prediction_name, None)
+            reference_error = ref_df[prediction_name] - ref_df[target_name]
+        return RegressionErrorNormalityResults(current_error=current_error, reference_error=reference_error)
+
+    def _make_df_for_plot(self, df, target_name: str, prediction_name: str, datetime_column_name: Optional[str]):
+        result = df.replace([np.inf, -np.inf], np.nan)
+        if datetime_column_name is not None:
+            result.dropna(
+                axis=0,
+                how="any",
+                inplace=True,
+                subset=[target_name, prediction_name, datetime_column_name],
             )
+            return result.sort_values(datetime_column_name)
+        result.dropna(axis=0, how="any", inplace=True, subset=[target_name, prediction_name])
+        return result.sort_index()
+
+
+@default_renderer(wrap_type=RegressionErrorNormality)
+class RegressionErrorNormalityRenderer(MetricRenderer):
+    def render_html(self, obj: RegressionErrorNormality) -> List[BaseWidgetInfo]:
+        result = obj.get_result()
+        current_error = result.current_error
+        reference_error = result.reference_error
+        color_options = self.color_options
+        cols = 1
+        subplot_titles: Union[list, str] = ""
+
+        if reference_error is not None:
+            cols = 2
+            subplot_titles = ["current", "reference"]
+
+        fig = make_subplots(rows=1, cols=cols, shared_yaxes=False, subplot_titles=subplot_titles)
+        curr_qq_lines = probplot(current_error, dist="norm", plot=None)
+        curr_theoretical_q_x = np.linspace(curr_qq_lines[0][0][0], curr_qq_lines[0][0][-1], 100)
+        sample_quantile_trace = go.Scatter(
+            x=curr_qq_lines[0][0],
+            y=curr_qq_lines[0][1],
+            mode="markers",
+            name="Dataset Quantiles",
+            legendgroup="Dataset Quantiles",
+            marker=dict(size=6, color=color_options.primary_color),
         )
 
-        output_values.add_trace(
-            go.Scattergl(
-                x=current_data[utility_columns_date]
-                if utility_columns_date
-                else current_data.index,
-                y=current_data[column_name],
-                mode="markers",
-                name="Current",
-                marker=dict(size=6, color=color_options.get_current_data_color()),
-            )
+        theoretical_quantile_trace = go.Scatter(
+            x=curr_theoretical_q_x,
+            y=curr_qq_lines[1][0] * curr_theoretical_q_x + curr_qq_lines[1][1],
+            mode="lines",
+            name="Theoretical Quantiles",
+            legendgroup="Theoretical Quantiles",
+            marker=dict(size=6, color=color_options.secondary_color),
         )
-
-        if utility_columns_date:
-            x0 = current_data[utility_columns_date].sort_values()[1]
-        else:
-            x0 = current_data.index.sort_values()[1]
-
-        output_values.add_trace(
-            go.Scatter(
-                x=[x0, x0],
-                y=[
-                    reference_mean - conf_interval_n_sigmas * reference_std,
-                    reference_mean + conf_interval_n_sigmas * reference_std,
-                ],
+        fig.add_trace(sample_quantile_trace, 1, 1)
+        fig.add_trace(theoretical_quantile_trace, 1, 1)
+        fig.update_xaxes(title_text="Theoretical Quantiles", row=1, col=1)
+        if reference_error is not None:
+            ref_qq_lines = probplot(reference_error, dist="norm", plot=None)
+            ref_theoretical_q_x = np.linspace(ref_qq_lines[0][0][0], ref_qq_lines[0][0][-1], 100)
+            sample_quantile_trace = go.Scatter(
+                x=ref_qq_lines[0][0],
+                y=ref_qq_lines[0][1],
                 mode="markers",
-                name="Current",
-                marker=dict(
-                    size=0.01, color=color_options.non_visible_color, opacity=0.005
-                ),
+                name="Dataset Quantiles",
+                legendgroup="Dataset Quantiles",
                 showlegend=False,
+                marker=dict(size=6, color=color_options.primary_color),
             )
-        )
 
-        output_values.update_layout(
-            xaxis_title=x_title,
-            yaxis_title=self.kind.title() + " Value",
-            showlegend=True,
-            legend=dict(
-                orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1
+            theoretical_quantile_trace = go.Scatter(
+                x=ref_theoretical_q_x,
+                y=ref_qq_lines[1][0] * ref_theoretical_q_x + ref_qq_lines[1][1],
+                mode="lines",
+                name="Theoretical Quantiles",
+                legendgroup="Theoretical Quantiles",
+                showlegend=False,
+                marker=dict(size=6, color=color_options.secondary_color),
+            )
+            fig.add_trace(sample_quantile_trace, 1, 2)
+            fig.add_trace(theoretical_quantile_trace, 1, 2)
+            fig.update_xaxes(title_text="Theoretical Quantiles", row=1, col=2)
+        fig.update_layout(yaxis_title="Dataset Quantiles")
+        fig = json.loads(fig.to_json())
+
+        return [
+            header_text(label="Error Normality"),
+            BaseWidgetInfo(
+                title="",
+                size=2,
+                type="big_graph",
+                params={"data": fig["data"], "layout": fig["layout"]},
             ),
-            shapes=[
-                dict(
-                    type="rect",
-                    # x-reference is assigned to the x-values
-                    xref="paper",
-                    # y-reference is assigned to the plot paper [0,1]
-                    yref="y",
-                    x0=0,
-                    y0=reference_mean - conf_interval_n_sigmas * reference_std,
-                    x1=1,
-                    y1=reference_mean + conf_interval_n_sigmas * reference_std,
-                    fillcolor=color_options.fill_color,
-                    opacity=0.5,
-                    layer="below",
-                    line_width=0,
-                ),
-                dict(
-                    type="line",
-                    name="Reference",
-                    xref="paper",
-                    yref="y",
-                    x0=0,  # min(testset_agg_by_date.index),
-                    y0=reference_mean,
-                    x1=1,  # max(testset_agg_by_date.index),
-                    y1=reference_mean,
-                    line=dict(color=color_options.zero_line_color, width=3),
-                ),
-            ],
-        )
-
-        output_values_json = json.loads(output_values.to_json())
-
-        return BaseWidgetInfo(
-            title=self.title,
-            type="big_graph",
-            size=1,
-            params={
-                "data": output_values_json["data"],
-                "layout": output_values_json["layout"],
-            },
-        )
+        ]
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/num_target_pred_feature_table_widget.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/visualization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,142 +1,125 @@
-#!/usr/bin/env python
-# coding: utf-8
-
 import json
+from typing import Dict
 from typing import Optional
+from typing import Union
 
+import numpy as np
 import pandas as pd
-import plotly.graph_objs as go
+from plotly import graph_objs as go
 from plotly.subplots import make_subplots
 
-from evidently import ColumnMapping
-from evidently.analyzers.num_target_drift_analyzer import NumTargetDriftAnalyzer
-from evidently.dashboard.widgets.widget import Widget
-from evidently.model.widget import AdditionalGraphInfo
-from evidently.model.widget import BaseWidgetInfo
-from evidently.options import ColorOptions
-
-
-class NumTargetPredFeatureTable(Widget):
-    def analyzers(self):
-        return [NumTargetDriftAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-        color_options = self.options_provider.get(ColorOptions)
-        results = NumTargetDriftAnalyzer.get_results(analyzers_results)
-
-        if current_data is None:
-            raise ValueError("current_data should be present")
-
-        target_column = results.columns.utility_columns.target
-        prediction_column = results.columns.utility_columns.prediction
-
-        if target_column and prediction_column:
-            return None
-
-        additional_graphs_data = []
-        params_data = []
-
-        for feature_name in results.columns.get_all_features_list(cat_before_num=False):
-            # add data for table in params
-            params_data.append(
-                {
-                    "details": {
-                        "parts": [
-                            {"title": "Feature values", "id": feature_name + "_values"}
-                        ],
-                        "insights": [],
-                    },
-                    "f1": feature_name,
-                }
+from evidently.metric_results import Histogram
+from evidently.metrics.regression_performance.objects import RegressionMetricScatter
+from evidently.metrics.regression_performance.objects import RegressionScatter
+from evidently.options.color_scheme import ColorOptions
+
+
+def plot_error_bias_colored_scatter(
+    curr_scatter_data: RegressionScatter,
+    ref_scatter_data: Optional[RegressionScatter],
+    color_options: ColorOptions,
+):
+    cols = 1
+    subplot_titles: Union[list, str] = ""
+
+    if ref_scatter_data is not None:
+        cols = 2
+        subplot_titles = ["current", "reference"]
+
+    fig = make_subplots(rows=1, cols=cols, shared_yaxes=True, subplot_titles=subplot_titles)
+
+    for name, value, color in zip(
+        ["Underestimation", "Overestimation", "Majority"],
+        [curr_scatter_data.underestimation, curr_scatter_data.overestimation, curr_scatter_data.majority],
+        [color_options.underestimation_color, color_options.overestimation_color, color_options.majority_color],
+    ):
+        trace = go.Scatter(
+            x=value.actual,
+            y=value.predicted,
+            mode="markers",
+            name=name,
+            legendgroup=name,
+            marker_color=color
+            # marker=dict(color=color_options.underestimation_color, showscale=False),
+        )
+        fig.add_trace(trace, 1, 1)
+    fig.update_xaxes(title_text="Actual value", row=1, col=1)
+
+    if ref_scatter_data is not None:
+        for name, value, color in zip(
+            ["Underestimation", "Overestimation", "Majority"],
+            [ref_scatter_data.underestimation, ref_scatter_data.overestimation, ref_scatter_data.majority],
+            [color_options.underestimation_color, color_options.overestimation_color, color_options.majority_color],
+        ):
+            trace = go.Scatter(
+                x=value.actual,
+                y=value.predicted,
+                mode="markers",
+                name=name,
+                legendgroup=name,
+                showlegend=False,
+                marker_color=color
+                # marker=dict(color=color_options.underestimation_color, showscale=False),
             )
+            fig.add_trace(trace, 1, 2)
+        fig.update_xaxes(title_text="Actual value", row=1, col=2)
 
-            # create plot
-            fig = make_subplots(rows=1, cols=2, subplot_titles=("Reference", "Current"))
+    fig.update_layout(
+        yaxis_title="Predicted value",
+        xaxis=dict(showticklabels=True),
+        yaxis=dict(showticklabels=True),
+    )
+    fig = json.loads(fig.to_json())
+    return fig
+
+
+def regression_perf_plot(
+    *,
+    val_for_plot: RegressionMetricScatter,
+    hist_for_plot: Histogram,
+    name: str,
+    curr_metric: float,
+    ref_metric: float = None,
+    color_options: ColorOptions,
+):
+    current_color = color_options.get_current_data_color()
+    reference_color = color_options.get_reference_data_color()
+    fig = make_subplots(rows=2, cols=1, shared_xaxes=True)
+    # todo: better typing
+    assert isinstance(val_for_plot.current, pd.Series)
+    sorted_index = val_for_plot.current.sort_index()
+    x = [str(idx) for idx in sorted_index.index]
+    y = list(sorted_index)
+    trace = go.Scatter(x=x, y=y, mode="lines+markers", name=name, marker_color=current_color)
+    fig.add_trace(trace, 1, 1)
+
+    df = hist_for_plot.current.to_df().sort_values("x")
+    x = [str(x) for x in df.x]
+    y = list(df["count"])
+    trace = go.Bar(name="current", x=x, y=y, marker_color=current_color)
+    fig.add_trace(trace, 2, 1)
+
+    if hist_for_plot.reference is not None:
+        # todo: better typing
+        assert isinstance(val_for_plot.reference, pd.Series)
+        sorted_index = val_for_plot.reference.sort_index()
+        x = [str(idx) for idx in sorted_index.index]
+        y = list(sorted_index)
+        trace = go.Scatter(x=x, y=y, mode="lines+markers", name=name, marker_color=reference_color)
+        fig.add_trace(trace, 1, 1)
+
+        df = hist_for_plot.reference.to_df().sort_values("x")
+        x = [str(x) for x in df.x]
+        y = list(df["count"])
+        trace = go.Bar(name="reference", x=x, y=y, marker_color=reference_color)
+        fig.add_trace(trace, 2, 1)
+
+    fig.update_yaxes(title_text=name, row=1, col=1)
+    fig.update_yaxes(title_text="count", row=2, col=1)
+    title = f"current {name}: {np.round(curr_metric, 3)}"
 
-            if prediction_column is not None:
-                fig.add_trace(
-                    go.Scattergl(
-                        x=reference_data[feature_name],
-                        y=reference_data[prediction_column],
-                        mode="markers",
-                        name="Prediction (ref)",
-                        marker=dict(size=6, color=color_options.secondary_color),
-                    ),
-                    row=1,
-                    col=1,
-                )
-
-            if target_column is not None:
-                fig.add_trace(
-                    go.Scattergl(
-                        x=reference_data[feature_name],
-                        y=reference_data[target_column],
-                        mode="markers",
-                        name="Target (ref)",
-                        marker=dict(size=6, color=color_options.primary_color),
-                    ),
-                    row=1,
-                    col=1,
-                )
-
-            if prediction_column is not None:
-                fig.add_trace(
-                    go.Scatter(
-                        x=current_data[feature_name],
-                        y=current_data[prediction_column],
-                        mode="markers",
-                        name="Prediction (curr)",
-                        marker=dict(size=6, color=color_options.secondary_color),
-                    ),
-                    row=1,
-                    col=2,
-                )
-
-            if target_column is not None:
-                fig.add_trace(
-                    go.Scatter(
-                        x=current_data[feature_name],
-                        y=current_data[target_column],
-                        mode="markers",
-                        name="Target (curr)",
-                        marker=dict(size=6, color=color_options.primary_color),
-                    ),
-                    row=1,
-                    col=2,
-                )
-
-            # Update xaxis properties
-            fig.update_xaxes(title_text=feature_name, showgrid=True, row=1, col=1)
-            fig.update_xaxes(title_text=feature_name, showgrid=True, row=1, col=2)
-
-            # Update yaxis properties
-            fig.update_yaxes(title_text="Value", showgrid=True, row=1, col=1)
-            fig.update_yaxes(title_text="Value", showgrid=True, row=1, col=2)
-
-            fig_json = json.loads(fig.to_json())
-
-            # write plot data in table as additional data
-            additional_graphs_data.append(
-                AdditionalGraphInfo(
-                    feature_name + "_values",
-                    {"data": fig_json["data"], "layout": fig_json["layout"]},
-                )
-            )
+    if hist_for_plot.reference is not None:
+        title += f", reference {name}: {np.round(ref_metric, 3) if ref_metric is not None else '--'}"
 
-        return BaseWidgetInfo(
-            title=self.title,
-            type="big_table",
-            size=2,
-            params={
-                "rowsPerPage": min(results.columns.get_features_len(), 10),
-                "columns": [{"title": "Feature", "field": "f1"}],
-                "data": params_data,
-            },
-            additionalGraphs=additional_graphs_data,
-        )
+    fig.update_layout(title=title)
+    return fig
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/prob_class_confusion_based_feature_distr_table_widget.py` & `evidently-0.3.0/src/evidently/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,388 +1,493 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-import json
+from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
-import plotly.express as px
 import plotly.graph_objs as go
+from pandas.api.types import is_numeric_dtype
 from plotly.subplots import make_subplots
 
-from evidently import ColumnMapping
-from evidently.analyzers.prob_classification_performance_analyzer import (
-    ProbClassificationPerformanceAnalyzer,
-)
-from evidently.dashboard.widgets.utils import CutQuantileTransformer
-from evidently.dashboard.widgets.widget import Widget
-from evidently.model.widget import AdditionalGraphInfo
+from evidently.metric_results import Boxes
+from evidently.metric_results import RatesPlotData
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options import ColorOptions
-from evidently.options import QualityMetricsOptions
+from evidently.renderers.base_renderer import DetailsInfo
+from evidently.renderers.html_widgets import plotly_figure
+from evidently.renderers.html_widgets import table_data
+from evidently.utils.types import ApproxValue
+
+
+def plot_check(fig, condition, color_options: ColorOptions):
+    lines = []
+    left_line = pd.Series([condition.gt, condition.gte]).max()
+
+    if not pd.isnull(left_line):
+        left_line_name = ["gt", "gte"][pd.Series([condition.gt, condition.gte]).argmax()]
+        lines.append((left_line, left_line_name))
+
+    right_line = pd.Series([condition.lt, condition.lte]).min()
+
+    if not pd.isnull(right_line):
+        right_line_name = ["lt", "lte"][pd.Series([condition.lt, condition.lte]).argmin()]
+        lines.append((right_line, right_line_name))
+
+    if condition.eq is not None and not isinstance(condition.eq, ApproxValue):
+        lines.append((condition.eq, "eq"))
+
+    if condition.eq is not None and isinstance(condition.eq, ApproxValue):
+        lines.append((condition.eq.value, "approx"))
+
+    if condition.not_eq is not None:
+        lines.append((condition.not_eq, "not_eq"))
+
+    fig = go.Figure(fig)
+    max_y = np.max([np.max(x["y"]) for x in fig.data])
+
+    if len(lines) > 0:
+        for line, name in lines:
+            fig.add_trace(
+                go.Scatter(
+                    x=(line, line),
+                    y=(0, max_y),
+                    mode="lines",
+                    line=dict(color=color_options.secondary_color, width=3, dash="dash"),
+                    name=name,
+                )
+            )
 
+    if left_line and right_line:
+        fig.add_vrect(x0=left_line, x1=right_line, fillcolor="green", opacity=0.25, line_width=0)
 
-class ProbClassConfusionBasedFeatureDistrTable(Widget):
-    def analyzers(self):
-        return [ProbClassificationPerformanceAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-        color_options = self.options_provider.get(ColorOptions)
-        results = ProbClassificationPerformanceAnalyzer.get_results(analyzers_results)
-        quality_metrics_options = self.options_provider.get(QualityMetricsOptions)
-        cut_quantile = quality_metrics_options.cut_quantile
-        utility_columns = results.columns.utility_columns
-
-        if utility_columns.target is None or utility_columns.prediction is None:
-            raise ValueError(
-                f"Widget [{self.title}] requires 'target' or 'prediction' columns"
+    if condition.eq is not None and isinstance(condition.eq, ApproxValue):
+        left_border = 0.0
+        right_border = 0.0
+
+        if condition.eq._relative > 1e-6:
+            left_border = condition.eq.value - condition.eq.value * condition.eq._relative
+            right_border = condition.eq.value + condition.eq.value * condition.eq._relative
+            fig.add_vrect(
+                x0=left_border,
+                x1=right_border,
+                fillcolor="green",
+                opacity=0.25,
+                line_width=0,
             )
 
-        if current_data is not None:
-            ref_array_prediction = reference_data[utility_columns.prediction].to_numpy()
-            ref_prediction_ids = np.argmax(ref_array_prediction, axis=-1)
-            ref_prediction_labels = [
-                utility_columns.prediction[x] for x in ref_prediction_ids
-            ]
-            reference_data["prediction_labels"] = ref_prediction_labels
-
-            current_array_prediction = current_data[
-                utility_columns.prediction
-            ].to_numpy()
-            current_prediction_ids = np.argmax(current_array_prediction, axis=-1)
-            current_prediction_labels = [
-                utility_columns.prediction[x] for x in current_prediction_ids
-            ]
-            current_data["prediction_labels"] = current_prediction_labels
-
-            additional_graphs_data = []
-            params_data = []
-
-            for feature_name in results.columns.get_all_features_list(
-                cat_before_num=False
-            ):
-                # add data for table in params
-                labels = utility_columns.prediction
-
-                params_data.append(
-                    {
-                        "details": {
-                            "parts": [
-                                {"title": "All", "id": "All" + "_" + str(feature_name)}
-                            ]
-                            + [
-                                {
-                                    "title": str(label),
-                                    "id": feature_name + "_" + str(label),
-                                }
-                                for label in labels
-                            ],
-                            "insights": [],
-                        },
-                        "f1": feature_name,
-                    }
-                )
-
-                # create confusion based plots
-                reference_data["dataset"] = "Reference"
-                current_data["dataset"] = "Current"
-                quantile = quality_metrics_options.get_cut_quantile(feature_name)
-                if cut_quantile and quantile is not None:
-                    side, q = quantile
-                    cqt = CutQuantileTransformer(side=side, q=q)
-                    cqt.fit(reference_data[feature_name])
-                    reference_data_to_plot = cqt.transform_df(
-                        reference_data, feature_name
-                    )
-                    current_data_to_plot = cqt.transform_df(current_data, feature_name)
-                else:
-                    reference_data_to_plot = reference_data
-                    current_data_to_plot = current_data
-                merged_data = pd.concat([reference_data_to_plot, current_data_to_plot])
-
-                fig = px.histogram(
-                    merged_data,
-                    x=feature_name,
-                    color=utility_columns.target,
-                    facet_col="dataset",
-                    histnorm="",
-                    barmode="overlay",
-                    category_orders={"dataset": ["Reference", "Current"]},
-                )
+        elif condition.eq._absolute > 1e-12:
+            left_border = condition.eq.value - condition.eq._absolute
+            right_border = condition.eq.value + condition.eq._absolute
+            fig.add_vrect(
+                x0=left_border,
+                x1=right_border,
+                fillcolor="green",
+                opacity=0.25,
+                line_width=0,
+            )
 
-                fig_json = json.loads(fig.to_json())
+        fig.add_vrect(
+            x0=left_border,
+            x1=right_border,
+            fillcolor="green",
+            opacity=0.25,
+            line_width=0,
+        )
 
-                # write plot data in table as additional data
-                additional_graphs_data.append(
-                    AdditionalGraphInfo(
-                        "All" + "_" + str(feature_name),
-                        {"data": fig_json["data"], "layout": fig_json["layout"]},
-                    )
-                )
+    fig.update_layout(showlegend=True)
+    return fig
 
-                for label in labels:
-                    fig = make_subplots(
-                        rows=1, cols=2, subplot_titles=("Reference", "Current")
-                    )
-
-                    # REF
-                    fig.add_trace(
-                        go.Scatter(
-                            x=reference_data[
-                                reference_data[utility_columns.target] == label
-                            ][feature_name],
-                            y=reference_data[
-                                reference_data[utility_columns.target] == label
-                            ][label],
-                            mode="markers",
-                            name=str(label) + " (ref)",
-                            marker=dict(
-                                size=6, color=color_options.get_current_data_color()
-                            ),
-                        ),
-                        row=1,
-                        col=1,
-                    )
-
-                    fig.add_trace(
-                        go.Scatter(
-                            x=reference_data[
-                                reference_data[utility_columns.target] != label
-                            ][feature_name],
-                            y=reference_data[
-                                reference_data[utility_columns.target] != label
-                            ][label],
-                            mode="markers",
-                            name="other (ref)",
-                            marker=dict(
-                                size=6, color=color_options.get_reference_data_color()
-                            ),
-                        ),
-                        row=1,
-                        col=1,
-                    )
-
-                    fig.update_layout(
-                        xaxis_title=feature_name,
-                        yaxis_title="Probability",
-                        xaxis=dict(showticklabels=True),
-                        yaxis=dict(range=(-0.1, 1.1), showticklabels=True),
-                    )
-
-                    # current Prediction
-                    fig.add_trace(
-                        go.Scatter(
-                            x=current_data[
-                                current_data[utility_columns.target] == label
-                            ][feature_name],
-                            y=current_data[
-                                current_data[utility_columns.target] == label
-                            ][label],
-                            mode="markers",
-                            name=str(label) + " (curr)",
-                            marker=dict(
-                                size=6,
-                                # set color equal to a variable
-                                color=color_options.get_current_data_color(),
-                            ),
-                        ),
-                        row=1,
-                        col=2,
-                    )
-
-                    fig.add_trace(
-                        go.Scatter(
-                            x=current_data[
-                                current_data[utility_columns.target] != label
-                            ][feature_name],
-                            y=current_data[
-                                current_data[utility_columns.target] != label
-                            ][label],
-                            mode="markers",
-                            name="other (curr)",
-                            marker=dict(
-                                size=6,
-                                # set color equal to a variable
-                                color=color_options.get_reference_data_color(),
-                            ),
-                        ),
-                        row=1,
-                        col=2,
-                    )
-
-                    fig.update_layout(
-                        xaxis_title=feature_name,
-                        yaxis_title="Probability",
-                        xaxis=dict(showticklabels=True),
-                        yaxis=dict(range=(-0.1, 1.1), showticklabels=True),
-                    )
-
-                    # Update xaxis properties
-                    fig.update_xaxes(
-                        title_text=feature_name, showgrid=True, row=1, col=1
-                    )
-                    fig.update_xaxes(
-                        title_text=feature_name, showgrid=True, row=1, col=2
-                    )
-
-                    # Update yaxis properties
-                    fig.update_yaxes(
-                        title_text="Probability", showgrid=True, row=1, col=1
-                    )
-                    fig.update_yaxes(
-                        title_text="Probability", showgrid=True, row=1, col=2
-                    )
-
-                    fig_json = json.loads(fig.to_json())
-
-                    # write plot data in table as additional data
-                    additional_graphs_data.append(
-                        AdditionalGraphInfo(
-                            feature_name + "_" + str(label),
-                            {"data": fig_json["data"], "layout": fig_json["layout"]},
-                        )
-                    )
-        else:
-            ref_array_prediction = reference_data[utility_columns.prediction].to_numpy()
-            ref_prediction_ids = np.argmax(ref_array_prediction, axis=-1)
-            ref_prediction_labels = [
-                utility_columns.prediction[x] for x in ref_prediction_ids
-            ]
-            reference_data["prediction_labels"] = ref_prediction_labels
-
-            additional_graphs_data = []
-            params_data = []
-
-            for feature_name in results.columns.get_all_features_list(
-                cat_before_num=False
-            ):
-                # add data for table in params
-                labels = utility_columns.prediction
-
-                params_data.append(
-                    {
-                        "details": {
-                            "parts": [
-                                {"title": "All", "id": "All" + "_" + str(feature_name)}
-                            ]
-                            + [
-                                {
-                                    "title": str(label),
-                                    "id": feature_name + "_" + str(label),
-                                }
-                                for label in labels
-                            ],
-                            "insights": [],
-                        },
-                        "f1": feature_name,
-                    }
-                )
 
-                # create confusion based plots
-                fig = px.histogram(
-                    reference_data,
-                    x=feature_name,
-                    color=utility_columns.target,
-                    histnorm="",
-                )
-                cut_quantile_options = quality_metrics_options.get_cut_quantile(
-                    feature_name
+def plot_metric_value(fig, metric_val: float, metric_name: str):
+    fig = go.Figure(fig)
+    max_y = np.max([np.max(x["y"]) for x in fig.data])
+    min_y = np.min([np.min(x["y"]) for x in fig.data])
+    fig.add_trace(
+        go.Scatter(
+            x=(metric_val, metric_val),
+            y=(min_y, max_y),
+            mode="lines",
+            line=dict(color="green", width=3),
+            name=metric_name,
+        )
+    )
+    fig.update_layout(showlegend=True)
+    return fig
+
+
+def plot_value_counts_tables(feature_name, values, curr_df, ref_df, id_prfx):
+    additional_plots = []
+    if values is not None:
+        curr_df = curr_df[curr_df["count"] != 0]
+        curr_vals_inside_lst = curr_df[curr_df.x.isin(values)].sort_values("count", ascending=False)
+        if curr_vals_inside_lst.shape[0] > 0:
+            additional_plots.append(
+                DetailsInfo(
+                    title="Values inside the list (top 10)",
+                    info=table_data(
+                        column_names=["value", "count"],
+                        data=curr_vals_inside_lst[:10].values,
+                    ),
                 )
-                if cut_quantile and cut_quantile_options is not None:
-                    side, q = cut_quantile_options
-                    cqt = CutQuantileTransformer(side=side, q=q)
-                    cqt.fit(reference_data[feature_name])
-                    reference_data_to_plot = cqt.transform_df(
-                        reference_data, feature_name
-                    )
-                else:
-                    reference_data_to_plot = reference_data
-
-                fig = px.histogram(
-                    reference_data_to_plot,
-                    x=feature_name,
-                    color=utility_columns.target,
-                    histnorm="",
-                    barmode="overlay",
+            )
+        curr_vals_outside_lst = curr_df[~curr_df.x.isin(values)].sort_values("count", ascending=False)
+        if curr_vals_outside_lst.shape[0] > 0:
+            additional_plots.append(
+                DetailsInfo(
+                    title="Values outside the list (top 10)",
+                    info=table_data(
+                        column_names=["value", "count"],
+                        data=curr_vals_outside_lst[:10].values,
+                    ),
                 )
+            )
+    elif ref_df is not None:
+        curr_df = curr_df[curr_df["count"] != 0]
+        ref_df = ref_df[ref_df["count"] != 0]
+
+        if is_numeric_dtype(curr_df.x):
+            new_values = np.setdiff1d(curr_df.x.values, ref_df.x.values)
+            missed_values = np.setdiff1d(ref_df.x.values, curr_df.x.values)
+        else:
+            curr_df["x"] = curr_df["x"].astype(str)
+            ref_df["x"] = ref_df["x"].astype(str)
+            new_values = np.setdiff1d(curr_df.x.values, ref_df.x.values)
+            missed_values = np.setdiff1d(ref_df.x.values, curr_df.x.values)
+        new_values_data = curr_df[curr_df.x.isin(new_values)].sort_values("count", ascending=False)
+        missed_values_data = ref_df[ref_df.x.isin(missed_values)].sort_values("count", ascending=False)
+        additional_plots.append(
+            DetailsInfo(
+                title="New values (top 10)",
+                info=table_data(column_names=["value", "count"], data=new_values_data[:10].values),
+            )
+        )
+        additional_plots.append(
+            DetailsInfo(
+                title="Missing values (top 10)",
+                info=table_data(column_names=["value", "count"], data=missed_values_data[:10].values),
+            )
+        )
 
-                fig_json = json.loads(fig.to_json())
+    return additional_plots
 
-                # write plot data in table as additional data
-                additional_graphs_data.append(
-                    AdditionalGraphInfo(
-                        "All" + "_" + str(feature_name),
-                        {"data": fig_json["data"], "layout": fig_json["layout"]},
-                    )
-                )
 
-                for label in labels:
-                    fig = go.Figure()
+def plot_value_counts_tables_ref_curr(feature_name, curr_df, ref_df, id_prfx):
+    additional_plots = []
+    curr_df = curr_df[curr_df["count"] != 0]
+
+    additional_plots.append(
+        DetailsInfo(
+            title="Current value counts (top 10)",
+            info=table_data(column_names=["value", "count"], data=curr_df[:10].values),
+        )
+    )
+    if ref_df is not None:
+        ref_df = ref_df[ref_df["count"] != 0]
+        additional_plots.append(
+            DetailsInfo(
+                title="Reference value counts (top 10)",
+                info=table_data(column_names=["value", "count"], data=ref_df[:10].values),
+            )
+        )
+    return additional_plots
+
+
+def approx(value, relative=None, absolute=None):
+    """Get approximate value for checking a value is equal to other within some tolerance"""
+    return ApproxValue(value=value, relative=relative, absolute=absolute)
+
+
+def dataframes_to_table(
+    current: pd.DataFrame,
+    reference: Optional[pd.DataFrame],
+    columns: List[str],
+    table_id: str,
+    sort_by: str = "curr",
+    na_position: str = "first",
+    asc: bool = False,
+):
+    display_columns = ["display"]
+    if reference is not None:
+        display_columns += ["ref_display"]
+        df = pd.merge(
+            current,
+            reference.rename(columns={"value": "ref_value", "display": "ref_display"}),
+            how="outer",
+            left_index=True,
+            right_index=True,
+        )
+        df["eq"] = (df["value"] == df["ref_value"]) | (df["value"].isna() & df["ref_value"].isna())
+        if "ref_display" not in df.columns:
+            df["ref_display"] = df["ref_value"].fillna("NA").astype(str)
+    else:
+        df = current
+    if "display" not in df.columns:
+        df["display"] = df["value"].fillna("NA").astype(str)
+    if sort_by == "curr":
+        df.sort_values("value", na_position=na_position, inplace=True, ascending=asc)
+    elif sort_by == "diff" and reference is not None:
+        df.sort_values("eq", inplace=True)
+
+    df = df[display_columns].fillna("NA")
+    return [
+        DetailsInfo(
+            id=table_id,
+            title="",
+            info=BaseWidgetInfo(
+                title="",
+                type="table",
+                params={
+                    "header": list(columns),
+                    "data": [[idx] + list(df.loc[idx].values) for idx in df.index],
+                },
+                size=2,
+            ),
+        )
+    ]
+
+
+def plot_dicts_to_table(
+    dict_curr: dict, dict_ref: Optional[dict], columns: list, id_prfx: str, sort_by: str = "curr", asc: bool = False
+):
+    return dataframes_to_table(
+        pd.DataFrame.from_dict(dict_curr, orient="index", columns=["value"]),
+        None if dict_ref is None else pd.DataFrame.from_dict(dict_ref, orient="index", columns=["value"]),
+        columns=columns,
+        table_id=id_prfx,
+        sort_by=sort_by,
+        na_position="first",
+        asc=asc,
+    )
+
+
+def plot_correlations(current_correlations, reference_correlations):
+    columns = current_correlations.columns
+    heatmap_text = None
+    heatmap_texttemplate = None
+
+    if reference_correlations is not None:
+        cols = 2
+        subplot_titles = ["current", "reference"]
+    else:
+        cols = 1
+        subplot_titles = [""]
+
+    fig = make_subplots(rows=1, cols=cols, subplot_titles=subplot_titles, shared_yaxes=True)
+    if len(columns) < 15:
+        heatmap_text = np.round(current_correlations, 2).astype(str)
+        heatmap_texttemplate = "%{text}"
+
+    trace = go.Heatmap(
+        z=current_correlations,
+        x=columns,
+        y=columns,
+        text=heatmap_text,
+        texttemplate=heatmap_texttemplate,
+        coloraxis="coloraxis",
+    )
+    fig.add_trace(trace, 1, 1)
+
+    if reference_correlations is not None:
+        if len(columns) < 15:
+            heatmap_text = np.round(reference_correlations, 2).astype(str)
+            heatmap_texttemplate = "%{text}"
+
+        trace = go.Heatmap(
+            z=reference_correlations,
+            x=columns,
+            y=columns,
+            text=heatmap_text,
+            texttemplate=heatmap_texttemplate,
+            coloraxis="coloraxis",
+        )
+        fig.add_trace(trace, 1, 2)
+    fig.update_layout(coloraxis={"colorscale": "RdBu_r"})
+    fig.update_yaxes(type="category")
+    fig.update_xaxes(tickangle=-45)
+    return fig
+
+
+# todo typing: ConfusionMatrix
+def plot_conf_mtrx(curr_mtrx, ref_mtrx):
+    if ref_mtrx is not None:
+        cols = 2
+        subplot_titles = ["current", "reference"]
+    else:
+        cols = 1
+        subplot_titles = [""]
+    fig = make_subplots(rows=1, cols=cols, subplot_titles=subplot_titles, shared_yaxes=True)
+    trace = go.Heatmap(
+        z=curr_mtrx.values,
+        x=list(map(str, curr_mtrx.labels)),
+        y=list(map(str, curr_mtrx.labels)),
+        text=np.array(curr_mtrx.values).astype(str),
+        texttemplate="%{text}",
+        coloraxis="coloraxis",
+    )
+    fig.add_trace(trace, 1, 1)
+
+    if ref_mtrx is not None:
+        trace = go.Heatmap(
+            z=ref_mtrx.values,
+            x=list(map(str, ref_mtrx.labels)),
+            y=list(map(str, ref_mtrx.labels)),
+            text=np.array(ref_mtrx.values).astype(str),
+            texttemplate="%{text}",
+            coloraxis="coloraxis",
+        )
+        fig.add_trace(trace, 1, 2)
+    fig.update_layout(coloraxis={"colorscale": "RdBu_r"})
+    return fig
+
+
+def plot_roc_auc(
+    *, curr_roc_curve: dict, ref_roc_curve: Optional[dict], color_options: ColorOptions
+) -> List[Tuple[str, BaseWidgetInfo]]:
+    additional_plots = []
+    cols = 1
+    subplot_titles = [""]
+    current_color = color_options.get_current_data_color()
+    reference_color = color_options.get_reference_data_color()
+
+    if ref_roc_curve is not None:
+        cols = 2
+        subplot_titles = ["current", "reference"]
+
+    for label in curr_roc_curve.keys():
+        fig = make_subplots(rows=1, cols=cols, subplot_titles=subplot_titles, shared_yaxes=True)
+        trace = go.Scatter(
+            x=curr_roc_curve[label]["fpr"],
+            y=curr_roc_curve[label]["tpr"],
+            mode="lines",
+            name="ROC",
+            marker=dict(
+                size=6,
+                color=current_color,
+            ),
+        )
+        fig.add_trace(trace, 1, 1)
+
+        if ref_roc_curve is not None:
+            trace = go.Scatter(
+                x=ref_roc_curve[label]["fpr"],
+                y=ref_roc_curve[label]["tpr"],
+                mode="lines",
+                name="ROC",
+                marker=dict(
+                    size=6,
+                    color=reference_color,
+                ),
+            )
+            fig.add_trace(trace, 1, 2)
+        fig.update_layout(
+            yaxis_title="True Positive Rate",
+            xaxis_title="False Positive Rate",
+            showlegend=True,
+        )
+        additional_plots.append((f"ROC Curve for label {label}", plotly_figure(title="", figure=fig)))
+
+    return additional_plots
+
 
-                    fig.add_trace(
-                        go.Scatter(
-                            x=reference_data[
-                                reference_data[utility_columns.target] == label
-                            ][feature_name],
-                            y=reference_data[
-                                reference_data[utility_columns.target] == label
-                            ][label],
-                            mode="markers",
-                            name=str(label),
-                            marker=dict(
-                                size=6,
-                                color=color_options.get_current_data_color(),  # set color equal to a variable
-                            ),
-                        )
-                    )
-
-                    fig.add_trace(
-                        go.Scatter(
-                            x=reference_data[
-                                reference_data[utility_columns.target] != label
-                            ][feature_name],
-                            y=reference_data[
-                                reference_data[utility_columns.target] != label
-                            ][label],
-                            mode="markers",
-                            name="other",
-                            marker=dict(
-                                size=6, color=color_options.get_reference_data_color()
-                            ),
-                        )
-                    )
-
-                    fig.update_layout(
-                        xaxis_title=feature_name,
-                        yaxis_title="Probability",
-                        xaxis=dict(showticklabels=True),
-                        yaxis=dict(range=(-0.1, 1.1), showticklabels=True),
-                    )
-
-                    fig_json = json.loads(fig.to_json())
-
-                    # write plot data in table as additional data
-                    additional_graphs_data.append(
-                        AdditionalGraphInfo(
-                            feature_name + "_" + str(label),
-                            {"data": fig_json["data"], "layout": fig_json["layout"]},
-                        )
-                    )
-
-        return BaseWidgetInfo(
-            title=self.title,
-            type="big_table",
-            size=2,
-            params={
-                "rowsPerPage": min(results.columns.get_features_len(), 10),
-                "columns": [{"title": "Feature", "field": "f1"}],
-                "data": params_data,
-            },
-            additionalGraphs=additional_graphs_data,
+def plot_boxes(*, curr_for_plots: Boxes, ref_for_plots: Optional[Boxes], color_options: ColorOptions):
+    current_color = color_options.get_current_data_color()
+    reference_color = color_options.get_reference_data_color()
+    fig = go.Figure()
+    trace = go.Box(
+        lowerfence=curr_for_plots.mins,
+        q1=curr_for_plots.lowers,
+        q3=curr_for_plots.uppers,
+        median=curr_for_plots.means,
+        upperfence=curr_for_plots.maxs,
+        name="current",
+        marker_color=current_color,
+    )
+    fig.add_trace(trace)
+    if ref_for_plots is not None:
+        trace = go.Box(
+            lowerfence=curr_for_plots.mins,
+            q1=ref_for_plots.lowers,
+            q3=ref_for_plots.uppers,
+            median=ref_for_plots.means,
+            upperfence=ref_for_plots.maxs,
+            name="reference",
+            marker_color=reference_color,
         )
+        fig.add_trace(trace)
+        fig.update_layout(boxmode="group")
+
+    fig.update_layout(
+        yaxis_title="Prerdictions",
+        xaxis_title="Class",
+    )
+    return fig
+
+
+def plot_rates(
+    *,
+    curr_rate_plots_data: RatesPlotData,
+    ref_rate_plots_data: Optional[RatesPlotData] = None,
+    color_options: ColorOptions,
+):
+    if ref_rate_plots_data is not None:
+        cols = 2
+        subplot_titles = ["current", "reference"]
+    else:
+        cols = 1
+        subplot_titles = [""]
+
+    curr_df = pd.DataFrame(
+        {
+            "thrs": curr_rate_plots_data.thrs,
+            "fpr": curr_rate_plots_data.fpr,
+            "tpr": curr_rate_plots_data.tpr,
+            "fnr": curr_rate_plots_data.fnr,
+            "tnr": curr_rate_plots_data.tnr,
+        }
+    )
+    curr_df = curr_df[curr_df.thrs <= 1]
+
+    fig = make_subplots(rows=1, cols=cols, subplot_titles=subplot_titles, shared_yaxes=True)
+    for i, metric in enumerate(["fpr", "tpr", "fnr", "tnr"]):
+        fig.add_trace(
+            go.Scatter(
+                x=curr_df["thrs"],
+                y=curr_df[metric],
+                mode="lines",
+                legendgroup=metric,
+                name=metric,
+                marker_color=color_options.color_sequence[i],
+            ),
+            1,
+            1,
+        )
+    if ref_rate_plots_data is not None:
+        ref_df = pd.DataFrame(
+            {
+                "thrs": ref_rate_plots_data.thrs,
+                "fpr": ref_rate_plots_data.fpr,
+                "tpr": ref_rate_plots_data.tpr,
+                "fnr": ref_rate_plots_data.fnr,
+                "tnr": ref_rate_plots_data.tnr,
+            }
+        )
+        ref_df = ref_df[ref_df.thrs <= 1]
+        for i, metric in enumerate(["fpr", "tpr", "fnr", "tnr"]):
+            fig.add_trace(
+                go.Scatter(
+                    x=ref_df["thrs"],
+                    y=ref_df[metric],
+                    mode="lines",
+                    legendgroup=metric,
+                    name=metric,
+                    showlegend=False,
+                    marker_color=color_options.color_sequence[i],
+                ),
+                1,
+                2,
+            )
+    fig.update_layout(
+        xaxis_title="threshold",
+    )
+
+    return fig
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/reg_colored_pred_vs_actual_widget.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/pr_table_metric.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,138 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-import json
+import dataclasses
+from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Union
 
-import numpy as np
 import pandas as pd
-import plotly.graph_objs as go
 
-from evidently import ColumnMapping
-from evidently.analyzers.regression_performance_analyzer import (
-    RegressionPerformanceAnalyzer,
-)
-from evidently.dashboard.widgets.widget import Widget
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.calculations.classification_performance import calculate_pr_table
+from evidently.calculations.classification_performance import get_prediction_data
+from evidently.metric_results import Label
+from evidently.metric_results import PredictionData
 from evidently.model.widget import BaseWidgetInfo
-from evidently.options import ColorOptions
-
-
-class RegColoredPredActualWidget(Widget):
-    def __init__(self, title: str, dataset: str = "reference"):
-        super().__init__(title)
-        self.dataset = dataset  # reference or current
-
-    def analyzers(self):
-        return [RegressionPerformanceAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-        color_options = self.options_provider.get(ColorOptions)
-        results = RegressionPerformanceAnalyzer.get_results(analyzers_results)
-        results_utility_columns = results.columns.utility_columns
-
-        if (
-            results_utility_columns.target is None
-            or results_utility_columns.prediction is None
-        ):
-            if self.dataset == "reference":
-                raise ValueError(
-                    f"Widget [{self.title}] requires 'target' and 'prediction' columns"
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import TabData
+from evidently.renderers.html_widgets import WidgetSize
+from evidently.renderers.html_widgets import table_data
+from evidently.renderers.html_widgets import widget_tabs
+from evidently.utils.data_operations import process_columns
+
+PRTable = Dict[Label, List[List[Union[float, int]]]]
+
+
+class ClassificationPRTableResults(MetricResult):
+    class Config:
+        smart_union = True
+
+    current: Optional[PRTable] = None
+    reference: Optional[PRTable] = None
+
+
+class ClassificationPRTable(Metric[ClassificationPRTableResults]):
+    def calculate(self, data: InputData) -> ClassificationPRTableResults:
+        dataset_columns = process_columns(data.current_data, data.column_mapping)
+        target_name = dataset_columns.utility_columns.target
+        prediction_name = dataset_columns.utility_columns.prediction
+        if target_name is None or prediction_name is None:
+            raise ValueError("The columns 'target' and 'prediction' columns should be present")
+        curr_prediction = get_prediction_data(data.current_data, dataset_columns, data.column_mapping.pos_label)
+        curr_pr_table = self.calculate_metrics(data.current_data[target_name], curr_prediction)
+        ref_pr_table = None
+        if data.reference_data is not None:
+            ref_prediction = get_prediction_data(data.reference_data, dataset_columns, data.column_mapping.pos_label)
+            ref_pr_table = self.calculate_metrics(data.reference_data[target_name], ref_prediction)
+        return ClassificationPRTableResults(
+            current=curr_pr_table,
+            reference=ref_pr_table,
+        )
+
+    def calculate_metrics(self, target_data: pd.Series, prediction: PredictionData):
+        labels = prediction.labels
+        if prediction.prediction_probas is None:
+            raise ValueError("PR Table can be calculated only on binary probabilistic predictions")
+        binaraized_target = (target_data.values.reshape(-1, 1) == labels).astype(int)
+        pr_table = {}
+        if len(labels) <= 2:
+            binaraized_target = pd.DataFrame(binaraized_target[:, 0])
+            binaraized_target.columns = ["target"]
+
+            binded = list(
+                zip(
+                    binaraized_target["target"].tolist(),
+                    prediction.prediction_probas.iloc[:, 0].tolist(),
                 )
-
-            return None
-
-        if self.dataset == "current":
-            dataset_to_plot = (
-                current_data.copy(deep=False) if current_data is not None else None
             )
-
+            pr_table[prediction.prediction_probas.columns[0]] = calculate_pr_table(binded)
         else:
-            dataset_to_plot = reference_data.copy(deep=False)
+            binaraized_target = pd.DataFrame(binaraized_target)
+            binaraized_target.columns = labels
 
-        if dataset_to_plot is None:
-            if self.dataset == "reference":
-                raise ValueError(
-                    f"Widget [{self.title}] requires reference dataset but it is None"
+            for label in labels:
+                binded = list(
+                    zip(
+                        binaraized_target[label].tolist(),
+                        prediction.prediction_probas[label],
+                    )
                 )
-            return None
+                pr_table[label] = calculate_pr_table(binded)
+        return pr_table
 
-        dataset_to_plot.replace([np.inf, -np.inf], np.nan, inplace=True)
-        dataset_to_plot.dropna(
-            axis=0,
-            how="any",
-            inplace=True,
-            subset=[results_utility_columns.target, results_utility_columns.prediction],
-        )
 
-        error = (
-            dataset_to_plot[results_utility_columns.prediction]
-            - dataset_to_plot[results_utility_columns.target]
-        )
-
-        quantile_5 = np.quantile(error, 0.05)
-        quantile_95 = np.quantile(error, 0.95)
-
-        dataset_to_plot["Error bias"] = list(
-            map(
-                lambda x: "Underestimation"
-                if x <= quantile_5
-                else "Majority"
-                if x < quantile_95
-                else "Overestimation",
-                error,
-            )
-        )
-
-        # plot output correlations
-        pred_actual = go.Figure()
-
-        pred_actual.add_trace(
-            go.Scatter(
-                x=dataset_to_plot[dataset_to_plot["Error bias"] == "Underestimation"][
-                    results_utility_columns.target
-                ],
-                y=dataset_to_plot[dataset_to_plot["Error bias"] == "Underestimation"][
-                    results_utility_columns.prediction
-                ],
-                mode="markers",
-                name="Underestimation",
-                marker=dict(color=color_options.underestimation_color, showscale=False),
-            )
-        )
-
-        pred_actual.add_trace(
-            go.Scatter(
-                x=dataset_to_plot[dataset_to_plot["Error bias"] == "Overestimation"][
-                    results_utility_columns.target
-                ],
-                y=dataset_to_plot[dataset_to_plot["Error bias"] == "Overestimation"][
-                    results_utility_columns.prediction
-                ],
-                mode="markers",
-                name="Overestimation",
-                marker=dict(color=color_options.overestimation_color, showscale=False),
-            )
-        )
-
-        pred_actual.add_trace(
-            go.Scatter(
-                x=dataset_to_plot[dataset_to_plot["Error bias"] == "Majority"][
-                    results_utility_columns.target
-                ],
-                y=dataset_to_plot[dataset_to_plot["Error bias"] == "Majority"][
-                    results_utility_columns.prediction
-                ],
-                mode="markers",
-                name="Majority",
-                marker=dict(color=color_options.majority_color, showscale=False),
-            )
-        )
-
-        pred_actual.update_layout(
-            xaxis_title="Actual value",
-            yaxis_title="Predicted value",
-            xaxis=dict(showticklabels=True),
-            yaxis=dict(showticklabels=True),
-        )
-
-        pred_actual_json = json.loads(pred_actual.to_json())
-
-        return BaseWidgetInfo(
-            title=self.title,
-            type="big_graph",
-            size=1 if current_data is not None else 2,
-            params={
-                "data": pred_actual_json["data"],
-                "layout": pred_actual_json["layout"],
-            },
-            additionalGraphs=[],
-        )
+@default_renderer(wrap_type=ClassificationPRTable)
+class ClassificationPRTableRenderer(MetricRenderer):
+    def render_html(self, obj: ClassificationPRTable) -> List[BaseWidgetInfo]:
+        reference_pr_table = obj.get_result().reference
+        current_pr_table = obj.get_result().current
+        columns = ["Top(%)", "Count", "Prob", "TP", "FP", "Precision", "Recall"]
+        result = []
+        size = WidgetSize.FULL
+        # if reference_pr_table is not None:
+        #     size = WidgetSize.HALF
+        if current_pr_table is not None:
+            if len(current_pr_table.keys()) == 1:
+                result.append(
+                    table_data(
+                        column_names=columns,
+                        data=current_pr_table[list(current_pr_table.keys())[0]],
+                        title="Current: Precision-Recall Table",
+                        size=size,
+                    )
+                )
+            else:
+                tab_data = []
+                for label in current_pr_table.keys():
+                    table = table_data(
+                        column_names=columns,
+                        data=current_pr_table[label],
+                        title="",
+                        size=size,
+                    )
+                    tab_data.append(TabData(str(label), table))
+                result.append(widget_tabs(title="Current: Precision-Recall Table", tabs=tab_data))
+        if reference_pr_table is not None:
+            if len(reference_pr_table.keys()) == 1:
+                result.append(
+                    table_data(
+                        column_names=columns,
+                        data=reference_pr_table[list(reference_pr_table.keys())[0]],
+                        title="Reference: Precision-Recall Table",
+                        size=size,
+                    )
+                )
+            else:
+                tab_data = []
+                for label in reference_pr_table.keys():
+                    table = table_data(
+                        column_names=columns,
+                        data=reference_pr_table[label],
+                        title="",
+                        size=size,
+                    )
+                    tab_data.append(TabData(str(label), table))
+                result.append(widget_tabs(title="Reference: Precision-Recall Table", tabs=tab_data))
+        return result
```

### Comparing `evidently-0.2.8/src/evidently/dashboard/widgets/reg_error_in_time_widget.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,123 +1,97 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-import json
+import dataclasses
+from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Union
 
 import numpy as np
 import pandas as pd
-import plotly.graph_objs as go
 
-from evidently import ColumnMapping
-from evidently.analyzers.regression_performance_analyzer import (
-    RegressionPerformanceAnalyzer,
-)
-from evidently.dashboard.widgets.widget import Widget
+from evidently.base_metric import InputData
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.metric_results import ColumnScatter
+from evidently.metric_results import ColumnScatterResult
 from evidently.model.widget import BaseWidgetInfo
-from evidently.options import ColorOptions
-
-
-class RegErrorTimeWidget(Widget):
-    def __init__(self, title: str, dataset: str = "reference"):
-        super().__init__(title)
-        self.dataset = dataset  # reference or current
-
-    def analyzers(self):
-        return [RegressionPerformanceAnalyzer]
-
-    def calculate(
-        self,
-        reference_data: pd.DataFrame,
-        current_data: Optional[pd.DataFrame],
-        column_mapping: ColumnMapping,
-        analyzers_results,
-    ) -> Optional[BaseWidgetInfo]:
-        color_options = self.options_provider.get(ColorOptions)
-        results = RegressionPerformanceAnalyzer.get_results(analyzers_results)
-        results_utility_columns = results.columns.utility_columns
-
-        if (
-            results_utility_columns.target is None
-            or results_utility_columns.prediction is None
-        ):
-            if self.dataset == "reference":
-                raise ValueError(
-                    f"Widget [{self.title}] requires 'target' and 'prediction' columns"
-                )
-
-            return None
-
-        if self.dataset == "current":
-            dataset_to_plot = (
-                current_data.copy(deep=False) if current_data is not None else None
-            )
-
+from evidently.renderers.base_renderer import MetricRenderer
+from evidently.renderers.base_renderer import default_renderer
+from evidently.renderers.html_widgets import header_text
+from evidently.utils.data_operations import process_columns
+from evidently.utils.visualizations import plot_pred_actual_time
+
+
+class RegressionPredictedVsActualPlot(Metric[ColumnScatterResult]):
+    def calculate(self, data: InputData) -> ColumnScatterResult:
+        dataset_columns = process_columns(data.current_data, data.column_mapping)
+        target_name = dataset_columns.utility_columns.target
+        prediction_name = dataset_columns.utility_columns.prediction
+        datetime_column_name = dataset_columns.utility_columns.date
+        curr_df = data.current_data
+        ref_df = data.reference_data
+        if target_name is None or prediction_name is None:
+            raise ValueError("The columns 'target' and 'prediction' columns should be present")
+        if not isinstance(prediction_name, str):
+            raise ValueError("Expect one column for prediction. List of columns was provided.")
+        curr_df = self._make_df_for_plot(curr_df, target_name, prediction_name, datetime_column_name)
+        current_scatter = {}
+        current_scatter["Predicted"] = curr_df[prediction_name]
+        current_scatter["Actual"] = curr_df[target_name]
+        if datetime_column_name is not None:
+            current_scatter["x"] = curr_df[datetime_column_name]
+            x_name = "Timestamp"
         else:
-            dataset_to_plot = reference_data.copy(deep=False)
-
-        if dataset_to_plot is None:
-            if self.dataset == "reference":
-                raise ValueError(
-                    f"Widget [{self.title}] requires reference dataset but it is None"
-                )
-            return None
-
-        dataset_to_plot.replace([np.inf, -np.inf], np.nan, inplace=True)
-        dataset_to_plot.dropna(
-            axis=0,
-            how="any",
-            inplace=True,
-            subset=[results_utility_columns.target, results_utility_columns.prediction],
-        )
-
-        # plot error in time
-        error_in_time = go.Figure()
+            current_scatter["x"] = curr_df.index
+            x_name = "Index"
 
-        error_trace = go.Scatter(
-            x=dataset_to_plot[results_utility_columns.date]
-            if results_utility_columns.date
-            else dataset_to_plot.index,
-            y=dataset_to_plot[results_utility_columns.prediction]
-            - dataset_to_plot[results_utility_columns.target],
-            mode="lines",
-            name="Predicted - Actual",
-            marker=dict(size=6, color=color_options.primary_color),
+        reference_scatter: Optional[dict] = None
+        if data.reference_data is not None:
+            ref_df = self._make_df_for_plot(ref_df, target_name, prediction_name, datetime_column_name)
+            reference_scatter = {}
+            reference_scatter["Predicted"] = ref_df[prediction_name]
+            reference_scatter["Actual"] = ref_df[target_name]
+            reference_scatter["x"] = ref_df[datetime_column_name] if datetime_column_name else ref_df.index
+        return ColumnScatterResult(
+            current=current_scatter,
+            reference=reference_scatter,
+            x_name=x_name,
         )
 
-        zero_trace = go.Scatter(
-            x=dataset_to_plot[results_utility_columns.date]
-            if results_utility_columns.date
-            else dataset_to_plot.index,
-            y=[0] * dataset_to_plot.shape[0],
-            mode="lines",
-            opacity=0.5,
-            marker=dict(
-                size=6,
-                color=color_options.zero_line_color,
-            ),
-            showlegend=False,
+    def _make_df_for_plot(self, df, target_name: str, prediction_name: str, datetime_column_name: Optional[str]):
+        result = df.replace([np.inf, -np.inf], np.nan)
+        if datetime_column_name is not None:
+            result.dropna(
+                axis=0,
+                how="any",
+                inplace=True,
+                subset=[target_name, prediction_name, datetime_column_name],
+            )
+            return result.sort_values(datetime_column_name)
+        result.dropna(axis=0, how="any", inplace=True, subset=[target_name, prediction_name])
+        return result.sort_index()
+
+
+@default_renderer(wrap_type=RegressionPredictedVsActualPlot)
+class RegressionPredictedVsActualPlotRenderer(MetricRenderer):
+    def render_html(self, obj: RegressionPredictedVsActualPlot) -> List[BaseWidgetInfo]:
+        result = obj.get_result()
+        current_scatter = result.current
+        reference_scatter = None
+        if result.reference is not None:
+            reference_scatter = result.reference
+        fig = plot_pred_actual_time(
+            curr=current_scatter,
+            ref=reference_scatter,
+            x_name="x",
+            xaxis_name=result.x_name,
+            yaxis_name="Value",
+            color_options=self.color_options,
         )
-
-        error_in_time.add_trace(error_trace)
-        error_in_time.add_trace(zero_trace)
-
-        error_in_time.update_layout(
-            xaxis_title="Timestamp" if results_utility_columns.date else "Index",
-            yaxis_title="Error",
-            legend=dict(
-                orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1
+        return [
+            header_text(label="Predicted vs Actual in Time"),
+            BaseWidgetInfo(
+                title="",
+                size=2,
+                type="big_graph",
+                params={"data": fig["data"], "layout": fig["layout"]},
             ),
-        )
-
-        error_in_time_json = json.loads(error_in_time.to_json())
-
-        return BaseWidgetInfo(
-            title=self.title,
-            type="big_graph",
-            size=1,
-            params={
-                "data": error_in_time_json["data"],
-                "layout": error_in_time_json["layout"],
-            },
-            additionalGraphs=[],
-        )
+        ]
```

### Comparing `evidently-0.2.8/src/evidently/descriptors/non_letter_character_percentage_descriptor.py` & `evidently-0.3.0/src/evidently/descriptors/non_letter_character_percentage_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/descriptors/oov_words_percentage_descriptor.py` & `evidently-0.3.0/src/evidently/descriptors/oov_words_percentage_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/descriptors/trigger_words_presence_descriptor.py` & `evidently-0.3.0/src/evidently/descriptors/trigger_words_presence_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/features/OOV_words_percentage_feature.py` & `evidently-0.3.0/src/evidently/features/OOV_words_percentage_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/features/generated_features.py` & `evidently-0.3.0/src/evidently/features/generated_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import abc
 import logging
+import typing
 from typing import Optional
 
 import pandas as pd
 
 from evidently.utils.data_preprocessing import DataDefinition
 
+if typing.TYPE_CHECKING:
+    from evidently.base_metric import ColumnName
+
 
 class GeneratedFeature:
     """
     Class for computation of additional features.
     """
 
     @abc.abstractmethod
@@ -19,15 +23,15 @@
 
         Returns:
             DataFrame with new features. Columns should be unique across all features of same type.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def feature_name(self):
+    def feature_name(self) -> "ColumnName":
         """
         get feature name for given features and parameters.
 
         Returns:
             Special feature name for unique identification results of give feature.
         """
         raise NotImplementedError()
```

### Comparing `evidently-0.2.8/src/evidently/features/non_letter_character_percentage_feature.py` & `evidently-0.3.0/src/evidently/features/non_letter_character_percentage_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/features/text_length_feature.py` & `evidently-0.3.0/src/evidently/features/text_length_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/features/trigger_words_presence_feature.py` & `evidently-0.3.0/src/evidently/features/trigger_words_presence_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metric_preset/classification_performance.py` & `evidently-0.3.0/src/evidently/metric_preset/classification_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metric_preset/data_drift.py` & `evidently-0.3.0/src/evidently/metric_preset/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metric_preset/data_quality.py` & `evidently-0.3.0/src/evidently/metric_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metric_preset/regression_performance.py` & `evidently-0.3.0/src/evidently/metric_preset/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metric_preset/target_drift.py` & `evidently-0.3.0/src/evidently/metric_preset/target_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metric_preset/text_overview.py` & `evidently-0.3.0/src/evidently/metric_preset/text_overview.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metric_results.py` & `evidently-0.3.0/src/evidently/metric_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,65 +4,67 @@
 from typing import Sequence
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
+from evidently.core import IncludeTags
 from evidently.pipeline.column_mapping import TargetNames
 
 Label = Union[int, str]
 ScatterData = Union[pd.Series, List[float], pd.Index]
 ColumnScatter = Dict[Label, ScatterData]
 
 
-class Distribution(MetricResultField):
+class Distribution(MetricResult):
     class Config:
         dict_include = False
         pd_include = False
+        tags = {IncludeTags.Render}
 
     x: Union[np.ndarray, list, pd.Categorical, pd.Series]
     y: Union[np.ndarray, list, pd.Categorical, pd.Series]
 
 
-class ConfusionMatrix(MetricResultField):
+class ConfusionMatrix(MetricResult):
     class Config:
         smart_union = True
 
     labels: Sequence[Label]
     values: list  # todo better typing
 
 
-class PredictionData(MetricResultField):
+class PredictionData(MetricResult):
     class Config:
         dict_include = False
 
     predictions: pd.Series
     prediction_probas: Optional[pd.DataFrame]
     labels: List[Label]
 
 
-class StatsByFeature(MetricResultField):
+class StatsByFeature(MetricResult):
     class Config:
         dict_include = False
         pd_include = False
+        tags = {IncludeTags.Render}
 
     plot_data: pd.DataFrame  # todo what type of plot?
     predictions: Optional[PredictionData]
 
 
-class DatasetUtilityColumns(MetricResultField):
+class DatasetUtilityColumns(MetricResult):
     date: Optional[str]
     id: Optional[str]
     target: Optional[str]
     prediction: Optional[Union[str, Sequence[str]]]
 
 
-class DatasetColumns(MetricResultField):
+class DatasetColumns(MetricResult):
     class Config:
         dict_exclude_fields = {"task", "target_type"}
 
     utility_columns: DatasetUtilityColumns
     target_type: Optional[str]
     num_feature_names: List[str]
     cat_feature_names: List[str]
@@ -139,94 +141,105 @@
 def df_from_column_scatter(value: ColumnScatter) -> pd.DataFrame:
     df = pd.DataFrame.from_dict(value)
     if "index" in df.columns:
         df.set_index("index", inplace=True)
     return df
 
 
-def column_scatter_from_df(df: pd.DataFrame, with_index: bool) -> ColumnScatter:
+def column_scatter_from_df(df: Optional[pd.DataFrame], with_index: bool) -> Optional[ColumnScatter]:
+    if df is None:
+        return None
     data = {column: df[column] for column in df.columns}
     if with_index:
         data["index"] = df.index
     return data
 
 
-class ScatterField(MetricResultField):
+class ScatterField(MetricResult):
     class Config:
         smart_union = True
         dict_include = False
         pd_include = False
 
+        tags = {IncludeTags.Render}
+
     scatter: ColumnScatter
     x_name: str
     plot_shape: Dict[str, float]
 
 
 class ColumnScatterResult(MetricResult):
     class Config:
         smart_union = True
         dict_include = False
 
+        tags = {IncludeTags.Render}
+
     current: ColumnScatter
     reference: Optional[ColumnScatter]
     x_name: str
 
 
 PlotData = List[float]
 
 
-class Boxes(MetricResultField):
+class Boxes(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     mins: PlotData
     lowers: PlotData
     means: PlotData
     uppers: PlotData
     maxs: PlotData
 
 
-class RatesPlotData(MetricResultField):
+class RatesPlotData(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     thrs: PlotData
     tpr: PlotData
     fpr: PlotData
     fnr: PlotData
     tnr: PlotData
 
 
-class PRCurveData(MetricResultField):
+class PRCurveData(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     pr: PlotData
     rcl: PlotData
     thrs: PlotData
 
 
 PRCurve = Dict[Label, PRCurveData]
 
 
-class ROCCurveData(MetricResultField):
+class ROCCurveData(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     fpr: PlotData
     tpr: PlotData
     thrs: PlotData
 
 
 ROCCurve = Dict[Label, ROCCurveData]
 
 
-class HistogramData(MetricResultField):
+class HistogramData(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     x: pd.Series
     count: pd.Series
     name: Optional[str] = None
 
     @classmethod
     def from_df(cls, value: Optional[pd.DataFrame]):
@@ -240,38 +253,39 @@
             return None
         return cls(x=pd.Series(dist.x), count=pd.Series(dist.y), name=name)
 
     def to_df(self):
         return pd.DataFrame.from_dict(self.dict(include={"x", "count"}))
 
 
-class Histogram(MetricResultField):
+class Histogram(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     current: HistogramData
     reference: Optional[HistogramData]
 
     current_log: Optional[HistogramData] = None
     reference_log: Optional[HistogramData] = None
 
 
 # todo need better config overriding logic in metricresult
 class DistributionIncluded(Distribution):
     class Config:
         dict_include = True
 
 
-class ColumnCorrelations(MetricResultField):
+class ColumnCorrelations(MetricResult):
     column_name: str
     kind: str
     values: DistributionIncluded
 
 
-class DatasetClassificationQuality(MetricResultField):
+class DatasetClassificationQuality(MetricResult):
     accuracy: float
     precision: float
     recall: float
     f1: float
     roc_auc: Optional[float] = None
     log_loss: Optional[float] = None
     tpr: Optional[float] = None
```

### Comparing `evidently-0.2.8/src/evidently/metrics/__init__.py` & `evidently-0.3.0/src/evidently/metrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .classification_performance.quality_by_class_metric import ClassificationQualityByClass
 from .classification_performance.quality_by_feature_table import ClassificationQualityByFeatureTable
 from .classification_performance.roc_curve_metric import ClassificationRocCurve
 from .data_drift.column_drift_metric import ColumnDriftMetric
 from .data_drift.column_value_plot import ColumnValuePlot
 from .data_drift.data_drift_table import DataDriftTable
 from .data_drift.dataset_drift_metric import DatasetDriftMetric
+from .data_drift.embeddings_drift import EmbeddingsDriftMetric
 from .data_drift.target_by_features_table import TargetByFeaturesTable
 from .data_drift.text_descriptors_drift_metric import TextDescriptorsDriftMetric
 from .data_integrity.column_missing_values_metric import ColumnMissingValuesMetric
 from .data_integrity.column_regexp_metric import ColumnRegExpMetric
 from .data_integrity.column_summary_metric import ColumnSummaryMetric
 from .data_integrity.dataset_missing_values_metric import DatasetMissingValuesMetric
 from .data_integrity.dataset_summary_metric import DatasetSummaryMetric
```

### Comparing `evidently-0.2.8/src/evidently/metrics/base_metric.py` & `evidently-0.3.0/src/evidently/metrics/base_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/base_classification_metric.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/base_classification_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/class_balance_metric.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/class_balance_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/classification_dummy_metric.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/classification_dummy_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/classification_quality_metric.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/classification_quality_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/objects.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from typing import Optional
 from typing import Union
 
 from pydantic import Field
 from pydantic import parse_obj_as
 from sklearn.metrics import classification_report
 
-from evidently.base_metric import MetricResultField
+from evidently.base_metric import MetricResult
 from evidently.metric_results import Label
 
 
-class ClassMetric(MetricResultField):
+class ClassMetric(MetricResult):
     precision: float
     recall: float
     f1: float = Field(alias="f1-score")
     support: Optional[float] = None
 
 
 ClassesMetrics = Dict[Label, ClassMetric]
 
 
-class ClassificationReport(MetricResultField):
+class ClassificationReport(MetricResult):
     classes: ClassesMetrics
     accuracy: float
     macro_avg: ClassMetric = Field(alias="macro avg")
     weighted_avg: ClassMetric = Field(alias="weighted avg")
 
     @classmethod
     def create(
```

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/pr_curve_metric.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/roc_curve_metric.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,92 +5,82 @@
 import pandas as pd
 from sklearn import metrics
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import get_prediction_data
-from evidently.metric_results import PRCurve
-from evidently.metric_results import PRCurveData
 from evidently.metric_results import PredictionData
+from evidently.metric_results import ROCCurve
+from evidently.metric_results import ROCCurveData
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
-from evidently.renderers.html_widgets import get_pr_rec_plot_data
+from evidently.renderers.html_widgets import get_roc_auc_tab_data
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.data_operations import process_columns
 
 
-class ClassificationPRCurveResults(MetricResult):
-    current_pr_curve: Optional[PRCurve] = None
-    reference_pr_curve: Optional[PRCurve] = None
+class ClassificationRocCurveResults(MetricResult):
+    current_roc_curve: Optional[ROCCurve] = None
+    reference_roc_curve: Optional[ROCCurve] = None
 
 
-class ClassificationPRCurve(Metric[ClassificationPRCurveResults]):
-    def calculate(self, data: InputData) -> ClassificationPRCurveResults:
+class ClassificationRocCurve(Metric[ClassificationRocCurveResults]):
+    def calculate(self, data: InputData) -> ClassificationRocCurveResults:
         dataset_columns = process_columns(data.current_data, data.column_mapping)
         target_name = dataset_columns.utility_columns.target
         prediction_name = dataset_columns.utility_columns.prediction
         if target_name is None or prediction_name is None:
             raise ValueError("The columns 'target' and 'prediction' columns should be present")
         curr_predictions = get_prediction_data(data.current_data, dataset_columns, data.column_mapping.pos_label)
-        curr_pr_curve = self.calculate_metrics(data.current_data[target_name], curr_predictions)
-        ref_pr_curve = None
+        if curr_predictions.prediction_probas is None:
+            raise ValueError("Roc Curve can be calculated only on binary probabilistic predictions")
+        curr_roc_curve = self.calculate_metrics(data.current_data[target_name], curr_predictions)
+        ref_roc_curve = None
         if data.reference_data is not None:
             ref_predictions = get_prediction_data(data.reference_data, dataset_columns, data.column_mapping.pos_label)
-            ref_pr_curve = self.calculate_metrics(data.reference_data[target_name], ref_predictions)
-        return ClassificationPRCurveResults(
-            current_pr_curve=curr_pr_curve,
-            reference_pr_curve=ref_pr_curve,
+            ref_roc_curve = self.calculate_metrics(data.reference_data[target_name], ref_predictions)
+        return ClassificationRocCurveResults(
+            current_roc_curve=curr_roc_curve,
+            reference_roc_curve=ref_roc_curve,
         )
 
-    def calculate_metrics(self, target_data: pd.Series, prediction: PredictionData) -> PRCurve:
+    def calculate_metrics(self, target_data: pd.Series, prediction: PredictionData) -> ROCCurve:
         labels = prediction.labels
         if prediction.prediction_probas is None:
-            raise ValueError("PR Curve can be calculated only on binary probabilistic predictions")
+            raise ValueError("Roc Curve can be calculated only on binary probabilistic predictions")
         binaraized_target = (target_data.values.reshape(-1, 1) == labels).astype(int)
-        pr_curve = {}
+        roc_curve = {}
         if len(labels) <= 2:
             binaraized_target = pd.DataFrame(binaraized_target[:, 0])
             binaraized_target.columns = ["target"]
-            pr, rcl, thrs = metrics.precision_recall_curve(binaraized_target, prediction.prediction_probas.iloc[:, 0])
-            pr_curve[prediction.prediction_probas.columns[0]] = PRCurveData(
-                pr=pr.tolist(),
-                rcl=rcl.tolist(),
-                thrs=thrs.tolist(),
+
+            fpr, tpr, thrs = metrics.roc_curve(binaraized_target, prediction.prediction_probas.iloc[:, 0])
+            roc_curve[prediction.prediction_probas.columns[0]] = ROCCurveData(
+                fpr=fpr.tolist(), tpr=tpr.tolist(), thrs=thrs.tolist()
             )
         else:
             binaraized_target = pd.DataFrame(binaraized_target)
             binaraized_target.columns = labels
+
             for label in labels:
+                fpr, tpr, thrs = metrics.roc_curve(binaraized_target[label], prediction.prediction_probas[label])
+                roc_curve[label] = ROCCurveData(fpr=fpr.tolist(), tpr=tpr.tolist(), thrs=thrs.tolist())
+        return roc_curve
+
 
-                pr, rcl, thrs = metrics.precision_recall_curve(
-                    binaraized_target[label],
-                    prediction.prediction_probas[label],
-                )
-
-                pr_curve[label] = PRCurveData(
-                    pr=pr.tolist(),
-                    rcl=rcl.tolist(),
-                    thrs=thrs.tolist(),
-                )
-        return pr_curve
-
-
-@default_renderer(wrap_type=ClassificationPRCurve)
-class ClassificationPRCurveRenderer(MetricRenderer):
-    def render_html(self, obj: ClassificationPRCurve) -> List[BaseWidgetInfo]:
-        current_pr_curve: Optional[PRCurve] = obj.get_result().current_pr_curve
-        reference_pr_curve: Optional[PRCurve] = obj.get_result().reference_pr_curve
-        if current_pr_curve is None:
+@default_renderer(wrap_type=ClassificationRocCurve)
+class ClassificationRocCurveRenderer(MetricRenderer):
+    def render_html(self, obj: ClassificationRocCurve) -> List[BaseWidgetInfo]:
+        current_roc_curve: Optional[ROCCurve] = obj.get_result().current_roc_curve
+        reference_roc_curve: Optional[ROCCurve] = obj.get_result().reference_roc_curve
+        if current_roc_curve is None:
             return []
 
-        tab_data = get_pr_rec_plot_data(current_pr_curve, reference_pr_curve, color_options=self.color_options)
+        tab_data = get_roc_auc_tab_data(current_roc_curve, reference_roc_curve, color_options=self.color_options)
         if len(tab_data) == 1:
-            return [header_text(label="Precision-Recall Curve"), tab_data[0][1]]
+            return [header_text(label="ROC Curve"), tab_data[0][1]]
         tabs = [TabData(name, widget) for name, widget in tab_data]
-        return [
-            header_text(label="Precision-Recall Curve"),
-            widget_tabs(title="", tabs=tabs),
-        ]
+        return [header_text(label="ROC Curve"), widget_tabs(title="", tabs=tabs)]
```

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/probability_distribution_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_distribution.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,156 +1,117 @@
-import dataclasses
 from typing import Dict
-from typing import Iterable
 from typing import List
 from typing import Optional
 
-import numpy as np
-import pandas as pd
-from plotly import figure_factory as ff
-
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.calculations.classification_performance import get_prediction_data
+from evidently.core import ColumnType
+from evidently.descriptors import OOV
+from evidently.descriptors import NonLetterCharacterPercentage
+from evidently.descriptors import TextLength
+from evidently.features.generated_features import FeatureDescriptor
+from evidently.features.generated_features import GeneratedFeature
+from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
-from evidently.renderers.html_widgets import GraphData
 from evidently.renderers.html_widgets import WidgetSize
-from evidently.renderers.html_widgets import plotly_graph_tabs
+from evidently.renderers.html_widgets import header_text
+from evidently.renderers.html_widgets import plotly_figure
+from evidently.renderers.render_utils import get_distribution_plot_figure
 from evidently.utils.data_operations import process_columns
+from evidently.utils.data_operations import recognize_column_type
+from evidently.utils.data_preprocessing import DataDefinition
+from evidently.utils.visualizations import get_distribution_for_column
 
 
-class ClassificationProbDistributionResults(MetricResult):
-    class Config:
-        dict_include = False
-        pd_include = False
-
-    current_distribution: Optional[Dict[str, list]]  # todo use DistributionField?
-    reference_distribution: Optional[Dict[str, list]]
-
-
-class ClassificationProbDistribution(Metric[ClassificationProbDistributionResults]):
-    @staticmethod
-    def get_distribution(dataset: pd.DataFrame, target_name: str, prediction_labels: Iterable) -> Dict[str, list]:
-        result = {}
-        dataset.replace([np.inf, -np.inf], np.nan, inplace=True)
-        for label in prediction_labels:
-            result[label] = [
-                dataset[dataset[target_name] == label][label],
-                dataset[dataset[target_name] != label][label],
-            ]
-
-        return result
-
-    def calculate(self, data: InputData) -> ClassificationProbDistributionResults:
-        columns = process_columns(data.current_data, data.column_mapping)
-        prediction = columns.utility_columns.prediction
-        target = columns.utility_columns.target
+class TextDescriptorsDistributionResult(MetricResult):
+    column_name: str
+    current: Dict[str, Distribution]
+    reference: Optional[Dict[str, Distribution]] = None
 
-        if target is None:
-            raise ValueError("Target column should be present")
 
-        if prediction is None:
-            raise ValueError("Prediction column should be present")
+class TextDescriptorsDistribution(Metric[TextDescriptorsDistributionResult]):
+    """Calculates distribution for the column"""
 
-        prediction_data = get_prediction_data(data.current_data, columns, data.column_mapping.pos_label)
-        if prediction_data.prediction_probas is None:
-            current_distribution = None
-            reference_distribution = None
+    column_name: str
+    generated_text_features: Dict[str, GeneratedFeature]
 
+    def __init__(self, column_name: str, descriptors: Optional[Dict[str, FeatureDescriptor]] = None) -> None:
+        self.column_name = column_name
+        if descriptors:
+            self.descriptors = descriptors
         else:
-            current_data_copy = data.current_data.copy()
-            for col in prediction_data.prediction_probas.columns:
-                current_data_copy[col] = prediction_data.prediction_probas[col]
-
-            current_distribution = self.get_distribution(
-                current_data_copy, target, prediction_data.prediction_probas.columns
-            )
+            self.descriptors = {
+                "Text Length": TextLength(),
+                "Non Letter Character %": NonLetterCharacterPercentage(),
+                "OOV %": OOV(),
+            }
+        self.generated_text_features = {}
+
+    def required_features(self, data_definition: DataDefinition):
+        column_type = data_definition.get_column(self.column_name).column_type
+        if column_type == ColumnType.Text:
+            self.generated_text_features = {
+                name: desc.feature(self.column_name) for name, desc in self.descriptors.items()
+            }
+            return list(self.generated_text_features.values())
+        return []
+
+    def get_parameters(self) -> tuple:
+        return (self.column_name,)
+
+    def calculate(self, data: InputData) -> TextDescriptorsDistributionResult:
+        current_results = {}
+        reference_results: Optional[Dict[str, Distribution]] = None
+        if data.reference_data is not None:
+            reference_results = {}
+        if self.column_name not in data.current_data:
+            raise ValueError(f"Column '{self.column_name}' was not found in current data.")
+
+        if data.reference_data is not None:
+            if self.column_name not in data.reference_data:
+                raise ValueError(f"Column '{self.column_name}' was not found in reference data.")
 
+        columns = process_columns(data.current_data, data.column_mapping)
+        column_type = recognize_column_type(dataset=data.current_data, column_name=self.column_name, columns=columns)
+        if column_type != "text":
+            raise ValueError("Text column expected")
+        for key, val in self.generated_text_features.items():
+            current_column = data.get_current_column(val.feature_name())
+            reference_column = None
             if data.reference_data is not None:
-                reference_data_copy = data.reference_data.copy()
-                for col in prediction_data.prediction_probas.columns:
-                    reference_data_copy[col] = prediction_data.prediction_probas[col]
-                reference_distribution = self.get_distribution(
-                    reference_data_copy, target, prediction_data.prediction_probas.columns
-                )
-
-            else:
-                reference_distribution = None
-
-        return ClassificationProbDistributionResults(
-            current_distribution=current_distribution,
-            reference_distribution=reference_distribution,
+                reference_column = data.get_reference_column(val.feature_name())
+            current, reference = get_distribution_for_column(
+                column_type="num",
+                current=current_column,
+                reference=reference_column,
+            )
+            current_results[key] = current
+            if reference_results is not None and reference is not None:
+                reference_results[key] = reference
+
+        return TextDescriptorsDistributionResult(
+            column_name=self.column_name,
+            current=current_results,
+            reference=reference_results,
         )
 
 
-@default_renderer(wrap_type=ClassificationProbDistribution)
-class ClassificationProbDistributionRenderer(MetricRenderer):
-    def _plot(self, distribution: Dict[str, list]):
-        # plot distributions
-        graphs = []
-
-        for label in distribution:
-            pred_distr = ff.create_distplot(
-                distribution[label],
-                [str(label), "other"],
-                colors=[
-                    self.color_options.primary_color,
-                    self.color_options.secondary_color,
-                ],
-                bin_size=0.05,
-                show_curve=False,
-                show_rug=True,
-            )
-
-            pred_distr.update_layout(
-                xaxis_title="Probability",
-                yaxis_title="Share",
-                legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1),
-            )
-            pred_distr_json = pred_distr.to_plotly_json()
-            graphs.append(
-                {
-                    "title": str(label),
-                    "data": pred_distr_json["data"],
-                    "layout": pred_distr_json["layout"],
-                }
-            )
-        return graphs
-
-    def render_html(self, obj: ClassificationProbDistribution) -> List[BaseWidgetInfo]:
+@default_renderer(wrap_type=TextDescriptorsDistribution)
+class TextDescriptorsDistributionRenderer(MetricRenderer):
+    def render_html(self, obj: TextDescriptorsDistribution) -> List[BaseWidgetInfo]:
         metric_result = obj.get_result()
-        reference_distribution = metric_result.reference_distribution
-        current_distribution = metric_result.current_distribution
-        result = []
-        size = WidgetSize.FULL
-
-        if reference_distribution is not None:
-            size = WidgetSize.HALF
-
-        if current_distribution is not None:
-            result.append(
-                plotly_graph_tabs(
-                    title="Current: Probability Distribution",
-                    size=size,
-                    figures=[
-                        GraphData(graph["title"], graph["data"], graph["layout"])
-                        for graph in self._plot(current_distribution)
-                    ],
-                )
-            )
-
-        if reference_distribution is not None:
-            result.append(
-                plotly_graph_tabs(
-                    title="Reference: Probability Distribution",
-                    size=size,
-                    figures=[
-                        GraphData(graph["title"], graph["data"], graph["layout"])
-                        for graph in self._plot(reference_distribution)
-                    ],
-                )
+        result = [header_text(label=f"Distribution for column '{metric_result.column_name}'.")]
+        for col in list(metric_result.current.keys()):
+            reference = None
+            if metric_result.reference is not None:
+                reference = metric_result.reference[col]
+            distr_fig = get_distribution_plot_figure(
+                current_distribution=metric_result.current[col],
+                reference_distribution=reference,
+                color_options=self.color_options,
             )
+            result.append(plotly_figure(title=col, figure=distr_fig, size=WidgetSize.FULL))
 
         return result
```

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/quality_by_class_metric.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_class_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 import plotly.figure_factory as ff
 import sklearn
 from plotly import graph_objs as go
 from plotly.subplots import make_subplots
 
 from evidently.base_metric import InputData
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.metric_results import DatasetColumns
 from evidently.metrics.classification_performance.base_classification_metric import ThresholdClassificationMetric
 from evidently.metrics.classification_performance.objects import ClassesMetrics
 from evidently.metrics.classification_performance.objects import ClassificationReport
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.utils.data_operations import process_columns
 
 
-class ClassificationQuality(MetricResultField):
+class ClassificationQuality(MetricResult):
     metrics: ClassesMetrics
     roc_aucs: Optional[List[float]]
 
     @property
     def metrics_dict(self):
         return self.dict(include={"metrics"})["metrics"]
 
@@ -135,14 +134,15 @@
         if reference_metrics is not None:
             ref_metrics_frame = pd.DataFrame(reference_metrics)
             z = ref_metrics_frame.iloc[:-1].values
             x = list(map(str, names))
             y = ["precision", "recall", "f1-score"]
 
             if current_roc_aucs is not None and len(current_roc_aucs) > 2:
+                assert reference_roc_aucs is not None
                 z = np.append(z, [reference_roc_aucs], axis=0)
                 y.append("roc-auc")
 
             z_text = [[str(round(y, 3)) for y in x] for x in z]
             trace = go.Heatmap(
                 z=z,
                 x=x,
```

### Comparing `evidently-0.2.8/src/evidently/metrics/classification_performance/quality_by_feature_table.py` & `evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_feature_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import plotly.express as px
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.classification_performance import get_prediction_data
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
 from evidently.metric_results import PredictionData
 from evidently.metric_results import StatsByFeature
 from evidently.model.widget import AdditionalGraphInfo
@@ -150,24 +149,26 @@
                         axis=1,
                     )
         table_columns = columns + [target_name]
         if isinstance(prediction_name, str):
             table_columns += [prediction_name]
         if isinstance(prediction_name, list):
             table_columns += prediction_name
-
+        reference = None
+        if ref_df is not None:
+            reference = StatsByFeature(
+                plot_data=ref_df[table_columns],
+                predictions=ref_predictions,
+            )
         return ClassificationQualityByFeatureTableResults(
             current=StatsByFeature(
                 plot_data=curr_df[table_columns],
                 predictions=curr_predictions,
             ),
-            reference=StatsByFeature(
-                plot_data=None if ref_df is None else ref_df[table_columns],
-                predictions=ref_predictions,
-            ),
+            reference=reference,
             columns=columns,
             target_name=target_name,
         )
 
 
 @default_renderer(wrap_type=ClassificationQualityByFeatureTable)
 class ClassificationQualityByFeatureTableRenderer(MetricRenderer):
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_drift/column_drift_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_drift/column_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/data_drift/column_value_plot.py` & `evidently-0.3.0/src/evidently/metrics/data_drift/column_value_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 from plotly import graph_objs as go
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
+from evidently.core import IncludeTags
 from evidently.metric_results import ColumnScatter
 from evidently.metric_results import column_scatter_from_df
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import plotly_figure
@@ -20,14 +21,15 @@
 
 
 class ColumnValuePlotResults(MetricResult):
     class Config:
         smart_union = True
         dict_include = False
         pd_include = False
+        tags = {IncludeTags.Render}
 
     column_name: str
     datetime_column_name: Optional[str]
     current: ColumnScatter
     reference: ColumnScatter
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_drift/dataset_drift_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_drift/dataset_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 
 
-class TextDomainField(MetricResultField):
+class TextDomainField(MetricResult):
     characteristic_examples: Optional[List[str]]
     characteristic_words: Optional[List[str]]
 
 
 class TextDomainClassifierDriftResult(MetricResult):
     text_column_name: str
     domain_classifier_roc_auc: float
@@ -61,15 +60,15 @@
 
         pipeline.fit(X_train, y_train)
         y_pred_proba = pipeline.predict_proba(X_test)[:, 1]
         roc_auc = roc_auc_score(y_test, y_pred_proba)
         return roc_auc, y_pred_proba, pipeline
 
     @staticmethod
-    def roc_auc_random_classifier_percentile(y_test: np.array, p_value=0.05, iter_num=1000, seed=42) -> float:
+    def roc_auc_random_classifier_percentile(y_test: np.ndarray, p_value=0.05, iter_num=1000, seed=42) -> float:
         def calc_roc_auc_random(y_test, seed=None):
             np.random.seed(seed)
             y_random_pred = np.random.rand(len(y_test))
             roc_auc_random = roc_auc_score(y_test, y_random_pred)
             return roc_auc_random
 
         np.random.seed(seed)
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_integrity/column_missing_values_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_integrity/column_missing_values_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 
 
-class ColumnMissingValues(MetricResultField):
+class ColumnMissingValues(MetricResult):
     """Statistics about missing values in a column"""
 
     # count of rows in the column
     number_of_rows: int
     # set of different missed values in the column
     different_missing_values: Dict[Any, int]
     # number of different missed values in the column
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_integrity/column_regexp_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_integrity/column_regexp_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 from typing import Pattern
 
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.data_quality import get_rows_count
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 
 
-class DataIntegrityValueByRegexpStat(MetricResultField):
+class DataIntegrityValueByRegexpStat(MetricResult):
     """Statistics about matched by a regular expression values in a column for one dataset"""
 
     # count of matched values in the column, without NaNs
     number_of_matched: int
     # count of not matched values in the column, without NaNs
     number_of_not_matched: int
     # count of rows in the column, including matched, not matched and NaNs
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_integrity/column_summary_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_integrity/column_summary_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_string_dtype
 
 from evidently.base_metric import ColumnMetric
 from evidently.base_metric import ColumnMetricResult
 from evidently.base_metric import InputData
-from evidently.base_metric import MetricResultField
+from evidently.base_metric import MetricResult
 from evidently.calculations.data_quality import DataQualityGetPlotData
 from evidently.calculations.data_quality import FeatureQualityStats
 from evidently.calculations.data_quality import get_features_stats
 from evidently.core import ColumnType
+from evidently.core import IncludeTags
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
 from evidently.metric_results import Histogram
 from evidently.model.widget import AdditionalGraphInfo
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
@@ -35,15 +36,15 @@
 from evidently.utils.visualizations import plot_distr
 from evidently.utils.visualizations import plot_distr_with_log_button
 from evidently.utils.visualizations import plot_num_feature_in_time
 from evidently.utils.visualizations import plot_num_num_rel
 from evidently.utils.visualizations import plot_time_feature_distr
 
 
-class ColumnCharacteristics(MetricResultField):
+class ColumnCharacteristics(MetricResult):
     number_of_rows: int
     count: int
     missing: Optional[int]
     missing_percentage: Optional[float]
 
 
 class NumericCharacteristics(ColumnCharacteristics):
@@ -88,48 +89,48 @@
     oov_mean: Optional[float]
     oov_max: Optional[float]
     non_letter_char_min: Optional[float]
     non_letter_char_mean: Optional[float]
     non_letter_char_max: Optional[float]
 
 
-class DataInTime(MetricResultField):
+class DataInTime(MetricResult):
     data_for_plots: Dict[str, Optional[pd.DataFrame]]
     freq: str
     datetime_name: str
 
 
-class DataByTarget(MetricResultField):
+class DataByTarget(MetricResult):
     data_for_plots: Union[
         Dict[
             str,
             Union[
                 Dict[str, Union[list, pd.DataFrame, np.ndarray, pd.Categorical]],
                 pd.DataFrame,
             ],
         ],
         None,
     ]
     target_name: str
     target_type: str
 
 
-class DataQualityPlot(MetricResultField):
+class DataQualityPlot(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     bins_for_hist: Optional[Histogram]
     data_in_time: Optional[DataInTime]
     data_by_target: Optional[DataByTarget]
     counts_of_values: Optional[Dict[str, pd.DataFrame]]
 
 
 class ColumnSummaryResult(ColumnMetricResult):
     class Config:
-        pd_exclude_fields = {"plot_data"}
         pd_name_mapping = {
             "reference_characteristics": "ref",
             "current_characteristics": "cur",
         }
 
     reference_characteristics: Optional[ColumnCharacteristics]
     current_characteristics: ColumnCharacteristics
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.data_quality import get_rows_count
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import HistogramData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import histogram
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 
 
-class DatasetMissingValues(MetricResultField):
+class DatasetMissingValues(MetricResult):
     """Statistics about missed values in a dataset"""
 
     # set of different missing values in the dataset
     different_missing_values: Dict[Any, int]
     # number of different missing values in the dataset
     number_of_different_missing_values: int
     # set of different missing values for each column
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_integrity/dataset_summary_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_summary_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import pandas as pd
 
 from evidently import ColumnMapping
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.data_integration import get_number_of_all_pandas_missed_values
 from evidently.calculations.data_integration import get_number_of_almost_constant_columns
 from evidently.calculations.data_integration import get_number_of_almost_duplicated_columns
 from evidently.calculations.data_integration import get_number_of_constant_columns
 from evidently.calculations.data_integration import get_number_of_duplicated_columns
 from evidently.calculations.data_integration import get_number_of_empty_columns
 from evidently.calculations.data_quality import get_rows_count
@@ -22,15 +21,15 @@
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
 from evidently.utils.data_operations import process_columns
 
 
-class DatasetSummary(MetricResultField):
+class DatasetSummary(MetricResult):
     """Columns information in a dataset"""
 
     class Config:
         dict_exclude_fields = {"columns_type"}
         pd_exclude_fields = {"columns_type"}
 
     target: Optional[str]
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/column_correlations_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/column_correlations_metric.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,103 @@
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Union
 
 import pandas as pd
 
-from evidently import ColumnMapping
+from evidently.base_metric import ColumnName
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.calculations.data_quality import calculate_category_column_correlations
-from evidently.calculations.data_quality import calculate_numerical_column_correlations
+from evidently.calculations.data_quality import calculate_category_correlation
+from evidently.calculations.data_quality import calculate_numerical_correlation
+from evidently.core import ColumnType
 from evidently.metric_results import ColumnCorrelations
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import get_histogram_for_distribution
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import widget_tabs
-from evidently.utils.data_operations import process_columns
-from evidently.utils.data_operations import recognize_column_type
+from evidently.utils.data_preprocessing import DataDefinition
 
 
 class ColumnCorrelationsMetricResult(MetricResult):
     column_name: str
     current: Dict[str, ColumnCorrelations]
     reference: Optional[Dict[str, ColumnCorrelations]] = None
 
 
 class ColumnCorrelationsMetric(Metric[ColumnCorrelationsMetricResult]):
     """Calculates correlations between the selected column and all the other columns.
     In the current and reference (if presented) datasets"""
 
-    column_name: str
+    column_name: ColumnName
 
-    def __init__(self, column_name: str) -> None:
-        self.column_name = column_name
+    def __init__(self, column_name: Union[str, ColumnName]) -> None:
+        if isinstance(column_name, ColumnName):
+            self.column_name = column_name
+        else:
+            self.column_name = ColumnName.main_dataset(column_name)
 
     @staticmethod
     def _calculate_correlation(
-        column_name: str, dataset: pd.DataFrame, column_mapping: ColumnMapping
+        column_name: ColumnName,
+        column_data: pd.Series,
+        dataset: pd.DataFrame,
+        data_definition: DataDefinition,
+        column_type: ColumnType,
     ) -> Dict[str, ColumnCorrelations]:
-        columns = process_columns(dataset, column_mapping)
-        column_type = recognize_column_type(dataset=dataset, column_name=column_name, columns=columns)
-
-        if column_type == "cat":
-            correlation_columns = [name for name in columns.cat_feature_names if name != column_name]
-            return calculate_category_column_correlations(column_name, dataset, correlation_columns)
-
-        elif column_type == "num":
-            correlation_columns = [name for name in columns.num_feature_names if name != column_name]
-            return calculate_numerical_column_correlations(column_name, dataset, correlation_columns)
+        if column_type == ColumnType.Categorical:
+            cat_features = data_definition.get_columns("categorical_features")
 
+            correlations = calculate_category_correlation(
+                column_name.display_name,
+                column_data,
+                dataset[[feature.column_name for feature in cat_features if feature.column_name != column_name.name]],
+            )
+        elif column_type == ColumnType.Numerical:
+            num_features = data_definition.get_columns("numerical_features")
+            correlations = calculate_numerical_correlation(
+                column_name.display_name,
+                column_data,
+                dataset[[feature.column_name for feature in num_features if feature.column_name != column_name.name]],
+            )
         else:
             raise ValueError(f"Cannot calculate correlations for '{column_type}' column type.")
+        return {corr.kind: corr for corr in correlations}
 
     def calculate(self, data: InputData) -> ColumnCorrelationsMetricResult:
-        if self.column_name not in data.current_data:
-            raise ValueError(f"Column '{self.column_name}' was not found in current data.")
+        if not data.has_column(self.column_name):
+            raise ValueError(f"Column '{self.column_name.name}' was not found in data.")
 
-        if data.reference_data is not None:
-            if self.column_name not in data.reference_data:
-                raise ValueError(f"Column '{self.column_name}' was not found in reference data.")
-
-        current_correlations = self._calculate_correlation(self.column_name, data.current_data, data.column_mapping)
-
-        if data.reference_data is not None:
-            reference_correlations: Optional[Dict[str, ColumnCorrelations]] = self._calculate_correlation(
-                self.column_name, data.reference_data, data.column_mapping
-            )
+        column_type, current_data, reference_data = data.get_data(self.column_name)
 
-        else:
-            reference_correlations = None
+        current_correlations = self._calculate_correlation(
+            self.column_name,
+            current_data,
+            data.current_data,
+            data.data_definition,
+            column_type,
+        )
+
+        reference_correlations = None
+        if reference_data is not None:
+            reference_correlations = self._calculate_correlation(
+                self.column_name,
+                reference_data,
+                data.reference_data,
+                data.data_definition,
+                column_type,
+            )
 
         return ColumnCorrelationsMetricResult(
-            column_name=self.column_name,
+            column_name=self.column_name.display_name,
             current=current_correlations,
             reference=reference_correlations if reference_correlations is not None else None,
         )
 
 
 @default_renderer(wrap_type=ColumnCorrelationsMetric)
 class ColumnCorrelationsMetricRenderer(MetricRenderer):
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/column_distribution_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/column_distribution_metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 from typing import List
 from typing import Optional
+from typing import Union
 
+from evidently.base_metric import ColumnName
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
+from evidently.core import ColumnType
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.renderers.render_utils import get_distribution_plot_figure
-from evidently.utils.data_operations import process_columns
-from evidently.utils.data_operations import recognize_column_type
 from evidently.utils.visualizations import get_distribution_for_column
 
 
 class ColumnDistributionMetricResult(MetricResult):
     column_name: str
     current: Distribution
     reference: Optional[Distribution] = None
 
 
 class ColumnDistributionMetric(Metric[ColumnDistributionMetricResult]):
     """Calculates distribution for the column"""
 
-    column_name: str
+    column_name: ColumnName
 
-    def __init__(self, column_name: str) -> None:
-        self.column_name = column_name
+    def __init__(self, column_name: Union[str, ColumnName]) -> None:
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
 
     def calculate(self, data: InputData) -> ColumnDistributionMetricResult:
-        if self.column_name not in data.current_data:
-            raise ValueError(f"Column '{self.column_name}' was not found in current data.")
-
-        if data.reference_data is not None:
-            if self.column_name not in data.reference_data:
-                raise ValueError(f"Column '{self.column_name}' was not found in reference data.")
+        if not data.has_column(self.column_name):
+            raise ValueError(f"Column '{self.column_name.display_name}' was not found in data.")
 
-        columns = process_columns(data.current_data, data.column_mapping)
-        column_type = recognize_column_type(dataset=data.current_data, column_name=self.column_name, columns=columns)
-        current_column = data.current_data[self.column_name]
+        if not self.column_name.is_main_dataset():
+            column_type = ColumnType.Numerical
+        else:
+            column_type = data.data_definition.get_column(self.column_name.name).column_type
+        current_column = data.get_current_column(self.column_name)
         reference_column = None
         if data.reference_data is not None:
-            reference_column = data.reference_data[self.column_name]
+            reference_column = data.get_reference_column(self.column_name)
         current, reference = get_distribution_for_column(
-            column_type=column_type,
+            column_type=column_type.value,
             current=current_column,
             reference=reference_column,
         )
 
         return ColumnDistributionMetricResult(
-            column_name=self.column_name,
+            column_name=self.column_name.display_name,
             current=current,
             reference=reference,
         )
 
 
 @default_renderer(wrap_type=ColumnDistributionMetric)
 class ColumnDistributionMetricRenderer(MetricRenderer):
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/column_quantile_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/column_quantile_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from typing import Optional
 
 import pandas as pd
 
 from evidently.base_metric import ColumnMetricResult
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
-from evidently.base_metric import MetricResultField
+from evidently.base_metric import MetricResult
 from evidently.core import ColumnType
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import HistogramData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import get_histogram_figure_with_quantile
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.utils.visualizations import get_distribution_for_column
 
 
-class QuantileStats(MetricResultField):
+class QuantileStats(MetricResult):
     value: float
     # calculated value of the quantile
     distribution: Distribution
     # distribution for the column
 
 
 class ColumnQuantileMetricResult(ColumnMetricResult):
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/column_value_list_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/column_value_list_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 from typing import Optional
 
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.data_quality import get_rows_count
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 
 
-class ValueListStat(MetricResultField):
+class ValueListStat(MetricResult):
     number_in_list: int
     number_not_in_list: int
     share_in_list: float
     share_not_in_list: float
     values_in_list: Dict[Any, int]
     values_not_in_list: Dict[Any, int]
     rows_count: int
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/column_value_range_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/column_value_range_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import dataclasses
 from typing import List
 from typing import Optional
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
+from evidently.base_metric import ColumnName
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.data_quality import get_rows_count
+from evidently.core import ColumnType
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import HistogramData
 from evidently.renderers.html_widgets import TabData
@@ -23,15 +24,15 @@
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.types import Numeric
 from evidently.utils.visualizations import get_distribution_for_column
 
 
-class ValuesInRangeStat(MetricResultField):
+class ValuesInRangeStat(MetricResult):
     number_in_range: int
     number_not_in_range: int
     share_in_range: float
     share_not_in_range: float
     # number of rows without null-like values
     number_of_values: int
     distribution: Distribution
@@ -44,19 +45,24 @@
     current: ValuesInRangeStat
     reference: Optional[ValuesInRangeStat] = None
 
 
 class ColumnValueRangeMetric(Metric[ColumnValueRangeMetricResult]):
     """Calculates count and shares of values in the predefined values range"""
 
-    column_name: str
+    column_name: Union[str, ColumnName]
     left: Optional[Numeric]
     right: Optional[Numeric]
 
-    def __init__(self, column_name: str, left: Optional[Numeric] = None, right: Optional[Numeric] = None) -> None:
+    def __init__(
+        self,
+        column_name: Union[str, ColumnName],
+        left: Optional[Numeric] = None,
+        right: Optional[Numeric] = None,
+    ) -> None:
         self.left = left
         self.right = right
         self.column_name = column_name
 
     @staticmethod
     def _calculate_in_range_stats(
         column: pd.Series, left: Numeric, right: Numeric, distribution: Distribution
@@ -82,66 +88,54 @@
             share_in_range=share_in_range,
             share_not_in_range=share_not_in_range,
             number_of_values=rows_count,
             distribution=distribution,
         )
 
     def calculate(self, data: InputData) -> ColumnValueRangeMetricResult:
-        if self.column_name not in data.current_data:
-            raise ValueError(f"Column {self.column_name} is not in current data.")
-
-        if not pd.api.types.is_numeric_dtype(data.current_data[self.column_name].dtype):
-            raise ValueError(f"Column {self.column_name} in current data should be numeric.")
-
-        if data.reference_data is not None:
-            if self.column_name not in data.reference_data:
-                raise ValueError(f"Column {self.column_name} is not in reference data.")
-
-            if not pd.api.types.is_numeric_dtype(data.reference_data[self.column_name].dtype):
-                raise ValueError(f"Column {self.column_name} in reference data should be numeric.")
+        if not data.has_column(self.column_name):
+            raise ValueError(f"Column {self.column_name} isn't present in data")
+        column_type, current_data, reference_data = data.get_data(self.column_name)
+        if column_type != ColumnType.Numerical:
+            raise ValueError(f"Column {self.column_name} in reference data should be numeric.")
 
         if self.left is None:
-            if data.reference_data is None:
+            if reference_data is None:
                 raise ValueError("Reference should be present")
-
             else:
-                left: Numeric = float(data.reference_data[self.column_name].min())
+                left: Numeric = float(reference_data.min())
 
         else:
             left = self.left
 
         if self.right is None:
-            if data.reference_data is None:
+            if reference_data is None:
                 raise ValueError("Reference should be present")
-
             else:
-                right: Numeric = float(data.reference_data[self.column_name].max())
+                right: Numeric = float(reference_data.max())
 
         else:
             right = self.right
 
         # calculate distribution for visualisation
-        current_column = data.current_data[self.column_name]
         cur_distribution, ref_distribution = get_distribution_for_column(
             column_type="num",
-            current=current_column,
-            reference=data.reference_data[self.column_name] if data.reference_data is not None else None,
+            current=current_data,
+            reference=reference_data if reference_data is not None else None,
         )
 
-        current = self._calculate_in_range_stats(data.current_data[self.column_name], left, right, cur_distribution)
+        current = self._calculate_in_range_stats(current_data, left, right, cur_distribution)
         reference = None
-        if data.reference_data is not None:
+        if reference_data is not None:
             # always should be present
             assert ref_distribution is not None
-            reference = self._calculate_in_range_stats(
-                data.reference_data[self.column_name], left, right, ref_distribution
-            )
+            reference = self._calculate_in_range_stats(reference_data, left, right, ref_distribution)
 
         return ColumnValueRangeMetricResult(
-            column_name=self.column_name,
+            column_name=self.column_name if isinstance(self.column_name, str) else self.column_name.display_name,
             left=left,
             right=right,
             current=current,
             reference=reference,
         )
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/conflict_prediction_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/conflict_prediction_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import List
 from typing import Optional
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.utils.data_operations import process_columns
 
 
-class ConflictPredictionData(MetricResultField):
+class ConflictPredictionData(MetricResult):
     number_not_stable_prediction: int
     share_not_stable_prediction: float
 
 
 class ConflictPredictionMetricResults(MetricResult):
     current: ConflictPredictionData
     reference: Optional[ConflictPredictionData]
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/conflict_target_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/conflict_target_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/dataset_correlations_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/dataset_correlations_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.classification_performance import get_prediction_data
 from evidently.calculations.data_quality import calculate_correlations
 from evidently.core import ColumnType
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
 from evidently.model.widget import BaseWidgetInfo
@@ -28,23 +27,23 @@
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.data_operations import process_columns
 from evidently.utils.data_preprocessing import ColumnDefinition
 from evidently.utils.data_preprocessing import DataDefinition
 from evidently.utils.data_preprocessing import PredictionColumns
 
 
-class CorrelationStats(MetricResultField):
+class CorrelationStats(MetricResult):
     target_prediction_correlation: Optional[float] = None
     abs_max_target_features_correlation: Optional[float] = None
     abs_max_prediction_features_correlation: Optional[float] = None
     abs_max_correlation: Optional[float] = None
     abs_max_features_correlation: Optional[float] = None
 
 
-class DatasetCorrelation(MetricResultField):
+class DatasetCorrelation(MetricResult):
     class Config:
         dict_exclude_fields = {"correlation", "correlations_calculate"}
         pd_exclude_fields = {"correlation", "correlations_calculate"}
 
     correlation: Dict[str, pd.DataFrame]
     stats: Dict[str, CorrelationStats]
     correlations_calculate: Optional[Dict[str, pd.DataFrame]]
```

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/stability_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/stability_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py` & `evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 from typing import Optional
 
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.calculations.data_quality import calculate_numerical_column_correlations
+from evidently.calculations.data_quality import calculate_numerical_correlation
 from evidently.core import ColumnType as ColumnType_data
 from evidently.descriptors import OOV
 from evidently.descriptors import NonLetterCharacterPercentage
 from evidently.descriptors import TextLength
 from evidently.features.generated_features import FeatureDescriptor
 from evidently.features.generated_features import GeneratedFeature
 from evidently.metric_results import ColumnCorrelations
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import get_histogram_for_distribution
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import widget_tabs
-from evidently.utils.data_operations import process_columns
 from evidently.utils.data_preprocessing import DataDefinition
 
 
 class TextDescriptorsCorrelationMetricResult(MetricResult):
     column_name: str
     current: Dict[str, Dict[str, ColumnCorrelations]]
     reference: Optional[Dict[str, Dict[str, ColumnCorrelations]]] = None
@@ -66,29 +65,19 @@
         if self.column_name not in data.current_data:
             raise ValueError(f"Column '{self.column_name}' was not found in current data.")
 
         if data.reference_data is not None:
             if self.column_name not in data.reference_data:
                 raise ValueError(f"Column '{self.column_name}' was not found in reference data.")
 
-        columns = process_columns(data.current_data, data.column_mapping)
-        correlation_columns = columns.num_feature_names
-
         curr_text_df = pd.concat(
             [data.get_current_column(x.feature_name()) for x in list(self.generated_text_features.values())],
             axis=1,
         )
         curr_text_df.columns = list(self.generated_text_features.keys())
-        curr_df = pd.concat(
-            [
-                data.current_data.copy().reset_index(drop=True),
-                curr_text_df.reset_index(drop=True),
-            ],
-            axis=1,
-        )
         ref_df = None
         if data.reference_data is not None:
             ref_text_df = pd.concat(
                 [data.get_reference_column(x.feature_name()) for x in list(self.generated_text_features.values())],
                 axis=1,
             )
             ref_text_df.columns = list(self.generated_text_features.keys())
@@ -100,18 +89,29 @@
                 axis=1,
             )
         curr_result = {}
         ref_result: Optional[dict] = None
         if ref_df is not None:
             ref_result = {}
 
-        for col in list(self.generated_text_features.keys()):
-            curr_result[col] = calculate_numerical_column_correlations(col, curr_df, correlation_columns)
+        num_features = data.data_definition.get_columns("numerical_features")
+        for name, feature in self.generated_text_features.items():
+            correlations = calculate_numerical_correlation(
+                name,
+                data.get_current_column(feature.feature_name()),
+                data.current_data[[feature.column_name for feature in num_features]],
+            )
+            curr_result[name] = {value.kind: value for value in correlations}
             if ref_df is not None and ref_result is not None:
-                ref_result[col] = calculate_numerical_column_correlations(col, ref_df, correlation_columns)
+                correlations = calculate_numerical_correlation(
+                    name,
+                    data.get_reference_column(feature.feature_name()),
+                    data.current_data[[feature.column_name for feature in num_features]],
+                )
+                ref_result[name] = {value.kind: value for value in correlations}
 
         # todo potential performance issues
         return TextDescriptorsCorrelationMetricResult(
             column_name=self.column_name,
             current=curr_result,
             reference=ref_result,
         )
```

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/error_bias_table.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/error_bias_table.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/error_distribution.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/error_distribution.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/error_in_time.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/error_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/objects.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Dict
 from typing import Optional
 from typing import overload
 
-from evidently.base_metric import MetricResultField
+from evidently.base_metric import MetricResult
 from evidently.metric_results import ScatterData
 
 
-class PredActualScatter(MetricResultField):
+class PredActualScatter(MetricResult):
     predicted: ScatterData
     actual: ScatterData
 
 
 @overload
 def scatter_as_dict(scatter: PredActualScatter) -> Dict[str, ScatterData]:
     ...
@@ -23,21 +23,21 @@
 
 def scatter_as_dict(scatter: Optional[PredActualScatter]) -> Optional[Dict[str, ScatterData]]:
     if scatter is None:
         return None
     return scatter.dict()
 
 
-class RegressionScatter(MetricResultField):
+class RegressionScatter(MetricResult):
     underestimation: PredActualScatter
     majority: PredActualScatter
     overestimation: PredActualScatter
 
 
-class RegressionMetricScatter(MetricResultField):
+class RegressionMetricScatter(MetricResult):
     current: ScatterData
     reference: Optional[ScatterData] = None
 
     def __mul__(self, other: float):
         # todo: will fail if data is not Series
         if isinstance(self.current, list) or isinstance(self.reference, list):
             return RegressionMetricScatter(
@@ -45,12 +45,12 @@
                 reference=[x * other for x in self.reference] if self.reference is not None else None,
             )
         return RegressionMetricScatter(
             current=self.current * other, reference=self.reference * other if self.reference is not None else None
         )
 
 
-class RegressionMetricsScatter(MetricResultField):
+class RegressionMetricsScatter(MetricResult):
     r2_score: RegressionMetricScatter
     rmse: RegressionMetricScatter
     mean_abs_error: RegressionMetricScatter
     mean_abs_perc_error: RegressionMetricScatter
```

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_vs_actual.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,53 @@
-import dataclasses
-from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Union
 
 import numpy as np
-import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.metric_results import ColumnScatter
-from evidently.metric_results import ColumnScatterResult
+from evidently.core import IncludeTags
+from evidently.metrics.regression_performance.objects import PredActualScatter
+from evidently.metrics.regression_performance.objects import scatter_as_dict
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.utils.data_operations import process_columns
-from evidently.utils.visualizations import plot_pred_actual_time
+from evidently.utils.visualizations import plot_scatter
 
 
-class RegressionPredictedVsActualPlot(Metric[ColumnScatterResult]):
-    def calculate(self, data: InputData) -> ColumnScatterResult:
+class RegressionPredictedVsActualScatterResults(MetricResult):
+    class Config:
+        dict_include = False
+        tags = {IncludeTags.Render}
+
+    current: PredActualScatter
+    reference: Optional[PredActualScatter]
+
+
+class RegressionPredictedVsActualScatter(Metric[RegressionPredictedVsActualScatterResults]):
+    def calculate(self, data: InputData) -> RegressionPredictedVsActualScatterResults:
         dataset_columns = process_columns(data.current_data, data.column_mapping)
         target_name = dataset_columns.utility_columns.target
         prediction_name = dataset_columns.utility_columns.prediction
-        datetime_column_name = dataset_columns.utility_columns.date
         curr_df = data.current_data
         ref_df = data.reference_data
         if target_name is None or prediction_name is None:
             raise ValueError("The columns 'target' and 'prediction' columns should be present")
         if not isinstance(prediction_name, str):
             raise ValueError("Expect one column for prediction. List of columns was provided.")
-        curr_df = self._make_df_for_plot(curr_df, target_name, prediction_name, datetime_column_name)
-        current_scatter = {}
-        current_scatter["Predicted"] = curr_df[prediction_name]
-        current_scatter["Actual"] = curr_df[target_name]
-        if datetime_column_name is not None:
-            current_scatter["x"] = curr_df[datetime_column_name]
-            x_name = "Timestamp"
-        else:
-            current_scatter["x"] = curr_df.index
-            x_name = "Index"
-
-        reference_scatter: Optional[dict] = None
+        curr_df = self._make_df_for_plot(curr_df, target_name, prediction_name, None)
+        current_scatter = PredActualScatter(predicted=curr_df[prediction_name], actual=curr_df[target_name])
+        reference_scatter: Optional[PredActualScatter] = None
         if data.reference_data is not None:
-            ref_df = self._make_df_for_plot(ref_df, target_name, prediction_name, datetime_column_name)
-            reference_scatter = {}
-            reference_scatter["Predicted"] = ref_df[prediction_name]
-            reference_scatter["Actual"] = ref_df[target_name]
-            reference_scatter["x"] = ref_df[datetime_column_name] if datetime_column_name else ref_df.index
-        return ColumnScatterResult(
-            current=current_scatter,
-            reference=reference_scatter,
-            x_name=x_name,
-        )
+            ref_df = self._make_df_for_plot(ref_df, target_name, prediction_name, None)
+            reference_scatter = PredActualScatter(predicted=ref_df[prediction_name], actual=ref_df[target_name])
+        return RegressionPredictedVsActualScatterResults(current=current_scatter, reference=reference_scatter)
 
     def _make_df_for_plot(self, df, target_name: str, prediction_name: str, datetime_column_name: Optional[str]):
         result = df.replace([np.inf, -np.inf], np.nan)
         if datetime_column_name is not None:
             result.dropna(
                 axis=0,
                 how="any",
@@ -66,32 +55,32 @@
                 subset=[target_name, prediction_name, datetime_column_name],
             )
             return result.sort_values(datetime_column_name)
         result.dropna(axis=0, how="any", inplace=True, subset=[target_name, prediction_name])
         return result.sort_index()
 
 
-@default_renderer(wrap_type=RegressionPredictedVsActualPlot)
-class RegressionPredictedVsActualPlotRenderer(MetricRenderer):
-    def render_html(self, obj: RegressionPredictedVsActualPlot) -> List[BaseWidgetInfo]:
+@default_renderer(wrap_type=RegressionPredictedVsActualScatter)
+class RegressionPredictedVsActualScatterRenderer(MetricRenderer):
+    def render_html(self, obj: RegressionPredictedVsActualScatter) -> List[BaseWidgetInfo]:
         result = obj.get_result()
         current_scatter = result.current
-        reference_scatter = None
-        if result.reference is not None:
-            reference_scatter = result.reference
-        fig = plot_pred_actual_time(
-            curr=current_scatter,
-            ref=reference_scatter,
-            x_name="x",
-            xaxis_name=result.x_name,
-            yaxis_name="Value",
+        reference_scatter = result.reference
+
+        fig = plot_scatter(
+            curr=scatter_as_dict(current_scatter),
+            ref=scatter_as_dict(reference_scatter),
+            x="actual",
+            y="predicted",
+            xaxis_name="Actual value",
+            yaxis_name="Predicted value",
             color_options=self.color_options,
         )
         return [
-            header_text(label="Predicted vs Actual in Time"),
+            header_text(label="Predicted vs Actual"),
             BaseWidgetInfo(
                 title="",
                 size=2,
                 type="big_graph",
                 params={"data": fig["data"], "layout": fig["layout"]},
             ),
         ]
```

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/regression_dummy_metric.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/regression_dummy_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/regression_performance_metrics.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/regression_performance_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from sklearn.metrics import mean_absolute_percentage_error
 from sklearn.metrics import mean_squared_error
 from sklearn.metrics import r2_score
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
 from evidently.calculations.regression_performance import calculate_regression_performance
 from evidently.metric_results import DatasetColumns
 from evidently.metric_results import Histogram
 from evidently.metrics.regression_performance.objects import RegressionMetricScatter
 from evidently.metrics.regression_performance.objects import RegressionMetricsScatter
 from evidently.metrics.regression_performance.utils import apply_func_to_binned_data
 from evidently.metrics.utils import make_target_bins_for_reg_plots
@@ -28,15 +27,15 @@
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.utils.data_operations import process_columns
 from evidently.utils.visualizations import make_hist_for_cat_plot
 from evidently.utils.visualizations import make_hist_for_num_plot
 
 
-class RegressionMetrics(MetricResultField):
+class RegressionMetrics(MetricResult):
     r2_score: float
     rmse: float
     mean_error: float
     mean_abs_error: float
     mean_abs_perc_error: float
     abs_error_max: float
     underperformance: dict
```

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/top_error.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/top_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
-from evidently.base_metric import MetricResultField
+from evidently.core import IncludeTags
 from evidently.metrics.regression_performance.objects import PredActualScatter
 from evidently.metrics.regression_performance.objects import RegressionScatter
 from evidently.metrics.regression_performance.visualization import plot_error_bias_colored_scatter
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.utils.data_operations import process_columns
 
 
-class TopData(MetricResultField):
+class TopData(MetricResult):
     mean_err_per_group: Dict[str, Dict[str, float]]
     scatter: RegressionScatter
 
 
 class RegressionTopErrorMetricResults(MetricResult):
     class Config:
         dict_include = False
+        tags = {IncludeTags.Render}
 
     current: TopData
     reference: Optional[TopData]
 
 
 class RegressionTopErrorMetric(Metric[RegressionTopErrorMetricResults]):
     def calculate(self, data: InputData) -> RegressionTopErrorMetricResults:
```

### Comparing `evidently-0.2.8/src/evidently/metrics/regression_performance/utils.py` & `evidently-0.3.0/src/evidently/metrics/regression_performance/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/metrics/utils.py` & `evidently-0.3.0/src/evidently/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/model/widget.py` & `evidently-0.3.0/src/evidently/model/widget.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/nbextension/static/index.js` & `evidently-0.3.0/src/evidently/nbextension/static/index.js`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/nbextension/static/index.js.LICENSE.txt` & `evidently-0.3.0/src/evidently/nbextension/static/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/nbextension/static/material-ui-icons.woff2` & `evidently-0.3.0/src/evidently/nbextension/static/material-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/options/__init__.py` & `evidently-0.3.0/src/evidently/options/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/options/color_scheme.py` & `evidently-0.3.0/src/evidently/options/color_scheme.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/options/data_drift.py` & `evidently-0.3.0/src/evidently/options/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/options/quality_metrics.py` & `evidently-0.3.0/src/evidently/options/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/pipeline/column_mapping.py` & `evidently-0.3.0/src/evidently/pipeline/column_mapping.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class TaskType:
     REGRESSION_TASK: str = "regression"
     CLASSIFICATION_TASK: str = "classification"
 
 
 TargetNames = Union[List[int], List[str], Dict[int, str], Dict[str, str]]
+Embeddings = Dict[str, List[str]]
 
 
 @dataclass
 class ColumnMapping:
     target: Optional[str] = "target"
     prediction: Optional[Union[str, int, Union[Sequence[str], Sequence[int]]]] = "prediction"
     datetime: Optional[str] = "datetime"
@@ -23,13 +24,14 @@
     numerical_features: Optional[List[str]] = None
     categorical_features: Optional[List[str]] = None
     datetime_features: Optional[List[str]] = None
     target_names: Optional[TargetNames] = None
     task: Optional[str] = None
     pos_label: Optional[Union[str, int]] = 1
     text_features: Optional[List[str]] = None
+    embeddings: Optional[Embeddings] = None
 
     def is_classification_task(self):
         return self.task == TaskType.CLASSIFICATION_TASK
 
     def is_regression_task(self):
         return self.task == TaskType.REGRESSION_TASK
```

### Comparing `evidently-0.2.8/src/evidently/renderers/base_renderer.py` & `evidently-0.3.0/src/evidently/renderers/base_renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options import ColorOptions
 
 if TYPE_CHECKING:
     from evidently.base_metric import Metric
     from evidently.base_metric import TResult
+    from evidently.core import IncludeOptions
+    from evidently.tests.base_test import Test
 
 
 class BaseRenderer:
     """Base class for all renderers"""
 
     color_options: ColorOptions
 
@@ -28,17 +30,23 @@
             self.color_options = color_options
 
 
 class MetricRenderer(BaseRenderer):
     def render_pandas(self, obj: "Metric[TResult]") -> pd.DataFrame:
         return obj.get_result().get_pandas()
 
-    def render_json(self, obj: "Metric[TResult]") -> dict:
+    def render_json(
+        self,
+        obj: "Metric[TResult]",
+        include_render: bool = False,
+        include: "IncludeOptions" = None,
+        exclude: "IncludeOptions" = None,
+    ) -> dict:
         result = obj.get_result()
-        return result.get_dict()
+        return result.get_dict(include_render=include_render, include=include, exclude=exclude)
 
     def render_html(self, obj) -> List[BaseWidgetInfo]:
         raise NotImplementedError()
 
 
 @dataclasses.dataclass
 class DetailsInfo:
@@ -57,39 +65,38 @@
 
     def with_details(self, title: str, info: BaseWidgetInfo):
         self.details.append(DetailsInfo(title, info))
         return self
 
 
 class TestRenderer(BaseRenderer):
-    def html_description(self, obj):
+    def html_description(self, obj: "Test"):
         return obj.get_result().description
 
-    def json_description(self, obj):
+    def json_description(self, obj: "Test"):
         return obj.get_result().description
 
     def render_html(self, obj) -> TestHtmlInfo:
         result = obj.get_result()
         return TestHtmlInfo(
             name=result.name,
             description=self.html_description(obj),
-            status=result.status,
+            status=result.status.value,
             details=[],
             groups=result.groups,
         )
 
-    def render_json(self, obj) -> dict:
-        result = obj.get_result()
-        return {
-            "name": result.name,
-            "description": self.json_description(obj),
-            "status": result.status,
-            "group": obj.group,
-            "parameters": {},
-        }
+    def render_json(
+        self,
+        obj: "Test",
+        include_render: bool = False,
+        include: "IncludeOptions" = None,
+        exclude: "IncludeOptions" = None,
+    ) -> dict:
+        return obj.get_result().get_dict(include_render=include_render, include=include, exclude=exclude)
 
 
 @dataclasses.dataclass
 class RenderersDefinitions:
     typed_renderers: dict = dataclasses.field(default_factory=dict)
     default_html_test_renderer: Optional[TestRenderer] = None
     default_html_metric_renderer: Optional[MetricRenderer] = None
```

### Comparing `evidently-0.2.8/src/evidently/renderers/html_widgets.py` & `evidently-0.3.0/src/evidently/renderers/html_widgets.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/renderers/notebook_utils.py` & `evidently-0.3.0/src/evidently/renderers/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/renderers/render_utils.py` & `evidently-0.3.0/src/evidently/renderers/render_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/report/report.py` & `evidently-0.3.0/src/evidently/report/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Union
 
 import pandas as pd
 
 from evidently import ColumnMapping
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
+from evidently.core import IncludeOptions
 from evidently.metric_preset.metric_preset import MetricPreset
 from evidently.metric_results import DatasetColumns
 from evidently.model.dashboard import DashboardInfo
 from evidently.model.widget import AdditionalGraphInfo
 from evidently.options import ColorOptions
 from evidently.renderers.base_renderer import DetailsInfo
 from evidently.suite.base_suite import Display
@@ -101,20 +102,37 @@
             ref_add,
             curr_add,
             column_mapping,
             data_definition,
         )
         self._inner_suite.run_calculate(data)
 
-    def as_dict(self) -> dict:
+    def as_dict(
+        self,
+        include_render: bool = False,
+        include: Dict[str, IncludeOptions] = None,
+        exclude: Dict[str, IncludeOptions] = None,
+    ) -> dict:
         metrics = []
-
+        include = include or {}
+        exclude = exclude or {}
         for metric in self._first_level_metrics:
             renderer = find_metric_renderer(type(metric), self._inner_suite.context.renderers)
-            metrics.append({"metric": metric.get_id(), "result": renderer.render_json(metric)})
+            metric_id = metric.get_id()
+            metrics.append(
+                {
+                    "metric": metric_id,
+                    "result": renderer.render_json(
+                        metric,
+                        include_render=include_render,
+                        include=include.get(metric_id),
+                        exclude=exclude.get(metric_id),
+                    ),
+                }
+            )
 
         return {
             "metrics": metrics,
         }
 
     def as_pandas(self, group: str = None) -> Union[Dict[str, pd.DataFrame], pd.DataFrame]:
         metrics = defaultdict(list)
```

### Comparing `evidently-0.2.8/src/evidently/runner/loader.py` & `evidently-0.3.0/src/evidently/runner/loader.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/runner/runner.py` & `evidently-0.3.0/src/evidently/runner/runner.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/suite/base_suite.py` & `evidently-0.3.0/src/evidently/suite/base_suite.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import abc
 import copy
 import dataclasses
 import json
 import logging
 from datetime import datetime
+from typing import Dict
 from typing import Iterator
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import pandas as pd
 
 import evidently
 from evidently.base_metric import ErrorResult
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
+from evidently.core import IncludeOptions
 from evidently.options import OptionsProvider
 from evidently.renderers.base_renderer import DEFAULT_RENDERERS
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import RenderersDefinitions
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.notebook_utils import determine_template
 from evidently.suite.execution_graph import ExecutionGraph
 from evidently.suite.execution_graph import SimpleExecutionGraph
 from evidently.tests.base_test import GroupingTypes
 from evidently.tests.base_test import Test
+from evidently.tests.base_test import TestParameters
 from evidently.tests.base_test import TestResult
+from evidently.tests.base_test import TestStatus
 from evidently.utils import NumpyEncoder
 from evidently.utils.dashboard import SaveMode
 from evidently.utils.dashboard import SaveModeMap
 from evidently.utils.dashboard import TemplateParams
 from evidently.utils.dashboard import save_data_file
 from evidently.utils.dashboard import save_lib_files
 from evidently.utils.data_preprocessing import DataDefinition
@@ -75,16 +80,16 @@
 @dataclasses.dataclass
 class Context:
     """Pipeline execution context tracks pipeline execution and lifecycle"""
 
     execution_graph: Optional[ExecutionGraph]
     metrics: list
     tests: list
-    metric_results: dict
-    test_results: dict
+    metric_results: Dict[Metric, MetricResult]
+    test_results: Dict[Test, TestResult]
     state: State
     renderers: RenderersDefinitions
 
 
 class ExecutionError(Exception):
     pass
 
@@ -158,35 +163,60 @@
                 font_file=font_file,
                 include_js_files=[lib_file, data_file],
             )
             with open(filename, "w", encoding="utf-8") as out_file:
                 out_file.write(self._render(determine_template("inline"), template_params))
 
     @abc.abstractmethod
-    def as_dict(self) -> dict:
+    def as_dict(
+        self,
+        include_render: bool = False,
+        include: Dict[str, IncludeOptions] = None,
+        exclude: Dict[str, IncludeOptions] = None,
+    ) -> dict:
         raise NotImplementedError()
 
-    def _get_json_content(self) -> dict:
+    def _get_json_content(
+        self,
+        include_render: bool = False,
+        include: Dict[str, IncludeOptions] = None,
+        exclude: Dict[str, IncludeOptions] = None,
+    ) -> dict:
         """Return all data for json representation"""
         result = {
             "version": evidently.__version__,
             "timestamp": str(datetime.now()),
         }
-        result.update(self.as_dict())
+        result.update(self.as_dict(include_render=include_render, include=include, exclude=exclude))
         return result
 
-    def json(self) -> str:
+    def json(
+        self,
+        include_render: bool = False,
+        include: Dict[str, IncludeOptions] = None,
+        exclude: Dict[str, IncludeOptions] = None,
+    ) -> str:
         return json.dumps(
-            self._get_json_content(),
+            self._get_json_content(include_render=include_render, include=include, exclude=exclude),
             cls=NumpyEncoder,
         )
 
-    def save_json(self, filename):
+    def save_json(
+        self,
+        filename,
+        include_render: bool = False,
+        include: Dict[str, IncludeOptions] = None,
+        exclude: Dict[str, IncludeOptions] = None,
+    ):
         with open(filename, "w", encoding="utf-8") as out_file:
-            json.dump(self._get_json_content(), out_file, cls=NumpyEncoder)
+            json.dump(
+                self._get_json_content(include_render=include_render, include=include, exclude=exclude),
+                out_file,
+                cls=NumpyEncoder,
+            )
 
     def _render(self, temple_func, template_params: TemplateParams):
         return temple_func(params=template_params)
 
 
 class Suite:
     context: Context
@@ -306,16 +336,18 @@
         for test in self.context.execution_graph.get_test_execution_iterator():
             try:
                 logging.debug(f"Executing {type(test)}...")
                 test_results[test] = test.check()
             except BaseException as ex:
                 test_results[test] = TestResult(
                     name=test.name,
-                    status=TestResult.ERROR,
+                    status=TestStatus.ERROR,
+                    group=test.group,
                     description=f"Test failed with exceptions: {ex}",
+                    parameters=TestParameters(),
                     exception=ex,
                 )
             test_results[test].groups.update(
                 {
                     GroupingTypes.TestGroup.id: test.group,
                     GroupingTypes.TestType.id: test.name,
                 }
```

### Comparing `evidently-0.2.8/src/evidently/suite/execution_graph.py` & `evidently-0.3.0/src/evidently/suite/execution_graph.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/telemetry/sender.py` & `evidently-0.3.0/src/evidently/telemetry/sender.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/__init__.py` & `evidently-0.3.0/src/evidently/test_preset/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/classification_binary.py` & `evidently-0.3.0/src/evidently/test_preset/classification_binary.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/classification_binary_topk.py` & `evidently-0.3.0/src/evidently/test_preset/classification_binary_topk.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/classification_multiclass.py` & `evidently-0.3.0/src/evidently/test_preset/classification_multiclass.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/data_drift.py` & `evidently-0.3.0/src/evidently/test_preset/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/data_quality.py` & `evidently-0.3.0/src/evidently/test_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/data_stability.py` & `evidently-0.3.0/src/evidently/test_preset/data_stability.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/no_target_performance.py` & `evidently-0.3.0/src/evidently/test_preset/no_target_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_preset/regression.py` & `evidently-0.3.0/src/evidently/test_preset/regression.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/test_suite/test_suite.py` & `evidently-0.3.0/src/evidently/test_suite/test_suite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import copy
 import dataclasses
 import uuid
 from collections import Counter
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from evidently.base_metric import InputData
+from evidently.core import IncludeOptions
 from evidently.metric_results import DatasetColumns
 from evidently.model.dashboard import DashboardInfo
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options import ColorOptions
 from evidently.pipeline.column_mapping import ColumnMapping
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.suite.base_suite import Display
 from evidently.suite.base_suite import Suite
 from evidently.suite.base_suite import find_test_renderer
 from evidently.test_preset.test_preset import TestPreset
 from evidently.tests.base_test import DEFAULT_GROUP
 from evidently.tests.base_test import Test
-from evidently.tests.base_test import TestResult
+from evidently.tests.base_test import TestStatus
 from evidently.utils.data_operations import process_columns
 from evidently.utils.data_preprocessing import create_data_definition
 from evidently.utils.generators import BaseGenerator
 
 
 class TestSuite(Display):
     _inner_suite: Suite
@@ -92,39 +94,49 @@
         self._inner_suite.verify()
         curr_add, ref_add = self._inner_suite.create_additional_features(current_data, reference_data, data_definition)
         data = InputData(reference_data, current_data, ref_add, curr_add, column_mapping, data_definition)
 
         self._inner_suite.run_calculate(data)
         self._inner_suite.run_checks()
 
-    def as_dict(self) -> dict:
+    def as_dict(
+        self,
+        include_render: bool = False,
+        include: Dict[str, IncludeOptions] = None,
+        exclude: Dict[str, IncludeOptions] = None,
+    ) -> dict:
         test_results = []
+        include = include or {}
+        exclude = exclude or {}
         counter = Counter(test_result.status for test_result in self._inner_suite.context.test_results.values())
 
         for test in self._inner_suite.context.test_results:
             renderer = find_test_renderer(type(test), self._inner_suite.context.renderers)
+            test_id = test.get_id()
             try:
-                test_data = renderer.render_json(test)
+                test_data = renderer.render_json(
+                    test, include_render=include_render, include=include.get(test_id), exclude=exclude.get(test_id)
+                )
                 test_results.append(test_data)
             except BaseException as e:
                 test_data = TestRenderer.render_json(renderer, test)
-                test_data["status"] = TestResult.ERROR
+                test_data["status"] = TestStatus.ERROR
                 test_data["description"] = f"Test failed with exception: {e}"
                 test_results.append(test_data)
 
         total_tests = len(self._inner_suite.context.test_results)
 
         return {
             "tests": test_results,
             "summary": {
                 "all_passed": bool(self),
                 "total_tests": total_tests,
-                "success_tests": counter["SUCCESS"] + counter["WARNING"],
-                "failed_tests": counter["FAIL"],
-                "by_status": counter,
+                "success_tests": counter[TestStatus.SUCCESS] + counter[TestStatus.WARNING],
+                "failed_tests": counter[TestStatus.FAIL],
+                "by_status": {k.value: v for k, v in counter.items()},
             },
         }
 
     def _build_dashboard_info(self):
         test_results = []
         total_tests = len(self._inner_suite.context.test_results)
         by_status = {}
@@ -139,16 +151,16 @@
         summary_widget = BaseWidgetInfo(
             title="",
             size=2,
             type="counter",
             params={
                 "counters": [{"value": f"{total_tests}", "label": "Tests"}]
                 + [
-                    {"value": f"{by_status.get(status, 0)}", "label": f"{status.title()}"}
-                    for status in [TestResult.SUCCESS, TestResult.WARNING, TestResult.FAIL, TestResult.ERROR]
+                    {"value": f"{by_status.get(status, 0)}", "label": f"{status.value.title()}"}
+                    for status in [TestStatus.SUCCESS, TestStatus.WARNING, TestStatus.FAIL, TestStatus.ERROR]
                 ]
             },
         )
         test_suite_widget = BaseWidgetInfo(
             title="",
             type="test_suite",
             size=2,
```

### Comparing `evidently-0.2.8/src/evidently/tests/__init__.py` & `evidently-0.3.0/src/evidently/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/tests/base_test.py` & `evidently-0.3.0/src/evidently/tests/base_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 import abc
 import dataclasses
 from abc import ABC
-from dataclasses import dataclass
+from enum import Enum
+from typing import TYPE_CHECKING
 from typing import Any
+from typing import ClassVar
 from typing import Dict
+from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Type
+from typing import TypeVar
 from typing import Union
 
+from pydantic import BaseModel
+from pydantic import Field
+
+from evidently.base_metric import Metric
+from evidently.base_metric import MetricResult
 from evidently.utils.generators import BaseGenerator
 from evidently.utils.generators import make_generator_by_columns
 from evidently.utils.types import ApproxValue
 from evidently.utils.types import Numeric
+from evidently.utils.types import NumericApprox
+
+if TYPE_CHECKING:
+    from pydantic.typing import DictStrAny
+
+    from evidently.suite.base_suite import Context
 
 
 @dataclasses.dataclass
 class GroupData:
     id: str
     title: str
     description: str
@@ -66,96 +81,131 @@
     GroupingTypes.ByFeature,
     GroupingTypes.TestGroup,
     GroupingTypes.TestType,
     GroupingTypes.ByClass,
 ]
 
 
-@dataclass
-class TestResult:
+class EnumValueMixin(BaseModel):
+    def dict(self, *args, **kwargs) -> "DictStrAny":
+        res = super().dict(*args, **kwargs)
+        return {k: v.value if isinstance(v, Enum) else v for k, v in res.items()}
+
+
+class ExcludeNoneMixin(BaseModel):
+    def dict(self, *args, **kwargs) -> "DictStrAny":
+        kwargs["exclude_none"] = True
+        return super().dict(*args, **kwargs)
+
+
+class TestStatus(Enum):
     # Constants for test result status
     SUCCESS = "SUCCESS"  # the test was passed
     FAIL = "FAIL"  # success pass for the test
     WARNING = "WARNING"  # the test was passed, but we have some issues during the execution
     ERROR = "ERROR"  # cannot calculate the test result, no data
     SKIPPED = "SKIPPED"  # the test was skipped
 
+
+class TestParameters(MetricResult):
+    pass
+
+
+class TestResult(EnumValueMixin, MetricResult):  # todo: create common base class
     # short name/title from the test class
     name: str
     # what was checked, what threshold (current value 13 is not ok with condition less than 5)
     description: str
     # status of the test result
-    status: str
+    status: TestStatus
     # grouping parameters
-    groups: Dict[str, str] = dataclasses.field(default_factory=dict)
-    exception: Optional[BaseException] = None
+    group: str
+    groups: Dict[str, str] = Field(default_factory=dict, exclude=True)
+    parameters: Optional[TestParameters]
+    exception: Optional[BaseException] = Field(None, exclude=True)
 
-    def set_status(self, status: str, description: Optional[str] = None) -> None:
+    def set_status(self, status: TestStatus, description: Optional[str] = None) -> None:
         self.status = status
 
         if description is not None:
             self.description = description
 
     def mark_as_fail(self, description: Optional[str] = None):
-        self.set_status(self.FAIL, description=description)
+        self.set_status(TestStatus.FAIL, description=description)
 
     def mark_as_error(self, description: Optional[str] = None):
-        self.set_status(self.ERROR, description=description)
+        self.set_status(TestStatus.ERROR, description=description)
 
     def mark_as_success(self, description: Optional[str] = None):
-        self.set_status(self.SUCCESS, description=description)
+        self.set_status(TestStatus.SUCCESS, description=description)
 
     def mark_as_warning(self, description: Optional[str] = None):
-        self.set_status(self.WARNING, description=description)
+        self.set_status(TestStatus.WARNING, description=description)
 
     def is_passed(self):
-        return self.status in [self.SUCCESS, self.WARNING]
+        return self.status in [TestStatus.SUCCESS, TestStatus.WARNING]
 
 
 class Test:
     """
     all fields in test class with type that is subclass of Metric would be used as dependencies of test.
     """
 
     name: str
     group: str
-    context = None
+    context: Optional["Context"] = None
 
     @abc.abstractmethod
     def check(self) -> TestResult:
-        raise NotImplementedError()
+        raise NotImplementedError
 
-    def set_context(self, context):
+    def set_context(self, context: "Context"):
         self.context = context
 
-    def get_result(self):
+    def get_result(self) -> TestResult:
         if self.context is None:
             raise ValueError("No context is set")
         result = self.context.test_results.get(self, None)
         if result is None:
             raise ValueError(f"No result found for metric {self} of type {type(self).__name__}")
-        return result
+        return result  # type: ignore[return-value]
+
+    def get_id(self) -> str:
+        return self.__class__.__name__
+
 
+class ValueSource(Enum):
+    USER = "user"
+    CURRENT = "current"
+    REFERENCE = "reference"
+    DUMMY = "dummy"
+    OTHER = "other"
 
-@dataclass
-class TestValueCondition:
+
+class TestValueCondition(ExcludeNoneMixin):
     """
     Class for processing a value conditions - should it be less, greater than, equals and so on.
 
     An object of the class stores specified conditions and can be used for checking a value by them.
     """
 
-    eq: Optional[Numeric] = None
-    gt: Optional[Numeric] = None
-    gte: Optional[Numeric] = None
+    class Config:
+        arbitrary_types_allowed = True
+        use_enum_values = True
+        smart_union = True
+
+    eq: Optional[NumericApprox] = None
+    gt: Optional[NumericApprox] = None
+    gte: Optional[NumericApprox] = None
     is_in: Optional[List[Union[Numeric, str, bool]]] = None
-    lt: Optional[Numeric] = None
-    lte: Optional[Numeric] = None
+    lt: Optional[NumericApprox] = None
+    lte: Optional[NumericApprox] = None
     not_eq: Optional[Numeric] = None
     not_in: Optional[List[Union[Numeric, str, bool]]] = None
+    source: Optional[ValueSource] = Field(None, exclude=True)  # todo: temporary to not fix tests
 
     def has_condition(self) -> bool:
         """
         Checks if we have a condition in the object and returns True in this case.
 
         If we have no conditions - returns False.
         """
@@ -216,37 +266,29 @@
                 conditions.append(f"{op}={value:.3g}")
 
             else:
                 conditions.append(f"{op}={value}")
 
         return f"{' and '.join(conditions)}"
 
-    def as_dict(self) -> dict:
-        result = {}
-        operations = ["eq", "gt", "gte", "lt", "lte", "not_eq", "is_in", "not_in"]
 
-        for op in operations:
-            value = getattr(self, op)
-
-            if value is not None:
-                result[op] = value
-
-        return result
+class ConditionTestParameters(TestParameters):
+    condition: TestValueCondition
 
 
 class BaseConditionsTest(Test, ABC):
     """
     Base class for all tests with a condition
     """
 
     condition: TestValueCondition
 
     def __init__(
         self,
-        eq: Optional[Numeric] = None,
+        eq: Optional[NumericApprox] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
@@ -259,14 +301,22 @@
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
 
 
+class CheckValueParameters(ConditionTestParameters):
+    value: Optional[Numeric]
+
+
+class ColumnCheckValueParameters(CheckValueParameters):
+    column_name: str
+
+
 class BaseCheckValueTest(BaseConditionsTest):
     """
     Base class for all tests with checking a value condition
     """
 
     value: Numeric
 
@@ -287,23 +337,29 @@
 
     def get_condition(self) -> TestValueCondition:
         return self.condition
 
     def groups(self) -> Dict[str, str]:
         return {}
 
+    def get_parameters(self) -> CheckValueParameters:
+        return CheckValueParameters(condition=self.get_condition(), value=self.value)
+
     def check(self):
         result = TestResult(
             name=self.name,
             description="The test was not launched",
-            status=TestResult.SKIPPED,
+            status=TestStatus.SKIPPED,
+            group=self.group,
+            parameters=None,
         )
         value = self.calculate_value_for_test()
         self.value = value
         result.description = self.get_description(value)
+        result.parameters = self.get_parameters()
 
         try:
             if value is None:
                 result.mark_as_error()
 
             else:
                 condition = self.get_condition()
@@ -322,14 +378,33 @@
         except ValueError:
             result.mark_as_error("Cannot calculate the condition")
 
         result.groups.update(self.groups())
         return result
 
 
+T = TypeVar("T", bound=MetricResult)
+
+
+class ConditionFromReferenceMixin(BaseCheckValueTest, Generic[T], ABC):
+    reference_field: ClassVar[str] = "reference"
+    metric: Metric
+
+    def get_condition_from_reference(self, reference: Optional[T]) -> TestValueCondition:
+        raise NotImplementedError
+
+    def get_condition(self) -> TestValueCondition:
+        if self.condition.has_condition():
+            return self.condition
+
+        reference_stats = getattr(self.metric.get_result(), self.reference_field)
+
+        return self.get_condition_from_reference(reference_stats)
+
+
 def generate_column_tests(
     test_class: Type[Test], columns: Optional[Union[str, list]] = None, parameters: Optional[Dict] = None
 ) -> BaseGenerator:
     """Function for generating tests for columns"""
     return make_generator_by_columns(
         base_class=test_class,
         columns=columns,
```

### Comparing `evidently-0.2.8/src/evidently/tests/classification_performance_tests.py` & `evidently-0.3.0/src/evidently/tests/classification_performance_tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 from abc import ABC
 from typing import Any
+from typing import ClassVar
 from typing import List
 from typing import Optional
 from typing import Union
 
 from evidently.metric_results import DatasetClassificationQuality
 from evidently.metric_results import Label
 from evidently.metric_results import ROCCurve
@@ -19,28 +20,32 @@
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import get_roc_auc_tab_data
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.tests.base_test import BaseCheckValueTest
+from evidently.tests.base_test import CheckValueParameters
 from evidently.tests.base_test import GroupData
 from evidently.tests.base_test import GroupingTypes
 from evidently.tests.base_test import TestValueCondition
+from evidently.tests.base_test import ValueSource
 from evidently.tests.utils import approx
 from evidently.tests.utils import plot_boxes
 from evidently.tests.utils import plot_conf_mtrx
 from evidently.tests.utils import plot_rates
 from evidently.utils.types import Numeric
 
 CLASSIFICATION_GROUP = GroupData("classification", "Classification", "")
 GroupingTypes.TestGroup.add_value(CLASSIFICATION_GROUP)
 
 
 class SimpleClassificationTest(BaseCheckValueTest):
+    condition_arg: ClassVar[str] = "gt"
+
     group = CLASSIFICATION_GROUP.id
     name: str
     metric: ClassificationQualityMetric
     dummy_metric: ClassificationDummyMetric
 
     def __init__(
         self,
@@ -72,20 +77,24 @@
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
 
         ref_metrics = self.metric.get_result().reference
 
         if ref_metrics is not None:
-            return TestValueCondition(eq=approx(self.get_value(ref_metrics), relative=0.2))
+            return TestValueCondition(
+                eq=approx(self.get_value(ref_metrics), relative=0.2), source=ValueSource.REFERENCE
+            )
 
         if self.get_value(self.dummy_metric.get_result().dummy) is None:
             raise ValueError("Neither required test parameters nor reference data has been provided.")
 
-        return TestValueCondition(gt=self.get_value(self.dummy_metric.get_result().dummy))
+        return TestValueCondition(
+            **{self.condition_arg: self.get_value(self.dummy_metric.get_result().dummy)}, source=ValueSource.DUMMY
+        )
 
     @abc.abstractmethod
     def get_value(self, result: DatasetClassificationQuality):
         raise NotImplementedError()
 
 
 class SimpleClassificationTestTopK(SimpleClassificationTest, ABC):
@@ -125,50 +134,27 @@
         self.dummy_metric = ClassificationDummyMetric(probas_threshold=self.probas_threshold, k=self.k)
         self.metric = ClassificationQualityMetric(probas_threshold=self.probas_threshold, k=self.k)
         self.conf_matrix = ClassificationConfusionMatrix(probas_threshold=self.probas_threshold, k=self.k)
 
     def calculate_value_for_test(self) -> Optional[Any]:
         return self.get_value(self.metric.get_result().current)
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        result = self.metric.get_result()
-        ref_metrics = result.reference
-
-        if ref_metrics is not None:
-            return TestValueCondition(eq=approx(self.get_value(ref_metrics), relative=0.2))
-
-        dummy_result = self.dummy_metric.get_result().dummy
-
-        if self.get_value(dummy_result) is None:
-            raise ValueError("Neither required test parameters nor reference data has been provided.")
-
-        return TestValueCondition(gt=self.get_value(dummy_result))
-
 
 class TestAccuracyScore(SimpleClassificationTestTopK):
     name = "Accuracy Score"
 
     def get_value(self, result: DatasetClassificationQuality):
         return result.accuracy
 
     def get_description(self, value: Numeric) -> str:
         return f"The Accuracy Score is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestAccuracyScore)
 class TestAccuracyScoreRenderer(TestRenderer):
-    def render_json(self, obj: TestAccuracyScore) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["accuracy"] = obj.value
-        return base
-
     def render_html(self, obj: TestAccuracyScore) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_matrix = obj.conf_matrix.get_result().current_matrix
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Accuracy Score", plotly_figure(figure=fig, title=""))
         return info
@@ -182,20 +168,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The Precision Score is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestPrecisionScore)
 class TestPrecisionScoreRenderer(TestRenderer):
-    def render_json(self, obj: TestPrecisionScore) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["precision"] = obj.value
-        return base
-
     def render_html(self, obj: TestPrecisionScore) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_matrix = obj.conf_matrix.get_result().current_matrix
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Precision Score", plotly_figure(figure=fig, title=""))
         return info
@@ -209,20 +189,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The F1 Score is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestF1Score)
 class TestF1ScoreRenderer(TestRenderer):
-    def render_json(self, obj: TestF1Score) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["f1"] = obj.value
-        return base
-
     def render_html(self, obj: TestF1Score) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_matrix = obj.conf_matrix.get_result().current_matrix
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("F1 Score", plotly_figure(title="", figure=fig))
         return info
@@ -236,20 +210,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The Recall Score is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestRecallScore)
 class TestRecallScoreRenderer(TestRenderer):
-    def render_json(self, obj: TestRecallScore) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["recall"] = obj.value
-        return base
-
     def render_html(self, obj: TestRecallScore) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_matrix = obj.conf_matrix.get_result().current_matrix
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Recall Score", plotly_figure(title="", figure=fig))
         return info
@@ -291,20 +259,14 @@
 
         else:
             return f"The ROC AUC Score is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestRocAuc)
 class TestRocAucRenderer(TestRenderer):
-    def render_json(self, obj: TestRocAuc) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["roc_auc"] = obj.value
-        return base
-
     def render_html(self, obj: TestRocAuc) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_roc_curve: Optional[ROCCurve] = obj.roc_curve.get_result().current_roc_curve
         ref_roc_curve: Optional[ROCCurve] = obj.roc_curve.get_result().reference_roc_curve
 
         if curr_roc_curve is None:
             return info
@@ -315,49 +277,30 @@
             return info.with_details("ROC Curve", tab_data[0][1])
 
         tabs = [TabData(name, widget) for name, widget in tab_data]
         return info.with_details("", widget_tabs(title="", tabs=tabs))
 
 
 class TestLogLoss(SimpleClassificationTest):
+    condition_arg = "lt"
     name = "Logarithmic Loss"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        ref_metrics = self.metric.get_result().reference
-
-        if ref_metrics is not None:
-            return TestValueCondition(eq=approx(self.get_value(ref_metrics), relative=0.2))
-
-        if self.get_value(self.dummy_metric.get_result().dummy) is None:
-            raise ValueError("Neither required test parameters nor reference data has been provided.")
-
-        return TestValueCondition(lt=self.get_value(self.dummy_metric.get_result().dummy))
-
     def get_value(self, result: DatasetClassificationQuality):
         return result.log_loss
 
     def get_description(self, value: Numeric) -> str:
         if value is None:
             return "Not enough data to calculate Logarithmic Loss. Consider providing probabilities instead of labels."
 
         else:
             return f"The Logarithmic Loss is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestLogLoss)
 class TestLogLossRenderer(TestRenderer):
-    def render_json(self, obj: TestLogLoss) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["log_loss"] = obj.value
-        return base
-
     def render_html(self, obj: TestLogLoss) -> TestHtmlInfo:
         info = super().render_html(obj)
         result: ClassificationQualityMetricResult = obj.metric.get_result()
 
         curr_metrics = result.current.plot_data
         ref_metrics = None if result.reference is None else result.reference.plot_data
 
@@ -383,20 +326,14 @@
             return "This test is applicable only for binary classification"
 
         return f"The True Positive Rate is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestTPR)
 class TestTPRRenderer(TestRenderer):
-    def render_json(self, obj: TestTPR) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["tpr"] = obj.value
-        return base
-
     def render_html(self, obj: TestF1Score) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_metrics = obj.metric.get_result().current
         ref_metrics = obj.metric.get_result().reference
         curr_rate_plots_data = curr_metrics.rate_plots_data
         ref_rate_plots_data = None
 
@@ -425,20 +362,14 @@
             return "This test is applicable only for binary classification"
 
         return f"The True Negative Rate is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestTNR)
 class TestTNRRenderer(TestRenderer):
-    def render_json(self, obj: TestTNR) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["tnr"] = obj.value
-        return base
-
     def render_html(self, obj: TestF1Score) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_metrics = obj.metric.get_result().current
         ref_metrics = obj.metric.get_result().reference
         curr_rate_plots_data = curr_metrics.rate_plots_data
         ref_rate_plots_data = None
 
@@ -453,50 +384,29 @@
             )
             info.with_details("TNR", plotly_figure(title="", figure=fig))
 
         return info
 
 
 class TestFPR(SimpleClassificationTestTopK):
+    condition_arg: ClassVar = "lt"
     name = "False Positive Rate"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        result = self.metric.get_result()
-        ref_metrics = result.reference
-        dummy_metrics = self.dummy_metric.get_result().dummy
-
-        if ref_metrics is not None:
-            return TestValueCondition(eq=approx(self.get_value(ref_metrics), relative=0.2))
-
-        if self.get_value(dummy_metrics) is None:
-            raise ValueError("Neither required test parameters nor reference data has been provided.")
-
-        return TestValueCondition(lt=self.get_value(dummy_metrics))
-
     def get_value(self, result: DatasetClassificationQuality):
         return result.fpr
 
     def get_description(self, value: Numeric) -> str:
         if value is None:
             return "This test is applicable only for binary classification"
 
         return f"The False Positive Rate is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestFPR)
 class TestFPRRenderer(TestRenderer):
-    def render_json(self, obj: TestFPR) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["fpr"] = obj.value
-        return base
-
     def render_html(self, obj: TestF1Score) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_metrics = obj.metric.get_result().current
         ref_metrics = obj.metric.get_result().reference
         curr_rate_plots_data = curr_metrics.rate_plots_data
         ref_rate_plots_data = None
 
@@ -511,50 +421,29 @@
             )
             info.with_details("FPR", plotly_figure(title="", figure=fig))
 
         return info
 
 
 class TestFNR(SimpleClassificationTestTopK):
+    condition_arg: ClassVar = "lt"
     name = "False Negative Rate"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        result = self.metric.get_result()
-        ref_metrics = result.reference
-        dummy_metrics = self.dummy_metric.get_result().dummy
-
-        if ref_metrics is not None:
-            return TestValueCondition(eq=approx(self.get_value(ref_metrics), relative=0.2))
-
-        if self.get_value(dummy_metrics) is None:
-            raise ValueError("Neither required test parameters nor reference data has been provided.")
-
-        return TestValueCondition(lt=self.get_value(dummy_metrics))
-
     def get_value(self, result: DatasetClassificationQuality):
         return result.fnr
 
     def get_description(self, value: Numeric) -> str:
         if value is None:
             return "This test is applicable only for binary classification"
 
         return f"The False Negative Rate is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestFNR)
 class TestFNRRenderer(TestRenderer):
-    def render_json(self, obj: TestFNR) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["fnr"] = obj.value
-        return base
-
     def render_html(self, obj: TestF1Score) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_metrics = obj.metric.get_result().current
         ref_metrics = obj.metric.get_result().reference
         curr_rate_plots_data = curr_metrics.rate_plots_data
         ref_rate_plots_data = None
 
@@ -568,14 +457,18 @@
                 color_options=self.color_options,
             )
             info.with_details("FNR", plotly_figure(title="", figure=fig))
 
         return info
 
 
+class ByClassParameters(CheckValueParameters):
+    label: Label
+
+
 class ByClassClassificationTest(BaseCheckValueTest, ABC):
     group = CLASSIFICATION_GROUP.id
     metric: ClassificationQualityMetric
     by_class_metric: ClassificationQualityByClass
     dummy_metric: ClassificationDummyMetric
     conf_matrix: ClassificationConfusionMatrix
 
@@ -635,14 +528,17 @@
 
         return TestValueCondition(gt=self.get_value(dummy_result))
 
     @abc.abstractmethod
     def get_value(self, result: ClassMetric):
         raise NotImplementedError()
 
+    def get_parameters(self) -> ByClassParameters:
+        return ByClassParameters(condition=self.get_condition(), value=self.value, label=self.label)
+
 
 class TestPrecisionByClass(ByClassClassificationTest):
     name: str = "Precision Score by Class"
 
     def get_value(self, result: ClassMetric):
         return result.precision
 
@@ -651,21 +547,14 @@
             f"The precision score of the label **{self.label}** is {value:.3g}. "
             f"The test threshold is {self.get_condition()}"
         )
 
 
 @default_renderer(wrap_type=TestPrecisionByClass)
 class TestPrecisionByClassRenderer(TestRenderer):
-    def render_json(self, obj: TestPrecisionByClass) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["precision"] = obj.value
-        base["parameters"]["label"] = obj.label
-        return base
-
     def render_html(self, obj: TestPrecisionByClass) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_matrix = obj.conf_matrix.get_result().current_matrix
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Precision by Class", plotly_figure(title="", figure=fig))
         return info
@@ -682,21 +571,14 @@
             f"The recall score of the label **{self.label}** is {value:.3g}. "
             f"The test threshold is {self.get_condition()}"
         )
 
 
 @default_renderer(wrap_type=TestRecallByClass)
 class TestRecallByClassRenderer(TestRenderer):
-    def render_json(self, obj: TestRecallByClass) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["recall"] = obj.value
-        base["parameters"]["label"] = obj.label
-        return base
-
     def render_html(self, obj: TestRecallByClass) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_matrix = obj.conf_matrix.get_result().current_matrix
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Recall by Class", plotly_figure(title="", figure=fig))
         return info
@@ -712,21 +594,14 @@
         return (
             f"The F1 score of the label **{self.label}** is {value:.3g}. The test threshold is {self.get_condition()}"
         )
 
 
 @default_renderer(wrap_type=TestF1ByClass)
 class TestF1ByClassRenderer(TestRenderer):
-    def render_json(self, obj: TestF1ByClass) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["f1"] = obj.value
-        base["parameters"]["label"] = obj.label
-        return base
-
     def render_html(self, obj: TestF1ByClass) -> TestHtmlInfo:
         info = super().render_html(obj)
         curr_matrix = obj.conf_matrix.get_result().current_matrix
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("F1 by Class", plotly_figure(title="", figure=fig))
         return info
```

### Comparing `evidently-0.2.8/src/evidently/tests/data_drift_tests.py` & `evidently-0.3.0/src/evidently/tests/data_drift_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,93 @@
-import dataclasses
 from abc import ABC
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
+from evidently.base_metric import ColumnName
+from evidently.calculations.data_drift import ColumnDataDriftMetrics
 from evidently.calculations.stattests import PossibleStatTestType
 from evidently.metric_results import DatasetColumns
 from evidently.metrics import ColumnDriftMetric
 from evidently.metrics import DataDriftTable
+from evidently.metrics.data_drift.data_drift_table import DataDriftTableResults
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import DetailsInfo
 from evidently.renderers.base_renderer import TestHtmlInfo
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.render_utils import get_distribution_plot_figure
 from evidently.tests.base_test import BaseCheckValueTest
+from evidently.tests.base_test import ConditionTestParameters
+from evidently.tests.base_test import ExcludeNoneMixin
 from evidently.tests.base_test import GroupData
 from evidently.tests.base_test import GroupingTypes
 from evidently.tests.base_test import Test
+from evidently.tests.base_test import TestParameters
 from evidently.tests.base_test import TestResult
+from evidently.tests.base_test import TestStatus
 from evidently.tests.base_test import TestValueCondition
 from evidently.utils.data_drift_utils import resolve_stattest_threshold
 from evidently.utils.generators import BaseGenerator
 from evidently.utils.types import Numeric
 
 DATA_DRIFT_GROUP = GroupData("data_drift", "Data Drift", "")
 GroupingTypes.TestGroup.add_value(DATA_DRIFT_GROUP)
 
 
-@dataclasses.dataclass
-class TestDataDriftResult(TestResult):
-    features: Dict[str, Tuple[str, float, float]] = dataclasses.field(default_factory=dict)
+class ColumnDriftParameter(ExcludeNoneMixin, TestParameters):
+    stattest: str
+    score: float
+    threshold: float
+    detected: bool
+    column_name: Optional[str] = None
+
+    @classmethod
+    def from_metric(cls, data: ColumnDataDriftMetrics, column_name: str = None):
+        return ColumnDriftParameter(
+            stattest=data.stattest_name,
+            score=np.round(data.drift_score, 3),
+            threshold=data.stattest_threshold,
+            detected=data.drift_detected,
+            column_name=column_name,
+        )
+
+
+class ColumnsDriftParameters(ConditionTestParameters):
+    # todo: rename to columns?
+    features: Dict[str, ColumnDriftParameter]
+
+    @classmethod
+    def from_data_drift_table(cls, table: DataDriftTableResults, condition: TestValueCondition):
+        return ColumnsDriftParameters(
+            features={
+                feature: ColumnDriftParameter.from_metric(data) for feature, data in table.drift_by_columns.items()
+            },
+            condition=condition,
+        )
+
+    def to_dataframe(self) -> pd.DataFrame:
+        return pd.DataFrame(
+            [
+                {
+                    "Feature name": feature,
+                    "Stattest": data.stattest,
+                    "Drift score": data.score,
+                    "Threshold": data.threshold,
+                    "Data Drift": "Detected" if data.detected else "Not detected",
+                }
+                for feature, data in self.features.items()
+            ],
+        )
 
 
 class BaseDataDriftMetricsTest(BaseCheckValueTest, ABC):
     group = DATA_DRIFT_GROUP.id
     metric: DataDriftTable
 
     def __init__(
@@ -90,27 +136,20 @@
             per_column_stattest_threshold=per_column_stattest_threshold,
         )
 
     def check(self):
         result = super().check()
         metrics = self.metric.get_result()
 
-        return TestDataDriftResult(
+        return TestResult(
             name=result.name,
             description=result.description,
-            status=result.status,
-            features={
-                feature: (
-                    data.stattest_name,
-                    np.round(data.drift_score, 3),
-                    data.stattest_threshold,
-                    "Detected" if data.drift_detected else "Not Detected",
-                )
-                for feature, data in metrics.drift_by_columns.items()
-            },
+            status=TestStatus(result.status),
+            group=self.group,
+            parameters=ColumnsDriftParameters.from_data_drift_table(metrics, self.get_condition()),
         )
 
 
 class TestNumberOfDriftedColumns(BaseDataDriftMetricsTest):
     name = "Number of Drifted Features"
 
     def get_condition(self) -> TestValueCondition:
@@ -151,54 +190,59 @@
         )
 
 
 class TestColumnDrift(Test):
     name = "Drift per Column"
     group = DATA_DRIFT_GROUP.id
     metric: ColumnDriftMetric
-    column_name: str
+    column_name: ColumnName
 
     def __init__(
         self,
-        column_name: str,
+        column_name: Union[str, ColumnName],
         stattest: Optional[PossibleStatTestType] = None,
         stattest_threshold: Optional[float] = None,
     ):
-        self.column_name = column_name
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
         self.metric = ColumnDriftMetric(
             column_name=column_name,
             stattest=stattest,
             stattest_threshold=stattest_threshold,
         )
 
     def check(self):
         drift_info = self.metric.get_result()
 
         p_value = np.round(drift_info.drift_score, 3)
         stattest_name = drift_info.stattest_name
         threshold = drift_info.stattest_threshold
         description = (
-            f"The drift score for the feature **{self.column_name}** is {p_value:.3g}. "
+            f"The drift score for the feature **{self.column_name.display_name}** is {p_value:.3g}. "
             f"The drift detection method is {stattest_name}. "
             f"The drift detection threshold is {threshold}."
         )
 
         if not drift_info.drift_detected:
-            result_status = TestResult.SUCCESS
+            result_status = TestStatus.SUCCESS
 
         else:
-            result_status = TestResult.FAIL
+            result_status = TestStatus.FAIL
 
         return TestResult(
             name=self.name,
             description=description,
             status=result_status,
+            group=self.group,
             groups={
-                GroupingTypes.ByFeature.id: self.column_name,
+                GroupingTypes.ByFeature.id: self.column_name.display_name,
             },
+            parameters=ColumnDriftParameter.from_metric(drift_info, column_name=self.column_name.display_name),
         )
 
 
 class TestAllFeaturesValueDrift(BaseGenerator):
     """Create value drift tests for numeric and category features"""
 
     columns: Optional[List[str]]
@@ -370,76 +414,34 @@
                 )
             )
         return result
 
 
 @default_renderer(wrap_type=TestNumberOfDriftedColumns)
 class TestNumberOfDriftedColumnsRenderer(TestRenderer):
-    def render_json(self, obj: TestNumberOfDriftedColumns) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["features"] = {
-            feature: {
-                "stattest": data[0],
-                "score": np.round(data[1], 3),
-                "threshold": data[2],
-                "data_drift": data[3],
-            }
-            for feature, data in obj.get_result().features.items()
-        }
-        return base
-
     def render_html(self, obj: TestNumberOfDriftedColumns) -> TestHtmlInfo:
         info = super().render_html(obj)
-        df = pd.DataFrame(
-            data=[[feature] + list(data) for feature, data in obj.get_result().features.items()],
-            columns=[
-                "Feature name",
-                "Stattest",
-                "Drift score",
-                "Threshold",
-                "Data Drift",
-            ],
-        )
+        parameters = obj.get_result().parameters
+        assert isinstance(parameters, ColumnsDriftParameters)
+        df = parameters.to_dataframe()
         df = df.sort_values("Data Drift")
         info.with_details(
             title="Drift Table",
             info=table_data(column_names=df.columns.to_list(), data=df.values),
         )
         return info
 
 
 @default_renderer(wrap_type=TestShareOfDriftedColumns)
 class TestShareOfDriftedColumnsRenderer(TestRenderer):
-    def render_json(self, obj: TestShareOfDriftedColumns) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["features"] = {
-            feature: {
-                "stattest": data[0],
-                "score": np.round(data[1], 3),
-                "threshold": data[2],
-                "data_drift": data[3],
-            }
-            for feature, data in obj.get_result().features.items()
-        }
-        return base
-
     def render_html(self, obj: TestShareOfDriftedColumns) -> TestHtmlInfo:
         info = super().render_html(obj)
-        df = pd.DataFrame(
-            data=[[feature] + list(data) for feature, data in obj.get_result().features.items()],
-            columns=[
-                "Feature name",
-                "Stattest",
-                "Drift score",
-                "Threshold",
-                "Data Drift",
-            ],
-        )
+        parameters = obj.get_result().parameters
+        assert isinstance(parameters, ColumnsDriftParameters)
+        df = parameters.to_dataframe()
         df = df.sort_values("Data Drift")
         info.details = [
             DetailsInfo(
                 id="drift_table",
                 title="",
                 info=BaseWidgetInfo(
                     title="",
@@ -450,28 +452,14 @@
             ),
         ]
         return info
 
 
 @default_renderer(wrap_type=TestColumnDrift)
 class TestColumnDriftRenderer(TestRenderer):
-    def render_json(self, obj: TestColumnDrift) -> dict:
-        feature_name = obj.column_name
-        drift_data = obj.metric.get_result()
-        base = super().render_json(obj)
-        base["parameters"]["features"] = {
-            feature_name: {
-                "stattest_name": drift_data.stattest_name,
-                "score": np.round(drift_data.drift_score, 3),
-                "stattest_threshold": drift_data.stattest_threshold,
-                "data_drift": drift_data.drift_detected,
-            }
-        }
-        return base
-
     def render_html(self, obj: TestColumnDrift) -> TestHtmlInfo:
         info = super().render_html(obj)
         result = obj.metric.get_result()
         column_name = obj.column_name
         if result.column_type == "text":
             if result.current.characteristic_words is not None and result.reference.characteristic_words is not None:
                 info.details = [
```

### Comparing `evidently-0.2.8/src/evidently/tests/data_integrity_tests.py` & `evidently-0.3.0/src/evidently/tests/data_integrity_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-import dataclasses
 from abc import ABC
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from pandas.core.dtypes.common import infer_dtype_from_object
 
 from evidently.metric_results import DatasetColumns
 from evidently.metrics import ColumnRegExpMetric
 from evidently.metrics import ColumnSummaryMetric
 from evidently.metrics import DatasetMissingValuesMetric
 from evidently.metrics import DatasetSummaryMetric
 from evidently.metrics.data_integrity.dataset_missing_values_metric import DatasetMissingValues
 from evidently.metrics.data_integrity.dataset_missing_values_metric import DatasetMissingValuesMetricResult
+from evidently.metrics.data_integrity.dataset_summary_metric import DatasetSummary
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import DetailsInfo
 from evidently.renderers.base_renderer import TestHtmlInfo
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.tests.base_test import BaseCheckValueTest
+from evidently.tests.base_test import ColumnCheckValueParameters
+from evidently.tests.base_test import ConditionFromReferenceMixin
 from evidently.tests.base_test import GroupData
 from evidently.tests.base_test import GroupingTypes
 from evidently.tests.base_test import Test
+from evidently.tests.base_test import TestParameters
 from evidently.tests.base_test import TestResult
+from evidently.tests.base_test import TestStatus
 from evidently.tests.base_test import TestValueCondition
+from evidently.tests.base_test import ValueSource
 from evidently.tests.utils import approx
 from evidently.tests.utils import dataframes_to_table
 from evidently.tests.utils import plot_dicts_to_table
 from evidently.tests.utils import plot_value_counts_tables_ref_curr
 from evidently.utils.generators import BaseGenerator
 from evidently.utils.types import Numeric
+from evidently.utils.types import NumericApprox
 
 DATA_INTEGRITY_GROUP = GroupData("data_integrity", "Data Integrity", "")
 GroupingTypes.TestGroup.add_value(DATA_INTEGRITY_GROUP)
 
 
-class BaseIntegrityValueTest(BaseCheckValueTest, ABC):
+class BaseIntegrityValueTest(ConditionFromReferenceMixin[DatasetSummary], ABC):
     group = DATA_INTEGRITY_GROUP.id
     metric: DatasetSummaryMetric
 
     def __init__(
         self,
-        eq: Optional[Numeric] = None,
+        eq: Optional[NumericApprox] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
@@ -68,40 +73,28 @@
 
 
 class TestNumberOfColumns(BaseIntegrityValueTest):
     """Number of all columns in the data, including utility columns (id/index, datetime, target, predictions)"""
 
     name = "Number of Columns"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_stats = self.metric.get_result().reference
-
-        if reference_stats is not None:
-            return TestValueCondition(eq=reference_stats.number_of_columns)
-
+    def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
+        if reference is not None:
+            return TestValueCondition(eq=reference.number_of_columns, source=ValueSource.REFERENCE)
         return TestValueCondition(gt=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_columns
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of columns is {value}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestNumberOfColumns)
 class TestNumberOfColumnsRenderer(TestRenderer):
-    def render_json(self, obj: TestNumberOfColumns) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_columns"] = obj.value
-        return base
-
     def render_html(self, obj: TestNumberOfColumns) -> TestHtmlInfo:
         info = super().render_html(obj)
         columns = ["column name", "current dtype"]
         dict_curr = obj.metric.get_result().current.columns_type
         dict_ref = None
         reference_stats = obj.metric.get_result().reference
 
@@ -115,42 +108,28 @@
 
 
 class TestNumberOfRows(BaseIntegrityValueTest):
     """Number of rows in the data"""
 
     name = "Number of Rows"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_stats = self.metric.get_result().reference
-
-        if reference_stats is not None:
-            return TestValueCondition(eq=approx(reference_stats.number_of_rows, relative=0.1))
+    def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
+        if reference is not None:
+            return TestValueCondition(eq=approx(reference.number_of_rows, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(gt=30)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_rows
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of rows is {value}. The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestNumberOfRows)
-class TestNumberOfRowsRenderer(TestRenderer):
-    def render_json(self, obj: TestNumberOfRows) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_rows"] = obj.value
-        return base
-
-
-class BaseIntegrityMissingValuesValuesTest(BaseCheckValueTest, ABC):
+class BaseIntegrityMissingValuesValuesTest(ConditionFromReferenceMixin[DatasetMissingValues], ABC):
     group = DATA_INTEGRITY_GROUP.id
     metric: DatasetMissingValuesMetric
 
     def __init__(
         self,
         missing_values: Optional[list] = None,
         replace: bool = True,
@@ -252,22 +231,17 @@
 
 
 class TestNumberOfDifferentMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of different encoded missing values."""
 
     name = "Different Types of Missing Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_missing_values = self.metric.get_result().reference
-
-        if reference_missing_values is not None:
-            return TestValueCondition(eq=reference_missing_values.number_of_different_missing_values)
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
+        if reference is not None:
+            return TestValueCondition(eq=reference.number_of_different_missing_values, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_different_missing_values
 
     def get_description(self, value: Numeric) -> str:
@@ -275,20 +249,14 @@
             f"The number of differently encoded types of missing values is {value}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
 @default_renderer(wrap_type=TestNumberOfDifferentMissingValues)
 class TestNumberOfDifferentMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestNumberOfDifferentMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_different_missing_values"] = obj.value
-        return base
-
     def render_html(self, obj: TestNumberOfDifferentMissingValues) -> TestHtmlInfo:
         """Get a table with a missing value and number of the value in the dataset"""
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         current_missing_values = metric_result.current.different_missing_values
 
         if metric_result.reference is None:
@@ -306,147 +274,112 @@
 
 
 class TestNumberOfMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of missing values."""
 
     name = "The Number of Missing Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_missing_values = self.metric.get_result().reference
-
-        if reference_missing_values is not None:
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
+        if reference is not None:
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
-            ref_number_of_rows = reference_missing_values.number_of_rows
+            ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
             return TestValueCondition(
                 lte=approx(
-                    reference_missing_values.number_of_missing_values * mult,
+                    reference.number_of_missing_values * mult,
                     relative=0.1,
-                )
+                ),
+                source=ValueSource.REFERENCE,
             )
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_missing_values
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of missing values is {value}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestNumberOfMissingValues)
 class TestNumberOfMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestNumberOfMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_missing_values"] = obj.value
-        return base
-
     def render_html(self, obj: TestNumberOfMissingValues) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         return self.get_table_with_missing_values_and_percents_by_column(
             info, metric_result, "number_of_missing_values"
         )
 
 
 class TestShareOfMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a share of missing values."""
 
     name = "Share of Missing Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference = self.metric.get_result().reference
-
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
-            return TestValueCondition(lte=approx(reference.share_of_missing_values, relative=0.1))
+            return TestValueCondition(
+                lte=approx(reference.share_of_missing_values, relative=0.1), source=ValueSource.REFERENCE
+            )
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_of_missing_values
 
     def get_description(self, value: Numeric) -> str:
         return f"The share of missing values is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestShareOfMissingValues)
 class TestShareOfMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestShareOfMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["share_of_missing_values"] = obj.value
-        return base
-
     def render_html(self, obj: TestNumberOfMissingValues) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         return self.get_table_with_missing_values_and_percents_by_column(info, metric_result, "share_of_missing_values")
 
 
 class TestNumberOfColumnsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of columns with a missing value."""
 
     name = "The Number of Columns With Missing Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference = self.metric.get_result().reference
-
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
-            return TestValueCondition(lte=reference.number_of_columns_with_missing_values)
+            return TestValueCondition(lte=reference.number_of_columns_with_missing_values, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_columns_with_missing_values
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The number of columns with missing values is {value}. " f"The test threshold is {self.get_condition()}."
         )
 
 
 @default_renderer(wrap_type=TestNumberOfColumnsWithMissingValues)
 class TestNumberOfColumnsWithMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestNumberOfColumnsWithMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_columns_with_missing_values"] = obj.value
-        return base
-
     def render_html(self, obj: TestNumberOfMissingValues) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         return self.get_table_with_missing_values_and_percents_by_column(
             info, metric_result, "number_of_columns_with_missing_values"
         )
 
 
 class TestShareOfColumnsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a share of columns with a missing value."""
 
     name = "The Share of Columns With Missing Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference = self.metric.get_result().reference
-
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
-            return TestValueCondition(lte=reference.share_of_columns_with_missing_values)
+            return TestValueCondition(lte=reference.share_of_columns_with_missing_values, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_of_columns_with_missing_values
 
     def get_description(self, value: Numeric) -> str:
@@ -454,98 +387,69 @@
             f"The share of columns with missing values is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
 @default_renderer(wrap_type=TestShareOfColumnsWithMissingValues)
 class TestShareOfColumnsWithMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestShareOfColumnsWithMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["share_of_columns_with_missing_values"] = obj.value
-        return base
-
     def render_html(self, obj: TestNumberOfMissingValues) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         return self.get_table_with_missing_values_and_percents_by_column(
             info, metric_result, "share_of_columns_with_missing_values"
         )
 
 
 class TestNumberOfRowsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of rows with a missing value."""
 
     name = "The Number Of Rows With Missing Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference = self.metric.get_result().reference
-
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
             ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
-            return TestValueCondition(lte=approx(reference.number_of_rows_with_missing_values * mult, relative=0.1))
+            return TestValueCondition(
+                lte=approx(reference.number_of_rows_with_missing_values * mult, relative=0.1),
+                source=ValueSource.REFERENCE,
+            )
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_rows_with_missing_values
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of rows with missing values is {value}. " f"The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestNumberOfRowsWithMissingValues)
-class TestNumberOfRowsWithMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestNumberOfRowsWithMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_rows_with_missing_values"] = obj.value
-        return base
-
-
 class TestShareOfRowsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a share of rows with a missing value."""
 
     name = "The Share of Rows With Missing Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference = self.metric.get_result().reference
-
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
-            return TestValueCondition(lte=approx(reference.share_of_rows_with_missing_values, relative=0.1))
+            return TestValueCondition(
+                lte=approx(reference.share_of_rows_with_missing_values, relative=0.1), source=ValueSource.REFERENCE
+            )
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_of_rows_with_missing_values
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The share of rows with missing values is {value:.3g}. " f"The test threshold is {self.get_condition()}."
         )
 
 
-@default_renderer(wrap_type=TestShareOfRowsWithMissingValues)
-class TestShareOfRowsWithMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestShareOfRowsWithMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["share_of_rows_with_missing_values"] = obj.value
-        return base
-
-
-class BaseIntegrityColumnMissingValuesTest(BaseCheckValueTest, ABC):
+class BaseIntegrityColumnMissingValuesTest(ConditionFromReferenceMixin[DatasetMissingValues], ABC):
     group = DATA_INTEGRITY_GROUP.id
     metric: DatasetMissingValuesMetric
     column_name: str
 
     def __init__(
         self,
         column_name: str,
@@ -575,28 +479,23 @@
 
 
 class TestColumnNumberOfDifferentMissingValues(BaseIntegrityColumnMissingValuesTest):
     """Check a number of differently encoded missing values in one column."""
 
     name = "Different Types of Missing Values in a Column"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_missing_values = self.metric.get_result().reference
-
-        if reference_missing_values is not None:
-            if self.column_name not in reference_missing_values.number_of_different_missing_values_by_column:
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
+        if reference is not None:
+            if self.column_name not in reference.number_of_different_missing_values_by_column:
                 raise ValueError(
                     f"Cannot define test default conditions: no column '{self.column_name}' in reference dataset."
                 )
 
-            ref_value = reference_missing_values.number_of_different_missing_values_by_column[self.column_name]
-            return TestValueCondition(lte=ref_value)
+            ref_value = reference.number_of_different_missing_values_by_column[self.column_name]
+            return TestValueCondition(lte=ref_value, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         metric_data = self.metric.get_result().current
         return metric_data.number_of_different_missing_values_by_column[self.column_name]
 
@@ -605,21 +504,14 @@
             f"The number of differently encoded types of missing values in the column **{self.column_name}** "
             f"is {value}. The test threshold is {self.get_condition()}."
         )
 
 
 @default_renderer(wrap_type=TestColumnNumberOfDifferentMissingValues)
 class TestColumnNumberOfDifferentMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestColumnNumberOfDifferentMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_different_missing_values"] = obj.value
-        base["parameters"]["column_name"] = obj.column_name
-        return base
-
     def render_html(self, obj: TestColumnNumberOfDifferentMissingValues) -> TestHtmlInfo:
         """Get a table with a missing value and number of the value in the dataset"""
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         current_missing_values = metric_result.current.different_missing_values_by_column[obj.column_name]
 
         if metric_result.reference is None:
@@ -637,75 +529,60 @@
 
 
 class TestColumnNumberOfMissingValues(BaseIntegrityColumnMissingValuesTest):
     """Check a number of missing values in one column."""
 
     name = "The Number of Missing Values in a Column"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_missing_values = self.metric.get_result().reference
-
-        if reference_missing_values is not None:
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
+        if reference is not None:
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
-            ref_number_of_rows = reference_missing_values.number_of_rows
+            ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
-            ref_value = reference_missing_values.number_of_missing_values_by_column[self.column_name]
-            return TestValueCondition(lte=approx(ref_value * mult, relative=0.1))
+            ref_value = reference.number_of_missing_values_by_column[self.column_name]
+            return TestValueCondition(lte=approx(ref_value * mult, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_missing_values_by_column[self.column_name]
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The number of missing values in the column **{self.column_name}** is {value}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
-@default_renderer(wrap_type=TestColumnNumberOfMissingValues)
-class TestColumnNumberOfMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestColumnNumberOfMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_missing_values"] = obj.value
-        base["parameters"]["column_name"] = obj.column_name
-        return base
-
-
 class TestColumnShareOfMissingValues(BaseIntegrityColumnMissingValuesTest):
     """Check a share of missing values in one column."""
 
     name = "The Share of Missing Values in a Column"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference = self.metric.get_result().reference
-
+    def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             ref_value = reference.share_of_missing_values_by_column[self.column_name]
-            return TestValueCondition(lte=approx(ref_value, relative=0.1))
+            return TestValueCondition(lte=approx(ref_value, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_of_missing_values_by_column[self.column_name]
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The share of missing values in the column **{self.column_name}** is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
+    def get_parameters(self):
+        return ColumnCheckValueParameters(
+            condition=self.get_condition(), value=self.value, column_name=self.column_name
+        )
+
 
 class TestAllColumnsShareOfMissingValues(BaseGenerator):
     columns: Optional[List[str]]
 
     def __init__(self, columns: Optional[List[str]] = None):
         self.columns = columns
 
@@ -715,56 +592,35 @@
 
         else:
             columns = self.columns
 
         return [TestColumnShareOfMissingValues(column_name=name) for name in columns]
 
 
-@default_renderer(wrap_type=TestColumnShareOfMissingValues)
-class TestColumnShareOfMissingValuesRenderer(BaseTestMissingValuesRenderer):
-    def render_json(self, obj: TestColumnShareOfMissingValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["share_of_missing_values"] = obj.value
-        base["parameters"]["column_name"] = obj.column_name
-        return base
-
-
 class TestNumberOfConstantColumns(BaseIntegrityValueTest):
     """Number of columns contained only one unique value"""
 
     name = "Number of Constant Columns"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_stats = self.metric.get_result().reference
-
-        if reference_stats is not None:
-            value = reference_stats.number_of_constant_columns
-            return TestValueCondition(lte=value)
+    def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
+        if reference is not None:
+            value = reference.number_of_constant_columns
+            return TestValueCondition(lte=value, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_constant_columns
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of constant columns is {value}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestNumberOfConstantColumns)
 class TestNumberOfConstantColumnsRenderer(TestRenderer):
-    def render_json(self, obj: TestNumberOfConstantColumns) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_constant_columns"] = obj.value
-        return base
-
     def render_html(self, obj: TestNumberOfConstantColumns) -> TestHtmlInfo:
         info = super().render_html(obj)
         columns = ["column name", "current nunique"]
         dict_curr = obj.metric.get_result().current.number_uniques_by_columns
         dict_ref = {}
         reference_stats = obj.metric.get_result().reference
 
@@ -778,26 +634,21 @@
 
 
 class TestNumberOfEmptyRows(BaseIntegrityValueTest):
     """Number of rows contained all NAN values"""
 
     name = "Number of Empty Rows"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_stats = self.metric.get_result().reference
-
-        if reference_stats is not None:
-            ref_number_of_empty_rows = reference_stats.number_of_empty_rows
+    def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
+        if reference is not None:
+            ref_number_of_empty_rows = reference.number_of_empty_rows
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
-            ref_number_of_rows = reference_stats.number_of_rows
+            ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
-            return TestValueCondition(eq=approx(ref_number_of_empty_rows * mult, 0.1))
+            return TestValueCondition(eq=approx(ref_number_of_empty_rows * mult, 0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_empty_rows
 
     def get_description(self, value: Numeric) -> str:
@@ -805,22 +656,17 @@
 
 
 class TestNumberOfEmptyColumns(BaseIntegrityValueTest):
     """Number of columns contained all NAN values"""
 
     name = "Number of Empty Columns"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_stats = self.metric.get_result().reference
-
-        if reference_stats is not None:
-            return TestValueCondition(lte=reference_stats.number_of_empty_columns)
+    def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
+        if reference is not None:
+            return TestValueCondition(lte=reference.number_of_empty_columns, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_empty_columns
 
     def get_description(self, value: Numeric) -> str:
@@ -846,78 +692,50 @@
 
 
 class TestNumberOfDuplicatedRows(BaseIntegrityValueTest):
     """How many rows have duplicates in the dataset"""
 
     name = "Number of Duplicate Rows"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_stats = self.metric.get_result().reference
-
-        if reference_stats is not None:
-            ref_num_of_duplicates = reference_stats.number_of_duplicated_rows
+    def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
+        if reference is not None:
+            ref_num_of_duplicates = reference.number_of_duplicated_rows
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
-            ref_number_of_rows = reference_stats.number_of_rows
+            ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
-            return TestValueCondition(eq=approx(ref_num_of_duplicates * mult, 0.1))
+            return TestValueCondition(eq=approx(ref_num_of_duplicates * mult, 0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_duplicated_rows
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of duplicate rows is {value}. The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestNumberOfDuplicatedRows)
-class TestNumberOfDuplicatedRowsRenderer(TestRenderer):
-    def render_json(self, obj: TestNumberOfDuplicatedRows) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_duplicated_rows"] = obj.value
-        return base
-
-
 class TestNumberOfDuplicatedColumns(BaseIntegrityValueTest):
     """How many columns have duplicates in the dataset"""
 
     name = "Number of Duplicate Columns"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_stats = self.metric.get_result().reference
-
-        if reference_stats is not None:
-            value = reference_stats.number_of_duplicated_columns
-            return TestValueCondition(lte=value)
+    def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
+        if reference is not None:
+            value = reference.number_of_duplicated_columns
+            return TestValueCondition(lte=value, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_of_duplicated_columns
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of duplicate columns is {value}. The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestNumberOfDuplicatedColumns)
-class TestNumberOfDuplicatedColumnsRenderer(TestRenderer):
-    def render_json(self, obj: TestNumberOfDuplicatedColumns) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["number_of_duplicated_columns"] = obj.value
-        return base
-
-
 class BaseIntegrityByColumnsConditionTest(BaseCheckValueTest, ABC):
     group = DATA_INTEGRITY_GROUP.id
     data_integrity_metric: ColumnSummaryMetric
     column_name: str
 
     def __init__(
         self,
@@ -976,20 +794,22 @@
 
         description = (
             f"The number of the unique values in the column **{column_name}** "
             f"is {uniques_in_column} out of {number_of_rows}"
         )
 
         if uniques_in_column <= 1:
-            status = TestResult.FAIL
+            status = TestStatus.FAIL
 
         else:
-            status = TestResult.SUCCESS
+            status = TestStatus.SUCCESS
 
-        return TestResult(name=self.name, description=description, status=status, groups=self.groups())
+        return TestResult(
+            name=self.name, description=description, status=status, groups=self.groups(), group=self.group
+        )
 
 
 @default_renderer(wrap_type=TestColumnAllConstantValues)
 class TestColumnAllConstantValuesRenderer(TestRenderer):
     def render_html(self, obj: TestColumnAllConstantValues) -> TestHtmlInfo:
         info = super().render_html(obj)
         column_name = obj.column_name
@@ -1017,20 +837,22 @@
 
         description = (
             f"The number of the unique values in the column **{column_name}** "
             f"is {uniques_in_column}  out of {number_of_rows}"
         )
 
         if uniques_in_column != number_of_rows - nans_in_column:
-            status = TestResult.FAIL
+            status = TestStatus.FAIL
 
         else:
-            status = TestResult.SUCCESS
+            status = TestStatus.SUCCESS
 
-        return TestResult(name=self.name, description=description, status=status, groups=self.groups())
+        return TestResult(
+            name=self.name, description=description, status=status, groups=self.groups(), group=self.group
+        )
 
 
 @default_renderer(wrap_type=TestColumnAllUniqueValues)
 class TestColumnAllUniqueValuesRenderer(TestRenderer):
     def render_html(self, obj: TestColumnAllUniqueValues) -> TestHtmlInfo:
         info = super().render_html(obj)
         column_name = obj.column_name
@@ -1041,113 +863,109 @@
             if "reference" in counts_data.keys():
                 ref_df = counts_data["reference"]
             additional_plots = plot_value_counts_tables_ref_curr(column_name, curr_df, ref_df, "AllUniqueValues")
             info.details = additional_plots
         return info
 
 
+class ColumnTypeParameter(TestParameters):
+    actual_type: str
+    column_name: str
+    expected_type: str
+
+
+class ColumnTypesParameter(TestParameters):
+    columns: List[ColumnTypeParameter]
+
+
 class TestColumnsType(Test):
     """This test compares columns type against the specified ones or a reference dataframe"""
 
     group = DATA_INTEGRITY_GROUP.id
     name = "Column Types"
     columns_type: Optional[dict]
     metric: DatasetSummaryMetric
 
-    @dataclasses.dataclass
-    class Result(TestResult):
-        columns_types: Dict[str, Tuple[str, str]] = dataclasses.field(default_factory=dict)
-
     def __init__(self, columns_type: Optional[dict] = None):
         self.columns_type = columns_type
         self.metric = DatasetSummaryMetric()
 
     def check(self):
-        status = TestResult.SUCCESS
+        status = TestStatus.SUCCESS
         data_columns_type = self.metric.get_result().current.columns_type
 
         if self.columns_type is None:
             if self.metric.get_result().reference is None:
-                status = TestResult.ERROR
+                status = TestStatus.ERROR
                 description = "Cannot compare column types without conditions or a reference"
-                return TestResult(name=self.name, description=description, status=status)
+                return TestResult(name=self.name, description=description, status=status, group=self.group)
 
             # get types from reference
             columns_type = self.metric.get_result().reference.columns_type
 
         else:
             columns_type = self.columns_type
 
             if not columns_type:
-                status = TestResult.ERROR
+                status = TestStatus.ERROR
                 description = "Columns type condition is empty"
-                return TestResult(name=self.name, description=description, status=status)
+                return TestResult(name=self.name, description=description, status=status, group=self.group)
 
         invalid_types_count = 0
-        columns_types = {}
+        columns = []
 
         for column_name, expected_type_object in columns_type.items():
             real_column_type_object = data_columns_type.get(column_name)
 
             if real_column_type_object is None:
-                status = TestResult.ERROR
+                status = TestStatus.ERROR
                 description = f"No column '{column_name}' in the metrics data"
-                return TestResult(name=self.name, description=description, status=status)
+                return TestResult(name=self.name, description=description, status=status, group=self.group)
 
             expected_type = infer_dtype_from_object(expected_type_object)
             real_column_type = infer_dtype_from_object(real_column_type_object)
-            columns_types[column_name] = (
-                real_column_type.__name__,
-                expected_type.__name__,
+            columns.append(
+                ColumnTypeParameter(
+                    actual_type=real_column_type.__name__, expected_type=expected_type.__name__, column_name=column_name
+                )
             )
 
             if expected_type == real_column_type or issubclass(real_column_type, expected_type):
                 # types are matched or expected type is a parent
                 continue
 
-            status = TestResult.FAIL
+            status = TestStatus.FAIL
             invalid_types_count += 1
 
-        return self.Result(
+        return TestResult(
             name=self.name,
             description=f"The number of columns with a type "
             f"mismatch is {invalid_types_count} out of {len(columns_type)}.",
             status=status,
-            columns_types=columns_types,
+            parameters=ColumnTypesParameter(columns=columns),
+            group=self.group,
         )
 
 
 @default_renderer(wrap_type=TestColumnsType)
 class TestColumnsTypeRenderer(TestRenderer):
-    def render_json(self, obj: TestColumnsType) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["columns"] = [
-            dict(
-                column_name=column_name,
-                actual_type=types[0],
-                expected_type=types[1],
-            )
-            for column_name, types in obj.get_result().columns_types.items()
-        ]
-        return base
-
     def render_html(self, obj: TestColumnsType) -> TestHtmlInfo:
         info = super().render_html(obj)
 
+        parameters = obj.get_result().parameters
+        assert isinstance(parameters, ColumnTypesParameter)
         info.details = [
             DetailsInfo(
                 title="",
                 info=BaseWidgetInfo(
                     title="",
                     type="table",
                     params={
                         "header": ["Column Name", "Actual Type", "Expected Type"],
-                        "data": [
-                            [column_name, *types] for column_name, types in obj.get_result().columns_types.items()
-                        ],
+                        "data": [[c.column_name, c.actual_type, c.expected_type] for c in parameters.columns],
                     },
                     size=2,
                 ),
             ),
         ]
         return info
 
@@ -1196,15 +1014,15 @@
         metric_result = self.metric.get_result()
 
         if metric_result.reference:
             ref_value = metric_result.reference.number_of_not_matched
             mult = metric_result.current.number_of_rows / metric_result.reference.number_of_rows
 
             if mult is not None:
-                return TestValueCondition(eq=approx(ref_value * mult, relative=0.1))
+                return TestValueCondition(eq=approx(ref_value * mult, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         return self.metric.get_result().current.number_of_not_matched
 
     def get_description(self, value: Numeric) -> str:
```

### Comparing `evidently-0.2.8/src/evidently/tests/data_quality_tests.py` & `evidently-0.3.0/src/evidently/tests/data_quality_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 from abc import ABC
+from typing import Any
+from typing import ClassVar
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
-import numpy as np
 import pandas as pd
 
+from evidently.base_metric import ColumnName
 from evidently.calculations.data_quality import get_corr_method
 from evidently.metric_results import DatasetColumns
 from evidently.metrics import ColumnQuantileMetric
 from evidently.metrics import ColumnSummaryMetric
 from evidently.metrics import ColumnValueListMetric
 from evidently.metrics import ColumnValueRangeMetric
 from evidently.metrics import ConflictPredictionMetric
 from evidently.metrics import ConflictTargetMetric
 from evidently.metrics import DatasetCorrelationsMetric
+from evidently.metrics.data_integrity.column_summary_metric import CategoricalCharacteristics
+from evidently.metrics.data_integrity.column_summary_metric import ColumnCharacteristics
 from evidently.metrics.data_integrity.column_summary_metric import ColumnSummaryResult
+from evidently.metrics.data_integrity.column_summary_metric import DatetimeCharacteristics
 from evidently.metrics.data_integrity.column_summary_metric import NumericCharacteristics
 from evidently.metrics.data_integrity.column_summary_metric import TextCharacteristics
+from evidently.metrics.data_quality.dataset_correlations_metric import DatasetCorrelation
 from evidently.renderers.base_renderer import TestHtmlInfo
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.renderers.render_utils import get_distribution_plot_figure
 from evidently.renderers.render_utils import plot_distr
 from evidently.tests.base_test import BaseCheckValueTest
+from evidently.tests.base_test import CheckValueParameters
+from evidently.tests.base_test import ColumnCheckValueParameters
+from evidently.tests.base_test import ConditionFromReferenceMixin
 from evidently.tests.base_test import GroupData
 from evidently.tests.base_test import GroupingTypes
 from evidently.tests.base_test import Test
+from evidently.tests.base_test import TestParameters
 from evidently.tests.base_test import TestResult
+from evidently.tests.base_test import TestStatus
 from evidently.tests.base_test import TestValueCondition
+from evidently.tests.base_test import ValueSource
 from evidently.tests.utils import approx
 from evidently.tests.utils import plot_check
 from evidently.tests.utils import plot_correlations
 from evidently.tests.utils import plot_metric_value
 from evidently.tests.utils import plot_value_counts_tables
 from evidently.tests.utils import plot_value_counts_tables_ref_curr
 from evidently.utils.generators import BaseGenerator
 from evidently.utils.types import Numeric
 
 DATA_QUALITY_GROUP = GroupData("data_quality", "Data Quality", "")
 GroupingTypes.TestGroup.add_value(DATA_QUALITY_GROUP)
 
 
-class BaseDataQualityMetricsValueTest(BaseCheckValueTest, ABC):
+class BaseDataQualityMetricsValueTest(ConditionFromReferenceMixin[ColumnCharacteristics], ABC):
+    reference_field: ClassVar = "reference_characteristics"
     group = DATA_QUALITY_GROUP.id
     metric: ColumnSummaryMetric
 
     def __init__(
         self,
         column_name: str,
         eq: Optional[Numeric] = None,
@@ -81,55 +94,55 @@
     def __init__(self):
         self.metric = ConflictTargetMetric()
 
     def check(self):
         metric_result = self.metric.get_result()
 
         if metric_result.number_not_stable_target is None:
-            test_result = TestResult.ERROR
+            test_result = TestStatus.ERROR
             description = "No target in the dataset"
 
         elif metric_result.number_not_stable_target > 0:
-            test_result = TestResult.FAIL
+            test_result = TestStatus.FAIL
             description = f"Not stable target rows count is {metric_result.number_not_stable_target}"
 
         else:
-            test_result = TestResult.SUCCESS
+            test_result = TestStatus.SUCCESS
             description = "Target is stable"
 
-        return TestResult(name=self.name, description=description, status=test_result)
+        return TestResult(name=self.name, description=description, status=test_result, group=self.group)
 
 
 class TestConflictPrediction(Test):
     group = DATA_QUALITY_GROUP.id
     name = "Test number of conflicts in prediction"
     metric: ConflictPredictionMetric
 
     def __init__(self):
         self.metric = ConflictPredictionMetric()
 
     def check(self):
         metric_result = self.metric.get_result()
 
         if metric_result.current.number_not_stable_prediction is None:
-            test_result = TestResult.ERROR
+            test_result = TestStatus.ERROR
             description = "No prediction in the dataset"
 
         elif metric_result.current.number_not_stable_prediction > 0:
-            test_result = TestResult.FAIL
+            test_result = TestStatus.FAIL
             description = f"Not stable prediction rows count is {metric_result.current.number_not_stable_prediction}"
 
         else:
-            test_result = TestResult.SUCCESS
+            test_result = TestStatus.SUCCESS
             description = "Prediction is stable"
 
-        return TestResult(name=self.name, description=description, status=test_result)
+        return TestResult(name=self.name, description=description, status=test_result, group=self.group)
 
 
-class BaseDataQualityCorrelationsMetricsValueTest(BaseCheckValueTest, ABC):
+class BaseDataQualityCorrelationsMetricsValueTest(ConditionFromReferenceMixin[DatasetCorrelation], ABC):
     group = DATA_QUALITY_GROUP.id
     metric: DatasetCorrelationsMetric
     method: Optional[str]
 
     def __init__(
         self,
         method: Optional[str] = None,
@@ -155,26 +168,21 @@
         )
         self.metric = DatasetCorrelationsMetric()
 
 
 class TestTargetPredictionCorrelation(BaseDataQualityCorrelationsMetricsValueTest):
     name = "Correlation between Target and Prediction"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference = self.metric.get_result().reference
-
+    def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
         if reference is not None:
             method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
             value = reference.stats[method].target_prediction_correlation
 
             if value is not None:
-                return TestValueCondition(eq=approx(value, absolute=0.25))
+                return TestValueCondition(eq=approx(value, absolute=0.25), source=ValueSource.REFERENCE)
 
         return TestValueCondition(gt=0)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
         return self.metric.get_result().current.stats[method].target_prediction_correlation
 
@@ -186,43 +194,32 @@
             f"The test threshold is {self.get_condition()}."
         )
 
 
 class TestHighlyCorrelatedColumns(BaseDataQualityCorrelationsMetricsValueTest):
     name = "Highly Correlated Columns"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_correlation = self.metric.get_result().reference
-
-        if reference_correlation is not None:
-            value = reference_correlation.stats[get_corr_method(self.method)].abs_max_features_correlation
+    def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
+        if reference is not None:
+            value = reference.stats[get_corr_method(self.method)].abs_max_features_correlation
 
             if value is not None:
-                return TestValueCondition(eq=approx(value, relative=0.1))
+                return TestValueCondition(eq=approx(value, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(lt=0.9)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         return self.metric.get_result().current.stats[get_corr_method(self.method)].abs_max_features_correlation
 
     def get_description(self, value: Numeric) -> str:
         return f"The maximum correlation is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestHighlyCorrelatedColumns)
 class TestHighlyCorrelatedColumnsRenderer(TestRenderer):
-    def render_json(self, obj: TestHighlyCorrelatedColumns) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["abs_max_num_features_correlation"] = np.round(obj.value, 3)
-        return base
-
     def render_html(self, obj: TestHighlyCorrelatedColumns) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         method = get_corr_method(obj.method)
         current_correlations = metric_result.current.correlation[method]
 
         if metric_result.reference is not None:
@@ -235,26 +232,21 @@
         info.with_details("Highly Correlated Features", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestTargetFeaturesCorrelations(BaseDataQualityCorrelationsMetricsValueTest):
     name = "Correlation between Target and Features"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_correlation = self.metric.get_result().reference
-
-        if reference_correlation is not None:
+    def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
+        if reference is not None:
             method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
-            value = reference_correlation.stats[method].abs_max_target_features_correlation
+            value = reference.stats[method].abs_max_target_features_correlation
 
             if value is not None:
-                return TestValueCondition(eq=approx(value, relative=0.1))
+                return TestValueCondition(eq=approx(value, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(lt=0.9)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
         return self.metric.get_result().current.stats[method].abs_max_target_features_correlation
 
@@ -262,58 +254,21 @@
         if value is None:
             return "No target in the current dataset"
 
         else:
             return f"The maximum correlation is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestTargetFeaturesCorrelations)
-class TestTargetFeaturesCorrelationsRenderer(TestRenderer):
-    def render_json(self, obj: TestTargetFeaturesCorrelations) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-
-        if obj.value is not None:
-            abs_max_target_features_correlation = np.round(obj.value, 3)
-
-        else:
-            abs_max_target_features_correlation = obj.value
-
-        base["parameters"]["abs_max_target_features_correlation"] = abs_max_target_features_correlation
-        return base
-
-    def render_html(self, obj: TestTargetFeaturesCorrelations) -> TestHtmlInfo:
-        info = super().render_html(obj)
-        metric_result = obj.metric.get_result()
-        method = get_corr_method(obj.method, metric_result.target_correlation, False)
-        current_correlations = metric_result.current.correlation[method]
-
-        if metric_result.reference is not None:
-            reference_correlations: Optional[pd.DataFrame] = metric_result.reference.correlation[method]
-
-        else:
-            reference_correlations = None
-
-        fig = plot_correlations(current_correlations, reference_correlations)
-        info.with_details("Target Features Correlations", plotly_figure(title="", figure=fig))
-        return info
-
-
 class TestPredictionFeaturesCorrelations(BaseDataQualityCorrelationsMetricsValueTest):
     name = "Correlation between Prediction and Features"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-
-        reference_correlation = self.metric.get_result().reference
-
-        if reference_correlation is not None:
+    def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
+        if reference is not None:
             method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
-            value = reference_correlation.stats[method].abs_max_prediction_features_correlation
+            value = reference.stats[method].abs_max_prediction_features_correlation
 
             if value is not None:
                 return TestValueCondition(eq=approx(value, relative=0.1))
 
         return TestValueCondition(lt=0.9)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
@@ -325,28 +280,16 @@
             return "No prediction in the current dataset"
 
         else:
             return f"The maximum correlation is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestPredictionFeaturesCorrelations)
+@default_renderer(wrap_type=TestTargetFeaturesCorrelations)
 class TestPredictionFeaturesCorrelationsRenderer(TestRenderer):
-    def render_json(self, obj: TestPredictionFeaturesCorrelations) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-
-        if obj.value is not None:
-            abs_max_prediction_features_correlation = np.round(obj.value, 3)
-
-        else:
-            abs_max_prediction_features_correlation = obj.value
-
-        base["parameters"]["abs_max_prediction_features_correlation"] = abs_max_prediction_features_correlation
-        return base
-
     def render_html(self, obj: TestTargetFeaturesCorrelations) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         method = get_corr_method(obj.method, metric_result.target_correlation, False)
         current_correlations = metric_result.current.correlation[method]
 
         if metric_result.reference is not None:
@@ -388,14 +331,17 @@
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
         self.corr_diff = corr_diff
 
+    def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
+        pass
+
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
 
         return TestValueCondition(eq=0)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
@@ -466,95 +412,62 @@
 
     def groups(self) -> Dict[str, str]:
         return {
             GroupingTypes.ByFeature.id: self.column_name,
         }
 
     def check(self):
-        result = TestResult(
-            name=self.name,
-            description="The test was not launched",
-            status=TestResult.SKIPPED,
-        )
-        # features_stats = self.metric.get_result().features_stats.get_all_features()
-
-        # if self.column_name not in features_stats:
-        #     result.mark_as_fail(f"Feature '{self.column_name}' was not found")
-        #     return result
-
         result = super().check()
 
         if self.value is None:
             result.mark_as_error(f"No value for the feature '{self.column_name}'")
             return result
 
         return result
 
+    def get_stat(self, current: NumericCharacteristics):
+        raise NotImplementedError
+
 
 class TestColumnValueMin(BaseFeatureDataQualityMetricsTest):
     name = "Min Value"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
+    def get_stat(self, current: NumericCharacteristics):
+        return current.min
 
-        ref_features_stats = self.metric.get_result().reference_characteristics
-        if ref_features_stats is not None:
-            if not isinstance(ref_features_stats, NumericCharacteristics):
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, NumericCharacteristics):
                 raise ValueError(f"{self.column_name} should be numerical or bool")
-            min_value = ref_features_stats.min
+            min_value = reference.min
             return TestValueCondition(gte=min_value)
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Optional[Union[Numeric, bool]]:
         features_stats = self.metric.get_result().current_characteristics
         if not isinstance(features_stats, NumericCharacteristics):
             raise ValueError(f"{self.column_name} should be numerical or bool")
         min_value = features_stats.min
         return min_value
 
     def get_description(self, value: Numeric) -> str:
         return f"The minimum value of the column **{self.column_name}** is {value} The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestColumnValueMin)
-class TestColumnValueMinRenderer(TestRenderer):
-    def render_html(self, obj: TestColumnValueMin) -> TestHtmlInfo:
-        column_name = obj.column_name
-        info = super().render_html(obj)
-        metric_result: ColumnSummaryResult = obj.metric.get_result()
-        bins_for_hist = metric_result.plot_data.bins_for_hist
-        if bins_for_hist is None:
-            raise ValueError(f"{column_name} should be numerical or bool")
-        curr_distr = bins_for_hist.current
-        ref_distr = bins_for_hist.reference
-        fig = plot_distr(hist_curr=curr_distr, hist_ref=ref_distr, color_options=self.color_options)
-        fig = plot_check(fig, obj.get_condition(), color_options=self.color_options)
-        current_characteristics = metric_result.current_characteristics
-        if not isinstance(current_characteristics, NumericCharacteristics):
-            raise ValueError(f"{column_name} should be numerical or bool")
-        min_value = current_characteristics.min
-
-        if min_value is not None:
-            fig = plot_metric_value(fig, float(min_value), f"current {column_name} min value")
-        info.with_details(f"Min Value {column_name}", plotly_figure(title="", figure=fig))
-        return info
-
-
 class TestColumnValueMax(BaseFeatureDataQualityMetricsTest):
     name = "Max Value"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-        ref_features_stats = self.metric.get_result().reference_characteristics
-        if ref_features_stats is not None:
-            if not isinstance(ref_features_stats, NumericCharacteristics):
+    def get_stat(self, current: NumericCharacteristics):
+        return current.max
+
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, NumericCharacteristics):
                 raise ValueError(f"{self.column_name} should be numerical or bool")
-            max_value = ref_features_stats.max
+            max_value = reference.max
             return TestValueCondition(lte=max_value)
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Optional[Union[Numeric, bool]]:
         features_stats = self.metric.get_result().current_characteristics
         if not isinstance(features_stats, NumericCharacteristics):
             raise ValueError(f"{self.column_name} should be numerical or bool")
@@ -563,143 +476,102 @@
             raise ValueError(f"{self.column_name} should be numerical or bool")
         return max_value
 
     def get_description(self, value: Numeric) -> str:
         return f"The maximum value of the column **{self.column_name}** is {value}. The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestColumnValueMax)
-class TestColumnValueMaxRenderer(TestRenderer):
-    def render_html(self, obj: TestColumnValueMax) -> TestHtmlInfo:
-        column_name = obj.column_name
-        info = super().render_html(obj)
-        metric_result: ColumnSummaryResult = obj.metric.get_result()
-        bins_for_hist = metric_result.plot_data.bins_for_hist
-        if bins_for_hist is None:
-            raise ValueError(f"{column_name} should be numerical or bool")
-        curr_distr = bins_for_hist.current
-        ref_distr = bins_for_hist.reference
-        fig = plot_distr(hist_curr=curr_distr, hist_ref=ref_distr, color_options=self.color_options)
-        fig = plot_check(fig, obj.get_condition(), color_options=self.color_options)
-        current_characteristics = metric_result.current_characteristics
-        if not isinstance(current_characteristics, NumericCharacteristics):
-            raise ValueError(f"{column_name} should be numerical or bool")
-        max_value = current_characteristics.max
-
-        if max_value is not None:
-            fig = plot_metric_value(fig, float(max_value), f"current {column_name} max value")
-        info.with_details(f"Max Value {column_name}", plotly_figure(title="", figure=fig))
-        return info
-
-
 class TestColumnValueMean(BaseFeatureDataQualityMetricsTest):
     name = "Mean Value"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-        ref_features_stats = self.metric.get_result().reference_characteristics
-        if ref_features_stats is not None:
-            if not isinstance(ref_features_stats, NumericCharacteristics):
+    def get_stat(self, current: NumericCharacteristics):
+        return current.mean
+
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, NumericCharacteristics):
                 raise ValueError(f"{self.column_name} should be numerical or bool")
-            return TestValueCondition(eq=approx(ref_features_stats.mean, 0.1))
+            return TestValueCondition(eq=approx(reference.mean, 0.1))
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         features_stats = self.metric.get_result().current_characteristics
         if not isinstance(features_stats, NumericCharacteristics):
             raise ValueError(f"{self.column_name} should be numerical or bool")
         return features_stats.mean
 
     def get_description(self, value: Numeric) -> str:
         return f"The mean value of the column **{self.column_name}** is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
-@default_renderer(wrap_type=TestColumnValueMean)
-class TestColumnValueMeanRenderer(TestRenderer):
-    def render_html(self, obj: TestColumnValueMean) -> TestHtmlInfo:
-        column_name = obj.column_name
-        info = super().render_html(obj)
-        metric_result: ColumnSummaryResult = obj.metric.get_result()
-        bins_for_hist = metric_result.plot_data.bins_for_hist
-        if bins_for_hist is None:
-            raise ValueError(f"{column_name} should be numerical or bool")
-        curr_distr = bins_for_hist.current
-        ref_distr = bins_for_hist.reference
-        fig = plot_distr(hist_curr=curr_distr, hist_ref=ref_distr, color_options=self.color_options)
-        fig = plot_check(fig, obj.get_condition(), color_options=self.color_options)
-        current_characteristics = metric_result.current_characteristics
-        if not isinstance(current_characteristics, NumericCharacteristics):
-            raise ValueError(f"{column_name} should be numerical or bool")
-        mean_value = current_characteristics.mean
-
-        if mean_value is not None:
-            fig = plot_metric_value(fig, mean_value, f"current {column_name} mean value")
-        info.with_details(f"Mean Value {column_name}", plotly_figure(title="", figure=fig))
-        return info
-
-
 class TestColumnValueMedian(BaseFeatureDataQualityMetricsTest):
     name = "Median Value"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-        ref_features_stats = self.metric.get_result().reference_characteristics
-        if ref_features_stats is not None:
-            if not isinstance(ref_features_stats, NumericCharacteristics):
+    def get_stat(self, current: NumericCharacteristics):
+        return current.p50
+
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, NumericCharacteristics):
                 raise ValueError(f"{self.column_name} should be numerical or bool")
-            return TestValueCondition(eq=approx(ref_features_stats.p50, 0.1))
+            return TestValueCondition(eq=approx(reference.p50, 0.1))
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         features_stats = self.metric.get_result().current_characteristics
         if not isinstance(features_stats, NumericCharacteristics):
             raise ValueError(f"{self.column_name} should be numerical or bool")
         return features_stats.p50
 
     def get_description(self, value: Numeric) -> str:
         return f"The median value of the column **{self.column_name}** is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
+@default_renderer(wrap_type=TestColumnValueMin)
+@default_renderer(wrap_type=TestColumnValueMax)
+@default_renderer(wrap_type=TestColumnValueMean)
 @default_renderer(wrap_type=TestColumnValueMedian)
-class TestColumnValueMedianRenderer(TestRenderer):
-    def render_html(self, obj: TestColumnValueMedian) -> TestHtmlInfo:
+class TestColumnValueFeatureRenderer(TestRenderer):
+    def render_html(self, obj: BaseFeatureDataQualityMetricsTest) -> TestHtmlInfo:
+        column_name, fig, info, metric_result = self._feature_render_html(obj)
+        fig = plot_check(fig, obj.get_condition(), color_options=self.color_options)
+        current_characteristics = metric_result.current_characteristics
+        if not isinstance(current_characteristics, NumericCharacteristics):
+            raise ValueError(f"{column_name} should be numerical or bool")
+
+        value = obj.get_stat(current_characteristics)
+        if value is not None:
+            fig = plot_metric_value(fig, float(value), f"current {column_name} {obj.name.lower()}")
+        info.with_details(f"{obj.name} {column_name}", plotly_figure(title="", figure=fig))
+        return info
+
+    def _feature_render_html(self, obj):
         column_name = obj.column_name
         info = super().render_html(obj)
         metric_result: ColumnSummaryResult = obj.metric.get_result()
         bins_for_hist = metric_result.plot_data.bins_for_hist
         if bins_for_hist is None:
             raise ValueError(f"{column_name} should be numerical or bool")
         curr_distr = bins_for_hist.current
         ref_distr = bins_for_hist.reference
         fig = plot_distr(hist_curr=curr_distr, hist_ref=ref_distr, color_options=self.color_options)
-        fig = plot_check(fig, obj.get_condition(), color_options=self.color_options)
-        current_characteristics = metric_result.current_characteristics
-        if not isinstance(current_characteristics, NumericCharacteristics):
-            raise ValueError(f"{column_name} should be numerical or bool")
-        percentile_50 = current_characteristics.p50
-
-        if percentile_50 is not None:
-            fig = plot_metric_value(fig, percentile_50, f"current {column_name} median value")
-        info.with_details(f"Median Value {column_name}", plotly_figure(title="", figure=fig))
-        return info
+        return column_name, fig, info, metric_result
 
 
 class TestColumnValueStd(BaseFeatureDataQualityMetricsTest):
     name = "Standard Deviation (SD)"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-        ref_features_stats = self.metric.get_result().reference_characteristics
-        if ref_features_stats is not None:
-            if not isinstance(ref_features_stats, NumericCharacteristics):
+    def get_stat(self, current: NumericCharacteristics):
+        return current.std
+
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, NumericCharacteristics):
                 raise ValueError(f"{self.column_name} should be numerical or bool")
-            return TestValueCondition(eq=approx(ref_features_stats.std, 0.1))
+            return TestValueCondition(eq=approx(reference.std, 0.1))
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         features_stats = self.metric.get_result().current_characteristics
         if not isinstance(features_stats, NumericCharacteristics):
             raise ValueError(f"{self.column_name} should be numerical or bool")
         return features_stats.std
@@ -708,41 +580,32 @@
         return (
             f"The standard deviation of the column **{self.column_name}** is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
 @default_renderer(wrap_type=TestColumnValueStd)
-class TestColumnValueStdRenderer(TestRenderer):
-    def render_html(self, obj: TestColumnValueStd) -> TestHtmlInfo:
-        column_name = obj.column_name
-        info = super().render_html(obj)
-        metric_result: ColumnSummaryResult = obj.metric.get_result()
-        bins_for_hist = metric_result.plot_data.bins_for_hist
-        if bins_for_hist is None:
-            raise ValueError(f"{column_name} should be numerical or bool")
-        curr_distr = bins_for_hist.current
-        ref_distr = bins_for_hist.reference
-        fig = plot_distr(hist_curr=curr_distr, hist_ref=ref_distr, color_options=self.color_options)
+class TestColumnValueStdRenderer(TestColumnValueFeatureRenderer):
+    def render_html(self, obj: BaseFeatureDataQualityMetricsTest) -> TestHtmlInfo:
+        column_name, fig, info, _ = self._feature_render_html(obj)
         info.with_details(f"Std Value {column_name}", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestNumberOfUniqueValues(BaseFeatureDataQualityMetricsTest):
     name = "Number of Unique Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
+    def get_stat(self, current: NumericCharacteristics):
+        return current.unique
 
-        reference_features_stats = self.metric.get_result().reference_characteristics
-        if reference_features_stats is not None:
-            if isinstance(reference_features_stats, TextCharacteristics):
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, (NumericCharacteristics, CategoricalCharacteristics, DatetimeCharacteristics)):
                 raise ValueError(f"{self.column_name} should be numerical, categorical or datetime")
-            unique_count = reference_features_stats.unique
+            unique_count = reference.unique
             return TestValueCondition(eq=approx(unique_count, relative=0.1))
 
         return TestValueCondition(gt=1)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
         features_stats = self.metric.get_result().current_characteristics
         if isinstance(features_stats, TextCharacteristics):
@@ -771,23 +634,22 @@
 
         return info
 
 
 class TestUniqueValuesShare(BaseFeatureDataQualityMetricsTest):
     name = "Share of Unique Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
+    def get_stat(self, current: NumericCharacteristics):
+        return current.unique_percentage
 
-        reference_features_stats = self.metric.get_result().reference_characteristics
-        if reference_features_stats is not None:
-            if isinstance(reference_features_stats, TextCharacteristics):
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, (NumericCharacteristics, CategoricalCharacteristics, DatetimeCharacteristics)):
                 raise ValueError(f"{self.column_name} should be numerical, categorical or datetime")
-            unique_percentage = reference_features_stats.unique_percentage
+            unique_percentage = reference.unique_percentage
 
             if unique_percentage is not None:
                 return TestValueCondition(eq=approx(unique_percentage / 100.0, relative=0.1))
 
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
@@ -823,23 +685,22 @@
 
         return info
 
 
 class TestMostCommonValueShare(BaseFeatureDataQualityMetricsTest):
     name = "Share of the Most Common Value"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
+    def get_stat(self, current: NumericCharacteristics):
+        return current.most_common_percentage
 
-        reference_features_stats = self.metric.get_result().reference_characteristics
-        if reference_features_stats is not None:
-            if isinstance(reference_features_stats, TextCharacteristics):
+    def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
+        if reference is not None:
+            if not isinstance(reference, (NumericCharacteristics, CategoricalCharacteristics, DatetimeCharacteristics)):
                 raise ValueError(f"{self.column_name} should be numerical, categorical or datetime")
-            most_common_percentage = reference_features_stats.most_common_percentage
+            most_common_percentage = reference.most_common_percentage
 
             if most_common_percentage is not None:
                 return TestValueCondition(eq=approx(most_common_percentage / 100.0, relative=0.1))
 
         return TestValueCondition(lt=0.8)
 
     def calculate_value_for_test(self) -> Optional[Numeric]:
@@ -860,24 +721,22 @@
         most_common_value = counts_data["current"].iloc[0, 0]
         return (
             f"The most common value in the column **{self.column_name}** is {most_common_value}. "
             f"Its share is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
+    def get_parameters(self) -> ColumnCheckValueParameters:
+        return ColumnCheckValueParameters(
+            column_name=self.column_name, condition=self.get_condition(), value=self.value
+        )
+
 
 @default_renderer(wrap_type=TestMostCommonValueShare)
 class TestMostCommonValueShareRenderer(TestRenderer):
-    def render_json(self, obj: TestMostCommonValueShare) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["column_name"] = obj.column_name
-        base["parameters"]["share_most_common_value"] = obj.value
-        return base
-
     def render_html(self, obj: TestMostCommonValueShare) -> TestHtmlInfo:
         info = super().render_html(obj)
         column_name = obj.column_name
 
         if column_name is None:
             raise ValueError("column_name should be present")
 
@@ -906,15 +765,24 @@
 
         else:
             columns = self.columns
 
         return [TestMostCommonValueShare(column_name=name) for name in columns]
 
 
+class MeanInNSigmasParameter(TestParameters):
+    column_name: str
+    current_mean: float
+    n_sigmas: int  # ? float
+    reference_mean: float
+    reference_std: float
+
+
 class TestMeanInNSigmas(Test):
+
     group = DATA_QUALITY_GROUP.id
     name = "Mean Value Stability"
     metric: ColumnSummaryMetric
     column_name: str
     n_sigmas: int
 
     def __init__(self, column_name: str, n_sigmas: int = 2):
@@ -922,66 +790,67 @@
         self.n_sigmas = n_sigmas
         self.metric = ColumnSummaryMetric(column_name)
 
     def check(self):
         reference_feature_stats = self.metric.get_result().reference_characteristics
         features_stats = self.metric.get_result().current_characteristics
 
+        # todo: this was thrown in a render, do we just cut it?
+        # if not isinstance(features_stats, NumericCharacteristics):
+        #     raise ValueError(f"{self.column_name} should be numerical or bool")
+
         if reference_feature_stats is None:
-            test_result = TestResult.ERROR
+            test_result = TestStatus.ERROR
             description = "Reference should be present"
-
+            parameters = None
         else:
+            # todo: look up
+            # if not isinstance(reference_feature_stats, NumericCharacteristics):
+            #     raise ValueError(f"{self.column_name} should be numerical or bool")
             current_mean = features_stats.mean
             reference_mean = reference_feature_stats.mean
             reference_std = reference_feature_stats.std
             sigmas_value = reference_std * self.n_sigmas
             left_condition = reference_mean - sigmas_value
             right_condition = reference_mean + sigmas_value
 
             if left_condition < current_mean < right_condition:
                 description = (
                     f"The mean value of the column **{self.column_name}** is {current_mean:.3g}."
                     f" The expected range is from {left_condition:.3g} to {right_condition:.3g}"
                 )
-                test_result = TestResult.SUCCESS
+                test_result = TestStatus.SUCCESS
 
             else:
                 description = (
                     f"The mean value of the column **{self.column_name}** is {current_mean:.3g}."
                     f" The expected range is from {left_condition:.3g} to {right_condition:.3g}"
                 )
-                test_result = TestResult.FAIL
+                test_result = TestStatus.FAIL
+
+            parameters = MeanInNSigmasParameter(
+                column_name=self.column_name,
+                n_sigmas=self.n_sigmas,
+                current_mean=current_mean,
+                reference_mean=reference_mean,
+                reference_std=reference_std,
+            )
 
         return TestResult(
             name=self.name,
             description=description,
             status=test_result,
             groups={GroupingTypes.ByFeature.id: self.column_name},
+            parameters=parameters,
+            group=self.group,
         )
 
 
 @default_renderer(wrap_type=TestMeanInNSigmas)
 class TestMeanInNSigmasRenderer(TestRenderer):
-    def render_json(self, obj: TestMeanInNSigmas) -> dict:
-        base = super().render_json(obj)
-        metric_result = obj.metric.get_result()
-        base["parameters"]["column_name"] = obj.column_name
-        base["parameters"]["n_sigmas"] = obj.n_sigmas
-        if not isinstance(metric_result.current_characteristics, NumericCharacteristics):
-            raise ValueError(f"{obj.column_name} should be numerical or bool")
-        base["parameters"]["current_mean"] = metric_result.current_characteristics.mean
-
-        if metric_result.reference_characteristics is not None:
-            if not isinstance(metric_result.reference_characteristics, NumericCharacteristics):
-                raise ValueError(f"{obj.column_name} should be numerical or bool")
-            base["parameters"]["reference_mean"] = metric_result.reference_characteristics.mean
-            base["parameters"]["reference_std"] = metric_result.reference_characteristics.std
-        return base
-
     def render_html(self, obj: TestMeanInNSigmas) -> TestHtmlInfo:
         column_name = obj.column_name
         metric_result: ColumnSummaryResult = obj.metric.get_result()
         info = super().render_html(obj)
 
         if metric_result.reference_characteristics is None or metric_result.plot_data.bins_for_hist is None:
             return info
@@ -1031,39 +900,48 @@
         return [TestMeanInNSigmas(column_name=name, n_sigmas=2) for name in columns]
 
 
 class TestValueRange(Test):
     group = DATA_QUALITY_GROUP.id
     name = "Value Range"
     metric: ColumnValueRangeMetric
-    column: str
+    column_name: ColumnName
     left: Optional[float]
     right: Optional[float]
 
-    def __init__(self, column_name: str, left: Optional[float] = None, right: Optional[float] = None):
-        self.column_name = column_name
+    def __init__(
+        self,
+        column_name: Union[str, ColumnName],
+        left: Optional[float] = None,
+        right: Optional[float] = None,
+    ):
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
         self.left = left
         self.right = right
-        self.metric = ColumnValueRangeMetric(column_name=column_name, left=left, right=right)
+        self.metric = ColumnValueRangeMetric(column_name=self.column_name, left=left, right=right)
 
     def check(self):
         number_not_in_range = self.metric.get_result().current.number_not_in_range
 
         if number_not_in_range > 0:
             description = f"The column **{self.column_name}** has values out of range."
-            test_result = TestResult.FAIL
+            test_result = TestStatus.FAIL
         else:
             description = f"All values in the column **{self.column_name}** are within range"
-            test_result = TestResult.SUCCESS
+            test_result = TestStatus.SUCCESS
 
         return TestResult(
             name=self.name,
             description=description,
             status=test_result,
-            groups={GroupingTypes.ByFeature.id: self.column_name},
+            groups={GroupingTypes.ByFeature.id: self.column_name.display_name},
+            group=self.group,
         )
 
 
 @default_renderer(wrap_type=TestValueRange)
 class TestValueRangeRenderer(TestRenderer):
     def render_html(self, obj: TestValueRange) -> TestHtmlInfo:
         column_name = obj.column_name
@@ -1074,40 +952,46 @@
             current_distribution=metric_result.current.distribution,
             reference_distribution=metric_result.reference.distribution
             if metric_result.reference is not None
             else None,
             color_options=self.color_options,
         )
         fig = plot_check(fig, condition_, color_options=self.color_options)
-        info.with_details(f"Value Range {column_name}", plotly_figure(title="", figure=fig))
+        info.with_details(
+            f"Value Range {column_name.display_name}",
+            plotly_figure(title="", figure=fig),
+        )
         return info
 
 
 class BaseDataQualityValueRangeMetricsTest(BaseCheckValueTest, ABC):
     group = DATA_QUALITY_GROUP.id
     metric: ColumnValueRangeMetric
-    column: str
+    column_name: ColumnName
     left: Optional[float]
     right: Optional[float]
 
     def __init__(
         self,
-        column_name: str,
+        column_name: Union[str, ColumnName],
         left: Optional[float] = None,
         right: Optional[float] = None,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
-        self.column_name = column_name
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
         self.left = left
         self.right = right
         self.metric = ColumnValueRangeMetric(column_name=column_name, left=left, right=right)
 
         super().__init__(
             eq=eq,
             gt=gt,
@@ -1116,99 +1000,76 @@
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
 
     def groups(self) -> Dict[str, str]:
-        return {GroupingTypes.ByFeature.id: self.column_name}
-
-
-class TestNumberOfOutRangeValues(BaseDataQualityValueRangeMetricsTest):
-    name = "Number of Out-of-Range Values "
+        return {GroupingTypes.ByFeature.id: self.column_name.display_name}
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         return TestValueCondition(eq=approx(0))
 
+
+class TestNumberOfOutRangeValues(BaseDataQualityValueRangeMetricsTest):
+    name = "Number of Out-of-Range Values "
+
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_not_in_range
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The number of values out of range in the column **{self.column_name}** is {value}. "
             f" The test threshold is {self.get_condition()}."
         )
 
 
-@default_renderer(wrap_type=TestNumberOfOutRangeValues)
-class TestNumberOfOutRangeValuesRenderer(TestRenderer):
-    def render_html(self, obj: TestNumberOfOutRangeValues) -> TestHtmlInfo:
-        column_name = obj.column_name
-        metric_result = obj.metric.get_result()
-        info = super().render_html(obj)
-        fig = get_distribution_plot_figure(
-            current_distribution=metric_result.current.distribution,
-            reference_distribution=metric_result.reference.distribution
-            if metric_result.reference is not None
-            else None,
-            color_options=self.color_options,
-        )
-        fig = plot_check(fig, obj.condition, color_options=self.color_options)
-        info.with_details(
-            f"Number Out of Range for {column_name}",
-            plotly_figure(title="", figure=fig),
-        )
-        return info
+class ShareOfOutRangeParameters(CheckValueParameters):
+    left: Optional[float]
+    right: Optional[float]
 
 
 class TestShareOfOutRangeValues(BaseDataQualityValueRangeMetricsTest):
     name = "Share of Out-of-Range Values"
 
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-        return TestValueCondition(eq=approx(0))
-
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_not_in_range
 
     def get_description(self, value: Numeric) -> str:
         current_result = self.metric.get_result().current
         return (
-            f"The share of values out of range in the column **{self.column_name}** is {value:.3g} "
+            f"The share of values out of range in the column **{self.column_name.display_name}** is {value:.3g} "
             f"({current_result.number_not_in_range} out of {current_result.number_of_values}). "
             f" The test threshold is {self.get_condition()}."
         )
 
+    def get_parameters(self) -> ShareOfOutRangeParameters:
+        return ShareOfOutRangeParameters(
+            condition=self.get_condition(), value=self.value, left=self.left, right=self.right
+        )
 
-@default_renderer(wrap_type=TestShareOfOutRangeValues)
-class TestShareOfOutRangeValuesRenderer(TestRenderer):
-    def render_json(self, obj: TestShareOfOutRangeValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["left"] = obj.left
-        base["parameters"]["right"] = obj.right
-        base["parameters"]["share_not_in_range"] = obj.value
-        return base
 
-    def render_html(self, obj: TestShareOfOutRangeValues) -> TestHtmlInfo:
+@default_renderer(wrap_type=TestShareOfOutRangeValues)
+@default_renderer(wrap_type=TestNumberOfOutRangeValues)
+class TestRangeValuesRenderer(TestRenderer):
+    def render_html(self, obj: BaseDataQualityValueRangeMetricsTest) -> TestHtmlInfo:
         column_name = obj.column_name
         metric_result = obj.metric.get_result()
         info = super().render_html(obj)
         fig = get_distribution_plot_figure(
             current_distribution=metric_result.current.distribution,
             reference_distribution=metric_result.reference.distribution
             if metric_result.reference is not None
             else None,
             color_options=self.color_options,
         )
         fig = plot_check(fig, obj.condition, color_options=self.color_options)
-        info.with_details(f"Share Out of Range for {column_name}", plotly_figure(title="", figure=fig))
+        info.with_details(f"{obj.name} for {column_name.display_name}", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestNumColumnsOutOfRangeValues(BaseGenerator):
     """Creates share of out of range values tests for all numeric columns"""
 
     columns: Optional[List[str]]
@@ -1222,73 +1083,58 @@
 
         else:
             columns = [column for column in self.columns if column in columns_info.num_feature_names]
 
         return [TestShareOfOutRangeValues(column_name=name) for name in columns]
 
 
+class ColumnValueListParameters(TestParameters):
+    value: Numeric
+    column_name: str
+    values: Optional[List[Any]] = None
+
+
 class TestValueList(Test):
     group = DATA_QUALITY_GROUP.id
     name = "Out-of-List Values"
+    alias = "value_list"
     metric: ColumnValueListMetric
     column_name: str
     values: Optional[list]
 
     def __init__(self, column_name: str, values: Optional[list] = None):
         self.column_name = column_name
         self.values = values
         self.metric = ColumnValueListMetric(column_name=column_name, values=values)
 
     def check(self):
         metric_result = self.metric.get_result()
 
         if metric_result.current.number_not_in_list > 0:
-            test_result = TestResult.FAIL
+            test_result = TestStatus.FAIL
             description = f"The column **{self.column_name}** has values out of list."
 
         else:
-            test_result = TestResult.SUCCESS
+            test_result = TestStatus.SUCCESS
             description = f"All values in the column **{self.column_name}** are in the list."
 
         return TestResult(
             name=self.name,
             description=description,
             status=test_result,
             groups={GroupingTypes.ByFeature.id: self.column_name},
+            group=self.group,
+            parameters=ColumnValueListParameters(
+                value=metric_result.current.number_not_in_list, values=self.values, column_name=self.column_name
+            ),
         )
 
 
-@default_renderer(wrap_type=TestValueList)
-class TestValueListRenderer(TestRenderer):
-    def render_json(self, obj: TestValueList) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["column_name"] = obj.column_name
-        base["parameters"]["values"] = obj.values
-        base["parameters"]["number_not_in_list"] = obj.metric.get_result().current.number_not_in_list
-        return base
-
-    def render_html(self, obj: TestValueList) -> TestHtmlInfo:
-        info = super().render_html(obj)
-        metric_result = obj.metric.get_result()
-        column_name = metric_result.column_name
-        values = metric_result.values
-        curr_df = pd.DataFrame(metric_result.current.values_in_list.items(), columns=["x", "count"])
-
-        if metric_result.reference is not None:
-            ref_df = pd.DataFrame(metric_result.reference.values_in_list.items(), columns=["x", "count"])
-
-        else:
-            ref_df = None
-
-        additional_plots = plot_value_counts_tables(column_name, values, curr_df, ref_df, "value_list")
-        info.details = additional_plots
-        return info
-
-
 class BaseDataQualityValueListMetricsTest(BaseCheckValueTest, ABC):
+    alias: ClassVar[str]
     group = DATA_QUALITY_GROUP.id
     metric: ColumnValueListMetric
     column_name: str
     values: Optional[list]
 
     def __init__(
         self,
@@ -1316,74 +1162,59 @@
             not_in=not_in,
         )
         self.metric = ColumnValueListMetric(column_name=column_name, values=values)
 
     def groups(self) -> Dict[str, str]:
         return {GroupingTypes.ByFeature.id: self.column_name}
 
-
-class TestNumberOfOutListValues(BaseDataQualityValueListMetricsTest):
-    name = "Number Out-of-List Values"
-
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         return TestValueCondition(eq=approx(0))
 
+
+class TestNumberOfOutListValues(BaseDataQualityValueListMetricsTest):
+    name = "Number Out-of-List Values"
+    alias = "number_value_list"
+
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_not_in_list
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The number of values out of list in the column **{self.column_name}** is {value}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
-@default_renderer(wrap_type=TestNumberOfOutListValues)
-class TestNumberOfOutListValuesRenderer(TestRenderer):
-    def render_html(self, obj: TestNumberOfOutListValues) -> TestHtmlInfo:
-        info = super().render_html(obj)
-        metric_result = obj.metric.get_result()
-        column_name = metric_result.column_name
-        values = metric_result.values
-        curr_df = pd.DataFrame(metric_result.current.values_in_list.items(), columns=["x", "count"])
-
-        if metric_result.reference is not None:
-            ref_df = pd.DataFrame(metric_result.reference.values_in_list.items(), columns=["x", "count"])
-
-        else:
-            ref_df = None
-
-        additional_plots = plot_value_counts_tables(column_name, values, curr_df, ref_df, "number_value_list")
-        info.details = additional_plots
-        return info
+class ValueListParameters(CheckValueParameters):
+    # todo: typing
+    values: Optional[List[Any]] = None
 
 
 class TestShareOfOutListValues(BaseDataQualityValueListMetricsTest):
     name = "Share of Out-of-List Values"
-
-    def get_condition(self) -> TestValueCondition:
-        if self.condition.has_condition():
-            return self.condition
-        return TestValueCondition(eq=approx(0))
+    alias = "share_value_list"
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_not_in_list
 
     def get_description(self, value: Numeric) -> str:
         metric_result = self.metric.get_result()
         number_not_in_range = metric_result.current.number_not_in_list
         rows_count = metric_result.current.rows_count
         return (
             f"The share of values out of list in the column **{self.column_name}** is {value:.3g} "
             f"({number_not_in_range} out of {rows_count}). "
             f"The test threshold is {self.get_condition()}."
         )
 
+    def get_parameters(self) -> CheckValueParameters:
+        return ValueListParameters(condition=self.get_condition(), value=self.value, values=self.values)
+
 
 class TestCatColumnsOutOfListValues(BaseGenerator):
     """Create share of out of list values tests for category columns"""
 
     columns: Optional[List[str]]
 
     def __init__(self, columns: Optional[List[str]] = None):
@@ -1439,15 +1270,15 @@
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
 
         reference = self.metric.get_result().reference
 
         if reference is not None:
-            return TestValueCondition(eq=approx(reference.value, 0.1))
+            return TestValueCondition(eq=approx(reference.value, 0.1), source=ValueSource.REFERENCE)
 
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.value
 
     def get_description(self, value: Numeric) -> str:
@@ -1477,31 +1308,26 @@
             f"current {column_name} {metric_result.quantile} quantile",
         )
         info.with_details("", plotly_figure(title="", figure=fig))
         return info
 
 
 @default_renderer(wrap_type=TestShareOfOutListValues)
-class TestShareOfOutListValuesRenderer(TestRenderer):
-    def render_json(self, obj: TestShareOfOutListValues) -> dict:
-        base = super().render_json(obj)
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["values"] = obj.values
-        base["parameters"]["share_not_in_list"] = obj.value
-        return base
-
-    def render_html(self, obj: TestShareOfOutListValues) -> TestHtmlInfo:
+@default_renderer(wrap_type=TestNumberOfOutListValues)
+@default_renderer(wrap_type=TestValueList)
+class TestListValuesRenderer(TestRenderer):
+    def render_html(self, obj: Union[BaseDataQualityValueListMetricsTest, TestValueList]) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         column_name = metric_result.column_name
         values = metric_result.values
         curr_df = pd.DataFrame(metric_result.current.values_in_list.items(), columns=["x", "count"])
 
         if metric_result.reference is not None:
             ref_df = pd.DataFrame(metric_result.reference.values_in_list.items(), columns=["x", "count"])
 
         else:
             ref_df = None
 
-        additional_plots = plot_value_counts_tables(column_name, values, curr_df, ref_df, "share_value_list")
+        additional_plots = plot_value_counts_tables(column_name, values, curr_df, ref_df, obj.alias)
         info.details = additional_plots
         return info
```

### Comparing `evidently-0.2.8/src/evidently/tests/regression_performance_tests.py` & `evidently-0.3.0/src/evidently/tests/regression_performance_tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -71,24 +71,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The MAE is {value:.3}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestValueMAE)
 class TestValueMAERenderer(TestRenderer):
-    def render_json(self, obj: TestValueMAE) -> dict:
-        base = super().render_json(obj)
-        metric_result = obj.metric.get_result()
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["mean_abs_error"] = metric_result.current.mean_abs_error
-        base["parameters"]["mean_abs_error_ref"] = (
-            metric_result.reference.mean_abs_error if metric_result.reference is not None else None
-        )
-        return base
-
     def render_html(self, obj: TestValueMAE) -> TestHtmlInfo:
         info = super().render_html(obj)
         result = obj.metric.get_result()
         fig = regression_perf_plot(
             val_for_plot=result.vals_for_plots.mean_abs_error,
             hist_for_plot=result.hist_for_plot,
             name="MAE",
@@ -117,25 +107,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The MAPE is {value:.3}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestValueMAPE)
 class TestValueMAPERenderer(TestRenderer):
-    def render_json(self, obj: TestValueMAPE) -> dict:
-        base = super().render_json(obj)
-        metric_result = obj.metric.get_result()
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["mean_abs_perc_error"] = metric_result.current.mean_abs_perc_error
-        base["parameters"]["mean_abs_perc_error_ref"] = (
-            metric_result.reference.mean_abs_perc_error if metric_result.reference is not None else None
-        )
-        base["parameters"]["mean_abs_perc_error_default"] = metric_result.mean_abs_perc_error_default
-        return base
-
     def render_html(self, obj: TestValueMAPE) -> TestHtmlInfo:
         info = super().render_html(obj)
         result = obj.metric.get_result()
         val_for_plot = result.vals_for_plots.mean_abs_perc_error
         val_for_plot = val_for_plot * 100
         fig = regression_perf_plot(
             val_for_plot=val_for_plot,
@@ -166,23 +145,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The RMSE is {value:.3}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestValueRMSE)
 class TestValueRMSERenderer(TestRenderer):
-    def render_json(self, obj: TestValueRMSE) -> dict:
-        base = super().render_json(obj)
-        metric_result = obj.metric.get_result()
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["rmse"] = metric_result.current.rmse
-        base["parameters"]["rmse_ref"] = metric_result.reference.rmse if metric_result.reference is not None else None
-        base["parameters"]["rmse_default"] = metric_result.rmse_default if metric_result.reference is not None else None
-        return base
-
     def render_html(self, obj: TestValueRMSE) -> TestHtmlInfo:
         info = super().render_html(obj)
         result = obj.metric.get_result()
         fig = regression_perf_plot(
             val_for_plot=result.vals_for_plots.rmse,
             hist_for_plot=result.hist_for_plot,
             name="RMSE",
@@ -207,21 +177,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The ME is {value:.3}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestValueMeanError)
 class TestValueMeanErrorRenderer(TestRenderer):
-    def render_json(self, obj: TestValueMeanError) -> dict:
-        base = super().render_json(obj)
-        metric_result = obj.metric.get_result()
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["mean_error"] = metric_result.current.mean_error
-        return base
-
     def render_html(self, obj: TestValueMeanError) -> TestHtmlInfo:
         info = super().render_html(obj)
         metric_result = obj.metric.get_result()
         me_hist_for_plot = metric_result.me_hist_for_plot
         hist_curr = me_hist_for_plot.current
         hist_ref = me_hist_for_plot.reference
 
@@ -249,27 +212,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The Max Absolute Error is {value:.3}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestValueAbsMaxError)
 class TestValueAbsMaxErrorRenderer(TestRenderer):
-    def render_json(self, obj: TestValueAbsMaxError) -> dict:
-        base = super().render_json(obj)
-        metric_result = obj.metric.get_result()
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["abs_error_max"] = metric_result.current.abs_error_max
-        base["parameters"]["abs_error_max_ref"] = (
-            metric_result.reference.abs_error_max if metric_result.reference is not None else None
-        )
-        base["parameters"]["abs_error_max_ref"] = (
-            metric_result.abs_error_max_default if metric_result.reference is not None else None
-        )
-        return base
-
     def render_html(self, obj: TestValueAbsMaxError) -> TestHtmlInfo:
         info = super().render_html(obj)
         me_hist_for_plot = obj.metric.get_result().me_hist_for_plot
         hist_curr = me_hist_for_plot.current
         hist_ref = me_hist_for_plot.reference
 
         fig = plot_distr(hist_curr=hist_curr, hist_ref=hist_ref, color_options=self.color_options)
@@ -294,25 +244,14 @@
 
     def get_description(self, value: Numeric) -> str:
         return f"The R2 score is {value:.3}. The test threshold is {self.get_condition()}."
 
 
 @default_renderer(wrap_type=TestValueR2Score)
 class TestValueR2ScoreRenderer(TestRenderer):
-    def render_json(self, obj: TestValueAbsMaxError) -> dict:
-        base = super().render_json(obj)
-        metric_result = obj.metric.get_result()
-        base["parameters"]["condition"] = obj.get_condition().as_dict()
-        base["parameters"]["r2_score"] = metric_result.current.r2_score
-        # todo will be removed with tests json render logic
-        base["parameters"]["r2_score_ref"] = (
-            metric_result.reference.r2_score if metric_result.reference is not None else None
-        )
-        return base
-
     def render_html(self, obj: TestValueR2Score) -> TestHtmlInfo:
         info = super().render_html(obj)
         result = obj.metric.get_result()
 
         fig = regression_perf_plot(
             val_for_plot=result.vals_for_plots.r2_score,
             hist_for_plot=result.hist_for_plot,
```

### Comparing `evidently-0.2.8/src/evidently/utils/dashboard.py` & `evidently-0.3.0/src/evidently/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/utils/data_drift_utils.py` & `evidently-0.3.0/src/evidently/utils/data_drift_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/utils/data_operations.py` & `evidently-0.3.0/src/evidently/utils/data_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
                 - utility_columns_set
                 - cat_feature_names_set
                 - text_feature_names_set
             )
         )
 
     else:
+        num_feature_names = [col for col in num_feature_names if col in dataset.columns]
         empty_cols = dataset[num_feature_names].isnull().mean()
         empty_cols = empty_cols[empty_cols == 1.0].index
         num_feature_names = sorted(
             list(set(dataset[num_feature_names].select_dtypes([np.number]).columns).union(set(empty_cols)))
         )
 
     if datetime_feature_names is None:
```

### Comparing `evidently-0.2.8/src/evidently/utils/data_preprocessing.py` & `evidently-0.3.0/src/evidently/utils/data_preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import logging
 from enum import Enum
+from typing import Collection
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Union
 
 import numpy as np
@@ -67,35 +68,38 @@
 @dataclasses.dataclass
 class DataDefinition:
     _columns: Dict[str, ColumnDefinition]
     _target: Optional[ColumnDefinition]
     _prediction_columns: Optional[PredictionColumns]
     _id_column: Optional[ColumnDefinition]
     _datetime_column: Optional[ColumnDefinition]
+    _embeddings: Optional[Dict[str, List[str]]]
 
     _task: Optional[str]
     _classification_labels: Optional[TargetNames]
 
     def __init__(
         self,
         columns: List[ColumnDefinition],
         target: Optional[ColumnDefinition],
         prediction_columns: Optional[PredictionColumns],
         id_column: Optional[ColumnDefinition],
         datetime_column: Optional[ColumnDefinition],
+        embeddings: Optional[Dict[str, List[str]]],
         task: Optional[str],
         classification_labels: Optional[TargetNames],
     ):
         self._columns = {column.column_name: column for column in columns}
         self._id_column = id_column
         self._datetime_column = datetime_column
         self._task = task
         self._target = target
         self._prediction_columns = prediction_columns
         self._classification_labels = classification_labels
+        self._embeddings = embeddings
 
     def get_column(self, column_name: str) -> ColumnDefinition:
         return self._columns[column_name]
 
     def get_columns(self, filter_def: str = "all") -> List[ColumnDefinition]:
         if self._prediction_columns is not None:
             prediction = self._prediction_columns.get_columns_list()
@@ -127,14 +131,17 @@
 
     def task(self) -> Optional[str]:
         return self._task
 
     def classification_labels(self) -> Optional[TargetNames]:
         return self._classification_labels
 
+    def embeddings(self) -> Optional[Dict]:
+        return self._embeddings
+
 
 def _process_column(
     column_name: Optional[str],
     data: _InputData,
     if_partially_present: str = "raise",
     predefined_type: Optional[ColumnType] = None,
     mapping: Optional[ColumnMapping] = None,
@@ -199,26 +206,84 @@
     raise ValueError("Unexpected type for prediction field in column_mapping")
 
 
 def _filter_by_type(column: Optional[ColumnDefinition], column_type: ColumnType, exclude: List[str]) -> bool:
     return column is not None and column.column_type == column_type and column.column_name not in exclude
 
 
+def _column_not_present_in_list(
+    column: Optional[str],
+    columns: Collection[str],
+    handle_error: str,
+    message: str,
+) -> Optional[str]:
+    if column is None:
+        return None
+    if column not in columns:
+        return column
+    if handle_error == "error":
+        raise ValueError(message.format(column=column))
+    if handle_error == "warning":
+        logging.warning(message.format(column=column))
+        return None
+    if handle_error == "skip":
+        return None
+    raise ValueError(f"Unknown handle error type {handle_error}")
+
+
 def create_data_definition(
     reference_data: Optional[pd.DataFrame], current_data: pd.DataFrame, mapping: ColumnMapping
 ) -> DataDefinition:
     data = _InputData(reference_data, current_data)
-    id_column = _process_column(mapping.id, data)
-    target_column = _process_column(mapping.target, data, mapping=mapping)
-    datetime_column = _process_column(mapping.datetime, data)
+    embedding_columns = set()
+    embeddings: Optional[Dict[str, List[str]]] = None
+    if mapping.embeddings is not None:
+        embeddings = dict()
+        for (embedding_name, columns) in mapping.embeddings.items():
+            embeddings[embedding_name] = []
+            for column in columns:
+                presence = _get_column_presence(column, data)
+                if presence != ColumnPresenceState.Present:
+                    logging.warning(f"Column {column} isn't present in data. Skipping it.")
+                else:
+                    embeddings[embedding_name].append(column)
+                    embedding_columns.add(column)
+
+    id_column = _process_column(
+        _column_not_present_in_list(
+            mapping.id,
+            embedding_columns,
+            "warning",
+            "Column {column} is in embeddings list and as an ID field. Ignoring ID field.",
+        ),
+        data,
+    )
+    target_column = _process_column(
+        _column_not_present_in_list(
+            mapping.target,
+            embedding_columns,
+            "warning",
+            "Column {column} is in embeddings list and as a target field. Ignoring target field.",
+        ),
+        data,
+        mapping=mapping,
+    )
+    datetime_column = _process_column(
+        _column_not_present_in_list(
+            mapping.datetime,
+            embedding_columns,
+            "warning",
+            "Column {column} is in embeddings list and as a datetime field. Ignoring datetime field.",
+        ),
+        data,
+    )
 
     prediction_columns = _prediction_column(
         mapping.prediction,
         target_column.column_type if target_column is not None else None,
-        # mapping.target_names,
         mapping.task,
         data,
         mapping,
     )
 
     prediction_cols = prediction_columns.get_columns_list() if prediction_columns is not None else []
 
@@ -231,70 +296,116 @@
     utility_column_names = [column.column_name for column in all_columns if column is not None]
     data_columns = set(data.current.columns) | (set(data.reference.columns) if data.reference is not None else set())
     col_defs = [
         _process_column(column_name, data, if_partially_present="skip", mapping=mapping) for column_name in data_columns
     ]
 
     if mapping.numerical_features is None:
-        num = [column for column in col_defs if _filter_by_type(column, ColumnType.Numerical, utility_column_names)]
+        num = [
+            column
+            for column in col_defs
+            if column is not None
+            and _filter_by_type(column, ColumnType.Numerical, utility_column_names)
+            and _column_not_present_in_list(column.column_name, embedding_columns, "skip", "")
+        ]
         all_columns.extend(num)
     else:
         all_columns.extend(
             [
                 _process_column(
                     column_name,
                     data,
                     predefined_type=ColumnType.Numerical,
                     mapping=mapping,
                 )
                 for column_name in mapping.numerical_features
                 if column_name not in utility_column_names
+                and _column_not_present_in_list(
+                    column_name,
+                    embedding_columns,
+                    "warning",
+                    "Column {column} is in embedding list and in numerical features list."
+                    " Ignoring it in a features list.",
+                )
             ]
         )
 
     if mapping.categorical_features is None:
-        cat = [column for column in col_defs if _filter_by_type(column, ColumnType.Categorical, utility_column_names)]
+        cat = [
+            column
+            for column in col_defs
+            if column is not None
+            and _filter_by_type(column, ColumnType.Categorical, utility_column_names)
+            and _column_not_present_in_list(column.column_name, embedding_columns, "skip", "")
+        ]
         all_columns.extend(cat)
     else:
         all_columns.extend(
             [
                 _process_column(
                     column_name,
                     data,
                     predefined_type=ColumnType.Categorical,
                     mapping=mapping,
                 )
                 for column_name in mapping.categorical_features
                 if column_name not in utility_column_names
+                and _column_not_present_in_list(
+                    column_name,
+                    embedding_columns,
+                    "warning",
+                    "Column {column} is in embedding list and in categorical features list."
+                    " Ignoring it in a features list.",
+                )
             ]
         )
 
     if mapping.datetime_features is None:
-        dt = [column for column in col_defs if _filter_by_type(column, ColumnType.Datetime, utility_column_names)]
+        dt = [
+            column
+            for column in col_defs
+            if column is not None
+            and _filter_by_type(column, ColumnType.Datetime, utility_column_names)
+            and _column_not_present_in_list(column.column_name, embedding_columns, "skip", "")
+        ]
         all_columns.extend(dt)
     else:
         all_columns.extend(
             [
                 _process_column(
                     column_name,
                     data,
                     predefined_type=ColumnType.Datetime,
                     mapping=mapping,
                 )
                 for column_name in mapping.datetime_features
                 if column_name not in utility_column_names
+                and _column_not_present_in_list(
+                    column_name,
+                    embedding_columns,
+                    "warning",
+                    "Column {column} is in embedding list and in datetime features list."
+                    " Ignoring it in a features list.",
+                )
             ]
         )
 
     if mapping.text_features is not None:
         all_columns.extend(
             [
                 _process_column(column_name, data, predefined_type=ColumnType.Text, mapping=mapping)
                 for column_name in mapping.text_features
                 if column_name not in utility_column_names
+                and _column_not_present_in_list(
+                    column_name,
+                    embedding_columns,
+                    "warning",
+                    "Column {column} is in embedding list and in text features list."
+                    " Ignoring it in a features list.",
+                )
             ]
         )
     task = mapping.task
     if task is None:
         if target_column is None:
             task = None
         elif target_column.column_type == ColumnType.Categorical:
@@ -308,14 +419,15 @@
         columns=[col for col in all_columns if col is not None],
         id_column=id_column,
         datetime_column=datetime_column,
         target=target_column,
         prediction_columns=prediction_columns,
         task=task,
         classification_labels=mapping.target_names,
+        embeddings=embeddings,
     )
 
 
 class ColumnPresenceState(Enum):
     Present = 0
     Partially = 1
     Missing = 2
```

### Comparing `evidently-0.2.8/src/evidently/utils/generators.py` & `evidently-0.3.0/src/evidently/utils/generators.py`

 * *Files identical despite different names*

### Comparing `evidently-0.2.8/src/evidently/utils/types.py` & `evidently-0.3.0/src/evidently/utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,7 +72,10 @@
         if self._relative is not None:
             result["relative"] = self._relative
 
         if self._absolute is not None:
             result["absolute"] = self._absolute
 
         return result
+
+
+NumericApprox = Union[int, float, ApproxValue]
```

### Comparing `evidently-0.2.8/src/evidently/utils/visualizations.py` & `evidently-0.3.0/src/evidently/utils/visualizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from plotly import graph_objs as go
 from plotly.subplots import make_subplots
+from scipy import stats
 
 from evidently.metric_results import Distribution
 from evidently.metric_results import Histogram
 from evidently.metric_results import HistogramData
 from evidently.metric_results import Label
 from evidently.metric_results import ScatterData
 from evidently.options.color_scheme import ColorOptions
@@ -740,7 +741,58 @@
             text=np.array(ref_mtrx.values).astype(str),
             texttemplate="%{text}",
             coloraxis="coloraxis",
         )
         fig.add_trace(trace, 1, 2)
     fig.update_layout(coloraxis={"colorscale": "RdBu_r"})
     return fig
+
+
+def get_gaussian_kde(m1, m2):
+    def border(x):
+        return int(max(2, abs(x) * 0.2))
+
+    xmin = m1.min()
+    xmax = m1.max()
+    ymin = m2.min()
+    ymax = m2.max()
+    X, Y = np.mgrid[xmin - border(xmin) : xmax + border(xmax) : 30j, ymin - border(ymin) : ymax + border(ymax) : 30j]
+    positions = np.vstack([X.ravel(), Y.ravel()])
+    values = np.vstack([m1, m2])
+    kernel = stats.gaussian_kde(values)
+    Z = np.reshape(kernel(positions).T, X.shape)
+    return Z
+
+
+def plot_contour(z1: np.ndarray, z2: Optional[np.ndarray], xtitle: str = "", ytitle: str = ""):
+    color_options = ColorOptions()
+    if z2 is not None:
+        cols = 2
+        subplot_titles = ["current", "reference"]
+    else:
+        cols = 1
+        subplot_titles = [""]
+    fig = make_subplots(rows=1, cols=cols, shared_yaxes=True, subplot_titles=subplot_titles)
+    trace = go.Contour(
+        z=z1,
+        line_width=1,
+        name="current",
+        showscale=False,
+        showlegend=True,
+        colorscale=[[0, "white"], [1, color_options.get_current_data_color()]],
+    )
+    fig.add_trace(trace, 1, 1)
+    fig.update_xaxes(title_text=xtitle, row=1, col=1)
+
+    if z2 is not None:
+        trace = go.Contour(
+            z=z2,
+            line_width=1,
+            name="reference",
+            showscale=False,
+            showlegend=True,
+            colorscale=[[0, "white"], [1, color_options.get_reference_data_color()]],
+        )
+        fig.add_trace(trace, 1, 2)
+        fig.update_xaxes(title_text=xtitle, row=1, col=2)
+    fig.update_layout(yaxis_title=ytitle)
+    return fig
```

