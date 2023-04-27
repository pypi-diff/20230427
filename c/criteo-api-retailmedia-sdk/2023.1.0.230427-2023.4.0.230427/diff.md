# Comparing `tmp/criteo-api-retailmedia-sdk-2023.1.0.230427.tar.gz` & `tmp/criteo-api-retailmedia-sdk-2023.4.0.230427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-retailmedia-sdk-2023.1.0.230427.tar", last modified: Thu Apr 27 13:30:36 2023, max compression
+gzip compressed data, was "criteo-api-retailmedia-sdk-2023.4.0.230427.tar", last modified: Thu Apr 27 13:30:51 2023, max compression
```

## Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427.tar` & `criteo-api-retailmedia-sdk-2023.4.0.230427.tar`

### file list

```diff
@@ -1,198 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.732598 criteo-api-retailmedia-sdk-2023.1.0.230427/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-27 13:30:36.732598 criteo-api-retailmedia-sdk-2023.1.0.230427/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.704597 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-27 13:30:36.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-04-27 13:30:36.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:30:36.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:30:36.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:30:36.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.704597 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.708597 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   335896 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39223 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.708597 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.732598 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/asset_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/asset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_create_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_update_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/audience_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/audience_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/audience_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/balance202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/category202204_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/choice_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/choice_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/choice_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/color_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_status_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_user_behavior_segment_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202110_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15072 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202207_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative_create_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative_update_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/customer_list_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/editable_campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/envelope_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/envelope_report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_line_item_capping202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_line_item_page202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_line_item_page_category202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_retailer_pages202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/files_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/files_variables_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/get_page_of_audiences_by_account_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/hyperlink_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/input_resource_of_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/input_resource_of_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_request_of_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/map_string.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/page_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/promoted_product202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/promoted_product202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/put_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_request_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_status_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_balance_campaign202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_creative202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/section.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/store_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/store_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/store_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/text_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/text_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/user_behavior_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/user_behavior_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    82568 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.732598 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/models/
--rw-r--r--   0 runner    (1001) docker     (123)    18586 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:30:36.732598 criteo-api-retailmedia-sdk-2023.1.0.230427/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:36.732598 criteo-api-retailmedia-sdk-2023.1.0.230427/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.1.0.230427/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.916910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.920910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.920910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   369292 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39223 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.920910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.992911 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/color_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/customer_list_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/map_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/page_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/page_type_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82568 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.992911 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.4.0.230427/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
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
-pip install criteo-api-retailmedia-sdk==2023.01.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_01
+import criteo_api_retailmedia_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/README.md` & `criteo-api-retailmedia-sdk-2023.4.0.230427/README.md`

 * *Files 7% similar despite different names*

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
-pip install criteo-api-retailmedia-sdk==2023.01.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_01
+import criteo_api_retailmedia_v2023_04
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
 
 Download the code or clone the repository locally, then execute the following command:
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_01
+import criteo_api_retailmedia_v2023_04
 ```
 
 ## Example
 Please see [test/example_application.py](test/example_application.py) for an example.
 
 ## Documentation for API Endpoints
 
@@ -98,16 +98,17 @@
  - [CreateRetailMediaAudienceV2](docs/CreateRetailMediaAudienceV2.md)
  - [CreateRetailMediaAudienceV2Attributes](docs/CreateRetailMediaAudienceV2Attributes.md)
  - [CreateRetailMediaAudienceV2Data](docs/CreateRetailMediaAudienceV2Data.md)
  - [CreateRetailMediaAudienceV2Request](docs/CreateRetailMediaAudienceV2Request.md)
  - [CreateUserBehaviorSegmentV2](docs/CreateUserBehaviorSegmentV2.md)
  - [Creative202110](docs/Creative202110.md)
  - [Creative202110ListResponse](docs/Creative202110ListResponse.md)
- - [Creative202207](docs/Creative202207.md)
- - [Creative202207Response](docs/Creative202207Response.md)
+ - [Creative202210](docs/Creative202210.md)
+ - [Creative202210ListResponse](docs/Creative202210ListResponse.md)
+ - [Creative202210Response](docs/Creative202210Response.md)
  - [CreativeCreateModel202207](docs/CreativeCreateModel202207.md)
  - [CreativeUpdateModel202207](docs/CreativeUpdateModel202207.md)
  - [CustomerListDetails](docs/CustomerListDetails.md)
  - [EditableCampaignAttributesV202301](docs/EditableCampaignAttributesV202301.md)
  - [EnvelopeReportRequest](docs/EnvelopeReportRequest.md)
  - [EnvelopeReportStatus](docs/EnvelopeReportStatus.md)
  - [Error](docs/Error.md)
@@ -162,14 +163,15 @@
  - [KeywordTarget202110Request](docs/KeywordTarget202110Request.md)
  - [KeywordTarget202110Response](docs/KeywordTarget202110Response.md)
  - [LineItemBidMultipliers](docs/LineItemBidMultipliers.md)
  - [LineItemBidMultipliersRequest](docs/LineItemBidMultipliersRequest.md)
  - [LineItemBidMultipliersResponse](docs/LineItemBidMultipliersResponse.md)
  - [MapString](docs/MapString.md)
  - [PageMetadata](docs/PageMetadata.md)
+ - [PageTypeEnvironment](docs/PageTypeEnvironment.md)
  - [PostCampaignV202301](docs/PostCampaignV202301.md)
  - [PreferredLineItem202110PagedListResponse](docs/PreferredLineItem202110PagedListResponse.md)
  - [PreferredLineItem202110Response](docs/PreferredLineItem202110Response.md)
  - [PreferredLineItemCreateModel202110Request](docs/PreferredLineItemCreateModel202110Request.md)
  - [PreferredLineItemUpdateModel202110Request](docs/PreferredLineItemUpdateModel202110Request.md)
  - [ProblemDetails](docs/ProblemDetails.md)
  - [PromotedProduct202110ListRequest](docs/PromotedProduct202110ListRequest.md)
@@ -182,26 +184,44 @@
  - [ResourceOfAuctionLineItem](docs/ResourceOfAuctionLineItem.md)
  - [ResourceOfAuctionLineItemUpdateModel](docs/ResourceOfAuctionLineItemUpdateModel.md)
  - [ResourceOfBalance202110](docs/ResourceOfBalance202110.md)
  - [ResourceOfBalanceCampaign202110](docs/ResourceOfBalanceCampaign202110.md)
  - [ResourceOfCategory202204](docs/ResourceOfCategory202204.md)
  - [ResourceOfCommonLineItem](docs/ResourceOfCommonLineItem.md)
  - [ResourceOfCreative202110](docs/ResourceOfCreative202110.md)
- - [ResourceOfCreative202207](docs/ResourceOfCreative202207.md)
+ - [ResourceOfCreative202210](docs/ResourceOfCreative202210.md)
  - [ResourceOfLineItemBidMultipliers](docs/ResourceOfLineItemBidMultipliers.md)
  - [ResourceOfPreferredLineItem202110](docs/ResourceOfPreferredLineItem202110.md)
  - [ResourceOfPreferredLineItemUpdateModel202110](docs/ResourceOfPreferredLineItemUpdateModel202110.md)
  - [ResourceOfPromotedProduct202110](docs/ResourceOfPromotedProduct202110.md)
  - [ResourceOfTemplate](docs/ResourceOfTemplate.md)
  - [RetailMediaAudience](docs/RetailMediaAudience.md)
  - [RetailMediaAudienceAttributes](docs/RetailMediaAudienceAttributes.md)
  - [RetailMediaAudienceV2](docs/RetailMediaAudienceV2.md)
  - [RetailMediaAudienceV2Attributes](docs/RetailMediaAudienceV2Attributes.md)
  - [RetailMediaAudienceV2ListResponse](docs/RetailMediaAudienceV2ListResponse.md)
  - [RetailMediaAudienceV2Response](docs/RetailMediaAudienceV2Response.md)
+ - [RetailMediaExternalv1AddRemoveKeywordModel](docs/RetailMediaExternalv1AddRemoveKeywordModel.md)
+ - [RetailMediaExternalv1AddRemoveKeywordsModel](docs/RetailMediaExternalv1AddRemoveKeywordsModel.md)
+ - [RetailMediaExternalv1AddRemoveKeywordsModelRequest](docs/RetailMediaExternalv1AddRemoveKeywordsModelRequest.md)
+ - [RetailMediaExternalv1AddRemoveKeywordsModelResource](docs/RetailMediaExternalv1AddRemoveKeywordsModelResource.md)
+ - [RetailMediaExternalv1InputKeywordsModel](docs/RetailMediaExternalv1InputKeywordsModel.md)
+ - [RetailMediaExternalv1KeywordDataModel](docs/RetailMediaExternalv1KeywordDataModel.md)
+ - [RetailMediaExternalv1KeywordsModel](docs/RetailMediaExternalv1KeywordsModel.md)
+ - [RetailMediaExternalv1KeywordsModelResource](docs/RetailMediaExternalv1KeywordsModelResource.md)
+ - [RetailMediaExternalv1KeywordsModelResponse](docs/RetailMediaExternalv1KeywordsModelResponse.md)
+ - [RetailMediaExternalv1ProblemDetails](docs/RetailMediaExternalv1ProblemDetails.md)
+ - [RetailMediaExternalv1ProposalStatusModel](docs/RetailMediaExternalv1ProposalStatusModel.md)
+ - [RetailMediaExternalv1ProposalStatusModelResource](docs/RetailMediaExternalv1ProposalStatusModelResource.md)
+ - [RetailMediaExternalv1ProposalStatusModelResponse](docs/RetailMediaExternalv1ProposalStatusModelResponse.md)
+ - [RetailMediaExternalv1ResourceOutcome](docs/RetailMediaExternalv1ResourceOutcome.md)
+ - [RetailMediaExternalv1SetBidModel](docs/RetailMediaExternalv1SetBidModel.md)
+ - [RetailMediaExternalv1SetBidsModel](docs/RetailMediaExternalv1SetBidsModel.md)
+ - [RetailMediaExternalv1SetBidsModelRequest](docs/RetailMediaExternalv1SetBidsModelRequest.md)
+ - [RetailMediaExternalv1SetBidsModelResource](docs/RetailMediaExternalv1SetBidsModelResource.md)
  - [Section](docs/Section.md)
  - [StoreIdsUpdateModel202110Request](docs/StoreIdsUpdateModel202110Request.md)
  - [StoreTarget202110Request](docs/StoreTarget202110Request.md)
  - [StoreTarget202110Response](docs/StoreTarget202110Response.md)
  - [Template](docs/Template.md)
  - [TemplateListResponse](docs/TemplateListResponse.md)
  - [TemplateResponse](docs/TemplateResponse.md)
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
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
-pip install criteo-api-retailmedia-sdk==2023.01.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_01
+import criteo_api_retailmedia_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,188 +2,208 @@
 setup.cfg
 setup.py
 criteo_api_retailmedia_sdk.egg-info/PKG-INFO
 criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
 criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
 criteo_api_retailmedia_sdk.egg-info/requires.txt
 criteo_api_retailmedia_sdk.egg-info/top_level.txt
-criteo_api_retailmedia_v2023_01/__init__.py
-criteo_api_retailmedia_v2023_01/api_client.py
-criteo_api_retailmedia_v2023_01/api_client_builder.py
-criteo_api_retailmedia_v2023_01/configuration.py
-criteo_api_retailmedia_v2023_01/criteo_api_client.py
-criteo_api_retailmedia_v2023_01/criteo_auth.py
-criteo_api_retailmedia_v2023_01/criteo_rest.py
-criteo_api_retailmedia_v2023_01/exceptions.py
-criteo_api_retailmedia_v2023_01/model_utils.py
-criteo_api_retailmedia_v2023_01/rest.py
-criteo_api_retailmedia_v2023_01/api/__init__.py
-criteo_api_retailmedia_v2023_01/api/analytics_api.py
-criteo_api_retailmedia_v2023_01/api/audience_api.py
-criteo_api_retailmedia_v2023_01/api/campaign_api.py
-criteo_api_retailmedia_v2023_01/api/gateway_api.py
-criteo_api_retailmedia_v2023_01/apis/__init__.py
-criteo_api_retailmedia_v2023_01/model/__init__.py
-criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py
-criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py
-criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py
-criteo_api_retailmedia_v2023_01/model/application_summary_model.py
-criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py
-criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py
-criteo_api_retailmedia_v2023_01/model/asset.py
-criteo_api_retailmedia_v2023_01/model/asset_resource.py
-criteo_api_retailmedia_v2023_01/model/asset_response.py
-criteo_api_retailmedia_v2023_01/model/auction_line_item_create_model_request.py
-criteo_api_retailmedia_v2023_01/model/auction_line_item_paged_list_response.py
-criteo_api_retailmedia_v2023_01/model/auction_line_item_response.py
-criteo_api_retailmedia_v2023_01/model/auction_line_item_update_model_request.py
-criteo_api_retailmedia_v2023_01/model/audience_ids_update_model202110_request.py
-criteo_api_retailmedia_v2023_01/model/audience_target202110_request.py
-criteo_api_retailmedia_v2023_01/model/audience_target202110_response.py
-criteo_api_retailmedia_v2023_01/model/bad_request.py
-criteo_api_retailmedia_v2023_01/model/balance202110_paged_list_response.py
-criteo_api_retailmedia_v2023_01/model/balance_campaign202110_list_request.py
-criteo_api_retailmedia_v2023_01/model/balance_campaign202110_paged_list_response.py
-criteo_api_retailmedia_v2023_01/model/campaign_attributes_v202301.py
-criteo_api_retailmedia_v2023_01/model/campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/category202204.py
-criteo_api_retailmedia_v2023_01/model/category202204_list_response.py
-criteo_api_retailmedia_v2023_01/model/choice_option.py
-criteo_api_retailmedia_v2023_01/model/choice_variable_specification.py
-criteo_api_retailmedia_v2023_01/model/choice_variable_value.py
-criteo_api_retailmedia_v2023_01/model/color_variable_value.py
-criteo_api_retailmedia_v2023_01/model/common_error.py
-criteo_api_retailmedia_v2023_01/model/common_line_item_paged_list_response.py
-criteo_api_retailmedia_v2023_01/model/common_line_item_response.py
-criteo_api_retailmedia_v2023_01/model/common_problem.py
-criteo_api_retailmedia_v2023_01/model/common_status_code_response.py
-criteo_api_retailmedia_v2023_01/model/common_warning.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_attributes.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_body.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_request.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_response.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_attributes.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_data.py
-criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_request.py
-criteo_api_retailmedia_v2023_01/model/create_user_behavior_segment_v2.py
-criteo_api_retailmedia_v2023_01/model/creative202110.py
-criteo_api_retailmedia_v2023_01/model/creative202110_list_response.py
-criteo_api_retailmedia_v2023_01/model/creative202207.py
-criteo_api_retailmedia_v2023_01/model/creative202207_response.py
-criteo_api_retailmedia_v2023_01/model/creative_create_model202207.py
-criteo_api_retailmedia_v2023_01/model/creative_update_model202207.py
-criteo_api_retailmedia_v2023_01/model/customer_list_details.py
-criteo_api_retailmedia_v2023_01/model/editable_campaign_attributes_v202301.py
-criteo_api_retailmedia_v2023_01/model/envelope_report_request.py
-criteo_api_retailmedia_v2023_01/model/envelope_report_status.py
-criteo_api_retailmedia_v2023_01/model/error.py
-criteo_api_retailmedia_v2023_01/model/external_account.py
-criteo_api_retailmedia_v2023_01/model/external_add_to_basket_ids_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/external_add_to_basket_target202110.py
-criteo_api_retailmedia_v2023_01/model/external_auction_line_item.py
-criteo_api_retailmedia_v2023_01/model/external_auction_line_item_create_model.py
-criteo_api_retailmedia_v2023_01/model/external_auction_line_item_update_model.py
-criteo_api_retailmedia_v2023_01/model/external_audience_ids_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/external_audience_target202110.py
-criteo_api_retailmedia_v2023_01/model/external_balance202110.py
-criteo_api_retailmedia_v2023_01/model/external_brand.py
-criteo_api_retailmedia_v2023_01/model/external_catalog_request.py
-criteo_api_retailmedia_v2023_01/model/external_catalog_status.py
-criteo_api_retailmedia_v2023_01/model/external_common_line_item.py
-criteo_api_retailmedia_v2023_01/model/external_keyword_target202110.py
-criteo_api_retailmedia_v2023_01/model/external_line_item_capping202110.py
-criteo_api_retailmedia_v2023_01/model/external_line_item_page202110.py
-criteo_api_retailmedia_v2023_01/model/external_line_item_page_category202110.py
-criteo_api_retailmedia_v2023_01/model/external_preferred_line_item202110.py
-criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_create_model202110.py
-criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/external_promoted_product202110.py
-criteo_api_retailmedia_v2023_01/model/external_retailer.py
-criteo_api_retailmedia_v2023_01/model/external_retailer_pages202110.py
-criteo_api_retailmedia_v2023_01/model/external_store_ids_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/external_store_target202110.py
-criteo_api_retailmedia_v2023_01/model/files_variable_value.py
-criteo_api_retailmedia_v2023_01/model/files_variables_specification.py
-criteo_api_retailmedia_v2023_01/model/get_page_of_audiences_by_account_id_response.py
-criteo_api_retailmedia_v2023_01/model/hyperlink_variable_value.py
-criteo_api_retailmedia_v2023_01/model/input_resource_of_auction_line_item_create_model.py
-criteo_api_retailmedia_v2023_01/model/input_resource_of_preferred_line_item_create_model202110.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
-criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_account.py
-criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_brand.py
-criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_retailer.py
-criteo_api_retailmedia_v2023_01/model/json_api_request_of_catalog_request.py
-criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_catalog_status.py
-criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py
-criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py
-criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py
-criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py
-criteo_api_retailmedia_v2023_01/model/map_string.py
-criteo_api_retailmedia_v2023_01/model/page_metadata.py
-criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py
-criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py
-criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py
-criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py
-criteo_api_retailmedia_v2023_01/model/problem_details.py
-criteo_api_retailmedia_v2023_01/model/promoted_product202110_list_request.py
-criteo_api_retailmedia_v2023_01/model/promoted_product202110_paged_list_response.py
-criteo_api_retailmedia_v2023_01/model/put_campaign_v202301.py
-criteo_api_retailmedia_v2023_01/model/report_request.py
-criteo_api_retailmedia_v2023_01/model/report_request_attributes.py
-criteo_api_retailmedia_v2023_01/model/report_status.py
-criteo_api_retailmedia_v2023_01/model/report_status_attributes.py
-criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item.py
-criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item_update_model.py
-criteo_api_retailmedia_v2023_01/model/resource_of_balance202110.py
-criteo_api_retailmedia_v2023_01/model/resource_of_balance_campaign202110.py
-criteo_api_retailmedia_v2023_01/model/resource_of_category202204.py
-criteo_api_retailmedia_v2023_01/model/resource_of_common_line_item.py
-criteo_api_retailmedia_v2023_01/model/resource_of_creative202110.py
-criteo_api_retailmedia_v2023_01/model/resource_of_creative202207.py
-criteo_api_retailmedia_v2023_01/model/resource_of_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item202110.py
-criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/resource_of_promoted_product202110.py
-criteo_api_retailmedia_v2023_01/model/resource_of_template.py
-criteo_api_retailmedia_v2023_01/model/retail_media_audience.py
-criteo_api_retailmedia_v2023_01/model/retail_media_audience_attributes.py
-criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2.py
-criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_attributes.py
-criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_list_response.py
-criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_response.py
-criteo_api_retailmedia_v2023_01/model/section.py
-criteo_api_retailmedia_v2023_01/model/store_ids_update_model202110_request.py
-criteo_api_retailmedia_v2023_01/model/store_target202110_request.py
-criteo_api_retailmedia_v2023_01/model/store_target202110_response.py
-criteo_api_retailmedia_v2023_01/model/template.py
-criteo_api_retailmedia_v2023_01/model/template_list_response.py
-criteo_api_retailmedia_v2023_01/model/template_response.py
-criteo_api_retailmedia_v2023_01/model/template_variable.py
-criteo_api_retailmedia_v2023_01/model/template_variable_value.py
-criteo_api_retailmedia_v2023_01/model/text_variable_specification.py
-criteo_api_retailmedia_v2023_01/model/text_variable_value.py
-criteo_api_retailmedia_v2023_01/model/user_behavior_details.py
-criteo_api_retailmedia_v2023_01/model/user_behavior_details_v2.py
-criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_target202110.py
-criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_ids_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_target202110.py
-criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py
-criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_ids_update_model202110.py
-criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_target202110.py
-criteo_api_retailmedia_v2023_01/models/__init__.py
+criteo_api_retailmedia_v2023_04/__init__.py
+criteo_api_retailmedia_v2023_04/api_client.py
+criteo_api_retailmedia_v2023_04/api_client_builder.py
+criteo_api_retailmedia_v2023_04/configuration.py
+criteo_api_retailmedia_v2023_04/criteo_api_client.py
+criteo_api_retailmedia_v2023_04/criteo_auth.py
+criteo_api_retailmedia_v2023_04/criteo_rest.py
+criteo_api_retailmedia_v2023_04/exceptions.py
+criteo_api_retailmedia_v2023_04/model_utils.py
+criteo_api_retailmedia_v2023_04/rest.py
+criteo_api_retailmedia_v2023_04/api/__init__.py
+criteo_api_retailmedia_v2023_04/api/analytics_api.py
+criteo_api_retailmedia_v2023_04/api/audience_api.py
+criteo_api_retailmedia_v2023_04/api/campaign_api.py
+criteo_api_retailmedia_v2023_04/api/gateway_api.py
+criteo_api_retailmedia_v2023_04/apis/__init__.py
+criteo_api_retailmedia_v2023_04/model/__init__.py
+criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py
+criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py
+criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py
+criteo_api_retailmedia_v2023_04/model/application_summary_model.py
+criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py
+criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py
+criteo_api_retailmedia_v2023_04/model/asset.py
+criteo_api_retailmedia_v2023_04/model/asset_resource.py
+criteo_api_retailmedia_v2023_04/model/asset_response.py
+criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py
+criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py
+criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py
+criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py
+criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py
+criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py
+criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py
+criteo_api_retailmedia_v2023_04/model/bad_request.py
+criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py
+criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py
+criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py
+criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py
+criteo_api_retailmedia_v2023_04/model/campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/category202204.py
+criteo_api_retailmedia_v2023_04/model/category202204_list_response.py
+criteo_api_retailmedia_v2023_04/model/choice_option.py
+criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py
+criteo_api_retailmedia_v2023_04/model/choice_variable_value.py
+criteo_api_retailmedia_v2023_04/model/color_variable_value.py
+criteo_api_retailmedia_v2023_04/model/common_error.py
+criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py
+criteo_api_retailmedia_v2023_04/model/common_line_item_response.py
+criteo_api_retailmedia_v2023_04/model/common_problem.py
+criteo_api_retailmedia_v2023_04/model/common_status_code_response.py
+criteo_api_retailmedia_v2023_04/model/common_warning.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py
+criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py
+criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py
+criteo_api_retailmedia_v2023_04/model/creative202110.py
+criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py
+criteo_api_retailmedia_v2023_04/model/creative202210.py
+criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py
+criteo_api_retailmedia_v2023_04/model/creative202210_response.py
+criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py
+criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py
+criteo_api_retailmedia_v2023_04/model/customer_list_details.py
+criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py
+criteo_api_retailmedia_v2023_04/model/envelope_report_request.py
+criteo_api_retailmedia_v2023_04/model/envelope_report_status.py
+criteo_api_retailmedia_v2023_04/model/error.py
+criteo_api_retailmedia_v2023_04/model/external_account.py
+criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py
+criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py
+criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py
+criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py
+criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py
+criteo_api_retailmedia_v2023_04/model/external_balance202110.py
+criteo_api_retailmedia_v2023_04/model/external_brand.py
+criteo_api_retailmedia_v2023_04/model/external_catalog_request.py
+criteo_api_retailmedia_v2023_04/model/external_catalog_status.py
+criteo_api_retailmedia_v2023_04/model/external_common_line_item.py
+criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py
+criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py
+criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py
+criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py
+criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py
+criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py
+criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py
+criteo_api_retailmedia_v2023_04/model/external_retailer.py
+criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py
+criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/external_store_target202110.py
+criteo_api_retailmedia_v2023_04/model/files_variable_value.py
+criteo_api_retailmedia_v2023_04/model/files_variables_specification.py
+criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py
+criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py
+criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py
+criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py
+criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py
+criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py
+criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py
+criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py
+criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py
+criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py
+criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py
+criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py
+criteo_api_retailmedia_v2023_04/model/map_string.py
+criteo_api_retailmedia_v2023_04/model/page_metadata.py
+criteo_api_retailmedia_v2023_04/model/page_type_environment.py
+criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py
+criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py
+criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py
+criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py
+criteo_api_retailmedia_v2023_04/model/problem_details.py
+criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py
+criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py
+criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py
+criteo_api_retailmedia_v2023_04/model/report_request.py
+criteo_api_retailmedia_v2023_04/model/report_request_attributes.py
+criteo_api_retailmedia_v2023_04/model/report_status.py
+criteo_api_retailmedia_v2023_04/model/report_status_attributes.py
+criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py
+criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py
+criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py
+criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py
+criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py
+criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py
+criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py
+criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py
+criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py
+criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py
+criteo_api_retailmedia_v2023_04/model/resource_of_template.py
+criteo_api_retailmedia_v2023_04/model/retail_media_audience.py
+criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py
+criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py
+criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py
+criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py
+criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py
+criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py
+criteo_api_retailmedia_v2023_04/model/section.py
+criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py
+criteo_api_retailmedia_v2023_04/model/store_target202110_request.py
+criteo_api_retailmedia_v2023_04/model/store_target202110_response.py
+criteo_api_retailmedia_v2023_04/model/template.py
+criteo_api_retailmedia_v2023_04/model/template_list_response.py
+criteo_api_retailmedia_v2023_04/model/template_response.py
+criteo_api_retailmedia_v2023_04/model/template_variable.py
+criteo_api_retailmedia_v2023_04/model/template_variable_value.py
+criteo_api_retailmedia_v2023_04/model/text_variable_specification.py
+criteo_api_retailmedia_v2023_04/model/text_variable_value.py
+criteo_api_retailmedia_v2023_04/model/user_behavior_details.py
+criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py
+criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py
+criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py
+criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py
+criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py
+criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py
+criteo_api_retailmedia_v2023_04/models/__init__.py
 test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/__init__.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/__init__.py`

 * *Files 10% similar despite different names*

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
-from criteo_api_retailmedia_v2023_01.api_client import ApiClient
-from criteo_api_retailmedia_v2023_01.criteo_api_client import CriteoApiClient
-from criteo_api_retailmedia_v2023_01.api_client_builder import ApiClientBuilder
+from criteo_api_retailmedia_v2023_04.api_client import ApiClient
+from criteo_api_retailmedia_v2023_04.criteo_api_client import CriteoApiClient
+from criteo_api_retailmedia_v2023_04.api_client_builder import ApiClientBuilder
 
 # import Configuration
-from criteo_api_retailmedia_v2023_01.configuration import Configuration
+from criteo_api_retailmedia_v2023_04.configuration import Configuration
 
 # import exceptions
-from criteo_api_retailmedia_v2023_01.exceptions import OpenApiException
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
-from criteo_api_retailmedia_v2023_01.exceptions import ApiTypeError
-from criteo_api_retailmedia_v2023_01.exceptions import ApiValueError
-from criteo_api_retailmedia_v2023_01.exceptions import ApiKeyError
-from criteo_api_retailmedia_v2023_01.exceptions import ApiException
+from criteo_api_retailmedia_v2023_04.exceptions import OpenApiException
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiTypeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiValueError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiKeyError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiException
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/analytics_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/analytics_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_01.model.bad_request import BadRequest
-from criteo_api_retailmedia_v2023_01.model.envelope_report_request import EnvelopeReportRequest
-from criteo_api_retailmedia_v2023_01.model.envelope_report_status import EnvelopeReportStatus
+from criteo_api_retailmedia_v2023_04.model.bad_request import BadRequest
+from criteo_api_retailmedia_v2023_04.model.envelope_report_request import EnvelopeReportRequest
+from criteo_api_retailmedia_v2023_04.model.envelope_report_status import EnvelopeReportStatus
 
 
 class AnalyticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -40,15 +40,15 @@
         self.get_report_output_endpoint = _Endpoint(
             settings={
                 'response_type': (int,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/reports/{reportId}/output',
+                'endpoint_path': '/2023-04/retail-media/reports/{reportId}/output',
                 'operation_id': 'get_report_output',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'report_id',
@@ -92,15 +92,15 @@
         self.get_report_status_endpoint = _Endpoint(
             settings={
                 'response_type': (EnvelopeReportStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/reports/{reportId}/status',
+                'endpoint_path': '/2023-04/retail-media/reports/{reportId}/status',
                 'operation_id': 'get_report_status',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'report_id',
@@ -144,15 +144,15 @@
         self.request_campaign_report_endpoint = _Endpoint(
             settings={
                 'response_type': (EnvelopeReportStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/reports/campaigns',
+                'endpoint_path': '/2023-04/retail-media/reports/campaigns',
                 'operation_id': 'request_campaign_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'envelope_report_request',
@@ -197,15 +197,15 @@
         self.request_line_item_report_endpoint = _Endpoint(
             settings={
                 'response_type': (EnvelopeReportStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/reports/line-items',
+                'endpoint_path': '/2023-04/retail-media/reports/line-items',
                 'operation_id': 'request_line_item_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'envelope_report_request',
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/audience_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/audience_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_01.model.common_status_code_response import CommonStatusCodeResponse
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
-from criteo_api_retailmedia_v2023_01.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
+from criteo_api_retailmedia_v2023_04.model.common_status_code_response import CommonStatusCodeResponse
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
+from criteo_api_retailmedia_v2023_04.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
 
 
 class AudienceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -44,15 +44,15 @@
         self.create_audience_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateRetailMediaAudienceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/audiences',
                 'operation_id': 'create_audience',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -103,15 +103,15 @@
         self.create_retail_media_audience_v2_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaAudienceV2Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/v2/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-04/retail-media/v2/accounts/{accountId}/audiences',
                 'operation_id': 'create_retail_media_audience_v2',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -162,15 +162,15 @@
         self.get_audiences_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (GetPageOfAudiencesByAccountIdResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/audiences',
                 'operation_id': 'get_audiences_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -230,15 +230,15 @@
         self.get_retail_media_audience_v2_list_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaAudienceV2ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/v2/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-04/retail-media/v2/accounts/{accountId}/audiences',
                 'operation_id': 'get_retail_media_audience_v2_list_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/campaign_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/campaign_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,99 +1,165 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_01.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.asset_response import AssetResponse
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_response import AuctionLineItemResponse
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
-from criteo_api_retailmedia_v2023_01.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.audience_target202110_request import AudienceTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.audience_target202110_response import AudienceTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.balance202110_paged_list_response import Balance202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
-from criteo_api_retailmedia_v2023_01.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.category202204 import Category202204
-from criteo_api_retailmedia_v2023_01.model.category202204_list_response import Category202204ListResponse
-from criteo_api_retailmedia_v2023_01.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_01.model.common_line_item_response import CommonLineItemResponse
-from criteo_api_retailmedia_v2023_01.model.creative202110_list_response import Creative202110ListResponse
-from criteo_api_retailmedia_v2023_01.model.creative202207_response import Creative202207Response
-from criteo_api_retailmedia_v2023_01.model.creative_create_model202207 import CreativeCreateModel202207
-from criteo_api_retailmedia_v2023_01.model.creative_update_model202207 import CreativeUpdateModel202207
-from criteo_api_retailmedia_v2023_01.model.external_retailer_pages202110 import ExternalRetailerPages202110
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
-from criteo_api_retailmedia_v2023_01.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
-from criteo_api_retailmedia_v2023_01.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
-from criteo_api_retailmedia_v2023_01.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_01.model.keyword_target202110_request import KeywordTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.keyword_target202110_response import KeywordTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
-from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
-from criteo_api_retailmedia_v2023_01.model.post_campaign_v202301 import PostCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item202110_response import PreferredLineItem202110Response
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
-from criteo_api_retailmedia_v2023_01.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.put_campaign_v202301 import PutCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.store_target202110_request import StoreTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.store_target202110_response import StoreTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.template_list_response import TemplateListResponse
-from criteo_api_retailmedia_v2023_01.model.template_response import TemplateResponse
+from criteo_api_retailmedia_v2023_04.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.asset_response import AssetResponse
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_response import AuctionLineItemResponse
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
+from criteo_api_retailmedia_v2023_04.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.audience_target202110_request import AudienceTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.audience_target202110_response import AudienceTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.balance202110_paged_list_response import Balance202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
+from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.category202204 import Category202204
+from criteo_api_retailmedia_v2023_04.model.category202204_list_response import Category202204ListResponse
+from criteo_api_retailmedia_v2023_04.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_04.model.common_line_item_response import CommonLineItemResponse
+from criteo_api_retailmedia_v2023_04.model.creative202110_list_response import Creative202110ListResponse
+from criteo_api_retailmedia_v2023_04.model.creative202210_list_response import Creative202210ListResponse
+from criteo_api_retailmedia_v2023_04.model.creative202210_response import Creative202210Response
+from criteo_api_retailmedia_v2023_04.model.creative_create_model202207 import CreativeCreateModel202207
+from criteo_api_retailmedia_v2023_04.model.creative_update_model202207 import CreativeUpdateModel202207
+from criteo_api_retailmedia_v2023_04.model.external_retailer_pages202110 import ExternalRetailerPages202110
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
+from criteo_api_retailmedia_v2023_04.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
+from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
+from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_04.model.keyword_target202110_request import KeywordTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.keyword_target202110_response import KeywordTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
+from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
+from criteo_api_retailmedia_v2023_04.model.post_campaign_v202301 import PostCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_response import PreferredLineItem202110Response
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
+from criteo_api_retailmedia_v2023_04.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.put_campaign_v202301 import PutCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model_request import RetailMediaExternalv1AddRemoveKeywordsModelRequest
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model_response import RetailMediaExternalv1KeywordsModelResponse
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model_response import RetailMediaExternalv1ProposalStatusModelResponse
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_resource_outcome import RetailMediaExternalv1ResourceOutcome
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model_request import RetailMediaExternalv1SetBidsModelRequest
+from criteo_api_retailmedia_v2023_04.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.store_target202110_request import StoreTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.store_target202110_response import StoreTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.template_list_response import TemplateListResponse
+from criteo_api_retailmedia_v2023_04.model.template_response import TemplateResponse
 
 
 class CampaignApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.add_remove_keywords_endpoint = _Endpoint(
+            settings={
+                'response_type': (RetailMediaExternalv1ResourceOutcome,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-04/retail-media/line-items/{id}/keywords/add-remove',
+                'operation_id': 'add_remove_keywords',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'retail_media_externalv1_add_remove_keywords_model_request',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'retail_media_externalv1_add_remove_keywords_model_request':
+                        (RetailMediaExternalv1AddRemoveKeywordsModelRequest,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'retail_media_externalv1_add_remove_keywords_model_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.create_asset_endpoint = _Endpoint(
             settings={
                 'response_type': (AssetResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/assets',
+                'endpoint_path': '/2023-04/retail-media/assets',
                 'operation_id': 'create_asset',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'asset_file',
@@ -134,22 +200,130 @@
                 ],
                 'content_type': [
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
+        self.fetch_keywords_endpoint = _Endpoint(
+            settings={
+                'response_type': (RetailMediaExternalv1KeywordsModelResponse,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-04/retail-media/line-items/{id}/keywords',
+                'operation_id': 'fetch_keywords',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.fetch_proposal_endpoint = _Endpoint(
+            settings={
+                'response_type': (RetailMediaExternalv1ProposalStatusModelResponse,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-04/retail-media/preferred-deal-line-items/{id}/proposal',
+                'operation_id': 'fetch_proposal',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_api202110_external_account_balances_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Balance202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{account-id}/balances',
+                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/balances',
                 'operation_id': 'get_api202110_external_account_balances_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -209,15 +383,15 @@
         self.get_api202110_external_account_creatives_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202110ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{account-id}/creatives',
+                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives',
                 'operation_id': 'get_api202110_external_account_creatives_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -261,15 +435,15 @@
         self.get_api202110_external_auction_line_item_targeting_keywords_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/auction-line-items/{line-item-id}/targeting/keywords',
+                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords',
                 'operation_id': 'get_api202110_external_auction_line_item_targeting_keywords_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -313,15 +487,15 @@
         self.get_api202110_external_balance_campaigns_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/balances/{balance-id}/campaigns',
+                'endpoint_path': '/2023-04/retail-media/balances/{balance-id}/campaigns',
                 'operation_id': 'get_api202110_external_balance_campaigns_by_balance_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -381,15 +555,15 @@
         self.get_api202110_external_campaign_preferred_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/campaigns/{campaign-id}/preferred-line-items',
+                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/preferred-line-items',
                 'operation_id': 'get_api202110_external_campaign_preferred_line_items_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -449,15 +623,15 @@
         self.get_api202110_external_line_item_products_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}/products',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products',
                 'operation_id': 'get_api202110_external_line_item_products_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -517,15 +691,15 @@
         self.get_api202110_external_preferred_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}',
                 'operation_id': 'get_api202110_external_preferred_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -569,15 +743,15 @@
         self.get_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -621,15 +795,15 @@
         self.get_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -673,15 +847,15 @@
         self.get_api202110_external_preferred_line_item_targeting_stores_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_stores_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -725,15 +899,15 @@
         self.get_api202110_external_retailer_pages_by_retailer_id_endpoint = _Endpoint(
             settings={
                 'response_type': (ExternalRetailerPages202110,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/retailers/{retailerId}/pages',
+                'endpoint_path': '/2023-04/retail-media/retailers/{retailerId}/pages',
                 'operation_id': 'get_api202110_external_retailer_pages_by_retailer_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -777,15 +951,15 @@
         self.get_api202204_external_categorie_by_category_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Category202204,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/categories/{categoryId}',
+                'endpoint_path': '/2023-04/retail-media/categories/{categoryId}',
                 'operation_id': 'get_api202204_external_categorie_by_category_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'category_id',
@@ -829,15 +1003,15 @@
         self.get_api202204_external_categories_endpoint = _Endpoint(
             settings={
                 'response_type': (Category202204ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/categories',
+                'endpoint_path': '/2023-04/retail-media/categories',
                 'operation_id': 'get_api202204_external_categories',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -899,92 +1073,90 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_api202207_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
+        self.get_api202207_external_retailer_by_retailer_id_templatestemplate_id_endpoint = _Endpoint(
             settings={
-                'response_type': (Creative202207Response,),
+                'response_type': (TemplateResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{account-id}/creatives/{creative-id}',
-                'operation_id': 'get_api202207_external_account_by_account_id_creativescreative_id',
+                'endpoint_path': '/2023-04/retail-media/retailers/{retailer-id}/templates/{template-id}',
+                'operation_id': 'get_api202207_external_retailer_by_retailer_id_templatestemplate_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'account_id',
-                    'creative_id',
+                    'retailer_id',
+                    'template_id',
                 ],
                 'required': [
-                    'account_id',
-                    'creative_id',
+                    'retailer_id',
+                    'template_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'account_id':
-                        (str,),
-                    'creative_id':
-                        (str,),
+                    'retailer_id':
+                        (int,),
+                    'template_id':
+                        (int,),
                 },
                 'attribute_map': {
-                    'account_id': 'account-id',
-                    'creative_id': 'creative-id',
+                    'retailer_id': 'retailer-id',
+                    'template_id': 'template-id',
                 },
                 'location_map': {
-                    'account_id': 'path',
-                    'creative_id': 'path',
+                    'retailer_id': 'path',
+                    'template_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_api202207_external_retailer_by_retailer_id_templatestemplate_id_endpoint = _Endpoint(
+        self.get_api202207_external_retailer_templates_by_retailer_id_endpoint = _Endpoint(
             settings={
-                'response_type': (TemplateResponse,),
+                'response_type': (TemplateListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/retailers/{retailer-id}/templates/{template-id}',
-                'operation_id': 'get_api202207_external_retailer_by_retailer_id_templatestemplate_id',
+                'endpoint_path': '/2023-04/retail-media/retailers/{retailer-id}/templates',
+                'operation_id': 'get_api202207_external_retailer_templates_by_retailer_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
-                    'template_id',
                 ],
                 'required': [
                     'retailer_id',
-                    'template_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -993,76 +1165,78 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'retailer_id':
                         (int,),
-                    'template_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'retailer_id': 'retailer-id',
-                    'template_id': 'template-id',
                 },
                 'location_map': {
                     'retailer_id': 'path',
-                    'template_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_api202207_external_retailer_templates_by_retailer_id_endpoint = _Endpoint(
+        self.get_api202210_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
             settings={
-                'response_type': (TemplateListResponse,),
+                'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/retailers/{retailer-id}/templates',
-                'operation_id': 'get_api202207_external_retailer_templates_by_retailer_id',
+                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives/{creative-id}',
+                'operation_id': 'get_api202210_external_account_by_account_id_creativescreative_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'retailer_id',
+                    'account_id',
+                    'creative_id',
                 ],
                 'required': [
-                    'retailer_id',
+                    'account_id',
+                    'creative_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'retailer_id':
-                        (int,),
+                    'account_id':
+                        (str,),
+                    'creative_id':
+                        (str,),
                 },
                 'attribute_map': {
-                    'retailer_id': 'retailer-id',
+                    'account_id': 'account-id',
+                    'creative_id': 'creative-id',
                 },
                 'location_map': {
-                    'retailer_id': 'path',
+                    'account_id': 'path',
+                    'creative_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -1074,15 +1248,15 @@
         self.get_api202301_external_account_campaigns_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{accountId}/campaigns',
+                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/campaigns',
                 'operation_id': 'get_api202301_external_account_campaigns_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1142,15 +1316,15 @@
         self.get_api202301_external_campaign_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/campaigns/{campaignId}',
+                'endpoint_path': '/2023-04/retail-media/campaigns/{campaignId}',
                 'operation_id': 'get_api202301_external_campaign_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -1194,15 +1368,15 @@
         self.get_api202301_external_line_item_bid_multipliers_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfLineItemBidMultipliers,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}/bid-multipliers',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/bid-multipliers',
                 'operation_id': 'get_api202301_external_line_item_bid_multipliers_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1248,15 +1422,15 @@
         self.get_api_v1_external_account_brands_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfBrand,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{accountId}/brands',
+                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/brands',
                 'operation_id': 'get_api_v1_external_account_brands_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1316,15 +1490,15 @@
         self.get_api_v1_external_account_retailers_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfRetailer,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{accountId}/retailers',
+                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/retailers',
                 'operation_id': 'get_api_v1_external_account_retailers_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1384,15 +1558,15 @@
         self.get_api_v1_external_accounts_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfAccount,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts',
+                'endpoint_path': '/2023-04/retail-media/accounts',
                 'operation_id': 'get_api_v1_external_accounts',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'limit_to_id',
@@ -1445,15 +1619,15 @@
         self.get_api_v1_external_catalog_output_by_catalog_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/catalogs/{catalogId}/output',
+                'endpoint_path': '/2023-04/retail-media/catalogs/{catalogId}/output',
                 'operation_id': 'get_api_v1_external_catalog_output_by_catalog_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'catalog_id',
@@ -1498,15 +1672,15 @@
         self.get_api_v1_external_catalog_status_by_catalog_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCatalogStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/catalogs/{catalogId}/status',
+                'endpoint_path': '/2023-04/retail-media/catalogs/{catalogId}/status',
                 'operation_id': 'get_api_v1_external_catalog_status_by_catalog_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'catalog_id',
@@ -1550,15 +1724,15 @@
         self.get_api_v2_external_account_line_items_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (CommonLineItemPagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{account-id}/line-items',
+                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/line-items',
                 'operation_id': 'get_api_v2_external_account_line_items_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1636,15 +1810,15 @@
         self.get_api_v2_external_auction_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/auction-line-items/{line-item-id}',
+                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}',
                 'operation_id': 'get_api_v2_external_auction_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1688,15 +1862,15 @@
         self.get_api_v2_external_campaign_auction_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemPagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/campaigns/{campaign-id}/auction-line-items',
+                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/auction-line-items',
                 'operation_id': 'get_api_v2_external_campaign_auction_line_items_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -1756,15 +1930,15 @@
         self.get_api_v2_external_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (CommonLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}',
                 'operation_id': 'get_api_v2_external_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1808,15 +1982,15 @@
         self.post_api202110_external_auction_line_item_targeting_keywords_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/auction-line-items/{line-item-id}/targeting/keywords/append',
+                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords/append',
                 'operation_id': 'post_api202110_external_auction_line_item_targeting_keywords_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1866,15 +2040,15 @@
         self.post_api202110_external_auction_line_item_targeting_keywords_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/auction-line-items/{line-item-id}/targeting/keywords/delete',
+                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords/delete',
                 'operation_id': 'post_api202110_external_auction_line_item_targeting_keywords_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1924,15 +2098,15 @@
         self.post_api202110_external_balance_campaigns_append_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/balances/{balance-id}/campaigns/append',
+                'endpoint_path': '/2023-04/retail-media/balances/{balance-id}/campaigns/append',
                 'operation_id': 'post_api202110_external_balance_campaigns_append_by_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -1982,15 +2156,15 @@
         self.post_api202110_external_balance_campaigns_delete_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/balances/{balance-id}/campaigns/delete',
+                'endpoint_path': '/2023-04/retail-media/balances/{balance-id}/campaigns/delete',
                 'operation_id': 'post_api202110_external_balance_campaigns_delete_by_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -2040,15 +2214,15 @@
         self.post_api202110_external_campaign_preferred_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/campaigns/{campaign-id}/preferred-line-items',
+                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/preferred-line-items',
                 'operation_id': 'post_api202110_external_campaign_preferred_line_items_by_campaign_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -2098,15 +2272,15 @@
         self.post_api202110_external_line_item_products_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}/products/append',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/append',
                 'operation_id': 'post_api202110_external_line_item_products_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2156,15 +2330,15 @@
         self.post_api202110_external_line_item_products_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}/products/delete',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/delete',
                 'operation_id': 'post_api202110_external_line_item_products_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2214,15 +2388,15 @@
         self.post_api202110_external_line_item_products_pause_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}/products/pause',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/pause',
                 'operation_id': 'post_api202110_external_line_item_products_pause_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2270,15 +2444,15 @@
         self.post_api202110_external_line_item_products_unpause_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}/products/unpause',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/unpause',
                 'operation_id': 'post_api202110_external_line_item_products_unpause_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2326,15 +2500,15 @@
         self.post_api202110_external_preferred_line_item_targeting_add_to_basket_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/append',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_add_to_basket_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2384,15 +2558,15 @@
         self.post_api202110_external_preferred_line_item_targeting_add_to_basket_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/delete',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_add_to_basket_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2442,15 +2616,15 @@
         self.post_api202110_external_preferred_line_item_targeting_audiences_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/append',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_audiences_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2500,15 +2674,15 @@
         self.post_api202110_external_preferred_line_item_targeting_audiences_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/delete',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_audiences_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2558,15 +2732,15 @@
         self.post_api202110_external_preferred_line_item_targeting_stores_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores/append',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_stores_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2616,15 +2790,15 @@
         self.post_api202110_external_preferred_line_item_targeting_stores_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores/delete',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_stores_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2667,23 +2841,23 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.post_api202207_external_account_creatives_by_account_id_endpoint = _Endpoint(
+        self.post_api202210_external_account_creatives_by_account_id_endpoint = _Endpoint(
             settings={
-                'response_type': (Creative202207Response,),
+                'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{account-id}/creatives',
-                'operation_id': 'post_api202207_external_account_creatives_by_account_id',
+                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives',
+                'operation_id': 'post_api202210_external_account_creatives_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
                     'creative_create_model202207',
@@ -2725,22 +2899,80 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.post_api202210_external_account_creatives_search_by_account_id_endpoint = _Endpoint(
+            settings={
+                'response_type': (Creative202210ListResponse,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives/search',
+                'operation_id': 'post_api202210_external_account_creatives_search_by_account_id',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'account_id',
+                    'creative_ids',
+                ],
+                'required': [
+                    'account_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'account_id':
+                        (str,),
+                    'creative_ids':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'account_id': 'account-id',
+                    'creative_ids': 'creative-ids',
+                },
+                'location_map': {
+                    'account_id': 'path',
+                    'creative_ids': 'query',
+                },
+                'collection_format_map': {
+                    'creative_ids': 'multi',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.post_api202301_external_account_campaigns_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{accountId}/campaigns',
+                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/campaigns',
                 'operation_id': 'post_api202301_external_account_campaigns_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -2790,15 +3022,15 @@
         self.post_api_v1_external_account_catalogs_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCatalogStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{accountId}/catalogs',
+                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/catalogs',
                 'operation_id': 'post_api_v1_external_account_catalogs_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -2848,15 +3080,15 @@
         self.post_api_v2_external_campaign_auction_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/campaigns/{campaign-id}/auction-line-items',
+                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/auction-line-items',
                 'operation_id': 'post_api_v2_external_campaign_auction_line_items_by_campaign_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -2906,15 +3138,15 @@
         self.put_api202110_external_preferred_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}',
                 'operation_id': 'put_api202110_external_preferred_line_item_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2964,15 +3196,15 @@
         self.put_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3022,15 +3254,15 @@
         self.put_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3080,15 +3312,15 @@
         self.put_api202110_external_preferred_line_item_targeting_stores_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
+                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_stores_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3131,23 +3363,23 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.put_api202207_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
+        self.put_api202210_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
             settings={
-                'response_type': (Creative202207Response,),
+                'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/accounts/{account-id}/creatives/{creative-id}',
-                'operation_id': 'put_api202207_external_account_by_account_id_creativescreative_id',
+                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives/{creative-id}',
+                'operation_id': 'put_api202210_external_account_by_account_id_creativescreative_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
                     'creative_id',
@@ -3202,15 +3434,15 @@
         self.put_api202301_external_campaign_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/campaigns/{campaignId}',
+                'endpoint_path': '/2023-04/retail-media/campaigns/{campaignId}',
                 'operation_id': 'put_api202301_external_campaign_by_campaign_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -3260,15 +3492,15 @@
         self.put_api202301_external_line_item_bid_multipliers_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (LineItemBidMultipliersResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/line-items/{line-item-id}/bid-multipliers',
+                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/bid-multipliers',
                 'operation_id': 'put_api202301_external_line_item_bid_multipliers_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3320,15 +3552,15 @@
         self.put_api_v2_external_auction_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-01/retail-media/auction-line-items/{line-item-id}',
+                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}',
                 'operation_id': 'put_api_v2_external_auction_line_item_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3371,14 +3603,212 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.set_keyword_bids_endpoint = _Endpoint(
+            settings={
+                'response_type': (RetailMediaExternalv1ResourceOutcome,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-04/retail-media/line-items/{id}/keywords/set-bid',
+                'operation_id': 'set_keyword_bids',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'retail_media_externalv1_set_bids_model_request',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'retail_media_externalv1_set_bids_model_request':
+                        (RetailMediaExternalv1SetBidsModelRequest,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'retail_media_externalv1_set_bids_model_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.submit_proposal_endpoint = _Endpoint(
+            settings={
+                'response_type': (RetailMediaExternalv1ProposalStatusModelResponse,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-04/retail-media/preferred-deal-line-items/{id}/proposal/submit',
+                'operation_id': 'submit_proposal',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+    def add_remove_keywords(
+        self,
+        id,
+        **kwargs
+    ):
+        """add_remove_keywords  # noqa: E501
+
+        Add or Remove keywords from the associated line item in bulk  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.add_remove_keywords(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Long external id of the associated line item
+
+        Keyword Args:
+            retail_media_externalv1_add_remove_keywords_model_request (RetailMediaExternalv1AddRemoveKeywordsModelRequest): Object containing keywords to be added or removed. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            RetailMediaExternalv1ResourceOutcome
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.add_remove_keywords_endpoint.call_with_http_info(**kwargs)
 
     def create_asset(
         self,
         asset_file,
         **kwargs
     ):
         """create_asset  # noqa: E501
@@ -3455,14 +3885,180 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['asset_file'] = \
             asset_file
         return self.create_asset_endpoint.call_with_http_info(**kwargs)
 
+    def fetch_keywords(
+        self,
+        id,
+        **kwargs
+    ):
+        """fetch_keywords  # noqa: E501
+
+        Fetch keywords associated with the specified line item  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.fetch_keywords(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Long external id of the associated line item
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            RetailMediaExternalv1KeywordsModelResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.fetch_keywords_endpoint.call_with_http_info(**kwargs)
+
+    def fetch_proposal(
+        self,
+        id,
+        **kwargs
+    ):
+        """fetch_proposal  # noqa: E501
+
+        Fetch the status of a proposal to modify a Preferred Deal Line Item.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.fetch_proposal(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): The external id of a line item.
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            RetailMediaExternalv1ProposalStatusModelResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.fetch_proposal_endpoint.call_with_http_info(**kwargs)
+
     def get_api202110_external_account_balances_by_account_id(
         self,
         account_id,
         **kwargs
     ):
         """get_api202110_external_account_balances_by_account_id  # noqa: E501
 
@@ -4545,32 +5141,32 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.get_api202204_external_categories_endpoint.call_with_http_info(**kwargs)
 
-    def get_api202207_external_account_by_account_id_creativescreative_id(
+    def get_api202207_external_retailer_by_retailer_id_templatestemplate_id(
         self,
-        account_id,
-        creative_id,
+        retailer_id,
+        template_id,
         **kwargs
     ):
-        """get_api202207_external_account_by_account_id_creativescreative_id  # noqa: E501
+        """get_api202207_external_retailer_by_retailer_id_templatestemplate_id  # noqa: E501
 
-        Get the specified creative  # noqa: E501
+        Gets the template for the specified retailer id and template id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_api202207_external_account_by_account_id_creativescreative_id(account_id, creative_id, async_req=True)
+        >>> thread = api.get_api202207_external_retailer_by_retailer_id_templatestemplate_id(retailer_id, template_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            account_id (str): External account id to retrieve creatives for
-            creative_id (str): Creative to get
+            retailer_id (int): Retailer Id
+            template_id (int): Template Id
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -4597,15 +5193,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            Creative202207Response
+            TemplateResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -4626,38 +5222,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['account_id'] = \
-            account_id
-        kwargs['creative_id'] = \
-            creative_id
-        return self.get_api202207_external_account_by_account_id_creativescreative_id_endpoint.call_with_http_info(**kwargs)
+        kwargs['retailer_id'] = \
+            retailer_id
+        kwargs['template_id'] = \
+            template_id
+        return self.get_api202207_external_retailer_by_retailer_id_templatestemplate_id_endpoint.call_with_http_info(**kwargs)
 
-    def get_api202207_external_retailer_by_retailer_id_templatestemplate_id(
+    def get_api202207_external_retailer_templates_by_retailer_id(
         self,
         retailer_id,
-        template_id,
         **kwargs
     ):
-        """get_api202207_external_retailer_by_retailer_id_templatestemplate_id  # noqa: E501
+        """get_api202207_external_retailer_templates_by_retailer_id  # noqa: E501
 
-        Gets the template for the specified retailer id and template id  # noqa: E501
+        Get retailer creative templates  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_api202207_external_retailer_by_retailer_id_templatestemplate_id(retailer_id, template_id, async_req=True)
+        >>> thread = api.get_api202207_external_retailer_templates_by_retailer_id(retailer_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            retailer_id (int): Retailer Id
-            template_id (int): Template Id
+            retailer_id (int): External retailer id to retrieve creative templates for
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -4684,15 +5278,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TemplateResponse
+            TemplateListResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -4715,34 +5309,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['retailer_id'] = \
             retailer_id
-        kwargs['template_id'] = \
-            template_id
-        return self.get_api202207_external_retailer_by_retailer_id_templatestemplate_id_endpoint.call_with_http_info(**kwargs)
+        return self.get_api202207_external_retailer_templates_by_retailer_id_endpoint.call_with_http_info(**kwargs)
 
-    def get_api202207_external_retailer_templates_by_retailer_id(
+    def get_api202210_external_account_by_account_id_creativescreative_id(
         self,
-        retailer_id,
+        account_id,
+        creative_id,
         **kwargs
     ):
-        """get_api202207_external_retailer_templates_by_retailer_id  # noqa: E501
+        """get_api202210_external_account_by_account_id_creativescreative_id  # noqa: E501
 
-        Get retailer creative templates  # noqa: E501
+        Get the specified creative  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_api202207_external_retailer_templates_by_retailer_id(retailer_id, async_req=True)
+        >>> thread = api.get_api202210_external_account_by_account_id_creativescreative_id(account_id, creative_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            retailer_id (int): External retailer id to retrieve creative templates for
+            account_id (str): External account id to retrieve creatives for
+            creative_id (str): Creative to get
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -4769,15 +5363,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TemplateListResponse
+            Creative202210Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -4798,17 +5392,19 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['retailer_id'] = \
-            retailer_id
-        return self.get_api202207_external_retailer_templates_by_retailer_id_endpoint.call_with_http_info(**kwargs)
+        kwargs['account_id'] = \
+            account_id
+        kwargs['creative_id'] = \
+            creative_id
+        return self.get_api202210_external_account_by_account_id_creativescreative_id_endpoint.call_with_http_info(**kwargs)
 
     def get_api202301_external_account_campaigns_by_account_id(
         self,
         account_id,
         **kwargs
     ):
         """get_api202301_external_account_campaigns_by_account_id  # noqa: E501
@@ -7073,26 +7669,26 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['line_item_id'] = \
             line_item_id
         return self.post_api202110_external_preferred_line_item_targeting_stores_delete_by_line_item_id_endpoint.call_with_http_info(**kwargs)
 
-    def post_api202207_external_account_creatives_by_account_id(
+    def post_api202210_external_account_creatives_by_account_id(
         self,
         account_id,
         **kwargs
     ):
-        """post_api202207_external_account_creatives_by_account_id  # noqa: E501
+        """post_api202210_external_account_creatives_by_account_id  # noqa: E501
 
         Create a creative for an account  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_api202207_external_account_creatives_by_account_id(account_id, async_req=True)
+        >>> thread = api.post_api202210_external_account_creatives_by_account_id(account_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             account_id (str): External account id to create a creative for
 
         Keyword Args:
             creative_create_model202207 (CreativeCreateModel202207): The creative to create. [optional]
@@ -7124,15 +7720,99 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            Creative202207Response
+            Creative202210Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['account_id'] = \
+            account_id
+        return self.post_api202210_external_account_creatives_by_account_id_endpoint.call_with_http_info(**kwargs)
+
+    def post_api202210_external_account_creatives_search_by_account_id(
+        self,
+        account_id,
+        **kwargs
+    ):
+        """post_api202210_external_account_creatives_search_by_account_id  # noqa: E501
+
+        Get account creatives  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.post_api202210_external_account_creatives_search_by_account_id(account_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            account_id (str): External account id to retrieve creatives for
+
+        Keyword Args:
+            creative_ids ([str]): Creatives to filter by. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Creative202210ListResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -7155,15 +7835,15 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['account_id'] = \
             account_id
-        return self.post_api202207_external_account_creatives_by_account_id_endpoint.call_with_http_info(**kwargs)
+        return self.post_api202210_external_account_creatives_search_by_account_id_endpoint.call_with_http_info(**kwargs)
 
     def post_api202301_external_account_campaigns_by_account_id(
         self,
         account_id,
         **kwargs
     ):
         """post_api202301_external_account_campaigns_by_account_id  # noqa: E501
@@ -7745,27 +8425,27 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['line_item_id'] = \
             line_item_id
         return self.put_api202110_external_preferred_line_item_targeting_stores_by_line_item_id_endpoint.call_with_http_info(**kwargs)
 
-    def put_api202207_external_account_by_account_id_creativescreative_id(
+    def put_api202210_external_account_by_account_id_creativescreative_id(
         self,
         account_id,
         creative_id,
         **kwargs
     ):
-        """put_api202207_external_account_by_account_id_creativescreative_id  # noqa: E501
+        """put_api202210_external_account_by_account_id_creativescreative_id  # noqa: E501
 
         Update a creative  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_api202207_external_account_by_account_id_creativescreative_id(account_id, creative_id, async_req=True)
+        >>> thread = api.put_api202210_external_account_by_account_id_creativescreative_id(account_id, creative_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             account_id (str): External account id containing the creative
             creative_id (str): Creative to update
 
         Keyword Args:
@@ -7798,15 +8478,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            Creative202207Response
+            Creative202210Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -7831,15 +8511,15 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['account_id'] = \
             account_id
         kwargs['creative_id'] = \
             creative_id
-        return self.put_api202207_external_account_by_account_id_creativescreative_id_endpoint.call_with_http_info(**kwargs)
+        return self.put_api202210_external_account_by_account_id_creativescreative_id_endpoint.call_with_http_info(**kwargs)
 
     def put_api202301_external_campaign_by_campaign_id(
         self,
         campaign_id,
         **kwargs
     ):
         """put_api202301_external_campaign_by_campaign_id  # noqa: E501
@@ -8085,7 +8765,174 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['line_item_id'] = \
             line_item_id
         return self.put_api_v2_external_auction_line_item_by_line_item_id_endpoint.call_with_http_info(**kwargs)
 
+    def set_keyword_bids(
+        self,
+        id,
+        **kwargs
+    ):
+        """set_keyword_bids  # noqa: E501
+
+        Set bid overrides for associated keywords to the given line item in bulk  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.set_keyword_bids(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Long external id of the associated line item
+
+        Keyword Args:
+            retail_media_externalv1_set_bids_model_request (RetailMediaExternalv1SetBidsModelRequest): Object containing a list of bid overrides for associated keywords. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            RetailMediaExternalv1ResourceOutcome
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.set_keyword_bids_endpoint.call_with_http_info(**kwargs)
+
+    def submit_proposal(
+        self,
+        id,
+        **kwargs
+    ):
+        """submit_proposal  # noqa: E501
+
+        Submit a proposal to modify a Preferred Deal Line Item for review.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.submit_proposal(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): The external id of a line item.
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            RetailMediaExternalv1ProposalStatusModelResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.submit_proposal_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api/gateway_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/gateway_api.py`

 * *Files 4% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_01.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_retailmedia_v2023_04.model.application_summary_model_response import ApplicationSummaryModelResponse
 
 
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
-                'endpoint_path': '/2023-01/retail-media/me',
+                'endpoint_path': '/2023-04/retail-media/me',
                 'operation_id': 'get_current_application',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/api_client.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api_client.py`

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
 
 
-from criteo_api_retailmedia_v2023_01 import rest
-from criteo_api_retailmedia_v2023_01.configuration import Configuration
-from criteo_api_retailmedia_v2023_01.exceptions import ApiTypeError, ApiValueError, ApiException
-from criteo_api_retailmedia_v2023_01.model_utils import (
+from criteo_api_retailmedia_v2023_04 import rest
+from criteo_api_retailmedia_v2023_04.configuration import Configuration
+from criteo_api_retailmedia_v2023_04.exceptions import ApiTypeError, ApiValueError, ApiException
+from criteo_api_retailmedia_v2023_04.model_utils import (
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

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/apis/__init__.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/apis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from criteo_api_retailmedia_v2023_01.api.analytics_api import AnalyticsApi
+#   from criteo_api_retailmedia_v2023_04.api.analytics_api import AnalyticsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from criteo_api_retailmedia_v2023_01.api.analytics_api import AnalyticsApi
-from criteo_api_retailmedia_v2023_01.api.audience_api import AudienceApi
-from criteo_api_retailmedia_v2023_01.api.campaign_api import CampaignApi
-from criteo_api_retailmedia_v2023_01.api.gateway_api import GatewayApi
+from criteo_api_retailmedia_v2023_04.api.analytics_api import AnalyticsApi
+from criteo_api_retailmedia_v2023_04.api.audience_api import AudienceApi
+from criteo_api_retailmedia_v2023_04.api.campaign_api import CampaignApi
+from criteo_api_retailmedia_v2023_04.api.gateway_api import GatewayApi
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/configuration.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/configuration.py`

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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiValueError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiValueError
 
 
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
-        self.logger["package_logger"] = logging.getLogger("criteo_api_retailmedia_v2023_01")
+        self.logger["package_logger"] = logging.getLogger("criteo_api_retailmedia_v2023_04")
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

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/criteo_api_client.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_api_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from criteo_api_retailmedia_v2023_01.api_client import ApiClient
-from criteo_api_retailmedia_v2023_01.criteo_rest import CriteoRESTClientObject
+from criteo_api_retailmedia_v2023_04.api_client import ApiClient
+from criteo_api_retailmedia_v2023_04.criteo_rest import CriteoRESTClientObject
 
 class CriteoApiClient(ApiClient):
     def __init__(self, configuration=None, header_name=None, header_value=None,
              cookie=None, pool_threads=1, additional_parameters= {}):
         super().__init__(configuration=configuration,header_name=header_name, header_value=header_value, cookie=cookie, pool_threads=pool_threads)
         self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/criteo_auth.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from datetime import datetime, timedelta
-from criteo_api_retailmedia_v2023_01.exceptions import ApiException
-from criteo_api_retailmedia_v2023_01.api_client import ApiClient
+from criteo_api_retailmedia_v2023_04.exceptions import ApiException
+from criteo_api_retailmedia_v2023_04.api_client import ApiClient
 
 class Token(object):
 
     def __init__(self, token_string , expiration_date = None):
         self.expiration_date = expiration_date 
         self.token_string = token_string
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/criteo_rest.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from criteo_api_retailmedia_v2023_01.rest import RESTClientObject
-from criteo_api_retailmedia_v2023_01.criteo_auth import *
+from criteo_api_retailmedia_v2023_04.rest import RESTClientObject
+from criteo_api_retailmedia_v2023_04.criteo_auth import *
 
 
 class CriteoRESTClientObject(RESTClientObject):
 
     def __init__(self, configuration, additional_parameters = {}, pools_size=4, maxsize=None):
         super().__init__(configuration, pools_size, maxsize)
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/exceptions.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/exceptions.py`

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

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/add_to_basket_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
     globals()['ValueTypeResourceOfAddToBasketIdsUpdateModel202110'] = ValueTypeResourceOfAddToBasketIdsUpdateModel202110
 
 
 class AddToBasketIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
     globals()['ValueTypeResourceOfAddToBasketTarget202110'] = ValueTypeResourceOfAddToBasketTarget202110
 
 
 class AddToBasketTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/add_to_basket_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfAddToBasketTarget202110'] = ValueTypeResourceOfAddToBasketTarget202110
 
 
 class AddToBasketTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/application_summary_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ApplicationSummaryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/application_summary_model_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.application_summary_model import ApplicationSummaryModel
+    from criteo_api_retailmedia_v2023_04.model.application_summary_model import ApplicationSummaryModel
     globals()['ApplicationSummaryModel'] = ApplicationSummaryModel
 
 
 class ApplicationSummaryModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/application_summary_model_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-    from criteo_api_retailmedia_v2023_01.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
     globals()['ApplicationSummaryModelResource'] = ApplicationSummaryModelResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class ApplicationSummaryModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/asset.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class Asset(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/asset_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_resource.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.asset import Asset
+    from criteo_api_retailmedia_v2023_04.model.asset import Asset
     globals()['Asset'] = Asset
 
 
 class AssetResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/asset_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.asset_resource import AssetResource
-    from criteo_api_retailmedia_v2023_01.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_04.model.asset_resource import AssetResource
+    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
     globals()['AssetResource'] = AssetResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AssetResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_create_model_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
+    from criteo_api_retailmedia_v2023_04.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
     globals()['InputResourceOfAuctionLineItemCreateModel'] = InputResourceOfAuctionLineItemCreateModel
 
 
 class AuctionLineItemCreateModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfAuctionLineItem'] = ResourceOfAuctionLineItem
 
 
 class AuctionLineItemPagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfAuctionLineItem'] = ResourceOfAuctionLineItem
 
 
 class AuctionLineItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/auction_line_item_update_model_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
+    from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
     globals()['ResourceOfAuctionLineItemUpdateModel'] = ResourceOfAuctionLineItemUpdateModel
 
 
 class AuctionLineItemUpdateModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/audience_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
     globals()['ValueTypeResourceOfAudienceIdsUpdateModel202110'] = ValueTypeResourceOfAudienceIdsUpdateModel202110
 
 
 class AudienceIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/audience_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
     globals()['ValueTypeResourceOfAudienceTarget202110'] = ValueTypeResourceOfAudienceTarget202110
 
 
 class AudienceTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/audience_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfAudienceTarget202110'] = ValueTypeResourceOfAudienceTarget202110
 
 
 class AudienceTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/bad_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/bad_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.error import Error
+    from criteo_api_retailmedia_v2023_04.model.error import Error
     globals()['Error'] = Error
 
 
 class BadRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/balance202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_balance202110 import ResourceOfBalance202110
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_balance202110 import ResourceOfBalance202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfBalance202110'] = ResourceOfBalance202110
 
 
 class Balance202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+    from criteo_api_retailmedia_v2023_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
     globals()['ResourceOfBalanceCampaign202110'] = ResourceOfBalanceCampaign202110
 
 
 class BalanceCampaign202110ListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/balance_campaign202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfBalanceCampaign202110'] = ResourceOfBalanceCampaign202110
 
 
 class BalanceCampaign202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CampaignAttributesV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/category202204.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class Category202204(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/category202204_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_category202204 import ResourceOfCategory202204
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_category202204 import ResourceOfCategory202204
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCategory202204'] = ResourceOfCategory202204
 
 
 class Category202204ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/choice_option.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_option.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.template_variable import TemplateVariable
+    from criteo_api_retailmedia_v2023_04.model.template_variable import TemplateVariable
     globals()['TemplateVariable'] = TemplateVariable
 
 
 class ChoiceOption(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/choice_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.choice_option import ChoiceOption
+    from criteo_api_retailmedia_v2023_04.model.choice_option import ChoiceOption
     globals()['ChoiceOption'] = ChoiceOption
 
 
 class ChoiceVariableSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/choice_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ChoiceVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/color_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/color_variable_value.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ColorVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_error.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_warning.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
-class CommonError(ModelNormal):
+class CommonWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -121,15 +121,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CommonError - a model defined in OpenAPI
+        """CommonWarning - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,15 +214,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CommonError - a model defined in OpenAPI
+        """CommonWarning - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_common_line_item import ResourceOfCommonLineItem
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCommonLineItem'] = ResourceOfCommonLineItem
 
 
 class CommonLineItemPagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_common_line_item import ResourceOfCommonLineItem
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCommonLineItem'] = ResourceOfCommonLineItem
 
 
 class CommonLineItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_problem.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_problem.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CommonProblem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_status_code_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
     globals()['CommonProblem'] = CommonProblem
 
 
 class CommonStatusCodeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/common_warning.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_error.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
-class CommonWarning(ModelNormal):
+class CommonError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -121,15 +121,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CommonWarning - a model defined in OpenAPI
+        """CommonError - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,15 +214,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CommonWarning - a model defined in OpenAPI
+        """CommonError - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
     globals()['CreateRetailMediaAudienceAttributes'] = CreateRetailMediaAudienceAttributes
 
 
 class CreateRetailMediaAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CreateRetailMediaAudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_body.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
     globals()['CreateRetailMediaAudienceAttributes'] = CreateRetailMediaAudienceAttributes
 
 
 class CreateRetailMediaAudienceBody(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
     globals()['CreateRetailMediaAudienceBody'] = CreateRetailMediaAudienceBody
 
 
 class CreateRetailMediaAudienceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py`

 * *Files 0% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience import CreateRetailMediaAudience
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience import CreateRetailMediaAudience
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['CreateRetailMediaAudience'] = CreateRetailMediaAudience
 
 
 class CreateRetailMediaAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
     globals()['CreateRetailMediaAudienceV2Attributes'] = CreateRetailMediaAudienceV2Attributes
 
 
 class CreateRetailMediaAudienceV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.user_behavior_details_v2 import UserBehaviorDetailsV2
+    from criteo_api_retailmedia_v2023_04.model.user_behavior_details_v2 import UserBehaviorDetailsV2
     globals()['UserBehaviorDetailsV2'] = UserBehaviorDetailsV2
 
 
 class CreateRetailMediaAudienceV2Attributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_data.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
     globals()['CreateRetailMediaAudienceV2Attributes'] = CreateRetailMediaAudienceV2Attributes
 
 
 class CreateRetailMediaAudienceV2Data(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_retail_media_audience_v2_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
     globals()['CreateRetailMediaAudienceV2Data'] = CreateRetailMediaAudienceV2Data
 
 
 class CreateRetailMediaAudienceV2Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/create_user_behavior_segment_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CreateUserBehaviorSegmentV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class Creative202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202110_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_creative202110 import ResourceOfCreative202110
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_creative202110 import ResourceOfCreative202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCreative202110'] = ResourceOfCreative202110
 
 
 class Creative202110ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202207.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.template_variable_value import TemplateVariableValue
-    globals()['TemplateVariableValue'] = TemplateVariableValue
+    from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
+    globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
+    globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
-class Creative202207(ModelNormal):
+class ExternalPreferredLineItemCreateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,40 +57,37 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('status',): {
-            'READY': "Ready",
-            'IN_USE': "In_Use",
-            'ARCHIVED': "Archived",
-            'DELETED': "Deleted",
-        },
-        ('creative_format_type',): {
-            'UNKNOWN': "Unknown",
-            'FLAGSHIP': "FlagShip",
-            'SHOWCASE': "Showcase",
-            'SPONSOREDPRODUCTS': "SponsoredProducts",
-            'BUTTERFLY': "Butterfly",
-            'BUNDLEBOOST': "BundleBoost",
-            'IAB': "IAB",
-            'CUSTOM': "CUSTOM",
-            'DISPLAYPANEL': "DisplayPanel",
-            'DIGITALSHELFTALKER': "DigitalShelfTalker",
+        ('pacing',): {
+            'UNKNOWN': "unknown",
+            'STANDARD': "standard",
+            'ACCELERATED': "accelerated",
         },
-        ('environments',): {
-            'WEB': "Web",
-            'MOBILE': "Mobile",
-            'APP': "App",
+        ('status',): {
+            'UNKNOWN': "unknown",
+            'ACTIVE': "active",
+            'SCHEDULED': "scheduled",
+            'DRAFT': "draft",
+            'PAUSED': "paused",
+            'BUDGETHIT': "budgetHit",
+            'ENDED': "ended",
+            'ARCHIVED': "archived",
+            'NOFUNDS': "noFunds",
         },
     }
 
     validations = {
+        ('name',): {
+            'max_length': 255,
+            'min_length': 0,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -107,58 +106,61 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
+            'start_date': (date,),  # noqa: E501
+            'end_date': (date,),  # noqa: E501
+            'pacing': (str,),  # noqa: E501
+            'page': (ExternalLineItemPage202110,),  # noqa: E501
+            'target_retailer_id': (str,),  # noqa: E501
+            'budget': (float,),  # noqa: E501
             'status': (str,),  # noqa: E501
-            'retailer_id': (int,),  # noqa: E501
-            'creative_format_type': (str,),  # noqa: E501
-            'environments': ([str],),  # noqa: E501
-            'template_variable_values': ([TemplateVariableValue],),  # noqa: E501
-            'brand_id': (int, none_type,),  # noqa: E501
-            'associated_line_item_ids': ([str],),  # noqa: E501
-            'updated_at': (datetime,),  # noqa: E501
+            'capping': (ExternalLineItemCapping202110,),  # noqa: E501
+            'creative_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
+        'start_date': 'startDate',  # noqa: E501
+        'end_date': 'endDate',  # noqa: E501
+        'pacing': 'pacing',  # noqa: E501
+        'page': 'page',  # noqa: E501
+        'target_retailer_id': 'targetRetailerId',  # noqa: E501
+        'budget': 'budget',  # noqa: E501
         'status': 'status',  # noqa: E501
-        'retailer_id': 'retailerId',  # noqa: E501
-        'creative_format_type': 'creativeFormatType',  # noqa: E501
-        'environments': 'environments',  # noqa: E501
-        'template_variable_values': 'templateVariableValues',  # noqa: E501
-        'brand_id': 'brandId',  # noqa: E501
-        'associated_line_item_ids': 'associatedLineItemIds',  # noqa: E501
-        'updated_at': 'updatedAt',  # noqa: E501
+        'capping': 'capping',  # noqa: E501
+        'creative_id': 'creativeId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, status, retailer_id, creative_format_type, environments, template_variable_values, *args, **kwargs):  # noqa: E501
-        """Creative202207 - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, start_date, end_date, pacing, page, target_retailer_id, budget, *args, **kwargs):  # noqa: E501
+        """ExternalPreferredLineItemCreateModel202110 - a model defined in OpenAPI
 
         Args:
-            name (str): Name
-            status (str): Creative Status
-            retailer_id (int): Retailer Id
-            creative_format_type (str): Creative format type
-            environments ([str]): Environment type (e.g. mobile, web, app)
-            template_variable_values ([TemplateVariableValue]): The template chosen values
+            name (str):
+            start_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
+            end_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
+            pacing (str):
+            page (ExternalLineItemPage202110):
+            target_retailer_id (str):
+            budget (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -183,17 +185,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            brand_id (int, none_type): Brand Id. [optional]  # noqa: E501
-            associated_line_item_ids ([str]): Associated Line Item Ids. [optional]  # noqa: E501
-            updated_at (datetime): Updated at time. [optional]  # noqa: E501
+            status (str): [optional]  # noqa: E501
+            capping (ExternalLineItemCapping202110): [optional]  # noqa: E501
+            creative_id (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -218,19 +220,20 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
-        self.status = status
-        self.retailer_id = retailer_id
-        self.creative_format_type = creative_format_type
-        self.environments = environments
-        self.template_variable_values = template_variable_values
+        self.start_date = start_date
+        self.end_date = end_date
+        self.pacing = pacing
+        self.page = page
+        self.target_retailer_id = target_retailer_id
+        self.budget = budget
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -243,24 +246,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, status, retailer_id, creative_format_type, environments, template_variable_values, *args, **kwargs):  # noqa: E501
-        """Creative202207 - a model defined in OpenAPI
+    def __init__(self, name, start_date, end_date, pacing, page, target_retailer_id, budget, *args, **kwargs):  # noqa: E501
+        """ExternalPreferredLineItemCreateModel202110 - a model defined in OpenAPI
 
         Args:
-            name (str): Name
-            status (str): Creative Status
-            retailer_id (int): Retailer Id
-            creative_format_type (str): Creative format type
-            environments ([str]): Environment type (e.g. mobile, web, app)
-            template_variable_values ([TemplateVariableValue]): The template chosen values
+            name (str):
+            start_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
+            end_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
+            pacing (str):
+            page (ExternalLineItemPage202110):
+            target_retailer_id (str):
+            budget (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -285,17 +289,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            brand_id (int, none_type): Brand Id. [optional]  # noqa: E501
-            associated_line_item_ids ([str]): Associated Line Item Ids. [optional]  # noqa: E501
-            updated_at (datetime): Updated at time. [optional]  # noqa: E501
+            status (str): [optional]  # noqa: E501
+            capping (ExternalLineItemCapping202110): [optional]  # noqa: E501
+            creative_id (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -318,19 +322,20 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
-        self.status = status
-        self.retailer_id = retailer_id
-        self.creative_format_type = creative_format_type
-        self.environments = environments
-        self.template_variable_values = template_variable_values
+        self.start_date = start_date
+        self.end_date = end_date
+        self.pacing = pacing
+        self.page = page
+        self.target_retailer_id = target_retailer_id
+        self.budget = budget
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative202207_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210_response.py`

 * *Files 2% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_creative202207 import ResourceOfCreative202207
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_creative202210 import ResourceOfCreative202210
     globals()['ProblemDetails'] = ProblemDetails
-    globals()['ResourceOfCreative202207'] = ResourceOfCreative202207
+    globals()['ResourceOfCreative202210'] = ResourceOfCreative202210
 
 
-class Creative202207Response(ModelNormal):
+class Creative202210Response(ModelNormal):
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
-            'data': (ResourceOfCreative202207,),  # noqa: E501
+            'data': (ResourceOfCreative202210,),  # noqa: E501
             'warnings': ([ProblemDetails],),  # noqa: E501
             'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Creative202207Response - a model defined in OpenAPI
+        """Creative202210Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,15 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfCreative202207): [optional]  # noqa: E501
+            data (ResourceOfCreative202210): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -199,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Creative202207Response - a model defined in OpenAPI
+        """Creative202210Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,15 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfCreative202207): [optional]  # noqa: E501
+            data (ResourceOfCreative202210): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative_create_model202207.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2023_04.model.template_variable_value import TemplateVariableValue
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class CreativeCreateModel202207(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/creative_update_model202207.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2023_04.model.template_variable_value import TemplateVariableValue
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class CreativeUpdateModel202207(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/customer_list_details.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/customer_list_details.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class CustomerListDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/editable_campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class EditableCampaignAttributesV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/envelope_report_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.report_request import ReportRequest
+    from criteo_api_retailmedia_v2023_04.model.report_request import ReportRequest
     globals()['ReportRequest'] = ReportRequest
 
 
 class EnvelopeReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/envelope_report_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.report_status import ReportStatus
+    from criteo_api_retailmedia_v2023_04.model.report_status import ReportStatus
     globals()['ReportStatus'] = ReportStatus
 
 
 class EnvelopeReportStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/error.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/error.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.map_string import MapString
+    from criteo_api_retailmedia_v2023_04.model.map_string import MapString
     globals()['MapString'] = MapString
 
 
 class Error(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_account.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_account.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAddToBasketIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAddToBasketTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItemCreateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItemUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAudienceIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAudienceTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_balance202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_balance202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalBalance202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_brand.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_brand.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalBrand(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalCommonLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalKeywordTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_line_item_capping202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalLineItemCapping202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_line_item_page202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
+    from criteo_api_retailmedia_v2023_04.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
     globals()['ExternalLineItemPageCategory202110'] = ExternalLineItemPageCategory202110
 
 
 class ExternalLineItemPage202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_line_item_page_category202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalLineItemPageCategory202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2023_01.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
 class ExternalPreferredLineItem202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py`

 * *Files 4% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2023_01.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
-class ExternalPreferredLineItemCreateModel202110(ModelNormal):
+class ExternalPreferredLineItemUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -57,30 +57,30 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('pacing',): {
-            'UNKNOWN': "unknown",
-            'STANDARD': "standard",
-            'ACCELERATED': "accelerated",
-        },
         ('status',): {
             'UNKNOWN': "unknown",
             'ACTIVE': "active",
             'SCHEDULED': "scheduled",
             'DRAFT': "draft",
             'PAUSED': "paused",
             'BUDGETHIT': "budgetHit",
             'ENDED': "ended",
             'ARCHIVED': "archived",
             'NOFUNDS': "noFunds",
         },
+        ('pacing',): {
+            'UNKNOWN': "unknown",
+            'STANDARD': "standard",
+            'ACCELERATED': "accelerated",
+        },
     }
 
     validations = {
         ('name',): {
             'max_length': 255,
             'min_length': 0,
         },
@@ -108,59 +108,54 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'start_date': (date,),  # noqa: E501
             'end_date': (date,),  # noqa: E501
+            'status': (str,),  # noqa: E501
             'pacing': (str,),  # noqa: E501
+            'capping': (ExternalLineItemCapping202110,),  # noqa: E501
             'page': (ExternalLineItemPage202110,),  # noqa: E501
-            'target_retailer_id': (str,),  # noqa: E501
             'budget': (float,),  # noqa: E501
-            'status': (str,),  # noqa: E501
-            'capping': (ExternalLineItemCapping202110,),  # noqa: E501
             'creative_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'start_date': 'startDate',  # noqa: E501
         'end_date': 'endDate',  # noqa: E501
+        'status': 'status',  # noqa: E501
         'pacing': 'pacing',  # noqa: E501
+        'capping': 'capping',  # noqa: E501
         'page': 'page',  # noqa: E501
-        'target_retailer_id': 'targetRetailerId',  # noqa: E501
         'budget': 'budget',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'capping': 'capping',  # noqa: E501
         'creative_id': 'creativeId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, start_date, end_date, pacing, page, target_retailer_id, budget, *args, **kwargs):  # noqa: E501
-        """ExternalPreferredLineItemCreateModel202110 - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, start_date, end_date, status, *args, **kwargs):  # noqa: E501
+        """ExternalPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
 
         Args:
             name (str):
             start_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
             end_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
-            pacing (str):
-            page (ExternalLineItemPage202110):
-            target_retailer_id (str):
-            budget (float):
+            status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,16 +180,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
+            pacing (str): [optional] if omitted the server will use the default value of "accelerated"  # noqa: E501
             capping (ExternalLineItemCapping202110): [optional]  # noqa: E501
+            page (ExternalLineItemPage202110): [optional]  # noqa: E501
+            budget (float): [optional]  # noqa: E501
             creative_id (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -222,18 +219,15 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.start_date = start_date
         self.end_date = end_date
-        self.pacing = pacing
-        self.page = page
-        self.target_retailer_id = target_retailer_id
-        self.budget = budget
+        self.status = status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -246,25 +240,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, start_date, end_date, pacing, page, target_retailer_id, budget, *args, **kwargs):  # noqa: E501
-        """ExternalPreferredLineItemCreateModel202110 - a model defined in OpenAPI
+    def __init__(self, name, start_date, end_date, status, *args, **kwargs):  # noqa: E501
+        """ExternalPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
 
         Args:
             name (str):
             start_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
             end_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
-            pacing (str):
-            page (ExternalLineItemPage202110):
-            target_retailer_id (str):
-            budget (float):
+            status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -289,16 +280,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
+            pacing (str): [optional] if omitted the server will use the default value of "accelerated"  # noqa: E501
             capping (ExternalLineItemCapping202110): [optional]  # noqa: E501
+            page (ExternalLineItemPage202110): [optional]  # noqa: E501
+            budget (float): [optional]  # noqa: E501
             creative_id (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -324,18 +317,15 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.start_date = start_date
         self.end_date = end_date
-        self.pacing = pacing
-        self.page = page
-        self.target_retailer_id = target_retailer_id
-        self.budget = budget
+        self.status = status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 """
     Criteo API
 
     Criteo publicly exposed API  # noqa: E501
 
-    The version of the OpenAPI document: 2023-01
+    The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2023_01.model.external_line_item_page202110 import ExternalLineItemPage202110
-    globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
-    globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
-
-class ExternalPreferredLineItemUpdateModel202110(ModelNormal):
+class RetailMediaExternalv1ProposalStatusModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -57,105 +51,95 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('status',): {
-            'UNKNOWN': "unknown",
-            'ACTIVE': "active",
-            'SCHEDULED': "scheduled",
-            'DRAFT': "draft",
-            'PAUSED': "paused",
-            'BUDGETHIT': "budgetHit",
-            'ENDED': "ended",
-            'ARCHIVED': "archived",
-            'NOFUNDS': "noFunds",
+        ('negotiation_state',): {
+            'INVALID': "Invalid",
+            'MODIFIED': "Modified",
+            'SUBMITTED': "Submitted",
+            'REVIEWED': "Reviewed",
+            'APPROVED': "Approved",
+        },
+        ('booking_status',): {
+            'NOTSUBMITTED': "NotSubmitted",
+            'SUBMITTED': "Submitted",
+            'REJECTED': "Rejected",
+            'APPROVED': "Approved",
         },
-        ('pacing',): {
-            'UNKNOWN': "unknown",
-            'STANDARD': "standard",
-            'ACCELERATED': "accelerated",
+        ('runnable_status',): {
+            'NOTSUBMITTED': "NotSubmitted",
+            'SUBMITTED': "Submitted",
+            'REJECTED': "Rejected",
+            'APPROVED': "Approved",
         },
     }
 
     validations = {
-        ('name',): {
-            'max_length': 255,
-            'min_length': 0,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'start_date': (date,),  # noqa: E501
-            'end_date': (date,),  # noqa: E501
-            'status': (str,),  # noqa: E501
-            'pacing': (str,),  # noqa: E501
-            'capping': (ExternalLineItemCapping202110,),  # noqa: E501
-            'page': (ExternalLineItemPage202110,),  # noqa: E501
-            'budget': (float,),  # noqa: E501
-            'creative_id': (str, none_type,),  # noqa: E501
+            'negotiation_state': (str,),  # noqa: E501
+            'booking_status': (str,),  # noqa: E501
+            'runnable_status': (str,),  # noqa: E501
+            'comment': (str,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'updated_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'start_date': 'startDate',  # noqa: E501
-        'end_date': 'endDate',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'pacing': 'pacing',  # noqa: E501
-        'capping': 'capping',  # noqa: E501
-        'page': 'page',  # noqa: E501
-        'budget': 'budget',  # noqa: E501
-        'creative_id': 'creativeId',  # noqa: E501
+        'negotiation_state': 'negotiationState',  # noqa: E501
+        'booking_status': 'bookingStatus',  # noqa: E501
+        'runnable_status': 'runnableStatus',  # noqa: E501
+        'comment': 'comment',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
+        'updated_at': 'updatedAt',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, start_date, end_date, status, *args, **kwargs):  # noqa: E501
-        """ExternalPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
+    def _from_openapi_data(cls, negotiation_state, booking_status, runnable_status, *args, **kwargs):  # noqa: E501
+        """RetailMediaExternalv1ProposalStatusModel - a model defined in OpenAPI
 
         Args:
-            name (str):
-            start_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
-            end_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
-            status (str):
+            negotiation_state (str):
+            booking_status (str):
+            runnable_status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -180,19 +164,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pacing (str): [optional] if omitted the server will use the default value of "accelerated"  # noqa: E501
-            capping (ExternalLineItemCapping202110): [optional]  # noqa: E501
-            page (ExternalLineItemPage202110): [optional]  # noqa: E501
-            budget (float): [optional]  # noqa: E501
-            creative_id (str, none_type): [optional]  # noqa: E501
+            comment (str): [optional]  # noqa: E501
+            created_at (datetime): [optional]  # noqa: E501
+            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,18 +198,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.start_date = start_date
-        self.end_date = end_date
-        self.status = status
+        self.negotiation_state = negotiation_state
+        self.booking_status = booking_status
+        self.runnable_status = runnable_status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -240,22 +221,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, start_date, end_date, status, *args, **kwargs):  # noqa: E501
-        """ExternalPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
+    def __init__(self, negotiation_state, booking_status, runnable_status, *args, **kwargs):  # noqa: E501
+        """RetailMediaExternalv1ProposalStatusModel - a model defined in OpenAPI
 
         Args:
-            name (str):
-            start_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
-            end_date (date): Represents the Date as a year, month, and day in the format YYYY-MM-DD
-            status (str):
+            negotiation_state (str):
+            booking_status (str):
+            runnable_status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -280,19 +260,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pacing (str): [optional] if omitted the server will use the default value of "accelerated"  # noqa: E501
-            capping (ExternalLineItemCapping202110): [optional]  # noqa: E501
-            page (ExternalLineItemPage202110): [optional]  # noqa: E501
-            budget (float): [optional]  # noqa: E501
-            creative_id (str, none_type): [optional]  # noqa: E501
+            comment (str): [optional]  # noqa: E501
+            created_at (datetime): [optional]  # noqa: E501
+            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -314,18 +292,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.start_date = start_date
-        self.end_date = end_date
-        self.status = status
+        self.negotiation_state = negotiation_state
+        self.booking_status = booking_status
+        self.runnable_status = runnable_status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalPromotedProduct202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_retailer.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalRetailer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_retailer_pages202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalRetailerPages202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalStoreIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/external_store_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ExternalStoreTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/files_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variable_value.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class FilesVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/files_variables_specification.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class FilesVariablesSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/get_page_of_audiences_by_account_id_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py`

 * *Files 1% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.retail_media_audience import RetailMediaAudience
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.retail_media_audience import RetailMediaAudience
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['PageMetadata'] = PageMetadata
     globals()['RetailMediaAudience'] = RetailMediaAudience
 
 
 class GetPageOfAudiencesByAccountIdResponse(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/hyperlink_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class HyperlinkVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/input_resource_of_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
+    from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
     globals()['ExternalAuctionLineItemCreateModel'] = ExternalAuctionLineItemCreateModel
 
 
 class InputResourceOfAuctionLineItemCreateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/input_resource_of_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
+    from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
     globals()['ExternalPreferredLineItemCreateModel202110'] = ExternalPreferredLineItemCreateModel202110
 
 
 class InputResourceOfPreferredLineItemCreateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
+    from criteo_api_retailmedia_v2023_04.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
     globals()['EditableCampaignAttributesV202301'] = EditableCampaignAttributesV202301
 
 
 class JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_account_and_account.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_account import ExternalAccount
+    from criteo_api_retailmedia_v2023_04.model.external_account import ExternalAccount
     globals()['ExternalAccount'] = ExternalAccount
 
 
 class JsonApiBodyWithIdOfInt64AndAccountAndAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_brand import ExternalBrand
+    from criteo_api_retailmedia_v2023_04.model.external_brand import ExternalBrand
     globals()['ExternalBrand'] = ExternalBrand
 
 
 class JsonApiBodyWithIdOfInt64AndBrandAndBrand(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.campaign_v202301 import CampaignV202301
+    from criteo_api_retailmedia_v2023_04.model.campaign_v202301 import CampaignV202301
     globals()['CampaignV202301'] = CampaignV202301
 
 
 class JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_catalog_status import ExternalCatalogStatus
+    from criteo_api_retailmedia_v2023_04.model.external_catalog_status import ExternalCatalogStatus
     globals()['ExternalCatalogStatus'] = ExternalCatalogStatus
 
 
 class JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers import LineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers import LineItemBidMultipliers
     globals()['LineItemBidMultipliers'] = LineItemBidMultipliers
 
 
 class JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_retailer import ExternalRetailer
+    from criteo_api_retailmedia_v2023_04.model.external_retailer import ExternalRetailer
     globals()['ExternalRetailer'] = ExternalRetailer
 
 
 class JsonApiBodyWithIdOfInt64AndRetailerAndRetailer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.campaign_attributes_v202301 import CampaignAttributesV202301
+    from criteo_api_retailmedia_v2023_04.model.campaign_attributes_v202301 import CampaignAttributesV202301
     globals()['CampaignAttributesV202301'] = CampaignAttributesV202301
 
 
 class JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_catalog_request import ExternalCatalogRequest
+    from criteo_api_retailmedia_v2023_04.model.external_catalog_request import ExternalCatalogRequest
     globals()['ExternalCatalogRequest'] = ExternalCatalogRequest
 
 
 class JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_account.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndAccountAndAccount'] = JsonApiBodyWithIdOfInt64AndAccountAndAccount
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfAccount(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_brand.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py`

 * *Files 1% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndBrandAndBrand'] = JsonApiBodyWithIdOfInt64AndBrandAndBrand
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfBrand(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301'] = JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfCampaignV202301(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_page_response_of_retailer.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py`

 * *Files 0% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndRetailerAndRetailer'] = JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfRetailer(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_request_of_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
     globals()['JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest'] = JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
 
 
 class JsonApiRequestOfCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301'] = JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
 
 
 class JsonApiSingleResponseOfCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus'] = JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
 
 
 class JsonApiSingleResponseOfCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/json_api_single_response_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py`

 * *Files 0% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers'] = JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
 
 
 class JsonApiSingleResponseOfLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/keyword_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
     globals()['ValueTypeResourceOfKeywordTarget202110'] = ValueTypeResourceOfKeywordTarget202110
 
 
 class KeywordTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/keyword_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfKeywordTarget202110'] = ValueTypeResourceOfKeywordTarget202110
 
 
 class KeywordTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class LineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
     globals()['ResourceOfLineItemBidMultipliers'] = ResourceOfLineItemBidMultipliers
 
 
 class LineItemBidMultipliersRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/line_item_bid_multipliers_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfLineItemBidMultipliers'] = ResourceOfLineItemBidMultipliers
 
 
 class LineItemBidMultipliersResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/map_string.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/map_string.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class MapString(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/page_metadata.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/page_metadata.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class PageMetadata(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/post_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
     globals()['JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301'] = JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
 
 
 class PostCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPreferredLineItem202110'] = ResourceOfPreferredLineItem202110
 
 
 class PreferredLineItem202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py`

 * *Files 3% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPreferredLineItem202110'] = ResourceOfPreferredLineItem202110
 
 
 class PreferredLineItem202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item_create_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
+    from criteo_api_retailmedia_v2023_04.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
     globals()['InputResourceOfPreferredLineItemCreateModel202110'] = InputResourceOfPreferredLineItemCreateModel202110
 
 
 class PreferredLineItemCreateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/preferred_line_item_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
     globals()['ResourceOfPreferredLineItemUpdateModel202110'] = ResourceOfPreferredLineItemUpdateModel202110
 
 
 class PreferredLineItemUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/problem_details.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/problem_details.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ProblemDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/promoted_product202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+    from criteo_api_retailmedia_v2023_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
     globals()['ResourceOfPromotedProduct202110'] = ResourceOfPromotedProduct202110
 
 
 class PromotedProduct202110ListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/promoted_product202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py`

 * *Files 4% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPromotedProduct202110'] = ResourceOfPromotedProduct202110
 
 
 class PromotedProduct202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/put_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
     globals()['JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301'] = JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
 
 
 class PutCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.report_request_attributes import ReportRequestAttributes
+    from criteo_api_retailmedia_v2023_04.model.report_request_attributes import ReportRequestAttributes
     globals()['ReportRequestAttributes'] = ReportRequestAttributes
 
 
 class ReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_request_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ReportRequestAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.report_status_attributes import ReportStatusAttributes
+    from criteo_api_retailmedia_v2023_04.model.report_status_attributes import ReportStatusAttributes
     globals()['ReportStatusAttributes'] = ReportStatusAttributes
 
 
 class ReportStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/report_status_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ReportStatusAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_auction_line_item import ExternalAuctionLineItem
+    from criteo_api_retailmedia_v2023_04.model.external_auction_line_item import ExternalAuctionLineItem
     globals()['ExternalAuctionLineItem'] = ExternalAuctionLineItem
 
 
 class ResourceOfAuctionLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
+    from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
     globals()['ExternalAuctionLineItemUpdateModel'] = ExternalAuctionLineItemUpdateModel
 
 
 class ResourceOfAuctionLineItemUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_balance202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_balance202110 import ExternalBalance202110
+    from criteo_api_retailmedia_v2023_04.model.external_balance202110 import ExternalBalance202110
     globals()['ExternalBalance202110'] = ExternalBalance202110
 
 
 class ResourceOfBalance202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_balance_campaign202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class ResourceOfBalanceCampaign202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_category202204.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.category202204 import Category202204
+    from criteo_api_retailmedia_v2023_04.model.category202204 import Category202204
     globals()['Category202204'] = Category202204
 
 
 class ResourceOfCategory202204(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_common_line_item import ExternalCommonLineItem
+    from criteo_api_retailmedia_v2023_04.model.external_common_line_item import ExternalCommonLineItem
     globals()['ExternalCommonLineItem'] = ExternalCommonLineItem
 
 
 class ResourceOfCommonLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_creative202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.creative202110 import Creative202110
+    from criteo_api_retailmedia_v2023_04.model.creative202110 import Creative202110
     globals()['Creative202110'] = Creative202110
 
 
 class ResourceOfCreative202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_creative202207.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py`

 * *Files 4% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.creative202207 import Creative202207
-    globals()['Creative202207'] = Creative202207
+    from criteo_api_retailmedia_v2023_04.model.creative202210 import Creative202210
+    globals()['Creative202210'] = Creative202210
 
 
-class ResourceOfCreative202207(ModelNormal):
+class ResourceOfCreative202210(ModelNormal):
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
-            'attributes': (Creative202207,),  # noqa: E501
+            'attributes': (Creative202210,),  # noqa: E501
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
-        """ResourceOfCreative202207 - a model defined in OpenAPI
+        """ResourceOfCreative202210 - a model defined in OpenAPI
 
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
-            attributes (Creative202207): [optional]  # noqa: E501
+            attributes (Creative202210): [optional]  # noqa: E501
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
-        """ResourceOfCreative202207 - a model defined in OpenAPI
+        """ResourceOfCreative202210 - a model defined in OpenAPI
 
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
-            attributes (Creative202207): [optional]  # noqa: E501
+            attributes (Creative202210): [optional]  # noqa: E501
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers import LineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers import LineItemBidMultipliers
     globals()['LineItemBidMultipliers'] = LineItemBidMultipliers
 
 
 class ResourceOfLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
+    from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
     globals()['ExternalPreferredLineItem202110'] = ExternalPreferredLineItem202110
 
 
 class ResourceOfPreferredLineItem202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
     globals()['ExternalPreferredLineItemUpdateModel202110'] = ExternalPreferredLineItemUpdateModel202110
 
 
 class ResourceOfPreferredLineItemUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_promoted_product202110 import ExternalPromotedProduct202110
+    from criteo_api_retailmedia_v2023_04.model.external_promoted_product202110 import ExternalPromotedProduct202110
     globals()['ExternalPromotedProduct202110'] = ExternalPromotedProduct202110
 
 
 class ResourceOfPromotedProduct202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/resource_of_template.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_template.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.template import Template
+    from criteo_api_retailmedia_v2023_04.model.template import Template
     globals()['Template'] = Template
 
 
 class ResourceOfTemplate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
+    from criteo_api_retailmedia_v2023_04.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
     globals()['RetailMediaAudienceAttributes'] = RetailMediaAudienceAttributes
 
 
 class RetailMediaAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py`

 * *Files 2% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.customer_list_details import CustomerListDetails
-    from criteo_api_retailmedia_v2023_01.model.user_behavior_details import UserBehaviorDetails
+    from criteo_api_retailmedia_v2023_04.model.customer_list_details import CustomerListDetails
+    from criteo_api_retailmedia_v2023_04.model.user_behavior_details_v2 import UserBehaviorDetailsV2
     globals()['CustomerListDetails'] = CustomerListDetails
-    globals()['UserBehaviorDetails'] = UserBehaviorDetails
+    globals()['UserBehaviorDetailsV2'] = UserBehaviorDetailsV2
 
 
-class RetailMediaAudienceAttributes(ModelNormal):
+class RetailMediaAudienceV2Attributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -87,15 +87,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'retailer_id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'user_behavior_details': (UserBehaviorDetails,),  # noqa: E501
+            'user_behavior_details': (UserBehaviorDetailsV2,),  # noqa: E501
             'customer_list_details': (CustomerListDetails,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, retailer_id, name, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceAttributes - a model defined in OpenAPI
+        """RetailMediaAudienceV2Attributes - a model defined in OpenAPI
 
         Args:
             retailer_id (str): ID of the retailer associated with this audience
             name (str): Name of the audience.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -148,15 +148,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_behavior_details (UserBehaviorDetails): [optional]  # noqa: E501
+            user_behavior_details (UserBehaviorDetailsV2): [optional]  # noqa: E501
             customer_list_details (CustomerListDetails): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -204,15 +204,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, retailer_id, name, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceAttributes - a model defined in OpenAPI
+        """RetailMediaAudienceV2Attributes - a model defined in OpenAPI
 
         Args:
             retailer_id (str): ID of the retailer associated with this audience
             name (str): Name of the audience.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -241,15 +241,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_behavior_details (UserBehaviorDetails): [optional]  # noqa: E501
+            user_behavior_details (UserBehaviorDetailsV2): [optional]  # noqa: E501
             customer_list_details (CustomerListDetails): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
+    from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
     globals()['RetailMediaAudienceV2Attributes'] = RetailMediaAudienceV2Attributes
 
 
 class RetailMediaAudienceV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py`

 * *Files 2% similar despite different names*

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.customer_list_details import CustomerListDetails
-    from criteo_api_retailmedia_v2023_01.model.user_behavior_details_v2 import UserBehaviorDetailsV2
+    from criteo_api_retailmedia_v2023_04.model.customer_list_details import CustomerListDetails
+    from criteo_api_retailmedia_v2023_04.model.user_behavior_details import UserBehaviorDetails
     globals()['CustomerListDetails'] = CustomerListDetails
-    globals()['UserBehaviorDetailsV2'] = UserBehaviorDetailsV2
+    globals()['UserBehaviorDetails'] = UserBehaviorDetails
 
 
-class RetailMediaAudienceV2Attributes(ModelNormal):
+class RetailMediaAudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -87,15 +87,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'retailer_id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'user_behavior_details': (UserBehaviorDetailsV2,),  # noqa: E501
+            'user_behavior_details': (UserBehaviorDetails,),  # noqa: E501
             'customer_list_details': (CustomerListDetails,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, retailer_id, name, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceV2Attributes - a model defined in OpenAPI
+        """RetailMediaAudienceAttributes - a model defined in OpenAPI
 
         Args:
             retailer_id (str): ID of the retailer associated with this audience
             name (str): Name of the audience.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -148,15 +148,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_behavior_details (UserBehaviorDetailsV2): [optional]  # noqa: E501
+            user_behavior_details (UserBehaviorDetails): [optional]  # noqa: E501
             customer_list_details (CustomerListDetails): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -204,15 +204,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, retailer_id, name, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceV2Attributes - a model defined in OpenAPI
+        """RetailMediaAudienceAttributes - a model defined in OpenAPI
 
         Args:
             retailer_id (str): ID of the retailer associated with this audience
             name (str): Name of the audience.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -241,15 +241,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_behavior_details (UserBehaviorDetailsV2): [optional]  # noqa: E501
+            user_behavior_details (UserBehaviorDetails): [optional]  # noqa: E501
             customer_list_details (CustomerListDetails): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2 import RetailMediaAudienceV2
+    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2 import RetailMediaAudienceV2
     globals()['CommonProblem'] = CommonProblem
     globals()['PageMetadata'] = PageMetadata
     globals()['RetailMediaAudienceV2'] = RetailMediaAudienceV2
 
 
 class RetailMediaAudienceV2ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/retail_media_audience_v2_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
+    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
     globals()['CommonProblem'] = CommonProblem
     globals()['CreateRetailMediaAudienceV2'] = CreateRetailMediaAudienceV2
 
 
 class RetailMediaAudienceV2Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/section.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/section.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.template_variable import TemplateVariable
+    from criteo_api_retailmedia_v2023_04.model.template_variable import TemplateVariable
     globals()['TemplateVariable'] = TemplateVariable
 
 
 class Section(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/store_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
     globals()['ValueTypeResourceOfStoreIdsUpdateModel202110'] = ValueTypeResourceOfStoreIdsUpdateModel202110
 
 
 class StoreIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/store_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
     globals()['ValueTypeResourceOfStoreTarget202110'] = ValueTypeResourceOfStoreTarget202110
 
 
 class StoreTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/store_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfStoreTarget202110'] = ValueTypeResourceOfStoreTarget202110
 
 
 class StoreTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.section import Section
+    from criteo_api_retailmedia_v2023_04.model.section import Section
     globals()['Section'] = Section
 
 
 class Template(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_list_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_template import ResourceOfTemplate
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_template import ResourceOfTemplate
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfTemplate'] = ResourceOfTemplate
 
 
 class TemplateListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_response.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_01.model.resource_of_template import ResourceOfTemplate
+    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_04.model.resource_of_template import ResourceOfTemplate
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfTemplate'] = ResourceOfTemplate
 
 
 class TemplateResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_variable.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.choice_variable_specification import ChoiceVariableSpecification
-    from criteo_api_retailmedia_v2023_01.model.files_variables_specification import FilesVariablesSpecification
-    from criteo_api_retailmedia_v2023_01.model.text_variable_specification import TextVariableSpecification
+    from criteo_api_retailmedia_v2023_04.model.choice_variable_specification import ChoiceVariableSpecification
+    from criteo_api_retailmedia_v2023_04.model.files_variables_specification import FilesVariablesSpecification
+    from criteo_api_retailmedia_v2023_04.model.text_variable_specification import TextVariableSpecification
     globals()['ChoiceVariableSpecification'] = ChoiceVariableSpecification
     globals()['FilesVariablesSpecification'] = FilesVariablesSpecification
     globals()['TextVariableSpecification'] = TextVariableSpecification
 
 
 class TemplateVariable(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/template_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable_value.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.choice_variable_value import ChoiceVariableValue
-    from criteo_api_retailmedia_v2023_01.model.color_variable_value import ColorVariableValue
-    from criteo_api_retailmedia_v2023_01.model.files_variable_value import FilesVariableValue
-    from criteo_api_retailmedia_v2023_01.model.hyperlink_variable_value import HyperlinkVariableValue
-    from criteo_api_retailmedia_v2023_01.model.text_variable_value import TextVariableValue
+    from criteo_api_retailmedia_v2023_04.model.choice_variable_value import ChoiceVariableValue
+    from criteo_api_retailmedia_v2023_04.model.color_variable_value import ColorVariableValue
+    from criteo_api_retailmedia_v2023_04.model.files_variable_value import FilesVariableValue
+    from criteo_api_retailmedia_v2023_04.model.hyperlink_variable_value import HyperlinkVariableValue
+    from criteo_api_retailmedia_v2023_04.model.text_variable_value import TextVariableValue
     globals()['ChoiceVariableValue'] = ChoiceVariableValue
     globals()['ColorVariableValue'] = ColorVariableValue
     globals()['FilesVariableValue'] = FilesVariableValue
     globals()['HyperlinkVariableValue'] = HyperlinkVariableValue
     globals()['TextVariableValue'] = TextVariableValue
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/text_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class TextVariableSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/text_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_value.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class TextVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/user_behavior_details.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 
 class UserBehaviorDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/user_behavior_details_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
+    from criteo_api_retailmedia_v2023_04.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
     globals()['CreateUserBehaviorSegmentV2'] = CreateUserBehaviorSegmentV2
 
 
 class UserBehaviorDetailsV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
     globals()['ExternalAddToBasketIdsUpdateModel202110'] = ExternalAddToBasketIdsUpdateModel202110
 
 
 class ValueTypeResourceOfAddToBasketIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
+    from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
     globals()['ExternalAddToBasketTarget202110'] = ExternalAddToBasketTarget202110
 
 
 class ValueTypeResourceOfAddToBasketTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
     globals()['ExternalAudienceIdsUpdateModel202110'] = ExternalAudienceIdsUpdateModel202110
 
 
 class ValueTypeResourceOfAudienceIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_audience_target202110 import ExternalAudienceTarget202110
+    from criteo_api_retailmedia_v2023_04.model.external_audience_target202110 import ExternalAudienceTarget202110
     globals()['ExternalAudienceTarget202110'] = ExternalAudienceTarget202110
 
 
 class ValueTypeResourceOfAudienceTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_keyword_target202110 import ExternalKeywordTarget202110
+    from criteo_api_retailmedia_v2023_04.model.external_keyword_target202110 import ExternalKeywordTarget202110
     globals()['ExternalKeywordTarget202110'] = ExternalKeywordTarget202110
 
 
 class ValueTypeResourceOfKeywordTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_04.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
     globals()['ExternalStoreIdsUpdateModel202110'] = ExternalStoreIdsUpdateModel202110
 
 
 class ValueTypeResourceOfStoreIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model/value_type_resource_of_store_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py`

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
 
-from criteo_api_retailmedia_v2023_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2023_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_01.model.external_store_target202110 import ExternalStoreTarget202110
+    from criteo_api_retailmedia_v2023_04.model.external_store_target202110 import ExternalStoreTarget202110
     globals()['ExternalStoreTarget202110'] = ExternalStoreTarget202110
 
 
 class ValueTypeResourceOfStoreTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/model_utils.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model_utils.py`

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
 
-from criteo_api_retailmedia_v2023_01.exceptions import (
+from criteo_api_retailmedia_v2023_04.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/models/__init__.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,173 +1,193 @@
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from criteo_api_retailmedia_v2023_01.model.pet import Pet
+# from criteo_api_retailmedia_v2023_04.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from criteo_api_retailmedia_v2023_01.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.application_summary_model import ApplicationSummaryModel
-from criteo_api_retailmedia_v2023_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-from criteo_api_retailmedia_v2023_01.model.application_summary_model_response import ApplicationSummaryModelResponse
-from criteo_api_retailmedia_v2023_01.model.asset import Asset
-from criteo_api_retailmedia_v2023_01.model.asset_resource import AssetResource
-from criteo_api_retailmedia_v2023_01.model.asset_response import AssetResponse
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_response import AuctionLineItemResponse
-from criteo_api_retailmedia_v2023_01.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
-from criteo_api_retailmedia_v2023_01.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.audience_target202110_request import AudienceTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.audience_target202110_response import AudienceTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.bad_request import BadRequest
-from criteo_api_retailmedia_v2023_01.model.balance202110_paged_list_response import Balance202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
-from criteo_api_retailmedia_v2023_01.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.campaign_attributes_v202301 import CampaignAttributesV202301
-from criteo_api_retailmedia_v2023_01.model.campaign_v202301 import CampaignV202301
-from criteo_api_retailmedia_v2023_01.model.category202204 import Category202204
-from criteo_api_retailmedia_v2023_01.model.category202204_list_response import Category202204ListResponse
-from criteo_api_retailmedia_v2023_01.model.choice_option import ChoiceOption
-from criteo_api_retailmedia_v2023_01.model.choice_variable_specification import ChoiceVariableSpecification
-from criteo_api_retailmedia_v2023_01.model.choice_variable_value import ChoiceVariableValue
-from criteo_api_retailmedia_v2023_01.model.color_variable_value import ColorVariableValue
-from criteo_api_retailmedia_v2023_01.model.common_error import CommonError
-from criteo_api_retailmedia_v2023_01.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_01.model.common_line_item_response import CommonLineItemResponse
-from criteo_api_retailmedia_v2023_01.model.common_problem import CommonProblem
-from criteo_api_retailmedia_v2023_01.model.common_status_code_response import CommonStatusCodeResponse
-from criteo_api_retailmedia_v2023_01.model.common_warning import CommonWarning
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience import CreateRetailMediaAudience
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
-from criteo_api_retailmedia_v2023_01.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
-from criteo_api_retailmedia_v2023_01.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
-from criteo_api_retailmedia_v2023_01.model.creative202110 import Creative202110
-from criteo_api_retailmedia_v2023_01.model.creative202110_list_response import Creative202110ListResponse
-from criteo_api_retailmedia_v2023_01.model.creative202207 import Creative202207
-from criteo_api_retailmedia_v2023_01.model.creative202207_response import Creative202207Response
-from criteo_api_retailmedia_v2023_01.model.creative_create_model202207 import CreativeCreateModel202207
-from criteo_api_retailmedia_v2023_01.model.creative_update_model202207 import CreativeUpdateModel202207
-from criteo_api_retailmedia_v2023_01.model.customer_list_details import CustomerListDetails
-from criteo_api_retailmedia_v2023_01.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
-from criteo_api_retailmedia_v2023_01.model.envelope_report_request import EnvelopeReportRequest
-from criteo_api_retailmedia_v2023_01.model.envelope_report_status import EnvelopeReportStatus
-from criteo_api_retailmedia_v2023_01.model.error import Error
-from criteo_api_retailmedia_v2023_01.model.external_account import ExternalAccount
-from criteo_api_retailmedia_v2023_01.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
-from criteo_api_retailmedia_v2023_01.model.external_auction_line_item import ExternalAuctionLineItem
-from criteo_api_retailmedia_v2023_01.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
-from criteo_api_retailmedia_v2023_01.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
-from criteo_api_retailmedia_v2023_01.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.external_audience_target202110 import ExternalAudienceTarget202110
-from criteo_api_retailmedia_v2023_01.model.external_balance202110 import ExternalBalance202110
-from criteo_api_retailmedia_v2023_01.model.external_brand import ExternalBrand
-from criteo_api_retailmedia_v2023_01.model.external_catalog_request import ExternalCatalogRequest
-from criteo_api_retailmedia_v2023_01.model.external_catalog_status import ExternalCatalogStatus
-from criteo_api_retailmedia_v2023_01.model.external_common_line_item import ExternalCommonLineItem
-from criteo_api_retailmedia_v2023_01.model.external_keyword_target202110 import ExternalKeywordTarget202110
-from criteo_api_retailmedia_v2023_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-from criteo_api_retailmedia_v2023_01.model.external_line_item_page202110 import ExternalLineItemPage202110
-from criteo_api_retailmedia_v2023_01.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
-from criteo_api_retailmedia_v2023_01.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
-from criteo_api_retailmedia_v2023_01.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
-from criteo_api_retailmedia_v2023_01.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.external_promoted_product202110 import ExternalPromotedProduct202110
-from criteo_api_retailmedia_v2023_01.model.external_retailer import ExternalRetailer
-from criteo_api_retailmedia_v2023_01.model.external_retailer_pages202110 import ExternalRetailerPages202110
-from criteo_api_retailmedia_v2023_01.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.external_store_target202110 import ExternalStoreTarget202110
-from criteo_api_retailmedia_v2023_01.model.files_variable_value import FilesVariableValue
-from criteo_api_retailmedia_v2023_01.model.files_variables_specification import FilesVariablesSpecification
-from criteo_api_retailmedia_v2023_01.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
-from criteo_api_retailmedia_v2023_01.model.hyperlink_variable_value import HyperlinkVariableValue
-from criteo_api_retailmedia_v2023_01.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
-from criteo_api_retailmedia_v2023_01.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
-from criteo_api_retailmedia_v2023_01.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
-from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
-from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
-from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_01.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
-from criteo_api_retailmedia_v2023_01.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
-from criteo_api_retailmedia_v2023_01.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
-from criteo_api_retailmedia_v2023_01.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
-from criteo_api_retailmedia_v2023_01.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_01.model.keyword_target202110_request import KeywordTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.keyword_target202110_response import KeywordTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers import LineItemBidMultipliers
-from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
-from criteo_api_retailmedia_v2023_01.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
-from criteo_api_retailmedia_v2023_01.model.map_string import MapString
-from criteo_api_retailmedia_v2023_01.model.page_metadata import PageMetadata
-from criteo_api_retailmedia_v2023_01.model.post_campaign_v202301 import PostCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item202110_response import PreferredLineItem202110Response
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.problem_details import ProblemDetails
-from criteo_api_retailmedia_v2023_01.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
-from criteo_api_retailmedia_v2023_01.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
-from criteo_api_retailmedia_v2023_01.model.put_campaign_v202301 import PutCampaignV202301
-from criteo_api_retailmedia_v2023_01.model.report_request import ReportRequest
-from criteo_api_retailmedia_v2023_01.model.report_request_attributes import ReportRequestAttributes
-from criteo_api_retailmedia_v2023_01.model.report_status import ReportStatus
-from criteo_api_retailmedia_v2023_01.model.report_status_attributes import ReportStatusAttributes
-from criteo_api_retailmedia_v2023_01.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
-from criteo_api_retailmedia_v2023_01.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
-from criteo_api_retailmedia_v2023_01.model.resource_of_balance202110 import ResourceOfBalance202110
-from criteo_api_retailmedia_v2023_01.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
-from criteo_api_retailmedia_v2023_01.model.resource_of_category202204 import ResourceOfCategory202204
-from criteo_api_retailmedia_v2023_01.model.resource_of_common_line_item import ResourceOfCommonLineItem
-from criteo_api_retailmedia_v2023_01.model.resource_of_creative202110 import ResourceOfCreative202110
-from criteo_api_retailmedia_v2023_01.model.resource_of_creative202207 import ResourceOfCreative202207
-from criteo_api_retailmedia_v2023_01.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_01.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
-from criteo_api_retailmedia_v2023_01.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
-from criteo_api_retailmedia_v2023_01.model.resource_of_template import ResourceOfTemplate
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience import RetailMediaAudience
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2 import RetailMediaAudienceV2
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
-from criteo_api_retailmedia_v2023_01.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
-from criteo_api_retailmedia_v2023_01.model.section import Section
-from criteo_api_retailmedia_v2023_01.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_01.model.store_target202110_request import StoreTarget202110Request
-from criteo_api_retailmedia_v2023_01.model.store_target202110_response import StoreTarget202110Response
-from criteo_api_retailmedia_v2023_01.model.template import Template
-from criteo_api_retailmedia_v2023_01.model.template_list_response import TemplateListResponse
-from criteo_api_retailmedia_v2023_01.model.template_response import TemplateResponse
-from criteo_api_retailmedia_v2023_01.model.template_variable import TemplateVariable
-from criteo_api_retailmedia_v2023_01.model.template_variable_value import TemplateVariableValue
-from criteo_api_retailmedia_v2023_01.model.text_variable_specification import TextVariableSpecification
-from criteo_api_retailmedia_v2023_01.model.text_variable_value import TextVariableValue
-from criteo_api_retailmedia_v2023_01.model.user_behavior_details import UserBehaviorDetails
-from criteo_api_retailmedia_v2023_01.model.user_behavior_details_v2 import UserBehaviorDetailsV2
-from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
-from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
-from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
-from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_01.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+from criteo_api_retailmedia_v2023_04.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.application_summary_model import ApplicationSummaryModel
+from criteo_api_retailmedia_v2023_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+from criteo_api_retailmedia_v2023_04.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_retailmedia_v2023_04.model.asset import Asset
+from criteo_api_retailmedia_v2023_04.model.asset_resource import AssetResource
+from criteo_api_retailmedia_v2023_04.model.asset_response import AssetResponse
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_response import AuctionLineItemResponse
+from criteo_api_retailmedia_v2023_04.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
+from criteo_api_retailmedia_v2023_04.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.audience_target202110_request import AudienceTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.audience_target202110_response import AudienceTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.bad_request import BadRequest
+from criteo_api_retailmedia_v2023_04.model.balance202110_paged_list_response import Balance202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
+from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.campaign_attributes_v202301 import CampaignAttributesV202301
+from criteo_api_retailmedia_v2023_04.model.campaign_v202301 import CampaignV202301
+from criteo_api_retailmedia_v2023_04.model.category202204 import Category202204
+from criteo_api_retailmedia_v2023_04.model.category202204_list_response import Category202204ListResponse
+from criteo_api_retailmedia_v2023_04.model.choice_option import ChoiceOption
+from criteo_api_retailmedia_v2023_04.model.choice_variable_specification import ChoiceVariableSpecification
+from criteo_api_retailmedia_v2023_04.model.choice_variable_value import ChoiceVariableValue
+from criteo_api_retailmedia_v2023_04.model.color_variable_value import ColorVariableValue
+from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
+from criteo_api_retailmedia_v2023_04.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_04.model.common_line_item_response import CommonLineItemResponse
+from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
+from criteo_api_retailmedia_v2023_04.model.common_status_code_response import CommonStatusCodeResponse
+from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience import CreateRetailMediaAudience
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
+from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
+from criteo_api_retailmedia_v2023_04.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
+from criteo_api_retailmedia_v2023_04.model.creative202110 import Creative202110
+from criteo_api_retailmedia_v2023_04.model.creative202110_list_response import Creative202110ListResponse
+from criteo_api_retailmedia_v2023_04.model.creative202210 import Creative202210
+from criteo_api_retailmedia_v2023_04.model.creative202210_list_response import Creative202210ListResponse
+from criteo_api_retailmedia_v2023_04.model.creative202210_response import Creative202210Response
+from criteo_api_retailmedia_v2023_04.model.creative_create_model202207 import CreativeCreateModel202207
+from criteo_api_retailmedia_v2023_04.model.creative_update_model202207 import CreativeUpdateModel202207
+from criteo_api_retailmedia_v2023_04.model.customer_list_details import CustomerListDetails
+from criteo_api_retailmedia_v2023_04.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
+from criteo_api_retailmedia_v2023_04.model.envelope_report_request import EnvelopeReportRequest
+from criteo_api_retailmedia_v2023_04.model.envelope_report_status import EnvelopeReportStatus
+from criteo_api_retailmedia_v2023_04.model.error import Error
+from criteo_api_retailmedia_v2023_04.model.external_account import ExternalAccount
+from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
+from criteo_api_retailmedia_v2023_04.model.external_auction_line_item import ExternalAuctionLineItem
+from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
+from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
+from criteo_api_retailmedia_v2023_04.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.external_audience_target202110 import ExternalAudienceTarget202110
+from criteo_api_retailmedia_v2023_04.model.external_balance202110 import ExternalBalance202110
+from criteo_api_retailmedia_v2023_04.model.external_brand import ExternalBrand
+from criteo_api_retailmedia_v2023_04.model.external_catalog_request import ExternalCatalogRequest
+from criteo_api_retailmedia_v2023_04.model.external_catalog_status import ExternalCatalogStatus
+from criteo_api_retailmedia_v2023_04.model.external_common_line_item import ExternalCommonLineItem
+from criteo_api_retailmedia_v2023_04.model.external_keyword_target202110 import ExternalKeywordTarget202110
+from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
+from criteo_api_retailmedia_v2023_04.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
+from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
+from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
+from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.external_promoted_product202110 import ExternalPromotedProduct202110
+from criteo_api_retailmedia_v2023_04.model.external_retailer import ExternalRetailer
+from criteo_api_retailmedia_v2023_04.model.external_retailer_pages202110 import ExternalRetailerPages202110
+from criteo_api_retailmedia_v2023_04.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.external_store_target202110 import ExternalStoreTarget202110
+from criteo_api_retailmedia_v2023_04.model.files_variable_value import FilesVariableValue
+from criteo_api_retailmedia_v2023_04.model.files_variables_specification import FilesVariablesSpecification
+from criteo_api_retailmedia_v2023_04.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
+from criteo_api_retailmedia_v2023_04.model.hyperlink_variable_value import HyperlinkVariableValue
+from criteo_api_retailmedia_v2023_04.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
+from criteo_api_retailmedia_v2023_04.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
+from criteo_api_retailmedia_v2023_04.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
+from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
+from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
+from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
+from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
+from criteo_api_retailmedia_v2023_04.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
+from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
+from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_04.model.keyword_target202110_request import KeywordTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.keyword_target202110_response import KeywordTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers import LineItemBidMultipliers
+from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
+from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
+from criteo_api_retailmedia_v2023_04.model.map_string import MapString
+from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+from criteo_api_retailmedia_v2023_04.model.page_type_environment import PageTypeEnvironment
+from criteo_api_retailmedia_v2023_04.model.post_campaign_v202301 import PostCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_response import PreferredLineItem202110Response
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
+from criteo_api_retailmedia_v2023_04.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
+from criteo_api_retailmedia_v2023_04.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
+from criteo_api_retailmedia_v2023_04.model.put_campaign_v202301 import PutCampaignV202301
+from criteo_api_retailmedia_v2023_04.model.report_request import ReportRequest
+from criteo_api_retailmedia_v2023_04.model.report_request_attributes import ReportRequestAttributes
+from criteo_api_retailmedia_v2023_04.model.report_status import ReportStatus
+from criteo_api_retailmedia_v2023_04.model.report_status_attributes import ReportStatusAttributes
+from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
+from criteo_api_retailmedia_v2023_04.model.resource_of_balance202110 import ResourceOfBalance202110
+from criteo_api_retailmedia_v2023_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+from criteo_api_retailmedia_v2023_04.model.resource_of_category202204 import ResourceOfCategory202204
+from criteo_api_retailmedia_v2023_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
+from criteo_api_retailmedia_v2023_04.model.resource_of_creative202110 import ResourceOfCreative202110
+from criteo_api_retailmedia_v2023_04.model.resource_of_creative202210 import ResourceOfCreative202210
+from criteo_api_retailmedia_v2023_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+from criteo_api_retailmedia_v2023_04.model.resource_of_template import ResourceOfTemplate
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience import RetailMediaAudience
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2 import RetailMediaAudienceV2
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
+from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keyword_model import RetailMediaExternalv1AddRemoveKeywordModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model import RetailMediaExternalv1AddRemoveKeywordsModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model_request import RetailMediaExternalv1AddRemoveKeywordsModelRequest
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model_resource import RetailMediaExternalv1AddRemoveKeywordsModelResource
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_input_keywords_model import RetailMediaExternalv1InputKeywordsModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keyword_data_model import RetailMediaExternalv1KeywordDataModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model import RetailMediaExternalv1KeywordsModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model_resource import RetailMediaExternalv1KeywordsModelResource
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model_response import RetailMediaExternalv1KeywordsModelResponse
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model import RetailMediaExternalv1ProposalStatusModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model_resource import RetailMediaExternalv1ProposalStatusModelResource
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model_response import RetailMediaExternalv1ProposalStatusModelResponse
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_resource_outcome import RetailMediaExternalv1ResourceOutcome
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bid_model import RetailMediaExternalv1SetBidModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model import RetailMediaExternalv1SetBidsModel
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model_request import RetailMediaExternalv1SetBidsModelRequest
+from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model_resource import RetailMediaExternalv1SetBidsModelResource
+from criteo_api_retailmedia_v2023_04.model.section import Section
+from criteo_api_retailmedia_v2023_04.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_04.model.store_target202110_request import StoreTarget202110Request
+from criteo_api_retailmedia_v2023_04.model.store_target202110_response import StoreTarget202110Response
+from criteo_api_retailmedia_v2023_04.model.template import Template
+from criteo_api_retailmedia_v2023_04.model.template_list_response import TemplateListResponse
+from criteo_api_retailmedia_v2023_04.model.template_response import TemplateResponse
+from criteo_api_retailmedia_v2023_04.model.template_variable import TemplateVariable
+from criteo_api_retailmedia_v2023_04.model.template_variable_value import TemplateVariableValue
+from criteo_api_retailmedia_v2023_04.model.text_variable_specification import TextVariableSpecification
+from criteo_api_retailmedia_v2023_04.model.text_variable_value import TextVariableValue
+from criteo_api_retailmedia_v2023_04.model.user_behavior_details import UserBehaviorDetails
+from criteo_api_retailmedia_v2023_04.model.user_behavior_details_v2 import UserBehaviorDetailsV2
+from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/criteo_api_retailmedia_v2023_01/rest.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/rest.py`

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
 
-from criteo_api_retailmedia_v2023_01.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from criteo_api_retailmedia_v2023_04.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/setup.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-retailmedia-sdk"
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
-pip install criteo-api-retailmedia-sdk==2023.01.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230427
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.01.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_01
+import criteo_api_retailmedia_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-retailmedia-sdk-2023.1.0.230427/test/test_gateway_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230427/test/test_gateway_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 
-from criteo_api_retailmedia_v2023_01.api.gateway_api import GatewayApi
-from criteo_api_retailmedia_v2023_01.api_client_builder import ApiClientBuilder
-from criteo_api_retailmedia_v2023_01.rest import ApiException
+from criteo_api_retailmedia_v2023_04.api.gateway_api import GatewayApi
+from criteo_api_retailmedia_v2023_04.api_client_builder import ApiClientBuilder
+from criteo_api_retailmedia_v2023_04.rest import ApiException
 from example_application import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
```

