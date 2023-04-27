# Comparing `tmp/rdmo-1.9.1.tar.gz` & `tmp/rdmo-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdmo-1.9.1.tar", last modified: Fri Feb  3 14:47:56 2023, max compression
+gzip compressed data, was "rdmo-1.9.2.tar", last modified: Thu Feb 23 20:57:37 2023, max compression
```

## Comparing `rdmo-1.9.1.tar` & `rdmo-1.9.2.tar`

### file list

```diff
@@ -1,1147 +1,1148 @@
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.475967 rdmo-1.9.1/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1701 2023-01-12 09:58:52.000000 rdmo-1.9.1/AUTHORS
--rw-rw-r--   0 ole       (1000) ole       (1000)    11359 2022-08-03 07:29:05.000000 rdmo-1.9.1/LICENSE
--rw-rw-r--   0 ole       (1000) ole       (1000)      102 2022-08-03 07:29:05.000000 rdmo-1.9.1/MANIFEST.in
--rw-rw-r--   0 ole       (1000) ole       (1000)     7844 2022-08-03 07:29:05.000000 rdmo-1.9.1/NOTICE
--rw-rw-r--   0 ole       (1000) ole       (1000)     2895 2023-02-03 14:47:56.475967 rdmo-1.9.1/PKG-INFO
--rw-rw-r--   0 ole       (1000) ole       (1000)     2011 2023-01-12 09:58:52.000000 rdmo-1.9.1/README.md
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.223972 rdmo-1.9.1/rdmo/
--rw-rw-r--   0 ole       (1000) ole       (1000)      171 2023-02-03 12:11:27.000000 rdmo-1.9.1/rdmo/__init__.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.223972 rdmo-1.9.1/rdmo/accounts/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      452 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/adapter.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      788 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      234 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3906 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/forms.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.231972 rdmo-1.9.1/rdmo/accounts/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1569 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0001_initial.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      579 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0002_detail_key_type_field_length_increased.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      687 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0003_hint_renamed_to_help_text.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      923 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0004_permission_added.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      563 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0005_field_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      426 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0006_permissions_removed.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2664 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0007_additional_fields.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      620 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0008_related_name.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      851 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0009_proxyuser.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1133 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0010_consentfieldvalue.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      595 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0011_rename_en_to_lang1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      596 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0012_rename_de_to_lang2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1692 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0013_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2661 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0014_add_language_fields.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      983 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0015_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3175 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0016_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1263 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0017_role.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      770 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0018_blank_fields.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      294 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/0019_delete_proxyuser.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5265 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      405 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/rules.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.231972 rdmo-1.9.1/rdmo/accounts/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1651 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/accounts/serializers/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5947 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/settings.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.211972 rdmo-1.9.1/rdmo/accounts/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.211972 rdmo-1.9.1/rdmo/accounts/static/accounts/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.231972 rdmo-1.9.1/rdmo/accounts/static/accounts/img/
--rw-rw-r--   0 ole       (1000) ole       (1000)    32038 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/static/accounts/img/keycloak_logo_200px.svg
--rw-rw-r--   0 ole       (1000) ole       (1000)    23495 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/static/accounts/img/orcid-signin.png
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/accounts/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.239971 rdmo-1.9.1/rdmo/accounts/templates/account/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.239971 rdmo-1.9.1/rdmo/accounts/templates/account/email/
--rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/email/password_reset_key_message.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)       43 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/email/password_reset_key_subject.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)     2784 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/email.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1019 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/email_confirm.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      159 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/login.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      828 2023-01-26 18:01:51.000000 rdmo-1.9.1/rdmo/accounts/templates/account/login_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      422 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/login_form_account.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      525 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/login_form_socialaccount.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      535 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/logout.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      238 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/logout_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      540 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/password_change.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      650 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/password_reset.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      633 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/password_reset_done.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      857 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/password_reset_from_key.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      341 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/password_reset_from_key_done.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      501 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/password_set.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1794 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/signup.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      215 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/signup_closed.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1934 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/signup_modal_terms_of_use.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      343 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/terms_of_use.html
--rw-rw-r--   0 ole       (1000) ole       (1000)       16 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/terms_of_use_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)       16 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/terms_of_use_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      381 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/verification_sent.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      776 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/account/verified_email_required.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.239971 rdmo-1.9.1/rdmo/accounts/templates/profile/
--rw-rw-r--   0 ole       (1000) ole       (1000)      219 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/profile/profile_remove_closed.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      238 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/profile/profile_remove_failed.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      747 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/profile/profile_remove_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      203 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/profile/profile_remove_success.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      219 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/profile/profile_update_closed.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1373 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/accounts/templates/profile/profile_update_form.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.243971 rdmo-1.9.1/rdmo/accounts/templates/socialaccount/
--rw-rw-r--   0 ole       (1000) ole       (1000)      303 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/socialaccount/authentication_error.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1879 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/socialaccount/connections.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      435 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/socialaccount/login_cancelled.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1929 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/socialaccount/signup.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.243971 rdmo-1.9.1/rdmo/accounts/templates/socialaccount/snippets/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1511 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templates/socialaccount/snippets/provider_list.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.243971 rdmo-1.9.1/rdmo/accounts/templatetags/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templatetags/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      728 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/templatetags/accounts_tags.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.243971 rdmo-1.9.1/rdmo/accounts/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     9595 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3174 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/tests/test_viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.243971 rdmo-1.9.1/rdmo/accounts/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1094 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      280 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1974 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/utils.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2505 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/accounts/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1331 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/accounts/viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.247971 rdmo-1.9.1/rdmo/conditions/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      793 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      190 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1253 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/imports.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.251971 rdmo-1.9.1/rdmo/conditions/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1748 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0001_initial.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      500 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0002_many_to_many_for_conditions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      705 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0003_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      486 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0004_condition_title.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      746 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0005_empty_relation.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      877 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0006_db_constraint_false.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      482 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0007_ordering.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      599 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0008_validator.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      600 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0009_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      793 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0010_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3110 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0011_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      532 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0012_permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2425 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0013_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1421 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0014_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      679 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0015_move_attribute_to_attributeentity.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1510 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0016_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      828 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0017_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1632 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0018_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      416 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0019_django2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      775 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0020_require_uri_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1054 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0021_related_name.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      474 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/0022_condition_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     7840 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1176 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/renderers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.251971 rdmo-1.9.1/rdmo/conditions/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      582 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/serializers/export.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2827 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/serializers/v1.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/conditions/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/conditions/static/conditions/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.251971 rdmo-1.9.1/rdmo/conditions/static/conditions/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/static/conditions/css/conditions.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.251971 rdmo-1.9.1/rdmo/conditions/static/conditions/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)     4754 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/static/conditions/js/conditions.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/conditions/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.255971 rdmo-1.9.1/rdmo/conditions/templates/conditions/
--rw-rw-r--   0 ole       (1000) ole       (1000)     5224 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      780 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2111 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_modal_delete_conditions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     7769 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_modal_form_conditions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2706 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_modal_show_conditions.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.255971 rdmo-1.9.1/rdmo/conditions/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      268 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/test_admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      763 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/test_models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2634 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/test_validator_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2527 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/test_validator_unique_uri.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1494 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6498 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/test_viewset_condition.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      663 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/tests/test_viewset_relation.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.255971 rdmo-1.9.1/rdmo/conditions/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      278 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      388 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1619 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2141 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/conditions/viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.259971 rdmo-1.9.1/rdmo/core/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1955 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/core/constants.py
--rw-rw-r--   0 ole       (1000) ole       (1000)       41 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/exceptions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      475 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/exports.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4807 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/imports.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      528 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/mail.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.259971 rdmo-1.9.1/rdmo/core/management/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/__init__.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.263971 rdmo-1.9.1/rdmo/core/management/commands/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      259 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/create_admin_user.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2174 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/delete_users.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      483 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/deploy.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2139 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/download_vendor_files.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1163 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/core/management/commands/find_inactive_users.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5275 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/find_spam_users.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3817 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/find_users.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2830 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/make_theme.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      468 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/poedit.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1815 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/set_uri_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      544 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/setup_groups.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      733 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/management/commands/upgrade.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1157 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/managers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1312 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3914 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      778 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/plugins.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1088 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/renderers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2184 2023-01-12 12:00:20.000000 rdmo-1.9.1/rdmo/core/serializers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    12536 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/core/settings.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/core/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/core/static/core/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.263971 rdmo-1.9.1/rdmo/core/static/core/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)     7899 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/base.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)      151 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/codemirror.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)      982 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/fonts.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)     1011 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/footer.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)     1837 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/header.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/style.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)      532 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/swagger.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)      878 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/css/variables.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.267971 rdmo-1.9.1/rdmo/core/static/core/fonts/
--rwxrwxr-x   0 ole       (1000) ole       (1000)    42480 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSans-Bold.ttf
--rwxrwxr-x   0 ole       (1000) ole       (1000)    41028 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSans.ttf
--rwxrwxr-x   0 ole       (1000) ole       (1000)   117072 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSansMono.ttf
--rwxrwxr-x   0 ole       (1000) ole       (1000)    48880 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif-Bold.ttf
--rwxrwxr-x   0 ole       (1000) ole       (1000)    45652 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif-BoldItalic.ttf
--rwxrwxr-x   0 ole       (1000) ole       (1000)    40416 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif-Italic.ttf
--rwxrwxr-x   0 ole       (1000) ole       (1000)    43648 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif.ttf
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.271971 rdmo-1.9.1/rdmo/core/static/core/html/
--rw-rw-r--   0 ole       (1000) ole       (1000)      471 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_checkbox.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      428 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_codemirror.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      442 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_number.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      811 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_select.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      591 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_selectmultiple.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      633 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_selectnumber.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      454 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_text.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      413 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/html/formgroup_textarea.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.271971 rdmo-1.9.1/rdmo/core/static/core/img/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1129 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/img/favicon.png
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.275971 rdmo-1.9.1/rdmo/core/static/core/img/header/
--rw-rw-r--   0 ole       (1000) ole       (1000)   155589 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/img/header/collection.jpg
--rw-rw-r--   0 ole       (1000) ole       (1000)   183545 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/img/header/library.jpg
--rw-rw-r--   0 ole       (1000) ole       (1000)    87777 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/img/header/supercomputer.jpg
--rw-rw-r--   0 ole       (1000) ole       (1000)     9109 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/img/rdmo-logo.svg
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.275971 rdmo-1.9.1/rdmo/core/static/core/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)     6934 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/js/core.js
--rw-rw-r--   0 ole       (1000) ole       (1000)      448 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/static/core/js/header.js
--rw-rw-r--   0 ole       (1000) ole       (1000)      655 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/swagger.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/core/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.283971 rdmo-1.9.1/rdmo/core/templates/core/
--rw-rw-r--   0 ole       (1000) ole       (1000)      207 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/400.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      196 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/403.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      193 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/404.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      211 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/500.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      377 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/about.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1502 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/about_text_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1363 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/about_text_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1522 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/about_text_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1341 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/about_text_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      107 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/back_to_project_link.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      599 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/base.html
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/base_analytics.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      139 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/base_footer.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1147 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/core/templates/core/base_head.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     6836 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/base_navigation.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      219 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/base_navigation_account.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      130 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/base_navigation_socialaccount.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      316 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/bootstrap_delete_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      397 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/bootstrap_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1561 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/bootstrap_form_field.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      327 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/bootstrap_form_fields.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      178 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/error.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      131 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      707 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/footer_text_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      703 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/footer_text_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      718 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/footer_text_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/footer_text_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2235 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/home.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      621 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/home_text_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      537 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/home_text_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      612 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/home_text_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/home_text_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      327 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/page.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1198 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/core/upload_form.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.283971 rdmo-1.9.1/rdmo/core/templates/rest_framework_swagger/
--rw-rw-r--   0 ole       (1000) ole       (1000)     2453 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templates/rest_framework_swagger/index.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.283971 rdmo-1.9.1/rdmo/core/templatetags/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templatetags/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5448 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/templatetags/core_tags.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.283971 rdmo-1.9.1/rdmo/core/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2649 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_mail.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      411 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_swagger.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      842 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_tags.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      569 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_utils.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1552 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1535 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      725 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_viewset_settings.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2992 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/tests/test_xml.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.287970 rdmo-1.9.1/rdmo/core/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      768 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      132 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/urls/swagger.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      919 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    11580 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/utils.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2696 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4209 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2927 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/core/viewsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2819 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/core/xml.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.287970 rdmo-1.9.1/rdmo/domain/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1303 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      178 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1432 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/imports.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.299970 rdmo-1.9.1/rdmo/domain/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     5213 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0001_initial_after_reset.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      415 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0002_additional_input.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      637 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0003_condition.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1078 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0004_verbosename.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      456 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0005_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      585 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0006_attributeentity_parent_collection.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      491 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0007_db_index.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      605 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0008_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0009_remove_condition.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      534 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0010_many_to_many_for_conditions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      499 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0011_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      426 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0012_renaming.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1972 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0013_mptt.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      449 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0014_is_attribute.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      640 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0015_label.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      268 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0016_label.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      602 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0017_url_value_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      607 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0018_validator.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      519 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0019_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      676 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0020_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      465 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0021_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      495 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0022_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      460 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0023_fix_label.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      519 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0024_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      776 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0025_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6809 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0026_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      489 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0027_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      416 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0028_path.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      558 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0029_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1257 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0030_permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1187 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0031_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      580 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0032_remove_unit_and_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      448 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0033_remove_attribute_optionsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0034_remove_attributeentity_conditions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      592 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0035_remove_is_collection_and_parent_collection.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      726 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0036_remove_range_and_verbosename.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1035 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0037_remove_attribute.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      424 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0038_rename_attributeentity_to_attribute.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2390 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0039_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      561 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0040_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      813 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0041_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1292 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0042_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      816 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0043_django2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      719 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0044_mptt.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      764 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0045_require_uri_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      628 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0046_parent_cascade.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      496 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0047_attribute_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      498 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/0048_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3207 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1137 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/renderers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.299970 rdmo-1.9.1/rdmo/domain/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      422 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/serializers/export.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3377 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/serializers/v1.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/domain/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/domain/static/domain/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.299970 rdmo-1.9.1/rdmo/domain/static/domain/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)       45 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/static/domain/css/domain.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.299970 rdmo-1.9.1/rdmo/domain/static/domain/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)     4331 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/static/domain/js/domain.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/domain/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.303970 rdmo-1.9.1/rdmo/domain/templates/domain/
--rw-rw-r--   0 ole       (1000) ole       (1000)     3904 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/templates/domain/domain.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      309 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/templates/domain/domain_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3568 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/templates/domain/domain_modal_delete_attributes.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     6031 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/templates/domain/domain_modal_form_attributes.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3490 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/templates/domain/domain_modal_show_attributes.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      943 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/templates/domain/domain_options.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.303970 rdmo-1.9.1/rdmo/domain/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      264 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/test_admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      791 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/test_models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6543 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/test_validator_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3636 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/test_validator_parent.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3134 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/test_validator_unique_uri.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1481 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6265 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/tests/test_viewset_attribute.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.303970 rdmo-1.9.1/rdmo/domain/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      253 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      299 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1742 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2070 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2385 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/domain/viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/locale/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/locale/de/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.307970 rdmo-1.9.1/rdmo/locale/de/LC_MESSAGES/
--rw-rw-r--   0 ole       (1000) ole       (1000)   100199 2023-02-03 12:13:41.000000 rdmo-1.9.1/rdmo/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 ole       (1000) ole       (1000)   191976 2023-02-03 12:59:55.000000 rdmo-1.9.1/rdmo/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/locale/es/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.307970 rdmo-1.9.1/rdmo/locale/es/LC_MESSAGES/
--rw-rw-r--   0 ole       (1000) ole       (1000)   100400 2023-02-03 12:13:41.000000 rdmo-1.9.1/rdmo/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 ole       (1000) ole       (1000)   182130 2023-02-03 12:59:42.000000 rdmo-1.9.1/rdmo/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/locale/fr/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.307970 rdmo-1.9.1/rdmo/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 ole       (1000) ole       (1000)   102473 2023-02-03 12:13:41.000000 rdmo-1.9.1/rdmo/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 ole       (1000) ole       (1000)   194518 2023-02-03 12:59:56.000000 rdmo-1.9.1/rdmo/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/locale/it/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.311970 rdmo-1.9.1/rdmo/locale/it/LC_MESSAGES/
--rw-rw-r--   0 ole       (1000) ole       (1000)    98657 2023-02-03 12:13:41.000000 rdmo-1.9.1/rdmo/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 ole       (1000) ole       (1000)   181203 2023-02-03 12:59:58.000000 rdmo-1.9.1/rdmo/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/locale/nl/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.311970 rdmo-1.9.1/rdmo/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 ole       (1000) ole       (1000)      380 2023-02-03 12:13:41.000000 rdmo-1.9.1/rdmo/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 ole       (1000) ole       (1000)   138451 2023-02-03 12:59:59.000000 rdmo-1.9.1/rdmo/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.311970 rdmo-1.9.1/rdmo/management/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      190 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4727 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/imports.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/management/management/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.311970 rdmo-1.9.1/rdmo/management/management/commands/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/management/commands/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      978 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/management/commands/import.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/management/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.315970 rdmo-1.9.1/rdmo/management/templates/management/
--rw-rw-r--   0 ole       (1000) ole       (1000)     3284 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/templates/management/import.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     4640 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/templates/management/upload.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.315970 rdmo-1.9.1/rdmo/management/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1322 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/tests/test_commands.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2167 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/tests/test_import.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6868 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/tests/test_views.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.315970 rdmo-1.9.1/rdmo/management/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/management/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5042 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/management/views.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.315970 rdmo-1.9.1/rdmo/options/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1442 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      181 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2405 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/imports.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.327970 rdmo-1.9.1/rdmo/options/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     2192 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0001_initial.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      880 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0002_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1683 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0003_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      519 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0004_conditions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      739 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0005_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4475 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0006_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      651 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0007_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      530 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0008_option_path.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      554 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0009_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      760 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0010_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      780 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0011_permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0012_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      557 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0013_order.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      421 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0014_rename_en_to_lang1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      434 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0015_rename_de_to_lang2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      807 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0016_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1666 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0017_add_language_fields.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1112 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0018_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3878 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0019_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1020 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0020_django2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      532 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0021_data_migrations.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      575 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0022_cascade_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1187 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0023_require_uri_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      545 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0024_related_name.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      531 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0025_optionset_provider_key.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      738 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0026_optionset_option_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      503 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/0027_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     7085 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      592 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/providers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2574 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/renderers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.327970 rdmo-1.9.1/rdmo/options/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1157 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/serializers/export.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4757 2023-01-16 11:16:32.000000 rdmo-1.9.1/rdmo/options/serializers/v1.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/options/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/options/static/options/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.327970 rdmo-1.9.1/rdmo/options/static/options/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/static/options/css/options.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.327970 rdmo-1.9.1/rdmo/options/static/options/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)     6187 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/static/options/js/options.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/options/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.331970 rdmo-1.9.1/rdmo/options/templates/options/
--rw-rw-r--   0 ole       (1000) ole       (1000)     8603 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1516 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2205 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_modal_delete_options.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2729 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_modal_delete_optionsets.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1666 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_modal_form_conditions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)    10359 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_modal_form_options.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     6471 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_modal_form_optionsets.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1733 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_modal_show_options.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1401 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/templates/options/options_modal_show_optionsets.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.331970 rdmo-1.9.1/rdmo/options/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      492 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1420 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3729 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_validator_locked_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2634 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_validator_locked_optionsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2872 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_validator_unique_uri_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2527 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_validator_unique_uri_optionsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1480 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6380 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_viewset_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6655 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/tests/test_viewset_optionsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.331970 rdmo-1.9.1/rdmo/options/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      260 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1174 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1643 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3976 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/options/viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.335970 rdmo-1.9.1/rdmo/overlays/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      310 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      183 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/apps.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.335970 rdmo-1.9.1/rdmo/overlays/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1455 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/migrations/0001_initial.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1107 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/models.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.215972 rdmo-1.9.1/rdmo/overlays/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/overlays/static/overlays/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.335970 rdmo-1.9.1/rdmo/overlays/static/overlays/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)      444 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/static/overlays/css/overlays.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.335970 rdmo-1.9.1/rdmo/overlays/static/overlays/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)     2593 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/overlays/static/overlays/js/overlays.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/overlays/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.335970 rdmo-1.9.1/rdmo/overlays/templates/overlays/
--rw-rw-r--   0 ole       (1000) ole       (1000)      286 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/templates/overlays/buttons.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      589 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/templates/overlays/reset_overlays.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.335970 rdmo-1.9.1/rdmo/overlays/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1020 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2030 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/tests/test_viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.335970 rdmo-1.9.1/rdmo/overlays/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      142 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      292 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      561 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/overlays/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2680 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/overlays/viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.339969 rdmo-1.9.1/rdmo/projects/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3494 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      345 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      291 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/constants.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5177 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/exports.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1211 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/filters.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    12820 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/forms.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2234 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/handlers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    12552 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/imports.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.339969 rdmo-1.9.1/rdmo/projects/management/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/management/__init__.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.339969 rdmo-1.9.1/rdmo/projects/management/commands/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/management/commands/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1169 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/management/commands/delete_projects.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4889 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/management/commands/export_projects.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1600 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/management/commands/find_inactive_projects.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1775 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/management/commands/prune_projects.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5444 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/managers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.355969 rdmo-1.9.1/rdmo/projects/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     3680 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0001_initial_after_reset.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1065 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0002_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      488 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0003_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      589 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0004_remove_current_snapshot.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      736 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0005_snapshot.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      813 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0006_project_values.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      676 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0007_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0008_not_null.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      623 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0009_options.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      564 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0010_add_db_contraint.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4186 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0011_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2158 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0012_membership.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      670 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0013_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      387 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0014_remove_owner.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1257 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0015_permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      651 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0016_catalog_on_delete.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      995 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0017_value_unit_and_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      770 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0018_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      678 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0019_option.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      584 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0020_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0021_order.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      658 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0022_move_attribute_to_attributeentity.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0023_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      734 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0024_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      511 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0025_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1392 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0026_django2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      968 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0027_project_site.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      553 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0028_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      328 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0029_remove_manager.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      523 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0030_project_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      523 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0031_project_tasks.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1001 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0032_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      622 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0033_default_value_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1319 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0034_issue.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      650 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0035_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      326 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0036_remove_project_tasks.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0037_project_tasks.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1962 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0038_integration_integrationoption.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      520 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0039_integrationoption_secret.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1258 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0040_issueresource.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      467 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0041_value_external_id.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      571 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0042_allow_site_null.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      598 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0043_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      575 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0044_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1297 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0045_value_file.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2061 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0046_project_mptt.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1631 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0047_continuation.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1210 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0048_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1749 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0049_invite.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1096 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0050_value_set_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      682 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0051_alter_value_value_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      923 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/0052_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    10505 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/mixins.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.355969 rdmo-1.9.1/rdmo/projects/models/
--rw-rw-r--   0 ole       (1000) ole       (1000)      282 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1078 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/continuation.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2708 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/integration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2269 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/invite.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3918 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/issue.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/membership.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5517 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/project.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2489 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/snapshot.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     7893 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/models/value.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8651 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/providers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3374 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/renderers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4198 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/rules.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.359969 rdmo-1.9.1/rdmo/projects/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2339 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/serializers/export.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.359969 rdmo-1.9.1/rdmo/projects/serializers/v1/
--rw-rw-r--   0 ole       (1000) ole       (1000)     6574 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/serializers/v1/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1605 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/serializers/v1/overview.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3817 2023-02-03 11:15:14.000000 rdmo-1.9.1/rdmo/projects/serializers/v1/questionset.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/projects/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/projects/static/projects/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.359969 rdmo-1.9.1/rdmo/projects/static/projects/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)      303 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/static/projects/css/project.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)     5912 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/static/projects/css/project_questions.scss
--rw-rw-r--   0 ole       (1000) ole       (1000)      370 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/static/projects/css/projects.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/projects/static/projects/js/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.359969 rdmo-1.9.1/rdmo/projects/static/projects/js/project_questions/
--rw-rw-r--   0 ole       (1000) ole       (1000)      187 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/static/projects/js/project_questions/app.js
--rw-rw-r--   0 ole       (1000) ole       (1000)      448 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/static/projects/js/project_questions/controllers.js
--rw-rw-r--   0 ole       (1000) ole       (1000)     3376 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/static/projects/js/project_questions/directives.js
--rw-rw-r--   0 ole       (1000) ole       (1000)    61227 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/static/projects/js/project_questions/services.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/projects/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.379969 rdmo-1.9.1/rdmo/projects/templates/projects/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.379969 rdmo-1.9.1/rdmo/projects/templates/projects/email/
--rw-rw-r--   0 ole       (1000) ole       (1000)      793 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/email/project_invite_message.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      215 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/email/project_invite_subject.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      467 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/integration_confirm_delete.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      473 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/integration_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      854 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/invite_confirm_delete.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1967 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_detail.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      184 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1828 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_send.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1004 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_send_email.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1322 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_send_integrations.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      472 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_send_message.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      487 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_send_sidebar.html
--rw-rw-r--   0 ole       (1000) ole       (1000)       38 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/issue_send_subject.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      510 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/membership_confirm_delete.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1109 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/membership_form.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.395968 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/
--rw-rw-r--   0 ole       (1000) ole       (1000)      256 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      236 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      237 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      413 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_message_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_message_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      378 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_message_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      348 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_issue_message_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      271 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_support_info_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      272 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_support_info_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      299 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_support_info_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      268 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/issue_send_support_info_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      318 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_export_project_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      272 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_export_project_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      298 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_export_project_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      276 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_export_project_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      332 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_import_project_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      285 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_import_project_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      298 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_import_project_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      274 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_import_project_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      243 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_catalog_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      245 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_catalog_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      255 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_catalog_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      241 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_catalog_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      688 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      613 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      708 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      627 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      402 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_memberships_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      337 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_memberships_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      390 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_memberships_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      351 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_memberships_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      528 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_questions_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      458 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_questions_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      540 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_questions_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      504 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_questions_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      443 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_snapshots_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      390 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_snapshots_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_snapshots_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      439 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_snapshots_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      679 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      592 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      681 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      627 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      271 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_support_info_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      272 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_support_info_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      299 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_support_info_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      268 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_support_info_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_create_project_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      233 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_create_project_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      260 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_create_project_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      240 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_create_project_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      384 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_import_project_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      331 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_import_project_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      351 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_import_project_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_import_project_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      534 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      514 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      566 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      526 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      271 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_support_info_de.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      272 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_support_info_en.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      299 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_support_info_fr.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      268 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_support_info_it.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2338 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_answers.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2029 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_answers_element.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      245 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_answers_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      458 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_answers_tree.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      399 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_confirm_cancel.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      829 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_confirm_delete.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      465 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_confirm_leave.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1927 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1336 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_header.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      346 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_header_catalog.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      363 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_header_description.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      623 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_header_hierarchy.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2440 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_integrations.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      252 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_integrations_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1432 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_invites.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3320 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_issues.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      290 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_issues_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3011 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_memberships.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      358 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_memberships_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     5089 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_sidebar.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      609 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_sidebar_parent_import.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2883 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_snapshots.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      350 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_snapshots_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2007 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_views.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      360 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_views_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      533 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_error.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1029 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     7959 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_import.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      414 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_import_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3318 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      369 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_add_field_button.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      326 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_add_field_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      396 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_add_set_button.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      328 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_add_set_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1868 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_buttons.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      235 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_default.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_done.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1422 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_element.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      320 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_erase_field.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      446 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_error.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2921 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_autocomplete.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1675 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_checkbox.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1559 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_date.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2006 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_file.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2675 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_radio.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1946 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_range.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1784 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_select.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1436 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_text.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1468 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_textarea.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2409 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_yesno.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      405 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_head.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2354 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_modal_delete_valuesets.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1603 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_modal_form_valuesets.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      942 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_navigation.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      480 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_navigation_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      389 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_overview.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      442 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_progress.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      107 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_question_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      194 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_question_label.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_question_warning.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2362 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_questionset_head.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      505 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_questionset_head_help.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      513 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_remove_field.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      428 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_remove_set.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      367 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_sidebar.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2352 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_view.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      104 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/project_view_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     5445 2023-02-03 12:06:55.000000 rdmo-1.9.1/rdmo/projects/templates/projects/projects.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      946 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/projects_pagination.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2281 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/site_projects.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      344 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/snapshot_form.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      496 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templates/projects/snapshot_rollback.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.395968 rdmo-1.9.1/rdmo/projects/templatetags/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templatetags/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2509 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/templatetags/projects_tags.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.399968 rdmo-1.9.1/rdmo/projects/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2231 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_commands.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2702 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/tests/test_handlers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1425 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8336 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_integration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8066 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_issue.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    10163 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_membership.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    22282 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_project.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    10210 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_project_create_import.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4160 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_project_join.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5152 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_project_leave.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    18078 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_project_update_import.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     7808 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_view_snapshot.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3582 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_integration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3421 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_issue.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3559 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_membership.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8503 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_project.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8327 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_integration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4764 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_issue.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5167 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_membership.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1246 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_questionset.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6633 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_snapshot.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    11770 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_value.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3346 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_snapshot.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5302 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/tests/test_viewset_value.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.403968 rdmo-1.9.1/rdmo/projects/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)     6163 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1901 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4633 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/utils.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      789 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/validators.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.403968 rdmo-1.9.1/rdmo/projects/views/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1243 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3103 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/integration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      614 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/invite.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     7611 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/issue.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4298 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/membership.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    10352 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/projects/views/project.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4201 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/project_answers.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3034 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/project_create.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4954 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/project_update.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3527 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/project_view.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2139 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/views/snapshot.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    17721 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/viewsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1341 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/projects/widgets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.407968 rdmo-1.9.1/rdmo/questions/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3632 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      187 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      408 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/constants.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      135 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/forms.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6924 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/imports.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2180 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/managers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.423968 rdmo-1.9.1/rdmo/questions/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     5793 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0001_initial_after_reset.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      712 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0002_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      422 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0003_renaming.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1129 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0004_full_title.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1309 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0005_label.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1162 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0006_auto_20160803_1619.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    11515 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0007_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1174 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0008_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1904 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0009_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1766 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0010_label.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      694 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0011_path.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1118 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0012_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1665 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0013_permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3138 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0014_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1005 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0015_question_unit_and_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      848 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0016_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      587 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0017_question_optionsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      691 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0018_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      627 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0019_questionentity_conditions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      699 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0020_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      571 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0021_questionentity_is_collection.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1176 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0022_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      695 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0023_option.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      578 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0024_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     7563 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0025_questionset_and_questionitem.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4444 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0026_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1121 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0027_remove_question_entity_and_question.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      442 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0028_rename_question.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3296 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0029_verbose_name_and_range.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1928 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0030_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      598 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0031_rename_attribute_entity_to_attribute.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1024 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0032_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      678 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0033_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1147 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0034_move_questionset_to_section.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1702 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0035_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1699 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0036_remove_subsection.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1850 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0037_rename_en_to_lang1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1851 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0038_rename_de_to_lang2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5848 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0039_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    11083 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0040_add_language_fields.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2077 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0041_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     9265 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0042_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1023 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0043_django2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2024 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0044_require_uri_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      866 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0045_catalog_sites.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      533 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0046_catalog_groups.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      538 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0047_manager.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1501 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0048_catalog_help.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      337 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0049_manager.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      585 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0050_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      498 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0051_sites_blank.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      494 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0052_available.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1850 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0053_related_name.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1114 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0054_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1297 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0055_catalog_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      480 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0056_question_is_optional.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1735 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0057_question_default_text.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      680 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0058_question_default_option.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      548 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0059_question_default_external_id.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      755 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0060_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      485 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0061_question_width.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     9097 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0062_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      630 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0063_questionset_questionset.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      476 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0064_widget_type_choices.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      800 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0065_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      681 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0066_alter_question_value_type.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1081 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0067_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      672 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/0068_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/migrations/__init__.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.427967 rdmo-1.9.1/rdmo/questions/models/
--rw-rw-r--   0 ole       (1000) ole       (1000)      126 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/models/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5291 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/models/catalog.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    11844 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/models/question.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    11535 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/models/questionset.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4067 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/models/section.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8222 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/renderers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.427967 rdmo-1.9.1/rdmo/questions/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3858 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/serializers/export.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     9841 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/serializers/v1.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/questions/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/questions/static/questions/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.427967 rdmo-1.9.1/rdmo/questions/static/questions/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)      401 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/static/questions/css/catalogs.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.427967 rdmo-1.9.1/rdmo/questions/static/questions/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)    15584 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/static/questions/js/catalogs.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/questions/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.431967 rdmo-1.9.1/rdmo/questions/templates/questions/
--rw-rw-r--   0 ole       (1000) ole       (1000)      133 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalog_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3793 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalog_tree.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     4936 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3737 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_element.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3497 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_catalogs.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1520 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_questions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2243 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_questionsets.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     2696 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_sections.html
--rw-rw-r--   0 ole       (1000) ole       (1000)    12937 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_catalogs.html
--rw-rw-r--   0 ole       (1000) ole       (1000)    30967 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_questions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)    19855 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_questionsets.html
--rw-rw-r--   0 ole       (1000) ole       (1000)    10733 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_sections.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      904 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_catalog.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      829 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_questions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1183 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_questionsets.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      941 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_sections.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     6452 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_sidebar.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1469 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_sidebar_showuri_checkboxes.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.435967 rdmo-1.9.1/rdmo/questions/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      966 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3337 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2528 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_catalogs.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5581 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_questions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4850 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_questionsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3739 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_sections.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2473 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_catalogs.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3974 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_questions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5731 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_questionsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2865 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_sections.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1571 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6807 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_viewset_catalog.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8868 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_viewset_question.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8417 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_viewset_questionset.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6956 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_viewset_section.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      669 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/tests/test_viewset_widgettype.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.435967 rdmo-1.9.1/rdmo/questions/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      305 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      765 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      539 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/utils.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3973 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2509 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)    10435 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/questions/viewsets.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      124 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/questions/widgets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.439967 rdmo-1.9.1/rdmo/services/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/services/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      184 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/services/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8860 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/services/providers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.439967 rdmo-1.9.1/rdmo/services/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      172 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/services/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1191 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/services/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      671 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/services/views.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.439967 rdmo-1.9.1/rdmo/share/
--rw-rw-r--   0 ole       (1000) ole       (1000)    11513 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/share/reference.docx
--rw-rw-r--   0 ole       (1000) ole       (1000)     7780 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/share/reference.odt
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.443967 rdmo-1.9.1/rdmo/tasks/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      810 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      175 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1563 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/imports.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      867 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/managers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.451967 rdmo-1.9.1/rdmo/tasks/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1285 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0001_initial.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      513 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0002_many_to_many_for_conditions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      487 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0003_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3261 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0004_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      578 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0005_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      455 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0006_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      495 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0007_permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      491 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0008_remove_time_period.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1852 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0009_timeframe.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1768 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0010_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      697 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0011_task_text.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1164 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0012_move_attribute_to_attributeentity.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1176 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0013_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1651 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0014_move_timeframe_to_task.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      836 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0015_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0016_remove_timeframe.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      571 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0017_rename_en_to_lang1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0018_rename_de_to_lang2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1271 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0019_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2940 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0020_add_language_fields.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1020 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0021_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3819 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0022_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      396 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0023_django2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      750 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0024_require_uri_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      826 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0025_task_sites.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      520 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0026_task_groups.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      329 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0027_manager.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      559 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0028_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      488 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0029_sites_blank.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      484 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0030_available.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1396 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0031_related_name.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      596 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0032_task_catalogs.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      460 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/0033_task_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6386 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1946 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/renderers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.451967 rdmo-1.9.1/rdmo/tasks/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1116 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/serializers/export.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1897 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/serializers/v1.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/tasks/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/tasks/static/tasks/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.451967 rdmo-1.9.1/rdmo/tasks/static/tasks/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/static/tasks/css/tasks.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.451967 rdmo-1.9.1/rdmo/tasks/static/tasks/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)     4950 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/static/tasks/js/tasks.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/tasks/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.455967 rdmo-1.9.1/rdmo/tasks/templates/tasks/
--rw-rw-r--   0 ole       (1000) ole       (1000)     5498 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1298 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1497 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_delete_tasks.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1661 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_form_conditions.html
--rw-rw-r--   0 ole       (1000) ole       (1000)    14012 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_form_tasks.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     3602 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_form_timeframes.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.455967 rdmo-1.9.1/rdmo/tasks/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      253 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/tests/test_admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1140 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/tests/test_models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2369 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/tests/test_validator_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2342 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/tests/test_validator_unique_uri.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1449 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     7036 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/tests/test_viewset_task.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.455967 rdmo-1.9.1/rdmo/tasks/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      278 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      535 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1779 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/tasks/viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.459967 rdmo-1.9.1/rdmo/views/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      810 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      175 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/apps.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1183 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/imports.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      867 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/managers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.467967 rdmo-1.9.1/rdmo/views/migrations/
--rw-rw-r--   0 ole       (1000) ole       (1000)      746 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0001_initial.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      441 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0002_view_template.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      554 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0003_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1775 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0004_refactoring.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1503 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0005_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1241 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0006_title_and_help.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      618 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0007_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      505 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0008_permissions.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      778 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0009_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      559 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0010_rename_en_to_lang1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0011_rename_de_to_lang2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1373 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0012_meta.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1889 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0013_add_language_fields.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1040 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0014_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     4097 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0015_remove_null_true.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      396 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0016_django2.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      750 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0017_require_uri_prefix.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      853 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0018_view_sites.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      520 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0019_view_groups.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      517 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0020_manager.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      585 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0021_view_catalogs.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      331 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0022_manager.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      559 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0023_data_migration.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      488 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0024_sites_blank.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      484 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0025_available.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      456 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/0026_view_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/migrations/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     5681 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1452 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/renderers.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.467967 rdmo-1.9.1/rdmo/views/serializers/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/serializers/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      640 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/serializers/export.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2344 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/serializers/v1.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/views/static/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/views/static/views/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.467967 rdmo-1.9.1/rdmo/views/static/views/css/
--rw-rw-r--   0 ole       (1000) ole       (1000)       35 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/static/views/css/views.scss
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.467967 rdmo-1.9.1/rdmo/views/static/views/js/
--rw-rw-r--   0 ole       (1000) ole       (1000)     4708 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/static/views/js/views.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.219972 rdmo-1.9.1/rdmo/views/templates/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.471967 rdmo-1.9.1/rdmo/views/templates/views/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.471967 rdmo-1.9.1/rdmo/views/templates/views/tags/
--rw-rw-r--   0 ole       (1000) ole       (1000)      130 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/tags/value.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1165 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/tags/value_file.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      108 2023-01-12 09:58:52.000000 rdmo-1.9.1/rdmo/views/templates/views/tags/value_inline_list.html
--rw-rw-r--   0 ole       (1000) ole       (1000)       92 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/tags/value_list.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     5292 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/views.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      680 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/views_export.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1497 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/views_modal_delete_views.html
--rw-rw-r--   0 ole       (1000) ole       (1000)     1790 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/views_modal_form_templates.html
--rw-rw-r--   0 ole       (1000) ole       (1000)    13885 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templates/views/views_modal_form_views.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.471967 rdmo-1.9.1/rdmo/views/templatetags/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templatetags/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     8006 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/templatetags/view_tags.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.475967 rdmo-1.9.1/rdmo/views/tests/
--rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      253 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/test_admin.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      896 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/test_models.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2369 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/test_validator_locked.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     2342 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/test_validator_unique_uri.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3066 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/test_view_tags.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1449 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/test_views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     6388 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/tests/test_viewset_view.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.475967 rdmo-1.9.1/rdmo/views/urls/
--rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/urls/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      278 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/urls/v1.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     3612 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/utils.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      535 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/validators.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/views.py
--rw-rw-r--   0 ole       (1000) ole       (1000)     1640 2022-08-03 07:29:05.000000 rdmo-1.9.1/rdmo/views/viewsets.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-03 14:47:56.223972 rdmo-1.9.1/rdmo.egg-info/
--rw-r--r--   0 ole       (1000) ole       (1000)     2895 2023-02-03 14:47:56.000000 rdmo-1.9.1/rdmo.egg-info/PKG-INFO
--rw-r--r--   0 ole       (1000) ole       (1000)    45132 2023-02-03 14:47:56.000000 rdmo-1.9.1/rdmo.egg-info/SOURCES.txt
--rw-r--r--   0 ole       (1000) ole       (1000)        1 2023-02-03 14:47:56.000000 rdmo-1.9.1/rdmo.egg-info/dependency_links.txt
--rw-r--r--   0 ole       (1000) ole       (1000)      573 2023-02-03 14:47:56.000000 rdmo-1.9.1/rdmo.egg-info/requires.txt
--rw-r--r--   0 ole       (1000) ole       (1000)        5 2023-02-03 14:47:56.000000 rdmo-1.9.1/rdmo.egg-info/top_level.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.1/requirements.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)       38 2023-02-03 14:47:56.475967 rdmo-1.9.1/setup.cfg
--rw-rw-r--   0 ole       (1000) ole       (1000)     1354 2022-08-03 07:29:05.000000 rdmo-1.9.1/setup.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.968849 rdmo-1.9.2/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1701 2023-01-12 09:58:52.000000 rdmo-1.9.2/AUTHORS
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11359 2022-08-03 07:29:05.000000 rdmo-1.9.2/LICENSE
+-rw-rw-r--   0 ole       (1000) ole       (1000)      102 2022-08-03 07:29:05.000000 rdmo-1.9.2/MANIFEST.in
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7844 2022-08-03 07:29:05.000000 rdmo-1.9.2/NOTICE
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2895 2023-02-23 20:57:37.968849 rdmo-1.9.2/PKG-INFO
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2011 2023-01-12 09:58:52.000000 rdmo-1.9.2/README.md
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.776852 rdmo-1.9.2/rdmo/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      171 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/__init__.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.776852 rdmo-1.9.2/rdmo/accounts/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      452 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/adapter.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      788 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      234 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3906 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/forms.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.780852 rdmo-1.9.2/rdmo/accounts/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1569 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      579 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0002_detail_key_type_field_length_increased.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      687 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0003_hint_renamed_to_help_text.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      923 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0004_permission_added.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      563 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0005_field_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      426 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0006_permissions_removed.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2664 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0007_additional_fields.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      620 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0008_related_name.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      851 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0009_proxyuser.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1133 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0010_consentfieldvalue.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      595 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0011_rename_en_to_lang1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      596 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0012_rename_de_to_lang2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1692 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0013_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2661 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0014_add_language_fields.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      983 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0015_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3175 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0016_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1263 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0017_role.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      770 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0018_blank_fields.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      294 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/0019_delete_proxyuser.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5265 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      405 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/rules.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.780852 rdmo-1.9.2/rdmo/accounts/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1651 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/accounts/serializers/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5947 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/settings.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/accounts/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/accounts/static/accounts/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.780852 rdmo-1.9.2/rdmo/accounts/static/accounts/img/
+-rw-rw-r--   0 ole       (1000) ole       (1000)    32038 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/static/accounts/img/keycloak_logo_200px.svg
+-rw-rw-r--   0 ole       (1000) ole       (1000)    23495 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/static/accounts/img/orcid-signin.png
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/accounts/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.820851 rdmo-1.9.2/rdmo/accounts/templates/account/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.820851 rdmo-1.9.2/rdmo/accounts/templates/account/email/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/email/password_reset_key_message.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)       43 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/email/password_reset_key_subject.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2784 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/email.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1019 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/email_confirm.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      159 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/login.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      828 2023-01-26 18:01:51.000000 rdmo-1.9.2/rdmo/accounts/templates/account/login_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      422 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/login_form_account.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      525 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/login_form_socialaccount.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      535 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/logout.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      238 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/logout_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      540 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/password_change.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      650 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/password_reset.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      633 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/password_reset_done.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      857 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/password_reset_from_key.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      341 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/password_reset_from_key_done.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      501 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/password_set.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1794 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/signup.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      215 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/signup_closed.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1934 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/signup_modal_terms_of_use.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      343 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/terms_of_use.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)       16 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/terms_of_use_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)       16 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/terms_of_use_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      381 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/verification_sent.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      776 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/account/verified_email_required.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.820851 rdmo-1.9.2/rdmo/accounts/templates/profile/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      219 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/profile/profile_remove_closed.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      238 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/profile/profile_remove_failed.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      747 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/profile/profile_remove_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      203 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/profile/profile_remove_success.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      219 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/profile/profile_update_closed.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1373 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/accounts/templates/profile/profile_update_form.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.824851 rdmo-1.9.2/rdmo/accounts/templates/socialaccount/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      303 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/socialaccount/authentication_error.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1879 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/socialaccount/connections.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      435 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/socialaccount/login_cancelled.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1929 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/socialaccount/signup.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.824851 rdmo-1.9.2/rdmo/accounts/templates/socialaccount/snippets/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1511 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templates/socialaccount/snippets/provider_list.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.824851 rdmo-1.9.2/rdmo/accounts/templatetags/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templatetags/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      728 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/templatetags/accounts_tags.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.824851 rdmo-1.9.2/rdmo/accounts/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     9595 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3174 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/tests/test_viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.824851 rdmo-1.9.2/rdmo/accounts/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1094 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      280 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1974 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/utils.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2505 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/accounts/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1331 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/accounts/viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.824851 rdmo-1.9.2/rdmo/conditions/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      793 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      190 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1253 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/imports.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.828851 rdmo-1.9.2/rdmo/conditions/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1748 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0001_initial.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      500 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0002_many_to_many_for_conditions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      705 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0003_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      486 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0004_condition_title.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      746 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0005_empty_relation.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      877 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0006_db_constraint_false.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      482 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0007_ordering.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      599 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0008_validator.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      600 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0009_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      793 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0010_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3110 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0011_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      532 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0012_permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2425 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0013_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1421 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0014_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      679 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0015_move_attribute_to_attributeentity.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1510 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0016_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      828 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0017_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1632 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0018_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      416 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0019_django2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      775 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0020_require_uri_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1054 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0021_related_name.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      474 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/0022_condition_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7840 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1176 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/renderers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.828851 rdmo-1.9.2/rdmo/conditions/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      582 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/serializers/export.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2827 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/serializers/v1.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/conditions/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/conditions/static/conditions/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.828851 rdmo-1.9.2/rdmo/conditions/static/conditions/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/static/conditions/css/conditions.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.828851 rdmo-1.9.2/rdmo/conditions/static/conditions/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4754 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/static/conditions/js/conditions.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/conditions/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.836851 rdmo-1.9.2/rdmo/conditions/templates/conditions/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5224 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      780 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2111 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_modal_delete_conditions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7769 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_modal_form_conditions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2706 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_modal_show_conditions.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.836851 rdmo-1.9.2/rdmo/conditions/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      268 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/test_admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      763 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/test_models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2634 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/test_validator_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2527 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/test_validator_unique_uri.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1494 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6498 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/test_viewset_condition.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      663 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/tests/test_viewset_relation.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.836851 rdmo-1.9.2/rdmo/conditions/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      278 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      388 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1619 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2141 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/conditions/viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.840851 rdmo-1.9.2/rdmo/core/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1955 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/core/constants.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)       41 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/exceptions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      475 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/exports.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4807 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/imports.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      528 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/mail.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.840851 rdmo-1.9.2/rdmo/core/management/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/__init__.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.840851 rdmo-1.9.2/rdmo/core/management/commands/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      259 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/create_admin_user.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2174 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/delete_users.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      483 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/deploy.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2139 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/download_vendor_files.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1163 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/core/management/commands/find_inactive_users.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5275 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/find_spam_users.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3817 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/find_users.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2830 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/make_theme.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      468 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/poedit.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1815 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/set_uri_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      544 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/setup_groups.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      733 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/management/commands/upgrade.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1157 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/managers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1312 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3914 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      778 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/plugins.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1088 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/renderers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2184 2023-01-12 12:00:20.000000 rdmo-1.9.2/rdmo/core/serializers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    12536 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/core/settings.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/core/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/core/static/core/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.840851 rdmo-1.9.2/rdmo/core/static/core/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7899 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/base.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)      151 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/codemirror.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)      982 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/fonts.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1011 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/footer.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1837 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/header.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/style.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)      532 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/swagger.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)      878 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/css/variables.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.844851 rdmo-1.9.2/rdmo/core/static/core/fonts/
+-rwxrwxr-x   0 ole       (1000) ole       (1000)    42480 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSans-Bold.ttf
+-rwxrwxr-x   0 ole       (1000) ole       (1000)    41028 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSans.ttf
+-rwxrwxr-x   0 ole       (1000) ole       (1000)   117072 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSansMono.ttf
+-rwxrwxr-x   0 ole       (1000) ole       (1000)    48880 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif-Bold.ttf
+-rwxrwxr-x   0 ole       (1000) ole       (1000)    45652 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif-BoldItalic.ttf
+-rwxrwxr-x   0 ole       (1000) ole       (1000)    40416 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif-Italic.ttf
+-rwxrwxr-x   0 ole       (1000) ole       (1000)    43648 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif.ttf
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.848851 rdmo-1.9.2/rdmo/core/static/core/html/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      471 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_checkbox.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      428 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_codemirror.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      442 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_number.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      811 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_select.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      591 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_selectmultiple.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      633 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_selectnumber.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      454 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_text.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      413 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/html/formgroup_textarea.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.848851 rdmo-1.9.2/rdmo/core/static/core/img/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1129 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/img/favicon.png
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.848851 rdmo-1.9.2/rdmo/core/static/core/img/header/
+-rw-rw-r--   0 ole       (1000) ole       (1000)   155589 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/img/header/collection.jpg
+-rw-rw-r--   0 ole       (1000) ole       (1000)   183545 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/img/header/library.jpg
+-rw-rw-r--   0 ole       (1000) ole       (1000)    87777 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/img/header/supercomputer.jpg
+-rw-rw-r--   0 ole       (1000) ole       (1000)     9109 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/img/rdmo-logo.svg
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.852851 rdmo-1.9.2/rdmo/core/static/core/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6934 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/js/core.js
+-rw-rw-r--   0 ole       (1000) ole       (1000)      448 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/static/core/js/header.js
+-rw-rw-r--   0 ole       (1000) ole       (1000)      655 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/swagger.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/core/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.864850 rdmo-1.9.2/rdmo/core/templates/core/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      207 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/400.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      196 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/403.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      193 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/404.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      211 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/500.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      377 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/about.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1502 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/about_text_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1363 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/about_text_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1522 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/about_text_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1341 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/about_text_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      107 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/back_to_project_link.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      599 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/base.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/base_analytics.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      139 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/base_footer.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1147 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/core/templates/core/base_head.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6836 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/base_navigation.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      219 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/base_navigation_account.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      130 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/base_navigation_socialaccount.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      316 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/bootstrap_delete_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      397 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/bootstrap_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1561 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/bootstrap_form_field.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      327 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/bootstrap_form_fields.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      178 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/error.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      131 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      707 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/footer_text_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      703 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/footer_text_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      718 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/footer_text_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/footer_text_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2235 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/home.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      621 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/home_text_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      537 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/home_text_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      612 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/home_text_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/home_text_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      327 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/page.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1198 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/core/upload_form.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.864850 rdmo-1.9.2/rdmo/core/templates/rest_framework_swagger/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2453 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templates/rest_framework_swagger/index.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.864850 rdmo-1.9.2/rdmo/core/templatetags/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/templatetags/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5448 2023-02-12 23:03:07.000000 rdmo-1.9.2/rdmo/core/templatetags/core_tags.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.864850 rdmo-1.9.2/rdmo/core/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2649 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_mail.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      411 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_swagger.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      842 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_tags.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      569 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_utils.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1552 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1535 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      725 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_viewset_settings.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2992 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/tests/test_xml.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.868850 rdmo-1.9.2/rdmo/core/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      768 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      132 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/urls/swagger.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      919 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11580 2023-02-12 23:33:22.000000 rdmo-1.9.2/rdmo/core/utils.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2696 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4209 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2927 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/core/viewsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2819 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/core/xml.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.868850 rdmo-1.9.2/rdmo/domain/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1303 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      178 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1432 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/imports.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.872850 rdmo-1.9.2/rdmo/domain/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5213 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0001_initial_after_reset.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      415 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0002_additional_input.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      637 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0003_condition.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1078 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0004_verbosename.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      456 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0005_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      585 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0006_attributeentity_parent_collection.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      491 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0007_db_index.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      605 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0008_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0009_remove_condition.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      534 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0010_many_to_many_for_conditions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      499 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0011_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      426 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0012_renaming.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1972 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0013_mptt.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      449 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0014_is_attribute.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      640 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0015_label.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      268 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0016_label.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      602 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0017_url_value_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      607 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0018_validator.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      519 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0019_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      676 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0020_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      465 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0021_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      495 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0022_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      460 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0023_fix_label.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      519 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0024_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      776 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0025_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6809 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0026_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      489 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0027_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      416 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0028_path.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      558 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0029_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1257 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0030_permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1187 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0031_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      580 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0032_remove_unit_and_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      448 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0033_remove_attribute_optionsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0034_remove_attributeentity_conditions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      592 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0035_remove_is_collection_and_parent_collection.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      726 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0036_remove_range_and_verbosename.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1035 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0037_remove_attribute.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      424 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0038_rename_attributeentity_to_attribute.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2390 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0039_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      561 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0040_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      813 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0041_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1292 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0042_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      816 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0043_django2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      719 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0044_mptt.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      764 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0045_require_uri_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      628 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0046_parent_cascade.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      496 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0047_attribute_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      498 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/0048_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3207 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1137 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/renderers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.872850 rdmo-1.9.2/rdmo/domain/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      422 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/serializers/export.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3403 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/domain/serializers/v1.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/domain/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/domain/static/domain/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.872850 rdmo-1.9.2/rdmo/domain/static/domain/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)       45 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/static/domain/css/domain.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.872850 rdmo-1.9.2/rdmo/domain/static/domain/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4331 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/static/domain/js/domain.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.768852 rdmo-1.9.2/rdmo/domain/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.872850 rdmo-1.9.2/rdmo/domain/templates/domain/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3904 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/templates/domain/domain.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      309 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/templates/domain/domain_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3568 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/templates/domain/domain_modal_delete_attributes.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6031 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/templates/domain/domain_modal_form_attributes.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3490 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/templates/domain/domain_modal_show_attributes.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      943 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/templates/domain/domain_options.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.872850 rdmo-1.9.2/rdmo/domain/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      264 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/test_admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      791 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/test_models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6543 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/test_validator_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3636 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/test_validator_parent.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3134 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/test_validator_unique_uri.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1481 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6265 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/tests/test_viewset_attribute.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.872850 rdmo-1.9.2/rdmo/domain/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      253 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      299 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1742 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2070 2023-02-09 08:26:39.000000 rdmo-1.9.2/rdmo/domain/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2385 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/domain/viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/locale/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/locale/de/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.876850 rdmo-1.9.2/rdmo/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 ole       (1000) ole       (1000)   100199 2023-02-03 12:13:41.000000 rdmo-1.9.2/rdmo/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 ole       (1000) ole       (1000)   191976 2023-02-03 12:59:55.000000 rdmo-1.9.2/rdmo/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/locale/es/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.876850 rdmo-1.9.2/rdmo/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 ole       (1000) ole       (1000)   100400 2023-02-03 12:13:41.000000 rdmo-1.9.2/rdmo/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 ole       (1000) ole       (1000)   182130 2023-02-03 12:59:42.000000 rdmo-1.9.2/rdmo/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/locale/fr/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.876850 rdmo-1.9.2/rdmo/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 ole       (1000) ole       (1000)   102473 2023-02-03 12:13:41.000000 rdmo-1.9.2/rdmo/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 ole       (1000) ole       (1000)   194518 2023-02-03 12:59:56.000000 rdmo-1.9.2/rdmo/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/locale/it/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.880850 rdmo-1.9.2/rdmo/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 ole       (1000) ole       (1000)    98657 2023-02-03 12:13:41.000000 rdmo-1.9.2/rdmo/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 ole       (1000) ole       (1000)   181203 2023-02-03 12:59:58.000000 rdmo-1.9.2/rdmo/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/locale/nl/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.880850 rdmo-1.9.2/rdmo/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      380 2023-02-03 12:13:41.000000 rdmo-1.9.2/rdmo/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 ole       (1000) ole       (1000)   138451 2023-02-03 12:59:59.000000 rdmo-1.9.2/rdmo/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.880850 rdmo-1.9.2/rdmo/management/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      190 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4727 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/imports.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/management/management/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.880850 rdmo-1.9.2/rdmo/management/management/commands/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/management/commands/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      978 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/management/commands/import.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/management/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.880850 rdmo-1.9.2/rdmo/management/templates/management/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3284 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/templates/management/import.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4640 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/templates/management/upload.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.880850 rdmo-1.9.2/rdmo/management/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1322 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/tests/test_commands.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2167 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/tests/test_import.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6868 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/tests/test_views.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.880850 rdmo-1.9.2/rdmo/management/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/management/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5042 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/management/views.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.884850 rdmo-1.9.2/rdmo/options/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1442 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      181 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2405 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/imports.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.884850 rdmo-1.9.2/rdmo/options/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2192 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0001_initial.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      880 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0002_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1683 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0003_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      519 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0004_conditions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      739 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0005_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4475 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0006_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      651 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0007_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      530 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0008_option_path.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      554 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0009_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      760 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0010_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      780 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0011_permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0012_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      557 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0013_order.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      421 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0014_rename_en_to_lang1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      434 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0015_rename_de_to_lang2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      807 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0016_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1666 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0017_add_language_fields.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1112 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0018_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3878 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0019_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1020 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0020_django2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      532 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0021_data_migrations.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      575 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0022_cascade_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1187 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0023_require_uri_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      545 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0024_related_name.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      531 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0025_optionset_provider_key.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      738 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0026_optionset_option_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      503 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/0027_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7085 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      592 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/providers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2574 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/renderers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.884850 rdmo-1.9.2/rdmo/options/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1157 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/serializers/export.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4757 2023-01-16 11:16:32.000000 rdmo-1.9.2/rdmo/options/serializers/v1.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/options/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/options/static/options/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.884850 rdmo-1.9.2/rdmo/options/static/options/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/static/options/css/options.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.884850 rdmo-1.9.2/rdmo/options/static/options/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6187 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/static/options/js/options.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/options/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.888850 rdmo-1.9.2/rdmo/options/templates/options/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8603 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1516 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2205 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_modal_delete_options.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2729 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_modal_delete_optionsets.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1666 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_modal_form_conditions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)    10359 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_modal_form_options.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6471 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_modal_form_optionsets.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1733 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_modal_show_options.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1401 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/templates/options/options_modal_show_optionsets.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.888850 rdmo-1.9.2/rdmo/options/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      492 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1420 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3729 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_validator_locked_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2634 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_validator_locked_optionsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2872 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_validator_unique_uri_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2527 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_validator_unique_uri_optionsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1480 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6380 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_viewset_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6655 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/tests/test_viewset_optionsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.888850 rdmo-1.9.2/rdmo/options/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      260 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1174 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1643 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3976 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/options/viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.888850 rdmo-1.9.2/rdmo/overlays/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      310 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      183 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/apps.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.888850 rdmo-1.9.2/rdmo/overlays/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1455 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/migrations/0001_initial.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1107 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/models.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/overlays/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/overlays/static/overlays/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.888850 rdmo-1.9.2/rdmo/overlays/static/overlays/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      444 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/static/overlays/css/overlays.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.888850 rdmo-1.9.2/rdmo/overlays/static/overlays/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2593 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/overlays/static/overlays/js/overlays.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/overlays/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.892850 rdmo-1.9.2/rdmo/overlays/templates/overlays/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      286 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/templates/overlays/buttons.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      589 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/templates/overlays/reset_overlays.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.892850 rdmo-1.9.2/rdmo/overlays/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1020 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2030 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/tests/test_viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.892850 rdmo-1.9.2/rdmo/overlays/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      142 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      292 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      561 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/overlays/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2680 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/overlays/viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.892850 rdmo-1.9.2/rdmo/projects/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3494 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      345 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      291 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/constants.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5177 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/exports.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1211 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/filters.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    12820 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/forms.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2234 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/handlers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    12552 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/imports.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.892850 rdmo-1.9.2/rdmo/projects/management/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/management/__init__.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.892850 rdmo-1.9.2/rdmo/projects/management/commands/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/management/commands/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1169 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/management/commands/delete_projects.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4889 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/management/commands/export_projects.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1600 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/management/commands/find_inactive_projects.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1775 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/management/commands/prune_projects.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5444 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/managers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.896850 rdmo-1.9.2/rdmo/projects/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3680 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0001_initial_after_reset.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1065 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0002_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      488 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0003_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      589 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0004_remove_current_snapshot.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      736 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0005_snapshot.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      813 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0006_project_values.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      676 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0007_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0008_not_null.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      623 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0009_options.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      564 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0010_add_db_contraint.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4186 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0011_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2158 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0012_membership.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      670 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0013_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      387 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0014_remove_owner.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1257 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0015_permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      651 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0016_catalog_on_delete.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      995 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0017_value_unit_and_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      770 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0018_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      678 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0019_option.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      584 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0020_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0021_order.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      658 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0022_move_attribute_to_attributeentity.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0023_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      734 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0024_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      511 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0025_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1392 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0026_django2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      968 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0027_project_site.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      553 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0028_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      328 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0029_remove_manager.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      523 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0030_project_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      523 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0031_project_tasks.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1001 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0032_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      622 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0033_default_value_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1319 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0034_issue.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      650 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0035_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      326 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0036_remove_project_tasks.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      555 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0037_project_tasks.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1962 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0038_integration_integrationoption.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      520 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0039_integrationoption_secret.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1258 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0040_issueresource.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      467 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0041_value_external_id.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      571 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0042_allow_site_null.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      598 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0043_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      575 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0044_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1297 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0045_value_file.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2061 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0046_project_mptt.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1631 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0047_continuation.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1210 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0048_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1749 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0049_invite.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1096 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0050_value_set_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      682 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0051_alter_value_value_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      923 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/0052_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    10505 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/mixins.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.896850 rdmo-1.9.2/rdmo/projects/models/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      282 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1078 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/continuation.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2708 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/integration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2261 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/models/invite.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3918 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/issue.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/membership.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5517 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/project.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2489 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/snapshot.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7893 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/models/value.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8651 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/providers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3374 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/renderers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4198 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/rules.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.896850 rdmo-1.9.2/rdmo/projects/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2339 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/serializers/export.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.900850 rdmo-1.9.2/rdmo/projects/serializers/v1/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6594 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/serializers/v1/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1605 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/serializers/v1/overview.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3817 2023-02-03 11:15:14.000000 rdmo-1.9.2/rdmo/projects/serializers/v1/questionset.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/projects/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/projects/static/projects/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.900850 rdmo-1.9.2/rdmo/projects/static/projects/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      303 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/static/projects/css/project.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5912 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/static/projects/css/project_questions.scss
+-rw-rw-r--   0 ole       (1000) ole       (1000)      370 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/static/projects/css/projects.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/projects/static/projects/js/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.900850 rdmo-1.9.2/rdmo/projects/static/projects/js/project_questions/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      187 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/static/projects/js/project_questions/app.js
+-rw-rw-r--   0 ole       (1000) ole       (1000)      448 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/static/projects/js/project_questions/controllers.js
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3376 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/static/projects/js/project_questions/directives.js
+-rw-rw-r--   0 ole       (1000) ole       (1000)    61227 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/static/projects/js/project_questions/services.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/projects/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.920849 rdmo-1.9.2/rdmo/projects/templates/projects/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.920849 rdmo-1.9.2/rdmo/projects/templates/projects/email/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      793 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/email/project_invite_message.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)      215 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/email/project_invite_subject.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)      467 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/integration_confirm_delete.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      473 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/integration_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      854 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/invite_confirm_delete.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1967 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_detail.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      184 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1828 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_send.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1004 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_send_email.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1322 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_send_integrations.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      472 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_send_message.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)      487 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_send_sidebar.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)       38 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/issue_send_subject.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)      510 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/membership_confirm_delete.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1109 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/membership_form.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.936849 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      256 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      236 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      237 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_attachments_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      413 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_message_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_message_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      378 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_message_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      348 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_issue_message_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      271 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_support_info_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      272 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_support_info_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      299 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_support_info_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      268 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/issue_send_support_info_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      318 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_export_project_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      272 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_export_project_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      298 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_export_project_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      276 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_export_project_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      332 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_import_project_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      285 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_import_project_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      298 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_import_project_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      274 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_import_project_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      243 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_catalog_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      245 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_catalog_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      255 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_catalog_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      241 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_catalog_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      688 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      613 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      708 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      627 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      402 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_memberships_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      337 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_memberships_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      390 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_memberships_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      351 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_memberships_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      528 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_questions_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      458 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_questions_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      540 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_questions_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      504 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_questions_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      443 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_snapshots_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      390 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_snapshots_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_snapshots_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      439 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_snapshots_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      679 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      592 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      681 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      627 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      271 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_support_info_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      272 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_support_info_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      299 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_support_info_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      268 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_support_info_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_create_project_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      233 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_create_project_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      260 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_create_project_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      240 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_create_project_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      384 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_import_project_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      331 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_import_project_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      351 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_import_project_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_import_project_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      534 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      514 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      566 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      526 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      271 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_support_info_de.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      272 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_support_info_en.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      299 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_support_info_fr.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      268 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_support_info_it.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2338 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_answers.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2029 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_answers_element.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      245 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_answers_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      458 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_answers_tree.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      399 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_confirm_cancel.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      829 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_confirm_delete.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      465 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_confirm_leave.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1927 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1336 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_header.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      346 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_header_catalog.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      363 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_header_description.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      872 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_header_hierarchy.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2440 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_integrations.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      252 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_integrations_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1432 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_invites.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3320 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_issues.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      290 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_issues_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3011 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_memberships.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      358 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_memberships_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5084 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_sidebar.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      604 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_sidebar_parent_import.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2883 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_snapshots.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      350 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_snapshots_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2007 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_views.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      360 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_views_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      533 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_error.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1029 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7959 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_import.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      414 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_import_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3318 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      369 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_add_field_button.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      326 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_add_field_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      396 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_add_set_button.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      328 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_add_set_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1868 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_buttons.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      235 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_default.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      338 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_done.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1422 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_element.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      320 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_erase_field.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      446 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_error.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2921 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_autocomplete.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1675 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_checkbox.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1559 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_date.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2006 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_file.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2675 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_radio.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1946 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_range.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1784 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_select.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1436 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_text.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1468 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_textarea.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2409 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_yesno.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      405 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_head.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2354 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_modal_delete_valuesets.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1603 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_modal_form_valuesets.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      942 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_navigation.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      480 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_navigation_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      389 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_overview.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      442 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_progress.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      107 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_question_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      194 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_question_label.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      461 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_question_warning.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2362 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_questionset_head.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      505 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_questionset_head_help.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      513 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_remove_field.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      428 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_remove_set.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      367 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_sidebar.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2352 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_view.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      104 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/project_view_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5445 2023-02-03 12:06:55.000000 rdmo-1.9.2/rdmo/projects/templates/projects/projects.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      946 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/projects_pagination.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2281 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/site_projects.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      344 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/snapshot_form.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      496 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templates/projects/snapshot_rollback.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.936849 rdmo-1.9.2/rdmo/projects/templatetags/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templatetags/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2509 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/templatetags/projects_tags.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.936849 rdmo-1.9.2/rdmo/projects/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2231 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_commands.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2702 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/tests/test_handlers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1425 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8336 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_integration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8066 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_issue.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    10163 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_membership.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3775 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_membership_multisite.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    22282 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_project.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    10210 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_project_create_import.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4161 2023-02-23 20:56:59.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_project_join.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5152 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_project_leave.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    18078 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_project_update_import.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7808 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_view_snapshot.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3582 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_integration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3421 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_issue.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3559 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_membership.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8503 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_project.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8327 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_integration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4764 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_issue.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5167 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_membership.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1246 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_questionset.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6633 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_snapshot.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11770 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_value.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3346 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_snapshot.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5302 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/tests/test_viewset_value.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.936849 rdmo-1.9.2/rdmo/projects/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6163 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1901 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5430 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/utils.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      789 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/validators.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.940849 rdmo-1.9.2/rdmo/projects/views/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1243 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/views/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3103 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/views/integration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      614 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/views/invite.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7611 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/views/issue.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4389 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/views/membership.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    10629 2023-02-23 18:02:22.000000 rdmo-1.9.2/rdmo/projects/views/project.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4201 2023-02-12 23:33:20.000000 rdmo-1.9.2/rdmo/projects/views/project_answers.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3034 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/views/project_create.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4954 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/views/project_update.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3527 2023-02-12 23:34:16.000000 rdmo-1.9.2/rdmo/projects/views/project_view.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2139 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/views/snapshot.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    17721 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/viewsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1341 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/projects/widgets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.940849 rdmo-1.9.2/rdmo/questions/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3632 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      187 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      408 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/constants.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      135 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/forms.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6924 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/imports.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2180 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/managers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.944849 rdmo-1.9.2/rdmo/questions/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5793 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0001_initial_after_reset.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      712 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0002_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      422 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0003_renaming.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1129 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0004_full_title.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1309 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0005_label.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1162 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0006_auto_20160803_1619.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11515 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0007_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1174 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0008_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1904 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0009_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1766 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0010_label.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      694 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0011_path.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1118 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0012_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1665 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0013_permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3138 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0014_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1005 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0015_question_unit_and_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      848 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0016_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      587 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0017_question_optionsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      691 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0018_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      627 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0019_questionentity_conditions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      699 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0020_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      571 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0021_questionentity_is_collection.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1176 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0022_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      695 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0023_option.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      578 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0024_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7563 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0025_questionset_and_questionitem.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4444 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0026_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1121 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0027_remove_question_entity_and_question.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      442 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0028_rename_question.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3296 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0029_verbose_name_and_range.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1928 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0030_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      598 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0031_rename_attribute_entity_to_attribute.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1024 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0032_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      678 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0033_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1147 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0034_move_questionset_to_section.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1702 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0035_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1699 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0036_remove_subsection.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1850 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0037_rename_en_to_lang1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1851 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0038_rename_de_to_lang2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5848 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0039_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11083 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0040_add_language_fields.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2077 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0041_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     9265 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0042_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1023 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0043_django2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2024 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0044_require_uri_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      866 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0045_catalog_sites.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      533 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0046_catalog_groups.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      538 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0047_manager.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1501 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0048_catalog_help.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      337 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0049_manager.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      585 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0050_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      498 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0051_sites_blank.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      494 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0052_available.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1850 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0053_related_name.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1114 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0054_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1297 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0055_catalog_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      480 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0056_question_is_optional.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1735 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0057_question_default_text.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      680 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0058_question_default_option.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      548 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0059_question_default_external_id.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      755 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0060_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      485 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0061_question_width.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     9097 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0062_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      630 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0063_questionset_questionset.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      476 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0064_widget_type_choices.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      800 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0065_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      681 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0066_alter_question_value_type.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1081 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0067_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      672 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/0068_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/migrations/__init__.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.944849 rdmo-1.9.2/rdmo/questions/models/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      126 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/models/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5291 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/models/catalog.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11844 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/models/question.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11535 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/models/questionset.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4067 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/models/section.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8222 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/renderers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.944849 rdmo-1.9.2/rdmo/questions/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3858 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/serializers/export.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     9841 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/serializers/v1.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/questions/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/questions/static/questions/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.944849 rdmo-1.9.2/rdmo/questions/static/questions/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      401 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/static/questions/css/catalogs.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.944849 rdmo-1.9.2/rdmo/questions/static/questions/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)    15584 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/static/questions/js/catalogs.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/questions/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.952849 rdmo-1.9.2/rdmo/questions/templates/questions/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      133 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalog_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3793 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalog_tree.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4936 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3737 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_element.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3497 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_catalogs.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1520 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_questions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2243 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_questionsets.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2696 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_sections.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)    12937 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_catalogs.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)    30967 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_questions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)    19855 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_questionsets.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)    10733 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_sections.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      904 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_catalog.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      829 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_questions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1183 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_questionsets.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      941 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_sections.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6452 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_sidebar.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1469 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_sidebar_showuri_checkboxes.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.952849 rdmo-1.9.2/rdmo/questions/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      966 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3337 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2528 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_catalogs.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5581 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_questions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4850 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_questionsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3739 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_sections.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2473 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_catalogs.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3974 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_questions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5731 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_questionsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2865 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_sections.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1571 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6807 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_viewset_catalog.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8868 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_viewset_question.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8417 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_viewset_questionset.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6956 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_viewset_section.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      669 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/tests/test_viewset_widgettype.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.952849 rdmo-1.9.2/rdmo/questions/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      305 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      765 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      539 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/utils.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3973 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2509 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)    10435 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/questions/viewsets.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      124 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/questions/widgets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.952849 rdmo-1.9.2/rdmo/services/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/services/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      184 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/services/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8860 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/services/providers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.952849 rdmo-1.9.2/rdmo/services/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      172 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/services/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1191 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/services/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      671 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/services/views.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.952849 rdmo-1.9.2/rdmo/share/
+-rw-rw-r--   0 ole       (1000) ole       (1000)    11513 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/share/reference.docx
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7780 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/share/reference.odt
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.956849 rdmo-1.9.2/rdmo/tasks/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      810 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      175 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1563 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/imports.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      867 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/managers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.956849 rdmo-1.9.2/rdmo/tasks/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1285 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      513 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0002_many_to_many_for_conditions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      487 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0003_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3261 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0004_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      578 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0005_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      455 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0006_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      495 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0007_permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      491 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0008_remove_time_period.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1852 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0009_timeframe.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1768 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0010_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      697 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0011_task_text.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1164 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0012_move_attribute_to_attributeentity.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1176 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0013_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1651 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0014_move_timeframe_to_task.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      836 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0015_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      690 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0016_remove_timeframe.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      571 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0017_rename_en_to_lang1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0018_rename_de_to_lang2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1271 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0019_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2940 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0020_add_language_fields.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1020 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0021_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3819 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0022_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      396 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0023_django2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      750 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0024_require_uri_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      826 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0025_task_sites.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      520 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0026_task_groups.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      329 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0027_manager.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      559 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0028_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      488 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0029_sites_blank.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      484 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0030_available.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1396 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0031_related_name.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      596 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0032_task_catalogs.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      460 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/0033_task_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6386 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1946 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/renderers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.956849 rdmo-1.9.2/rdmo/tasks/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1116 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/serializers/export.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1897 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/serializers/v1.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/tasks/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/tasks/static/tasks/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.956849 rdmo-1.9.2/rdmo/tasks/static/tasks/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/static/tasks/css/tasks.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.956849 rdmo-1.9.2/rdmo/tasks/static/tasks/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4950 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/static/tasks/js/tasks.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.772852 rdmo-1.9.2/rdmo/tasks/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.960849 rdmo-1.9.2/rdmo/tasks/templates/tasks/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5498 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1298 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1497 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_delete_tasks.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1661 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_form_conditions.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)    14012 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_form_tasks.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3602 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_form_timeframes.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.960849 rdmo-1.9.2/rdmo/tasks/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      253 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/tests/test_admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1140 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/tests/test_models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2369 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/tests/test_validator_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2342 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/tests/test_validator_unique_uri.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1449 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7036 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/tests/test_viewset_task.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.960849 rdmo-1.9.2/rdmo/tasks/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      278 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      535 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1779 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/tasks/viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.960849 rdmo-1.9.2/rdmo/views/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      810 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      175 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/apps.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1183 2023-02-13 09:46:16.000000 rdmo-1.9.2/rdmo/views/imports.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      867 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/managers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.964849 rdmo-1.9.2/rdmo/views/migrations/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      746 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0001_initial.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      441 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0002_view_template.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      554 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0003_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1775 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0004_refactoring.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1503 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0005_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1241 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0006_title_and_help.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      618 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0007_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      505 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0008_permissions.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      778 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0009_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      559 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0010_rename_en_to_lang1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0011_rename_de_to_lang2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1373 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0012_meta.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1889 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0013_add_language_fields.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1040 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0014_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4097 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0015_remove_null_true.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      396 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0016_django2.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      750 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0017_require_uri_prefix.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      853 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0018_view_sites.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      520 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0019_view_groups.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      517 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0020_manager.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      585 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0021_view_catalogs.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      331 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0022_manager.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      559 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0023_data_migration.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      488 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0024_sites_blank.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      484 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0025_available.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      456 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/0026_view_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/migrations/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5681 2023-02-23 14:22:38.000000 rdmo-1.9.2/rdmo/views/models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1452 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/renderers.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.964849 rdmo-1.9.2/rdmo/views/serializers/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/serializers/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      640 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/serializers/export.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2344 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/serializers/v1.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.776852 rdmo-1.9.2/rdmo/views/static/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.776852 rdmo-1.9.2/rdmo/views/static/views/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.964849 rdmo-1.9.2/rdmo/views/static/views/css/
+-rw-rw-r--   0 ole       (1000) ole       (1000)       35 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/static/views/css/views.scss
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.964849 rdmo-1.9.2/rdmo/views/static/views/js/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     4708 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/static/views/js/views.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.776852 rdmo-1.9.2/rdmo/views/templates/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.964849 rdmo-1.9.2/rdmo/views/templates/views/
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.968849 rdmo-1.9.2/rdmo/views/templates/views/tags/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      130 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templates/views/tags/value.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1165 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templates/views/tags/value_file.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      108 2023-01-12 09:58:52.000000 rdmo-1.9.2/rdmo/views/templates/views/tags/value_inline_list.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)       92 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templates/views/tags/value_list.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5292 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templates/views/views.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      680 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templates/views/views_export.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1497 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templates/views/views_modal_delete_views.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1790 2023-02-23 14:22:40.000000 rdmo-1.9.2/rdmo/views/templates/views/views_modal_form_templates.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)    13885 2023-02-23 14:22:41.000000 rdmo-1.9.2/rdmo/views/templates/views/views_modal_form_views.html
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.968849 rdmo-1.9.2/rdmo/views/templatetags/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templatetags/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     8006 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/templatetags/view_tags.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.968849 rdmo-1.9.2/rdmo/views/tests/
+-rw-rw-r--   0 ole       (1000) ole       (1000)        0 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      253 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/test_admin.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      896 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/test_models.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2369 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/test_validator_locked.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2342 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/test_validator_unique_uri.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3066 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/test_view_tags.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1449 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/test_views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     6388 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/tests/test_viewset_view.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.968849 rdmo-1.9.2/rdmo/views/urls/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      248 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/urls/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      278 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/urls/v1.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3612 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/utils.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      535 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/validators.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1504 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/views.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1640 2022-08-03 07:29:05.000000 rdmo-1.9.2/rdmo/views/viewsets.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-02-23 20:57:37.776852 rdmo-1.9.2/rdmo.egg-info/
+-rw-r--r--   0 ole       (1000) ole       (1000)     2895 2023-02-23 20:57:37.000000 rdmo-1.9.2/rdmo.egg-info/PKG-INFO
+-rw-r--r--   0 ole       (1000) ole       (1000)    45186 2023-02-23 20:57:37.000000 rdmo-1.9.2/rdmo.egg-info/SOURCES.txt
+-rw-r--r--   0 ole       (1000) ole       (1000)        1 2023-02-23 20:57:37.000000 rdmo-1.9.2/rdmo.egg-info/dependency_links.txt
+-rw-r--r--   0 ole       (1000) ole       (1000)      573 2023-02-23 20:57:37.000000 rdmo-1.9.2/rdmo.egg-info/requires.txt
+-rw-r--r--   0 ole       (1000) ole       (1000)        5 2023-02-23 20:57:37.000000 rdmo-1.9.2/rdmo.egg-info/top_level.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)      573 2022-08-03 07:29:05.000000 rdmo-1.9.2/requirements.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)       38 2023-02-23 20:57:37.968849 rdmo-1.9.2/setup.cfg
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1354 2022-08-03 07:29:05.000000 rdmo-1.9.2/setup.py
```

### Comparing `rdmo-1.9.1/AUTHORS` & `rdmo-1.9.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/LICENSE` & `rdmo-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/NOTICE` & `rdmo-1.9.2/NOTICE`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/PKG-INFO` & `rdmo-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdmo
-Version: 1.9.1
+Version: 1.9.2
 Summary: RDMO is a tool to support the systematic planning, organisation and implementation of the data management throughout the course of a research project.
 Home-page: https://github.com/rdmorganiser/rdmo
 Author: RDMO Arbeitsgemeinschaft
 Author-email: rdmo-team@listserv.dfn.de
 Maintainer: RDMO Arbeitsgemeinschaft
 Maintainer-email: rdmo-team@listserv.dfn.de
 License: Apache-2.0
```

### Comparing `rdmo-1.9.1/README.md` & `rdmo-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/admin.py` & `rdmo-1.9.2/rdmo/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/forms.py` & `rdmo-1.9.2/rdmo/accounts/forms.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0001_initial.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0002_detail_key_type_field_length_increased.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0002_detail_key_type_field_length_increased.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0003_hint_renamed_to_help_text.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0003_hint_renamed_to_help_text.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0004_permission_added.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0004_permission_added.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0005_field_type.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0005_field_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0007_additional_fields.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0007_additional_fields.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0008_related_name.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0008_related_name.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0009_proxyuser.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0009_proxyuser.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0010_consentfieldvalue.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0010_consentfieldvalue.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0011_rename_en_to_lang1.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0011_rename_en_to_lang1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0012_rename_de_to_lang2.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0012_rename_de_to_lang2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0013_meta.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0013_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0014_add_language_fields.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0014_add_language_fields.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0015_data_migration.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0015_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0016_remove_null_true.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0016_remove_null_true.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0017_role.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0017_role.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/migrations/0018_blank_fields.py` & `rdmo-1.9.2/rdmo/accounts/migrations/0018_blank_fields.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/models.py` & `rdmo-1.9.2/rdmo/accounts/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/serializers/v1.py` & `rdmo-1.9.2/rdmo/accounts/serializers/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/settings.py` & `rdmo-1.9.2/rdmo/accounts/settings.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/static/accounts/img/keycloak_logo_200px.svg` & `rdmo-1.9.2/rdmo/accounts/static/accounts/img/keycloak_logo_200px.svg`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/static/accounts/img/orcid-signin.png` & `rdmo-1.9.2/rdmo/accounts/static/accounts/img/orcid-signin.png`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/email/password_reset_key_message.txt` & `rdmo-1.9.2/rdmo/accounts/templates/account/email/password_reset_key_message.txt`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/email.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/email_confirm.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/login_form.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/login_form.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/login_form_socialaccount.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/login_form_socialaccount.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/logout.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/password_change.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/password_reset.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/password_reset_done.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/password_reset_from_key.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/signup.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/signup_modal_terms_of_use.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/signup_modal_terms_of_use.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/account/verified_email_required.html` & `rdmo-1.9.2/rdmo/accounts/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/profile/profile_remove_form.html` & `rdmo-1.9.2/rdmo/accounts/templates/profile/profile_remove_form.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/profile/profile_update_form.html` & `rdmo-1.9.2/rdmo/accounts/templates/profile/profile_update_form.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/socialaccount/connections.html` & `rdmo-1.9.2/rdmo/accounts/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/socialaccount/signup.html` & `rdmo-1.9.2/rdmo/accounts/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templates/socialaccount/snippets/provider_list.html` & `rdmo-1.9.2/rdmo/accounts/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/templatetags/accounts_tags.py` & `rdmo-1.9.2/rdmo/accounts/templatetags/accounts_tags.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/tests/test_views.py` & `rdmo-1.9.2/rdmo/accounts/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/tests/test_viewsets.py` & `rdmo-1.9.2/rdmo/accounts/tests/test_viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/urls/__init__.py` & `rdmo-1.9.2/rdmo/accounts/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/utils.py` & `rdmo-1.9.2/rdmo/accounts/utils.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/views.py` & `rdmo-1.9.2/rdmo/accounts/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/accounts/viewsets.py` & `rdmo-1.9.2/rdmo/accounts/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/admin.py` & `rdmo-1.9.2/rdmo/conditions/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/imports.py` & `rdmo-1.9.2/rdmo/conditions/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0001_initial.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0003_meta.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0003_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0005_empty_relation.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0005_empty_relation.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0006_db_constraint_false.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0006_db_constraint_false.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0008_validator.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0008_validator.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0009_options.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0009_options.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0010_refactoring.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0010_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0011_refactoring.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0011_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0012_permissions.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0012_permissions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0013_meta.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0013_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0014_meta.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0014_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0015_move_attribute_to_attributeentity.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0015_move_attribute_to_attributeentity.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0016_meta.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0016_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0017_data_migration.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0017_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0018_remove_null_true.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0018_remove_null_true.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0020_require_uri_prefix.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0020_require_uri_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/migrations/0021_related_name.py` & `rdmo-1.9.2/rdmo/conditions/migrations/0021_related_name.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/models.py` & `rdmo-1.9.2/rdmo/conditions/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/renderers.py` & `rdmo-1.9.2/rdmo/conditions/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/serializers/export.py` & `rdmo-1.9.2/rdmo/conditions/serializers/export.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/serializers/v1.py` & `rdmo-1.9.2/rdmo/conditions/serializers/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/static/conditions/js/conditions.js` & `rdmo-1.9.2/rdmo/conditions/static/conditions/js/conditions.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions.html` & `rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_export.html` & `rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_export.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_modal_delete_conditions.html` & `rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_modal_delete_conditions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_modal_form_conditions.html` & `rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_modal_form_conditions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/templates/conditions/conditions_modal_show_conditions.html` & `rdmo-1.9.2/rdmo/conditions/templates/conditions/conditions_modal_show_conditions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/tests/test_models.py` & `rdmo-1.9.2/rdmo/conditions/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/tests/test_validator_locked.py` & `rdmo-1.9.2/rdmo/conditions/tests/test_validator_locked.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/tests/test_validator_unique_uri.py` & `rdmo-1.9.2/rdmo/conditions/tests/test_validator_unique_uri.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/tests/test_views.py` & `rdmo-1.9.2/rdmo/conditions/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/tests/test_viewset_condition.py` & `rdmo-1.9.2/rdmo/conditions/tests/test_viewset_condition.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/tests/test_viewset_relation.py` & `rdmo-1.9.2/rdmo/conditions/tests/test_viewset_relation.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/validators.py` & `rdmo-1.9.2/rdmo/conditions/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/views.py` & `rdmo-1.9.2/rdmo/conditions/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/conditions/viewsets.py` & `rdmo-1.9.2/rdmo/conditions/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/constants.py` & `rdmo-1.9.2/rdmo/core/constants.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/imports.py` & `rdmo-1.9.2/rdmo/core/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/mail.py` & `rdmo-1.9.2/rdmo/core/mail.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/delete_users.py` & `rdmo-1.9.2/rdmo/core/management/commands/delete_users.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/download_vendor_files.py` & `rdmo-1.9.2/rdmo/core/management/commands/download_vendor_files.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/find_inactive_users.py` & `rdmo-1.9.2/rdmo/core/management/commands/find_inactive_users.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/find_spam_users.py` & `rdmo-1.9.2/rdmo/core/management/commands/find_spam_users.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/find_users.py` & `rdmo-1.9.2/rdmo/core/management/commands/find_users.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/make_theme.py` & `rdmo-1.9.2/rdmo/core/management/commands/make_theme.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/set_uri_prefix.py` & `rdmo-1.9.2/rdmo/core/management/commands/set_uri_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/setup_groups.py` & `rdmo-1.9.2/rdmo/core/management/commands/setup_groups.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/management/commands/upgrade.py` & `rdmo-1.9.2/rdmo/core/management/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/managers.py` & `rdmo-1.9.2/rdmo/core/managers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/models.py` & `rdmo-1.9.2/rdmo/core/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/permissions.py` & `rdmo-1.9.2/rdmo/core/permissions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/plugins.py` & `rdmo-1.9.2/rdmo/core/plugins.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/renderers.py` & `rdmo-1.9.2/rdmo/core/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/serializers.py` & `rdmo-1.9.2/rdmo/core/serializers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/settings.py` & `rdmo-1.9.2/rdmo/core/settings.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/css/base.scss` & `rdmo-1.9.2/rdmo/core/static/core/css/base.scss`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/css/fonts.scss` & `rdmo-1.9.2/rdmo/core/static/core/css/fonts.scss`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/css/footer.scss` & `rdmo-1.9.2/rdmo/core/static/core/css/footer.scss`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/css/header.scss` & `rdmo-1.9.2/rdmo/core/static/core/css/header.scss`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/css/swagger.scss` & `rdmo-1.9.2/rdmo/core/static/core/css/swagger.scss`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/css/variables.scss` & `rdmo-1.9.2/rdmo/core/static/core/css/variables.scss`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSans-Bold.ttf` & `rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSans.ttf` & `rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSansMono.ttf` & `rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif-Bold.ttf` & `rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif-BoldItalic.ttf` & `rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif-Italic.ttf` & `rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/fonts/DroidSerif.ttf` & `rdmo-1.9.2/rdmo/core/static/core/fonts/DroidSerif.ttf`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/html/formgroup_select.html` & `rdmo-1.9.2/rdmo/core/static/core/html/formgroup_select.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/html/formgroup_selectmultiple.html` & `rdmo-1.9.2/rdmo/core/static/core/html/formgroup_selectmultiple.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/html/formgroup_selectnumber.html` & `rdmo-1.9.2/rdmo/core/static/core/html/formgroup_selectnumber.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/img/favicon.png` & `rdmo-1.9.2/rdmo/core/static/core/img/favicon.png`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/img/header/collection.jpg` & `rdmo-1.9.2/rdmo/core/static/core/img/header/collection.jpg`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/img/header/library.jpg` & `rdmo-1.9.2/rdmo/core/static/core/img/header/library.jpg`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/img/header/supercomputer.jpg` & `rdmo-1.9.2/rdmo/core/static/core/img/header/supercomputer.jpg`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/img/rdmo-logo.svg` & `rdmo-1.9.2/rdmo/core/static/core/img/rdmo-logo.svg`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/static/core/js/core.js` & `rdmo-1.9.2/rdmo/core/static/core/js/core.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/swagger.py` & `rdmo-1.9.2/rdmo/core/swagger.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/about_text_de.html` & `rdmo-1.9.2/rdmo/core/templates/core/about_text_de.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/about_text_en.html` & `rdmo-1.9.2/rdmo/core/templates/core/about_text_en.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/about_text_fr.html` & `rdmo-1.9.2/rdmo/core/templates/core/about_text_fr.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/about_text_it.html` & `rdmo-1.9.2/rdmo/core/templates/core/about_text_it.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/base.html` & `rdmo-1.9.2/rdmo/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/base_head.html` & `rdmo-1.9.2/rdmo/core/templates/core/base_head.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/base_navigation.html` & `rdmo-1.9.2/rdmo/core/templates/core/base_navigation.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/bootstrap_form_field.html` & `rdmo-1.9.2/rdmo/core/templates/core/bootstrap_form_field.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/footer_text_de.html` & `rdmo-1.9.2/rdmo/core/templates/core/footer_text_de.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/footer_text_en.html` & `rdmo-1.9.2/rdmo/core/templates/core/footer_text_en.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/footer_text_fr.html` & `rdmo-1.9.2/rdmo/core/templates/core/footer_text_fr.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/footer_text_it.html` & `rdmo-1.9.2/rdmo/core/templates/core/footer_text_it.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/home.html` & `rdmo-1.9.2/rdmo/core/templates/core/home.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/home_text_de.html` & `rdmo-1.9.2/rdmo/core/templates/core/home_text_de.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/home_text_en.html` & `rdmo-1.9.2/rdmo/core/templates/core/home_text_en.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/home_text_fr.html` & `rdmo-1.9.2/rdmo/core/templates/core/home_text_fr.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/home_text_it.html` & `rdmo-1.9.2/rdmo/core/templates/core/home_text_it.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/core/upload_form.html` & `rdmo-1.9.2/rdmo/core/templates/core/upload_form.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templates/rest_framework_swagger/index.html` & `rdmo-1.9.2/rdmo/core/templates/rest_framework_swagger/index.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/templatetags/core_tags.py` & `rdmo-1.9.2/rdmo/core/templatetags/core_tags.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/tests/test_mail.py` & `rdmo-1.9.2/rdmo/core/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/tests/test_tags.py` & `rdmo-1.9.2/rdmo/core/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/tests/test_utils.py` & `rdmo-1.9.2/rdmo/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/tests/test_validators.py` & `rdmo-1.9.2/rdmo/core/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/tests/test_views.py` & `rdmo-1.9.2/rdmo/core/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/tests/test_viewset_settings.py` & `rdmo-1.9.2/rdmo/core/tests/test_viewset_settings.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/tests/test_xml.py` & `rdmo-1.9.2/rdmo/core/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/urls/__init__.py` & `rdmo-1.9.2/rdmo/core/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/urls/v1.py` & `rdmo-1.9.2/rdmo/core/urls/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/utils.py` & `rdmo-1.9.2/rdmo/core/utils.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/validators.py` & `rdmo-1.9.2/rdmo/core/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/views.py` & `rdmo-1.9.2/rdmo/core/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/viewsets.py` & `rdmo-1.9.2/rdmo/core/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/core/xml.py` & `rdmo-1.9.2/rdmo/core/xml.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/admin.py` & `rdmo-1.9.2/rdmo/domain/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/imports.py` & `rdmo-1.9.2/rdmo/domain/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0001_initial_after_reset.py` & `rdmo-1.9.2/rdmo/domain/migrations/0001_initial_after_reset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0003_condition.py` & `rdmo-1.9.2/rdmo/domain/migrations/0003_condition.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0004_verbosename.py` & `rdmo-1.9.2/rdmo/domain/migrations/0004_verbosename.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0006_attributeentity_parent_collection.py` & `rdmo-1.9.2/rdmo/domain/migrations/0006_attributeentity_parent_collection.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0008_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0008_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0009_remove_condition.py` & `rdmo-1.9.2/rdmo/domain/migrations/0009_remove_condition.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0010_many_to_many_for_conditions.py` & `rdmo-1.9.2/rdmo/domain/migrations/0010_many_to_many_for_conditions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0013_mptt.py` & `rdmo-1.9.2/rdmo/domain/migrations/0013_mptt.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0015_label.py` & `rdmo-1.9.2/rdmo/domain/migrations/0015_label.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0017_url_value_type.py` & `rdmo-1.9.2/rdmo/domain/migrations/0017_url_value_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0018_validator.py` & `rdmo-1.9.2/rdmo/domain/migrations/0018_validator.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0019_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0019_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0020_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0020_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0024_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0024_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0025_refactoring.py` & `rdmo-1.9.2/rdmo/domain/migrations/0025_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0026_refactoring.py` & `rdmo-1.9.2/rdmo/domain/migrations/0026_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0029_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0029_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0030_permissions.py` & `rdmo-1.9.2/rdmo/domain/migrations/0030_permissions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0031_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0031_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0032_remove_unit_and_type.py` & `rdmo-1.9.2/rdmo/domain/migrations/0032_remove_unit_and_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0035_remove_is_collection_and_parent_collection.py` & `rdmo-1.9.2/rdmo/domain/migrations/0035_remove_is_collection_and_parent_collection.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0036_remove_range_and_verbosename.py` & `rdmo-1.9.2/rdmo/domain/migrations/0036_remove_range_and_verbosename.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0037_remove_attribute.py` & `rdmo-1.9.2/rdmo/domain/migrations/0037_remove_attribute.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0039_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0039_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0040_meta.py` & `rdmo-1.9.2/rdmo/domain/migrations/0040_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0041_data_migration.py` & `rdmo-1.9.2/rdmo/domain/migrations/0041_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0042_remove_null_true.py` & `rdmo-1.9.2/rdmo/domain/migrations/0042_remove_null_true.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0043_django2.py` & `rdmo-1.9.2/rdmo/domain/migrations/0043_django2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0044_mptt.py` & `rdmo-1.9.2/rdmo/domain/migrations/0044_mptt.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0045_require_uri_prefix.py` & `rdmo-1.9.2/rdmo/domain/migrations/0045_require_uri_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/migrations/0046_parent_cascade.py` & `rdmo-1.9.2/rdmo/domain/migrations/0046_parent_cascade.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/models.py` & `rdmo-1.9.2/rdmo/domain/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/renderers.py` & `rdmo-1.9.2/rdmo/domain/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/serializers/v1.py` & `rdmo-1.9.2/rdmo/domain/serializers/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,10 +126,11 @@
 class AttributeIndexSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = Attribute
         fields = (
             'id',
             'uri',
+            'uri_prefix',
             'key',
             'path'
         )
```

### Comparing `rdmo-1.9.1/rdmo/domain/static/domain/js/domain.js` & `rdmo-1.9.2/rdmo/domain/static/domain/js/domain.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/templates/domain/domain.html` & `rdmo-1.9.2/rdmo/domain/templates/domain/domain.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/templates/domain/domain_modal_delete_attributes.html` & `rdmo-1.9.2/rdmo/domain/templates/domain/domain_modal_delete_attributes.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/templates/domain/domain_modal_form_attributes.html` & `rdmo-1.9.2/rdmo/domain/templates/domain/domain_modal_form_attributes.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/templates/domain/domain_modal_show_attributes.html` & `rdmo-1.9.2/rdmo/domain/templates/domain/domain_modal_show_attributes.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/templates/domain/domain_options.html` & `rdmo-1.9.2/rdmo/domain/templates/domain/domain_options.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/tests/test_models.py` & `rdmo-1.9.2/rdmo/domain/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/tests/test_validator_locked.py` & `rdmo-1.9.2/rdmo/domain/tests/test_validator_locked.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/tests/test_validator_parent.py` & `rdmo-1.9.2/rdmo/domain/tests/test_validator_parent.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/tests/test_validator_unique_uri.py` & `rdmo-1.9.2/rdmo/domain/tests/test_validator_unique_uri.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/tests/test_views.py` & `rdmo-1.9.2/rdmo/domain/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/tests/test_viewset_attribute.py` & `rdmo-1.9.2/rdmo/domain/tests/test_viewset_attribute.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/validators.py` & `rdmo-1.9.2/rdmo/domain/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/views.py` & `rdmo-1.9.2/rdmo/domain/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/domain/viewsets.py` & `rdmo-1.9.2/rdmo/domain/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/de/LC_MESSAGES/django.mo` & `rdmo-1.9.2/rdmo/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/de/LC_MESSAGES/django.po` & `rdmo-1.9.2/rdmo/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/es/LC_MESSAGES/django.mo` & `rdmo-1.9.2/rdmo/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/es/LC_MESSAGES/django.po` & `rdmo-1.9.2/rdmo/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/fr/LC_MESSAGES/django.mo` & `rdmo-1.9.2/rdmo/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/fr/LC_MESSAGES/django.po` & `rdmo-1.9.2/rdmo/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/it/LC_MESSAGES/django.mo` & `rdmo-1.9.2/rdmo/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/it/LC_MESSAGES/django.po` & `rdmo-1.9.2/rdmo/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/locale/nl/LC_MESSAGES/django.po` & `rdmo-1.9.2/rdmo/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/imports.py` & `rdmo-1.9.2/rdmo/management/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/management/commands/import.py` & `rdmo-1.9.2/rdmo/management/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/templates/management/import.html` & `rdmo-1.9.2/rdmo/management/templates/management/import.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/templates/management/upload.html` & `rdmo-1.9.2/rdmo/management/templates/management/upload.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/tests/test_commands.py` & `rdmo-1.9.2/rdmo/management/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/tests/test_import.py` & `rdmo-1.9.2/rdmo/management/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/tests/test_views.py` & `rdmo-1.9.2/rdmo/management/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/management/views.py` & `rdmo-1.9.2/rdmo/management/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/admin.py` & `rdmo-1.9.2/rdmo/options/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/imports.py` & `rdmo-1.9.2/rdmo/options/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0001_initial.py` & `rdmo-1.9.2/rdmo/options/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0002_meta.py` & `rdmo-1.9.2/rdmo/options/migrations/0002_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0003_data_migration.py` & `rdmo-1.9.2/rdmo/options/migrations/0003_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0004_conditions.py` & `rdmo-1.9.2/rdmo/options/migrations/0004_conditions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0005_refactoring.py` & `rdmo-1.9.2/rdmo/options/migrations/0005_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0006_refactoring.py` & `rdmo-1.9.2/rdmo/options/migrations/0006_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0007_meta.py` & `rdmo-1.9.2/rdmo/options/migrations/0007_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0008_option_path.py` & `rdmo-1.9.2/rdmo/options/migrations/0008_option_path.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0009_data_migration.py` & `rdmo-1.9.2/rdmo/options/migrations/0009_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0010_meta.py` & `rdmo-1.9.2/rdmo/options/migrations/0010_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0011_permissions.py` & `rdmo-1.9.2/rdmo/options/migrations/0011_permissions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0012_meta.py` & `rdmo-1.9.2/rdmo/options/migrations/0012_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0013_order.py` & `rdmo-1.9.2/rdmo/options/migrations/0013_order.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0016_meta.py` & `rdmo-1.9.2/rdmo/options/migrations/0016_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0017_add_language_fields.py` & `rdmo-1.9.2/rdmo/options/migrations/0017_add_language_fields.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0018_data_migration.py` & `rdmo-1.9.2/rdmo/options/migrations/0018_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0019_remove_null_true.py` & `rdmo-1.9.2/rdmo/options/migrations/0019_remove_null_true.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0020_django2.py` & `rdmo-1.9.2/rdmo/options/migrations/0020_django2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0021_data_migrations.py` & `rdmo-1.9.2/rdmo/options/migrations/0021_data_migrations.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0022_cascade_options.py` & `rdmo-1.9.2/rdmo/options/migrations/0022_cascade_options.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0023_require_uri_prefix.py` & `rdmo-1.9.2/rdmo/options/migrations/0023_require_uri_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0024_related_name.py` & `rdmo-1.9.2/rdmo/options/migrations/0024_related_name.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0025_optionset_provider_key.py` & `rdmo-1.9.2/rdmo/options/migrations/0025_optionset_provider_key.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/migrations/0026_optionset_option_locked.py` & `rdmo-1.9.2/rdmo/options/migrations/0026_optionset_option_locked.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/models.py` & `rdmo-1.9.2/rdmo/options/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/providers.py` & `rdmo-1.9.2/rdmo/options/providers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/renderers.py` & `rdmo-1.9.2/rdmo/options/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/serializers/export.py` & `rdmo-1.9.2/rdmo/options/serializers/export.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/serializers/v1.py` & `rdmo-1.9.2/rdmo/options/serializers/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/static/options/js/options.js` & `rdmo-1.9.2/rdmo/options/static/options/js/options.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options.html` & `rdmo-1.9.2/rdmo/options/templates/options/options.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_export.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_export.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_modal_delete_options.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_modal_delete_options.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_modal_delete_optionsets.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_modal_delete_optionsets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_modal_form_conditions.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_modal_form_conditions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_modal_form_options.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_modal_form_options.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_modal_form_optionsets.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_modal_form_optionsets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_modal_show_options.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_modal_show_options.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/templates/options/options_modal_show_optionsets.html` & `rdmo-1.9.2/rdmo/options/templates/options/options_modal_show_optionsets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_models.py` & `rdmo-1.9.2/rdmo/options/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_validator_locked_options.py` & `rdmo-1.9.2/rdmo/options/tests/test_validator_locked_options.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_validator_locked_optionsets.py` & `rdmo-1.9.2/rdmo/options/tests/test_validator_locked_optionsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_validator_unique_uri_options.py` & `rdmo-1.9.2/rdmo/options/tests/test_validator_unique_uri_options.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_validator_unique_uri_optionsets.py` & `rdmo-1.9.2/rdmo/options/tests/test_validator_unique_uri_optionsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_views.py` & `rdmo-1.9.2/rdmo/options/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_viewset_options.py` & `rdmo-1.9.2/rdmo/options/tests/test_viewset_options.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/tests/test_viewset_optionsets.py` & `rdmo-1.9.2/rdmo/options/tests/test_viewset_optionsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/validators.py` & `rdmo-1.9.2/rdmo/options/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/views.py` & `rdmo-1.9.2/rdmo/options/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/options/viewsets.py` & `rdmo-1.9.2/rdmo/options/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/migrations/0001_initial.py` & `rdmo-1.9.2/rdmo/overlays/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/models.py` & `rdmo-1.9.2/rdmo/overlays/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/static/overlays/js/overlays.js` & `rdmo-1.9.2/rdmo/overlays/static/overlays/js/overlays.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/templates/overlays/reset_overlays.html` & `rdmo-1.9.2/rdmo/overlays/templates/overlays/reset_overlays.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/tests/test_views.py` & `rdmo-1.9.2/rdmo/overlays/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/tests/test_viewsets.py` & `rdmo-1.9.2/rdmo/overlays/tests/test_viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/views.py` & `rdmo-1.9.2/rdmo/overlays/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/overlays/viewsets.py` & `rdmo-1.9.2/rdmo/overlays/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/admin.py` & `rdmo-1.9.2/rdmo/projects/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/exports.py` & `rdmo-1.9.2/rdmo/projects/exports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/filters.py` & `rdmo-1.9.2/rdmo/projects/filters.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/forms.py` & `rdmo-1.9.2/rdmo/projects/forms.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/handlers.py` & `rdmo-1.9.2/rdmo/projects/handlers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/imports.py` & `rdmo-1.9.2/rdmo/projects/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/management/commands/delete_projects.py` & `rdmo-1.9.2/rdmo/projects/management/commands/delete_projects.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/management/commands/export_projects.py` & `rdmo-1.9.2/rdmo/projects/management/commands/export_projects.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/management/commands/find_inactive_projects.py` & `rdmo-1.9.2/rdmo/projects/management/commands/find_inactive_projects.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/management/commands/prune_projects.py` & `rdmo-1.9.2/rdmo/projects/management/commands/prune_projects.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/managers.py` & `rdmo-1.9.2/rdmo/projects/managers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0001_initial_after_reset.py` & `rdmo-1.9.2/rdmo/projects/migrations/0001_initial_after_reset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0002_meta.py` & `rdmo-1.9.2/rdmo/projects/migrations/0002_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0004_remove_current_snapshot.py` & `rdmo-1.9.2/rdmo/projects/migrations/0004_remove_current_snapshot.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0005_snapshot.py` & `rdmo-1.9.2/rdmo/projects/migrations/0005_snapshot.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0006_project_values.py` & `rdmo-1.9.2/rdmo/projects/migrations/0006_project_values.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0007_data_migration.py` & `rdmo-1.9.2/rdmo/projects/migrations/0007_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0008_not_null.py` & `rdmo-1.9.2/rdmo/projects/migrations/0008_not_null.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0009_options.py` & `rdmo-1.9.2/rdmo/projects/migrations/0009_options.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0010_add_db_contraint.py` & `rdmo-1.9.2/rdmo/projects/migrations/0010_add_db_contraint.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0011_refactoring.py` & `rdmo-1.9.2/rdmo/projects/migrations/0011_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0012_membership.py` & `rdmo-1.9.2/rdmo/projects/migrations/0012_membership.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0013_data_migration.py` & `rdmo-1.9.2/rdmo/projects/migrations/0013_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0015_permissions.py` & `rdmo-1.9.2/rdmo/projects/migrations/0015_permissions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0016_catalog_on_delete.py` & `rdmo-1.9.2/rdmo/projects/migrations/0016_catalog_on_delete.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0017_value_unit_and_type.py` & `rdmo-1.9.2/rdmo/projects/migrations/0017_value_unit_and_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0018_data_migration.py` & `rdmo-1.9.2/rdmo/projects/migrations/0018_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0019_option.py` & `rdmo-1.9.2/rdmo/projects/migrations/0019_option.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0020_data_migration.py` & `rdmo-1.9.2/rdmo/projects/migrations/0020_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0021_order.py` & `rdmo-1.9.2/rdmo/projects/migrations/0021_order.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0022_move_attribute_to_attributeentity.py` & `rdmo-1.9.2/rdmo/projects/migrations/0022_move_attribute_to_attributeentity.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0023_meta.py` & `rdmo-1.9.2/rdmo/projects/migrations/0023_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0024_data_migration.py` & `rdmo-1.9.2/rdmo/projects/migrations/0024_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0026_django2.py` & `rdmo-1.9.2/rdmo/projects/migrations/0026_django2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0027_project_site.py` & `rdmo-1.9.2/rdmo/projects/migrations/0027_project_site.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0028_meta.py` & `rdmo-1.9.2/rdmo/projects/migrations/0028_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0030_project_views.py` & `rdmo-1.9.2/rdmo/projects/migrations/0030_project_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0031_project_tasks.py` & `rdmo-1.9.2/rdmo/projects/migrations/0031_project_tasks.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0032_data_migration.py` & `rdmo-1.9.2/rdmo/projects/migrations/0032_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0033_default_value_type.py` & `rdmo-1.9.2/rdmo/projects/migrations/0033_default_value_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0034_issue.py` & `rdmo-1.9.2/rdmo/projects/migrations/0034_issue.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0035_data_migration.py` & `rdmo-1.9.2/rdmo/projects/migrations/0035_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0037_project_tasks.py` & `rdmo-1.9.2/rdmo/projects/migrations/0037_project_tasks.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0038_integration_integrationoption.py` & `rdmo-1.9.2/rdmo/projects/migrations/0038_integration_integrationoption.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0039_integrationoption_secret.py` & `rdmo-1.9.2/rdmo/projects/migrations/0039_integrationoption_secret.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0040_issueresource.py` & `rdmo-1.9.2/rdmo/projects/migrations/0040_issueresource.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0042_allow_site_null.py` & `rdmo-1.9.2/rdmo/projects/migrations/0042_allow_site_null.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0043_meta.py` & `rdmo-1.9.2/rdmo/projects/migrations/0043_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0044_meta.py` & `rdmo-1.9.2/rdmo/projects/migrations/0044_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0045_value_file.py` & `rdmo-1.9.2/rdmo/projects/migrations/0045_value_file.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0046_project_mptt.py` & `rdmo-1.9.2/rdmo/projects/migrations/0046_project_mptt.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0047_continuation.py` & `rdmo-1.9.2/rdmo/projects/migrations/0047_continuation.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0048_meta.py` & `rdmo-1.9.2/rdmo/projects/migrations/0048_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0049_invite.py` & `rdmo-1.9.2/rdmo/projects/migrations/0049_invite.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0050_value_set_prefix.py` & `rdmo-1.9.2/rdmo/projects/migrations/0050_value_set_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0051_alter_value_value_type.py` & `rdmo-1.9.2/rdmo/projects/migrations/0051_alter_value_value_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/migrations/0052_meta.py` & `rdmo-1.9.2/rdmo/projects/migrations/0052_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/mixins.py` & `rdmo-1.9.2/rdmo/projects/mixins.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/models/continuation.py` & `rdmo-1.9.2/rdmo/projects/models/continuation.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/models/integration.py` & `rdmo-1.9.2/rdmo/projects/models/integration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/models/invite.py` & `rdmo-1.9.2/rdmo/projects/models/invite.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,17 +56,17 @@
         super().save(*args, **kwargs)
 
     def get_absolute_url(self):
         return reverse('project', kwargs={'pk': self.project.pk})
 
     @property
     def is_expired(self):
-        if settings.PROJECT_INVITE_TIMEOUT is None:
-            return False
-        else:
+        if settings.PROJECT_INVITE_TIMEOUT:
             return (now() - self.timestamp).total_seconds() > settings.PROJECT_INVITE_TIMEOUT
+        else:
+            return False
 
     def make_token(self):
         self.token = salted_hmac(self.key_salt, self._make_hash_value()).hexdigest()[::2]
 
     def _make_hash_value(self):
         return str(self.project_id) + str(self.email) + str(self.role) + str(self.timestamp)
```

### Comparing `rdmo-1.9.1/rdmo/projects/models/issue.py` & `rdmo-1.9.2/rdmo/projects/models/issue.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/models/membership.py` & `rdmo-1.9.2/rdmo/projects/models/membership.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/models/project.py` & `rdmo-1.9.2/rdmo/projects/models/project.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/models/snapshot.py` & `rdmo-1.9.2/rdmo/projects/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/models/value.py` & `rdmo-1.9.2/rdmo/projects/models/value.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/providers.py` & `rdmo-1.9.2/rdmo/projects/providers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/renderers.py` & `rdmo-1.9.2/rdmo/projects/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/rules.py` & `rdmo-1.9.2/rdmo/projects/rules.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/serializers/export.py` & `rdmo-1.9.2/rdmo/projects/serializers/export.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/serializers/v1/__init__.py` & `rdmo-1.9.2/rdmo/projects/serializers/v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
             'snapshots',
             'parent',
             'owners',
             'managers',
             'authors',
             'guests',
             'created',
-            'updated'
+            'updated',
+            'site'
         )
         read_only_fields = (
             'snapshots',
         )
 
 
 class ProjectMembershipSerializer(serializers.ModelSerializer):
```

### Comparing `rdmo-1.9.1/rdmo/projects/serializers/v1/overview.py` & `rdmo-1.9.2/rdmo/projects/serializers/v1/overview.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/serializers/v1/questionset.py` & `rdmo-1.9.2/rdmo/projects/serializers/v1/questionset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/static/projects/css/project_questions.scss` & `rdmo-1.9.2/rdmo/projects/static/projects/css/project_questions.scss`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/static/projects/js/project_questions/directives.js` & `rdmo-1.9.2/rdmo/projects/static/projects/js/project_questions/directives.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/static/projects/js/project_questions/services.js` & `rdmo-1.9.2/rdmo/projects/static/projects/js/project_questions/services.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/email/project_invite_message.txt` & `rdmo-1.9.2/rdmo/projects/templates/projects/email/project_invite_message.txt`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/invite_confirm_delete.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/invite_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/issue_detail.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/issue_detail.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/issue_send.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/issue_send.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/issue_send_email.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/issue_send_email.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/issue_send_integrations.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/issue_send_integrations.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/membership_form.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/membership_form.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_de.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_de.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_en.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_en.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_fr.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_fr.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_issues_it.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_issues_it.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_questions_de.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_questions_de.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_questions_fr.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_questions_fr.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_de.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_de.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_en.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_en.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_fr.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_fr.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/project_project_views_it.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/project_project_views_it.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_de.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_de.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_en.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_en.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_fr.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_fr.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/overlays/projects_projects_table_it.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/overlays/projects_projects_table_it.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_answers.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_answers.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_answers_element.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_answers_element.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_confirm_delete.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_header.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_header.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_header_hierarchy.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_header_hierarchy.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 {% load i18n %}
+{% load rules %}
 {% load projects_tags %}
 
 {% if can_change_project %}
 <p class="pull-right">
     <a href="{% url 'project_update_parent' project.pk %}" title="{% trans 'Update parent project' %}">
         <i class="fa fa-pencil"></i>
     </a>
 </p>
 {% endif %}
 
 <ul class="list-unstyled">
 {% for node in project_tree %}
     <li>
         {% projects_indent node.level %}
-        <a href="{% url 'project' node.id %}">
-            {% if node.id == project.id %}
-            <strong>{{ node.title }}</strong>
-            {% else %}
-            {{ node.title }}
-            {% endif %}
-        </a>
+
+        {% has_perm 'projects.view_project_object' request.user node as can_view_parent_project %}
+        {% if can_view_parent_project %}
+           <a href="{% url 'project' node.id %}">
+                {% if node.id == project.id %}
+                <strong>{{ node.title }}</strong>
+                {% else %}
+                {{ node.title }}
+                {% endif %}
+            </a>
+        {% else %}
+        {{ node.title }}
+        {% endif %}
     </li>
 {% endfor %}
 </ul>
```

#### html2text {}

```diff
@@ -1,6 +1,10 @@
-{% load i18n %} {% load projects_tags %} {% if can_change_project %}
+{% load i18n %} {% load rules %} {% load projects_tags %} {% if
+can_change_project %}
 {% endif %}
     * {% for node in project_tree %}
-    * {% projects_indent node.level %} {%_if_node.id_==_project.id_%}_{
-      {_node.title_}}_{%_else_%}_{{_node.title_}}_{%_endif_%}
+    * {% projects_indent node.level %} {% has_perm
+      'projects.view_project_object' request.user node as
+      can_view_parent_project %} {% if can_view_parent_project %} {%_if_node.id
+      ==_project.id_%}_{{_node.title_}}_{%_else_%}_{{_node.title_}}_{%_endif_%}
+      {% else %} {{ node.title }} {% endif %}
     * {% endfor %}
```

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_integrations.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_integrations.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_invites.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_invites.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_issues.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_issues.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_memberships.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_memberships.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_sidebar.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_sidebar.html`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     <li>
         <p>
             <strong>{% trans 'Import from file' %}</strong>
         </p>
         {% url 'project_update_import' project.id as upload_url %}
         {% include 'core/upload_form.html' with upload_url=upload_url label=True %}
     </li>
-    {% if settings.NESTED_PROJECTS and project.get_ancestors %}
+    {% if settings.NESTED_PROJECTS and ancestors_import %}
     <li>
         <p>
             <strong>{% trans 'Import from parent project' %}</strong>
         </p>
         {% include 'projects/project_detail_sidebar_parent_import.html' %}
     </li>
     {% endif %}
```

#### html2text {}

```diff
@@ -45,15 +45,15 @@
 {% endif %} {% has_perm 'projects.import_project_object' request.user project
 as can_import_project %} {% if settings.PROJECT_IMPORTS and can_import_project
 %}
 ***** {% trans 'Import values' %} *****
     * {% trans 'Import from file' %}
       {% url 'project_update_import' project.id as upload_url %} {% include
       'core/upload_form.html' with upload_url=upload_url label=True %}
-    * {% if settings.NESTED_PROJECTS and project.get_ancestors %}
+    * {% if settings.NESTED_PROJECTS and ancestors_import %}
     * {% trans 'Import from parent project' %}
       {% include 'projects/project_detail_sidebar_parent_import.html' %}
     * {% endif %} {% if settings.PROJECT_IMPORTS_LIST %}
     * {% trans 'Import directly' %}
     * {% for key, label, class in settings.PROJECT_IMPORTS %} {% if key in
       settings.PROJECT_IMPORTS_LIST %}
     * {{_label_}}
```

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_sidebar_parent_import.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_sidebar_parent_import.html`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <form class="sidebar-form" action="{% url 'project_update_import' project.id %}" method="post">
     {% csrf_token %}
 
     <input type="hidden" name="method" value="import_project">
 
     <select class="form-control" name="source">
-        {% for project in project.get_ancestors %}
+        {% for project in ancestors_import %}
         <option value="{{ project.id }}">{{ project.title }}</option>
         {% endfor %}
     </select>
 
     <div class="sidebar-form-button">
         <button class="btn btn-primary" type="submit" title="{% trans 'Import' %}">
             <i class="fa fa-arrow-right"></i>
```

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_snapshots.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_snapshots.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_detail_views.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_detail_views.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_error.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_error.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_form.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_form.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_import.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_import.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_buttons.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_buttons.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_element.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_element.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_autocomplete.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_autocomplete.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_checkbox.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_checkbox.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_date.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_date.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_file.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_file.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_radio.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_radio.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_range.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_range.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_select.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_select.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_text.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_text.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_textarea.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_textarea.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_form_group_yesno.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_form_group_yesno.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_modal_delete_valuesets.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_modal_delete_valuesets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_modal_form_valuesets.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_modal_form_valuesets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_navigation.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_navigation.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_questionset_head.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_questionset_head.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_questions_remove_field.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_questions_remove_field.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/project_view.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/project_view.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/projects.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/projects.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/projects_pagination.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/projects_pagination.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templates/projects/site_projects.html` & `rdmo-1.9.2/rdmo/projects/templates/projects/site_projects.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/templatetags/projects_tags.py` & `rdmo-1.9.2/rdmo/projects/templatetags/projects_tags.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_commands.py` & `rdmo-1.9.2/rdmo/projects/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_handlers.py` & `rdmo-1.9.2/rdmo/projects/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_models.py` & `rdmo-1.9.2/rdmo/projects/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_integration.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_integration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_issue.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_issue.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_membership.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_membership.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_project.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_project.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_project_create_import.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_project_create_import.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_project_join.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_project_join.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models import Invite, Membership, Project
 
 membership_roles = ('owner', 'manager', 'author', 'guest')
 
 
 @pytest.fixture()
 def use_project_invite_timeout(settings):
-    settings.PROJECT_INVITE_TIMEOUT = 0
+    settings.PROJECT_INVITE_TIMEOUT = -1
 
 
 @pytest.mark.parametrize('membership_role', membership_roles)
 def test_project_join(db, client, membership_role):
     client.login(username='user', password='user')
 
     project = Project.objects.get(id=1)
```

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_project_leave.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_project_leave.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_project_update_import.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_project_update_import.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_view_snapshot.py` & `rdmo-1.9.2/rdmo/projects/tests/test_view_snapshot.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_integration.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_integration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_issue.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_issue.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_membership.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_membership.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_project.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_project.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_integration.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_integration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_issue.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_issue.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_membership.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_membership.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_questionset.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_questionset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_snapshot.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_snapshot.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_project_value.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_project_value.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_snapshot.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_snapshot.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/tests/test_viewset_value.py` & `rdmo-1.9.2/rdmo/projects/tests/test_viewset_value.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/urls/__init__.py` & `rdmo-1.9.2/rdmo/projects/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/urls/v1.py` & `rdmo-1.9.2/rdmo/projects/urls/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/validators.py` & `rdmo-1.9.2/rdmo/projects/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/__init__.py` & `rdmo-1.9.2/rdmo/projects/views/__init__.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/integration.py` & `rdmo-1.9.2/rdmo/projects/views/integration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/invite.py` & `rdmo-1.9.2/rdmo/projects/views/invite.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/issue.py` & `rdmo-1.9.2/rdmo/projects/views/issue.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/membership.py` & `rdmo-1.9.2/rdmo/projects/views/membership.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from rdmo.accounts.utils import is_site_manager
 from rdmo.core.mail import send_mail
 from rdmo.core.views import ObjectPermissionMixin, RedirectViewMixin
 
 from ..forms import MembershipCreateForm
 from ..models import Membership, Project
-from ..utils import is_last_owner
+from ..utils import is_last_owner, get_invite_email_project_path
 
 logger = logging.getLogger(__name__)
 
 
 class MembershipCreateView(ObjectPermissionMixin, RedirectViewMixin, FormView):
     model = Membership
     form_class = MembershipCreateForm
@@ -44,16 +44,18 @@
 
     def get_success_url(self):
         return self.project.get_absolute_url()
 
     def form_valid(self, form):
         invite = form.save()
         if invite is not None:
+            
+            project_invite_path = get_invite_email_project_path(invite)
             context = {
-                'invite_url': self.request.build_absolute_uri(reverse('project_join', args=[invite.token])),
+                'invite_url': self.request.build_absolute_uri(project_invite_path),
                 'invite_user': invite.user,
                 'project': invite.project,
                 'user': self.request.user,
                 'site': Site.objects.get_current()
             }
 
             subject = render_to_string('projects/email/project_invite_subject.txt', context)
```

### Comparing `rdmo-1.9.1/rdmo/projects/views/project.py` & `rdmo-1.9.2/rdmo/projects/views/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,22 +122,26 @@
                                                  .filter_catalog(self.object.catalog) \
                                                  .filter_group(self.request.user) \
                                                  .filter_availability(self.request.user).exists()
         context['views_available'] = View.objects.filter_current_site() \
                                                  .filter_catalog(self.object.catalog) \
                                                  .filter_group(self.request.user) \
                                                  .filter_availability(self.request.user).exists()
+        ancestors_import = []
+        for instance in ancestors.exclude(id=project.id):
+            if self.request.user.has_perm('projects.view_project_object', instance):
+                ancestors_import.append(instance)
+        context['ancestors_import'] = ancestors_import
         context['memberships'] = memberships.order_by('user__last_name', '-project__level')
         context['integrations'] = integrations.order_by('provider_key', '-project__level')
         context['providers'] = get_plugins('PROJECT_ISSUE_PROVIDERS')
         context['issues'] = [issue for issue in project.issues.all() if issue.resolve(values)]
         context['snapshots'] = project.snapshots.all()
         context['invites'] = project.invites.all()
         context['membership'] = Membership.objects.filter(project=project, user=self.request.user).first()
-
         return context
 
 
 class ProjectDeleteView(ObjectPermissionMixin, RedirectViewMixin, DeleteView):
     model = Project
     queryset = Project.objects.all()
     success_url = reverse_lazy('projects')
```

### Comparing `rdmo-1.9.1/rdmo/projects/views/project_answers.py` & `rdmo-1.9.2/rdmo/projects/views/project_answers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/project_create.py` & `rdmo-1.9.2/rdmo/projects/views/project_create.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/project_update.py` & `rdmo-1.9.2/rdmo/projects/views/project_update.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/project_view.py` & `rdmo-1.9.2/rdmo/projects/views/project_view.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/views/snapshot.py` & `rdmo-1.9.2/rdmo/projects/views/snapshot.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/viewsets.py` & `rdmo-1.9.2/rdmo/projects/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/projects/widgets.py` & `rdmo-1.9.2/rdmo/projects/widgets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/admin.py` & `rdmo-1.9.2/rdmo/questions/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/imports.py` & `rdmo-1.9.2/rdmo/questions/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/managers.py` & `rdmo-1.9.2/rdmo/questions/managers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0001_initial_after_reset.py` & `rdmo-1.9.2/rdmo/questions/migrations/0001_initial_after_reset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0002_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0002_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0004_full_title.py` & `rdmo-1.9.2/rdmo/questions/migrations/0004_full_title.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0005_label.py` & `rdmo-1.9.2/rdmo/questions/migrations/0005_label.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0006_auto_20160803_1619.py` & `rdmo-1.9.2/rdmo/questions/migrations/0006_auto_20160803_1619.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0007_refactoring.py` & `rdmo-1.9.2/rdmo/questions/migrations/0007_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0008_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0008_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0009_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0009_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0010_label.py` & `rdmo-1.9.2/rdmo/questions/migrations/0010_label.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0011_path.py` & `rdmo-1.9.2/rdmo/questions/migrations/0011_path.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0012_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0012_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0013_permissions.py` & `rdmo-1.9.2/rdmo/questions/migrations/0013_permissions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0014_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0014_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0015_question_unit_and_type.py` & `rdmo-1.9.2/rdmo/questions/migrations/0015_question_unit_and_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0016_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0016_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0017_question_optionsets.py` & `rdmo-1.9.2/rdmo/questions/migrations/0017_question_optionsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0018_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0018_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0019_questionentity_conditions.py` & `rdmo-1.9.2/rdmo/questions/migrations/0019_questionentity_conditions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0020_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0020_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0021_questionentity_is_collection.py` & `rdmo-1.9.2/rdmo/questions/migrations/0021_questionentity_is_collection.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0022_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0022_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0023_option.py` & `rdmo-1.9.2/rdmo/questions/migrations/0023_option.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0024_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0024_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0025_questionset_and_questionitem.py` & `rdmo-1.9.2/rdmo/questions/migrations/0025_questionset_and_questionitem.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0026_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0026_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0027_remove_question_entity_and_question.py` & `rdmo-1.9.2/rdmo/questions/migrations/0027_remove_question_entity_and_question.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0029_verbose_name_and_range.py` & `rdmo-1.9.2/rdmo/questions/migrations/0029_verbose_name_and_range.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0030_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0030_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0031_rename_attribute_entity_to_attribute.py` & `rdmo-1.9.2/rdmo/questions/migrations/0031_rename_attribute_entity_to_attribute.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0032_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0032_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0033_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0033_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0034_move_questionset_to_section.py` & `rdmo-1.9.2/rdmo/questions/migrations/0034_move_questionset_to_section.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0035_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0035_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0036_remove_subsection.py` & `rdmo-1.9.2/rdmo/questions/migrations/0036_remove_subsection.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0037_rename_en_to_lang1.py` & `rdmo-1.9.2/rdmo/questions/migrations/0037_rename_en_to_lang1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0038_rename_de_to_lang2.py` & `rdmo-1.9.2/rdmo/questions/migrations/0038_rename_de_to_lang2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0039_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0039_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0040_add_language_fields.py` & `rdmo-1.9.2/rdmo/questions/migrations/0040_add_language_fields.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0041_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0041_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0042_remove_null_true.py` & `rdmo-1.9.2/rdmo/questions/migrations/0042_remove_null_true.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0043_django2.py` & `rdmo-1.9.2/rdmo/questions/migrations/0043_django2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0044_require_uri_prefix.py` & `rdmo-1.9.2/rdmo/questions/migrations/0044_require_uri_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0045_catalog_sites.py` & `rdmo-1.9.2/rdmo/questions/migrations/0045_catalog_sites.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0046_catalog_groups.py` & `rdmo-1.9.2/rdmo/questions/migrations/0046_catalog_groups.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0047_manager.py` & `rdmo-1.9.2/rdmo/questions/migrations/0047_manager.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0048_catalog_help.py` & `rdmo-1.9.2/rdmo/questions/migrations/0048_catalog_help.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0050_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0050_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0053_related_name.py` & `rdmo-1.9.2/rdmo/questions/migrations/0053_related_name.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0054_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0054_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0055_catalog_locked.py` & `rdmo-1.9.2/rdmo/questions/migrations/0055_catalog_locked.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0057_question_default_text.py` & `rdmo-1.9.2/rdmo/questions/migrations/0057_question_default_text.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0058_question_default_option.py` & `rdmo-1.9.2/rdmo/questions/migrations/0058_question_default_option.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0059_question_default_external_id.py` & `rdmo-1.9.2/rdmo/questions/migrations/0059_question_default_external_id.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0060_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0060_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0062_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0062_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0063_questionset_questionset.py` & `rdmo-1.9.2/rdmo/questions/migrations/0063_questionset_questionset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0065_data_migration.py` & `rdmo-1.9.2/rdmo/questions/migrations/0065_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0066_alter_question_value_type.py` & `rdmo-1.9.2/rdmo/questions/migrations/0066_alter_question_value_type.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0067_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0067_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/migrations/0068_meta.py` & `rdmo-1.9.2/rdmo/questions/migrations/0068_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/models/catalog.py` & `rdmo-1.9.2/rdmo/questions/models/catalog.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/models/question.py` & `rdmo-1.9.2/rdmo/questions/models/question.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/models/questionset.py` & `rdmo-1.9.2/rdmo/questions/models/questionset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/models/section.py` & `rdmo-1.9.2/rdmo/questions/models/section.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/renderers.py` & `rdmo-1.9.2/rdmo/questions/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/serializers/export.py` & `rdmo-1.9.2/rdmo/questions/serializers/export.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/serializers/v1.py` & `rdmo-1.9.2/rdmo/questions/serializers/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/static/questions/js/catalogs.js` & `rdmo-1.9.2/rdmo/questions/static/questions/js/catalogs.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalog_tree.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalog_tree.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_element.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_element.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_catalogs.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_catalogs.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_questions.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_questions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_questionsets.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_questionsets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_delete_sections.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_delete_sections.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_catalogs.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_catalogs.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_questions.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_questions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_questionsets.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_questionsets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_modal_form_sections.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_modal_form_sections.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_catalog.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_catalog.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_questions.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_questions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_questionsets.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_questionsets.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_options_sections.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_options_sections.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_sidebar.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_sidebar.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/templates/questions/catalogs_sidebar_showuri_checkboxes.html` & `rdmo-1.9.2/rdmo/questions/templates/questions/catalogs_sidebar_showuri_checkboxes.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_admin.py` & `rdmo-1.9.2/rdmo/questions/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_models.py` & `rdmo-1.9.2/rdmo/questions/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_catalogs.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_catalogs.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_questions.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_questions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_questionsets.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_questionsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_locked_sections.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_locked_sections.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_catalogs.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_catalogs.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_questions.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_questions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_questionsets.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_questionsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_validator_unique_uri_sections.py` & `rdmo-1.9.2/rdmo/questions/tests/test_validator_unique_uri_sections.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_views.py` & `rdmo-1.9.2/rdmo/questions/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_viewset_catalog.py` & `rdmo-1.9.2/rdmo/questions/tests/test_viewset_catalog.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_viewset_question.py` & `rdmo-1.9.2/rdmo/questions/tests/test_viewset_question.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_viewset_questionset.py` & `rdmo-1.9.2/rdmo/questions/tests/test_viewset_questionset.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_viewset_section.py` & `rdmo-1.9.2/rdmo/questions/tests/test_viewset_section.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/tests/test_viewset_widgettype.py` & `rdmo-1.9.2/rdmo/questions/tests/test_viewset_widgettype.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/urls/v1.py` & `rdmo-1.9.2/rdmo/questions/urls/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/utils.py` & `rdmo-1.9.2/rdmo/questions/utils.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/validators.py` & `rdmo-1.9.2/rdmo/questions/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/views.py` & `rdmo-1.9.2/rdmo/questions/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/questions/viewsets.py` & `rdmo-1.9.2/rdmo/questions/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/services/providers.py` & `rdmo-1.9.2/rdmo/services/providers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/services/validators.py` & `rdmo-1.9.2/rdmo/services/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/services/views.py` & `rdmo-1.9.2/rdmo/services/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/share/reference.docx` & `rdmo-1.9.2/rdmo/share/reference.docx`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/share/reference.odt` & `rdmo-1.9.2/rdmo/share/reference.odt`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/admin.py` & `rdmo-1.9.2/rdmo/tasks/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/imports.py` & `rdmo-1.9.2/rdmo/tasks/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/managers.py` & `rdmo-1.9.2/rdmo/tasks/managers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0001_initial.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0002_many_to_many_for_conditions.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0002_many_to_many_for_conditions.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0004_refactoring.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0004_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0005_data_migration.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0005_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0009_timeframe.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0009_timeframe.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0010_meta.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0010_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0011_task_text.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0011_task_text.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0012_move_attribute_to_attributeentity.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0012_move_attribute_to_attributeentity.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0013_meta.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0013_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0014_move_timeframe_to_task.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0014_move_timeframe_to_task.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0015_data_migration.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0015_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0016_remove_timeframe.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0016_remove_timeframe.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0017_rename_en_to_lang1.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0017_rename_en_to_lang1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0018_rename_de_to_lang2.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0018_rename_de_to_lang2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0019_meta.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0019_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0020_add_language_fields.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0020_add_language_fields.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0021_data_migration.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0021_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0022_remove_null_true.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0022_remove_null_true.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0024_require_uri_prefix.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0024_require_uri_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0025_task_sites.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0025_task_sites.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0026_task_groups.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0026_task_groups.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0028_data_migration.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0028_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0031_related_name.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0031_related_name.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/migrations/0032_task_catalogs.py` & `rdmo-1.9.2/rdmo/tasks/migrations/0032_task_catalogs.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/models.py` & `rdmo-1.9.2/rdmo/tasks/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/renderers.py` & `rdmo-1.9.2/rdmo/tasks/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/serializers/export.py` & `rdmo-1.9.2/rdmo/tasks/serializers/export.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/serializers/v1.py` & `rdmo-1.9.2/rdmo/tasks/serializers/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/static/tasks/js/tasks.js` & `rdmo-1.9.2/rdmo/tasks/static/tasks/js/tasks.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks.html` & `rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_export.html` & `rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_export.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_delete_tasks.html` & `rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_delete_tasks.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_form_conditions.html` & `rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_form_conditions.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_form_tasks.html` & `rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_form_tasks.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/templates/tasks/tasks_modal_form_timeframes.html` & `rdmo-1.9.2/rdmo/tasks/templates/tasks/tasks_modal_form_timeframes.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/tests/test_models.py` & `rdmo-1.9.2/rdmo/tasks/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/tests/test_validator_locked.py` & `rdmo-1.9.2/rdmo/tasks/tests/test_validator_locked.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/tests/test_validator_unique_uri.py` & `rdmo-1.9.2/rdmo/tasks/tests/test_validator_unique_uri.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/tests/test_views.py` & `rdmo-1.9.2/rdmo/tasks/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/tests/test_viewset_task.py` & `rdmo-1.9.2/rdmo/tasks/tests/test_viewset_task.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/validators.py` & `rdmo-1.9.2/rdmo/tasks/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/views.py` & `rdmo-1.9.2/rdmo/tasks/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/tasks/viewsets.py` & `rdmo-1.9.2/rdmo/tasks/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/admin.py` & `rdmo-1.9.2/rdmo/views/admin.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/imports.py` & `rdmo-1.9.2/rdmo/views/imports.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/managers.py` & `rdmo-1.9.2/rdmo/views/managers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0001_initial.py` & `rdmo-1.9.2/rdmo/views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0003_refactoring.py` & `rdmo-1.9.2/rdmo/views/migrations/0003_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0004_refactoring.py` & `rdmo-1.9.2/rdmo/views/migrations/0004_refactoring.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0005_meta.py` & `rdmo-1.9.2/rdmo/views/migrations/0005_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0006_title_and_help.py` & `rdmo-1.9.2/rdmo/views/migrations/0006_title_and_help.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0007_data_migration.py` & `rdmo-1.9.2/rdmo/views/migrations/0007_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0009_meta.py` & `rdmo-1.9.2/rdmo/views/migrations/0009_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0010_rename_en_to_lang1.py` & `rdmo-1.9.2/rdmo/views/migrations/0010_rename_en_to_lang1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0011_rename_de_to_lang2.py` & `rdmo-1.9.2/rdmo/views/migrations/0011_rename_de_to_lang2.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0012_meta.py` & `rdmo-1.9.2/rdmo/views/migrations/0012_meta.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0013_add_language_fields.py` & `rdmo-1.9.2/rdmo/views/migrations/0013_add_language_fields.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0014_data_migration.py` & `rdmo-1.9.2/rdmo/views/migrations/0014_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0015_remove_null_true.py` & `rdmo-1.9.2/rdmo/views/migrations/0015_remove_null_true.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0017_require_uri_prefix.py` & `rdmo-1.9.2/rdmo/views/migrations/0017_require_uri_prefix.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0018_view_sites.py` & `rdmo-1.9.2/rdmo/views/migrations/0018_view_sites.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0019_view_groups.py` & `rdmo-1.9.2/rdmo/views/migrations/0019_view_groups.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0020_manager.py` & `rdmo-1.9.2/rdmo/views/migrations/0020_manager.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0021_view_catalogs.py` & `rdmo-1.9.2/rdmo/views/migrations/0021_view_catalogs.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/migrations/0023_data_migration.py` & `rdmo-1.9.2/rdmo/views/migrations/0023_data_migration.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/models.py` & `rdmo-1.9.2/rdmo/views/models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/renderers.py` & `rdmo-1.9.2/rdmo/views/renderers.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/serializers/export.py` & `rdmo-1.9.2/rdmo/views/serializers/export.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/serializers/v1.py` & `rdmo-1.9.2/rdmo/views/serializers/v1.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/static/views/js/views.js` & `rdmo-1.9.2/rdmo/views/static/views/js/views.js`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/templates/views/tags/value_file.html` & `rdmo-1.9.2/rdmo/views/templates/views/tags/value_file.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/templates/views/views.html` & `rdmo-1.9.2/rdmo/views/templates/views/views.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/templates/views/views_export.html` & `rdmo-1.9.2/rdmo/views/templates/views/views_export.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/templates/views/views_modal_delete_views.html` & `rdmo-1.9.2/rdmo/views/templates/views/views_modal_delete_views.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/templates/views/views_modal_form_templates.html` & `rdmo-1.9.2/rdmo/views/templates/views/views_modal_form_templates.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/templates/views/views_modal_form_views.html` & `rdmo-1.9.2/rdmo/views/templates/views/views_modal_form_views.html`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/templatetags/view_tags.py` & `rdmo-1.9.2/rdmo/views/templatetags/view_tags.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/tests/test_models.py` & `rdmo-1.9.2/rdmo/views/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/tests/test_validator_locked.py` & `rdmo-1.9.2/rdmo/views/tests/test_validator_locked.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/tests/test_validator_unique_uri.py` & `rdmo-1.9.2/rdmo/views/tests/test_validator_unique_uri.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/tests/test_view_tags.py` & `rdmo-1.9.2/rdmo/views/tests/test_view_tags.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/tests/test_views.py` & `rdmo-1.9.2/rdmo/views/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/tests/test_viewset_view.py` & `rdmo-1.9.2/rdmo/views/tests/test_viewset_view.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/utils.py` & `rdmo-1.9.2/rdmo/views/utils.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/validators.py` & `rdmo-1.9.2/rdmo/views/validators.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/views.py` & `rdmo-1.9.2/rdmo/views/views.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo/views/viewsets.py` & `rdmo-1.9.2/rdmo/views/viewsets.py`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/rdmo.egg-info/PKG-INFO` & `rdmo-1.9.2/rdmo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdmo
-Version: 1.9.1
+Version: 1.9.2
 Summary: RDMO is a tool to support the systematic planning, organisation and implementation of the data management throughout the course of a research project.
 Home-page: https://github.com/rdmorganiser/rdmo
 Author: RDMO Arbeitsgemeinschaft
 Author-email: rdmo-team@listserv.dfn.de
 Maintainer: RDMO Arbeitsgemeinschaft
 Maintainer-email: rdmo-team@listserv.dfn.de
 License: Apache-2.0
```

### Comparing `rdmo-1.9.1/rdmo.egg-info/SOURCES.txt` & `rdmo-1.9.2/rdmo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -688,14 +688,15 @@
 rdmo/projects/tests/__init__.py
 rdmo/projects/tests/test_commands.py
 rdmo/projects/tests/test_handlers.py
 rdmo/projects/tests/test_models.py
 rdmo/projects/tests/test_view_integration.py
 rdmo/projects/tests/test_view_issue.py
 rdmo/projects/tests/test_view_membership.py
+rdmo/projects/tests/test_view_membership_multisite.py
 rdmo/projects/tests/test_view_project.py
 rdmo/projects/tests/test_view_project_create_import.py
 rdmo/projects/tests/test_view_project_join.py
 rdmo/projects/tests/test_view_project_leave.py
 rdmo/projects/tests/test_view_project_update_import.py
 rdmo/projects/tests/test_view_snapshot.py
 rdmo/projects/tests/test_viewset_integration.py
```

### Comparing `rdmo-1.9.1/rdmo.egg-info/requires.txt` & `rdmo-1.9.2/rdmo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/requirements.txt` & `rdmo-1.9.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `rdmo-1.9.1/setup.py` & `rdmo-1.9.2/setup.py`

 * *Files identical despite different names*

