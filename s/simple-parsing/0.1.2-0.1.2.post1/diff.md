# Comparing `tmp/simple_parsing-0.1.2.tar.gz` & `tmp/simple_parsing-0.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_parsing-0.1.2.tar", last modified: Wed Apr 19 15:30:25 2023, max compression
+gzip compressed data, was "simple_parsing-0.1.2.post1.tar", last modified: Thu Apr 27 19:03:25 2023, max compression
```

## Comparing `simple_parsing-0.1.2.tar` & `simple_parsing-0.1.2.post1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/simple_parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/simple_parsing/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.522964 simple_parsing-0.1.2/simple_parsing/annotation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/annotation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/annotation_utils/get_field_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/help_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.522964 simple_parsing-0.1.2/simple_parsing/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/flatten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.526964 simple_parsing-0.1.2/simple_parsing/helpers/hparams/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/hparam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/hparams/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/nested_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.526964 simple_parsing-0.1.2/simple_parsing/helpers/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/serialization/yaml_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/helpers/subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/replace.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.526964 simple_parsing-0.1.2/simple_parsing/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/dataclass_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/field_metavar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/field_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/field_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/simple_parsing/wrappers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.522964 simple_parsing-0.1.2/simple_parsing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 15:30:25.000000 simple_parsing-0.1.2/simple_parsing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:30:25.530964 simple_parsing-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_bools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_custom_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_default_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_future_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_generation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_huggingface_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_initvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue64.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_107.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_132.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_144.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_46.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_48.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_issue_96.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_optional_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_optional_union.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_positional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_set_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_suppress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_tuples.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/test/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-04-19 15:29:59.000000 simple_parsing-0.1.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/simple_parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/simple_parsing/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.707081 simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/get_field_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/help_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/flatten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/nested_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/yaml_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/dataclass_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_metavar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.707081 simple_parsing-0.1.2.post1/simple_parsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_bools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_custom_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_default_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_future_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_generation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_huggingface_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_initvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_132.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_46.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_96.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_optional_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_optional_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_positional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_set_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_suppress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/versioneer.py
```

### Comparing `simple_parsing-0.1.2/LICENSE` & `simple_parsing-0.1.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/PKG-INFO` & `simple_parsing-0.1.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_parsing
-Version: 0.1.2
+Version: 0.1.2.post1
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.2/README.md` & `simple_parsing-0.1.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/setup.py` & `simple_parsing-0.1.2.post1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/__init__.py` & `simple_parsing-0.1.2.post1/simple_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/annotation_utils/get_field_annotations.py` & `simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/get_field_annotations.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/conflicts.py` & `simple_parsing-0.1.2.post1/simple_parsing/conflicts.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/decorators.py` & `simple_parsing-0.1.2.post1/simple_parsing/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/docstring.py` & `simple_parsing-0.1.2.post1/simple_parsing/docstring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility for retrieveing the docstring of a dataclass's attributes
 @author: Fabrice Normandin
 """
 from __future__ import annotations
 
+import functools
 import inspect
 from dataclasses import dataclass
 from logging import getLogger
 
 import docstring_parser as dp
 from docstring_parser.common import Docstring
 
@@ -91,14 +92,15 @@
                 f"{dataclass} or any of its base classes {','.join(t.__name__ for t in mro[1:])}."
             )
         )
         return AttributeDocString()
     return created_docstring
 
 
+@functools.lru_cache(2048)
 def _get_attribute_docstring(dataclass: type, field_name: str) -> AttributeDocString | None:
     """Gets the AttributeDocString of the given field in the given dataclass.
     Doesn't inspect base classes.
     """
     try:
         source = inspect.getsource(dataclass)
     except (TypeError, OSError) as e:
```

### Comparing `simple_parsing-0.1.2/simple_parsing/help_formatter.py` & `simple_parsing-0.1.2.post1/simple_parsing/help_formatter.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/custom_actions.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/fields.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/flatten.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/flatten.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/hparams/hparam.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hparam.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/hparams/hyperparameters_test.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/hparams/priors_test.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/nested_partial.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/nested_partial.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/partial.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/partial.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/serialization/decoding.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/decoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/serialization/encoding.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/encoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/serialization/serializable.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/serialization/yaml_serialization.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/helpers/subgroups.py` & `simple_parsing-0.1.2.post1/simple_parsing/helpers/subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/parsing.py` & `simple_parsing-0.1.2.post1/simple_parsing/parsing.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/replace.py` & `simple_parsing-0.1.2.post1/simple_parsing/replace.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/utils.py` & `simple_parsing-0.1.2.post1/simple_parsing/utils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/wrappers/dataclass_wrapper.py` & `simple_parsing-0.1.2.post1/simple_parsing/wrappers/dataclass_wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/wrappers/field_metavar.py` & `simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/wrappers/field_parsing.py` & `simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,17 @@
         logger.error(
             f"Couldn't parse value {val}, returning the value as-is. (exceptions: {exceptions})"
         )
         raise ValueError(
             f"Couldn't parse value {val}, returning the value as-is. (exceptions: {exceptions})"
         )
 
-    _try_functions.__name__ = "Try<" + " and ".join(str(func.__name__) for func in funcs) + ">"
+    _try_functions.__name__ = (
+        "Try<" + " and ".join(str(getattr(func, "__name__", func)) for func in funcs) + ">"
+    )
     return _try_functions
 
 
 def parse_union(*types: Type[T]) -> Callable[[Any], Union[T, Any]]:
     types = list(types)
     optional = type(None) in types
     # Partition the Union into None and non-None types.
```

### Comparing `simple_parsing-0.1.2/simple_parsing/wrappers/field_wrapper.py` & `simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing/wrappers/wrapper.py` & `simple_parsing-0.1.2.post1/simple_parsing/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/simple_parsing.egg-info/PKG-INFO` & `simple_parsing-0.1.2.post1/simple_parsing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-parsing
-Version: 0.1.2
+Version: 0.1.2.post1
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.2/simple_parsing.egg-info/SOURCES.txt` & `simple_parsing-0.1.2.post1/simple_parsing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_aliases.py` & `simple_parsing-0.1.2.post1/test/test_aliases.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_base.py` & `simple_parsing-0.1.2.post1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_bools.py` & `simple_parsing-0.1.2.post1/test/test_bools.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_choice.py` & `simple_parsing-0.1.2.post1/test/test_choice.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_conflicts.py` & `simple_parsing-0.1.2.post1/test/test_conflicts.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_custom_args.py` & `simple_parsing-0.1.2.post1/test/test_custom_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_decoding.py` & `simple_parsing-0.1.2.post1/test/test_decoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_decorator.py` & `simple_parsing-0.1.2.post1/test/test_decorator.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_default_args.py` & `simple_parsing-0.1.2.post1/test/test_default_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_docstrings.py` & `simple_parsing-0.1.2.post1/test/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_examples.py` & `simple_parsing-0.1.2.post1/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_fields.py` & `simple_parsing-0.1.2.post1/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_forward_ref.py` & `simple_parsing-0.1.2.post1/test/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_future_annotations.py` & `simple_parsing-0.1.2.post1/test/test_future_annotations.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_generation_mode.py` & `simple_parsing-0.1.2.post1/test/test_generation_mode.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_huggingface_compat.py` & `simple_parsing-0.1.2.post1/test/test_huggingface_compat.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_inheritance.py` & `simple_parsing-0.1.2.post1/test/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_initvar.py` & `simple_parsing-0.1.2.post1/test/test_initvar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_issue64.py` & `simple_parsing-0.1.2.post1/test/test_issue64.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_issue_107.py` & `simple_parsing-0.1.2.post1/test/test_issue_107.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_issue_132.py` & `simple_parsing-0.1.2.post1/test/test_issue_132.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_issue_144.py` & `simple_parsing-0.1.2.post1/test/test_issue_144.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_issue_46.py` & `simple_parsing-0.1.2.post1/test/test_issue_46.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_issue_48.py` & `simple_parsing-0.1.2.post1/test/test_issue_48.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_issue_96.py` & `simple_parsing-0.1.2.post1/test/test_issue_96.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_lists.py` & `simple_parsing-0.1.2.post1/test/test_lists.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_literal.py` & `simple_parsing-0.1.2.post1/test/test_literal.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_multiple.py` & `simple_parsing-0.1.2.post1/test/test_multiple.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_optional.py` & `simple_parsing-0.1.2.post1/test/test_optional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_optional_subparsers.py` & `simple_parsing-0.1.2.post1/test/test_optional_subparsers.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_positional.py` & `simple_parsing-0.1.2.post1/test/test_positional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_replace.py` & `simple_parsing-0.1.2.post1/test/test_replace.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_set_defaults.py` & `simple_parsing-0.1.2.post1/test/test_set_defaults.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_subgroups.py` & `simple_parsing-0.1.2.post1/test/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_subparsers.py` & `simple_parsing-0.1.2.post1/test/test_subparsers.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_suppress.py` & `simple_parsing-0.1.2.post1/test/test_suppress.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_tuples.py` & `simple_parsing-0.1.2.post1/test/test_tuples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_union.py` & `simple_parsing-0.1.2.post1/test/test_union.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/test_utils.py` & `simple_parsing-0.1.2.post1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/test/testutils.py` & `simple_parsing-0.1.2.post1/test/testutils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2/versioneer.py` & `simple_parsing-0.1.2.post1/versioneer.py`

 * *Files identical despite different names*

