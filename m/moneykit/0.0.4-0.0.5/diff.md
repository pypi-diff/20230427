# Comparing `tmp/moneykit-0.0.4.tar.gz` & `tmp/moneykit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneykit-0.0.4.tar", last modified: Wed Apr 26 19:41:37 2023, max compression
+gzip compressed data, was "moneykit-0.0.5.tar", max compression
```

## Comparing `moneykit-0.0.4.tar` & `moneykit-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:37.605117 moneykit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-26 19:41:37.605117 moneykit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 19:41:16.000000 moneykit-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:37.601117 moneykit-0.0.4/moneykit/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 19:41:16.000000 moneykit-0.0.4/moneykit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:37.605117 moneykit-0.0.4/moneykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-26 19:41:37.000000 moneykit-0.0.4/moneykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-26 19:41:37.000000 moneykit-0.0.4/moneykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:41:37.000000 moneykit-0.0.4/moneykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 19:41:37.000000 moneykit-0.0.4/moneykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 19:41:37.000000 moneykit-0.0.4/moneykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 19:41:16.000000 moneykit-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 19:41:37.605117 moneykit-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-26 19:41:16.000000 moneykit-0.0.4/setup.py
+-rw-r--r--   0        0        0      267 2023-04-27 11:34:46.000000 moneykit-0.0.5/README.md
+-rw-r--r--   0        0        0    10452 2023-04-27 12:57:29.879022 moneykit-0.0.5/moneykit/__init__.py
+-rw-r--r--   0        0        0      574 2023-04-27 11:35:01.734051 moneykit-0.0.5/moneykit/api/__init__.py
+-rw-r--r--   0        0        0    23590 2023-04-27 11:39:18.921305 moneykit-0.0.5/moneykit/api/access_token_api.py
+-rw-r--r--   0        0        0     8190 2023-04-27 11:35:02.540824 moneykit-0.0.5/moneykit/api/account_numbers_api.py
+-rw-r--r--   0        0        0    32713 2023-04-27 11:35:02.546470 moneykit-0.0.5/moneykit/api/accounts_api.py
+-rw-r--r--   0        0        0     9001 2023-04-27 11:35:02.547779 moneykit-0.0.5/moneykit/api/identity_api.py
+-rw-r--r--   0        0        0    17287 2023-04-27 11:35:02.550100 moneykit-0.0.5/moneykit/api/institutions_api.py
+-rw-r--r--   0        0        0    28888 2023-04-27 11:35:02.550985 moneykit-0.0.5/moneykit/api/links_api.py
+-rw-r--r--   0        0        0    15610 2023-04-27 11:35:02.543465 moneykit-0.0.5/moneykit/api/money_link_api.py
+-rw-r--r--   0        0        0     8760 2023-04-27 11:35:02.540731 moneykit-0.0.5/moneykit/api/products_api.py
+-rw-r--r--   0        0        0    34812 2023-04-27 11:35:02.555073 moneykit-0.0.5/moneykit/api/transactions_api.py
+-rw-r--r--   0        0        0    32182 2023-04-27 11:35:02.547684 moneykit-0.0.5/moneykit/api/users_api.py
+-rw-r--r--   0        0        0    27824 2023-04-27 11:35:02.542924 moneykit-0.0.5/moneykit/api_client.py
+-rw-r--r--   0        0        0    16781 2023-04-27 11:35:02.563727 moneykit-0.0.5/moneykit/configuration.py
+-rw-r--r--   0        0        0     5100 2023-04-27 11:35:01.801893 moneykit-0.0.5/moneykit/exceptions.py
+-rw-r--r--   0        0        0     9481 2023-04-27 11:35:01.846623 moneykit-0.0.5/moneykit/models/__init__.py
+-rw-r--r--   0        0        0     3780 2023-04-27 11:35:02.550296 moneykit-0.0.5/moneykit/models/account_balances.py
+-rw-r--r--   0        0        0     2888 2023-04-27 11:35:02.545611 moneykit-0.0.5/moneykit/models/account_group.py
+-rw-r--r--   0        0        0     4250 2023-04-27 11:35:02.555317 moneykit-0.0.5/moneykit/models/account_identity.py
+-rw-r--r--   0        0        0     2400 2023-04-27 11:35:02.559523 moneykit-0.0.5/moneykit/models/account_numbers.py
+-rw-r--r--   0        0        0     3290 2023-04-27 11:35:02.545290 moneykit-0.0.5/moneykit/models/account_numbers_link_product.py
+-rw-r--r--   0        0        0     2520 2023-04-27 11:35:02.545049 moneykit-0.0.5/moneykit/models/account_numbers_product_settings.py
+-rw-r--r--   0        0        0      916 2023-04-27 11:35:02.550187 moneykit-0.0.5/moneykit/models/account_type.py
+-rw-r--r--   0        0        0     4068 2023-04-27 11:35:02.556391 moneykit-0.0.5/moneykit/models/account_with_account_numbers.py
+-rw-r--r--   0        0        0     2705 2023-04-27 11:35:02.547527 moneykit-0.0.5/moneykit/models/accounts_link_product.py
+-rw-r--r--   0        0        0     2459 2023-04-27 11:35:02.548730 moneykit-0.0.5/moneykit/models/ach_number.py
+-rw-r--r--   0        0        0     3720 2023-04-27 11:35:02.560613 moneykit-0.0.5/moneykit/models/address.py
+-rw-r--r--   0        0        0     2950 2023-04-27 11:35:02.550796 moneykit-0.0.5/moneykit/models/api_client_out.py
+-rw-r--r--   0        0        0     3148 2023-04-27 11:35:02.560510 moneykit-0.0.5/moneykit/models/api_error_auth_expired_access_token_response.py
+-rw-r--r--   0        0        0     2939 2023-04-27 11:35:02.551042 moneykit-0.0.5/moneykit/models/api_error_auth_unauthorized_response.py
+-rw-r--r--   0        0        0     3082 2023-04-27 11:35:02.549594 moneykit-0.0.5/moneykit/models/api_error_rate_limit_exceeded_response.py
+-rw-r--r--   0        0        0     1824 2023-04-27 11:35:02.552253 moneykit-0.0.5/moneykit/models/app.py
+-rw-r--r--   0        0        0     3751 2023-04-27 11:35:02.552092 moneykit-0.0.5/moneykit/models/app_api_public_accounts_account_out.py
+-rw-r--r--   0        0        0     3232 2023-04-27 11:35:02.554445 moneykit-0.0.5/moneykit/models/app_api_public_users_transactions_account_out.py
+-rw-r--r--   0        0        0     1897 2023-04-27 11:35:02.556983 moneykit-0.0.5/moneykit/models/bacs_number.py
+-rw-r--r--   0        0        0     3942 2023-04-27 11:35:02.540386 moneykit-0.0.5/moneykit/models/balances.py
+-rw-r--r--   0        0        0      518 2023-04-27 11:39:18.921514 moneykit-0.0.5/moneykit/models/country.py
+-rw-r--r--   0        0        0     5363 2023-04-27 11:35:02.558860 moneykit-0.0.5/moneykit/models/create_link_session_body.py
+-rw-r--r--   0        0        0     1943 2023-04-27 11:35:02.553289 moneykit-0.0.5/moneykit/models/create_link_session_response.py
+-rw-r--r--   0        0        0     3569 2023-04-27 11:35:02.551603 moneykit-0.0.5/moneykit/models/currency.py
+-rw-r--r--   0        0        0     1987 2023-04-27 11:39:18.921686 moneykit-0.0.5/moneykit/models/cursor.py
+-rw-r--r--   0        0        0     2051 2023-04-27 11:35:02.558780 moneykit-0.0.5/moneykit/models/cursor_pagination.py
+-rw-r--r--   0        0        0     1995 2023-04-27 11:35:02.555943 moneykit-0.0.5/moneykit/models/cursors.py
+-rw-r--r--   0        0        0     1907 2023-04-27 11:35:02.546802 moneykit-0.0.5/moneykit/models/customer_app_out.py
+-rw-r--r--   0        0        0     3533 2023-04-27 11:35:02.553691 moneykit-0.0.5/moneykit/models/customer_user.py
+-rw-r--r--   0        0        0     2155 2023-04-27 11:35:02.547890 moneykit-0.0.5/moneykit/models/eft_number.py
+-rw-r--r--   0        0        0     2030 2023-04-27 11:35:02.553433 moneykit-0.0.5/moneykit/models/email.py
+-rw-r--r--   0        0        0     2978 2023-04-27 11:35:02.557397 moneykit-0.0.5/moneykit/models/email1.py
+-rw-r--r--   0        0        0     1919 2023-04-27 11:39:18.921969 moneykit-0.0.5/moneykit/models/exchange_token_body.py
+-rw-r--r--   0        0        0     1862 2023-04-27 11:35:02.560138 moneykit-0.0.5/moneykit/models/exchange_token_response.py
+-rw-r--r--   0        0        0     2788 2023-04-27 11:35:02.560702 moneykit-0.0.5/moneykit/models/get_account_numbers_response.py
+-rw-r--r--   0        0        0     2528 2023-04-27 11:35:02.549618 moneykit-0.0.5/moneykit/models/get_account_response.py
+-rw-r--r--   0        0        0     2775 2023-04-27 11:39:18.922205 moneykit-0.0.5/moneykit/models/get_accounts_response.py
+-rw-r--r--   0        0        0     3974 2023-04-27 11:35:02.550492 moneykit-0.0.5/moneykit/models/get_transactions_response.py
+-rw-r--r--   0        0        0     3696 2023-04-27 11:35:02.543788 moneykit-0.0.5/moneykit/models/http_validation_error.py
+-rw-r--r--   0        0        0     2352 2023-04-27 11:35:02.551706 moneykit-0.0.5/moneykit/models/identity.py
+-rw-r--r--   0        0        0     3217 2023-04-27 11:35:02.549625 moneykit-0.0.5/moneykit/models/identity_link_product.py
+-rw-r--r--   0        0        0     2472 2023-04-27 11:35:02.552832 moneykit-0.0.5/moneykit/models/identity_product_settings.py
+-rw-r--r--   0        0        0     2748 2023-04-27 11:35:02.540595 moneykit-0.0.5/moneykit/models/identity_response.py
+-rw-r--r--   0        0        0     3027 2023-04-27 11:35:02.555220 moneykit-0.0.5/moneykit/models/institution_error_not_found_response.py
+-rw-r--r--   0        0        0     3375 2023-04-27 11:35:02.547467 moneykit-0.0.5/moneykit/models/institution_out.py
+-rw-r--r--   0        0        0     1889 2023-04-27 11:35:02.556550 moneykit-0.0.5/moneykit/models/international_number.py
+-rw-r--r--   0        0        0     1779 2023-04-27 11:35:02.541899 moneykit-0.0.5/moneykit/models/jwk_set.py
+-rw-r--r--   0        0        0     3777 2023-04-27 11:35:02.558161 moneykit-0.0.5/moneykit/models/link.py
+-rw-r--r--   0        0        0     3786 2023-04-27 11:35:02.548862 moneykit-0.0.5/moneykit/models/link1.py
+-rw-r--r--   0        0        0     3782 2023-04-27 11:35:02.544818 moneykit-0.0.5/moneykit/models/link2.py
+-rw-r--r--   0        0        0     3786 2023-04-27 11:35:02.557116 moneykit-0.0.5/moneykit/models/link3.py
+-rw-r--r--   0        0        0      724 2023-04-27 11:35:02.558581 moneykit-0.0.5/moneykit/models/link_error.py
+-rw-r--r--   0        0        0     2885 2023-04-27 11:35:02.551936 moneykit-0.0.5/moneykit/models/link_error_bad_state_response.py
+-rw-r--r--   0        0        0     2845 2023-04-27 11:35:02.540325 moneykit-0.0.5/moneykit/models/link_error_deleted_response.py
+-rw-r--r--   0        0        0     2939 2023-04-27 11:35:02.546086 moneykit-0.0.5/moneykit/models/link_error_forbidden_action_response.py
+-rw-r--r--   0        0        0     2899 2023-04-27 11:35:02.554972 moneykit-0.0.5/moneykit/models/link_error_not_found_response.py
+-rw-r--r--   0        0        0     3071 2023-04-27 11:35:02.560384 moneykit-0.0.5/moneykit/models/link_error_unauthorized_access_response.py
+-rw-r--r--   0        0        0     3812 2023-04-27 11:35:02.558586 moneykit-0.0.5/moneykit/models/link_out_common.py
+-rw-r--r--   0        0        0     4377 2023-04-27 11:35:02.553519 moneykit-0.0.5/moneykit/models/link_out_full.py
+-rw-r--r--   0        0        0      667 2023-04-27 11:35:02.541343 moneykit-0.0.5/moneykit/models/link_permission_scope.py
+-rw-r--r--   0        0        0     2627 2023-04-27 11:35:02.552705 moneykit-0.0.5/moneykit/models/link_permissions.py
+-rw-r--r--   0        0        0     3680 2023-04-27 11:35:02.542665 moneykit-0.0.5/moneykit/models/link_products.py
+-rw-r--r--   0        0        0     3392 2023-04-27 11:35:02.540392 moneykit-0.0.5/moneykit/models/link_session_customer_user.py
+-rw-r--r--   0        0        0     3000 2023-04-27 11:35:02.558913 moneykit-0.0.5/moneykit/models/link_session_customer_user_email.py
+-rw-r--r--   0        0        0     3464 2023-04-27 11:35:02.544503 moneykit-0.0.5/moneykit/models/link_session_customer_user_phone.py
+-rw-r--r--   0        0        0     3027 2023-04-27 11:35:02.543402 moneykit-0.0.5/moneykit/models/link_session_error_forbidden_config_response.py
+-rw-r--r--   0        0        0     3027 2023-04-27 11:35:02.542420 moneykit-0.0.5/moneykit/models/link_session_error_invalid_token_exchange.py
+-rw-r--r--   0        0        0      636 2023-04-27 11:35:02.559318 moneykit-0.0.5/moneykit/models/link_state.py
+-rw-r--r--   0        0        0     4499 2023-04-27 11:35:02.545064 moneykit-0.0.5/moneykit/models/link_state_changed_webhook.py
+-rw-r--r--   0        0        0     3767 2023-04-27 11:35:02.556600 moneykit-0.0.5/moneykit/models/location_inner.py
+-rw-r--r--   0        0        0      534 2023-04-27 11:35:02.542312 moneykit-0.0.5/moneykit/models/money_kit_env.py
+-rw-r--r--   0        0        0     2360 2023-04-27 11:35:02.555425 moneykit-0.0.5/moneykit/models/money_link_features.py
+-rw-r--r--   0        0        0     2384 2023-04-27 11:35:02.556121 moneykit-0.0.5/moneykit/models/moneylink_features.py
+-rw-r--r--   0        0        0     4104 2023-04-27 11:35:02.553866 moneykit-0.0.5/moneykit/models/numbers.py
+-rw-r--r--   0        0        0     3805 2023-04-27 11:35:02.549404 moneykit-0.0.5/moneykit/models/owner.py
+-rw-r--r--   0        0        0     2840 2023-04-27 11:35:02.559666 moneykit-0.0.5/moneykit/models/paged_institution_response.py
+-rw-r--r--   0        0        0     3441 2023-04-27 11:35:02.554595 moneykit-0.0.5/moneykit/models/phone.py
+-rw-r--r--   0        0        0     2262 2023-04-27 11:35:02.555014 moneykit-0.0.5/moneykit/models/phone_number.py
+-rw-r--r--   0        0        0      562 2023-04-27 11:35:02.559606 moneykit-0.0.5/moneykit/models/phone_number_type.py
+-rw-r--r--   0        0        0      625 2023-04-27 11:35:02.540938 moneykit-0.0.5/moneykit/models/product.py
+-rw-r--r--   0        0        0     3685 2023-04-27 11:35:02.556322 moneykit-0.0.5/moneykit/models/products.py
+-rw-r--r--   0        0        0     3105 2023-04-27 11:35:02.556981 moneykit-0.0.5/moneykit/models/products1.py
+-rw-r--r--   0        0        0     3083 2023-04-27 11:35:02.547688 moneykit-0.0.5/moneykit/models/products_settings.py
+-rw-r--r--   0        0        0      585 2023-04-27 11:35:02.552566 moneykit-0.0.5/moneykit/models/provider.py
+-rw-r--r--   0        0        0     2011 2023-04-27 11:35:02.544218 moneykit-0.0.5/moneykit/models/refresh_products_body.py
+-rw-r--r--   0        0        0     2616 2023-04-27 11:35:02.558995 moneykit-0.0.5/moneykit/models/requested_link_permission.py
+-rw-r--r--   0        0        0     5403 2023-04-27 11:35:02.552070 moneykit-0.0.5/moneykit/models/response401_disconnect_links_id_delete.py
+-rw-r--r--   0        0        0     4608 2023-04-27 11:35:02.546355 moneykit-0.0.5/moneykit/models/response401_exchange_token_link_session_exchange_token_post.py
+-rw-r--r--   0        0        0     5515 2023-04-27 11:35:02.549870 moneykit-0.0.5/moneykit/models/response401_get_account_links_id_accounts_account_id_get.py
+-rw-r--r--   0        0        0     5555 2023-04-27 11:35:02.555649 moneykit-0.0.5/moneykit/models/response401_get_account_numbers_links_id_accounts_numbers_get.py
+-rw-r--r--   0        0        0     5451 2023-04-27 11:35:02.551127 moneykit-0.0.5/moneykit/models/response401_get_accounts_links_id_accounts_get.py
+-rw-r--r--   0        0        0     5467 2023-04-27 11:35:02.553396 moneykit-0.0.5/moneykit/models/response401_get_identities_links_id_identity_get.py
+-rw-r--r--   0        0        0     4616 2023-04-27 11:35:02.557416 moneykit-0.0.5/moneykit/models/response401_get_institution_institutions_institution_id_get.py
+-rw-r--r--   0        0        0     4520 2023-04-27 11:35:02.548409 moneykit-0.0.5/moneykit/models/response401_get_institutions_institutions_get.py
+-rw-r--r--   0        0        0     5355 2023-04-27 11:35:02.541719 moneykit-0.0.5/moneykit/models/response401_get_link_links_id_get.py
+-rw-r--r--   0        0        0     5593 2023-04-27 11:35:02.556219 moneykit-0.0.5/moneykit/models/response401_get_transactions_diff_links_id_transactions_sync_get.py
+-rw-r--r--   0        0        0     5515 2023-04-27 11:35:02.542230 moneykit-0.0.5/moneykit/models/response401_get_transactions_links_id_transactions_get.py
+-rw-r--r--   0        0        0     4544 2023-04-27 11:35:02.549999 moneykit-0.0.5/moneykit/models/response401_get_user_accounts_users_id_accounts_get.py
+-rw-r--r--   0        0        0     4496 2023-04-27 11:35:02.551226 moneykit-0.0.5/moneykit/models/response401_get_user_links_users_id_links_get.py
+-rw-r--r--   0        0        0     4608 2023-04-27 11:35:02.546557 moneykit-0.0.5/moneykit/models/response401_get_user_transactions_users_id_transactions_get.py
+-rw-r--r--   0        0        0     4568 2023-04-27 11:35:02.548254 moneykit-0.0.5/moneykit/models/response401_get_well_known_jwks_well_known_jwks_json_get.py
+-rw-r--r--   0        0        0     4552 2023-04-27 11:35:02.548709 moneykit-0.0.5/moneykit/models/response401_instrospect_client_auth_introspect_get.py
+-rw-r--r--   0        0        0     5491 2023-04-27 11:35:02.552188 moneykit-0.0.5/moneykit/models/response401_refresh_products_links_id_products_post.py
+-rw-r--r--   0        0        0     5395 2023-04-27 11:35:02.558231 moneykit-0.0.5/moneykit/models/response401_update_link_links_id_patch.py
+-rw-r--r--   0        0        0     4160 2023-04-27 11:35:02.555146 moneykit-0.0.5/moneykit/models/setting_overrides.py
+-rw-r--r--   0        0        0     4169 2023-04-27 11:35:02.544318 moneykit-0.0.5/moneykit/models/settings.py
+-rw-r--r--   0        0        0      532 2023-04-27 11:35:02.543657 moneykit-0.0.5/moneykit/models/supported_version.py
+-rw-r--r--   0        0        0     2133 2023-04-27 11:35:02.554143 moneykit-0.0.5/moneykit/models/token.py
+-rw-r--r--   0        0        0     5024 2023-04-27 11:35:02.557613 moneykit-0.0.5/moneykit/models/transaction.py
+-rw-r--r--   0        0        0     3299 2023-04-27 11:35:02.541802 moneykit-0.0.5/moneykit/models/transaction_diff.py
+-rw-r--r--   0        0        0     3253 2023-04-27 11:35:02.547055 moneykit-0.0.5/moneykit/models/transaction_sync_response.py
+-rw-r--r--   0        0        0      526 2023-04-27 11:35:02.552454 moneykit-0.0.5/moneykit/models/transaction_type.py
+-rw-r--r--   0        0        0      532 2023-04-27 11:35:02.547566 moneykit-0.0.5/moneykit/models/transaction_type_filter.py
+-rw-r--r--   0        0        0     2818 2023-04-27 11:35:02.558331 moneykit-0.0.5/moneykit/models/transactions.py
+-rw-r--r--   0        0        0     3320 2023-04-27 11:35:02.540818 moneykit-0.0.5/moneykit/models/transactions1.py
+-rw-r--r--   0        0        0     3265 2023-04-27 11:35:02.554325 moneykit-0.0.5/moneykit/models/transactions_link_product.py
+-rw-r--r--   0        0        0     2938 2023-04-27 11:35:02.543159 moneykit-0.0.5/moneykit/models/transactions_product_settings.py
+-rw-r--r--   0        0        0     2529 2023-04-27 11:35:02.546257 moneykit-0.0.5/moneykit/models/update_link_body.py
+-rw-r--r--   0        0        0     2485 2023-04-27 11:35:02.542597 moneykit-0.0.5/moneykit/models/user_accounts_out.py
+-rw-r--r--   0        0        0     2444 2023-04-27 11:35:02.546203 moneykit-0.0.5/moneykit/models/user_links_out.py
+-rw-r--r--   0        0        0     3730 2023-04-27 11:35:02.545567 moneykit-0.0.5/moneykit/models/user_transactions_paged_response.py
+-rw-r--r--   0        0        0     2475 2023-04-27 11:35:02.554671 moneykit-0.0.5/moneykit/models/validation_error.py
+-rw-r--r--   0        0        0      963 2023-04-27 11:35:11.820343 moneykit-0.0.5/moneykit/plaid_compatible/__init__.py
+-rw-r--r--   0        0        0      227 2023-04-27 11:35:11.854087 moneykit-0.0.5/moneykit/plaid_compatible/api/__init__.py
+-rw-r--r--   0        0        0    50030 2023-04-27 11:35:11.854973 moneykit-0.0.5/moneykit/plaid_compatible/api/plaid_api.py
+-rw-r--r--   0        0        0    36839 2023-04-27 11:35:11.855928 moneykit-0.0.5/moneykit/plaid_compatible/api_client.py
+-rw-r--r--   0        0        0      470 2023-04-27 11:35:11.819804 moneykit-0.0.5/moneykit/plaid_compatible/apis/__init__.py
+-rw-r--r--   0        0        0    17735 2023-04-27 11:35:11.819610 moneykit-0.0.5/moneykit/plaid_compatible/configuration.py
+-rw-r--r--   0        0        0     5093 2023-04-27 11:35:11.855324 moneykit-0.0.5/moneykit/plaid_compatible/exceptions.py
+-rw-r--r--   0        0        0      348 2023-04-27 11:35:11.833066 moneykit-0.0.5/moneykit/plaid_compatible/model/__init__.py
+-rw-r--r--   0        0        0    10890 2023-04-27 11:35:11.839671 moneykit-0.0.5/moneykit/plaid_compatible/model/account_balance.py
+-rw-r--r--   0        0        0    10741 2023-04-27 11:35:11.836341 moneykit-0.0.5/moneykit/plaid_compatible/model/account_base.py
+-rw-r--r--   0        0        0    11657 2023-04-27 11:35:11.830291 moneykit-0.0.5/moneykit/plaid_compatible/model/account_identity.py
+-rw-r--r--   0        0        0    11414 2023-04-27 11:35:11.835673 moneykit-0.0.5/moneykit/plaid_compatible/model/account_subtype.py
+-rw-r--r--   0        0        0     7191 2023-04-27 11:35:11.850620 moneykit-0.0.5/moneykit/plaid_compatible/model/account_type.py
+-rw-r--r--   0        0        0     7674 2023-04-27 11:35:11.836650 moneykit-0.0.5/moneykit/plaid_compatible/model/accounts_get_request.py
+-rw-r--r--   0        0        0     6636 2023-04-27 11:35:11.847676 moneykit-0.0.5/moneykit/plaid_compatible/model/accounts_get_request_options.py
+-rw-r--r--   0        0        0     7447 2023-04-27 11:35:11.843173 moneykit-0.0.5/moneykit/plaid_compatible/model/accounts_get_response.py
+-rw-r--r--   0        0        0     6925 2023-04-27 11:35:11.822805 moneykit-0.0.5/moneykit/plaid_compatible/model/address.py
+-rw-r--r--   0        0        0     7501 2023-04-27 11:35:11.837882 moneykit-0.0.5/moneykit/plaid_compatible/model/address_data.py
+-rw-r--r--   0        0        0     7793 2023-04-27 11:35:11.848070 moneykit-0.0.5/moneykit/plaid_compatible/model/auth_get_numbers.py
+-rw-r--r--   0        0        0     7642 2023-04-27 11:35:11.846341 moneykit-0.0.5/moneykit/plaid_compatible/model/auth_get_request.py
+-rw-r--r--   0        0        0     6715 2023-04-27 11:35:11.836010 moneykit-0.0.5/moneykit/plaid_compatible/model/auth_get_request_options.py
+-rw-r--r--   0        0        0     7635 2023-04-27 11:35:11.852862 moneykit-0.0.5/moneykit/plaid_compatible/model/auth_get_response.py
+-rw-r--r--   0        0        0     7265 2023-04-27 11:35:11.824943 moneykit-0.0.5/moneykit/plaid_compatible/model/counterparty_type.py
+-rw-r--r--   0        0        0     6955 2023-04-27 11:35:11.848478 moneykit-0.0.5/moneykit/plaid_compatible/model/country_code.py
+-rw-r--r--   0        0        0     7029 2023-04-27 11:35:11.825241 moneykit-0.0.5/moneykit/plaid_compatible/model/credit_account_subtype.py
+-rw-r--r--   0        0        0     7070 2023-04-27 11:35:11.822110 moneykit-0.0.5/moneykit/plaid_compatible/model/credit_filter.py
+-rw-r--r--   0        0        0     7417 2023-04-27 11:35:11.844709 moneykit-0.0.5/moneykit/plaid_compatible/model/depository_account_subtype.py
+-rw-r--r--   0        0        0     7102 2023-04-27 11:35:11.846860 moneykit-0.0.5/moneykit/plaid_compatible/model/depository_filter.py
+-rw-r--r--   0        0        0     6966 2023-04-27 11:35:11.841239 moneykit-0.0.5/moneykit/plaid_compatible/model/email.py
+-rw-r--r--   0        0        0     6965 2023-04-27 11:35:11.853184 moneykit-0.0.5/moneykit/plaid_compatible/model/employment_source_type.py
+-rw-r--r--   0        0        0     6724 2023-04-27 11:35:11.837517 moneykit-0.0.5/moneykit/plaid_compatible/model/http_validation_error.py
+-rw-r--r--   0        0        0     9101 2023-04-27 11:35:11.841559 moneykit-0.0.5/moneykit/plaid_compatible/model/id_number_type.py
+-rw-r--r--   0        0        0     7674 2023-04-27 11:35:11.843482 moneykit-0.0.5/moneykit/plaid_compatible/model/identity_get_request.py
+-rw-r--r--   0        0        0     6723 2023-04-27 11:35:11.844382 moneykit-0.0.5/moneykit/plaid_compatible/model/identity_get_request_options.py
+-rw-r--r--   0        0        0     7362 2023-04-27 11:35:11.842158 moneykit-0.0.5/moneykit/plaid_compatible/model/identity_get_response.py
+-rw-r--r--   0        0        0     7111 2023-04-27 11:35:11.824335 moneykit-0.0.5/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py
+-rw-r--r--   0        0        0     6981 2023-04-27 11:35:11.826706 moneykit-0.0.5/moneykit/plaid_compatible/model/income_verification_source_type.py
+-rw-r--r--   0        0        0     9913 2023-04-27 11:35:11.850917 moneykit-0.0.5/moneykit/plaid_compatible/model/investment_account_subtype.py
+-rw-r--r--   0        0        0     7102 2023-04-27 11:35:11.839019 moneykit-0.0.5/moneykit/plaid_compatible/model/investment_filter.py
+-rw-r--r--   0        0        0    10420 2023-04-27 11:35:11.852347 moneykit-0.0.5/moneykit/plaid_compatible/model/item.py
+-rw-r--r--   0        0        0     7717 2023-04-27 11:35:11.836929 moneykit-0.0.5/moneykit/plaid_compatible/model/item_error_webhook.py
+-rw-r--r--   0        0        0     7265 2023-04-27 11:35:11.840950 moneykit-0.0.5/moneykit/plaid_compatible/model/item_get_request.py
+-rw-r--r--   0        0        0     7287 2023-04-27 11:35:11.824057 moneykit-0.0.5/moneykit/plaid_compatible/model/item_get_response.py
+-rw-r--r--   0        0        0     7331 2023-04-27 11:35:11.841878 moneykit-0.0.5/moneykit/plaid_compatible/model/item_public_token_exchange_request.py
+-rw-r--r--   0        0        0     7235 2023-04-27 11:35:11.853485 moneykit-0.0.5/moneykit/plaid_compatible/model/item_public_token_exchange_response.py
+-rw-r--r--   0        0        0     7271 2023-04-27 11:35:11.825784 moneykit-0.0.5/moneykit/plaid_compatible/model/item_remove_request.py
+-rw-r--r--   0        0        0     6715 2023-04-27 11:35:11.849531 moneykit-0.0.5/moneykit/plaid_compatible/model/item_remove_response.py
+-rw-r--r--   0        0        0     7362 2023-04-27 11:35:11.847285 moneykit-0.0.5/moneykit/plaid_compatible/model/item_status_investments.py
+-rw-r--r--   0        0        0     6852 2023-04-27 11:35:11.838677 moneykit-0.0.5/moneykit/plaid_compatible/model/item_status_last_webhook.py
+-rw-r--r--   0        0        0     7489 2023-04-27 11:35:11.845090 moneykit-0.0.5/moneykit/plaid_compatible/model/item_status_nullable.py
+-rw-r--r--   0        0        0     7366 2023-04-27 11:35:11.828455 moneykit-0.0.5/moneykit/plaid_compatible/model/item_status_transactions.py
+-rw-r--r--   0        0        0     7595 2023-04-27 11:35:11.851218 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_account_filters.py
+-rw-r--r--   0        0        0     6644 2023-04-27 11:35:11.835353 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_institution_data.py
+-rw-r--r--   0        0        0    21548 2023-04-27 11:35:11.849967 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request.py
+-rw-r--r--   0        0        0     8258 2023-04-27 11:35:11.823705 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_auth.py
+-rw-r--r--   0        0        0     6733 2023-04-27 11:35:11.829894 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py
+-rw-r--r--   0        0        0     7534 2023-04-27 11:35:11.830663 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_employment.py
+-rw-r--r--   0        0        0     6722 2023-04-27 11:35:11.832528 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py
+-rw-r--r--   0        0        0     7661 2023-04-27 11:35:11.840337 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py
+-rw-r--r--   0        0        0    10586 2023-04-27 11:35:11.848899 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py
+-rw-r--r--   0        0        0     7020 2023-04-27 11:35:11.820927 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py
+-rw-r--r--   0        0        0     7697 2023-04-27 11:35:11.831311 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py
+-rw-r--r--   0        0        0     6937 2023-04-27 11:35:11.821785 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py
+-rw-r--r--   0        0        0     6940 2023-04-27 11:35:11.839332 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_transfer.py
+-rw-r--r--   0        0        0     6779 2023-04-27 11:35:11.828113 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_update.py
+-rw-r--r--   0        0        0    11399 2023-04-27 11:35:11.822453 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_user.py
+-rw-r--r--   0        0        0     6963 2023-04-27 11:35:11.851479 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_user_name.py
+-rw-r--r--   0        0        0     8414 2023-04-27 11:35:11.827722 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py
+-rw-r--r--   0        0        0     7615 2023-04-27 11:35:11.831602 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_create_response.py
+-rw-r--r--   0        0        0     6616 2023-04-27 11:35:11.844044 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_eu_config.py
+-rw-r--r--   0        0        0     6769 2023-04-27 11:35:11.852018 moneykit-0.0.5/moneykit/plaid_compatible/model/link_token_investments.py
+-rw-r--r--   0        0        0     7573 2023-04-27 11:35:11.831003 moneykit-0.0.5/moneykit/plaid_compatible/model/loan_account_subtype.py
+-rw-r--r--   0        0        0     7054 2023-04-27 11:35:11.834211 moneykit-0.0.5/moneykit/plaid_compatible/model/loan_filter.py
+-rw-r--r--   0        0        0     7487 2023-04-27 11:35:11.838245 moneykit-0.0.5/moneykit/plaid_compatible/model/location.py
+-rw-r--r--   0        0        0     7716 2023-04-27 11:35:11.833608 moneykit-0.0.5/moneykit/plaid_compatible/model/money_link_features.py
+-rw-r--r--   0        0        0     8621 2023-04-27 11:35:11.849245 moneykit-0.0.5/moneykit/plaid_compatible/model/numbers_ach.py
+-rw-r--r--   0        0        0     7019 2023-04-27 11:35:11.827039 moneykit-0.0.5/moneykit/plaid_compatible/model/numbers_bacs.py
+-rw-r--r--   0        0        0     7225 2023-04-27 11:35:11.832844 moneykit-0.0.5/moneykit/plaid_compatible/model/numbers_eft.py
+-rw-r--r--   0        0        0     7007 2023-04-27 11:35:11.837232 moneykit-0.0.5/moneykit/plaid_compatible/model/numbers_international.py
+-rw-r--r--   0        0        0     8304 2023-04-27 11:35:11.834513 moneykit-0.0.5/moneykit/plaid_compatible/model/owner.py
+-rw-r--r--   0        0        0     7593 2023-04-27 11:35:11.821448 moneykit-0.0.5/moneykit/plaid_compatible/model/payment_meta.py
+-rw-r--r--   0        0        0     6930 2023-04-27 11:35:11.825524 moneykit-0.0.5/moneykit/plaid_compatible/model/personal_finance_category.py
+-rw-r--r--   0        0        0     6934 2023-04-27 11:35:11.831943 moneykit-0.0.5/moneykit/plaid_compatible/model/phone_number.py
+-rw-r--r--   0        0        0     9494 2023-04-27 11:35:11.853840 moneykit-0.0.5/moneykit/plaid_compatible/model/plaid_error.py
+-rw-r--r--   0        0        0     8113 2023-04-27 11:35:11.823138 moneykit-0.0.5/moneykit/plaid_compatible/model/plaid_error_type.py
+-rw-r--r--   0        0        0     7129 2023-04-27 11:35:11.833325 moneykit-0.0.5/moneykit/plaid_compatible/model/products.py
+-rw-r--r--   0        0        0     6610 2023-04-27 11:35:11.823415 moneykit-0.0.5/moneykit/plaid_compatible/model/removed_transaction.py
+-rw-r--r--   0        0        0    16756 2023-04-27 11:35:11.829250 moneykit-0.0.5/moneykit/plaid_compatible/model/transaction.py
+-rw-r--r--   0        0        0     7632 2023-04-27 11:35:11.833930 moneykit-0.0.5/moneykit/plaid_compatible/model/transaction_code.py
+-rw-r--r--   0        0        0     7510 2023-04-27 11:35:11.826412 moneykit-0.0.5/moneykit/plaid_compatible/model/transaction_counterparty.py
+-rw-r--r--   0        0        0     8236 2023-04-27 11:35:11.842444 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_get_request.py
+-rw-r--r--   0        0        0     9639 2023-04-27 11:35:11.840024 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_get_request_options.py
+-rw-r--r--   0        0        0     8530 2023-04-27 11:35:11.845536 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_get_response.py
+-rw-r--r--   0        0        0     7289 2023-04-27 11:35:11.851751 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_refresh_request.py
+-rw-r--r--   0        0        0     6733 2023-04-27 11:35:11.824599 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_refresh_response.py
+-rw-r--r--   0        0        0     8397 2023-04-27 11:35:11.842794 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_sync_request.py
+-rw-r--r--   0        0        0     8427 2023-04-27 11:35:11.845971 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_sync_request_options.py
+-rw-r--r--   0        0        0     8900 2023-04-27 11:35:11.835062 moneykit-0.0.5/moneykit/plaid_compatible/model/transactions_sync_response.py
+-rw-r--r--   0        0        0     7916 2023-04-27 11:35:11.840648 moneykit-0.0.5/moneykit/plaid_compatible/model/user_address.py
+-rw-r--r--   0        0        0     6950 2023-04-27 11:35:11.843772 moneykit-0.0.5/moneykit/plaid_compatible/model/user_id_number.py
+-rw-r--r--   0        0        0     7625 2023-04-27 11:35:11.850269 moneykit-0.0.5/moneykit/plaid_compatible/model/user_stated_income_source_category.py
+-rw-r--r--   0        0        0     7187 2023-04-27 11:35:11.827407 moneykit-0.0.5/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py
+-rw-r--r--   0        0        0     7027 2023-04-27 11:35:11.832247 moneykit-0.0.5/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py
+-rw-r--r--   0        0        0     6793 2023-04-27 11:35:11.826107 moneykit-0.0.5/moneykit/plaid_compatible/model/validation_error.py
+-rw-r--r--   0        0        0     7069 2023-04-27 11:35:11.829579 moneykit-0.0.5/moneykit/plaid_compatible/model/webhook_environment_values.py
+-rw-r--r--   0        0        0    74795 2023-04-27 11:35:11.819140 moneykit-0.0.5/moneykit/plaid_compatible/model_utils.py
+-rw-r--r--   0        0        0     8892 2023-04-27 11:35:11.820594 moneykit-0.0.5/moneykit/plaid_compatible/models/__init__.py
+-rw-r--r--   0        0        0    12537 2023-04-27 11:35:11.820111 moneykit-0.0.5/moneykit/plaid_compatible/rest.py
+-rw-r--r--   0        0        0    12478 2023-04-27 11:35:02.561012 moneykit-0.0.5/moneykit/rest.py
+-rw-r--r--   0        0        0      935 2023-04-27 12:57:29.878211 moneykit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 moneykit-0.0.5/PKG-INFO
```

