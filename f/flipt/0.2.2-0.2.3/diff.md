# Comparing `tmp/flipt-0.2.2.tar.gz` & `tmp/flipt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipt-0.2.2.tar", max compression
+gzip compressed data, was "flipt-0.2.3.tar", max compression
```

## Comparing `flipt-0.2.2.tar` & `flipt-0.2.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0      407 2023-04-12 21:15:30.391660 flipt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2491 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/__init__.py
--rw-r--r--   0        0        0     5307 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/client.py
--rw-r--r--   0        0        0      348 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/__init__.py
--rw-r--r--   0        0        0      326 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      158 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/environment.py
--rw-r--r--   0        0        0        0 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/py.typed
--rw-r--r--   0        0        0     2513 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/__init__.py
--rw-r--r--   0        0        0      261 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/__init__.py
--rw-r--r--   0        0        0     8838 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/client.py
--rw-r--r--   0        0        0      369 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/__init__.py
--rw-r--r--   0        0        0     1128 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication.py
--rw-r--r--   0        0        0      943 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication_list.py
--rw-r--r--   0        0        0      988 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication_method.py
--rw-r--r--   0        0        0     1015 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication_token.py
--rw-r--r--   0        0        0       65 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_k_8_s/__init__.py
--rw-r--r--   0        0        0     2837 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_k_8_s/client.py
--rw-r--r--   0        0        0      195 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/client.py
--rw-r--r--   0        0        0      252 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/__init__.py
--rw-r--r--   0        0        0      854 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py
--rw-r--r--   0        0        0      923 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py
--rw-r--r--   0        0        0       65 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_token/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_token/client.py
--rw-r--r--   0        0        0      117 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/commons/__init__.py
--rw-r--r--   0        0        0      120 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      933 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/commons/types/pageable.py
--rw-r--r--   0        0        0      279 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/__init__.py
--rw-r--r--   0        0        0     6649 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/client.py
--rw-r--r--   0        0        0      399 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint.py
--rw-r--r--   0        0        0     1215 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint_comparison_type.py
--rw-r--r--   0        0        0      913 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint_create_request.py
--rw-r--r--   0        0        0      913 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint_update_request.py
--rw-r--r--   0        0        0      237 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/__init__.py
--rw-r--r--   0        0        0     7184 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/client.py
--rw-r--r--   0        0        0      324 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/distribution.py
--rw-r--r--   0        0        0      868 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/distribution_create_request.py
--rw-r--r--   0        0        0      868 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/distribution_update_request.py
--rw-r--r--   0        0        0      365 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/__init__.py
--rw-r--r--   0        0        0     4878 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/client.py
--rw-r--r--   0        0        0      490 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_request.py
--rw-r--r--   0        0        0     1028 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_response.py
--rw-r--r--   0        0        0     1446 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_reason.py
--rw-r--r--   0        0        0      999 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_request.py
--rw-r--r--   0        0        0     1328 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_response.py
--rw-r--r--   0        0        0      211 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/flags/__init__.py
--rw-r--r--   0        0        0     9920 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/flags/client.py
--rw-r--r--   0        0        0      296 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/__init__.py
--rw-r--r--   0        0        0     1047 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag.py
--rw-r--r--   0        0        0      839 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag_create_request.py
--rw-r--r--   0        0        0      951 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag_list.py
--rw-r--r--   0        0        0      826 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag_update_request.py
--rw-r--r--   0        0        0      251 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/__init__.py
--rw-r--r--   0        0        0     9630 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/client.py
--rw-r--r--   0        0        0      356 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/__init__.py
--rw-r--r--   0        0        0      973 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace.py
--rw-r--r--   0        0        0      809 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_create_request.py
--rw-r--r--   0        0        0      976 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_list.py
--rw-r--r--   0        0        0      796 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_update_request.py
--rw-r--r--   0        0        0      249 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/__init__.py
--rw-r--r--   0        0        0    12302 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/client.py
--rw-r--r--   0        0        0      365 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1142 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule.py
--rw-r--r--   0        0        0      857 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_create_request.py
--rw-r--r--   0        0        0      951 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_list.py
--rw-r--r--   0        0        0      849 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_order_request.py
--rw-r--r--   0        0        0      843 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_update_request.py
--rw-r--r--   0        0        0      273 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/__init__.py
--rw-r--r--   0        0        0    10154 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/client.py
--rw-r--r--   0        0        0      401 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment.py
--rw-r--r--   0        0        0      954 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_create_request.py
--rw-r--r--   0        0        0      966 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_list.py
--rw-r--r--   0        0        0      566 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_match_type.py
--rw-r--r--   0        0        0      941 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_update_request.py
--rw-r--r--   0        0        0      207 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/__init__.py
--rw-r--r--   0        0        0     6568 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/client.py
--rw-r--r--   0        0        0      279 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/__init__.py
--rw-r--r--   0        0        0     1035 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/variant.py
--rw-r--r--   0        0        0      861 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/variant_create_request.py
--rw-r--r--   0        0        0      861 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/variant_update_request.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 flipt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      407 2023-04-27 09:54:13.828655 flipt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2491 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/__init__.py
+-rw-r--r--   0        0        0     5307 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/client.py
+-rw-r--r--   0        0        0      348 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      158 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/environment.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/py.typed
+-rw-r--r--   0        0        0     2513 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/__init__.py
+-rw-r--r--   0        0        0      261 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth/__init__.py
+-rw-r--r--   0        0        0     8838 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth/client.py
+-rw-r--r--   0        0        0      369 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth/types/__init__.py
+-rw-r--r--   0        0        0     1128 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth/types/authentication.py
+-rw-r--r--   0        0        0      943 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth/types/authentication_list.py
+-rw-r--r--   0        0        0      988 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth/types/authentication_method.py
+-rw-r--r--   0        0        0     1015 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth/types/authentication_token.py
+-rw-r--r--   0        0        0       65 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_k_8_s/__init__.py
+-rw-r--r--   0        0        0     2837 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_k_8_s/client.py
+-rw-r--r--   0        0        0      195 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_oidc/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_oidc/client.py
+-rw-r--r--   0        0        0      252 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_oidc/types/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py
+-rw-r--r--   0        0        0      923 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py
+-rw-r--r--   0        0        0       65 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_token/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/auth_method_token/client.py
+-rw-r--r--   0        0        0      117 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/commons/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      933 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/commons/types/pageable.py
+-rw-r--r--   0        0        0      279 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/constraints/__init__.py
+-rw-r--r--   0        0        0     6649 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/constraints/client.py
+-rw-r--r--   0        0        0      399 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/constraints/types/__init__.py
+-rw-r--r--   0        0        0     1127 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/constraints/types/constraint.py
+-rw-r--r--   0        0        0     1215 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/constraints/types/constraint_comparison_type.py
+-rw-r--r--   0        0        0      913 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/constraints/types/constraint_create_request.py
+-rw-r--r--   0        0        0      913 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/constraints/types/constraint_update_request.py
+-rw-r--r--   0        0        0      237 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/distributions/__init__.py
+-rw-r--r--   0        0        0     7184 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/distributions/client.py
+-rw-r--r--   0        0        0      324 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/distributions/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/distributions/types/distribution.py
+-rw-r--r--   0        0        0      868 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/distributions/types/distribution_create_request.py
+-rw-r--r--   0        0        0      868 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/distributions/types/distribution_update_request.py
+-rw-r--r--   0        0        0      365 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/__init__.py
+-rw-r--r--   0        0        0     4878 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/client.py
+-rw-r--r--   0        0        0      490 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/types/batch_evaluation_request.py
+-rw-r--r--   0        0        0     1029 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/types/batch_evaluation_response.py
+-rw-r--r--   0        0        0     1446 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/types/evaluation_reason.py
+-rw-r--r--   0        0        0      999 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/types/evaluation_request.py
+-rw-r--r--   0        0        0     1328 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/evaluate/types/evaluation_response.py
+-rw-r--r--   0        0        0      211 2023-04-27 09:54:13.828655 flipt-0.2.3/src/flipt/resources/flags/__init__.py
+-rw-r--r--   0        0        0     9920 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/flags/client.py
+-rw-r--r--   0        0        0      296 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/flags/types/__init__.py
+-rw-r--r--   0        0        0     1047 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/flags/types/flag.py
+-rw-r--r--   0        0        0      839 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/flags/types/flag_create_request.py
+-rw-r--r--   0        0        0      951 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/flags/types/flag_list.py
+-rw-r--r--   0        0        0      826 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/flags/types/flag_update_request.py
+-rw-r--r--   0        0        0      251 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/namespaces/__init__.py
+-rw-r--r--   0        0        0     9630 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/namespaces/client.py
+-rw-r--r--   0        0        0      356 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/namespaces/types/__init__.py
+-rw-r--r--   0        0        0      973 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/namespaces/types/namespace.py
+-rw-r--r--   0        0        0      809 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/namespaces/types/namespace_create_request.py
+-rw-r--r--   0        0        0      976 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/namespaces/types/namespace_list.py
+-rw-r--r--   0        0        0      796 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/namespaces/types/namespace_update_request.py
+-rw-r--r--   0        0        0      249 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/__init__.py
+-rw-r--r--   0        0        0    12302 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/client.py
+-rw-r--r--   0        0        0      365 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1142 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/types/rule.py
+-rw-r--r--   0        0        0      857 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/types/rule_create_request.py
+-rw-r--r--   0        0        0      951 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/types/rule_list.py
+-rw-r--r--   0        0        0      849 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/types/rule_order_request.py
+-rw-r--r--   0        0        0      843 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/rules/types/rule_update_request.py
+-rw-r--r--   0        0        0      273 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/__init__.py
+-rw-r--r--   0        0        0    10154 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/client.py
+-rw-r--r--   0        0        0      401 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/types/__init__.py
+-rw-r--r--   0        0        0     1165 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/types/segment.py
+-rw-r--r--   0        0        0      954 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/types/segment_create_request.py
+-rw-r--r--   0        0        0      966 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/types/segment_list.py
+-rw-r--r--   0        0        0      566 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/types/segment_match_type.py
+-rw-r--r--   0        0        0      941 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/segments/types/segment_update_request.py
+-rw-r--r--   0        0        0      207 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/variants/__init__.py
+-rw-r--r--   0        0        0     6568 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/variants/client.py
+-rw-r--r--   0        0        0      279 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/variants/types/__init__.py
+-rw-r--r--   0        0        0     1035 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/variants/types/variant.py
+-rw-r--r--   0        0        0      861 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/variants/types/variant_create_request.py
+-rw-r--r--   0        0        0      861 2023-04-27 09:54:13.832655 flipt-0.2.3/src/flipt/resources/variants/types/variant_update_request.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 flipt-0.2.3/PKG-INFO
```

### Comparing `flipt-0.2.2/src/flipt/__init__.py` & `flipt-0.2.3/src/flipt/__init__.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/client.py` & `flipt-0.2.3/src/flipt/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/core/datetime_utils.py` & `flipt-0.2.3/src/flipt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/core/jsonable_encoder.py` & `flipt-0.2.3/src/flipt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/__init__.py` & `flipt-0.2.3/src/flipt/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth/client.py` & `flipt-0.2.3/src/flipt/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth/types/authentication.py` & `flipt-0.2.3/src/flipt/resources/auth/types/authentication.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth/types/authentication_list.py` & `flipt-0.2.3/src/flipt/resources/auth/types/authentication_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth/types/authentication_method.py` & `flipt-0.2.3/src/flipt/resources/auth/types/authentication_method.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth/types/authentication_token.py` & `flipt-0.2.3/src/flipt/resources/auth/types/authentication_token.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth_method_k_8_s/client.py` & `flipt-0.2.3/src/flipt/resources/auth_method_k_8_s/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth_method_oidc/client.py` & `flipt-0.2.3/src/flipt/resources/auth_method_oidc/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py` & `flipt-0.2.3/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py` & `flipt-0.2.3/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/auth_method_token/client.py` & `flipt-0.2.3/src/flipt/resources/auth_method_token/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/commons/types/pageable.py` & `flipt-0.2.3/src/flipt/resources/commons/types/pageable.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/constraints/client.py` & `flipt-0.2.3/src/flipt/resources/constraints/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/constraints/types/constraint.py` & `flipt-0.2.3/src/flipt/resources/constraints/types/constraint.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/constraints/types/constraint_comparison_type.py` & `flipt-0.2.3/src/flipt/resources/constraints/types/constraint_comparison_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/constraints/types/constraint_create_request.py` & `flipt-0.2.3/src/flipt/resources/constraints/types/constraint_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/constraints/types/constraint_update_request.py` & `flipt-0.2.3/src/flipt/resources/constraints/types/constraint_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/distributions/client.py` & `flipt-0.2.3/src/flipt/resources/distributions/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/distributions/types/distribution.py` & `flipt-0.2.3/src/flipt/resources/distributions/types/distribution.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/distributions/types/distribution_create_request.py` & `flipt-0.2.3/src/flipt/resources/distributions/types/distribution_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/distributions/types/distribution_update_request.py` & `flipt-0.2.3/src/flipt/resources/distributions/types/distribution_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/evaluate/client.py` & `flipt-0.2.3/src/flipt/resources/evaluate/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_request.py` & `flipt-0.2.3/src/flipt/resources/evaluate/types/batch_evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_response.py` & `flipt-0.2.3/src/flipt/resources/evaluate/types/batch_evaluation_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ....core.datetime_utils import serialize_datetime
 from .evaluation_response import evaluationResponse
 
 
 class batchEvaluationResponse(pydantic.BaseModel):
     request_id: str = pydantic.Field(alias="requestId")
-    response: typing.List[evaluationResponse]
+    responses: typing.List[evaluationResponse]
     request_duration_millis: float = pydantic.Field(alias="requestDurationMillis")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_reason.py` & `flipt-0.2.3/src/flipt/resources/evaluate/types/evaluation_reason.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_request.py` & `flipt-0.2.3/src/flipt/resources/evaluate/types/evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_response.py` & `flipt-0.2.3/src/flipt/resources/evaluate/types/evaluation_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/flags/client.py` & `flipt-0.2.3/src/flipt/resources/flags/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/flags/types/flag.py` & `flipt-0.2.3/src/flipt/resources/flags/types/flag.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/flags/types/flag_create_request.py` & `flipt-0.2.3/src/flipt/resources/flags/types/flag_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/flags/types/flag_list.py` & `flipt-0.2.3/src/flipt/resources/flags/types/flag_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/flags/types/flag_update_request.py` & `flipt-0.2.3/src/flipt/resources/flags/types/flag_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/namespaces/client.py` & `flipt-0.2.3/src/flipt/resources/namespaces/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace.py` & `flipt-0.2.3/src/flipt/resources/namespaces/types/namespace.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_create_request.py` & `flipt-0.2.3/src/flipt/resources/namespaces/types/namespace_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_list.py` & `flipt-0.2.3/src/flipt/resources/namespaces/types/namespace_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_update_request.py` & `flipt-0.2.3/src/flipt/resources/namespaces/types/namespace_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/rules/client.py` & `flipt-0.2.3/src/flipt/resources/rules/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/rules/types/rule.py` & `flipt-0.2.3/src/flipt/resources/rules/types/rule.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/rules/types/rule_create_request.py` & `flipt-0.2.3/src/flipt/resources/rules/types/rule_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/rules/types/rule_list.py` & `flipt-0.2.3/src/flipt/resources/rules/types/rule_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/rules/types/rule_order_request.py` & `flipt-0.2.3/src/flipt/resources/rules/types/rule_order_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/rules/types/rule_update_request.py` & `flipt-0.2.3/src/flipt/resources/rules/types/rule_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/segments/client.py` & `flipt-0.2.3/src/flipt/resources/segments/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/segments/types/segment.py` & `flipt-0.2.3/src/flipt/resources/segments/types/segment.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/segments/types/segment_create_request.py` & `flipt-0.2.3/src/flipt/resources/segments/types/segment_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/segments/types/segment_list.py` & `flipt-0.2.3/src/flipt/resources/segments/types/segment_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/segments/types/segment_match_type.py` & `flipt-0.2.3/src/flipt/resources/segments/types/segment_match_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/segments/types/segment_update_request.py` & `flipt-0.2.3/src/flipt/resources/segments/types/segment_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/variants/client.py` & `flipt-0.2.3/src/flipt/resources/variants/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/variants/types/variant.py` & `flipt-0.2.3/src/flipt/resources/variants/types/variant.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/variants/types/variant_create_request.py` & `flipt-0.2.3/src/flipt/resources/variants/types/variant_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/src/flipt/resources/variants/types/variant_update_request.py` & `flipt-0.2.3/src/flipt/resources/variants/types/variant_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.2/PKG-INFO` & `flipt-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipt
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

