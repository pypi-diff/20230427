# Comparing `tmp/criteo-api-marketingsolutions-sdk-2023.1.0.230427.tar.gz` & `tmp/criteo-api-marketingsolutions-sdk-2023.4.0.230427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.1.0.230427.tar", last modified: Thu Apr 27 13:29:25 2023, max compression
+gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.4.0.230427.tar", last modified: Thu Apr 27 13:29:39 2023, max compression
```

## Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427.tar` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.947090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 13:29:25.947090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.923090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 13:29:25.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-27 13:29:25.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:29:25.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:29:25.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 13:29:25.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.927090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.927090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    66384 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39252 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.927090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.947090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_frequency_capping.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_name_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/basic_audience_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14244 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/criteo_api_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/criteo_api_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/delete_audience_contact_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/delete_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/entity_of_portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/error_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/get_audiences_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/get_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/modify_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/problems_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_model_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/replace_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/replace_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/replace_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/request_ad_set_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/requests_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/requests_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/response_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/response_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/responses_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/responses_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/statistics_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/write_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/write_model_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    82575 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.947090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:29:25.951090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:25.947090 criteo-api-marketingsolutions-sdk-2023.1.0.230427/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.1.0.230427/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66384 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39252 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14244 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problems_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82575 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/test/test_gateway_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
-Version: 2023.1.0.230427
+Version: 2023.4.0.230427
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,21 +20,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_01
+import criteo_api_marketingsolutions_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/README.md` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 API Client Libraries can facilitate your use of the Criteo API allowing you to build unique and customized solutions to serve your businesses and clients.
 These libraries can reduce the amount of code you need to write in order to start accessing Criteo programmatically. They also can help expedite troubleshooting, should you encounter any issues.
 
 More information: [https://developers.criteo.com/](https://developers.criteo.com/)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- Package version: 2023.01.0.230427
+- Package version: 2023.04.0.230427
 
 ## Requirements
 
 Python 2.7 and 3.5+
 
 ## Installation & Usage
 ### pip install
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_01
+import criteo_api_marketingsolutions_v2023_04
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
 
 Download the code or clone the repository locally, then execute the following command:
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_01
+import criteo_api_marketingsolutions_v2023_04
 ```
 
 ## Example
 Please see [test/example_application.py](test/example_application.py) for an example.
 
 ## Documentation for API Endpoints
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
-Version: 2023.1.0.230427
+Version: 2023.4.0.230427
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,21 +20,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_01
+import criteo_api_marketingsolutions_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,131 +2,131 @@
 setup.cfg
 setup.py
 criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
 criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
 criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
 criteo_api_marketingsolutions_sdk.egg-info/requires.txt
 criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-criteo_api_marketingsolutions_v2023_01/__init__.py
-criteo_api_marketingsolutions_v2023_01/api_client.py
-criteo_api_marketingsolutions_v2023_01/api_client_builder.py
-criteo_api_marketingsolutions_v2023_01/configuration.py
-criteo_api_marketingsolutions_v2023_01/criteo_api_client.py
-criteo_api_marketingsolutions_v2023_01/criteo_auth.py
-criteo_api_marketingsolutions_v2023_01/criteo_rest.py
-criteo_api_marketingsolutions_v2023_01/exceptions.py
-criteo_api_marketingsolutions_v2023_01/model_utils.py
-criteo_api_marketingsolutions_v2023_01/rest.py
-criteo_api_marketingsolutions_v2023_01/api/__init__.py
-criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py
-criteo_api_marketingsolutions_v2023_01/api/analytics_api.py
-criteo_api_marketingsolutions_v2023_01/api/audience_api.py
-criteo_api_marketingsolutions_v2023_01/api/campaign_api.py
-criteo_api_marketingsolutions_v2023_01/api/gateway_api.py
-criteo_api_marketingsolutions_v2023_01/apis/__init__.py
-criteo_api_marketingsolutions_v2023_01/model/__init__.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_frequency_capping.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_geo_location.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_search_filter.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting.py
-criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting_rule.py
-criteo_api_marketingsolutions_v2023_01/model/application_summary_model.py
-criteo_api_marketingsolutions_v2023_01/model/application_summary_model_resource.py
-criteo_api_marketingsolutions_v2023_01/model/application_summary_model_response.py
-criteo_api_marketingsolutions_v2023_01/model/audience.py
-criteo_api_marketingsolutions_v2023_01/model/audience_attributes.py
-criteo_api_marketingsolutions_v2023_01/model/audience_error.py
-criteo_api_marketingsolutions_v2023_01/model/audience_name_description.py
-criteo_api_marketingsolutions_v2023_01/model/audience_warning.py
-criteo_api_marketingsolutions_v2023_01/model/basic_audience_definition.py
-criteo_api_marketingsolutions_v2023_01/model/campaign.py
-criteo_api_marketingsolutions_v2023_01/model/campaign_list_response.py
-criteo_api_marketingsolutions_v2023_01/model/campaign_read_resource.py
-criteo_api_marketingsolutions_v2023_01/model/campaign_response.py
-criteo_api_marketingsolutions_v2023_01/model/campaign_search_filters.py
-criteo_api_marketingsolutions_v2023_01/model/campaign_search_request.py
-criteo_api_marketingsolutions_v2023_01/model/campaign_spend_limit.py
-criteo_api_marketingsolutions_v2023_01/model/common_problem.py
-criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment.py
-criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_attributes.py
-criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_request.py
-criteo_api_marketingsolutions_v2023_01/model/contactlist_operation.py
-criteo_api_marketingsolutions_v2023_01/model/contactlist_operation_attributes.py
-criteo_api_marketingsolutions_v2023_01/model/criteo_api_error.py
-criteo_api_marketingsolutions_v2023_01/model/criteo_api_warning.py
-criteo_api_marketingsolutions_v2023_01/model/delete_audience_contact_list_response.py
-criteo_api_marketingsolutions_v2023_01/model/delete_audience_response.py
-criteo_api_marketingsolutions_v2023_01/model/entity_of_portfolio_message.py
-criteo_api_marketingsolutions_v2023_01/model/error_code_response.py
-criteo_api_marketingsolutions_v2023_01/model/get_audiences_response.py
-criteo_api_marketingsolutions_v2023_01/model/get_portfolio_response.py
-criteo_api_marketingsolutions_v2023_01/model/modify_audience_response.py
-criteo_api_marketingsolutions_v2023_01/model/new_audience.py
-criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py
-criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py
-criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py
-criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py
-criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py
-criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py
-criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_resource.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_list_request.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_resource.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_list_response.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_resource.py
-criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_scheduling.py
-criteo_api_marketingsolutions_v2023_01/model/patch_campaign.py
-criteo_api_marketingsolutions_v2023_01/model/patch_campaign_list_request.py
-criteo_api_marketingsolutions_v2023_01/model/patch_campaign_spend_limit.py
-criteo_api_marketingsolutions_v2023_01/model/patch_campaign_write_resource.py
-criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_list_response.py
-criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_read_resource.py
-criteo_api_marketingsolutions_v2023_01/model/placements_report_query_data_message.py
-criteo_api_marketingsolutions_v2023_01/model/placements_report_query_entity_message.py
-criteo_api_marketingsolutions_v2023_01/model/placements_report_query_message.py
-criteo_api_marketingsolutions_v2023_01/model/portfolio_message.py
-criteo_api_marketingsolutions_v2023_01/model/problem_details.py
-criteo_api_marketingsolutions_v2023_01/model/problems_details.py
-criteo_api_marketingsolutions_v2023_01/model/read_ad_set.py
-criteo_api_marketingsolutions_v2023_01/model/read_ad_set_bidding.py
-criteo_api_marketingsolutions_v2023_01/model/read_ad_set_budget.py
-criteo_api_marketingsolutions_v2023_01/model/read_ad_set_schedule.py
-criteo_api_marketingsolutions_v2023_01/model/read_model_ad_set_id.py
-criteo_api_marketingsolutions_v2023_01/model/read_model_read_ad_set.py
-criteo_api_marketingsolutions_v2023_01/model/replace_audience.py
-criteo_api_marketingsolutions_v2023_01/model/replace_audience_request.py
-criteo_api_marketingsolutions_v2023_01/model/replace_audience_response.py
-criteo_api_marketingsolutions_v2023_01/model/request_ad_set_search.py
-criteo_api_marketingsolutions_v2023_01/model/requests_ad_set_id.py
-criteo_api_marketingsolutions_v2023_01/model/requests_patch_ad_set.py
-criteo_api_marketingsolutions_v2023_01/model/response_ad_set_id.py
-criteo_api_marketingsolutions_v2023_01/model/response_read_ad_set.py
-criteo_api_marketingsolutions_v2023_01/model/responses_ad_set_id.py
-criteo_api_marketingsolutions_v2023_01/model/responses_read_ad_set.py
-criteo_api_marketingsolutions_v2023_01/model/statistics_report_query_message.py
-criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_data_message.py
-criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_entity_message.py
-criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_message.py
-criteo_api_marketingsolutions_v2023_01/model/transparency_query_message.py
-criteo_api_marketingsolutions_v2023_01/model/transparency_report_attributes.py
-criteo_api_marketingsolutions_v2023_01/model/transparency_report_data_message.py
-criteo_api_marketingsolutions_v2023_01/model/transparency_report_entity_message.py
-criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py
-criteo_api_marketingsolutions_v2023_01/model/write_model_ad_set_id.py
-criteo_api_marketingsolutions_v2023_01/model/write_model_patch_ad_set.py
-criteo_api_marketingsolutions_v2023_01/models/__init__.py
+criteo_api_marketingsolutions_v2023_04/__init__.py
+criteo_api_marketingsolutions_v2023_04/api_client.py
+criteo_api_marketingsolutions_v2023_04/api_client_builder.py
+criteo_api_marketingsolutions_v2023_04/configuration.py
+criteo_api_marketingsolutions_v2023_04/criteo_api_client.py
+criteo_api_marketingsolutions_v2023_04/criteo_auth.py
+criteo_api_marketingsolutions_v2023_04/criteo_rest.py
+criteo_api_marketingsolutions_v2023_04/exceptions.py
+criteo_api_marketingsolutions_v2023_04/model_utils.py
+criteo_api_marketingsolutions_v2023_04/rest.py
+criteo_api_marketingsolutions_v2023_04/api/__init__.py
+criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py
+criteo_api_marketingsolutions_v2023_04/api/analytics_api.py
+criteo_api_marketingsolutions_v2023_04/api/audience_api.py
+criteo_api_marketingsolutions_v2023_04/api/campaign_api.py
+criteo_api_marketingsolutions_v2023_04/api/gateway_api.py
+criteo_api_marketingsolutions_v2023_04/apis/__init__.py
+criteo_api_marketingsolutions_v2023_04/model/__init__.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py
+criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py
+criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py
+criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py
+criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py
+criteo_api_marketingsolutions_v2023_04/model/audience.py
+criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py
+criteo_api_marketingsolutions_v2023_04/model/audience_error.py
+criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py
+criteo_api_marketingsolutions_v2023_04/model/audience_warning.py
+criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py
+criteo_api_marketingsolutions_v2023_04/model/campaign.py
+criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py
+criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py
+criteo_api_marketingsolutions_v2023_04/model/campaign_response.py
+criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py
+criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py
+criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py
+criteo_api_marketingsolutions_v2023_04/model/common_problem.py
+criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py
+criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py
+criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py
+criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py
+criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py
+criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py
+criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py
+criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py
+criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py
+criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py
+criteo_api_marketingsolutions_v2023_04/model/error_code_response.py
+criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py
+criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py
+criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py
+criteo_api_marketingsolutions_v2023_04/model/new_audience.py
+criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py
+criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py
+criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py
+criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py
+criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py
+criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py
+criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py
+criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py
+criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py
+criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py
+criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py
+criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py
+criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py
+criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py
+criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py
+criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py
+criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py
+criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py
+criteo_api_marketingsolutions_v2023_04/model/problem_details.py
+criteo_api_marketingsolutions_v2023_04/model/problems_details.py
+criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py
+criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py
+criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py
+criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py
+criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py
+criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py
+criteo_api_marketingsolutions_v2023_04/model/replace_audience.py
+criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py
+criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py
+criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py
+criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py
+criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py
+criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py
+criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py
+criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py
+criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py
+criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py
+criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py
+criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py
+criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py
+criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py
+criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py
+criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py
+criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py
+criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py
+criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py
+criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py
+criteo_api_marketingsolutions_v2023_04/models/__init__.py
 test/test_gateway_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2023.01.0.230427"
+__version__ = "2023.04.0.230427"
 
 # import ApiClient
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient
-from criteo_api_marketingsolutions_v2023_01.criteo_api_client import CriteoApiClient
-from criteo_api_marketingsolutions_v2023_01.api_client_builder import ApiClientBuilder
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
+from criteo_api_marketingsolutions_v2023_04.criteo_api_client import CriteoApiClient
+from criteo_api_marketingsolutions_v2023_04.api_client_builder import ApiClientBuilder
 
 # import Configuration
-from criteo_api_marketingsolutions_v2023_01.configuration import Configuration
+from criteo_api_marketingsolutions_v2023_04.configuration import Configuration
 
 # import exceptions
-from criteo_api_marketingsolutions_v2023_01.exceptions import OpenApiException
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiTypeError
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiValueError
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiKeyError
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiException
+from criteo_api_marketingsolutions_v2023_04.exceptions import OpenApiException
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiTypeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiValueError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiKeyError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiException
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/advertiser_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_01.model.get_portfolio_response import GetPortfolioResponse
+from criteo_api_marketingsolutions_v2023_04.model.get_portfolio_response import GetPortfolioResponse
 
 
 class AdvertiserApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -38,15 +38,15 @@
         self.api_portfolio_get_endpoint = _Endpoint(
             settings={
                 'response_type': (GetPortfolioResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/advertisers/me',
+                'endpoint_path': '/2023-04/advertisers/me',
                 'operation_id': 'api_portfolio_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/analytics_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_01.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2023_01.model.problems_details import ProblemsDetails
-from criteo_api_marketingsolutions_v2023_01.model.statistics_report_query_message import StatisticsReportQueryMessage
-from criteo_api_marketingsolutions_v2023_01.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2023_01.model.transparency_query_message import TransparencyQueryMessage
-from criteo_api_marketingsolutions_v2023_01.model.transparency_report_data_message import TransparencyReportDataMessage
+from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2023_04.model.problems_details import ProblemsDetails
+from criteo_api_marketingsolutions_v2023_04.model.statistics_report_query_message import StatisticsReportQueryMessage
+from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2023_04.model.transparency_query_message import TransparencyQueryMessage
+from criteo_api_marketingsolutions_v2023_04.model.transparency_report_data_message import TransparencyReportDataMessage
 
 
 class AnalyticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -43,15 +43,15 @@
         self.get_adset_report_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/statistics/report',
+                'endpoint_path': '/2023-04/statistics/report',
                 'operation_id': 'get_adset_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'statistics_report_query_message',
@@ -102,15 +102,15 @@
         self.get_placements_report_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/placements/report',
+                'endpoint_path': '/2023-04/placements/report',
                 'operation_id': 'get_placements_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'placements_report_query_data_message',
@@ -158,15 +158,15 @@
         self.get_transactions_report_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/transactions/report',
+                'endpoint_path': '/2023-04/transactions/report',
                 'operation_id': 'get_transactions_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'transactions_report_query_data_message',
@@ -217,15 +217,15 @@
         self.get_transparency_report_endpoint = _Endpoint(
             settings={
                 'response_type': (TransparencyReportDataMessage,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/log-level/advertisers/{advertiser-id}/report',
+                'endpoint_path': '/2023-04/log-level/advertisers/{advertiser-id}/report',
                 'operation_id': 'get_transparency_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/audience_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/audience_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_01.model.contactlist_amendment_request import ContactlistAmendmentRequest
-from criteo_api_marketingsolutions_v2023_01.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
-from criteo_api_marketingsolutions_v2023_01.model.delete_audience_response import DeleteAudienceResponse
-from criteo_api_marketingsolutions_v2023_01.model.error_code_response import ErrorCodeResponse
-from criteo_api_marketingsolutions_v2023_01.model.get_audiences_response import GetAudiencesResponse
-from criteo_api_marketingsolutions_v2023_01.model.modify_audience_response import ModifyAudienceResponse
-from criteo_api_marketingsolutions_v2023_01.model.new_audience_request import NewAudienceRequest
-from criteo_api_marketingsolutions_v2023_01.model.new_audience_response import NewAudienceResponse
-from criteo_api_marketingsolutions_v2023_01.model.replace_audience_request import ReplaceAudienceRequest
-from criteo_api_marketingsolutions_v2023_01.model.replace_audience_response import ReplaceAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment_request import ContactlistAmendmentRequest
+from criteo_api_marketingsolutions_v2023_04.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
+from criteo_api_marketingsolutions_v2023_04.model.delete_audience_response import DeleteAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.error_code_response import ErrorCodeResponse
+from criteo_api_marketingsolutions_v2023_04.model.get_audiences_response import GetAudiencesResponse
+from criteo_api_marketingsolutions_v2023_04.model.modify_audience_response import ModifyAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.new_audience_request import NewAudienceRequest
+from criteo_api_marketingsolutions_v2023_04.model.new_audience_response import NewAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.replace_audience_request import ReplaceAudienceRequest
+from criteo_api_marketingsolutions_v2023_04.model.replace_audience_response import ReplaceAudienceResponse
 
 
 class AudienceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -47,15 +47,15 @@
         self.create_audience_endpoint = _Endpoint(
             settings={
                 'response_type': (NewAudienceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/audiences',
+                'endpoint_path': '/2023-04/audiences',
                 'operation_id': 'create_audience',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'new_audience_request',
@@ -100,15 +100,15 @@
         self.delete_identifiers_endpoint = _Endpoint(
             settings={
                 'response_type': (DeleteAudienceContactListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/audiences/{audience-id}/contactlist',
+                'endpoint_path': '/2023-04/audiences/{audience-id}/contactlist',
                 'operation_id': 'delete_identifiers',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_id',
@@ -152,15 +152,15 @@
         self.get_audiences_endpoint = _Endpoint(
             settings={
                 'response_type': (GetAudiencesResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/audiences',
+                'endpoint_path': '/2023-04/audiences',
                 'operation_id': 'get_audiences',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -202,15 +202,15 @@
         self.modify_audience_endpoint = _Endpoint(
             settings={
                 'response_type': (ReplaceAudienceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/audiences/{audience-id}',
+                'endpoint_path': '/2023-04/audiences/{audience-id}',
                 'operation_id': 'modify_audience',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_id',
@@ -261,15 +261,15 @@
         self.modify_audience_users_endpoint = _Endpoint(
             settings={
                 'response_type': (ModifyAudienceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/audiences/{audience-id}/contactlist',
+                'endpoint_path': '/2023-04/audiences/{audience-id}/contactlist',
                 'operation_id': 'modify_audience_users',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_id',
@@ -320,15 +320,15 @@
         self.remove_audience_endpoint = _Endpoint(
             settings={
                 'response_type': (DeleteAudienceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/audiences/{audience-id}',
+                'endpoint_path': '/2023-04/audiences/{audience-id}',
                 'operation_id': 'remove_audience',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_id',
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/campaign_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
-from criteo_api_marketingsolutions_v2023_01.model.campaign_list_response import CampaignListResponse
-from criteo_api_marketingsolutions_v2023_01.model.campaign_response import CampaignResponse
-from criteo_api_marketingsolutions_v2023_01.model.campaign_search_request import CampaignSearchRequest
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
-from criteo_api_marketingsolutions_v2023_01.model.patch_campaign_list_request import PatchCampaignListRequest
-from criteo_api_marketingsolutions_v2023_01.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
-from criteo_api_marketingsolutions_v2023_01.model.request_ad_set_search import RequestAdSetSearch
-from criteo_api_marketingsolutions_v2023_01.model.requests_ad_set_id import RequestsAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.requests_patch_ad_set import RequestsPatchAdSet
-from criteo_api_marketingsolutions_v2023_01.model.response_ad_set_id import ResponseAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.response_read_ad_set import ResponseReadAdSet
-from criteo_api_marketingsolutions_v2023_01.model.responses_ad_set_id import ResponsesAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.responses_read_ad_set import ResponsesReadAdSet
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
+from criteo_api_marketingsolutions_v2023_04.model.campaign_list_response import CampaignListResponse
+from criteo_api_marketingsolutions_v2023_04.model.campaign_response import CampaignResponse
+from criteo_api_marketingsolutions_v2023_04.model.campaign_search_request import CampaignSearchRequest
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
+from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_list_request import PatchCampaignListRequest
+from criteo_api_marketingsolutions_v2023_04.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
+from criteo_api_marketingsolutions_v2023_04.model.request_ad_set_search import RequestAdSetSearch
+from criteo_api_marketingsolutions_v2023_04.model.requests_ad_set_id import RequestsAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.requests_patch_ad_set import RequestsPatchAdSet
+from criteo_api_marketingsolutions_v2023_04.model.response_ad_set_id import ResponseAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.response_read_ad_set import ResponseReadAdSet
+from criteo_api_marketingsolutions_v2023_04.model.responses_ad_set_id import ResponsesAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.responses_read_ad_set import ResponsesReadAdSet
 
 
 class CampaignApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -55,15 +55,15 @@
         self.get_ad_set_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponseReadAdSet,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/{adSetId}',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{adSetId}',
                 'operation_id': 'get_ad_set',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -109,15 +109,15 @@
         self.get_campaign_endpoint = _Endpoint(
             settings={
                 'response_type': (CampaignResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/campaigns/{campaign-id}',
+                'endpoint_path': '/2023-04/marketing-solutions/campaigns/{campaign-id}',
                 'operation_id': 'get_campaign',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -163,15 +163,15 @@
         self.get_category_bid_list_endpoint = _Endpoint(
             settings={
                 'response_type': (AdSetCategoryBidListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
                 'operation_id': 'get_category_bid_list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -217,15 +217,15 @@
         self.get_display_multipliers_endpoint = _Endpoint(
             settings={
                 'response_type': (AdSetDisplayMultiplierListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
                 'operation_id': 'get_display_multipliers',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -271,15 +271,15 @@
         self.patch_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponseAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets',
                 'operation_id': 'patch_ad_sets',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_patch_ad_set',
@@ -327,15 +327,15 @@
         self.patch_campaigns_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchResultCampaignListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/campaigns',
+                'endpoint_path': '/2023-04/marketing-solutions/campaigns',
                 'operation_id': 'patch_campaigns',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'patch_campaign_list_request',
@@ -383,15 +383,15 @@
         self.patch_category_bid_list_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchAdSetCategoryBidResultListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
                 'operation_id': 'patch_category_bid_list',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -446,15 +446,15 @@
         self.patch_display_multipliers_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchAdSetDisplayMultiplierResultListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
                 'operation_id': 'patch_display_multipliers',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -509,15 +509,15 @@
         self.search_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesReadAdSet,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/search',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/search',
                 'operation_id': 'search_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'request_ad_set_search',
@@ -565,15 +565,15 @@
         self.search_campaigns_endpoint = _Endpoint(
             settings={
                 'response_type': (CampaignListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/campaigns/search',
+                'endpoint_path': '/2023-04/marketing-solutions/campaigns/search',
                 'operation_id': 'search_campaigns',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_search_request',
@@ -621,15 +621,15 @@
         self.start_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/start',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/start',
                 'operation_id': 'start_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_ad_set_id',
@@ -677,15 +677,15 @@
         self.stop_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/ad-sets/stop',
+                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/stop',
                 'operation_id': 'stop_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_ad_set_id',
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api/gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_01.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_marketingsolutions_v2023_04.model.application_summary_model_response import ApplicationSummaryModelResponse
 
 
 class GatewayApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -38,15 +38,15 @@
         self.get_current_application_endpoint = _Endpoint(
             settings={
                 'response_type': (ApplicationSummaryModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/marketing-solutions/me',
+                'endpoint_path': '/2023-04/marketing-solutions/me',
                 'operation_id': 'get_current_application',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/api_client.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -16,18 +16,18 @@
 import os
 import re
 import typing
 from urllib.parse import quote
 from urllib3.fields import RequestField
 
 
-from criteo_api_marketingsolutions_v2023_01 import rest
-from criteo_api_marketingsolutions_v2023_01.configuration import Configuration
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiTypeError, ApiValueError, ApiException
-from criteo_api_marketingsolutions_v2023_01.model_utils import (
+from criteo_api_marketingsolutions_v2023_04 import rest
+from criteo_api_marketingsolutions_v2023_04.configuration import Configuration
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiTypeError, ApiValueError, ApiException
+from criteo_api_marketingsolutions_v2023_04.model_utils import (
     ModelNormal,
     ModelSimple,
     ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2023.01.0.230427/python'
+        self.user_agent = 'OpenAPI-Generator/2023.04.0.230427/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/apis/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/apis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from criteo_api_marketingsolutions_v2023_01.api.advertiser_api import AdvertiserApi
+#   from criteo_api_marketingsolutions_v2023_04.api.advertiser_api import AdvertiserApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from criteo_api_marketingsolutions_v2023_01.api.advertiser_api import AdvertiserApi
-from criteo_api_marketingsolutions_v2023_01.api.analytics_api import AnalyticsApi
-from criteo_api_marketingsolutions_v2023_01.api.audience_api import AudienceApi
-from criteo_api_marketingsolutions_v2023_01.api.campaign_api import CampaignApi
-from criteo_api_marketingsolutions_v2023_01.api.gateway_api import GatewayApi
+from criteo_api_marketingsolutions_v2023_04.api.advertiser_api import AdvertiserApi
+from criteo_api_marketingsolutions_v2023_04.api.analytics_api import AnalyticsApi
+from criteo_api_marketingsolutions_v2023_04.api.audience_api import AudienceApi
+from criteo_api_marketingsolutions_v2023_04.api.campaign_api import CampaignApi
+from criteo_api_marketingsolutions_v2023_04.api.gateway_api import GatewayApi
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/configuration.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiValueError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
@@ -129,15 +129,15 @@
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("criteo_api_marketingsolutions_v2023_01")
+        self.logger["package_logger"] = logging.getLogger("criteo_api_marketingsolutions_v2023_04")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -390,16 +390,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2023-01\n"\
-               "SDK Package Version: 2023.01.0.230427".\
+               "Version of the API: 2023-04\n"\
+               "SDK Package Version: 2023.04.0.230427".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/criteo_api_client.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient
-from criteo_api_marketingsolutions_v2023_01.criteo_rest import CriteoRESTClientObject
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
+from criteo_api_marketingsolutions_v2023_04.criteo_rest import CriteoRESTClientObject
 
 class CriteoApiClient(ApiClient):
     def __init__(self, configuration=None, header_name=None, header_value=None,
              cookie=None, pool_threads=1, additional_parameters= {}):
         super().__init__(configuration=configuration,header_name=header_name, header_value=header_value, cookie=cookie, pool_threads=pool_threads)
         self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/criteo_auth.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from datetime import datetime, timedelta
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiException
-from criteo_api_marketingsolutions_v2023_01.api_client import ApiClient
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiException
+from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
 
 class Token(object):
 
     def __init__(self, token_string , expiration_date = None):
         self.expiration_date = expiration_date 
         self.token_string = token_string
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/criteo_rest.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from criteo_api_marketingsolutions_v2023_01.rest import RESTClientObject
-from criteo_api_marketingsolutions_v2023_01.criteo_auth import *
+from criteo_api_marketingsolutions_v2023_04.rest import RESTClientObject
+from criteo_api_marketingsolutions_v2023_04.criteo_auth import *
 
 
 class CriteoRESTClientObject(RESTClientObject):
 
     def __init__(self, configuration, additional_parameters = {}, pools_size=4, maxsize=None):
         super().__init__(configuration, pools_size, maxsize)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/exceptions.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AdSetCategoryBid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid_resource import AdSetCategoryBidResource
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid_resource import AdSetCategoryBidResource
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['AdSetCategoryBidResource'] = AdSetCategoryBidResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class AdSetCategoryBidListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid import AdSetCategoryBid
-    globals()['AdSetCategoryBid'] = AdSetCategoryBid
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
+    globals()['PatchAdSetCategoryBid'] = PatchAdSetCategoryBid
 
 
-class AdSetCategoryBidResource(ModelNormal):
+class PatchAdSetCategoryBidResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (AdSetCategoryBid,),  # noqa: E501
+            'attributes': (PatchAdSetCategoryBid,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AdSetCategoryBidResource - a model defined in OpenAPI
+        """PatchAdSetCategoryBidResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +140,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (AdSetCategoryBid): [optional]  # noqa: E501
+            attributes (PatchAdSetCategoryBid): [optional]  # noqa: E501
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AdSetCategoryBidResource - a model defined in OpenAPI
+        """PatchAdSetCategoryBidResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,15 +228,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (AdSetCategoryBid): [optional]  # noqa: E501
+            attributes (PatchAdSetCategoryBid): [optional]  # noqa: E501
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_delivery_limitations.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AdSetDeliveryLimitations(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AdSetDisplayMultiplier(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['AdSetDisplayMultiplierResource'] = AdSetDisplayMultiplierResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class AdSetDisplayMultiplierListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier import AdSetDisplayMultiplier
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier import AdSetDisplayMultiplier
     globals()['AdSetDisplayMultiplier'] = AdSetDisplayMultiplier
 
 
 class AdSetDisplayMultiplierResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_frequency_capping.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AdSetFrequencyCapping(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_geo_location.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
     globals()['NillableAdSetTargetingRule'] = NillableAdSetTargetingRule
 
 
 class AdSetGeoLocation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_search_filter.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AdSetSearchFilter(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_frequency_capping import AdSetFrequencyCapping
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_geo_location import AdSetGeoLocation
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_frequency_capping import AdSetFrequencyCapping
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_geo_location import AdSetGeoLocation
     globals()['AdSetDeliveryLimitations'] = AdSetDeliveryLimitations
     globals()['AdSetFrequencyCapping'] = AdSetFrequencyCapping
     globals()['AdSetGeoLocation'] = AdSetGeoLocation
 
 
 class AdSetTargeting(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AdSetTargetingRule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/application_summary_model.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ApplicationSummaryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.application_summary_model import ApplicationSummaryModel
+    from criteo_api_marketingsolutions_v2023_04.model.application_summary_model import ApplicationSummaryModel
     globals()['ApplicationSummaryModel'] = ApplicationSummaryModel
 
 
 class ApplicationSummaryModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/application_summary_model_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-    from criteo_api_marketingsolutions_v2023_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2023_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+    from criteo_api_marketingsolutions_v2023_04.model.common_problem import CommonProblem
     globals()['ApplicationSummaryModelResource'] = ApplicationSummaryModelResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class ApplicationSummaryModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_attributes import AudienceAttributes
+    from criteo_api_marketingsolutions_v2023_04.model.audience_attributes import AudienceAttributes
     globals()['AudienceAttributes'] = AudienceAttributes
 
 
 class Audience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_error.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AudienceError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_name_description.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AudienceNameDescription(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/audience_warning.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class AudienceWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/basic_audience_definition.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_name_description import AudienceNameDescription
+    from criteo_api_marketingsolutions_v2023_04.model.audience_name_description import AudienceNameDescription
     globals()['AudienceNameDescription'] = AudienceNameDescription
 
 
 class BasicAudienceDefinition(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.campaign_spend_limit import CampaignSpendLimit
+    from criteo_api_marketingsolutions_v2023_04.model.campaign_spend_limit import CampaignSpendLimit
     globals()['CampaignSpendLimit'] = CampaignSpendLimit
 
 
 class Campaign(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.campaign_read_resource import CampaignReadResource
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.campaign_read_resource import CampaignReadResource
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['CampaignReadResource'] = CampaignReadResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class CampaignListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.campaign import Campaign
+    from criteo_api_marketingsolutions_v2023_04.model.campaign import Campaign
     globals()['Campaign'] = Campaign
 
 
 class CampaignReadResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.campaign_read_resource import CampaignReadResource
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.campaign_read_resource import CampaignReadResource
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['CampaignReadResource'] = CampaignReadResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class CampaignResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_search_filters.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CampaignSearchFilters(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_search_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.campaign_search_filters import CampaignSearchFilters
+    from criteo_api_marketingsolutions_v2023_04.model.campaign_search_filters import CampaignSearchFilters
     globals()['CampaignSearchFilters'] = CampaignSearchFilters
 
 
 class CampaignSearchRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class CampaignSpendLimit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/common_problem.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/common_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CommonProblem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
+    from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
     globals()['ContactlistAmendmentAttributes'] = ContactlistAmendmentAttributes
 
 
 class ContactlistAmendment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ContactlistAmendmentAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_amendment_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.contactlist_amendment import ContactlistAmendment
+    from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment import ContactlistAmendment
     globals()['ContactlistAmendment'] = ContactlistAmendment
 
 
 class ContactlistAmendmentRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.contactlist_operation_attributes import ContactlistOperationAttributes
+    from criteo_api_marketingsolutions_v2023_04.model.contactlist_operation_attributes import ContactlistOperationAttributes
     globals()['ContactlistOperationAttributes'] = ContactlistOperationAttributes
 
 
 class ContactlistOperation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/contactlist_operation_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ContactlistOperationAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/criteo_api_error.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CriteoApiError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/criteo_api_warning.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CriteoApiWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/delete_audience_contact_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_01.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class DeleteAudienceContactListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/delete_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_01.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class DeleteAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/entity_of_portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.portfolio_message import PortfolioMessage
+    from criteo_api_marketingsolutions_v2023_04.model.portfolio_message import PortfolioMessage
     globals()['PortfolioMessage'] = PortfolioMessage
 
 
 class EntityOfPortfolioMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/error_code_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
 
 
 class ErrorCodeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/get_audiences_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience import Audience
-    from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_04.model.audience import Audience
+    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
     globals()['Audience'] = Audience
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
 
 
 class GetAudiencesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/get_portfolio_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.criteo_api_error import CriteoApiError
-    from criteo_api_marketingsolutions_v2023_01.model.criteo_api_warning import CriteoApiWarning
-    from criteo_api_marketingsolutions_v2023_01.model.entity_of_portfolio_message import EntityOfPortfolioMessage
+    from criteo_api_marketingsolutions_v2023_04.model.criteo_api_error import CriteoApiError
+    from criteo_api_marketingsolutions_v2023_04.model.criteo_api_warning import CriteoApiWarning
+    from criteo_api_marketingsolutions_v2023_04.model.entity_of_portfolio_message import EntityOfPortfolioMessage
     globals()['CriteoApiError'] = CriteoApiError
     globals()['CriteoApiWarning'] = CriteoApiWarning
     globals()['EntityOfPortfolioMessage'] = EntityOfPortfolioMessage
 
 
 class GetPortfolioResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/modify_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_01.model.contactlist_operation import ContactlistOperation
+    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_04.model.contactlist_operation import ContactlistOperation
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['ContactlistOperation'] = ContactlistOperation
 
 
 class ModifyAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.new_audience_attributes import NewAudienceAttributes
+    from criteo_api_marketingsolutions_v2023_04.model.new_audience_attributes import NewAudienceAttributes
     globals()['NewAudienceAttributes'] = NewAudienceAttributes
 
 
 class NewAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class NewAudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.new_audience import NewAudience
-    globals()['NewAudience'] = NewAudience
+    from criteo_api_marketingsolutions_v2023_04.model.write_model_patch_ad_set import WriteModelPatchAdSet
+    globals()['WriteModelPatchAdSet'] = WriteModelPatchAdSet
 
 
-class NewAudienceRequest(ModelNormal):
+class RequestsPatchAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,14 +58,16 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('data',): {
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -83,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (NewAudience,),  # noqa: E501
+            'data': ([WriteModelPatchAdSet],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -103,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """NewAudienceRequest - a model defined in OpenAPI
+        """RequestsPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (NewAudience): [optional]  # noqa: E501
+            data ([WriteModelPatchAdSet]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """NewAudienceRequest - a model defined in OpenAPI
+        """RequestsPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +224,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (NewAudience): [optional]  # noqa: E501
+            data ([WriteModelPatchAdSet]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/new_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_01.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class NewAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
     globals()['NillableAdSetTargetingRuleValue'] = NillableAdSetTargetingRuleValue
 
 
 class NillableAdSetTargetingRule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_ad_set_targeting_rule_value.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_targeting_rule import AdSetTargetingRule
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting_rule import AdSetTargetingRule
     globals()['AdSetTargetingRule'] = AdSetTargetingRule
 
 
 class NillableAdSetTargetingRuleValue(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_date_time.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class NillableDateTime(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/nillable_decimal.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class NillableDecimal(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_targeting import AdSetTargeting
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_bidding import PatchAdSetBidding
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_budget import PatchAdSetBudget
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_scheduling import PatchAdSetScheduling
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting import AdSetTargeting
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_bidding import PatchAdSetBidding
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_budget import PatchAdSetBudget
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_scheduling import PatchAdSetScheduling
     globals()['AdSetTargeting'] = AdSetTargeting
     globals()['PatchAdSetBidding'] = PatchAdSetBidding
     globals()['PatchAdSetBudget'] = PatchAdSetBudget
     globals()['PatchAdSetScheduling'] = PatchAdSetScheduling
 
 
 class PatchAdSet(ModelNormal):
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchAdSetBudget(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetCategoryBid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
     globals()['PatchAdSetCategoryBidResource'] = PatchAdSetCategoryBidResource
 
 
 class PatchAdSetCategoryBidListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
-    globals()['PatchAdSetCategoryBid'] = PatchAdSetCategoryBid
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid import AdSetCategoryBid
+    globals()['AdSetCategoryBid'] = AdSetCategoryBid
 
 
-class PatchAdSetCategoryBidResource(ModelNormal):
+class AdSetCategoryBidResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (PatchAdSetCategoryBid,),  # noqa: E501
+            'attributes': (AdSetCategoryBid,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchAdSetCategoryBidResource - a model defined in OpenAPI
+        """AdSetCategoryBidResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +140,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (PatchAdSetCategoryBid): [optional]  # noqa: E501
+            attributes (AdSetCategoryBid): [optional]  # noqa: E501
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchAdSetCategoryBidResource - a model defined in OpenAPI
+        """AdSetCategoryBidResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,15 +228,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (PatchAdSetCategoryBid): [optional]  # noqa: E501
+            attributes (AdSetCategoryBid): [optional]  # noqa: E501
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['PatchAdSetCategoryBidResultResource'] = PatchAdSetCategoryBidResultResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class PatchAdSetCategoryBidResultListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_category_bid_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetCategoryBidResultResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetDisplayMultiplier(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
     globals()['PatchAdSetDisplayMultiplierResource'] = PatchAdSetDisplayMultiplierResource
 
 
 class PatchAdSetDisplayMultiplierListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
     globals()['PatchAdSetDisplayMultiplier'] = PatchAdSetDisplayMultiplier
 
 
 class PatchAdSetDisplayMultiplierResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['PatchAdSetDisplayMultiplierResultResource'] = PatchAdSetDisplayMultiplierResultResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class PatchAdSetDisplayMultiplierResultListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_display_multiplier_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetDisplayMultiplierResultResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_ad_set_scheduling.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_date_time import NillableDateTime
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_date_time import NillableDateTime
     globals()['NillableDateTime'] = NillableDateTime
 
 
 class PatchAdSetScheduling(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
+    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
     globals()['PatchCampaignSpendLimit'] = PatchCampaignSpendLimit
 
 
 class PatchCampaign(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_campaign_write_resource import PatchCampaignWriteResource
+    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_write_resource import PatchCampaignWriteResource
     globals()['PatchCampaignWriteResource'] = PatchCampaignWriteResource
 
 
 class PatchCampaignListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchCampaignSpendLimit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_campaign_write_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_campaign import PatchCampaign
+    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign import PatchCampaign
     globals()['PatchCampaign'] = PatchCampaign
 
 
 class PatchCampaignWriteResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['PatchResultCampaignReadResource'] = PatchResultCampaignReadResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class PatchResultCampaignListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/patch_result_campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PatchResultCampaignReadResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
+    from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
     globals()['PlacementsReportQueryEntityMessage'] = PlacementsReportQueryEntityMessage
 
 
 class PlacementsReportQueryDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.placements_report_query_message import PlacementsReportQueryMessage
+    from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_message import PlacementsReportQueryMessage
     globals()['PlacementsReportQueryMessage'] = PlacementsReportQueryMessage
 
 
 class PlacementsReportQueryEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/placements_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PlacementsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PortfolioMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/problem_details.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ProblemDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/problems_details.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problems_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class ProblemsDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_targeting import AdSetTargeting
-    from criteo_api_marketingsolutions_v2023_01.model.read_ad_set_bidding import ReadAdSetBidding
-    from criteo_api_marketingsolutions_v2023_01.model.read_ad_set_budget import ReadAdSetBudget
-    from criteo_api_marketingsolutions_v2023_01.model.read_ad_set_schedule import ReadAdSetSchedule
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting import AdSetTargeting
+    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_bidding import ReadAdSetBidding
+    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_budget import ReadAdSetBudget
+    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_schedule import ReadAdSetSchedule
     globals()['AdSetTargeting'] = AdSetTargeting
     globals()['ReadAdSetBidding'] = ReadAdSetBidding
     globals()['ReadAdSetBudget'] = ReadAdSetBudget
     globals()['ReadAdSetSchedule'] = ReadAdSetSchedule
 
 
 class ReadAdSet(ModelNormal):
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBudget(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_ad_set_schedule.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.nillable_date_time import NillableDateTime
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_date_time import NillableDateTime
     globals()['NillableDateTime'] = NillableDateTime
 
 
 class ReadAdSetSchedule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ReadModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/read_model_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.read_ad_set import ReadAdSet
+    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set import ReadAdSet
     globals()['ReadAdSet'] = ReadAdSet
 
 
 class ReadModelReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/replace_audience.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_name_description import AudienceNameDescription
+    from criteo_api_marketingsolutions_v2023_04.model.audience_name_description import AudienceNameDescription
     globals()['AudienceNameDescription'] = AudienceNameDescription
 
 
 class ReplaceAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/replace_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.replace_audience import ReplaceAudience
+    from criteo_api_marketingsolutions_v2023_04.model.replace_audience import ReplaceAudience
     globals()['ReplaceAudience'] = ReplaceAudience
 
 
 class ReplaceAudienceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/replace_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_01.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class ReplaceAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/request_ad_set_search.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.ad_set_search_filter import AdSetSearchFilter
+    from criteo_api_marketingsolutions_v2023_04.model.ad_set_search_filter import AdSetSearchFilter
     globals()['AdSetSearchFilter'] = AdSetSearchFilter
 
 
 class RequestAdSetSearch(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/requests_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.write_model_ad_set_id import WriteModelAdSetId
+    from criteo_api_marketingsolutions_v2023_04.model.write_model_ad_set_id import WriteModelAdSetId
     globals()['WriteModelAdSetId'] = WriteModelAdSetId
 
 
 class RequestsAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/requests_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.write_model_patch_ad_set import WriteModelPatchAdSet
-    globals()['WriteModelPatchAdSet'] = WriteModelPatchAdSet
+    from criteo_api_marketingsolutions_v2023_04.model.transparency_report_entity_message import TransparencyReportEntityMessage
+    globals()['TransparencyReportEntityMessage'] = TransparencyReportEntityMessage
 
 
-class RequestsPatchAdSet(ModelNormal):
+class TransparencyReportDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([WriteModelPatchAdSet],),  # noqa: E501
+            'data': ([TransparencyReportEntityMessage],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,16 +104,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RequestsPatchAdSet - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TransparencyReportDataMessage - a model defined in OpenAPI
+
+        Args:
+            data ([TransparencyReportEntityMessage]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +141,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WriteModelPatchAdSet]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,14 +172,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,16 +193,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """RequestsPatchAdSet - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TransparencyReportDataMessage - a model defined in OpenAPI
+
+        Args:
+            data ([TransparencyReportEntityMessage]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,15 +230,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WriteModelPatchAdSet]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -254,14 +259,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/response_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_01.model.read_model_ad_set_id import ReadModelAdSetId
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.read_model_ad_set_id import ReadModelAdSetId
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ReadModelAdSetId'] = ReadModelAdSetId
 
 
 class ResponseAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/response_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_01.model.read_model_read_ad_set import ReadModelReadAdSet
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.read_model_ad_set_id import ReadModelAdSetId
     globals()['ProblemDetails'] = ProblemDetails
-    globals()['ReadModelReadAdSet'] = ReadModelReadAdSet
+    globals()['ReadModelAdSetId'] = ReadModelAdSetId
 
 
-class ResponseReadAdSet(ModelNormal):
+class ResponsesAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,14 +60,16 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('data',): {
+        },
         ('warnings',): {
         },
         ('errors',): {
         },
     }
 
     @cached_property
@@ -89,15 +91,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (ReadModelReadAdSet,),  # noqa: E501
+            'data': ([ReadModelAdSetId],),  # noqa: E501
             'warnings': ([ProblemDetails],),  # noqa: E501
             'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -106,24 +108,25 @@
     attribute_map = {
         'data': 'data',  # noqa: E501
         'warnings': 'warnings',  # noqa: E501
         'errors': 'errors',  # noqa: E501
     }
 
     read_only_vars = {
+        'data',  # noqa: E501
         'warnings',  # noqa: E501
         'errors',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResponseReadAdSet - a model defined in OpenAPI
+        """ResponsesAdSetId - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -148,15 +151,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ReadModelReadAdSet): [optional]  # noqa: E501
+            data ([ReadModelAdSetId]): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -203,15 +206,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResponseReadAdSet - a model defined in OpenAPI
+        """ResponsesAdSetId - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -236,15 +239,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ReadModelReadAdSet): [optional]  # noqa: E501
+            data ([ReadModelAdSetId]): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/responses_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_01.model.read_model_ad_set_id import ReadModelAdSetId
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.read_model_read_ad_set import ReadModelReadAdSet
     globals()['ProblemDetails'] = ProblemDetails
-    globals()['ReadModelAdSetId'] = ReadModelAdSetId
+    globals()['ReadModelReadAdSet'] = ReadModelReadAdSet
 
 
-class ResponsesAdSetId(ModelNormal):
+class ResponseReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,16 +60,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('data',): {
-        },
         ('warnings',): {
         },
         ('errors',): {
         },
     }
 
     @cached_property
@@ -91,15 +89,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([ReadModelAdSetId],),  # noqa: E501
+            'data': (ReadModelReadAdSet,),  # noqa: E501
             'warnings': ([ProblemDetails],),  # noqa: E501
             'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -108,25 +106,24 @@
     attribute_map = {
         'data': 'data',  # noqa: E501
         'warnings': 'warnings',  # noqa: E501
         'errors': 'errors',  # noqa: E501
     }
 
     read_only_vars = {
-        'data',  # noqa: E501
         'warnings',  # noqa: E501
         'errors',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResponsesAdSetId - a model defined in OpenAPI
+        """ResponseReadAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,15 +148,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ReadModelAdSetId]): [optional]  # noqa: E501
+            data (ReadModelReadAdSet): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -206,15 +203,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResponsesAdSetId - a model defined in OpenAPI
+        """ResponseReadAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,15 +236,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ReadModelAdSetId]): [optional]  # noqa: E501
+            data (ReadModelReadAdSet): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/responses_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_01.model.read_model_read_ad_set import ReadModelReadAdSet
+    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_04.model.read_model_read_ad_set import ReadModelReadAdSet
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ReadModelReadAdSet'] = ReadModelReadAdSet
 
 
 class ResponsesReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/statistics_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class StatisticsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
+    from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
     globals()['TransactionsReportQueryEntityMessage'] = TransactionsReportQueryEntityMessage
 
 
 class TransactionsReportQueryDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.transactions_report_query_message import TransactionsReportQueryMessage
+    from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_message import TransactionsReportQueryMessage
     globals()['TransactionsReportQueryMessage'] = TransactionsReportQueryMessage
 
 
 class TransactionsReportQueryEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transactions_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class TransactionsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class TransparencyQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.transparency_report_file import TransparencyReportFile
+    from criteo_api_marketingsolutions_v2023_04.model.transparency_report_file import TransparencyReportFile
     globals()['TransparencyReportFile'] = TransparencyReportFile
 
 
 class TransparencyReportAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.transparency_report_entity_message import TransparencyReportEntityMessage
-    globals()['TransparencyReportEntityMessage'] = TransparencyReportEntityMessage
+    from criteo_api_marketingsolutions_v2023_04.model.transparency_report_attributes import TransparencyReportAttributes
+    globals()['TransparencyReportAttributes'] = TransparencyReportAttributes
 
 
-class TransparencyReportDataMessage(ModelNormal):
+class TransparencyReportEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,16 +58,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('data',): {
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -85,38 +83,42 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([TransparencyReportEntityMessage],),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': (TransparencyReportAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
+        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TransparencyReportDataMessage - a model defined in OpenAPI
+    def _from_openapi_data(cls, type, attributes, *args, **kwargs):  # noqa: E501
+        """TransparencyReportEntityMessage - a model defined in OpenAPI
 
         Args:
-            data ([TransparencyReportEntityMessage]):
+            type (str):
+            attributes (TransparencyReportAttributes):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -172,15 +174,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.type = type
+        self.attributes = attributes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,19 +196,18 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TransparencyReportDataMessage - a model defined in OpenAPI
+    def __init__(self, attributes, *args, **kwargs):  # noqa: E501
+        """TransparencyReportEntityMessage - a model defined in OpenAPI
 
-        Args:
-            data ([TransparencyReportEntityMessage]):
+            attributes (TransparencyReportAttributes):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -259,15 +261,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.attributes = attributes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.transparency_report_attributes import TransparencyReportAttributes
-    globals()['TransparencyReportAttributes'] = TransparencyReportAttributes
+    from criteo_api_marketingsolutions_v2023_04.model.new_audience import NewAudience
+    globals()['NewAudience'] = NewAudience
 
 
-class TransparencyReportEntityMessage(ModelNormal):
+class NewAudienceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,42 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'attributes': (TransparencyReportAttributes,),  # noqa: E501
+            'data': (NewAudience,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
-        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, attributes, *args, **kwargs):  # noqa: E501
-        """TransparencyReportEntityMessage - a model defined in OpenAPI
-
-        Args:
-            type (str):
-            attributes (TransparencyReportAttributes):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """NewAudienceRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            data (NewAudience): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,16 +168,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.attributes = attributes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,18 +188,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, *args, **kwargs):  # noqa: E501
-        """TransparencyReportEntityMessage - a model defined in OpenAPI
-
-            attributes (TransparencyReportAttributes):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """NewAudienceRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,14 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            data (NewAudience): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -261,15 +252,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.attributes = attributes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/transparency_report_file.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class TransparencyReportFile(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/write_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
 class WriteModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model/write_model_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set import PatchAdSet
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set import PatchAdSet
     globals()['PatchAdSet'] = PatchAdSet
 
 
 class WriteModelPatchAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/model_utils.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
@@ -16,15 +16,15 @@
 import pprint
 import re
 import tempfile
 import uuid
 
 from dateutil.parser import parse
 
-from criteo_api_marketingsolutions_v2023_01.exceptions import (
+from criteo_api_marketingsolutions_v2023_04.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/models/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from criteo_api_marketingsolutions_v2023_01.model.pet import Pet
+# from criteo_api_marketingsolutions_v2023_04.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid import AdSetCategoryBid
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_category_bid_resource import AdSetCategoryBidResource
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier import AdSetDisplayMultiplier
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_frequency_capping import AdSetFrequencyCapping
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_geo_location import AdSetGeoLocation
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_search_filter import AdSetSearchFilter
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_targeting import AdSetTargeting
-from criteo_api_marketingsolutions_v2023_01.model.ad_set_targeting_rule import AdSetTargetingRule
-from criteo_api_marketingsolutions_v2023_01.model.application_summary_model import ApplicationSummaryModel
-from criteo_api_marketingsolutions_v2023_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-from criteo_api_marketingsolutions_v2023_01.model.application_summary_model_response import ApplicationSummaryModelResponse
-from criteo_api_marketingsolutions_v2023_01.model.audience import Audience
-from criteo_api_marketingsolutions_v2023_01.model.audience_attributes import AudienceAttributes
-from criteo_api_marketingsolutions_v2023_01.model.audience_error import AudienceError
-from criteo_api_marketingsolutions_v2023_01.model.audience_name_description import AudienceNameDescription
-from criteo_api_marketingsolutions_v2023_01.model.audience_warning import AudienceWarning
-from criteo_api_marketingsolutions_v2023_01.model.basic_audience_definition import BasicAudienceDefinition
-from criteo_api_marketingsolutions_v2023_01.model.campaign import Campaign
-from criteo_api_marketingsolutions_v2023_01.model.campaign_list_response import CampaignListResponse
-from criteo_api_marketingsolutions_v2023_01.model.campaign_read_resource import CampaignReadResource
-from criteo_api_marketingsolutions_v2023_01.model.campaign_response import CampaignResponse
-from criteo_api_marketingsolutions_v2023_01.model.campaign_search_filters import CampaignSearchFilters
-from criteo_api_marketingsolutions_v2023_01.model.campaign_search_request import CampaignSearchRequest
-from criteo_api_marketingsolutions_v2023_01.model.campaign_spend_limit import CampaignSpendLimit
-from criteo_api_marketingsolutions_v2023_01.model.common_problem import CommonProblem
-from criteo_api_marketingsolutions_v2023_01.model.contactlist_amendment import ContactlistAmendment
-from criteo_api_marketingsolutions_v2023_01.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
-from criteo_api_marketingsolutions_v2023_01.model.contactlist_amendment_request import ContactlistAmendmentRequest
-from criteo_api_marketingsolutions_v2023_01.model.contactlist_operation import ContactlistOperation
-from criteo_api_marketingsolutions_v2023_01.model.contactlist_operation_attributes import ContactlistOperationAttributes
-from criteo_api_marketingsolutions_v2023_01.model.criteo_api_error import CriteoApiError
-from criteo_api_marketingsolutions_v2023_01.model.criteo_api_warning import CriteoApiWarning
-from criteo_api_marketingsolutions_v2023_01.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
-from criteo_api_marketingsolutions_v2023_01.model.delete_audience_response import DeleteAudienceResponse
-from criteo_api_marketingsolutions_v2023_01.model.entity_of_portfolio_message import EntityOfPortfolioMessage
-from criteo_api_marketingsolutions_v2023_01.model.error_code_response import ErrorCodeResponse
-from criteo_api_marketingsolutions_v2023_01.model.get_audiences_response import GetAudiencesResponse
-from criteo_api_marketingsolutions_v2023_01.model.get_portfolio_response import GetPortfolioResponse
-from criteo_api_marketingsolutions_v2023_01.model.modify_audience_response import ModifyAudienceResponse
-from criteo_api_marketingsolutions_v2023_01.model.new_audience import NewAudience
-from criteo_api_marketingsolutions_v2023_01.model.new_audience_attributes import NewAudienceAttributes
-from criteo_api_marketingsolutions_v2023_01.model.new_audience_request import NewAudienceRequest
-from criteo_api_marketingsolutions_v2023_01.model.new_audience_response import NewAudienceResponse
-from criteo_api_marketingsolutions_v2023_01.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
-from criteo_api_marketingsolutions_v2023_01.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
-from criteo_api_marketingsolutions_v2023_01.model.nillable_date_time import NillableDateTime
-from criteo_api_marketingsolutions_v2023_01.model.nillable_decimal import NillableDecimal
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set import PatchAdSet
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_bidding import PatchAdSetBidding
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_budget import PatchAdSetBudget
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
-from criteo_api_marketingsolutions_v2023_01.model.patch_ad_set_scheduling import PatchAdSetScheduling
-from criteo_api_marketingsolutions_v2023_01.model.patch_campaign import PatchCampaign
-from criteo_api_marketingsolutions_v2023_01.model.patch_campaign_list_request import PatchCampaignListRequest
-from criteo_api_marketingsolutions_v2023_01.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
-from criteo_api_marketingsolutions_v2023_01.model.patch_campaign_write_resource import PatchCampaignWriteResource
-from criteo_api_marketingsolutions_v2023_01.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
-from criteo_api_marketingsolutions_v2023_01.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
-from criteo_api_marketingsolutions_v2023_01.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2023_01.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
-from criteo_api_marketingsolutions_v2023_01.model.placements_report_query_message import PlacementsReportQueryMessage
-from criteo_api_marketingsolutions_v2023_01.model.portfolio_message import PortfolioMessage
-from criteo_api_marketingsolutions_v2023_01.model.problem_details import ProblemDetails
-from criteo_api_marketingsolutions_v2023_01.model.problems_details import ProblemsDetails
-from criteo_api_marketingsolutions_v2023_01.model.read_ad_set import ReadAdSet
-from criteo_api_marketingsolutions_v2023_01.model.read_ad_set_bidding import ReadAdSetBidding
-from criteo_api_marketingsolutions_v2023_01.model.read_ad_set_budget import ReadAdSetBudget
-from criteo_api_marketingsolutions_v2023_01.model.read_ad_set_schedule import ReadAdSetSchedule
-from criteo_api_marketingsolutions_v2023_01.model.read_model_ad_set_id import ReadModelAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.read_model_read_ad_set import ReadModelReadAdSet
-from criteo_api_marketingsolutions_v2023_01.model.replace_audience import ReplaceAudience
-from criteo_api_marketingsolutions_v2023_01.model.replace_audience_request import ReplaceAudienceRequest
-from criteo_api_marketingsolutions_v2023_01.model.replace_audience_response import ReplaceAudienceResponse
-from criteo_api_marketingsolutions_v2023_01.model.request_ad_set_search import RequestAdSetSearch
-from criteo_api_marketingsolutions_v2023_01.model.requests_ad_set_id import RequestsAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.requests_patch_ad_set import RequestsPatchAdSet
-from criteo_api_marketingsolutions_v2023_01.model.response_ad_set_id import ResponseAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.response_read_ad_set import ResponseReadAdSet
-from criteo_api_marketingsolutions_v2023_01.model.responses_ad_set_id import ResponsesAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.responses_read_ad_set import ResponsesReadAdSet
-from criteo_api_marketingsolutions_v2023_01.model.statistics_report_query_message import StatisticsReportQueryMessage
-from criteo_api_marketingsolutions_v2023_01.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2023_01.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
-from criteo_api_marketingsolutions_v2023_01.model.transactions_report_query_message import TransactionsReportQueryMessage
-from criteo_api_marketingsolutions_v2023_01.model.transparency_query_message import TransparencyQueryMessage
-from criteo_api_marketingsolutions_v2023_01.model.transparency_report_attributes import TransparencyReportAttributes
-from criteo_api_marketingsolutions_v2023_01.model.transparency_report_data_message import TransparencyReportDataMessage
-from criteo_api_marketingsolutions_v2023_01.model.transparency_report_entity_message import TransparencyReportEntityMessage
-from criteo_api_marketingsolutions_v2023_01.model.transparency_report_file import TransparencyReportFile
-from criteo_api_marketingsolutions_v2023_01.model.write_model_ad_set_id import WriteModelAdSetId
-from criteo_api_marketingsolutions_v2023_01.model.write_model_patch_ad_set import WriteModelPatchAdSet
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid import AdSetCategoryBid
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid_resource import AdSetCategoryBidResource
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier import AdSetDisplayMultiplier
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_frequency_capping import AdSetFrequencyCapping
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_geo_location import AdSetGeoLocation
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_search_filter import AdSetSearchFilter
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting import AdSetTargeting
+from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting_rule import AdSetTargetingRule
+from criteo_api_marketingsolutions_v2023_04.model.application_summary_model import ApplicationSummaryModel
+from criteo_api_marketingsolutions_v2023_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+from criteo_api_marketingsolutions_v2023_04.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_marketingsolutions_v2023_04.model.audience import Audience
+from criteo_api_marketingsolutions_v2023_04.model.audience_attributes import AudienceAttributes
+from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
+from criteo_api_marketingsolutions_v2023_04.model.audience_name_description import AudienceNameDescription
+from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
+from criteo_api_marketingsolutions_v2023_04.model.campaign import Campaign
+from criteo_api_marketingsolutions_v2023_04.model.campaign_list_response import CampaignListResponse
+from criteo_api_marketingsolutions_v2023_04.model.campaign_read_resource import CampaignReadResource
+from criteo_api_marketingsolutions_v2023_04.model.campaign_response import CampaignResponse
+from criteo_api_marketingsolutions_v2023_04.model.campaign_search_filters import CampaignSearchFilters
+from criteo_api_marketingsolutions_v2023_04.model.campaign_search_request import CampaignSearchRequest
+from criteo_api_marketingsolutions_v2023_04.model.campaign_spend_limit import CampaignSpendLimit
+from criteo_api_marketingsolutions_v2023_04.model.common_problem import CommonProblem
+from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment import ContactlistAmendment
+from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
+from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment_request import ContactlistAmendmentRequest
+from criteo_api_marketingsolutions_v2023_04.model.contactlist_operation import ContactlistOperation
+from criteo_api_marketingsolutions_v2023_04.model.contactlist_operation_attributes import ContactlistOperationAttributes
+from criteo_api_marketingsolutions_v2023_04.model.criteo_api_error import CriteoApiError
+from criteo_api_marketingsolutions_v2023_04.model.criteo_api_warning import CriteoApiWarning
+from criteo_api_marketingsolutions_v2023_04.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
+from criteo_api_marketingsolutions_v2023_04.model.delete_audience_response import DeleteAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.entity_of_portfolio_message import EntityOfPortfolioMessage
+from criteo_api_marketingsolutions_v2023_04.model.error_code_response import ErrorCodeResponse
+from criteo_api_marketingsolutions_v2023_04.model.get_audiences_response import GetAudiencesResponse
+from criteo_api_marketingsolutions_v2023_04.model.get_portfolio_response import GetPortfolioResponse
+from criteo_api_marketingsolutions_v2023_04.model.modify_audience_response import ModifyAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.new_audience import NewAudience
+from criteo_api_marketingsolutions_v2023_04.model.new_audience_attributes import NewAudienceAttributes
+from criteo_api_marketingsolutions_v2023_04.model.new_audience_request import NewAudienceRequest
+from criteo_api_marketingsolutions_v2023_04.model.new_audience_response import NewAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
+from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
+from criteo_api_marketingsolutions_v2023_04.model.nillable_date_time import NillableDateTime
+from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set import PatchAdSet
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_bidding import PatchAdSetBidding
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_budget import PatchAdSetBudget
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
+from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_scheduling import PatchAdSetScheduling
+from criteo_api_marketingsolutions_v2023_04.model.patch_campaign import PatchCampaign
+from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_list_request import PatchCampaignListRequest
+from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
+from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_write_resource import PatchCampaignWriteResource
+from criteo_api_marketingsolutions_v2023_04.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
+from criteo_api_marketingsolutions_v2023_04.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
+from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
+from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_message import PlacementsReportQueryMessage
+from criteo_api_marketingsolutions_v2023_04.model.portfolio_message import PortfolioMessage
+from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+from criteo_api_marketingsolutions_v2023_04.model.problems_details import ProblemsDetails
+from criteo_api_marketingsolutions_v2023_04.model.read_ad_set import ReadAdSet
+from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_bidding import ReadAdSetBidding
+from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_budget import ReadAdSetBudget
+from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_schedule import ReadAdSetSchedule
+from criteo_api_marketingsolutions_v2023_04.model.read_model_ad_set_id import ReadModelAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.read_model_read_ad_set import ReadModelReadAdSet
+from criteo_api_marketingsolutions_v2023_04.model.replace_audience import ReplaceAudience
+from criteo_api_marketingsolutions_v2023_04.model.replace_audience_request import ReplaceAudienceRequest
+from criteo_api_marketingsolutions_v2023_04.model.replace_audience_response import ReplaceAudienceResponse
+from criteo_api_marketingsolutions_v2023_04.model.request_ad_set_search import RequestAdSetSearch
+from criteo_api_marketingsolutions_v2023_04.model.requests_ad_set_id import RequestsAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.requests_patch_ad_set import RequestsPatchAdSet
+from criteo_api_marketingsolutions_v2023_04.model.response_ad_set_id import ResponseAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.response_read_ad_set import ResponseReadAdSet
+from criteo_api_marketingsolutions_v2023_04.model.responses_ad_set_id import ResponsesAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.responses_read_ad_set import ResponsesReadAdSet
+from criteo_api_marketingsolutions_v2023_04.model.statistics_report_query_message import StatisticsReportQueryMessage
+from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
+from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_message import TransactionsReportQueryMessage
+from criteo_api_marketingsolutions_v2023_04.model.transparency_query_message import TransparencyQueryMessage
+from criteo_api_marketingsolutions_v2023_04.model.transparency_report_attributes import TransparencyReportAttributes
+from criteo_api_marketingsolutions_v2023_04.model.transparency_report_data_message import TransparencyReportDataMessage
+from criteo_api_marketingsolutions_v2023_04.model.transparency_report_entity_message import TransparencyReportEntityMessage
+from criteo_api_marketingsolutions_v2023_04.model.transparency_report_file import TransparencyReportFile
+from criteo_api_marketingsolutions_v2023_04.model.write_model_ad_set_id import WriteModelAdSetId
+from criteo_api_marketingsolutions_v2023_04.model.write_model_patch_ad_set import WriteModelPatchAdSet
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/criteo_api_marketingsolutions_v2023_01/rest.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
@@ -15,15 +15,15 @@
 import ssl
 from urllib.parse import urlencode
 from urllib.parse import urlparse
 from urllib.request import proxy_bypass_environment
 import urllib3
 import ipaddress
 
-from criteo_api_marketingsolutions_v2023_01.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from criteo_api_marketingsolutions_v2023_04.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/setup.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-marketingsolutions-sdk"
-VERSION = "2023.01.0.230427"
+VERSION = "2023.04.0.230427"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -20,21 +20,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_01
+import criteo_api_marketingsolutions_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.1.0.230427/test/test_gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230427/test/test_gateway_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 
-from criteo_api_marketingsolutions_v2023_01.api.gateway_api import GatewayApi
-from criteo_api_marketingsolutions_v2023_01.api_client_builder import ApiClientBuilder
-from criteo_api_marketingsolutions_v2023_01.rest import ApiException
+from criteo_api_marketingsolutions_v2023_04.api.gateway_api import GatewayApi
+from criteo_api_marketingsolutions_v2023_04.api_client_builder import ApiClientBuilder
+from criteo_api_marketingsolutions_v2023_04.rest import ApiException
 from example_application import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
```

