# Comparing `tmp/stytch-6.7.1.tar.gz` & `tmp/stytch-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-6.7.1.tar", last modified: Wed Apr 12 19:53:52 2023, max compression
+gzip compressed data, was "stytch-6.8.0.tar", last modified: Thu Apr 27 15:23:04 2023, max compression
```

## Comparing `stytch-6.7.1.tar` & `stytch-6.8.0.tar`

### file list

```diff
@@ -1,88 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.769403 stytch-6.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 19:53:38.000000 stytch-6.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-12 19:53:52.769403 stytch-6.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 19:53:38.000000 stytch-6.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 19:53:52.769403 stytch-6.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-12 19:53:38.000000 stytch-6.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.757403 stytch-6.7.1/stytch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.761403 stytch-6.7.1/stytch/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.761403 stytch-6.7.1/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    49021 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17130 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/b2b/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/api_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.769403 stytch-6.7.1/stytch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.761403 stytch-6.7.1/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.769403 stytch-6.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-04-12 19:53:38.000000 stytch-6.7.1/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-12 19:53:38.000000 stytch-6.7.1/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.458717 stytch-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-27 15:22:27.000000 stytch-6.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-27 15:23:04.458717 stytch-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-27 15:22:27.000000 stytch-6.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 15:23:04.458717 stytch-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-27 15:22:27.000000 stytch-6.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.446716 stytch-6.8.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.450716 stytch-6.8.0/stytch/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.450716 stytch-6.8.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49021 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17130 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/b2b/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/api_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.458717 stytch-6.8.0/stytch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.450716 stytch-6.8.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.458717 stytch-6.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-04-27 15:22:27.000000 stytch-6.8.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-27 15:22:27.000000 stytch-6.8.0/test/test_integration_async.py
```

### Comparing `stytch-6.7.1/LICENSE.txt` & `stytch-6.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/PKG-INFO` & `stytch-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.7.1
+Version: 6.8.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-6.7.1/README.md` & `stytch-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/setup.py` & `stytch-6.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/crypto_wallets.py` & `stytch-6.8.0/stytch/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/magic_links.py` & `stytch-6.8.0/stytch/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/magic_links_email.py` & `stytch-6.8.0/stytch/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/oauth.py` & `stytch-6.8.0/stytch/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/otp.py` & `stytch-6.8.0/stytch/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/otp_email.py` & `stytch-6.8.0/stytch/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/otp_sms.py` & `stytch-6.8.0/stytch/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/otp_whatsapp.py` & `stytch-6.8.0/stytch/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/passwords.py` & `stytch-6.8.0/stytch/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/passwords_email.py` & `stytch-6.8.0/stytch/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/passwords_existing_password.py` & `stytch-6.8.0/stytch/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/passwords_session.py` & `stytch-6.8.0/stytch/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/sessions.py` & `stytch-6.8.0/stytch/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/totps.py` & `stytch-6.8.0/stytch/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/users.py` & `stytch-6.8.0/stytch/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/api/webauthn.py` & `stytch-6.8.0/stytch/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/api/magic_links.py` & `stytch-6.8.0/stytch/b2b/api/magic_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from typing import Any, Dict, Optional
 
+from stytch.b2b.api.magic_links_discovery import Discovery
 from stytch.b2b.api.magic_links_email import Email
 from stytch.b2b.models.magic_links import AuthenticateResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class MagicLinks:
@@ -19,14 +20,15 @@
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
         self.email = Email(api_base, sync_client, async_client)
+        self.discovery = Discovery(api_base, sync_client, async_client)
 
     @property
     def sub_url(self) -> str:
         return "magic_links"
 
     def authenticate(
         self,
@@ -41,17 +43,17 @@
 
         Parameters:
 
         - `magic_links_token`: The token to authenticate.
 
         - `pkce_code_verifier`: A base64url encoded one-time secret used to validate that the request starts and ends on the same device.
 
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session Management guide.
+        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
 
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session Management guide.
+        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
 
         - `session_duration_minutes`: The Session lifetime of this many minutes from now; minimum of 5 and a maximum of 129600 minutes (90 days). Note that a successful authentication will continue to extend the Session this many minutes.
 
         - `session_custom_claims`: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in Session duration minutes. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
           Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
         """  # noqa
 
@@ -88,17 +90,17 @@
 
         Parameters:
 
         - `magic_links_token`: The token to authenticate.
 
         - `pkce_code_verifier`: A base64url encoded one-time secret used to validate that the request starts and ends on the same device.
 
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session Management guide.
+        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
 
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session Management guide.
+        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
 
         - `session_duration_minutes`: The Session lifetime of this many minutes from now; minimum of 5 and a maximum of 129600 minutes (90 days). Note that a successful authentication will continue to extend the Session this many minutes.
 
         - `session_custom_claims`: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in Session duration minutes. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
           Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
         """  # noqa
```

### Comparing `stytch-6.7.1/stytch/b2b/api/magic_links_email.py` & `stytch-6.8.0/stytch/b2b/api/magic_links_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from typing import Any, Dict, Optional
 
+from stytch.b2b.api.magic_links_email_discovery import Discovery
 from stytch.b2b.models.magic_links_email import InviteResponse, LoginOrSignupResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class Email:
     def __init__(
@@ -17,14 +18,15 @@
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
+        self.discovery = Discovery(api_base, sync_client, async_client)
 
     @property
     def sub_url(self) -> str:
         return "magic_links/email"
 
     def login_or_signup(
         self,
```

### Comparing `stytch-6.7.1/stytch/b2b/api/organizations.py` & `stytch-6.8.0/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/api/passwords.py` & `stytch-6.8.0/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/api/passwords_email.py` & `stytch-6.8.0/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/api/passwords_existing_password.py` & `stytch-6.8.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/api/passwords_session.py` & `stytch-6.8.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/client.py` & `stytch-6.8.0/stytch/b2b/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import warnings
 
 from stytch.b2b.api.magic_links import MagicLinks
 from stytch.b2b.api.organizations import Organizations
 from stytch.b2b.api.passwords import Passwords
 from stytch.b2b.api.sessions import Sessions
+from stytch.b2b.api.discovery import Discovery
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class Client:
     """
     Stytch B2B API Python client.
@@ -29,14 +30,15 @@
         sync_client = SyncClient(project_id, secret)
         async_client = AsyncClient(project_id, secret)
 
         self.magic_links = MagicLinks(api_base, sync_client, async_client)
         self.organizations = Organizations(api_base, sync_client, async_client)
         self.sessions = Sessions(api_base, sync_client, async_client)
         self.passwords = Passwords(api_base, sync_client, async_client)
+        self.discovery = Discovery(api_base, sync_client, async_client)
 
     @classmethod
     def _env_url(cls, env: str, suppress_warnings: bool = False) -> str:
         """Resolve the base URL for the Stytch API environment."""
 
         # Supported production environments
         if env == "test":
```

### Comparing `stytch-6.7.1/stytch/b2b/core/models.py` & `stytch-6.8.0/stytch/b2b/core/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,7 +55,19 @@
     member_session_id: str
     member_id: str
     started_at: datetime.datetime
     last_accessed_at: datetime.datetime
     expires_at: datetime.datetime
     authentication_factors: List[Dict[str, Any]]
     custom_claims: Optional[Dict[str, Any]]
+
+
+class Membership(pydantic.BaseModel):
+    type: str
+    details: Optional[Dict[str, Any]]
+    member: Optional[Member]
+
+
+class DiscoveredOrganization(pydantic.BaseModel):
+    organization: Organization
+    membership: Membership
+    member_authenticated: bool
```

### Comparing `stytch-6.7.1/stytch/b2b/models/magic_links.py` & `stytch-6.8.0/stytch/b2b/models/magic_links.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization so be sure to preserve this value.
 
     - `member`: The Member object.
 
     - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
 
-    - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session Management guide.
+    - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
 
     - `member_session`: The B2BStytchSession object.
     """  # noqa
 
     member_id: str
     method_id: str
     reset_sessions: bool
```

### Comparing `stytch-6.7.1/stytch/b2b/models/magic_links_email.py` & `stytch-6.8.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/models/organizations.py` & `stytch-6.8.0/stytch/b2b/models/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/models/passwords.py` & `stytch-6.8.0/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/models/passwords_email.py` & `stytch-6.8.0/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/models/passwords_existing_password.py` & `stytch-6.8.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/models/passwords_session.py` & `stytch-6.8.0/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/b2b/models/sessions.py` & `stytch-6.8.0/stytch/b2b/models/sessions.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,7 +37,31 @@
 
 
 class RevokeResponse(ResponseBase):
     """Response fields beyond those defined in `ResponseBase`:
 
     (None)
     """  # noqa
+
+
+class ExchangeResponse(ResponseBase):
+    """Response fields beyond those defined in `ResponseBase`:
+
+    - `member_id`: The UUID of the Member object that was created.
+
+    - `session_token`: A secret token for a given Stytch session.
+
+    - `session_jwt`: The JSON Web Token (JWT) for a given Stytch session.
+
+    - `member_session`: The B2BStytchSession object.
+
+    - `member`: The [Member](https://stytch.com/docs/b2b/api/member-object) object.
+
+    - `organization`: The [Organization](https://stytch.com/docs/b2b/api/organization-object) object.
+    """  # noqa
+
+    member_id: str
+    member_session: B2BStytchSession
+    session_token: str
+    session_jwt: str
+    member: Member
+    organization: Organization
```

### Comparing `stytch-6.7.1/stytch/client.py` & `stytch-6.8.0/stytch/client.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/core/http/client.py` & `stytch-6.8.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/core/models.py` & `stytch-6.8.0/stytch/core/models.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/crypto_wallets.py` & `stytch-6.8.0/stytch/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/magic_links.py` & `stytch-6.8.0/stytch/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/magic_links_email.py` & `stytch-6.8.0/stytch/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/oauth.py` & `stytch-6.8.0/stytch/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/passwords.py` & `stytch-6.8.0/stytch/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/sessions.py` & `stytch-6.8.0/stytch/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/totps.py` & `stytch-6.8.0/stytch/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/users.py` & `stytch-6.8.0/stytch/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch/models/webauthn.py` & `stytch-6.8.0/stytch/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/stytch.egg-info/PKG-INFO` & `stytch-6.8.0/stytch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.7.1
+Version: 6.8.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-6.7.1/stytch.egg-info/SOURCES.txt` & `stytch-6.8.0/stytch.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -26,27 +26,37 @@
 stytch/api/sessions.py
 stytch/api/totps.py
 stytch/api/users.py
 stytch/api/webauthn.py
 stytch/b2b/__init__.py
 stytch/b2b/client.py
 stytch/b2b/api/__init__.py
+stytch/b2b/api/discovery.py
+stytch/b2b/api/discovery_intermediate_sessions.py
+stytch/b2b/api/discovery_organizations.py
 stytch/b2b/api/magic_links.py
+stytch/b2b/api/magic_links_discovery.py
 stytch/b2b/api/magic_links_email.py
+stytch/b2b/api/magic_links_email_discovery.py
 stytch/b2b/api/organizations.py
 stytch/b2b/api/passwords.py
 stytch/b2b/api/passwords_email.py
 stytch/b2b/api/passwords_existing_password.py
 stytch/b2b/api/passwords_session.py
 stytch/b2b/api/sessions.py
 stytch/b2b/core/__init__.py
 stytch/b2b/core/models.py
 stytch/b2b/models/__init__.py
+stytch/b2b/models/discovery.py
+stytch/b2b/models/discovery_intermediate_sessions.py
+stytch/b2b/models/discovery_organizations.py
 stytch/b2b/models/magic_links.py
+stytch/b2b/models/magic_links_discovery.py
 stytch/b2b/models/magic_links_email.py
+stytch/b2b/models/magic_links_email_discovery.py
 stytch/b2b/models/organizations.py
 stytch/b2b/models/passwords.py
 stytch/b2b/models/passwords_email.py
 stytch/b2b/models/passwords_existing_password.py
 stytch/b2b/models/passwords_session.py
 stytch/b2b/models/sessions.py
 stytch/core/__init__.py
```

### Comparing `stytch-6.7.1/test/test_integration.py` & `stytch-6.8.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.1/test/test_integration_async.py` & `stytch-6.8.0/test/test_integration_async.py`

 * *Files identical despite different names*

