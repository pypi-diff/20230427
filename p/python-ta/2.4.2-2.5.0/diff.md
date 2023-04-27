# Comparing `tmp/python-ta-2.4.2.tar.gz` & `tmp/python-ta-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ta-2.4.2.tar", last modified: Tue Jan 31 19:11:12 2023, max compression
+gzip compressed data, was "python-ta-2.5.0.tar", last modified: Thu Apr 27 15:29:43 2023, max compression
```

## Comparing `python-ta-2.4.2.tar` & `python-ta-2.5.0.tar`

### file list

```diff
@@ -1,146 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.607924 python-ta-2.4.2/
--rw-rw-rw-   0        0        0    35141 2020-09-24 17:22:04.000000 python-ta-2.4.2/LICENSE
--rw-rw-rw-   0        0        0      178 2022-04-18 16:52:09.000000 python-ta-2.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3457 2023-01-31 19:11:12.607924 python-ta-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3004 2023-01-30 20:58:29.000000 python-ta-2.4.2/README.md
--rw-rw-rw-   0        0        0      404 2021-08-24 20:57:44.000000 python-ta-2.4.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.355983 python-ta-2.4.2/python_ta/
--rw-rw-rw-   0        0        0    17054 2023-01-31 18:39:07.000000 python-ta-2.4.2/python_ta/__init__.py
--rw-rw-rw-   0        0        0     2322 2022-01-27 00:26:16.000000 python-ta-2.4.2/python_ta/__main__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.387980 python-ta-2.4.2/python_ta/cfg/
--rw-rw-rw-   0        0        0       44 2020-09-24 17:22:04.000000 python-ta-2.4.2/python_ta/cfg/__init__.py
--rw-rw-rw-   0        0        0     6530 2021-08-17 17:13:02.000000 python-ta-2.4.2/python_ta/cfg/graph.py
--rw-rw-rw-   0        0        0     9111 2021-08-23 01:35:55.000000 python-ta-2.4.2/python_ta/cfg/visitor.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.407987 python-ta-2.4.2/python_ta/checkers/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.4.2/python_ta/checkers/__init__.py
--rw-rw-rw-   0        0        0     2907 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/forbidden_import_checker.py
--rw-rw-rw-   0        0        0     2873 2022-10-14 01:27:28.000000 python-ta-2.4.2/python_ta/checkers/forbidden_io_function_checker.py
--rw-rw-rw-   0        0        0     3572 2022-10-14 01:27:28.000000 python-ta-2.4.2/python_ta/checkers/global_variables_checker.py
--rw-rw-rw-   0        0        0     1635 2022-11-27 20:47:51.000000 python-ta-2.4.2/python_ta/checkers/invalid_for_target_checker.py
--rw-rw-rw-   0        0        0     2354 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/invalid_range_index_checker.py
--rw-rw-rw-   0        0        0     2480 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/missing_space_in_doctest_checker.py
--rw-rw-rw-   0        0        0     2507 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/one_iteration_checker.py
--rw-rw-rw-   0        0        0     6237 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/possibly_undefined_checker.py
--rw-rw-rw-   0        0        0     1420 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/pycodestyle_checker.py
--rw-rw-rw-   0        0        0     5722 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/redundant_assignment_checker.py
--rw-rw-rw-   0        0        0     1412 2023-01-30 20:43:19.000000 python-ta-2.4.2/python_ta/checkers/shadowing_in_comprehension_checker.py
--rw-rw-rw-   0        0        0     2627 2022-12-12 02:59:49.000000 python-ta-2.4.2/python_ta/checkers/top_level_code_checker.py
--rw-rw-rw-   0        0        0     3778 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/type_annotation_checker.py
--rw-rw-rw-   0        0        0     1250 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/checkers/type_inference_checker.py
--rw-rw-rw-   0        0        0     6273 2022-10-24 01:36:54.000000 python-ta-2.4.2/python_ta/checkers/unnecessary_indexing_checker.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.407987 python-ta-2.4.2/python_ta/config/
--rw-rw-rw-   0        0        0     4159 2022-12-07 20:53:21.000000 python-ta-2.4.2/python_ta/config/.pylintrc
--rw-rw-rw-   0        0        0    14352 2023-01-30 20:43:19.000000 python-ta-2.4.2/python_ta/config/messages_config.toml
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.411980 python-ta-2.4.2/python_ta/contracts/
--rw-rw-rw-   0        0        0    22633 2023-01-31 18:38:30.000000 python-ta-2.4.2/python_ta/contracts/__init__.py
--rw-rw-rw-   0        0        0     3563 2021-11-06 03:28:14.000000 python-ta-2.4.2/python_ta/contracts/__main__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.411980 python-ta-2.4.2/python_ta/debug/
--rw-rw-rw-   0        0        0       50 2022-08-07 18:08:41.000000 python-ta-2.4.2/python_ta/debug/__init__.py
--rw-rw-rw-   0        0        0     6541 2022-12-12 02:59:49.000000 python-ta-2.4.2/python_ta/debug/accumulation_table.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.420225 python-ta-2.4.2/python_ta/patches/
--rw-rw-rw-   0        0        0      410 2022-12-07 17:07:10.000000 python-ta-2.4.2/python_ta/patches/__init__.py
--rw-rw-rw-   0        0        0     3921 2022-10-14 01:27:28.000000 python-ta-2.4.2/python_ta/patches/checkers.py
--rw-rw-rw-   0        0        0      933 2022-04-18 16:52:09.000000 python-ta-2.4.2/python_ta/patches/error_messages.py
--rw-rw-rw-   0        0        0      895 2022-06-30 13:49:27.000000 python-ta-2.4.2/python_ta/patches/messages.py
--rw-rw-rw-   0        0        0      864 2022-12-07 20:53:21.000000 python-ta-2.4.2/python_ta/patches/transforms.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.428235 python-ta-2.4.2/python_ta/reporters/
--rw-rw-rw-   0        0        0      296 2021-08-17 17:13:02.000000 python-ta-2.4.2/python_ta/reporters/__init__.py
--rw-rw-rw-   0        0        0     1937 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/reporters/color_reporter.py
--rw-rw-rw-   0        0        0    10213 2022-09-05 23:10:07.000000 python-ta-2.4.2/python_ta/reporters/core.py
--rw-rw-rw-   0        0        0     5864 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/reporters/html_reporter.py
--rw-rw-rw-   0        0        0     1156 2022-09-05 23:10:07.000000 python-ta-2.4.2/python_ta/reporters/json_reporter.py
--rw-rw-rw-   0        0        0     5368 2022-06-30 12:34:36.000000 python-ta-2.4.2/python_ta/reporters/node_printers.py
--rw-rw-rw-   0        0        0     3028 2022-07-07 23:34:28.000000 python-ta-2.4.2/python_ta/reporters/plain_reporter.py
--rw-rw-rw-   0        0        0      824 2021-08-17 17:13:02.000000 python-ta-2.4.2/python_ta/reporters/stat_reporter.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.485709 python-ta-2.4.2/python_ta/reporters/templates/
--rw-rw-rw-   0        0        0   160658 2023-01-09 17:16:14.000000 python-ta-2.4.2/python_ta/reporters/templates/jquery-3.2.1.min.js
--rw-rw-rw-   0        0        0    13773 2020-09-24 17:22:04.000000 python-ta-2.4.2/python_ta/reporters/templates/pyta_logo_markdown.png
--rw-rw-rw-   0        0        0     1435 2021-08-17 17:13:02.000000 python-ta-2.4.2/python_ta/reporters/templates/script.js
--rw-rw-rw-   0        0        0     9635 2021-08-23 23:35:24.000000 python-ta-2.4.2/python_ta/reporters/templates/stylesheet.css
--rw-rw-rw-   0        0        0    16873 2021-12-04 00:01:01.000000 python-ta-2.4.2/python_ta/reporters/templates/template.html.jinja
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.497708 python-ta-2.4.2/python_ta/transforms/
--rw-rw-rw-   0        0        0     5298 2022-08-24 00:15:57.000000 python-ta-2.4.2/python_ta/transforms/ExprWrapper.py
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.4.2/python_ta/transforms/__init__.py
--rw-rw-rw-   0        0        0    24351 2022-12-07 20:53:21.000000 python-ta-2.4.2/python_ta/transforms/setendings.py
--rw-rw-rw-   0        0        0    43708 2021-08-23 01:35:55.000000 python-ta-2.4.2/python_ta/transforms/type_inference_visitor.py
--rw-rw-rw-   0        0        0     1999 2022-08-24 00:15:57.000000 python-ta-2.4.2/python_ta/transforms/z3_visitor.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.505710 python-ta-2.4.2/python_ta/typecheck/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.4.2/python_ta/typecheck/__init__.py
--rw-rw-rw-   0        0        0    40815 2021-08-23 01:35:55.000000 python-ta-2.4.2/python_ta/typecheck/base.py
--rw-rw-rw-   0        0        0     6635 2021-08-23 01:35:55.000000 python-ta-2.4.2/python_ta/typecheck/errors.py
--rw-rw-rw-   0        0        0     7147 2021-08-23 01:35:55.000000 python-ta-2.4.2/python_ta/typecheck/type_store.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.509710 python-ta-2.4.2/python_ta/typecheck/typeshed/
--rw-rw-rw-   0        0        0     1453 2021-08-17 17:13:02.000000 python-ta-2.4.2/python_ta/typecheck/typeshed/README.md
--rw-rw-rw-   0        0        0    70480 2022-04-07 16:59:30.000000 python-ta-2.4.2/python_ta/typecheck/typeshed/builtins.pyi
--rw-rw-rw-   0        0        0     3829 2021-08-17 17:13:02.000000 python-ta-2.4.2/python_ta/upload.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.513716 python-ta-2.4.2/python_ta/util/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.4.2/python_ta/util/__init__.py
--rw-rw-rw-   0        0        0     1078 2021-08-17 17:13:02.000000 python-ta-2.4.2/python_ta/util/monad.py
--rw-rw-rw-   0        0        0     1257 2022-10-14 01:27:28.000000 python-ta-2.4.2/python_ta/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.384042 python-ta-2.4.2/python_ta.egg-info/
--rw-rw-rw-   0        0        0     3457 2023-01-31 19:11:12.000000 python-ta-2.4.2/python_ta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4538 2023-01-31 19:11:12.000000 python-ta-2.4.2/python_ta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 19:11:12.000000 python-ta-2.4.2/python_ta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-01-31 19:11:12.000000 python-ta-2.4.2/python_ta.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-09-26 00:08:53.000000 python-ta-2.4.2/python_ta.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      267 2023-01-31 19:11:12.000000 python-ta-2.4.2/python_ta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-01-31 19:11:12.000000 python-ta-2.4.2/python_ta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.529719 python-ta-2.4.2/sample_usage/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.4.2/sample_usage/__init__.py
--rw-rw-rw-   0        0        0     2154 2021-08-23 01:35:55.000000 python-ta-2.4.2/sample_usage/draw_cfg.py
--rw-rw-rw-   0        0        0     3299 2021-08-23 01:35:55.000000 python-ta-2.4.2/sample_usage/draw_tnodes.py
--rw-rw-rw-   0        0        0     1547 2021-08-17 17:13:02.000000 python-ta-2.4.2/sample_usage/print_ast.py
--rw-rw-rw-   0        0        0     3092 2021-08-17 17:13:02.000000 python-ta-2.4.2/sample_usage/print_nodes.py
--rw-rw-rw-   0        0        0     2074 2022-08-08 17:55:51.000000 python-ta-2.4.2/sample_usage/print_table.py
--rw-rw-rw-   0        0        0     5758 2021-08-17 17:13:02.000000 python-ta-2.4.2/sample_usage/pyta_stats.py
--rw-rw-rw-   0        0        0     5538 2021-08-17 17:13:02.000000 python-ta-2.4.2/sample_usage/stats_analysis.py
--rw-rw-rw-   0        0        0      924 2023-01-31 19:11:12.615968 python-ta-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0       38 2021-08-24 20:57:44.000000 python-ta-2.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.546445 python-ta-2.4.2/tests/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.4.2/tests/__init__.py
--rw-rw-rw-   0        0        0    11609 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/custom_hypothesis_support.py
--rw-rw-rw-   0        0        0     7213 2023-01-30 20:43:19.000000 python-ta-2.4.2/tests/test_check.py
--rw-rw-rw-   0        0        0    11322 2022-12-09 22:37:04.000000 python-ta-2.4.2/tests/test_class_contracts.py
--rw-rw-rw-   0        0        0    19381 2023-01-31 18:38:30.000000 python-ta-2.4.2/tests/test_contracts.py
--rw-rw-rw-   0        0        0     4153 2023-01-28 01:41:43.000000 python-ta-2.4.2/tests/test_examples.py
--rw-rw-rw-   0        0        0    17767 2021-12-09 21:58:56.000000 python-ta-2.4.2/tests/test_setendings.py
--rw-rw-rw-   0        0        0     5330 2021-08-17 17:13:02.000000 python-ta-2.4.2/tests/test_subclass_contracts.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.550512 python-ta-2.4.2/tests/test_type_constraints/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.4.2/tests/test_type_constraints/__init__.py
--rw-rw-rw-   0        0        0    15992 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_constraints/test_tnode_structure.py
--rw-rw-rw-   0        0        0     6429 2021-08-17 17:13:02.000000 python-ta-2.4.2/tests/test_type_constraints/test_unify.py
-drwxrwxrwx   0        0        0        0 2023-01-31 19:11:12.607924 python-ta-2.4.2/tests/test_type_inference/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.4.2/tests/test_type_inference/__init__.py
--rw-rw-rw-   0        0        0     8416 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_annassign.py
--rw-rw-rw-   0        0        0    11246 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_assign.py
--rw-rw-rw-   0        0        0     4353 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_assign_tuple.py
--rw-rw-rw-   0        0        0     6670 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_attribute.py
--rw-rw-rw-   0        0        0     3912 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_binops.py
--rw-rw-rw-   0        0        0     1290 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_boolops.py
--rw-rw-rw-   0        0        0     4907 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_classdef.py
--rw-rw-rw-   0        0        0     3068 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_compare.py
--rw-rw-rw-   0        0        0      651 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_const.py
--rw-rw-rw-   0        0        0     2514 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_dict.py
--rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_dictcomp.py
--rw-rw-rw-   0        0        0     2486 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_errors.py
--rw-rw-rw-   0        0        0     5710 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_for.py
--rw-rw-rw-   0        0        0     5265 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_function_annotation.py
--rw-rw-rw-   0        0        0     8871 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_function_def_inference.py
--rw-rw-rw-   0        0        0     4905 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_function_overload.py
--rw-rw-rw-   0        0        0    21649 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_functions.py
--rw-rw-rw-   0        0        0      555 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_ifexpr.py
--rw-rw-rw-   0        0        0     3749 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_imports.py
--rw-rw-rw-   0        0        0     2142 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_initializer.py
--rw-rw-rw-   0        0        0     4382 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_lambda.py
--rw-rw-rw-   0        0        0     3763 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_list.py
--rw-rw-rw-   0        0        0     2093 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_listcomp.py
--rw-rw-rw-   0        0        0      856 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_literals.py
--rw-rw-rw-   0        0        0      641 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_name.py
--rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_set.py
--rw-rw-rw-   0        0        0     1935 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_setcomp.py
--rw-rw-rw-   0        0        0     5197 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_starred.py
--rw-rw-rw-   0        0        0     5718 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_subscript.py
--rw-rw-rw-   0        0        0      586 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_tuple.py
--rw-rw-rw-   0        0        0     4614 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_typefail_reason.py
--rw-rw-rw-   0        0        0     1090 2021-08-23 01:35:55.000000 python-ta-2.4.2/tests/test_type_inference/test_unaryops.py
--rw-rw-rw-   0        0        0     1444 2022-08-24 00:15:57.000000 python-ta-2.4.2/tests/test_z3_visitor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.890178 python-ta-2.5.0/
+-rw-rw-rw-   0        0        0    35141 2020-09-24 17:22:04.000000 python-ta-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0      178 2022-04-18 16:52:09.000000 python-ta-2.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3457 2023-04-27 15:29:43.890178 python-ta-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3004 2023-01-30 20:58:29.000000 python-ta-2.5.0/README.md
+-rw-rw-rw-   0        0        0      404 2021-08-24 20:57:44.000000 python-ta-2.5.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.759791 python-ta-2.5.0/python_ta/
+-rw-rw-rw-   0        0        0    17406 2023-04-27 15:28:54.000000 python-ta-2.5.0/python_ta/__init__.py
+-rw-rw-rw-   0        0        0     2322 2022-01-27 00:26:16.000000 python-ta-2.5.0/python_ta/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.825838 python-ta-2.5.0/python_ta/cfg/
+-rw-rw-rw-   0        0        0       44 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/cfg/__init__.py
+-rw-rw-rw-   0        0        0     6958 2023-04-08 02:58:51.000000 python-ta-2.5.0/python_ta/cfg/graph.py
+-rw-rw-rw-   0        0        0    13501 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/cfg/visitor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.885765 python-ta-2.5.0/python_ta/checkers/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/checkers/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/forbidden_import_checker.py
+-rw-rw-rw-   0        0        0     2872 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/forbidden_io_function_checker.py
+-rw-rw-rw-   0        0        0     1623 2023-03-22 15:35:32.000000 python-ta-2.5.0/python_ta/checkers/forbidden_python_syntax_checker.py
+-rw-rw-rw-   0        0        0     3571 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/global_variables_checker.py
+-rw-rw-rw-   0        0        0     1635 2022-11-27 20:47:51.000000 python-ta-2.5.0/python_ta/checkers/invalid_for_target_checker.py
+-rw-rw-rw-   0        0        0     2351 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/invalid_range_index_checker.py
+-rw-rw-rw-   0        0        0     2479 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/missing_space_in_doctest_checker.py
+-rw-rw-rw-   0        0        0     2506 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/one_iteration_checker.py
+-rw-rw-rw-   0        0        0     6312 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/possibly_undefined_checker.py
+-rw-rw-rw-   0        0        0     1419 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/pycodestyle_checker.py
+-rw-rw-rw-   0        0        0     5721 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/redundant_assignment_checker.py
+-rw-rw-rw-   0        0        0     1411 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/shadowing_in_comprehension_checker.py
+-rw-rw-rw-   0        0        0     2627 2022-12-12 02:59:49.000000 python-ta-2.5.0/python_ta/checkers/top_level_code_checker.py
+-rw-rw-rw-   0        0        0     3777 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/type_annotation_checker.py
+-rw-rw-rw-   0        0        0     1249 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/type_inference_checker.py
+-rw-rw-rw-   0        0        0     6273 2022-10-24 01:36:54.000000 python-ta-2.5.0/python_ta/checkers/unnecessary_indexing_checker.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.917094 python-ta-2.5.0/python_ta/config/
+-rw-rw-rw-   0        0        0     4159 2022-12-07 20:53:21.000000 python-ta-2.5.0/python_ta/config/.pylintrc
+-rw-rw-rw-   0        0        0    14352 2023-01-30 20:43:19.000000 python-ta-2.5.0/python_ta/config/messages_config.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.933160 python-ta-2.5.0/python_ta/contracts/
+-rw-rw-rw-   0        0        0    22633 2023-01-31 18:38:30.000000 python-ta-2.5.0/python_ta/contracts/__init__.py
+-rw-rw-rw-   0        0        0     3563 2021-11-06 03:28:14.000000 python-ta-2.5.0/python_ta/contracts/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.964470 python-ta-2.5.0/python_ta/debug/
+-rw-rw-rw-   0        0        0       50 2022-08-07 18:08:41.000000 python-ta-2.5.0/python_ta/debug/__init__.py
+-rw-rw-rw-   0        0        0     6541 2022-12-12 02:59:49.000000 python-ta-2.5.0/python_ta/debug/accumulation_table.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.011294 python-ta-2.5.0/python_ta/patches/
+-rw-rw-rw-   0        0        0      410 2022-12-07 17:07:10.000000 python-ta-2.5.0/python_ta/patches/__init__.py
+-rw-rw-rw-   0        0        0     3921 2022-10-14 01:27:28.000000 python-ta-2.5.0/python_ta/patches/checkers.py
+-rw-rw-rw-   0        0        0      933 2022-04-18 16:52:09.000000 python-ta-2.5.0/python_ta/patches/error_messages.py
+-rw-rw-rw-   0        0        0      895 2022-06-30 13:49:27.000000 python-ta-2.5.0/python_ta/patches/messages.py
+-rw-rw-rw-   0        0        0      864 2022-12-07 20:53:21.000000 python-ta-2.5.0/python_ta/patches/transforms.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.089856 python-ta-2.5.0/python_ta/reporters/
+-rw-rw-rw-   0        0        0      296 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/reporters/__init__.py
+-rw-rw-rw-   0        0        0     1937 2022-07-07 23:34:28.000000 python-ta-2.5.0/python_ta/reporters/color_reporter.py
+-rw-rw-rw-   0        0        0    10213 2022-09-05 23:10:07.000000 python-ta-2.5.0/python_ta/reporters/core.py
+-rw-rw-rw-   0        0        0     5864 2022-07-07 23:34:28.000000 python-ta-2.5.0/python_ta/reporters/html_reporter.py
+-rw-rw-rw-   0        0        0     1156 2022-09-05 23:10:07.000000 python-ta-2.5.0/python_ta/reporters/json_reporter.py
+-rw-rw-rw-   0        0        0     5368 2022-06-30 12:34:36.000000 python-ta-2.5.0/python_ta/reporters/node_printers.py
+-rw-rw-rw-   0        0        0     3028 2022-07-07 23:34:28.000000 python-ta-2.5.0/python_ta/reporters/plain_reporter.py
+-rw-rw-rw-   0        0        0      823 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/reporters/stat_reporter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.199376 python-ta-2.5.0/python_ta/reporters/templates/
+-rw-rw-rw-   0        0        0   160658 2023-01-09 17:16:14.000000 python-ta-2.5.0/python_ta/reporters/templates/jquery-3.2.1.min.js
+-rw-rw-rw-   0        0        0    13773 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/reporters/templates/pyta_logo_markdown.png
+-rw-rw-rw-   0        0        0     1435 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/reporters/templates/script.js
+-rw-rw-rw-   0        0        0     9635 2021-08-23 23:35:24.000000 python-ta-2.5.0/python_ta/reporters/templates/stylesheet.css
+-rw-rw-rw-   0        0        0    16873 2021-12-04 00:01:01.000000 python-ta-2.5.0/python_ta/reporters/templates/template.html.jinja
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.246824 python-ta-2.5.0/python_ta/transforms/
+-rw-rw-rw-   0        0        0     5298 2022-08-24 00:15:57.000000 python-ta-2.5.0/python_ta/transforms/ExprWrapper.py
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/transforms/__init__.py
+-rw-rw-rw-   0        0        0    24351 2023-03-22 15:29:31.000000 python-ta-2.5.0/python_ta/transforms/setendings.py
+-rw-rw-rw-   0        0        0    43708 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/transforms/type_inference_visitor.py
+-rw-rw-rw-   0        0        0     1999 2022-08-24 00:15:57.000000 python-ta-2.5.0/python_ta/transforms/z3_visitor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.293659 python-ta-2.5.0/python_ta/typecheck/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/typecheck/__init__.py
+-rw-rw-rw-   0        0        0    40815 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/typecheck/base.py
+-rw-rw-rw-   0        0        0     6635 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/typecheck/errors.py
+-rw-rw-rw-   0        0        0     7147 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/typecheck/type_store.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.309294 python-ta-2.5.0/python_ta/typecheck/typeshed/
+-rw-rw-rw-   0        0        0     1453 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/typecheck/typeshed/README.md
+-rw-rw-rw-   0        0        0    70480 2022-04-07 16:59:30.000000 python-ta-2.5.0/python_ta/typecheck/typeshed/builtins.pyi
+-rw-rw-rw-   0        0        0     3829 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/upload.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.327553 python-ta-2.5.0/python_ta/util/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/util/__init__.py
+-rw-rw-rw-   0        0        0     1078 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/util/monad.py
+-rw-rw-rw-   0        0        0     1257 2022-10-14 01:27:28.000000 python-ta-2.5.0/python_ta/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.790990 python-ta-2.5.0/python_ta.egg-info/
+-rw-rw-rw-   0        0        0     3457 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4592 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-09-26 00:08:53.000000 python-ta-2.5.0/python_ta.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      322 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.387583 python-ta-2.5.0/sample_usage/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/sample_usage/__init__.py
+-rw-rw-rw-   0        0        0     2512 2023-04-27 15:16:56.000000 python-ta-2.5.0/sample_usage/draw_cfg.py
+-rw-rw-rw-   0        0        0     3299 2021-08-23 01:35:55.000000 python-ta-2.5.0/sample_usage/draw_tnodes.py
+-rw-rw-rw-   0        0        0     1547 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/print_ast.py
+-rw-rw-rw-   0        0        0     3092 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/print_nodes.py
+-rw-rw-rw-   0        0        0     2074 2022-08-08 17:55:51.000000 python-ta-2.5.0/sample_usage/print_table.py
+-rw-rw-rw-   0        0        0     5758 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/pyta_stats.py
+-rw-rw-rw-   0        0        0     5538 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/stats_analysis.py
+-rw-rw-rw-   0        0        0      999 2023-04-27 15:29:43.905867 python-ta-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0       38 2021-08-24 20:57:44.000000 python-ta-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.497490 python-ta-2.5.0/tests/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    11609 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/custom_hypothesis_support.py
+-rw-rw-rw-   0        0        0     7213 2023-01-30 20:43:19.000000 python-ta-2.5.0/tests/test_check.py
+-rw-rw-rw-   0        0        0    11322 2022-12-09 22:37:04.000000 python-ta-2.5.0/tests/test_class_contracts.py
+-rw-rw-rw-   0        0        0    19381 2023-01-31 18:38:30.000000 python-ta-2.5.0/tests/test_contracts.py
+-rw-rw-rw-   0        0        0     4153 2023-01-28 01:41:43.000000 python-ta-2.5.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0    17767 2021-12-09 21:58:56.000000 python-ta-2.5.0/tests/test_setendings.py
+-rw-rw-rw-   0        0        0     5330 2021-08-17 17:13:02.000000 python-ta-2.5.0/tests/test_subclass_contracts.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.528117 python-ta-2.5.0/tests/test_type_constraints/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.5.0/tests/test_type_constraints/__init__.py
+-rw-rw-rw-   0        0        0    15992 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_constraints/test_tnode_structure.py
+-rw-rw-rw-   0        0        0     6429 2021-08-17 17:13:02.000000 python-ta-2.5.0/tests/test_type_constraints/test_unify.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.890178 python-ta-2.5.0/tests/test_type_inference/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.5.0/tests/test_type_inference/__init__.py
+-rw-rw-rw-   0        0        0     8416 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_annassign.py
+-rw-rw-rw-   0        0        0    11246 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_assign.py
+-rw-rw-rw-   0        0        0     4353 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_assign_tuple.py
+-rw-rw-rw-   0        0        0     6670 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_attribute.py
+-rw-rw-rw-   0        0        0     3912 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_binops.py
+-rw-rw-rw-   0        0        0     1290 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_boolops.py
+-rw-rw-rw-   0        0        0     4907 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_classdef.py
+-rw-rw-rw-   0        0        0     3068 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_compare.py
+-rw-rw-rw-   0        0        0      651 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_const.py
+-rw-rw-rw-   0        0        0     2514 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_dict.py
+-rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_dictcomp.py
+-rw-rw-rw-   0        0        0     2486 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_errors.py
+-rw-rw-rw-   0        0        0     5710 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_for.py
+-rw-rw-rw-   0        0        0     5265 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_function_annotation.py
+-rw-rw-rw-   0        0        0     8871 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_function_def_inference.py
+-rw-rw-rw-   0        0        0     4905 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_function_overload.py
+-rw-rw-rw-   0        0        0    21649 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_functions.py
+-rw-rw-rw-   0        0        0      555 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_ifexpr.py
+-rw-rw-rw-   0        0        0     3749 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_imports.py
+-rw-rw-rw-   0        0        0     2142 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_initializer.py
+-rw-rw-rw-   0        0        0     4382 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_lambda.py
+-rw-rw-rw-   0        0        0     3763 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_list.py
+-rw-rw-rw-   0        0        0     2093 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_listcomp.py
+-rw-rw-rw-   0        0        0      856 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_literals.py
+-rw-rw-rw-   0        0        0      641 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_name.py
+-rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_set.py
+-rw-rw-rw-   0        0        0     1935 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_setcomp.py
+-rw-rw-rw-   0        0        0     5197 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_starred.py
+-rw-rw-rw-   0        0        0     5718 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_subscript.py
+-rw-rw-rw-   0        0        0      586 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_tuple.py
+-rw-rw-rw-   0        0        0     4614 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_typefail_reason.py
+-rw-rw-rw-   0        0        0     1090 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_unaryops.py
+-rw-rw-rw-   0        0        0     1444 2022-08-24 00:15:57.000000 python-ta-2.5.0/tests/test_z3_visitor.py
```

### Comparing `python-ta-2.4.2/LICENSE` & `python-ta-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/PKG-INFO` & `python-ta-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ta
-Version: 2.4.2
+Version: 2.5.0
 Summary: Code checking tool for teaching Python
 Home-page: https://github.com/pyta-uoft/pyta
 Author: David Liu
 Author-email: david@cs.toronto.edu
 License: MIT
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `python-ta-2.4.2/README.md` & `python-ta-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/__init__.py` & `python-ta-2.5.0/python_ta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Or, put the following code in your Python module:
 
 if __name__ == '__main__':
     import python_ta
     python_ta.check_all()
 """
-__version__ = "2.4.2"  # Version number
+__version__ = "2.5.0"  # Version number
 
 # First, remove underscore from builtins if it has been bound in the REPL.
 import builtins
 
 from pylint.lint import PyLinter
 
 from .reporters.core import PythonTaReporter
@@ -105,21 +105,26 @@
     global PYLINT_PATCHED
     if not PYLINT_PATCHED:
         patch_all(messages_config)  # Monkeypatch pylint (override certain methods)
         PYLINT_PATCHED = True
 
     # Try to check file, issue error message for invalid files.
     try:
+        # Flag indicating whether at least one file has been checked
+        is_any_file_checked = False
+
         for locations in _get_valid_files_to_check(module_name):
             f_paths = []  # Paths to files for data submission
             errs = []  # Errors caught in files for data submission
             config = {}  # Configuration settings for data submission
             for file_py in get_file_paths(locations):
                 if not _verify_pre_check(file_py):
                     continue  # Check the other files
+                # The current file can actually be checked so update the flag
+                is_any_file_checked = True
                 # Load config file in user location. Construct new linter each
                 # time, so config options don't bleed to unintended files.
                 # Reuse the same reporter each time to accumulate the results across different files.
                 linter = reset_linter(config=local_config, file_linted=file_py)
                 linter.set_reporter(current_reporter)
                 module_name = os.path.splitext(os.path.basename(file_py))[0]
                 if module_name in MANAGER.astroid_cache:  # Remove module from astroid cache
@@ -151,15 +156,17 @@
                 upload_to_server(
                     errors=errs,
                     paths=f_paths,
                     config=config,
                     url=linter.config.pyta_server_address,
                     version=__version__,
                 )
-        linter.generate_reports()
+        # Only generate reports (display the webpage) if there were valid files to check
+        if is_any_file_checked:
+            linter.generate_reports()
         return current_reporter
     except Exception as e:
         print(
             "[ERROR] Unexpected error encountered! Please report this to your instructor (and attach the code that caused the error)."
         )
         print('[ERROR] Error message: "{}"'.format(e))
         raise e
```

### Comparing `python-ta-2.4.2/python_ta/__main__.py` & `python-ta-2.5.0/python_ta/__main__.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/cfg/graph.py` & `python-ta-2.5.0/python_ta/cfg/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from typing import Generator, List, Optional, Set, Tuple, Union
+from typing import Any, Generator, List, Optional, Set, Tuple, Union
 
-from astroid import Break, Continue, NodeNG, Return
+from astroid import Break, Continue, NodeNG, Raise, Return
 
 
 class ControlFlowGraph:
     """A graph representing the control flow of a Python program."""
 
     start: CFGBlock
     end: CFGBlock
@@ -17,54 +17,62 @@
 
     def __init__(self) -> None:
         self.block_count = 0
         self.unreachable_blocks = set()
         self.start = self.create_block()
         self.end = self.create_block()
 
-    def create_block(self, pred: Optional[CFGBlock] = None) -> CFGBlock:
+    def create_block(
+        self, pred: Optional[CFGBlock] = None, edge_label: Optional[Any] = None
+    ) -> CFGBlock:
         """Create a new CFGBlock for this graph.
 
         If pred is specified, set that block as a predecessor of the new block.
+
+        If edge_label is specified, set the corresponding edge in the CFG with that label.
         """
         new_block = CFGBlock(self.block_count)
         self.unreachable_blocks.add(new_block)
 
         self.block_count += 1
         if pred:
-            self.link_or_merge(pred, new_block)
+            self.link_or_merge(pred, new_block, edge_label)
         return new_block
 
     def link(self, source: CFGBlock, target: CFGBlock) -> None:
         """Link source to target."""
         if not source.is_jump():
             CFGEdge(source, target)
 
-    def link_or_merge(self, source: CFGBlock, target: CFGBlock) -> None:
+    def link_or_merge(
+        self, source: CFGBlock, target: CFGBlock, edge_label: Optional[Any] = None
+    ) -> None:
         """Link source to target, or merge source into target if source is empty.
 
         An "empty" node for this purpose is when source has no statements.
 
         source with a jump statement cannot be further linked or merged to
         another target.
+
+        If edge_label is specified, set the corresponding edge in the CFG with that label.
         """
         if source.is_jump():
             return
         if source.statements == []:
             if source is self.start:
                 self.start = target
             else:
                 for edge in source.predecessors:
                     edge.target = target
                     target.predecessors.append(edge)
             # source is a utility block that helps build the cfg that does not
             # represent any part of the program so it is redundant.
             self.unreachable_blocks.remove(source)
         else:
-            CFGEdge(source, target)
+            CFGEdge(source, target, edge_label)
 
     def multiple_link_or_merge(self, source: CFGBlock, targets: List[CFGBlock]) -> None:
         """Link source to multiple target, or merge source into targets if source is empty.
 
         An "empty" node for this purpose is when source has no statements.
 
         source with a jump statement cannot be further linked or merged to
@@ -168,24 +176,28 @@
     def jump(self) -> Optional[NodeNG]:
         if len(self.statements) > 0:
             return self.statements[-1]
 
     def is_jump(self) -> bool:
         """Returns True if the block has a statement that branches
         the control flow (ex: `break`)"""
-        return isinstance(self.jump, (Break, Continue, Return))
+        return isinstance(self.jump, (Break, Continue, Return, Raise))
 
 
 class CFGEdge:
     """An edge in a control flow graph.
 
     Edges are directed, and in the future may be augmented with auxiliary metadata about the control flow.
     """
 
     source: CFGBlock
     target: CFGBlock
+    label: Optional[Any]
 
-    def __init__(self, source: CFGBlock, target: CFGBlock) -> None:
+    def __init__(
+        self, source: CFGBlock, target: CFGBlock, edge_label: Optional[Any] = None
+    ) -> None:
         self.source = source
         self.target = target
+        self.label = edge_label
         self.source.successors.append(self)
         self.target.predecessors.append(self)
```

### Comparing `python-ta-2.4.2/python_ta/checkers/forbidden_import_checker.py` & `python-ta-2.5.0/python_ta/checkers/forbidden_import_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from astroid import nodes
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 
 class ForbiddenImportChecker(BaseChecker):
-
     name = "forbidden_import"
     msgs = {
         "E9999": (
             "You may not import any modules - you imported %s on line %s.",
             "forbidden-import",
             "Used when you use import",
         )
```

### Comparing `python-ta-2.4.2/python_ta/checkers/forbidden_io_function_checker.py` & `python-ta-2.5.0/python_ta/checkers/forbidden_io_function_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from python_ta.utils import _is_in_main
 
 FORBIDDEN_BUILTIN = ["input", "print", "open"]
 
 
 class IOFunctionChecker(BaseChecker):
-
     name = "IO_Function"
     msgs = {
         "E9998": (
             "Used input/output function %s",
             "forbidden-IO-function",
             'Used when you use the I/O functions "print", "open" or "input". These '
             "functions should not be used except where specified by your instructor.",
```

### Comparing `python-ta-2.4.2/python_ta/checkers/global_variables_checker.py` & `python-ta-2.5.0/python_ta/checkers/global_variables_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pylint.checkers import BaseChecker
 from pylint.checkers.base import UpperCaseStyle
 
 from python_ta.utils import _is_in_main
 
 
 class GlobalVariablesChecker(BaseChecker):
-
     name = "global_variables"
     msgs = {
         "E9997": (
             "Global variables must be constants in CSC108/CSC148: " "%s",
             "forbidden-global-variables",
             "",
         )
```

### Comparing `python-ta-2.4.2/python_ta/checkers/invalid_for_target_checker.py` & `python-ta-2.5.0/python_ta/checkers/invalid_for_target_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/checkers/invalid_range_index_checker.py` & `python-ta-2.5.0/python_ta/checkers/invalid_range_index_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from astroid import nodes
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 
 class InvalidRangeIndexChecker(BaseChecker):
-
     name = "invalid_range_index"
     msgs = {
         "E9993": (
             "You should not use invalid range index on line %s",
             "invalid-range-index",
             "Used when you use invalid index range",
         )
@@ -34,26 +33,24 @@
                 # check if there is no args in 'range' call
                 if (
                     len(arg) == 0
                     or not all([isinstance(c, int) for c in eval_parm])
                     or (len(arg) == 1 and eval_parm[0] < 2)
                     or (len(arg) == 2 and eval_parm[1] - eval_parm[0] < 2)
                 ):
-
                     args = "{}".format(node.lineno)
                     self.add_message("invalid-range-index", node=node, args=args)
 
                 if len(arg) == 3:
                     if (
                         abs(eval_parm[2]) >= abs(eval_parm[0] - eval_parm[1])
                         or eval_parm[2] == 0
                         or (eval_parm[0] > eval_parm[1] and eval_parm[2] < 0)
                         or (eval_parm[0] < eval_parm[1] and eval_parm[2] > 0)
                     ):
-
                         args = "{}".format(node.lineno)
                         self.add_message("invalid-range-index", node=node, args=args)
 
 
 def register(linter):
     """required method to auto register this checker"""
     linter.register_checker(InvalidRangeIndexChecker(linter))
```

### Comparing `python-ta-2.4.2/python_ta/checkers/missing_space_in_doctest_checker.py` & `python-ta-2.5.0/python_ta/checkers/missing_space_in_doctest_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 DOCTEST = ">>>"
 
 
 class MissingSpaceInDoctestChecker(BaseChecker):
-
     name = "missing_space_in_doctest"
     msgs = {
         "E9973": (
             'Space missing after >>> in the docstring of "%s."',
             "missing-space-in-doctest",
             "Used when a doctest is missing a space before the code to be executed",
         )
```

### Comparing `python-ta-2.4.2/python_ta/checkers/one_iteration_checker.py` & `python-ta-2.5.0/python_ta/checkers/one_iteration_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from astroid import nodes
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 
 class OneIterationChecker(BaseChecker):
-
     # name is the same as file name but without _checker part
     name = "one_iteration"
     # use dashes for connecting words in message symbol
     msgs = {
         "E9996": (
             "This loop will only ever run for one iteration",
             "one-iteration",
```

### Comparing `python-ta-2.4.2/python_ta/checkers/possibly_undefined_checker.py` & `python-ta-2.5.0/python_ta/checkers/possibly_undefined_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pylint.checkers import BaseChecker, utils
 from pylint.checkers.utils import only_required_for_messages
 
 from python_ta.cfg.graph import CFGBlock, ControlFlowGraph
 
 
 class PossiblyUndefinedChecker(BaseChecker):
-
     # name is the same as file name but without _checker part
     name = "possibly_undefined"
     # use dashes for connecting words in message symbol
     msgs = {
         "E9969": (
             "This variable might not be defined when this statement is executed.",
             "possibly-undefined",
@@ -138,15 +137,15 @@
                 statement.generators
             )  # statement.generators is a list of nodes
             if not hasattr(statement, "elt"):
                 yield from self.get_nodes(statement.key)  # keys evaluated first
                 yield from self.get_nodes(statement.value)
             else:
                 yield from self.get_nodes(statement.elt)
-        else:
-            yield from statement.nodes_of_class(
-                (nodes.AssignName, nodes.DelName, nodes.Name), nodes.FunctionDef
-            )
+        elif isinstance(statement, (nodes.AssignName, nodes.DelName, nodes.Name)):
+            yield statement
+        elif not isinstance(statement, nodes.FunctionDef):
+            yield from multiple_nodes(statement.get_children())
 
 
 def register(linter):
     linter.register_checker(PossiblyUndefinedChecker(linter))
```

### Comparing `python-ta-2.4.2/python_ta/checkers/pycodestyle_checker.py` & `python-ta-2.5.0/python_ta/checkers/pycodestyle_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pycodestyle
 from pylint.checkers import BaseRawFileChecker
 
 
 class PycodestyleChecker(BaseRawFileChecker):
-
     name = "pep8_errors"
     msgs = {"E9989": ("Found pycodestyle (PEP8) style error at %s", "pep8-errors", "")}
 
     options = (
         (
             "pycodestyle-ignore",
             {
```

### Comparing `python-ta-2.4.2/python_ta/checkers/redundant_assignment_checker.py` & `python-ta-2.5.0/python_ta/checkers/redundant_assignment_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 from python_ta.cfg.graph import CFGBlock, ControlFlowGraph
 
 
 class RedundantAssignmentChecker(BaseChecker):
-
     # name is the same as file name but without _checker part
     name = "redundant_assignment"
     # use dashes for connecting words in message symbol
     msgs = {
         "E9959": (
             "This assignment statement is redundant;" " You can remove it from the program.",
             "redundant-assignment",
```

### Comparing `python-ta-2.4.2/python_ta/checkers/shadowing_in_comprehension_checker.py` & `python-ta-2.5.0/python_ta/checkers/shadowing_in_comprehension_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """
 from astroid import nodes
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 
 class ShadowingInComprehensionChecker(BaseChecker):
-
     name = "shadowing_in_comprehension"
     msgs = {
         "E9988": (
             "Comprehension variable '%s' shadows a variable in an outer scope",
             "shadowing-in-comprehension",
             "Used when there is shadowing inside a comprehension",
         )
```

### Comparing `python-ta-2.4.2/python_ta/checkers/top_level_code_checker.py` & `python-ta-2.5.0/python_ta/checkers/top_level_code_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/checkers/type_annotation_checker.py` & `python-ta-2.5.0/python_ta/checkers/type_annotation_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from astroid import Uninferable, nodes
 from astroid.exceptions import NoDefault
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 
 class TypeAnnotationChecker(BaseChecker):
-
     name = "TypeAnnotationChecker"
     msgs = {
         "E9970": (
             "Function parameter is missing type annotation",
             "missing-param-type",
             "Presented when a type annotation is missing.",
         ),
```

### Comparing `python-ta-2.4.2/python_ta/checkers/type_inference_checker.py` & `python-ta-2.5.0/python_ta/checkers/type_inference_checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 from python_ta.typecheck.base import TypeFail
 
 
 class TypeInferenceChecker(BaseChecker):
-
     name = "TypeInferenceChecker"
     msgs = {
         "E9900": (
             "Type error: %s",
             "type-error",
             "Presented when there is some kind of error with types.",
         )
```

### Comparing `python-ta-2.4.2/python_ta/checkers/unnecessary_indexing_checker.py` & `python-ta-2.5.0/python_ta/checkers/unnecessary_indexing_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/config/.pylintrc` & `python-ta-2.5.0/python_ta/config/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/config/messages_config.toml` & `python-ta-2.5.0/python_ta/config/messages_config.toml`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/contracts/__init__.py` & `python-ta-2.5.0/python_ta/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/contracts/__main__.py` & `python-ta-2.5.0/python_ta/contracts/__main__.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/debug/accumulation_table.py` & `python-ta-2.5.0/python_ta/debug/accumulation_table.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/patches/checkers.py` & `python-ta-2.5.0/python_ta/patches/checkers.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/patches/error_messages.py` & `python-ta-2.5.0/python_ta/patches/error_messages.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/patches/messages.py` & `python-ta-2.5.0/python_ta/patches/messages.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/patches/transforms.py` & `python-ta-2.5.0/python_ta/patches/transforms.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/color_reporter.py` & `python-ta-2.5.0/python_ta/reporters/color_reporter.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/core.py` & `python-ta-2.5.0/python_ta/reporters/core.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/html_reporter.py` & `python-ta-2.5.0/python_ta/reporters/html_reporter.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/json_reporter.py` & `python-ta-2.5.0/python_ta/reporters/json_reporter.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/node_printers.py` & `python-ta-2.5.0/python_ta/reporters/node_printers.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/plain_reporter.py` & `python-ta-2.5.0/python_ta/reporters/plain_reporter.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/stat_reporter.py` & `python-ta-2.5.0/python_ta/reporters/stat_reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .plain_reporter import PlainReporter
 
 
 class StatReporter(PlainReporter):
-
     error_messages = []
     style_messages = []
 
     def __init__(self, source_lines=None):
         """Initialize a StatReporter.
 
         Clear the two class-level message lists.
```

### Comparing `python-ta-2.4.2/python_ta/reporters/templates/jquery-3.2.1.min.js` & `python-ta-2.5.0/python_ta/reporters/templates/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/templates/pyta_logo_markdown.png` & `python-ta-2.5.0/python_ta/reporters/templates/pyta_logo_markdown.png`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/templates/script.js` & `python-ta-2.5.0/python_ta/reporters/templates/script.js`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/templates/stylesheet.css` & `python-ta-2.5.0/python_ta/reporters/templates/stylesheet.css`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/reporters/templates/template.html.jinja` & `python-ta-2.5.0/python_ta/reporters/templates/template.html.jinja`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/transforms/ExprWrapper.py` & `python-ta-2.5.0/python_ta/transforms/ExprWrapper.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/transforms/setendings.py` & `python-ta-2.5.0/python_ta/transforms/setendings.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/transforms/type_inference_visitor.py` & `python-ta-2.5.0/python_ta/transforms/type_inference_visitor.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/transforms/z3_visitor.py` & `python-ta-2.5.0/python_ta/transforms/z3_visitor.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/typecheck/base.py` & `python-ta-2.5.0/python_ta/typecheck/base.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/typecheck/errors.py` & `python-ta-2.5.0/python_ta/typecheck/errors.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/typecheck/type_store.py` & `python-ta-2.5.0/python_ta/typecheck/type_store.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/typecheck/typeshed/README.md` & `python-ta-2.5.0/python_ta/typecheck/typeshed/README.md`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/typecheck/typeshed/builtins.pyi` & `python-ta-2.5.0/python_ta/typecheck/typeshed/builtins.pyi`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/upload.py` & `python-ta-2.5.0/python_ta/upload.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/util/monad.py` & `python-ta-2.5.0/python_ta/util/monad.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta/utils.py` & `python-ta-2.5.0/python_ta/utils.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/python_ta.egg-info/PKG-INFO` & `python-ta-2.5.0/python_ta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ta
-Version: 2.4.2
+Version: 2.5.0
 Summary: Code checking tool for teaching Python
 Home-page: https://github.com/pyta-uoft/pyta
 Author: David Liu
 Author-email: david@cs.toronto.edu
 License: MIT
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `python-ta-2.4.2/python_ta.egg-info/SOURCES.txt` & `python-ta-2.5.0/python_ta.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 python_ta.egg-info/top_level.txt
 python_ta/cfg/__init__.py
 python_ta/cfg/graph.py
 python_ta/cfg/visitor.py
 python_ta/checkers/__init__.py
 python_ta/checkers/forbidden_import_checker.py
 python_ta/checkers/forbidden_io_function_checker.py
+python_ta/checkers/forbidden_python_syntax_checker.py
 python_ta/checkers/global_variables_checker.py
 python_ta/checkers/invalid_for_target_checker.py
 python_ta/checkers/invalid_range_index_checker.py
 python_ta/checkers/missing_space_in_doctest_checker.py
 python_ta/checkers/one_iteration_checker.py
 python_ta/checkers/possibly_undefined_checker.py
 python_ta/checkers/pycodestyle_checker.py
```

### Comparing `python-ta-2.4.2/sample_usage/draw_cfg.py` & `python-ta-2.5.0/sample_usage/draw_cfg.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,55 +4,61 @@
 import graphviz
 from astroid import nodes
 from astroid.builder import AstroidBuilder
 
 from python_ta.cfg import CFGBlock, CFGVisitor, ControlFlowGraph
 
 USAGE = "USAGE: python -m sample_usage.draw_cfg <your-file.py>"
-GRAPH_OPTIONS = {"format": "jpg", "node_attr": {"shape": "box", "fontname": "Courier New"}}
+GRAPH_OPTIONS = {"format": "svg", "node_attr": {"shape": "box", "fontname": "Courier New"}}
+SUBGRAPH_OPTIONS = {"fontname": "Courier New"}
 
 
 def display(cfgs: Dict[nodes.NodeNG, ControlFlowGraph], filename: str, view: bool = True) -> None:
     graph = graphviz.Digraph(name=filename, **GRAPH_OPTIONS)
     for node, cfg in cfgs.items():
         if isinstance(node, nodes.Module):
             subgraph_label = "__main__"
         elif isinstance(node, nodes.FunctionDef):
             subgraph_label = node.name
         else:
             continue
         with graph.subgraph(name=f"cluster_{id(node)}") as c:
             visited = set()
-            _visit(cfg.start, c, visited)
+            _visit(cfg.start, c, visited, cfg.end)
             for block in cfg.unreachable_blocks:
-                _visit(block, c, visited)
-            c.attr(label=subgraph_label)
+                _visit(block, c, visited, cfg.end)
+            c.attr(label=subgraph_label, **SUBGRAPH_OPTIONS)
 
     graph.render(filename, view=view)
 
 
-def _visit(block: CFGBlock, graph: graphviz.Digraph, visited: Set[int]) -> None:
+def _visit(block: CFGBlock, graph: graphviz.Digraph, visited: Set[int], end: CFGBlock) -> None:
     node_id = f"{graph.name}_{block.id}"
     if node_id in visited:
         return
 
     label = "\n".join([s.as_string() for s in block.statements]) + "\n"
     # Need to escape backslashes explicitly.
     label = label.replace("\\", "\\\\")
     # \l is used for left alignment.
     label = label.replace("\n", "\\l")
 
     fill_color = "grey93" if not block.reachable else "white"
+    # Change the fill colour if block is the end of the cfg
+    fill_color = "black" if block == end else fill_color
 
     graph.node(node_id, label=label, fillcolor=fill_color, style="filled")
     visited.add(node_id)
 
     for edge in block.successors:
-        graph.edge(node_id, f"{graph.name}_{edge.target.id}")
-        _visit(edge.target, graph, visited)
+        if edge.label is not None:
+            graph.edge(node_id, f"{graph.name}_{edge.target.id}", str(edge.label))
+        else:
+            graph.edge(node_id, f"{graph.name}_{edge.target.id}")
+        _visit(edge.target, graph, visited, end)
 
 
 def main(filepath: str) -> None:
     filename = os.path.splitext(os.path.basename(filepath))[0]
     mod = AstroidBuilder().file_build(filepath)
     visitor = CFGVisitor()
     mod.accept(visitor)
```

### Comparing `python-ta-2.4.2/sample_usage/draw_tnodes.py` & `python-ta-2.5.0/sample_usage/draw_tnodes.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/sample_usage/print_ast.py` & `python-ta-2.5.0/sample_usage/print_ast.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/sample_usage/print_nodes.py` & `python-ta-2.5.0/sample_usage/print_nodes.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/sample_usage/print_table.py` & `python-ta-2.5.0/sample_usage/print_table.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/sample_usage/pyta_stats.py` & `python-ta-2.5.0/sample_usage/pyta_stats.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/sample_usage/stats_analysis.py` & `python-ta-2.5.0/sample_usage/stats_analysis.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/setup.cfg` & `python-ta-2.5.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -18,41 +18,46 @@
 00000110: 725f 656d 6169 6c20 3d20 6461 7669 6440  r_email = david@
 00000120: 6373 2e74 6f72 6f6e 746f 2e65 6475 0d0a  cs.toronto.edu..
 00000130: 6c69 6365 6e73 6520 3d20 4d49 540d 0a0d  license = MIT...
 00000140: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 7374  .[options]..inst
 00000150: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
 00000160: 0a09 6173 7472 6f69 6420 7e3d 2032 2e31  ..astroid ~= 2.1
 00000170: 322e 3133 0d0a 0970 7963 6f64 6573 7479  2.13...pycodesty
-00000180: 6c65 0d0a 0970 796c 696e 7420 7e3d 2032  le...pylint ~= 2
-00000190: 2e31 352e 380d 0a09 7461 6275 6c61 7465  .15.8...tabulate
-000001a0: 7e3d 302e 382e 390d 0a09 636f 6c6f 7261  ~=0.8.9...colora
-000001b0: 6d61 0d0a 0973 6978 0d0a 096a 696e 6a61  ma...six...jinja
-000001c0: 320d 0a09 7079 676d 656e 7473 0d0a 0977  2...pygments...w
-000001d0: 7261 7074 203e 3d20 312e 3134 2e31 0d0a  rapt >= 1.14.1..
-000001e0: 0974 7970 6567 7561 7264 203e 3d20 322e  .typeguard >= 2.
-000001f0: 3133 2e33 0d0a 0972 6571 7565 7374 730d  13.3...requests.
-00000200: 0a09 636c 6963 6b20 3e3d 2038 2e30 2e31  ..click >= 8.0.1
-00000210: 0d0a 0974 6f6d 6c0d 0a70 6163 6b61 6765  ...toml..package
-00000220: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000230: 6e5f 7265 7175 6972 6573 203d 207e 3d33  n_requires = ~=3
-00000240: 2e38 0d0a 7a69 705f 7361 6665 203d 2046  .8..zip_safe = F
-00000250: 616c 7365 0d0a 696e 636c 7564 655f 7061  alse..include_pa
-00000260: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-00000270: 650d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  e....[options.ex
-00000280: 7472 6173 5f72 6571 7569 7265 5d0d 0a64  tras_require]..d
-00000290: 6576 203d 200d 0a09 6772 6170 6876 697a  ev = ...graphviz
-000002a0: 0d0a 0968 7970 6f74 6865 7369 730d 0a09  ...hypothesis...
-000002b0: 696e 666c 6563 7469 6f6e 0d0a 096d 7973  inflection...mys
-000002c0: 742d 7061 7273 6572 0d0a 0970 7265 2d63  t-parser...pre-c
-000002d0: 6f6d 6d69 740d 0a09 7079 7465 7374 0d0a  ommit...pytest..
-000002e0: 0970 7974 6573 742d 636f 760d 0a09 7370  .pytest-cov...sp
-000002f0: 6869 6e78 0d0a 0973 7068 696e 782d 7274  hinx...sphinx-rt
-00000300: 642d 7468 656d 650d 0a7a 3320 3d20 0d0a  d-theme..z3 = ..
-00000310: 097a 332d 736f 6c76 6572 0d0a 0d0a 5b6f  .z3-solver....[o
-00000320: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-00000330: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-00000340: 7269 7074 7320 3d20 0d0a 0970 7974 686f  ripts = ...pytho
-00000350: 6e5f 7461 203d 2070 7974 686f 6e5f 7461  n_ta = python_ta
-00000360: 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e 0d0a  .__main__:main..
-00000370: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000380: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000390: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000180: 6c65 207e 3d20 322e 3130 2e30 0d0a 0970  le ~= 2.10.0...p
+00000190: 796c 696e 7420 7e3d 2032 2e31 352e 380d  ylint ~= 2.15.8.
+000001a0: 0a09 7461 6275 6c61 7465 207e 3d20 302e  ..tabulate ~= 0.
+000001b0: 392e 300d 0a09 636f 6c6f 7261 6d61 207e  9.0...colorama ~
+000001c0: 3d20 302e 342e 360d 0a09 7369 780d 0a09  = 0.4.6...six...
+000001d0: 6a69 6e6a 6132 207e 3d20 332e 312e 320d  jinja2 ~= 3.1.2.
+000001e0: 0a09 7079 676d 656e 7473 207e 3d20 322e  ..pygments ~= 2.
+000001f0: 3134 2e30 0d0a 0977 7261 7074 203e 3d20  14.0...wrapt >= 
+00000200: 312e 3135 2e30 2c20 3c20 320d 0a09 7479  1.15.0, < 2...ty
+00000210: 7065 6775 6172 6420 3e3d 2032 2e31 332e  peguard >= 2.13.
+00000220: 332c 203c 2033 0d0a 0972 6571 7565 7374  3, < 3...request
+00000230: 7320 7e3d 2032 2e32 382e 300d 0a09 636c  s ~= 2.28.0...cl
+00000240: 6963 6b20 3e3d 2038 2e30 2e31 2c20 3c20  ick >= 8.0.1, < 
+00000250: 390d 0a09 746f 6d6c 207e 3d20 302e 3130  9...toml ~= 0.10
+00000260: 2e32 0d0a 7061 636b 6167 6573 203d 2066  .2..packages = f
+00000270: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
+00000280: 7569 7265 7320 3d20 7e3d 332e 380d 0a7a  uires = ~=3.8..z
+00000290: 6970 5f73 6166 6520 3d20 4661 6c73 650d  ip_safe = False.
+000002a0: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+000002b0: 5f64 6174 6120 3d20 5472 7565 0d0a 0d0a  _data = True....
+000002c0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+000002d0: 7265 7175 6972 655d 0d0a 6465 7620 3d20  require]..dev = 
+000002e0: 0d0a 0967 7261 7068 7669 7a0d 0a09 6879  ...graphviz...hy
+000002f0: 706f 7468 6573 6973 0d0a 0969 6e66 6c65  pothesis...infle
+00000300: 6374 696f 6e0d 0a09 6d79 7374 2d70 6172  ction...myst-par
+00000310: 7365 720d 0a09 7072 652d 636f 6d6d 6974  ser...pre-commit
+00000320: 0d0a 0970 7974 6573 740d 0a09 7079 7465  ...pytest...pyte
+00000330: 7374 2d63 6f76 0d0a 0973 7068 696e 780d  st-cov...sphinx.
+00000340: 0a09 7370 6869 6e78 2d72 7464 2d74 6865  ..sphinx-rtd-the
+00000350: 6d65 0d0a 7a33 203d 200d 0a09 7a33 2d73  me..z3 = ...z3-s
+00000360: 6f6c 7665 720d 0a0d 0a5b 6f70 7469 6f6e  olver....[option
+00000370: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+00000380: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+00000390: 203d 200d 0a09 7079 7468 6f6e 5f74 6120   = ...python_ta 
+000003a0: 3d20 7079 7468 6f6e 5f74 612e 5f5f 6d61  = python_ta.__ma
+000003b0: 696e 5f5f 3a6d 6169 6e0d 0a0d 0a5b 6567  in__:main....[eg
+000003c0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000003d0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000003e0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `python-ta-2.4.2/tests/custom_hypothesis_support.py` & `python-ta-2.5.0/tests/custom_hypothesis_support.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_check.py` & `python-ta-2.5.0/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_class_contracts.py` & `python-ta-2.5.0/tests/test_class_contracts.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_contracts.py` & `python-ta-2.5.0/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_examples.py` & `python-ta-2.5.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_setendings.py` & `python-ta-2.5.0/tests/test_setendings.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_subclass_contracts.py` & `python-ta-2.5.0/tests/test_subclass_contracts.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_constraints/test_tnode_structure.py` & `python-ta-2.5.0/tests/test_type_constraints/test_tnode_structure.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_constraints/test_unify.py` & `python-ta-2.5.0/tests/test_type_constraints/test_unify.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_annassign.py` & `python-ta-2.5.0/tests/test_type_inference/test_annassign.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_assign.py` & `python-ta-2.5.0/tests/test_type_inference/test_assign.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_assign_tuple.py` & `python-ta-2.5.0/tests/test_type_inference/test_assign_tuple.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_attribute.py` & `python-ta-2.5.0/tests/test_type_inference/test_attribute.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_binops.py` & `python-ta-2.5.0/tests/test_type_inference/test_binops.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_boolops.py` & `python-ta-2.5.0/tests/test_type_inference/test_boolops.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_classdef.py` & `python-ta-2.5.0/tests/test_type_inference/test_classdef.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_compare.py` & `python-ta-2.5.0/tests/test_type_inference/test_compare.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_const.py` & `python-ta-2.5.0/tests/test_type_inference/test_const.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_dict.py` & `python-ta-2.5.0/tests/test_type_inference/test_dict.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_dictcomp.py` & `python-ta-2.5.0/tests/test_type_inference/test_dictcomp.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_errors.py` & `python-ta-2.5.0/tests/test_type_inference/test_errors.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_for.py` & `python-ta-2.5.0/tests/test_type_inference/test_for.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_function_annotation.py` & `python-ta-2.5.0/tests/test_type_inference/test_function_annotation.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_function_def_inference.py` & `python-ta-2.5.0/tests/test_type_inference/test_function_def_inference.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_function_overload.py` & `python-ta-2.5.0/tests/test_type_inference/test_function_overload.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_functions.py` & `python-ta-2.5.0/tests/test_type_inference/test_functions.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_ifexpr.py` & `python-ta-2.5.0/tests/test_type_inference/test_ifexpr.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_imports.py` & `python-ta-2.5.0/tests/test_type_inference/test_imports.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_initializer.py` & `python-ta-2.5.0/tests/test_type_inference/test_initializer.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_lambda.py` & `python-ta-2.5.0/tests/test_type_inference/test_lambda.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_list.py` & `python-ta-2.5.0/tests/test_type_inference/test_list.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_listcomp.py` & `python-ta-2.5.0/tests/test_type_inference/test_listcomp.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_literals.py` & `python-ta-2.5.0/tests/test_type_inference/test_literals.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_name.py` & `python-ta-2.5.0/tests/test_type_inference/test_name.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_set.py` & `python-ta-2.5.0/tests/test_type_inference/test_set.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_setcomp.py` & `python-ta-2.5.0/tests/test_type_inference/test_setcomp.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_starred.py` & `python-ta-2.5.0/tests/test_type_inference/test_starred.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_subscript.py` & `python-ta-2.5.0/tests/test_type_inference/test_subscript.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_tuple.py` & `python-ta-2.5.0/tests/test_type_inference/test_tuple.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_typefail_reason.py` & `python-ta-2.5.0/tests/test_type_inference/test_typefail_reason.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_type_inference/test_unaryops.py` & `python-ta-2.5.0/tests/test_type_inference/test_unaryops.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.4.2/tests/test_z3_visitor.py` & `python-ta-2.5.0/tests/test_z3_visitor.py`

 * *Files identical despite different names*

