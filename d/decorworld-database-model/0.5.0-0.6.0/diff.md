# Comparing `tmp/decorworld_database_model-0.5.0.tar.gz` & `tmp/decorworld_database_model-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorworld_database_model-0.5.0.tar", max compression
+gzip compressed data, was "decorworld_database_model-0.6.0.tar", max compression
```

## Comparing `decorworld_database_model-0.5.0.tar` & `decorworld_database_model-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0        0 2022-11-14 11:28:19.771512 decorworld_database_model-0.5.0/decorworld_database_model/__init__.py
--rw-r--r--   0        0        0     2058 2022-11-14 11:36:26.543490 decorworld_database_model-0.5.0/decorworld_database_model/alembic/env.py
--rw-r--r--   0        0        0       38 2022-11-14 11:28:32.706440 decorworld_database_model-0.5.0/decorworld_database_model/alembic/README
--rw-r--r--   0        0        0      510 2022-11-14 11:28:32.707432 decorworld_database_model-0.5.0/decorworld_database_model/alembic/script.py.mako
--rw-r--r--   0        0        0     1091 2022-11-17 17:32:55.256233 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py
--rw-r--r--   0        0        0      833 2022-11-25 16:07:54.940915 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py
--rw-r--r--   0        0        0      923 2022-11-14 11:36:28.443321 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py
--rw-r--r--   0        0        0      971 2022-11-17 17:39:09.649589 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py
--rw-r--r--   0        0        0     1093 2022-11-17 17:32:22.727240 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py
--rw-r--r--   0        0        0      709 2022-11-27 07:47:32.279073 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py
--rw-r--r--   0        0        0     1034 2022-11-25 13:12:14.766306 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py
--rw-r--r--   0        0        0      713 2023-03-29 07:57:25.407378 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py
--rw-r--r--   0        0        0     2041 2022-11-17 17:20:22.941546 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py
--rw-r--r--   0        0        0      870 2022-11-17 17:19:16.180388 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py
--rw-r--r--   0        0        0      943 2022-11-17 17:41:41.614167 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py
--rw-r--r--   0        0        0      852 2022-11-19 09:43:34.355183 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py
--rw-r--r--   0        0        0     1039 2022-11-17 09:29:10.463996 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py
--rw-r--r--   0        0        0     1073 2022-11-17 17:37:07.585121 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py
--rw-r--r--   0        0        0      746 2022-11-14 16:04:04.381269 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py
--rw-r--r--   0        0        0     1241 2022-11-17 15:39:46.868782 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py
--rw-r--r--   0        0        0      790 2022-11-17 17:31:37.522016 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py
--rw-r--r--   0        0        0      948 2022-12-01 09:11:30.894051 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py
--rw-r--r--   0        0        0      706 2022-11-17 18:49:14.442466 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py
--rw-r--r--   0        0        0      866 2022-11-17 17:19:57.038988 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py
--rw-r--r--   0        0        0     1103 2022-11-17 14:11:09.276179 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py
--rw-r--r--   0        0        0      880 2022-11-19 09:34:42.463405 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py
--rw-r--r--   0        0        0      877 2022-11-25 14:27:47.383698 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py
--rw-r--r--   0        0        0      698 2022-11-17 15:39:42.615558 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py
--rw-r--r--   0        0        0      835 2022-11-21 17:24:22.320177 decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py
--rw-r--r--   0        0        0     3234 2022-11-14 11:34:58.943979 decorworld_database_model-0.5.0/decorworld_database_model/alembic.ini
--rw-r--r--   0        0        0      481 2022-11-25 16:07:28.613701 decorworld_database_model-0.5.0/decorworld_database_model/tables/__init__.py
--rw-r--r--   0        0        0     1143 2022-11-17 15:24:28.613902 decorworld_database_model-0.5.0/decorworld_database_model/tables/address.py
--rw-r--r--   0        0        0      160 2022-11-14 11:30:54.004559 decorworld_database_model-0.5.0/decorworld_database_model/tables/base.py
--rw-r--r--   0        0        0      627 2022-11-17 17:31:41.812875 decorworld_database_model-0.5.0/decorworld_database_model/tables/category.py
--rw-r--r--   0        0        0     1081 2022-11-17 17:36:45.627341 decorworld_database_model-0.5.0/decorworld_database_model/tables/discount.py
--rw-r--r--   0        0        0      789 2022-11-17 17:38:48.011520 decorworld_database_model-0.5.0/decorworld_database_model/tables/favorite.py
--rw-r--r--   0        0        0      786 2022-11-17 17:41:18.193528 decorworld_database_model-0.5.0/decorworld_database_model/tables/image.py
--rw-r--r--   0        0        0     1285 2022-11-17 15:27:23.728985 decorworld_database_model-0.5.0/decorworld_database_model/tables/invoice_data.py
--rw-r--r--   0        0        0     4194 2023-03-29 07:55:31.124716 decorworld_database_model-0.5.0/decorworld_database_model/tables/order.py
--rw-r--r--   0        0        0     1184 2022-11-27 10:47:07.768493 decorworld_database_model-0.5.0/decorworld_database_model/tables/order_item.py
--rw-r--r--   0        0        0      647 2022-11-25 16:07:28.582459 decorworld_database_model-0.5.0/decorworld_database_model/tables/page_image.py
--rw-r--r--   0        0        0      726 2022-11-17 17:18:35.911436 decorworld_database_model-0.5.0/decorworld_database_model/tables/payment_method.py
--rw-r--r--   0        0        0     1316 2022-12-01 09:07:26.623964 decorworld_database_model-0.5.0/decorworld_database_model/tables/product.py
--rw-r--r--   0        0        0     1328 2023-03-29 07:53:54.242622 decorworld_database_model-0.5.0/decorworld_database_model/tables/review.py
--rw-r--r--   0        0        0      732 2022-11-17 17:11:19.312230 decorworld_database_model-0.5.0/decorworld_database_model/tables/shipping_method.py
--rw-r--r--   0        0        0     1507 2022-11-27 07:46:49.104190 decorworld_database_model-0.5.0/decorworld_database_model/tables/user.py
--rw-r--r--   0        0        0      405 2023-03-29 08:48:41.888096 decorworld_database_model-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      805 2023-03-29 08:48:46.792484 decorworld_database_model-0.5.0/setup.py
--rw-r--r--   0        0        0      479 2023-03-29 08:48:46.793478 decorworld_database_model-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-11-14 11:28:19.771512 decorworld_database_model-0.6.0/decorworld_database_model/__init__.py
+-rw-r--r--   0        0        0     2058 2022-11-14 11:36:26.543490 decorworld_database_model-0.6.0/decorworld_database_model/alembic/env.py
+-rw-r--r--   0        0        0       38 2022-11-14 11:28:32.706440 decorworld_database_model-0.6.0/decorworld_database_model/alembic/README
+-rw-r--r--   0        0        0      510 2022-11-14 11:28:32.707432 decorworld_database_model-0.6.0/decorworld_database_model/alembic/script.py.mako
+-rw-r--r--   0        0        0     1091 2022-11-17 17:32:55.256233 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py
+-rw-r--r--   0        0        0     1176 2023-04-27 06:22:16.258902 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/13a3b750c40e_add_pre_order_and_discount_columns_to_.py
+-rw-r--r--   0        0        0      833 2022-11-25 16:07:54.940915 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py
+-rw-r--r--   0        0        0     1313 2023-04-27 06:20:08.624820 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/21550951e198_drop_discounts_table.py
+-rw-r--r--   0        0        0      923 2022-11-14 11:36:28.443321 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py
+-rw-r--r--   0        0        0      971 2022-11-17 17:39:09.649589 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py
+-rw-r--r--   0        0        0     1093 2022-11-17 17:32:22.727240 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py
+-rw-r--r--   0        0        0      709 2022-11-27 07:47:32.279073 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py
+-rw-r--r--   0        0        0     1034 2022-11-25 13:12:14.766306 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py
+-rw-r--r--   0        0        0      741 2023-03-29 08:51:06.588874 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py
+-rw-r--r--   0        0        0     2041 2022-11-17 17:20:22.941546 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py
+-rw-r--r--   0        0        0      870 2022-11-17 17:19:16.180388 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py
+-rw-r--r--   0        0        0      943 2022-11-17 17:41:41.614167 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py
+-rw-r--r--   0        0        0      852 2022-11-19 09:43:34.355183 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py
+-rw-r--r--   0        0        0     1039 2022-11-17 09:29:10.463996 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py
+-rw-r--r--   0        0        0     1073 2022-11-17 17:37:07.585121 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py
+-rw-r--r--   0        0        0      746 2022-11-14 16:04:04.381269 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py
+-rw-r--r--   0        0        0     1241 2022-11-17 15:39:46.868782 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py
+-rw-r--r--   0        0        0      790 2022-11-17 17:31:37.522016 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py
+-rw-r--r--   0        0        0      948 2022-12-01 09:11:30.894051 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py
+-rw-r--r--   0        0        0      706 2022-11-17 18:49:14.442466 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py
+-rw-r--r--   0        0        0      866 2022-11-17 17:19:57.038988 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py
+-rw-r--r--   0        0        0     1103 2022-11-17 14:11:09.276179 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py
+-rw-r--r--   0        0        0      880 2022-11-19 09:34:42.463405 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py
+-rw-r--r--   0        0        0      877 2022-11-25 14:27:47.383698 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py
+-rw-r--r--   0        0        0      698 2022-11-17 15:39:42.615558 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py
+-rw-r--r--   0        0        0      835 2022-11-21 17:24:22.320177 decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py
+-rw-r--r--   0        0        0     3234 2022-11-14 11:34:58.943979 decorworld_database_model-0.6.0/decorworld_database_model/alembic.ini
+-rw-r--r--   0        0        0      449 2023-04-27 06:18:17.177337 decorworld_database_model-0.6.0/decorworld_database_model/tables/__init__.py
+-rw-r--r--   0        0        0     1143 2022-11-17 15:24:28.613902 decorworld_database_model-0.6.0/decorworld_database_model/tables/address.py
+-rw-r--r--   0        0        0      160 2022-11-14 11:30:54.004559 decorworld_database_model-0.6.0/decorworld_database_model/tables/base.py
+-rw-r--r--   0        0        0      628 2023-04-27 06:17:17.160232 decorworld_database_model-0.6.0/decorworld_database_model/tables/category.py
+-rw-r--r--   0        0        0      790 2023-04-27 06:17:17.107376 decorworld_database_model-0.6.0/decorworld_database_model/tables/favorite.py
+-rw-r--r--   0        0        0      784 2023-04-27 06:17:17.113356 decorworld_database_model-0.6.0/decorworld_database_model/tables/image.py
+-rw-r--r--   0        0        0     1290 2023-04-27 06:17:17.082439 decorworld_database_model-0.6.0/decorworld_database_model/tables/invoice_data.py
+-rw-r--r--   0        0        0     4192 2023-04-27 06:17:17.094407 decorworld_database_model-0.6.0/decorworld_database_model/tables/order.py
+-rw-r--r--   0        0        0     1184 2022-11-27 10:47:07.768493 decorworld_database_model-0.6.0/decorworld_database_model/tables/order_item.py
+-rw-r--r--   0        0        0      647 2022-11-25 16:07:28.582459 decorworld_database_model-0.6.0/decorworld_database_model/tables/page_image.py
+-rw-r--r--   0        0        0      733 2023-04-27 06:17:17.101389 decorworld_database_model-0.6.0/decorworld_database_model/tables/payment_method.py
+-rw-r--r--   0        0        0     1809 2023-04-27 06:19:48.880864 decorworld_database_model-0.6.0/decorworld_database_model/tables/product.py
+-rw-r--r--   0        0        0     1328 2023-03-29 08:51:06.589872 decorworld_database_model-0.6.0/decorworld_database_model/tables/review.py
+-rw-r--r--   0        0        0      740 2023-04-27 06:17:17.167212 decorworld_database_model-0.6.0/decorworld_database_model/tables/shipping_method.py
+-rw-r--r--   0        0        0     1507 2022-11-27 07:46:49.104190 decorworld_database_model-0.6.0/decorworld_database_model/tables/user.py
+-rw-r--r--   0        0        0      405 2023-04-27 06:25:32.847295 decorworld_database_model-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      805 2023-04-27 06:26:57.287834 decorworld_database_model-0.6.0/setup.py
+-rw-r--r--   0        0        0      479 2023-04-27 06:26:57.287834 decorworld_database_model-0.6.0/PKG-INFO
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/env.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/env.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-"""add date column to review
+"""create category table
 
-Revision ID: 4cfd3fc062af
-Revises: 8f89b8df2fba
-Create Date: 2023-03-29 09:57:25.402390
+Revision ID: 88d8f0924ac3
+Revises: 556ff2c83f9f
+Create Date: 2022-11-17 18:31:06.837908
 
 """
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
-revision = '4cfd3fc062af'
-down_revision = '8f89b8df2fba'
+revision = '88d8f0924ac3'
+down_revision = '556ff2c83f9f'
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.add_column('reviews', sa.Column('date', sa.DateTime(), server_default=sa.text('now()'), nullable=False))
+    op.create_table('categories',
+    sa.Column('id', sa.Integer(), autoincrement=True, nullable=False),
+    sa.Column('name', sa.String(25), nullable=False),
+    sa.PrimaryKeyConstraint('id')
+    )
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.drop_column('reviews', 'date')
+    op.drop_table('categories')
     # ### end Alembic commands ###
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""create category table
+"""modify review description to nullable
 
-Revision ID: 88d8f0924ac3
-Revises: 556ff2c83f9f
-Create Date: 2022-11-17 18:31:06.837908
+Revision ID: b2424975cff5
+Revises: 46fe20e7d2c8
+Create Date: 2022-11-25 15:27:47.383698
 
 """
 from alembic import op
 import sqlalchemy as sa
-
+from sqlalchemy.dialects import mysql
 
 # revision identifiers, used by Alembic.
-revision = '88d8f0924ac3'
-down_revision = '556ff2c83f9f'
+revision = 'b2424975cff5'
+down_revision = '46fe20e7d2c8'
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.create_table('categories',
-    sa.Column('id', sa.Integer(), autoincrement=True, nullable=False),
-    sa.Column('name', sa.String(25), nullable=False),
-    sa.PrimaryKeyConstraint('id')
-    )
+    op.alter_column('reviews', 'description',
+               existing_type=mysql.VARCHAR(length=100),
+               nullable=True)
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.drop_table('categories')
+    op.alter_column('reviews', 'description',
+               existing_type=mysql.VARCHAR(length=100),
+               nullable=False)
     # ### end Alembic commands ###
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-"""modify review description to nullable
-
-Revision ID: b2424975cff5
-Revises: 46fe20e7d2c8
-Create Date: 2022-11-25 15:27:47.383698
-
-"""
-from alembic import op
-import sqlalchemy as sa
-from sqlalchemy.dialects import mysql
-
-# revision identifiers, used by Alembic.
-revision = 'b2424975cff5'
-down_revision = '46fe20e7d2c8'
-branch_labels = None
-depends_on = None
-
-
-def upgrade() -> None:
-    # ### commands auto generated by Alembic - please adjust! ###
-    op.alter_column('reviews', 'description',
-               existing_type=mysql.VARCHAR(length=100),
-               nullable=True)
-    # ### end Alembic commands ###
-
-
-def downgrade() -> None:
-    # ### commands auto generated by Alembic - please adjust! ###
-    op.alter_column('reviews', 'description',
-               existing_type=mysql.VARCHAR(length=100),
-               nullable=False)
-    # ### end Alembic commands ###
+"""add date column to review
+
+Revision ID: 4cfd3fc062af
+Revises: 8f89b8df2fba
+Create Date: 2023-03-29 09:57:25.402390
+
+"""
+from alembic import op
+import sqlalchemy as sa
+
+
+# revision identifiers, used by Alembic.
+revision = '4cfd3fc062af'
+down_revision = '8f89b8df2fba'
+branch_labels = None
+depends_on = None
+
+
+def upgrade() -> None:
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.add_column('reviews', sa.Column('date', sa.DateTime(), server_default=sa.text('now()'), nullable=False))
+    # ### end Alembic commands ###
+
+
+def downgrade() -> None:
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.drop_column('reviews', 'date')
+    # ### end Alembic commands ###
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/alembic.ini` & `decorworld_database_model-0.6.0/decorworld_database_model/alembic.ini`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/address.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/address.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/category.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/category.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 
     model_class = Category
 
     id = fields.Integer()
     name = fields.String()
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_category(self, data, **kwargs):
         return Category(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/discount.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/review.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from sqlalchemy import Column
 from sqlalchemy import Integer
 from sqlalchemy import ForeignKey
+from sqlalchemy import String
 from sqlalchemy import DateTime
-from sqlalchemy import func
+from sqlalchemy.sql import func
+from sqlalchemy.orm import relationship
 from marshmallow import fields
 from marshmallow import Schema
 from marshmallow import post_load
-
+from .product import ProductSchema
 from .base import Base
 
 
-class Discount(Base):
-    __tablename__ = 'discounts'
+class Review(Base):
+    __tablename__ = 'reviews'
 
     id = Column(Integer, primary_key=True, autoincrement=True, nullable=False)
+    date = Column(DateTime, nullable=False, server_default=func.now())
     product_id = Column(ForeignKey('products.id'), nullable=False)
-    percent = Column(Integer, nullable=False)
-    created_date = Column(DateTime, nullable=False, server_default=func.now())
-    expiration_date = Column(DateTime, nullable=False)
+    name = Column(String(30), nullable=False)
+    rating = Column(Integer, nullable=False)
+    description = Column(String(100), nullable=True)
+
+    product = relationship('Product', primaryjoin='Product.id == Review.product_id')
 
 
-class DiscountSchema(Schema):
+class ReviewSchema(Schema):
 
-    model_class = Discount
+    model_class = Review
 
     id = fields.Integer()
-    product_id = fields.Integer(data_key='productID')
-    percent = fields.Integer()
-    created_date = fields.DateTime(data_key='createdDate')
-    expiration_date = fields.DateTime(data_key='expirationDate')
+    date = fields.DateTime()
+    product_id = fields.Integer(data_key='productId')
+    name = fields.String()
+    rating = fields.Integer()
+    description = fields.String()
+
+    product = fields.Nested(ProductSchema, many=False)
 
     @post_load
-    def make_address(self, data, **kwargs):
-        return Discount(**data)
+    def make_review(self, data, **kwargs):
+        return Review(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/favorite.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/favorite.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     model_class = Favorite
 
     id = fields.Integer()
     user_id = fields.Integer(data_key='userID')
     product_id = fields.Integer(data_key='productID')
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_favorite(self, data, **kwargs):
         return Favorite(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/image.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     model_class = Image
 
     id = fields.Integer()
     product_id = fields.Integer(data_key='productID')
     image = fields.String()
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_image(self, data, **kwargs):
         return Image(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/invoice_data.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/invoice_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     zip_code = fields.String(data_key='zipCode')
     city = fields.String()
     address = fields.String()
     tax_number = fields.String(allow_none=True, data_key='taxNumber')
     description = fields.String(allow_none=True)
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_invoice_data(self, data, **kwargs):
         return InvoiceData(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/order.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,9 +83,9 @@
     payment_method = fields.Integer(data_key='paymentMethod')
 
     order_items = fields.Nested(OrderItemSchema, many=True, data_key='orderItems')
     shipping = fields.Nested(ShippingMethodSchema, many=False)
     payment = fields.Nested(PaymentMethodSchema, many=False)
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_order(self, data, **kwargs):
         return Order(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/order_item.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/order_item.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/page_image.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/page_image.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/payment_method.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/payment_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     model_class = PaymentMethod
 
     id = fields.Integer()
     name = fields.String()
     price = fields.Integer()
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_payment_method(self, data, **kwargs):
         return PaymentMethod(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/product.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/product.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from sqlalchemy import Column
 from sqlalchemy import Integer
 from sqlalchemy import ForeignKey
 from sqlalchemy import String
 from sqlalchemy import Text
+from sqlalchemy import Boolean
+from sqlalchemy import text
+from sqlalchemy.dialects.mysql import DOUBLE
 from sqlalchemy.orm import relationship
 from marshmallow import fields
 from marshmallow import Schema
 from marshmallow import post_load
 from .image import ImageSchema
 
 from .base import Base
@@ -18,14 +21,17 @@
     id = Column(Integer, primary_key=True, autoincrement=True, nullable=False)
     category_id = Column(ForeignKey('categories.id'), nullable=False)
     name = Column(String(50), nullable=False)
     number = Column(String(25), nullable=False)
     price = Column(Integer, nullable=False)
     quantity = Column(Integer, nullable=False)
     description = Column(Text, nullable=False)
+    available_for_pre_order = Column(Boolean, nullable=False, server_default=text('false'))
+    active_discount = Column(Boolean, nullable=False, server_default=text('false'))
+    discount_percent = Column(DOUBLE, nullable=False, server_default=text('0'))
 
     image = relationship('Image', foreign_keys='Image.product_id')
 
 
 class ProductSchema(Schema):
 
     model_class = Product
@@ -33,13 +39,16 @@
     id = fields.Integer()
     category_id = fields.Integer(data_key='categoryID')
     name = fields.String()
     number = fields.String()
     price = fields.Integer()
     quantity = fields.Integer()
     description = fields.String()
+    available_for_pre_order = fields.Boolean()
+    active_discount = fields.Boolean()
+    discount_percent = fields.Float()
 
     image = fields.Nested(ImageSchema)
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_product(self, data, **kwargs):
         return Product(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/shipping_method.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/shipping_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     model_class = ShippingMethod
 
     id = fields.Integer()
     name = fields.String()
     price = fields.Integer()
 
     @post_load
-    def make_address(self, data, **kwargs):
+    def make_shipping_method(self, data, **kwargs):
         return ShippingMethod(**data)
```

### Comparing `decorworld_database_model-0.5.0/decorworld_database_model/tables/user.py` & `decorworld_database_model-0.6.0/decorworld_database_model/tables/user.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.5.0/setup.py` & `decorworld_database_model-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['marshmallow==3.14.1', 'sqlalchemy==1.3.18']
 
 setup_kwargs = {
     'name': 'decorworld-database-model',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Database models for DecorWorld',
     'long_description': None,
     'author': 'Pintér Tamás',
     'author_email': 'tamas.pinter@pannonszoftver.hu',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

