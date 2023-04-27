# Comparing `tmp/pddl-plus-parser-3.3.5.tar.gz` & `tmp/pddl-plus-parser-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddl-plus-parser-3.3.5.tar", last modified: Tue Apr 25 14:27:05 2023, max compression
+gzip compressed data, was "pddl-plus-parser-3.3.6.tar", last modified: Thu Apr 27 10:37:42 2023, max compression
```

## Comparing `pddl-plus-parser-3.3.5.tar` & `pddl-plus-parser-3.3.6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.361264 pddl-plus-parser-3.3.5/
--rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.3.5/LICENSE
--rw-rw-rw-   0        0        0     1519 2023-04-25 14:27:05.360264 pddl-plus-parser-3.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1249 2023-04-17 12:20:18.000000 pddl-plus-parser-3.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.292231 pddl-plus-parser-3.3.5/pddl_plus_parser/
--rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.301239 pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/
--rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/__init__.py
--rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/domain_exporter.py
--rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/enhsp_output_parser.py
--rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/ff_output_parser.py
--rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
--rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/problem_exporter.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.309241 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/
--rw-rw-rw-   0        0        0      376 2023-04-17 14:54:54.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/__init__.py
--rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/domain_parser.py
--rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/effects_parser.py
--rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/parsing_utils.py
--rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
--rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
--rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/preconditions_parser.py
--rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/problem_parser.py
--rw-rw-rw-   0        0        0    10281 2023-02-20 11:23:13.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/trajectory_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.327241 pddl-plus-parser-3.3.5/pddl_plus_parser/models/
--rw-rw-rw-   0        0        0      929 2023-04-09 14:33:10.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/__init__.py
--rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/action_call.py
--rw-rw-rw-   0        0        0     1853 2023-04-13 11:59:48.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/conditional_effect.py
--rw-rw-rw-   0        0        0     5945 2023-04-17 10:57:12.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/grounded_effect.py
--rw-rw-rw-   0        0        0    12934 2023-04-17 09:01:49.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/grounded_precondition.py
--rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/grounding_utils.py
--rw-rw-rw-   0        0        0     7500 2023-04-16 13:28:59.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/numerical_expression.py
--rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/observation.py
--rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_action.py
--rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_domain.py
--rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_function.py
--rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_object.py
--rw-rw-rw-   0        0        0     8519 2023-04-17 10:10:02.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_operator.py
--rw-rw-rw-   0        0        0     7704 2023-04-25 14:26:48.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_precondition.py
--rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_predicate.py
--rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_problem.py
--rw-rw-rw-   0        0        0     2845 2023-04-16 13:40:45.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_state.py
--rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_type.py
--rw-rw-rw-   0        0        0     1865 2023-04-09 08:35:12.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/models/universal_quantifier.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.333238 pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/
--rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/common.py
--rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
--rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
--rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
--rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.341241 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/
--rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/__init__.py
--rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/common.py
--rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/counters_generator.py
--rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/depots_generator.py
--rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/farmland_generator.py
--rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/plant_watering_generator.py
--rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/sailing_generator.py
--rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/settlers_problem_generator.py
--rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/zenotravel_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.296231 pddl-plus-parser-3.3.5/pddl_plus_parser.egg-info/
--rw-rw-rw-   0        0        0     1519 2023-04-25 14:27:05.000000 pddl-plus-parser-3.3.5/pddl_plus_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3567 2023-04-25 14:27:05.000000 pddl-plus-parser-3.3.5/pddl_plus_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 14:27:05.000000 pddl-plus-parser-3.3.5/pddl_plus_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-25 14:27:05.000000 pddl-plus-parser-3.3.5/pddl_plus_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 14:27:05.361264 pddl-plus-parser-3.3.5/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-04-25 14:26:54.000000 pddl-plus-parser-3.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.289232 pddl-plus-parser-3.3.5/tests/
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.342241 pddl-plus-parser-3.3.5/tests/exporters_tests/
--rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.3.5/tests/exporters_tests/__init__.py
--rw-rw-rw-   0        0        0     9454 2023-04-17 10:52:47.000000 pddl-plus-parser-3.3.5/tests/exporters_tests/numeric_trajectory_exporter_test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.347241 pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/
--rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/__init__.py
--rw-rw-rw-   0        0        0     3288 2023-04-17 12:07:14.000000 pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/consts.py
--rw-rw-rw-   0        0        0    39905 2023-04-17 12:16:07.000000 pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/domain_parser_test.py
--rw-rw-rw-   0        0        0     3578 2023-04-09 11:50:45.000000 pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/pddl_tokenizer_test.py
--rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/problem_parser_test.py
--rw-rw-rw-   0        0        0     6285 2023-02-21 16:00:23.000000 pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/trajectory_parser_test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.354239 pddl-plus-parser-3.3.5/tests/models_tests/
--rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.3.5/tests/models_tests/__init__.py
--rw-rw-rw-   0        0        0      427 2022-12-05 14:12:59.000000 pddl-plus-parser-3.3.5/tests/models_tests/consts.py
--rw-rw-rw-   0        0        0    15208 2023-04-17 10:08:25.000000 pddl-plus-parser-3.3.5/tests/models_tests/grounded_effect_test.py
--rw-rw-rw-   0        0        0    25195 2023-04-17 09:16:34.000000 pddl-plus-parser-3.3.5/tests/models_tests/grounded_precondition_test.py
--rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.3.5/tests/models_tests/numerical_expression_test.py
--rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.3.5/tests/models_tests/operator_test.py
--rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.3.5/tests/models_tests/pddl_function_test.py
--rw-rw-rw-   0        0        0     4116 2023-04-20 15:01:48.000000 pddl-plus-parser-3.3.5/tests/models_tests/pddl_precondition_test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:05.359238 pddl-plus-parser-3.3.5/tests/multi_agent_tests/
--rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.3.5/tests/multi_agent_tests/__init__.py
--rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.3.5/tests/multi_agent_tests/consts.py
--rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.3.5/tests/multi_agent_tests/multi_agent_domain_converter_test.py
--rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.3.5/tests/multi_agent_tests/multi_agent_problem_converter_test.py
--rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.3.5/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
--rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.3.5/tests/multi_agent_tests/single_agent_plan_converter_test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.547000 pddl-plus-parser-3.3.6/
+-rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.3.6/LICENSE
+-rw-rw-rw-   0        0        0     1519 2023-04-27 10:37:42.547000 pddl-plus-parser-3.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2023-04-17 12:20:18.000000 pddl-plus-parser-3.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.455577 pddl-plus-parser-3.3.6/pddl_plus_parser/
+-rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.467095 pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/
+-rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/__init__.py
+-rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/domain_exporter.py
+-rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/enhsp_output_parser.py
+-rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/ff_output_parser.py
+-rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
+-rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/problem_exporter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.479516 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/
+-rw-rw-rw-   0        0        0      376 2023-04-17 14:54:54.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/__init__.py
+-rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/domain_parser.py
+-rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/effects_parser.py
+-rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/parsing_utils.py
+-rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
+-rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
+-rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/preconditions_parser.py
+-rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/problem_parser.py
+-rw-rw-rw-   0        0        0    10281 2023-02-20 11:23:13.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/trajectory_parser.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.501059 pddl-plus-parser-3.3.6/pddl_plus_parser/models/
+-rw-rw-rw-   0        0        0      929 2023-04-09 14:33:10.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/action_call.py
+-rw-rw-rw-   0        0        0     1853 2023-04-13 11:59:48.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/conditional_effect.py
+-rw-rw-rw-   0        0        0     5945 2023-04-17 10:57:12.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/grounded_effect.py
+-rw-rw-rw-   0        0        0    12934 2023-04-17 09:01:49.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/grounded_precondition.py
+-rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/grounding_utils.py
+-rw-rw-rw-   0        0        0     7500 2023-04-16 13:28:59.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/numerical_expression.py
+-rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/observation.py
+-rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_action.py
+-rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_domain.py
+-rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_function.py
+-rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_object.py
+-rw-rw-rw-   0        0        0     8519 2023-04-17 10:10:02.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_operator.py
+-rw-rw-rw-   0        0        0     9709 2023-04-27 10:37:17.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_precondition.py
+-rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_predicate.py
+-rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_problem.py
+-rw-rw-rw-   0        0        0     2845 2023-04-16 13:40:45.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_state.py
+-rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_type.py
+-rw-rw-rw-   0        0        0     1865 2023-04-09 08:35:12.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/models/universal_quantifier.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.508074 pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/
+-rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/common.py
+-rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
+-rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
+-rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
+-rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.518074 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/
+-rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/__init__.py
+-rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/common.py
+-rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/counters_generator.py
+-rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/depots_generator.py
+-rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/farmland_generator.py
+-rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/plant_watering_generator.py
+-rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/sailing_generator.py
+-rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/settlers_problem_generator.py
+-rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/zenotravel_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.459086 pddl-plus-parser-3.3.6/pddl_plus_parser.egg-info/
+-rw-rw-rw-   0        0        0     1519 2023-04-27 10:37:42.000000 pddl-plus-parser-3.3.6/pddl_plus_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3567 2023-04-27 10:37:42.000000 pddl-plus-parser-3.3.6/pddl_plus_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:37:42.000000 pddl-plus-parser-3.3.6/pddl_plus_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-27 10:37:42.000000 pddl-plus-parser-3.3.6/pddl_plus_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:37:42.547000 pddl-plus-parser-3.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-04-27 10:33:43.000000 pddl-plus-parser-3.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.451561 pddl-plus-parser-3.3.6/tests/
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.520098 pddl-plus-parser-3.3.6/tests/exporters_tests/
+-rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.3.6/tests/exporters_tests/__init__.py
+-rw-rw-rw-   0        0        0     9454 2023-04-17 10:52:47.000000 pddl-plus-parser-3.3.6/tests/exporters_tests/numeric_trajectory_exporter_test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.528008 pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/__init__.py
+-rw-rw-rw-   0        0        0     3288 2023-04-17 12:07:14.000000 pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/consts.py
+-rw-rw-rw-   0        0        0    39905 2023-04-17 12:16:07.000000 pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/domain_parser_test.py
+-rw-rw-rw-   0        0        0     3578 2023-04-09 11:50:45.000000 pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/pddl_tokenizer_test.py
+-rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/problem_parser_test.py
+-rw-rw-rw-   0        0        0     6285 2023-02-21 16:00:23.000000 pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/trajectory_parser_test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.537989 pddl-plus-parser-3.3.6/tests/models_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.3.6/tests/models_tests/__init__.py
+-rw-rw-rw-   0        0        0      427 2022-12-05 14:12:59.000000 pddl-plus-parser-3.3.6/tests/models_tests/consts.py
+-rw-rw-rw-   0        0        0    15208 2023-04-17 10:08:25.000000 pddl-plus-parser-3.3.6/tests/models_tests/grounded_effect_test.py
+-rw-rw-rw-   0        0        0    25195 2023-04-17 09:16:34.000000 pddl-plus-parser-3.3.6/tests/models_tests/grounded_precondition_test.py
+-rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.3.6/tests/models_tests/numerical_expression_test.py
+-rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.3.6/tests/models_tests/operator_test.py
+-rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.3.6/tests/models_tests/pddl_function_test.py
+-rw-rw-rw-   0        0        0     6075 2023-04-27 10:33:43.000000 pddl-plus-parser-3.3.6/tests/models_tests/pddl_precondition_test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:37:42.544996 pddl-plus-parser-3.3.6/tests/multi_agent_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.3.6/tests/multi_agent_tests/__init__.py
+-rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.3.6/tests/multi_agent_tests/consts.py
+-rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.3.6/tests/multi_agent_tests/multi_agent_domain_converter_test.py
+-rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.3.6/tests/multi_agent_tests/multi_agent_problem_converter_test.py
+-rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.3.6/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
+-rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.3.6/tests/multi_agent_tests/single_agent_plan_converter_test.py
```

### Comparing `pddl-plus-parser-3.3.5/LICENSE` & `pddl-plus-parser-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/PKG-INFO` & `pddl-plus-parser-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.3.5
+Version: 3.3.6
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
```

### Comparing `pddl-plus-parser-3.3.5/README.md` & `pddl-plus-parser-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/domain_exporter.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/domain_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/enhsp_output_parser.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/enhsp_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/ff_output_parser.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/ff_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/numeric_trajectory_exporter.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/numeric_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/exporters/problem_exporter.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/exporters/problem_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/domain_parser.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/domain_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/effects_parser.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/effects_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/parsing_utils.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/preconditions_parser.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/preconditions_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/problem_parser.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/problem_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/lisp_parsers/trajectory_parser.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/lisp_parsers/trajectory_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/__init__.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/action_call.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/action_call.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/conditional_effect.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/conditional_effect.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/grounded_effect.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/grounded_effect.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/grounded_precondition.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/grounded_precondition.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/grounding_utils.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/grounding_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/numerical_expression.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/numerical_expression.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/observation.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/observation.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_action.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_action.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_domain.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_domain.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_function.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_function.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_operator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_operator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_precondition.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_precondition.py`

 * *Files 21% similar despite different names*

```diff
@@ -111,14 +111,42 @@
             if condition.to_pddl() not in current_expressions:
                 self.operands.add(condition)
         else:
             current_compound_conditions = [str(cond) for cond in self.__iter__() if isinstance(cond, Precondition)]
             if str(condition) not in current_compound_conditions:
                 self.operands.add(condition)
 
+    @staticmethod
+    def _remove_condition(
+            condition_to_remove: Union["Precondition", Predicate, GroundedPredicate, NumericalExpressionTree],
+            searched_condition: "Precondition") -> bool:
+        """Tries to remove the input precondition from the searched precondition.
+
+        :param condition_to_remove: the condition to remove.
+        :param searched_condition: the precondition to search in.
+        :return: True if the condition was removed, False otherwise.
+        """
+        for operand in searched_condition.operands:
+            if type(operand) == type(condition_to_remove) and operand == condition_to_remove:
+                searched_condition.operands.remove(operand)
+                return True
+
+            elif isinstance(operand, Precondition):
+                if Precondition._remove_condition(condition_to_remove, operand):
+                    return True
+
+    def remove_condition(
+            self, condition: Union["Precondition", Predicate, GroundedPredicate, NumericalExpressionTree]) -> bool:
+        """Remove a condition from the precondition.
+
+        :param condition: the condition to remove.
+        :return: True if the condition was removed, False otherwise.
+        """
+        return self._remove_condition(condition, self)
+
     def add_equality_condition(self, condition: Tuple[str, str], inequality: bool = False) -> None:
         """Add an equality condition to the precondition.
 
         :param condition: the equality condition to add
         :param inequality: whether the condition is an inequality
         """
         if not inequality:
@@ -166,7 +194,24 @@
         return str(self.root)
 
     def __iter__(self) -> Tuple[str, Union[Precondition, UniversalPrecondition]]:
         yield from self.root
 
     def __eq__(self, other: "CompoundPrecondition") -> bool:
         return self.root == other.root
+
+    def add_condition(
+            self, condition: Union[
+                Precondition, UniversalPrecondition, Predicate, GroundedPredicate, NumericalExpressionTree]) -> None:
+        """Add a condition to the compound precondition.
+
+        :param condition: the condition to add.
+        """
+        self.root.add_condition(condition)
+
+    def remove_condition(self, condition: Union[
+        Precondition, UniversalPrecondition, Predicate, GroundedPredicate, NumericalExpressionTree]) -> None:
+        """Remove a condition from the compound precondition.
+
+        :param condition: the condition to remove.
+        """
+        self.root.remove_condition(condition)
```

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_predicate.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_predicate.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_problem.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_problem.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_state.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_state.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/pddl_type.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/pddl_type.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/models/universal_quantifier.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/models/universal_quantifier.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/common.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/common.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/multi_agent/single_agent_plan_converter.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/multi_agent/single_agent_plan_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/counters_generator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/counters_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/depots_generator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/depots_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/farmland_generator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/farmland_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/plant_watering_generator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/plant_watering_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/sailing_generator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/sailing_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/settlers_problem_generator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/settlers_problem_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser/problem_generators/zenotravel_generator.py` & `pddl-plus-parser-3.3.6/pddl_plus_parser/problem_generators/zenotravel_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser.egg-info/PKG-INFO` & `pddl-plus-parser-3.3.6/pddl_plus_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.3.5
+Version: 3.3.6
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
```

### Comparing `pddl-plus-parser-3.3.5/pddl_plus_parser.egg-info/SOURCES.txt` & `pddl-plus-parser-3.3.6/pddl_plus_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/exporters_tests/numeric_trajectory_exporter_test.py` & `pddl-plus-parser-3.3.6/tests/exporters_tests/numeric_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/consts.py` & `pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/domain_parser_test.py` & `pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/domain_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/pddl_tokenizer_test.py` & `pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/pddl_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/problem_parser_test.py` & `pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/problem_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/lisp_parsers_tests/trajectory_parser_test.py` & `pddl-plus-parser-3.3.6/tests/lisp_parsers_tests/trajectory_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/models_tests/grounded_effect_test.py` & `pddl-plus-parser-3.3.6/tests/models_tests/grounded_effect_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/models_tests/grounded_precondition_test.py` & `pddl-plus-parser-3.3.6/tests/models_tests/grounded_precondition_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/models_tests/numerical_expression_test.py` & `pddl-plus-parser-3.3.6/tests/models_tests/numerical_expression_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/models_tests/operator_test.py` & `pddl-plus-parser-3.3.6/tests/models_tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/models_tests/pddl_function_test.py` & `pddl-plus-parser-3.3.6/tests/models_tests/pddl_function_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/models_tests/pddl_precondition_test.py` & `pddl-plus-parser-3.3.6/tests/models_tests/pddl_precondition_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module that tests the functionality of the pddl_precondition module."""
-from pddl_plus_parser.lisp_parsers import DomainParser
-from pddl_plus_parser.models import Predicate, Domain, construct_expression_tree, NumericalExpressionTree
-from pddl_plus_parser.models.pddl_precondition import CompoundPrecondition, Precondition
-
-from pytest import fixture, fail
+from pytest import fixture
 
+from pddl_plus_parser.lisp_parsers import DomainParser
+from pddl_plus_parser.models import Domain, construct_expression_tree, NumericalExpressionTree
+from pddl_plus_parser.models.pddl_precondition import Precondition
 from tests.models_tests.consts import TEST_HARD_NUMERIC_DOMAIN
 
 
 @fixture()
 def domain() -> Domain:
     domain_parser = DomainParser(TEST_HARD_NUMERIC_DOMAIN)
     return domain_parser.parse_domain()
@@ -88,7 +87,44 @@
 
     other_precondition = Precondition("or")
     other_precondition.add_condition(test_predicate)
     other_precondition.add_condition(numeric_expression)
 
     assert not simple_precondition == other_precondition
 
+
+def test_remove_condition_returns_true_and_removes_precondition_from_a_non_nested_precondition_that_includes_only_predicates(
+        simple_precondition: Precondition, domain: Domain):
+    test_predicate = domain.predicates["on_board"]
+    simple_precondition.add_condition(test_predicate)
+    assert test_predicate in simple_precondition.operands
+
+    assert simple_precondition.remove_condition(test_predicate)
+    assert test_predicate not in simple_precondition.operands
+
+
+def test_remove_condition_returns_false_when_predicate_not_in_non_nested_precondition_that_includes_only_predicates(
+        simple_precondition: Precondition, domain: Domain):
+    test_predicate = domain.predicates["on_board"]
+    test_predicate_to_remove = domain.predicates["power_avail"]
+    simple_precondition.add_condition(test_predicate)
+    assert test_predicate in simple_precondition.operands
+    assert test_predicate_to_remove not in simple_precondition.operands
+
+    assert not simple_precondition.remove_condition(test_predicate_to_remove)
+
+
+def test_remove_condition_returns_true_and_removes_precondition_from_a_non_nested_precondition_that_a_precondition(
+        simple_precondition: Precondition, domain: Domain):
+    test_predicate = domain.predicates["on_board"]
+    test_predicate_to_remove = domain.predicates["power_avail"]
+    test_predicate_to_remove2 = domain.predicates["power_on"]
+    simple_precondition.add_condition(test_predicate)
+    test_inner_precondition = Precondition("and")
+    test_inner_precondition.add_condition(test_predicate_to_remove)
+    test_inner_precondition.add_condition(test_predicate_to_remove2)
+    simple_precondition.add_condition(test_inner_precondition)
+    assert test_predicate in simple_precondition.operands
+    assert test_inner_precondition in simple_precondition.operands
+
+    assert simple_precondition.remove_condition(test_inner_precondition)
+    assert test_inner_precondition not in simple_precondition.operands
```

### Comparing `pddl-plus-parser-3.3.5/tests/multi_agent_tests/consts.py` & `pddl-plus-parser-3.3.6/tests/multi_agent_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/multi_agent_tests/multi_agent_domain_converter_test.py` & `pddl-plus-parser-3.3.6/tests/multi_agent_tests/multi_agent_domain_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/multi_agent_tests/multi_agent_problem_converter_test.py` & `pddl-plus-parser-3.3.6/tests/multi_agent_tests/multi_agent_problem_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py` & `pddl-plus-parser-3.3.6/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.5/tests/multi_agent_tests/single_agent_plan_converter_test.py` & `pddl-plus-parser-3.3.6/tests/multi_agent_tests/single_agent_plan_converter_test.py`

 * *Files identical despite different names*

