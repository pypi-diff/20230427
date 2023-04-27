# Comparing `tmp/requests_auth-6.0.0.tar.gz` & `tmp/requests_auth-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/requests_auth-6.0.0.tar", last modified: Tue Jan 11 18:24:22 2022, max compression
+gzip compressed data, was "requests_auth-7.0.0.tar", last modified: Thu Apr 27 16:15:49 2023, max compression
```

## Comparing `requests_auth-6.0.0.tar` & `requests_auth-7.0.0.tar`

### file list

```diff
@@ -1,19 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 18:24:22.000000 requests_auth-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    98551 2022-01-11 18:24:22.000000 requests_auth-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    90914 2022-01-11 18:24:11.000000 requests_auth-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 18:24:22.000000 requests_auth-6.0.0/requests_auth/
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-01-11 18:24:11.000000 requests_auth-6.0.0/requests_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    64968 2022-01-11 18:24:11.000000 requests_auth-6.0.0/requests_auth/authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     6423 2022-01-11 18:24:11.000000 requests_auth-6.0.0/requests_auth/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     8655 2022-01-11 18:24:11.000000 requests_auth-6.0.0/requests_auth/oauth2_authentication_responses_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     9307 2022-01-11 18:24:11.000000 requests_auth-6.0.0/requests_auth/oauth2_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     5575 2022-01-11 18:24:11.000000 requests_auth-6.0.0/requests_auth/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-01-11 18:24:11.000000 requests_auth-6.0.0/requests_auth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 18:24:22.000000 requests_auth-6.0.0/requests_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    98551 2022-01-11 18:24:22.000000 requests_auth-6.0.0/requests_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-01-11 18:24:22.000000 requests_auth-6.0.0/requests_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-11 18:24:22.000000 requests_auth-6.0.0/requests_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-01-11 18:24:22.000000 requests_auth-6.0.0/requests_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-11 18:24:22.000000 requests_auth-6.0.0/requests_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-11 18:24:22.000000 requests_auth-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-01-11 18:24:11.000000 requests_auth-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.907633 requests_auth-7.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.903633 requests_auth-7.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.903633 requests_auth-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-27 16:15:20.000000 requests_auth-7.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-27 16:15:20.000000 requests_auth-7.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-27 16:15:20.000000 requests_auth-7.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 16:15:20.000000 requests_auth-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-04-27 16:15:20.000000 requests_auth-7.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 16:15:20.000000 requests_auth-7.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 16:15:20.000000 requests_auth-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    97300 2023-04-27 16:15:49.907633 requests_auth-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    94747 2023-04-27 16:15:20.000000 requests_auth-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 16:15:20.000000 requests_auth-7.0.0/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-27 16:15:20.000000 requests_auth-7.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.903633 requests_auth-7.0.0/requests_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-27 16:15:20.000000 requests_auth-7.0.0/requests_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68229 2023-04-27 16:15:20.000000 requests_auth-7.0.0/requests_auth/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-27 16:15:20.000000 requests_auth-7.0.0/requests_auth/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-27 16:15:20.000000 requests_auth-7.0.0/requests_auth/oauth2_authentication_responses_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-04-27 16:15:20.000000 requests_auth-7.0.0/requests_auth/oauth2_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-27 16:15:20.000000 requests_auth-7.0.0/requests_auth/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 16:15:20.000000 requests_auth-7.0.0/requests_auth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.903633 requests_auth-7.0.0/requests_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    97300 2023-04-27 16:15:49.000000 requests_auth-7.0.0/requests_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-27 16:15:49.000000 requests_auth-7.0.0/requests_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:15:49.000000 requests_auth-7.0.0/requests_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-27 16:15:49.000000 requests_auth-7.0.0/requests_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 16:15:49.000000 requests_auth-7.0.0/requests_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:15:49.907633 requests_auth-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.907633 requests_auth-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/auth_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.907633 requests_auth-7.0.0/tests/failing_ntlm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/failing_ntlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/failing_ntlm/requests_negotiate_sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/failing_ntlm/requests_ntlm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:49.907633 requests_auth-7.0.0/tests/success_ntlm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/success_ntlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/success_ntlm/requests_negotiate_sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/success_ntlm/requests_ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_add_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_and_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_auths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_json_token_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49140 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_authorization_code_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57026 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_authorization_code_pkce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45955 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_authorization_code_pkce_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_client_credential_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41825 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_implicit_azure_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_implicit_id_token_azure_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_implicit_id_token_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_implicit_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_resource_owner_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28080 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_oauth2_resource_owner_password_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_testing_oauth2_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_testing_oauth2_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-27 16:15:20.000000 requests_auth-7.0.0/tests/test_testing_token_mock.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `requests_auth-6.0.0/PKG-INFO` & `requests_auth-7.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,814 +1,823 @@
-Metadata-Version: 2.1
-Name: requests_auth
-Version: 6.0.0
-Summary: Authentication for Requests
-Home-page: https://colin-b.github.io/requests_auth/
-Author: Colin Bounouar
-Author-email: colin.bounouar.dev@gmail.com
-Maintainer: Colin Bounouar
-Maintainer-email: colin.bounouar.dev@gmail.com
-License: MIT
-Download-URL: https://pypi.org/project/requests-auth/
-Project-URL: GitHub, https://github.com/Colin-b/requests_auth
-Project-URL: Changelog, https://github.com/Colin-b/requests_auth/blob/master/CHANGELOG.md
-Project-URL: Issues, https://github.com/Colin-b/requests_auth/issues
-Description: <h2 align="center">Authentication for Requests</h2>
-        
-        <p align="center">
-        <a href="https://pypi.org/project/requests-auth/"><img alt="pypi version" src="https://img.shields.io/pypi/v/requests_auth"></a>
-        <a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Build status" src="https://github.com/Colin-b/requests_auth/workflows/Release/badge.svg"></a>
-        <a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Coverage" src="https://img.shields.io/badge/coverage-100%25-brightgreen"></a>
-        <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-        <a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Number of tests" src="https://img.shields.io/badge/tests-275 passed-blue"></a>
-        <a href="https://pypi.org/project/requests-auth/"><img alt="Number of downloads" src="https://img.shields.io/pypi/dm/requests_auth"></a>
-        </p>
-        
-        Provides authentication classes to be used with [`requests`][1] [authentication parameter][2].
-        
-        <p align="center">
-            <a href="https://oauth.net/2/"><img alt="OAuth2" src="https://oauth.net/images/oauth-2-sm.png"></a>
-            <a href="https://www.okta.com"><img alt="Okta" src="https://www.okta.com/sites/all/themes/Okta/images/logos/developer/Dev_Logo-03_Large.png" height="120"></a>
-            <a href="https://azure.microsoft.com/en-us/services/active-directory/"><img alt="Azure Active Directory (AD)" src="https://azurecomcdn.azureedge.net/cvt-cda59ccd0aa5ced6ff5a2052417cf596b92980921e88e667127eaca2232a31ab/images/shared/services/pricing-glyph-lock.svg" height="120"></a>
-        </p>
-        <p align="center">Some of the supported authentication</p>
-        
-        ## Available authentication
-        
-        - [OAuth2](#oauth-2)
-          - [Authorization Code Flow](#authorization-code-flow)
-            - [Okta](#okta-oauth2-authorization-code)
-          - [Authorization Code Flow with PKCE](#authorization-code-flow-with-proof-key-for-code-exchange)
-            - [Okta](#okta-oauth2-proof-key-for-code-exchange)
-          - [Resource Owner Password Credentials flow](#resource-owner-password-credentials-flow)
-          - [Client Credentials Flow](#client-credentials-flow)
-            - [Okta](#okta-oauth2-client-credentials)
-          - [Implicit Flow](#implicit-flow)
-            - [Azure AD (Access Token)](#microsoft---azure-active-directory-oauth2-access-token)
-            - [Azure AD (ID token)](#microsoft---azure-active-directory-openid-connect-id-token)
-            - [Okta (Access Token)](#okta-oauth2-implicit-access-token)
-            - [Okta (ID token)](#okta-openid-connect-implicit-id-token)
-          - [Managing token cache](#managing-token-cache)
-        - API key
-          - [In header](#api-key-in-header)
-          - [In query](#api-key-in-query)
-        - [Basic](#basic)
-        - [NTLM (Windows)](#ntlm)
-        - [Multiple authentication at once](#multiple-authentication-at-once)
-        - [Endorsements](#endorsements)
-        
-        ## OAuth 2
-        
-        Most of [OAuth2](https://oauth.net/2/) flows are supported.
-        
-        If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
-        
-        ### Authorization Code flow
-        
-        Authorization Code Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.1).
-        
-        Use `requests_auth.OAuth2AuthorizationCode` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OAuth2AuthorizationCode
-        
-        requests.get('https://www.example.com', auth=OAuth2AuthorizationCode('https://www.authorization.url', 'https://www.token.url'))
-        ```
-        
-        #### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
-        | `authorization_url`     | OAuth 2 authorization URL.                                                                                                                                                                                                                                                                        | Mandatory  |                |
-        | `token_url`             | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''             |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 code will be started.                                                                                                                                                                                                                      | Optional   | 5000           |
-        | `timeout`               | Maximum amount of seconds to wait for a code or a token to be received once requested.                                                                                                                                                                                                            | Optional   | 60             |
-        | `success_display_time`  | In case a code is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                           | Optional   | 1              |
-        | `failure_display_time`  | In case received code is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                                | Optional   | 5000           |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | code           |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
-        | `code_field_name`       | Field name containing the code.                                                                                                                                                                                                                                                                   | Optional   | code           |
-        | `username`              | User name in case basic authentication should be used to retrieve token.                                                                                                                                                                                                                          | Optional   |                |
-        | `password`              | User password in case basic authentication should be used to retrieve token.                                                                                                                                                                                                                      | Optional   |                |
-        | `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
-        
-        Any other parameter will be put as query parameter in the authorization URL and as body parameters in the token URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `client_id`     | Corresponding to your Application ID (in Microsoft Azure app portal) |
-        | `client_secret` | If client is not authenticated with the authorization server         |
-        | `nonce`         | Refer to [OpenID ID Token specifications][3] for more details        |
-        
-        #### Common providers
-        
-        Most of [OAuth2](https://oauth.net/2/) Authorization Code Grant providers are supported.
-        
-        If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
-        
-        ##### Okta (OAuth2 Authorization Code)
-        
-        [Okta Authorization Code Grant](https://developer.okta.com/docs/guides/implement-auth-code/overview/) providing access tokens is supported.
-        
-        Use `requests_auth.OktaAuthorizationCode` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OktaAuthorizationCode
-        
-        
-        okta = OktaAuthorizationCode(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
-        requests.get('https://www.example.com', auth=okta)
-        ```
-        
-        ###### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
-        | `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
-        | `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | token                                        |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
-        | `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
-        | `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | openid                                       |
-        | `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
-        | `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
-        | `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
-        | `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
-        | `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                                              |
-        
-        Any other parameter will be put as query parameter in the authorization URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `prompt`        | none to avoid prompting the user if a session is already opened.     |
-        
-        ### Authorization Code Flow with Proof Key for Code Exchange
-        
-        Proof Key for Code Exchange is implemented following [rfc7636](https://tools.ietf.org/html/rfc7636).
-        
-        Use `requests_auth.OAuth2AuthorizationCodePKCE` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OAuth2AuthorizationCodePKCE
-        
-        requests.get('https://www.example.com', auth=OAuth2AuthorizationCodePKCE('https://www.authorization.url', 'https://www.token.url'))
-        ```
-        
-        #### Parameters 
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
-        | `authorization_url`     | OAuth 2 authorization URL.                                                                                                                                                                                                                                                                        | Mandatory  |                |
-        | `token_url`             | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''             |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 code will be started.                                                                                                                                                                                                                      | Optional   | 5000           |
-        | `timeout`               | Maximum amount of seconds to wait for a code or a token to be received once requested.                                                                                                                                                                                                            | Optional   | 60             |
-        | `success_display_time`  | In case a code is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                           | Optional   | 1              |
-        | `failure_display_time`  | In case received code is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                                | Optional   | 5000           |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | code           |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
-        | `code_field_name`       | Field name containing the code.                                                                                                                                                                                                                                                                   | Optional   | code           |
-        | `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
-        
-        Any other parameter will be put as query parameter in the authorization URL and as body parameters in the token URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `client_id`     | Corresponding to your Application ID (in Microsoft Azure app portal) |
-        | `client_secret` | If client is not authenticated with the authorization server         |
-        | `nonce`         | Refer to [OpenID ID Token specifications][3] for more details        |
-        
-        #### Common providers
-        
-        Most of [OAuth2](https://oauth.net/2/) Proof Key for Code Exchange providers are supported.
-        
-        If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
-        
-        ##### Okta (OAuth2 Proof Key for Code Exchange)
-        
-        [Okta Proof Key for Code Exchange](https://developer.okta.com/docs/guides/implement-auth-code-pkce/overview/) providing access tokens is supported.
-        
-        Use `requests_auth.OktaAuthorizationCodePKCE` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OktaAuthorizationCodePKCE
-        
-        
-        okta = OktaAuthorizationCodePKCE(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
-        requests.get('https://www.example.com', auth=okta)
-        ```
-        
-        ###### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
-        | `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
-        | `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | code                                         |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
-        | `code_field_name`       | Field name containing the code.                                                                                                                                                                                                                                                                   | Optional   | code                                         |
-        | `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
-        | `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | openid                                       |
-        | `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
-        | `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
-        | `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
-        | `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
-        | `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                                              |
-        
-        Any other parameter will be put as query parameter in the authorization URL and as body parameters in the token URL.        
-        
-        Usual extra parameters are:
-        
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `client_secret`        | If client is not authenticated with the authorization server     |
-        | `nonce`        | Refer to [OpenID ID Token specifications][3] for more details     |
-        
-        ### Resource Owner Password Credentials flow 
-        
-        Resource Owner Password Credentials Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.3).
-        
-        Use `requests_auth.OAuth2ResourceOwnerPasswordCredentials` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OAuth2ResourceOwnerPasswordCredentials
-        
-        requests.get('https://www.example.com', auth=OAuth2ResourceOwnerPasswordCredentials('https://www.token.url', 'user name', 'user password'))
-        ```
-        
-        #### Parameters
-        
-        | Name               | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
-        |:-------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
-        | `token_url`        | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
-        | `username`         | Resource owner user name.                                                                                                                                                                                                                                                                         | Mandatory  |                |
-        | `password`         | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory  |                |
-        | `timeout`          | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60             |
-        | `header_name`      | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
-        | `header_value`     | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
-        | `scope`            | Scope parameter sent to token URL as body. Can also be a list of scopes.                                                                                                                                                                                                                          | Optional   |                |
-        | `token_field_name` | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
-        | `early_expiry`     | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
-        | `session`          | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
-        
-        Any other parameter will be put as body parameter in the token URL.
-        
-        ### Client Credentials flow
-        
-        Client Credentials Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.4).
-        
-        Use `requests_auth.OAuth2ClientCredentials` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OAuth2ClientCredentials
-        
-        requests.get('https://www.example.com', auth=OAuth2ClientCredentials('https://www.token.url', client_id='id', client_secret='secret'))
-        ```
-        
-        #### Parameters
-        
-        | Name               | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
-        |:-------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
-        | `token_url`        | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
-        | `client_id`        | Resource owner user name.                                                                                                                                                                                                                                                                         | Mandatory  |                |
-        | `client_secret`    | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory  |                |
-        | `timeout`          | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60             |
-        | `header_name`      | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
-        | `header_value`     | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
-        | `scope`            | Scope parameter sent to token URL as body. Can also be a list of scopes.                                                                                                                                                                                                                          | Optional   |                |
-        | `token_field_name` | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
-        | `early_expiry`     | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
-        | `session`          | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
-        
-        Any other parameter will be put as body parameter in the token URL.
-        
-        #### Common providers
-        
-        Most of [OAuth2](https://oauth.net/2/) Client Credentials Grant providers are supported.
-        
-        If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
-        
-        ##### Okta (OAuth2 Client Credentials)
-        
-        [Okta Client Credentials Grant](https://developer.okta.com/docs/guides/implement-client-creds/overview/) providing access tokens is supported.
-        
-        Use `requests_auth.OktaClientCredentials` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OktaClientCredentials
-        
-        
-        okta = OktaClientCredentials(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_secret="secret")
-        requests.get('https://www.example.com', auth=okta)
-        ```
-        
-        ###### Parameters
-        
-        | Name                   | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
-        |:-----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
-        | `instance`             | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                |
-        | `client_id`            | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                |
-        | `client_secret`        | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory  |                |
-        | `authorization_server` | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'      |
-        | `timeout`              | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60             |
-        | `header_name`          | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
-        | `header_value`         | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
-        | `scope`                | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | openid         |
-        | `token_field_name`     | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
-        | `early_expiry`         | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
-        | `session`              | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
-        
-        Any other parameter will be put as query parameter in the token URL.        
-        
-        ### Implicit flow
-        
-        Implicit Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.2).
-        
-        Use `requests_auth.OAuth2Implicit` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OAuth2Implicit
-        
-        requests.get('https://www.example.com', auth=OAuth2Implicit('https://www.authorization.url'))
-        ```
-        
-        #### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory | Default value                                                 |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:--------------------------------------------------------------|
-        | `authorization_url`     | OAuth 2 authorization URL.                                                                                                                                                                                                                                                                        | Mandatory |                                                               |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional  | token                                                         |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional  | id_token if response_type is id_token, otherwise access_token |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional  | 30.0                                                          |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional  | ''                                                            |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional  | 5000                                                          |
-        | `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional  | 60                                                            |
-        | `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional  | 1                                                             |
-        | `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional  | 5000                                                          |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional  | Authorization                                                 |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional  | Bearer {token}                                                |
-        
-        Any other parameter will be put as query parameter in the authorization URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `client_id`     | Corresponding to your Application ID (in Microsoft Azure app portal) |
-        | `nonce`         | Refer to [OpenID ID Token specifications][3] for more details        |
-        | `prompt`        | none to avoid prompting the user if a session is already opened.     |
-        
-        #### Common providers
-        
-        Most of [OAuth2](https://oauth.net/2/) Implicit Grant providers are supported.
-        
-        If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
-        
-        ##### Microsoft - Azure Active Directory (OAuth2 Access Token)
-        
-        [Microsoft identity platform access tokens](https://docs.microsoft.com/en-us/azure/active-directory/develop/access-tokens) are supported.
-        
-        Use `requests_auth.AzureActiveDirectoryImplicit` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import AzureActiveDirectoryImplicit
-        
-        
-        aad = AzureActiveDirectoryImplicit(tenant_id='45239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
-        requests.get('https://www.example.com', auth=aad)
-        ```
-        
-        You can retrieve Microsoft Azure Active Directory application information thanks to the [application list on Azure portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/).
-        
-        ###### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
-        | `tenant_id`             | Microsoft Tenant Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
-        | `client_id`             | Microsoft Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                   | Mandatory  |                                              |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | token                                        |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
-        | `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details                                                                                                                                                                                                                                     | Optional   | Newly generated Universal Unique Identifier. |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
-        | `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
-        | `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
-        | `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
-        
-        Any other parameter will be put as query parameter in the authorization URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `prompt`        | none to avoid prompting the user if a session is already opened.     |
-        
-        ##### Microsoft - Azure Active Directory (OpenID Connect ID token)
-        
-        [Microsoft identity platform ID tokens](https://docs.microsoft.com/en-us/azure/active-directory/develop/id-tokens) are supported.
-        
-        Use `requests_auth.AzureActiveDirectoryImplicitIdToken` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import AzureActiveDirectoryImplicitIdToken
-        
-        
-        aad = AzureActiveDirectoryImplicitIdToken(tenant_id='45239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
-        requests.get('https://www.example.com', auth=aad)
-        ```
-        
-        You can retrieve Microsoft Azure Active Directory application information thanks to the [application list on Azure portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/).
-        
-        ###### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory | Default value                                |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:---------------------------------------------|
-        | `tenant_id`             | Microsoft Tenant Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory |                                              |
-        | `client_id`             | Microsoft Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                   | Mandatory |                                              |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional  | id_token                                     |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional  | id_token                                     |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional  | 30.0                                         |
-        | `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details                                                                                                                                                                                                                                     | Optional  | Newly generated Universal Unique Identifier. |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional  | ''                                           |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional  | 5000                                         |
-        | `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional  | 60                                           |
-        | `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional  | 1                                            |
-        | `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional  | 5000                                         |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional  | Authorization                                |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional  | Bearer {token}                               |
-        
-        Any other parameter will be put as query parameter in the authorization URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `prompt`        | none to avoid prompting the user if a session is already opened.     |
-        
-        ##### Okta (OAuth2 Implicit Access Token)
-        
-        [Okta Implicit Grant](https://developer.okta.com/docs/guides/implement-implicit/overview/) providing access tokens is supported.
-        
-        Use `requests_auth.OktaImplicit` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OktaImplicit
-        
-        
-        okta = OktaImplicit(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
-        requests.get('https://www.example.com', auth=okta)
-        ```
-        
-        ###### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
-        | `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
-        | `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | token                                        |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
-        | `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
-        | `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | ['openid', 'profile', 'email']               |
-        | `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
-        | `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
-        | `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
-        | `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
-        
-        Any other parameter will be put as query parameter in the authorization URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `prompt`        | none to avoid prompting the user if a session is already opened.     |
-        
-        ##### Okta (OpenID Connect Implicit ID token)
-        
-        [Okta Implicit Grant](https://developer.okta.com/docs/guides/implement-implicit/overview/) providing ID tokens is supported.
-        
-        Use `requests_auth.OktaImplicitIdToken` to configure this kind of authentication.
-        
-        ```python
-        import requests
-        from requests_auth import OktaImplicitIdToken
-        
-        
-        okta = OktaImplicitIdToken(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
-        requests.get('https://www.example.com', auth=okta)
-        ```
-        
-        ###### Parameters
-        
-        | Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
-        |:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
-        | `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
-        | `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
-        | `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | id_token                                     |
-        | `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | id_token                                     |
-        | `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
-        | `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
-        | `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | ['openid', 'profile', 'email']               |
-        | `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
-        | `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
-        | `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
-        | `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
-        | `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
-        | `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
-        | `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
-        | `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
-        
-        Any other parameter will be put as query parameter in the authorization URL.        
-        
-        Usual extra parameters are:
-                
-        | Name            | Description                                                          |
-        |:----------------|:---------------------------------------------------------------------|
-        | `prompt`        | none to avoid prompting the user if a session is already opened.     |
-        
-        ### Managing token cache
-        
-        To avoid asking for a new token every new request, a token cache is used.
-        
-        Default cache is in memory but it is also possible to use a physical cache.
-        
-        You need to provide the location of your token cache file. It can be a full or relative path.
-        
-        If the file already exists it will be used, if the file do not exists it will be created.
-        
-        ```python
-        from requests_auth import OAuth2, JsonTokenFileCache
-        
-        OAuth2.token_cache = JsonTokenFileCache('path/to/my_token_cache.json')
-        ```
-        
-        ## API key in header
-        
-        You can send an API key inside the header of your request using `requests_auth.HeaderApiKey`.
-        
-        ```python
-        import requests
-        from requests_auth import HeaderApiKey
-        
-        requests.get('https://www.example.com', auth=HeaderApiKey('my_api_key'))
-        ```
-        
-        ### Parameters
-        
-        | Name                    | Description                    | Mandatory | Default value |
-        |:------------------------|:-------------------------------|:----------|:--------------|
-        | `api_key`               | The API key that will be sent. | Mandatory |               |
-        | `header_name`           | Name of the header field.      | Optional  | "X-API-Key"   |
-        
-        ## API key in query
-        
-        You can send an API key inside the query parameters of your request using `requests_auth.QueryApiKey`.
-        
-        ```python
-        import requests
-        from requests_auth import QueryApiKey
-        
-        requests.get('https://www.example.com', auth=QueryApiKey('my_api_key'))
-        ```
-        
-        ### Parameters
-        
-        | Name                    | Description                    | Mandatory | Default value |
-        |:------------------------|:-------------------------------|:----------|:--------------|
-        | `api_key`               | The API key that will be sent. | Mandatory |               |
-        | `query_parameter_name`  | Name of the query parameter.   | Optional  | "api_key"     |
-        
-        ## Basic
-        
-        You can use basic authentication using `requests_auth.Basic`.
-        
-        The only advantage of using this class instead of `requests` native support of basic authentication, is to be able to use it in [multiple authentication](#multiple-authentication-at-once).
-        
-        ```python
-        import requests
-        from requests_auth import Basic
-        
-        requests.get('https://www.example.com', auth=Basic('username', 'password'))
-        ```
-        
-        ### Parameters
-        
-        | Name                    | Description                    | Mandatory | Default value |
-        |:------------------------|:-------------------------------|:----------|:--------------|
-        | `username`              | User name.                     | Mandatory |               |
-        | `password`              | User password.                 | Mandatory |               |
-        
-        ## NTLM
-        
-        Requires [`requests-negotiate-sspi` module][4] or [`requests_ntlm` module][5] depending on provided parameters.
-        
-        You can use Windows authentication using `requests_auth.NTLM`.
-        
-        ```python
-        import requests
-        from requests_auth import NTLM
-        
-        requests.get('https://www.example.com', auth=NTLM())
-        ```
-        
-        ### Parameters
-        
-        | Name                    | Description                    | Mandatory | Default value |
-        |:------------------------|:-------------------------------|:----------|:--------------|
-        | `username`              | User name.                     | Mandatory if `requests_negotiate_sspi` module is not installed. In such a case `requests_ntlm` module is mandatory. |               |
-        | `password`              | User password.                 | Mandatory if `requests_negotiate_sspi` module is not installed. In such a case `requests_ntlm` module is mandatory. |               |
-        
-        ## Multiple authentication at once
-        
-        You can also use a combination of authentication using `+` or `&` as in the following sample:
-        
-        ```python
-        import requests
-        from requests_auth import HeaderApiKey, OAuth2Implicit
-        
-        api_key = HeaderApiKey('my_api_key')
-        oauth2 = OAuth2Implicit('https://www.example.com')
-        requests.get('https://www.example.com', auth=api_key + oauth2)
-        ```
-        
-        ## Available pytest fixtures
-        
-        Testing the code using `requests_auth` authentication classes can be achieved using provided [`pytest`][6] fixtures.
-        
-        ### token_cache_mock
-        
-        ```python
-        from requests_auth.testing import token_cache_mock, token_mock
-        
-        def test_something(token_cache_mock):
-            # perform code using authentication
-            pass
-        ```
-        
-        Use this fixture to mock authentication success for any of the following classes:
-         * OAuth2AuthorizationCodePKCE
-         * OktaAuthorizationCodePKCE
-         * OAuth2Implicit
-         * OktaImplicit
-         * OktaImplicitIdToken
-         * AzureActiveDirectoryImplicit
-         * AzureActiveDirectoryImplicitIdToken
-         * OAuth2AuthorizationCode
-         * OktaAuthorizationCode
-         * OAuth2ClientCredentials
-         * OktaClientCredentials
-         * OAuth2ResourceOwnerPasswordCredentials,
-        
-        By default, an access token with value `2YotnFZFEjr1zCsicMWpAA` is generated.
-        
-        You can however return your custom token by providing your own `token_mock` fixture as in the following sample:
-        
-        ```python
-        import pytest
-        
-        from requests_auth.testing import token_cache_mock
-        
-        
-        @pytest.fixture
-        def token_mock() -> str:
-            return "MyCustomTokenValue"
-        
-        
-        def test_something(token_cache_mock):
-            # perform code using authentication
-            pass
-        ```
-        
-        You can even return a more complex token by using the `create_token` function.
-        
-        Note that [`pyjwt`](https://pypi.org/project/PyJWT/) is a required dependency in this case as it is used to generate the token returned by the authentication.
-        
-        ```python
-        import pytest
-        
-        from requests_auth.testing import token_cache_mock, create_token
-        
-        
-        @pytest.fixture
-        def token_mock() -> str:
-            expiry = None  # TODO Compute your expiry
-            return create_token(expiry)
-        
-        
-        def test_something(token_cache_mock):
-            # perform code using authentication
-            pass
-        ```
-        
-        ### Advanced testing
-        
-        #### token_cache
-        
-        This [`pytest`][6] fixture will return the token cache and ensure it is reset at the end of the test case.
-        
-        ```python
-        from requests_auth.testing import token_cache
-        
-        def test_something(token_cache):
-            # perform code using authentication
-            pass
-        ```
-        
-        #### browser_mock
-        
-        This [`pytest`][6] fixture will allow to mock the behavior of a web browser.
-        
-        With this [`pytest`][6] fixture you will be allowed to fine tune your authentication related failures handling.
-        
-        [`pyjwt`](https://pypi.org/project/PyJWT/) is a required dependency if you use `create_token` helper function.
-        
-        ```python
-        import datetime
-        
-        from requests_auth.testing import browser_mock, BrowserMock, create_token
-        
-        def test_something(browser_mock: BrowserMock):
-            token_expiry = datetime.datetime.utcnow() + datetime.timedelta(hours=1)
-            token = create_token(token_expiry)
-            tab = browser_mock.add_response(
-                opened_url="http://url_opened_by_browser?state=1234",
-                reply_url=f"http://localhost:5000#access_token={token}&state=1234",
-            )
-        
-            # perform code using authentication
-        
-            tab.assert_success(
-                "You are now authenticated on 1234 You may close this tab."
-            )
-        ```
-        
-        ## Endorsements
-        
-        > I love requests_auth. As a ~15 year pythonista, this library makes working with OAuth services a breeze. <333
-        
-        **Randall Degges**, Head of Evangelism, [Okta](https://developer.okta.com)
-        
-        [1]: https://pypi.python.org/pypi/requests "requests module"
-        [2]: https://2.python-requests.org/en/master/user/authentication/ "authentication parameter on requests module"
-        [3]: https://openid.net/specs/openid-connect-core-1_0.html#IDToken "OpenID ID Token specifications"
-        [4]: https://pypi.python.org/pypi/requests-negotiate-sspi "requests-negotiate-sspi module"
-        [5]: https://pypi.python.org/pypi/requests_ntlm "requests_ntlm module"
-        [6]: https://docs.pytest.org/en/latest/ "pytest module"
-Keywords: authentication,ntlm,oauth2,azure-active-directory,azure-ad,okta,apikey,multiple
-Platform: Windows
-Platform: Linux
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: testing
+<h2 align="center">Authentication for Requests</h2>
+
+<p align="center">
+<a href="https://pypi.org/project/requests-auth/"><img alt="pypi version" src="https://img.shields.io/pypi/v/requests_auth"></a>
+<a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Build status" src="https://github.com/Colin-b/requests_auth/workflows/Release/badge.svg"></a>
+<a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Coverage" src="https://img.shields.io/badge/coverage-100%25-brightgreen"></a>
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+<a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Number of tests" src="https://img.shields.io/badge/tests-305 passed-blue"></a>
+<a href="https://pypi.org/project/requests-auth/"><img alt="Number of downloads" src="https://img.shields.io/pypi/dm/requests_auth"></a>
+</p>
+
+Provides authentication classes to be used with [`requests`][1] [authentication parameter][2].
+
+<p align="center">
+    <a href="https://oauth.net/2/"><img alt="OAuth2" src="https://oauth.net/images/oauth-2-sm.png"></a>
+    <a href="https://www.okta.com"><img alt="Okta" src="https://www.okta.com/sites/all/themes/Okta/images/logos/developer/Dev_Logo-03_Large.png" height="120"></a>
+    <a href="https://azure.microsoft.com/en-us/services/active-directory/"><img alt="Azure Active Directory (AD)" src="https://azurecomcdn.azureedge.net/cvt-cda59ccd0aa5ced6ff5a2052417cf596b92980921e88e667127eaca2232a31ab/images/shared/services/pricing-glyph-lock.svg" height="120"></a>
+</p>
+<p align="center">Some of the supported authentication</p>
+
+## Available authentication
+
+- [OAuth2](#oauth-2)
+  - [Authorization Code Flow](#authorization-code-flow)
+    - [Okta](#okta-oauth2-authorization-code)
+  - [Authorization Code Flow with PKCE](#authorization-code-flow-with-proof-key-for-code-exchange)
+    - [Okta](#okta-oauth2-proof-key-for-code-exchange)
+  - [Resource Owner Password Credentials flow](#resource-owner-password-credentials-flow)
+  - [Client Credentials Flow](#client-credentials-flow)
+    - [Okta](#okta-oauth2-client-credentials)
+  - [Implicit Flow](#implicit-flow)
+    - [Azure AD (Access Token)](#microsoft---azure-active-directory-oauth2-access-token)
+    - [Azure AD (ID token)](#microsoft---azure-active-directory-openid-connect-id-token)
+    - [Okta (Access Token)](#okta-oauth2-implicit-access-token)
+    - [Okta (ID token)](#okta-openid-connect-implicit-id-token)
+  - [Managing token cache](#managing-token-cache)
+- API key
+  - [In header](#api-key-in-header)
+  - [In query](#api-key-in-query)
+- [Basic](#basic)
+- [NTLM (Windows)](#ntlm)
+- [Multiple authentication at once](#multiple-authentication-at-once)
+- [Endorsements](#endorsements)
+
+## OAuth 2
+
+Most of [OAuth2](https://oauth.net/2/) flows are supported.
+
+If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
+
+### Authorization Code flow
+
+Authorization Code Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.1).
+
+Use `requests_auth.OAuth2AuthorizationCode` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OAuth2AuthorizationCode
+
+requests.get('https://www.example.com', auth=OAuth2AuthorizationCode('https://www.authorization.url', 'https://www.token.url'))
+```
+
+#### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
+| `authorization_url`     | OAuth 2 authorization URL.                                                                                                                                                                                                                                                                        | Mandatory  |                |
+| `token_url`             | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''             |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 code will be started.                                                                                                                                                                                                                      | Optional   | 5000           |
+| `timeout`               | Maximum amount of seconds to wait for a code or a token to be received once requested.                                                                                                                                                                                                            | Optional   | 60             |
+| `success_display_time`  | In case a code is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                           | Optional   | 1              |
+| `failure_display_time`  | In case received code is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                                | Optional   | 5000           |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | code           |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
+| `code_field_name`       | Field name containing the code.                                                                                                                                                                                                                                                                   | Optional   | code           |
+| `username`              | User name in case basic authentication should be used to retrieve token.                                                                                                                                                                                                                          | Optional   |                |
+| `password`              | User password in case basic authentication should be used to retrieve token.                                                                                                                                                                                                                      | Optional   |                |
+| `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
+
+Any other parameter will be put as query parameter in the authorization URL and as body parameters in the token URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `client_id`     | Corresponding to your Application ID (in Microsoft Azure app portal) |
+| `client_secret` | If client is not authenticated with the authorization server         |
+| `nonce`         | Refer to [OpenID ID Token specifications][3] for more details        |
+
+#### Common providers
+
+Most of [OAuth2](https://oauth.net/2/) Authorization Code Grant providers are supported.
+
+If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
+
+##### Okta (OAuth2 Authorization Code)
+
+[Okta Authorization Code Grant](https://developer.okta.com/docs/guides/implement-auth-code/overview/) providing access tokens is supported.
+
+Use `requests_auth.OktaAuthorizationCode` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OktaAuthorizationCode
+
+
+okta = OktaAuthorizationCode(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
+requests.get('https://www.example.com', auth=okta)
+```
+
+###### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
+| `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
+| `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | token                                        |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
+| `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
+| `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | openid                                       |
+| `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
+| `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
+| `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
+| `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                                              |
+
+Any other parameter will be put as query parameter in the authorization URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `prompt`        | none to avoid prompting the user if a session is already opened.     |
+
+### Authorization Code Flow with Proof Key for Code Exchange
+
+Proof Key for Code Exchange is implemented following [rfc7636](https://tools.ietf.org/html/rfc7636).
+
+Use `requests_auth.OAuth2AuthorizationCodePKCE` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OAuth2AuthorizationCodePKCE
+
+requests.get('https://www.example.com', auth=OAuth2AuthorizationCodePKCE('https://www.authorization.url', 'https://www.token.url'))
+```
+
+#### Parameters 
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
+| `authorization_url`     | OAuth 2 authorization URL.                                                                                                                                                                                                                                                                        | Mandatory  |                |
+| `token_url`             | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''             |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 code will be started.                                                                                                                                                                                                                      | Optional   | 5000           |
+| `timeout`               | Maximum amount of seconds to wait for a code or a token to be received once requested.                                                                                                                                                                                                            | Optional   | 60             |
+| `success_display_time`  | In case a code is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                           | Optional   | 1              |
+| `failure_display_time`  | In case received code is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                                | Optional   | 5000           |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | code           |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
+| `code_field_name`       | Field name containing the code.                                                                                                                                                                                                                                                                   | Optional   | code           |
+| `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
+
+Any other parameter will be put as query parameter in the authorization URL and as body parameters in the token URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `client_id`     | Corresponding to your Application ID (in Microsoft Azure app portal) |
+| `client_secret` | If client is not authenticated with the authorization server         |
+| `nonce`         | Refer to [OpenID ID Token specifications][3] for more details        |
+
+#### Common providers
+
+Most of [OAuth2](https://oauth.net/2/) Proof Key for Code Exchange providers are supported.
+
+If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
+
+##### Okta (OAuth2 Proof Key for Code Exchange)
+
+[Okta Proof Key for Code Exchange](https://developer.okta.com/docs/guides/implement-auth-code-pkce/overview/) providing access tokens is supported.
+
+Use `requests_auth.OktaAuthorizationCodePKCE` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OktaAuthorizationCodePKCE
+
+
+okta = OktaAuthorizationCodePKCE(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
+requests.get('https://www.example.com', auth=okta)
+```
+
+###### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
+| `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
+| `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | code                                         |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
+| `code_field_name`       | Field name containing the code.                                                                                                                                                                                                                                                                   | Optional   | code                                         |
+| `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
+| `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | openid                                       |
+| `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
+| `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
+| `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
+| `session`               | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                                              |
+
+Any other parameter will be put as query parameter in the authorization URL and as body parameters in the token URL.        
+
+Usual extra parameters are:
+
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `client_secret`        | If client is not authenticated with the authorization server     |
+| `nonce`        | Refer to [OpenID ID Token specifications][3] for more details     |
+
+### Resource Owner Password Credentials flow
+
+Resource Owner Password Credentials Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.3).
+
+Use `requests_auth.OAuth2ResourceOwnerPasswordCredentials` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OAuth2ResourceOwnerPasswordCredentials
+
+requests.get('https://www.example.com', auth=OAuth2ResourceOwnerPasswordCredentials('https://www.token.url', 'user name', 'user password'))
+```
+
+#### Parameters
+
+| Name               | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
+|:-------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
+| `token_url`        | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
+| `username`         | Resource owner user name.                                                                                                                                                                                                                                                                         | Mandatory  |                |
+| `password`         | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory  |                |
+| `session_auth`     | Client authentication if the client type is confidential or the client was issued client credentials (or assigned other authentication requirements). Can be a tuple or any requests authentication class instance.                                                                               | Optional  |               |
+| `timeout`          | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60             |
+| `header_name`      | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
+| `header_value`     | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
+| `scope`            | Scope parameter sent to token URL as body. Can also be a list of scopes.                                                                                                                                                                                                                          | Optional   |                |
+| `token_field_name` | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
+| `early_expiry`     | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
+| `session`          | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
+
+Any other parameter will be put as body parameter in the token URL.
+
+#### Common providers
+
+Most of [OAuth2](https://oauth.net/2/) Resource Owner Password Credentials providers are supported.
+
+If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
+
+##### Okta (OAuth2 Resource Owner Password Credentials)
+
+[Okta Resource Owner Password Credentials](https://developer.okta.com/docs/guides/implement-grant-type/ropassword/main/) providing access tokens is supported.
+
+Use `requests_auth.OktaResourceOwnerPasswordCredentials` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OktaResourceOwnerPasswordCredentials
+
+
+okta = OktaResourceOwnerPasswordCredentials(instance='testserver.okta-emea.com', username='user name', password='user password', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_secret="0c5MB")
+requests.get('https://www.example.com', auth=okta)
+```
+
+###### Parameters
+
+| Name                    | Description                | Mandatory | Default value |
+|:------------------------|:---------------------------|:----------|:--------------|
+| `instance`              | Okta instance (like "testserver.okta-emea.com"). | Mandatory |               |
+| `username`           | Resource owner user name.                                                                                                                                                                                                                                                                         | Mandatory |               |
+| `password`           | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory |               |
+| `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier). | Mandatory |               |
+| `client_secret`        | Resource owner password.     | Mandatory |               |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested. | Optional | 60 |
+| `header_name`           | Name of the header field used to send token. | Optional | Authorization |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token. | Optional | Bearer {token} |
+| `scope`                 | Scope parameter sent in query. Can also be a list of scopes. | Optional | openid |
+| `token_field_name`      | Field name containing the token. | Optional | access_token |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional  | 30.0  |
+| `session`          | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
+
+Any other parameter will be put as body parameters in the token URL.
+
+### Client Credentials flow
+
+Client Credentials Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.4).
+
+Use `requests_auth.OAuth2ClientCredentials` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OAuth2ClientCredentials
+
+requests.get('https://www.example.com', auth=OAuth2ClientCredentials('https://www.token.url', client_id='id', client_secret='secret'))
+```
+
+#### Parameters
+
+| Name               | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
+|:-------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
+| `token_url`        | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
+| `client_id`        | Resource owner user name.                                                                                                                                                                                                                                                                         | Mandatory  |                |
+| `client_secret`    | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory  |                |
+| `timeout`          | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60             |
+| `header_name`      | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
+| `header_value`     | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
+| `scope`            | Scope parameter sent to token URL as body. Can also be a list of scopes.                                                                                                                                                                                                                          | Optional   |                |
+| `token_field_name` | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
+| `early_expiry`     | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
+| `session`          | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
+
+Any other parameter will be put as body parameter in the token URL.
+
+#### Common providers
+
+Most of [OAuth2](https://oauth.net/2/) Client Credentials Grant providers are supported.
+
+If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
+
+##### Okta (OAuth2 Client Credentials)
+
+[Okta Client Credentials Grant](https://developer.okta.com/docs/guides/implement-client-creds/overview/) providing access tokens is supported.
+
+Use `requests_auth.OktaClientCredentials` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OktaClientCredentials
+
+
+okta = OktaClientCredentials(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_secret="secret")
+requests.get('https://www.example.com', auth=okta)
+```
+
+###### Parameters
+
+| Name                   | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
+|:-----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
+| `instance`             | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                |
+| `client_id`            | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                |
+| `client_secret`        | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory  |                |
+| `authorization_server` | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'      |
+| `timeout`              | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60             |
+| `header_name`          | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
+| `header_value`         | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
+| `scope`                | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | openid         |
+| `token_field_name`     | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
+| `early_expiry`         | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
+| `session`              | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
+
+Any other parameter will be put as query parameter in the token URL.        
+
+### Implicit flow
+
+Implicit Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.2).
+
+Use `requests_auth.OAuth2Implicit` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OAuth2Implicit
+
+requests.get('https://www.example.com', auth=OAuth2Implicit('https://www.authorization.url'))
+```
+
+#### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory | Default value                                                 |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:--------------------------------------------------------------|
+| `authorization_url`     | OAuth 2 authorization URL.                                                                                                                                                                                                                                                                        | Mandatory |                                                               |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional  | token                                                         |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional  | id_token if response_type is id_token, otherwise access_token |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional  | 30.0                                                          |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional  | ''                                                            |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional  | 5000                                                          |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional  | 60                                                            |
+| `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional  | 1                                                             |
+| `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional  | 5000                                                          |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional  | Authorization                                                 |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional  | Bearer {token}                                                |
+
+Any other parameter will be put as query parameter in the authorization URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `client_id`     | Corresponding to your Application ID (in Microsoft Azure app portal) |
+| `nonce`         | Refer to [OpenID ID Token specifications][3] for more details        |
+| `prompt`        | none to avoid prompting the user if a session is already opened.     |
+
+#### Common providers
+
+Most of [OAuth2](https://oauth.net/2/) Implicit Grant providers are supported.
+
+If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
+
+##### Microsoft - Azure Active Directory (OAuth2 Access Token)
+
+[Microsoft identity platform access tokens](https://docs.microsoft.com/en-us/azure/active-directory/develop/access-tokens) are supported.
+
+Use `requests_auth.AzureActiveDirectoryImplicit` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import AzureActiveDirectoryImplicit
+
+
+aad = AzureActiveDirectoryImplicit(tenant_id='45239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
+requests.get('https://www.example.com', auth=aad)
+```
+
+You can retrieve Microsoft Azure Active Directory application information thanks to the [application list on Azure portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/).
+
+###### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
+| `tenant_id`             | Microsoft Tenant Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
+| `client_id`             | Microsoft Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                   | Mandatory  |                                              |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | token                                        |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
+| `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details                                                                                                                                                                                                                                     | Optional   | Newly generated Universal Unique Identifier. |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
+| `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
+| `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
+
+Any other parameter will be put as query parameter in the authorization URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `prompt`        | none to avoid prompting the user if a session is already opened.     |
+
+##### Microsoft - Azure Active Directory (OpenID Connect ID token)
+
+[Microsoft identity platform ID tokens](https://docs.microsoft.com/en-us/azure/active-directory/develop/id-tokens) are supported.
+
+Use `requests_auth.AzureActiveDirectoryImplicitIdToken` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import AzureActiveDirectoryImplicitIdToken
+
+
+aad = AzureActiveDirectoryImplicitIdToken(tenant_id='45239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
+requests.get('https://www.example.com', auth=aad)
+```
+
+You can retrieve Microsoft Azure Active Directory application information thanks to the [application list on Azure portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/).
+
+###### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory | Default value                                |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:---------------------------------------------|
+| `tenant_id`             | Microsoft Tenant Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory |                                              |
+| `client_id`             | Microsoft Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                   | Mandatory |                                              |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional  | id_token                                     |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional  | id_token                                     |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional  | 30.0                                         |
+| `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details                                                                                                                                                                                                                                     | Optional  | Newly generated Universal Unique Identifier. |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional  | ''                                           |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional  | 5000                                         |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional  | 60                                           |
+| `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional  | 1                                            |
+| `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional  | 5000                                         |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional  | Authorization                                |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional  | Bearer {token}                               |
+
+Any other parameter will be put as query parameter in the authorization URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `prompt`        | none to avoid prompting the user if a session is already opened.     |
+
+##### Okta (OAuth2 Implicit Access Token)
+
+[Okta Implicit Grant](https://developer.okta.com/docs/guides/implement-implicit/overview/) providing access tokens is supported.
+
+Use `requests_auth.OktaImplicit` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OktaImplicit
+
+
+okta = OktaImplicit(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
+requests.get('https://www.example.com', auth=okta)
+```
+
+###### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
+| `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
+| `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | token                                        |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token                                 |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
+| `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
+| `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | ['openid', 'profile', 'email']               |
+| `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
+| `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
+| `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
+
+Any other parameter will be put as query parameter in the authorization URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `prompt`        | none to avoid prompting the user if a session is already opened.     |
+
+##### Okta (OpenID Connect Implicit ID token)
+
+[Okta Implicit Grant](https://developer.okta.com/docs/guides/implement-implicit/overview/) providing ID tokens is supported.
+
+Use `requests_auth.OktaImplicitIdToken` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OktaImplicitIdToken
+
+
+okta = OktaImplicitIdToken(instance='testserver.okta-emea.com', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd')
+requests.get('https://www.example.com', auth=okta)
+```
+
+###### Parameters
+
+| Name                    | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value                                |
+|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------------------------------------|
+| `instance`              | Okta instance (like "testserver.okta-emea.com").                                                                                                                                                                                                                                                  | Mandatory  |                                              |
+| `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier).                                                                                                                                                                                                                        | Mandatory  |                                              |
+| `response_type`         | Value of the response_type query parameter if not already provided in authorization URL.                                                                                                                                                                                                          | Optional   | id_token                                     |
+| `token_field_name`      | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | id_token                                     |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0                                         |
+| `nonce`                 | Refer to [OpenID ID Token specifications][3] for more details.                                                                                                                                                                                                                                    | Optional   | Newly generated Universal Unique Identifier. |
+| `scope`                 | Scope parameter sent in query. Can also be a list of scopes.                                                                                                                                                                                                                                      | Optional   | ['openid', 'profile', 'email']               |
+| `authorization_server`  | Okta authorization server.                                                                                                                                                                                                                                                                        | Optional   | 'default'                                    |
+| `redirect_uri_endpoint` | Custom endpoint that will be used as redirect_uri the following way: http://localhost:<redirect_uri_port>/<redirect_uri_endpoint>.                                                                                                                                                                | Optional   | ''                                           |
+| `redirect_uri_port`     | The port on which the server listening for the OAuth 2 token will be started.                                                                                                                                                                                                                     | Optional   | 5000                                         |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60                                           |
+| `success_display_time`  | In case a token is successfully received, this is the maximum amount of milliseconds the success page will be displayed in your browser.                                                                                                                                                          | Optional   | 1                                            |
+| `failure_display_time`  | In case received token is not valid, this is the maximum amount of milliseconds the failure page will be displayed in your browser.                                                                                                                                                               | Optional   | 5000                                         |
+| `header_name`           | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization                                |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token}                               |
+
+Any other parameter will be put as query parameter in the authorization URL.        
+
+Usual extra parameters are:
+        
+| Name            | Description                                                          |
+|:----------------|:---------------------------------------------------------------------|
+| `prompt`        | none to avoid prompting the user if a session is already opened.     |
+
+### Managing token cache
+
+To avoid asking for a new token every new request, a token cache is used.
+
+Default cache is in memory but it is also possible to use a physical cache.
+
+You need to provide the location of your token cache file. It can be a full or relative path.
+
+If the file already exists it will be used, if the file do not exists it will be created.
+
+```python
+from requests_auth import OAuth2, JsonTokenFileCache
+
+OAuth2.token_cache = JsonTokenFileCache('path/to/my_token_cache.json')
+```
+
+## API key in header
+
+You can send an API key inside the header of your request using `requests_auth.HeaderApiKey`.
+
+```python
+import requests
+from requests_auth import HeaderApiKey
+
+requests.get('https://www.example.com', auth=HeaderApiKey('my_api_key'))
+```
+
+### Parameters
+
+| Name                    | Description                    | Mandatory | Default value |
+|:------------------------|:-------------------------------|:----------|:--------------|
+| `api_key`               | The API key that will be sent. | Mandatory |               |
+| `header_name`           | Name of the header field.      | Optional  | "X-API-Key"   |
+
+## API key in query
+
+You can send an API key inside the query parameters of your request using `requests_auth.QueryApiKey`.
+
+```python
+import requests
+from requests_auth import QueryApiKey
+
+requests.get('https://www.example.com', auth=QueryApiKey('my_api_key'))
+```
+
+### Parameters
+
+| Name                    | Description                    | Mandatory | Default value |
+|:------------------------|:-------------------------------|:----------|:--------------|
+| `api_key`               | The API key that will be sent. | Mandatory |               |
+| `query_parameter_name`  | Name of the query parameter.   | Optional  | "api_key"     |
+
+## Basic
+
+You can use basic authentication using `requests_auth.Basic`.
+
+The only advantage of using this class instead of `requests` native support of basic authentication, is to be able to use it in [multiple authentication](#multiple-authentication-at-once).
+
+```python
+import requests
+from requests_auth import Basic
+
+requests.get('https://www.example.com', auth=Basic('username', 'password'))
+```
+
+### Parameters
+
+| Name                    | Description                    | Mandatory | Default value |
+|:------------------------|:-------------------------------|:----------|:--------------|
+| `username`              | User name.                     | Mandatory |               |
+| `password`              | User password.                 | Mandatory |               |
+
+## NTLM
+
+Requires [`requests-negotiate-sspi` module][4] or [`requests_ntlm` module][5] depending on provided parameters.
+
+You can use Windows authentication using `requests_auth.NTLM`.
+
+```python
+import requests
+from requests_auth import NTLM
+
+requests.get('https://www.example.com', auth=NTLM())
+```
+
+### Parameters
+
+| Name                    | Description                    | Mandatory | Default value |
+|:------------------------|:-------------------------------|:----------|:--------------|
+| `username`              | User name.                     | Mandatory if `requests_negotiate_sspi` module is not installed. In such a case `requests_ntlm` module is mandatory. |               |
+| `password`              | User password.                 | Mandatory if `requests_negotiate_sspi` module is not installed. In such a case `requests_ntlm` module is mandatory. |               |
+
+## Multiple authentication at once
+
+You can also use a combination of authentication using `+` or `&` as in the following sample:
+
+```python
+import requests
+from requests_auth import HeaderApiKey, OAuth2Implicit
+
+api_key = HeaderApiKey('my_api_key')
+oauth2 = OAuth2Implicit('https://www.example.com')
+requests.get('https://www.example.com', auth=api_key + oauth2)
+```
+
+## Available pytest fixtures
+
+Testing the code using `requests_auth` authentication classes can be achieved using provided [`pytest`][6] fixtures.
+
+### token_cache_mock
+
+```python
+from requests_auth.testing import token_cache_mock, token_mock
+
+def test_something(token_cache_mock):
+    # perform code using authentication
+    pass
+```
+
+Use this fixture to mock authentication success for any of the following classes:
+ * OAuth2AuthorizationCodePKCE
+ * OktaAuthorizationCodePKCE
+ * OAuth2Implicit
+ * OktaImplicit
+ * OktaImplicitIdToken
+ * AzureActiveDirectoryImplicit
+ * AzureActiveDirectoryImplicitIdToken
+ * OAuth2AuthorizationCode
+ * OktaAuthorizationCode
+ * OAuth2ClientCredentials
+ * OktaClientCredentials
+ * OAuth2ResourceOwnerPasswordCredentials,
+
+By default, an access token with value `2YotnFZFEjr1zCsicMWpAA` is generated.
+
+You can however return your custom token by providing your own `token_mock` fixture as in the following sample:
+
+```python
+import pytest
+
+from requests_auth.testing import token_cache_mock
+
+
+@pytest.fixture
+def token_mock() -> str:
+    return "MyCustomTokenValue"
+
+
+def test_something(token_cache_mock):
+    # perform code using authentication
+    pass
+```
+
+You can even return a more complex token by using the `create_token` function.
+
+Note that [`pyjwt`](https://pypi.org/project/PyJWT/) is a required dependency in this case as it is used to generate the token returned by the authentication.
+
+```python
+import pytest
+
+from requests_auth.testing import token_cache_mock, create_token
+
+
+@pytest.fixture
+def token_mock() -> str:
+    expiry = None  # TODO Compute your expiry
+    return create_token(expiry)
+
+
+def test_something(token_cache_mock):
+    # perform code using authentication
+    pass
+```
+
+### Advanced testing
+
+#### token_cache
+
+This [`pytest`][6] fixture will return the token cache and ensure it is reset at the end of the test case.
+
+```python
+from requests_auth.testing import token_cache
+
+def test_something(token_cache):
+    # perform code using authentication
+    pass
+```
+
+#### browser_mock
+
+This [`pytest`][6] fixture will allow to mock the behavior of a web browser.
+
+With this [`pytest`][6] fixture you will be allowed to fine tune your authentication related failures handling.
+
+[`pyjwt`](https://pypi.org/project/PyJWT/) is a required dependency if you use `create_token` helper function.
+
+```python
+import datetime
+
+from requests_auth.testing import browser_mock, BrowserMock, create_token
+
+def test_something(browser_mock: BrowserMock):
+    token_expiry = datetime.datetime.utcnow() + datetime.timedelta(hours=1)
+    token = create_token(token_expiry)
+    tab = browser_mock.add_response(
+        opened_url="http://url_opened_by_browser?state=1234",
+        reply_url=f"http://localhost:5000#access_token={token}&state=1234",
+    )
+
+    # perform code using authentication
+
+    tab.assert_success(
+        "You are now authenticated on 1234 You may close this tab."
+    )
+```
+
+## Endorsements
+
+> I love requests_auth. As a ~15 year pythonista, this library makes working with OAuth services a breeze. <333
+
+**Randall Degges**, Head of Evangelism, [Okta](https://developer.okta.com)
+
+[1]: https://pypi.python.org/pypi/requests "requests module"
+[2]: https://2.python-requests.org/en/master/user/authentication/ "authentication parameter on requests module"
+[3]: https://openid.net/specs/openid-connect-core-1_0.html#IDToken "OpenID ID Token specifications"
+[4]: https://pypi.python.org/pypi/requests-negotiate-sspi "requests-negotiate-sspi module"
+[5]: https://pypi.python.org/pypi/requests_ntlm "requests_ntlm module"
+[6]: https://docs.pytest.org/en/latest/ "pytest module"
```

#### html2text {}

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1 Name: requests_auth Version: 6.0.0 Summary:
-Authentication for Requests Home-page: https://colin-b.github.io/requests_auth/
-Author: Colin Bounouar Author-email: colin.bounouar.dev@gmail.com Maintainer:
-Colin Bounouar Maintainer-email: colin.bounouar.dev@gmail.com License: MIT
-Download-URL: https://pypi.org/project/requests-auth/ Project-URL: GitHub,
-https://github.com/Colin-b/requests_auth Project-URL: Changelog, https://
-github.com/Colin-b/requests_auth/blob/master/CHANGELOG.md Project-URL: Issues,
-https://github.com/Colin-b/requests_auth/issues Description:
                     ***** Authentication for Requests *****
 [pypi_version] [Build_status] [Coverage] [Code_style:_black] [Number_of_tests]
                              [Number_of_downloads]
 Provides authentication classes to be used with [`requests`][1] [authentication
 parameter][2].
                  [OAuth2] [Okta] [Azure_Active_Directory_(AD)]
                      Some of the supported authentication
@@ -227,31 +219,68 @@
 name', 'user password')) ``` #### Parameters | Name | Description | Mandatory |
 Default value | |:-------------------|:----------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------|:-----------|:---------------| | `token_url` | OAuth 2 token URL.
 | Mandatory | | | `username` | Resource owner user name. | Mandatory | | |
-`password` | Resource owner password. | Mandatory | | | `timeout` | Maximum
-amount of seconds to wait for a token to be received once requested. | Optional
-| 60 | | `header_name` | Name of the header field used to send token. |
-Optional | Authorization | | `header_value` | Format used to send the token
-value. "{token}" must be present as it will be replaced by the actual token. |
-Optional | Bearer {token} | | `scope` | Scope parameter sent to token URL as
-body. Can also be a list of scopes. | Optional | | | `token_field_name` | Field
-name containing the token. | Optional | access_token | | `early_expiry` |
-Number of seconds before actual token expiry where token will be considered as
-expired. Used to ensure token will not expire between the time of retrieval and
-the time the request reaches the actual server. Set it to 0 to deactivate this
-feature and use the same token until actual expiry. | Optional | 30.0 | |
+`password` | Resource owner password. | Mandatory | | | `session_auth` | Client
+authentication if the client type is confidential or the client was issued
+client credentials (or assigned other authentication requirements). Can be a
+tuple or any requests authentication class instance. | Optional | | | `timeout`
+| Maximum amount of seconds to wait for a token to be received once requested.
+| Optional | 60 | | `header_name` | Name of the header field used to send
+token. | Optional | Authorization | | `header_value` | Format used to send the
+token value. "{token}" must be present as it will be replaced by the actual
+token. | Optional | Bearer {token} | | `scope` | Scope parameter sent to token
+URL as body. Can also be a list of scopes. | Optional | | | `token_field_name`
+| Field name containing the token. | Optional | access_token | | `early_expiry`
+| Number of seconds before actual token expiry where token will be considered
+as expired. Used to ensure token will not expire between the time of retrieval
+and the time the request reaches the actual server. Set it to 0 to deactivate
+this feature and use the same token until actual expiry. | Optional | 30.0 | |
 `session` | `requests.Session` instance that will be used to request the token.
 Use it to provide a custom proxying rule for instance. | Optional | | Any other
-parameter will be put as body parameter in the token URL. ### Client
-Credentials flow Client Credentials Grant is implemented following [rfc6749]
-(https://tools.ietf.org/html/rfc6749#section-4.4). Use
+parameter will be put as body parameter in the token URL. #### Common providers
+Most of [OAuth2](https://oauth.net/2/) Resource Owner Password Credentials
+providers are supported. If the one you are looking for is not yet supported,
+feel free to [ask for its implementation](https://github.com/Colin-b/
+requests_auth/issues/new). ##### Okta (OAuth2 Resource Owner Password
+Credentials) [Okta Resource Owner Password Credentials](https://
+developer.okta.com/docs/guides/implement-grant-type/ropassword/main/) providing
+access tokens is supported. Use
+`requests_auth.OktaResourceOwnerPasswordCredentials` to configure this kind of
+authentication. ```python import requests from requests_auth import
+OktaResourceOwnerPasswordCredentials okta =
+OktaResourceOwnerPasswordCredentials(instance='testserver.okta-emea.com',
+username='user name', password='user password', client_id='54239d18-c68c-4c47-
+8bdd-ce71ea1d50cd', client_secret="0c5MB") requests.get('https://
+www.example.com', auth=okta) ``` ###### Parameters | Name | Description |
+Mandatory | Default value | |:------------------------|:-----------------------
+----|:----------|:--------------| | `instance` | Okta instance (like
+"testserver.okta-emea.com"). | Mandatory | | | `username` | Resource owner user
+name. | Mandatory | | | `password` | Resource owner password. | Mandatory | | |
+`client_id` | Okta Application Identifier (formatted as an Universal Unique
+Identifier). | Mandatory | | | `client_secret` | Resource owner password. |
+Mandatory | | | `timeout` | Maximum amount of seconds to wait for a token to be
+received once requested. | Optional | 60 | | `header_name` | Name of the header
+field used to send token. | Optional | Authorization | | `header_value` |
+Format used to send the token value. "{token}" must be present as it will be
+replaced by the actual token. | Optional | Bearer {token} | | `scope` | Scope
+parameter sent in query. Can also be a list of scopes. | Optional | openid | |
+`token_field_name` | Field name containing the token. | Optional | access_token
+| | `early_expiry` | Number of seconds before actual token expiry where token
+will be considered as expired. Used to ensure token will not expire between the
+time of retrieval and the time the request reaches the actual server. Set it to
+0 to deactivate this feature and use the same token until actual expiry. |
+Optional | 30.0 | | `session` | `requests.Session` instance that will be used
+to request the token. Use it to provide a custom proxying rule for instance. |
+Optional | | Any other parameter will be put as body parameters in the token
+URL. ### Client Credentials flow Client Credentials Grant is implemented
+following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.4). Use
 `requests_auth.OAuth2ClientCredentials` to configure this kind of
 authentication. ```python import requests from requests_auth import
 OAuth2ClientCredentials requests.get('https://www.example.com',
 auth=OAuth2ClientCredentials('https://www.token.url', client_id='id',
 client_secret='secret')) ``` #### Parameters | Name | Description | Mandatory |
 Default value | |:-------------------|:----------------------------------------
 -------------------------------------------------------------------------------
@@ -611,19 +640,8 @@
 Head of Evangelism, [Okta](https://developer.okta.com) [1]: https://
 pypi.python.org/pypi/requests "requests module" [2]: https://2.python-
 requests.org/en/master/user/authentication/ "authentication parameter on
 requests module" [3]: https://openid.net/specs/openid-connect-core-
 1_0.html#IDToken "OpenID ID Token specifications" [4]: https://pypi.python.org/
 pypi/requests-negotiate-sspi "requests-negotiate-sspi module" [5]: https://
 pypi.python.org/pypi/requests_ntlm "requests_ntlm module" [6]: https://
-docs.pytest.org/en/latest/ "pytest module" Keywords:
-authentication,ntlm,oauth2,azure-active-directory,azure-ad,okta,apikey,multiple
-Platform: Windows Platform: Linux Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language :: English
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Software
-Development :: Build Tools Requires-Python: >=3.6 Description-Content-Type:
-text/markdown Provides-Extra: testing
+docs.pytest.org/en/latest/ "pytest module"
```

### Comparing `requests_auth-6.0.0/README.md` & `requests_auth-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,65 @@
+Metadata-Version: 2.1
+Name: requests_auth
+Version: 7.0.0
+Summary: Authentication for Requests
+Author-email: Colin Bounouar <colin.bounouar.dev@gmail.com>
+Maintainer-email: Colin Bounouar <colin.bounouar.dev@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Colin Bounouar
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: documentation, https://colin-b.github.io/requests_auth/
+Project-URL: repository, https://github.com/Colin-b/requests_auth
+Project-URL: changelog, https://github.com/Colin-b/requests_auth/blob/master/CHANGELOG.md
+Project-URL: issues, https://github.com/Colin-b/requests_auth/issues
+Keywords: authentication,ntlm,oauth2,azure-active-directory,azure-ad,okta,apikey,multiple
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 <h2 align="center">Authentication for Requests</h2>
 
 <p align="center">
 <a href="https://pypi.org/project/requests-auth/"><img alt="pypi version" src="https://img.shields.io/pypi/v/requests_auth"></a>
 <a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Build status" src="https://github.com/Colin-b/requests_auth/workflows/Release/badge.svg"></a>
 <a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Coverage" src="https://img.shields.io/badge/coverage-100%25-brightgreen"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Number of tests" src="https://img.shields.io/badge/tests-275 passed-blue"></a>
+<a href="https://github.com/Colin-b/requests_auth/actions"><img alt="Number of tests" src="https://img.shields.io/badge/tests-305 passed-blue"></a>
 <a href="https://pypi.org/project/requests-auth/"><img alt="Number of downloads" src="https://img.shields.io/pypi/dm/requests_auth"></a>
 </p>
 
 Provides authentication classes to be used with [`requests`][1] [authentication parameter][2].
 
 <p align="center">
     <a href="https://oauth.net/2/"><img alt="OAuth2" src="https://oauth.net/images/oauth-2-sm.png"></a>
@@ -232,15 +282,15 @@
 Usual extra parameters are:
 
 | Name            | Description                                                          |
 |:----------------|:---------------------------------------------------------------------|
 | `client_secret`        | If client is not authenticated with the authorization server     |
 | `nonce`        | Refer to [OpenID ID Token specifications][3] for more details     |
 
-### Resource Owner Password Credentials flow 
+### Resource Owner Password Credentials flow
 
 Resource Owner Password Credentials Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.3).
 
 Use `requests_auth.OAuth2ResourceOwnerPasswordCredentials` to configure this kind of authentication.
 
 ```python
 import requests
@@ -252,24 +302,65 @@
 #### Parameters
 
 | Name               | Description                                                                                                                                                                                                                                                                                       | Mandatory  | Default value  |
 |:-------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:---------------|
 | `token_url`        | OAuth 2 token URL.                                                                                                                                                                                                                                                                                | Mandatory  |                |
 | `username`         | Resource owner user name.                                                                                                                                                                                                                                                                         | Mandatory  |                |
 | `password`         | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory  |                |
+| `session_auth`     | Client authentication if the client type is confidential or the client was issued client credentials (or assigned other authentication requirements). Can be a tuple or any requests authentication class instance.                                                                               | Optional  |               |
 | `timeout`          | Maximum amount of seconds to wait for a token to be received once requested.                                                                                                                                                                                                                      | Optional   | 60             |
 | `header_name`      | Name of the header field used to send token.                                                                                                                                                                                                                                                      | Optional   | Authorization  |
 | `header_value`     | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token.                                                                                                                                                                                        | Optional   | Bearer {token} |
 | `scope`            | Scope parameter sent to token URL as body. Can also be a list of scopes.                                                                                                                                                                                                                          | Optional   |                |
 | `token_field_name` | Field name containing the token.                                                                                                                                                                                                                                                                  | Optional   | access_token   |
 | `early_expiry`     | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional   | 30.0           |
 | `session`          | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
 
 Any other parameter will be put as body parameter in the token URL.
 
+#### Common providers
+
+Most of [OAuth2](https://oauth.net/2/) Resource Owner Password Credentials providers are supported.
+
+If the one you are looking for is not yet supported, feel free to [ask for its implementation](https://github.com/Colin-b/requests_auth/issues/new).
+
+##### Okta (OAuth2 Resource Owner Password Credentials)
+
+[Okta Resource Owner Password Credentials](https://developer.okta.com/docs/guides/implement-grant-type/ropassword/main/) providing access tokens is supported.
+
+Use `requests_auth.OktaResourceOwnerPasswordCredentials` to configure this kind of authentication.
+
+```python
+import requests
+from requests_auth import OktaResourceOwnerPasswordCredentials
+
+
+okta = OktaResourceOwnerPasswordCredentials(instance='testserver.okta-emea.com', username='user name', password='user password', client_id='54239d18-c68c-4c47-8bdd-ce71ea1d50cd', client_secret="0c5MB")
+requests.get('https://www.example.com', auth=okta)
+```
+
+###### Parameters
+
+| Name                    | Description                | Mandatory | Default value |
+|:------------------------|:---------------------------|:----------|:--------------|
+| `instance`              | Okta instance (like "testserver.okta-emea.com"). | Mandatory |               |
+| `username`           | Resource owner user name.                                                                                                                                                                                                                                                                         | Mandatory |               |
+| `password`           | Resource owner password.                                                                                                                                                                                                                                                                          | Mandatory |               |
+| `client_id`             | Okta Application Identifier (formatted as an Universal Unique Identifier). | Mandatory |               |
+| `client_secret`        | Resource owner password.     | Mandatory |               |
+| `timeout`               | Maximum amount of seconds to wait for a token to be received once requested. | Optional | 60 |
+| `header_name`           | Name of the header field used to send token. | Optional | Authorization |
+| `header_value`          | Format used to send the token value. "{token}" must be present as it will be replaced by the actual token. | Optional | Bearer {token} |
+| `scope`                 | Scope parameter sent in query. Can also be a list of scopes. | Optional | openid |
+| `token_field_name`      | Field name containing the token. | Optional | access_token |
+| `early_expiry`          | Number of seconds before actual token expiry where token will be considered as expired. Used to ensure token will not expire between the time of retrieval and the time the request reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry. | Optional  | 30.0  |
+| `session`          | `requests.Session` instance that will be used to request the token. Use it to provide a custom proxying rule for instance.                                                                                                                                                                        | Optional   |                |
+
+Any other parameter will be put as body parameters in the token URL.
+
 ### Client Credentials flow
 
 Client Credentials Grant is implemented following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.4).
 
 Use `requests_auth.OAuth2ClientCredentials` to configure this kind of authentication.
 
 ```python
@@ -775,8 +866,8 @@
 **Randall Degges**, Head of Evangelism, [Okta](https://developer.okta.com)
 
 [1]: https://pypi.python.org/pypi/requests "requests module"
 [2]: https://2.python-requests.org/en/master/user/authentication/ "authentication parameter on requests module"
 [3]: https://openid.net/specs/openid-connect-core-1_0.html#IDToken "OpenID ID Token specifications"
 [4]: https://pypi.python.org/pypi/requests-negotiate-sspi "requests-negotiate-sspi module"
 [5]: https://pypi.python.org/pypi/requests_ntlm "requests_ntlm module"
-[6]: https://docs.pytest.org/en/latest/ "pytest module"
+[6]: https://docs.pytest.org/en/latest/ "pytest module"
```

#### html2text {}

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1 Name: requests_auth Version: 7.0.0 Summary:
+Authentication for Requests Author-email: Colin Bounouar
+bounouar.dev@gmail.com> Maintainer-email: Colin Bounouar
+bounouar.dev@gmail.com> License: MIT License Copyright (c) 2023 Colin Bounouar
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Project-URL: documentation, https://colin-
+b.github.io/requests_auth/ Project-URL: repository, https://github.com/Colin-b/
+requests_auth Project-URL: changelog, https://github.com/Colin-b/requests_auth/
+blob/master/CHANGELOG.md Project-URL: issues, https://github.com/Colin-b/
+requests_auth/issues Keywords: authentication,ntlm,oauth2,azure-active-
+directory,azure-ad,okta,apikey,multiple Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Software
+Development :: Build Tools Requires-Python: >=3.7 Description-Content-Type:
+text/markdown Provides-Extra: testing License-File: LICENSE
                     ***** Authentication for Requests *****
 [pypi_version] [Build_status] [Coverage] [Code_style:_black] [Number_of_tests]
                              [Number_of_downloads]
 Provides authentication classes to be used with [`requests`][1] [authentication
 parameter][2].
                  [OAuth2] [Okta] [Azure_Active_Directory_(AD)]
                      Some of the supported authentication
@@ -219,31 +251,68 @@
 name', 'user password')) ``` #### Parameters | Name | Description | Mandatory |
 Default value | |:-------------------|:----------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------|:-----------|:---------------| | `token_url` | OAuth 2 token URL.
 | Mandatory | | | `username` | Resource owner user name. | Mandatory | | |
-`password` | Resource owner password. | Mandatory | | | `timeout` | Maximum
-amount of seconds to wait for a token to be received once requested. | Optional
-| 60 | | `header_name` | Name of the header field used to send token. |
-Optional | Authorization | | `header_value` | Format used to send the token
-value. "{token}" must be present as it will be replaced by the actual token. |
-Optional | Bearer {token} | | `scope` | Scope parameter sent to token URL as
-body. Can also be a list of scopes. | Optional | | | `token_field_name` | Field
-name containing the token. | Optional | access_token | | `early_expiry` |
-Number of seconds before actual token expiry where token will be considered as
-expired. Used to ensure token will not expire between the time of retrieval and
-the time the request reaches the actual server. Set it to 0 to deactivate this
-feature and use the same token until actual expiry. | Optional | 30.0 | |
+`password` | Resource owner password. | Mandatory | | | `session_auth` | Client
+authentication if the client type is confidential or the client was issued
+client credentials (or assigned other authentication requirements). Can be a
+tuple or any requests authentication class instance. | Optional | | | `timeout`
+| Maximum amount of seconds to wait for a token to be received once requested.
+| Optional | 60 | | `header_name` | Name of the header field used to send
+token. | Optional | Authorization | | `header_value` | Format used to send the
+token value. "{token}" must be present as it will be replaced by the actual
+token. | Optional | Bearer {token} | | `scope` | Scope parameter sent to token
+URL as body. Can also be a list of scopes. | Optional | | | `token_field_name`
+| Field name containing the token. | Optional | access_token | | `early_expiry`
+| Number of seconds before actual token expiry where token will be considered
+as expired. Used to ensure token will not expire between the time of retrieval
+and the time the request reaches the actual server. Set it to 0 to deactivate
+this feature and use the same token until actual expiry. | Optional | 30.0 | |
 `session` | `requests.Session` instance that will be used to request the token.
 Use it to provide a custom proxying rule for instance. | Optional | | Any other
-parameter will be put as body parameter in the token URL. ### Client
-Credentials flow Client Credentials Grant is implemented following [rfc6749]
-(https://tools.ietf.org/html/rfc6749#section-4.4). Use
+parameter will be put as body parameter in the token URL. #### Common providers
+Most of [OAuth2](https://oauth.net/2/) Resource Owner Password Credentials
+providers are supported. If the one you are looking for is not yet supported,
+feel free to [ask for its implementation](https://github.com/Colin-b/
+requests_auth/issues/new). ##### Okta (OAuth2 Resource Owner Password
+Credentials) [Okta Resource Owner Password Credentials](https://
+developer.okta.com/docs/guides/implement-grant-type/ropassword/main/) providing
+access tokens is supported. Use
+`requests_auth.OktaResourceOwnerPasswordCredentials` to configure this kind of
+authentication. ```python import requests from requests_auth import
+OktaResourceOwnerPasswordCredentials okta =
+OktaResourceOwnerPasswordCredentials(instance='testserver.okta-emea.com',
+username='user name', password='user password', client_id='54239d18-c68c-4c47-
+8bdd-ce71ea1d50cd', client_secret="0c5MB") requests.get('https://
+www.example.com', auth=okta) ``` ###### Parameters | Name | Description |
+Mandatory | Default value | |:------------------------|:-----------------------
+----|:----------|:--------------| | `instance` | Okta instance (like
+"testserver.okta-emea.com"). | Mandatory | | | `username` | Resource owner user
+name. | Mandatory | | | `password` | Resource owner password. | Mandatory | | |
+`client_id` | Okta Application Identifier (formatted as an Universal Unique
+Identifier). | Mandatory | | | `client_secret` | Resource owner password. |
+Mandatory | | | `timeout` | Maximum amount of seconds to wait for a token to be
+received once requested. | Optional | 60 | | `header_name` | Name of the header
+field used to send token. | Optional | Authorization | | `header_value` |
+Format used to send the token value. "{token}" must be present as it will be
+replaced by the actual token. | Optional | Bearer {token} | | `scope` | Scope
+parameter sent in query. Can also be a list of scopes. | Optional | openid | |
+`token_field_name` | Field name containing the token. | Optional | access_token
+| | `early_expiry` | Number of seconds before actual token expiry where token
+will be considered as expired. Used to ensure token will not expire between the
+time of retrieval and the time the request reaches the actual server. Set it to
+0 to deactivate this feature and use the same token until actual expiry. |
+Optional | 30.0 | | `session` | `requests.Session` instance that will be used
+to request the token. Use it to provide a custom proxying rule for instance. |
+Optional | | Any other parameter will be put as body parameters in the token
+URL. ### Client Credentials flow Client Credentials Grant is implemented
+following [rfc6749](https://tools.ietf.org/html/rfc6749#section-4.4). Use
 `requests_auth.OAuth2ClientCredentials` to configure this kind of
 authentication. ```python import requests from requests_auth import
 OAuth2ClientCredentials requests.get('https://www.example.com',
 auth=OAuth2ClientCredentials('https://www.token.url', client_id='id',
 client_secret='secret')) ``` #### Parameters | Name | Description | Mandatory |
 Default value | |:-------------------|:----------------------------------------
 -------------------------------------------------------------------------------
```

### Comparing `requests_auth-6.0.0/requests_auth/__init__.py` & `requests_auth-7.0.0/requests_auth/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     AzureActiveDirectoryImplicit,
     AzureActiveDirectoryImplicitIdToken,
     OAuth2AuthorizationCode,
     OktaAuthorizationCode,
     OAuth2ClientCredentials,
     OktaClientCredentials,
     OAuth2ResourceOwnerPasswordCredentials,
+    OktaResourceOwnerPasswordCredentials,
 )
 from requests_auth.oauth2_tokens import JsonTokenFileCache
 from requests_auth.errors import (
     GrantNotProvided,
     TimeoutOccurred,
     AuthenticationFailed,
     StateNotProvided,
```

### Comparing `requests_auth-6.0.0/requests_auth/authentication.py` & `requests_auth-7.0.0/requests_auth/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,17 @@
     """
 
     def __init__(self, token_url: str, username: str, password: str, **kwargs):
         """
         :param token_url: OAuth 2 token URL.
         :param username: Resource owner user name.
         :param password: Resource owner password.
+        :param session_auth: Client authentication if the client type is confidential
+        or the client was issued client credentials (or assigned other authentication requirements).
+        Can be a tuple or any requests authentication class instance.
         :param timeout: Maximum amount of seconds to wait for a token to be received once requested.
         Wait for 1 minute by default.
         :param header_name: Name of the header field used to send token.
         Token will be sent in Authorization header field by default.
         :param header_value: Format used to send the token value.
         "{token}" must be present as it will be replaced by the actual token.
         Token will be sent as "Bearer {token}" by default.
@@ -173,15 +176,17 @@
 
         self.token_field_name = kwargs.pop("token_field_name", None) or "access_token"
         self.early_expiry = float(kwargs.pop("early_expiry", None) or 30.0)
 
         # Time is expressed in seconds
         self.timeout = int(kwargs.pop("timeout", None) or 60)
         self.session = kwargs.pop("session", None) or requests.Session()
-        self.session.auth = (self.username, self.password)
+        session_auth = kwargs.pop("session_auth", None)
+        if session_auth:
+            self.session.auth = session_auth
 
         # As described in https://tools.ietf.org/html/rfc6749#section-4.3.2
         self.data = {
             "grant_type": "password",
             "username": self.username,
             "password": self.password,
         }
@@ -1183,14 +1188,72 @@
             f"https://{instance}/oauth2/{authorization_server}/v1/token",
             client_id=client_id,
             client_secret=client_secret,
             **kwargs,
         )
 
 
+class OktaResourceOwnerPasswordCredentials(OAuth2ResourceOwnerPasswordCredentials):
+    """
+    Describes an Okta (OAuth 2) resource owner password credentials (also called password) flow requests authentication.
+    """
+
+    def __init__(
+        self,
+        instance: str,
+        username: str,
+        password: str,
+        client_id: str,
+        client_secret: str,
+        **kwargs,
+    ):
+        """
+        :param instance: Okta instance (like "testserver.okta-emea.com")
+        :param username: Resource owner user name.
+        :param password: Resource owner password.
+        :param client_id: Okta Application Identifier (formatted as an Universal Unique Identifier)
+        :param client_secret: Resource owner password.
+        :param authorization_server: Okta authorization server
+        default by default.
+        :param timeout: Maximum amount of seconds to wait for a token to be received once requested.
+        Wait for 1 minute by default.
+        :param header_name: Name of the header field used to send token.
+        Token will be sent in Authorization header field by default.
+        :param header_value: Format used to send the token value.
+        "{token}" must be present as it will be replaced by the actual token.
+        Token will be sent as "Bearer {token}" by default.
+        :param scope: Scope parameter sent to token URL as body. Can also be a list of scopes.
+        Request 'openid' by default.
+        :param token_field_name: Field name containing the token. access_token by default.
+        :param early_expiry: Number of seconds before actual token expiry where token will be considered as expired.
+        Default to 30 seconds to ensure token will not expire between the time of retrieval and the time the request
+        reaches the actual server. Set it to 0 to deactivate this feature and use the same token until actual expiry.
+        :param session: requests.Session instance that will be used to request the token.
+        Use it to provide a custom proxying rule for instance.
+        :param kwargs: all additional authorization parameters that should be put as body parameters in the token URL.
+        """
+        if not instance:
+            raise Exception("Instance is mandatory.")
+        if not client_id:
+            raise Exception("Client ID is mandatory.")
+        if not client_secret:
+            raise Exception("Client secret is mandatory.")
+        authorization_server = kwargs.pop("authorization_server", None) or "default"
+        scopes = kwargs.pop("scope", "openid")
+        kwargs["scope"] = " ".join(scopes) if isinstance(scopes, list) else scopes
+        OAuth2ResourceOwnerPasswordCredentials.__init__(
+            self,
+            f"https://{instance}/oauth2/{authorization_server}/v1/token",
+            username=username,
+            password=password,
+            session_auth=(client_id, client_secret),
+            **kwargs,
+        )
+
+
 class HeaderApiKey(requests.auth.AuthBase, SupportMultiAuth):
     """Describes an API Key requests authentication."""
 
     def __init__(self, api_key: str, header_name: str = None):
         """
         :param api_key: The API key that will be sent.
         :param header_name: Name of the header field. "X-API-Key" by default.
```

### Comparing `requests_auth-6.0.0/requests_auth/errors.py` & `requests_auth-7.0.0/requests_auth/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from json import JSONDecodeError
 from typing import Union
 
 from requests import Response
 
 
 class AuthenticationFailed(Exception):
-    """ User was not authenticated. """
+    """User was not authenticated."""
 
     def __init__(self):
         Exception.__init__(self, "User was not authenticated.")
 
 
 class TimeoutOccurred(Exception):
-    """ No response within timeout interval. """
+    """No response within timeout interval."""
 
     def __init__(self, timeout: float):
         Exception.__init__(
             self, f"User authentication was not received within {timeout} seconds."
         )
 
 
 class InvalidToken(Exception):
-    """ Token is invalid. """
+    """Token is invalid."""
 
     def __init__(self, token_name: str):
         Exception.__init__(self, f"{token_name} is invalid.")
 
 
 class GrantNotProvided(Exception):
-    """ Grant was not provided. """
+    """Grant was not provided."""
 
     def __init__(self, grant_name: str, dictionary_without_grant: dict):
         Exception.__init__(
             self, f"{grant_name} not provided within {dictionary_without_grant}."
         )
 
 
@@ -111,20 +111,20 @@
                 message += f"\nAdditional information: {content}"
         else:
             message = f"{content}"
         return message
 
 
 class StateNotProvided(Exception):
-    """ State was not provided. """
+    """State was not provided."""
 
     def __init__(self, dictionary_without_state: dict):
         Exception.__init__(
             self, f"state not provided within {dictionary_without_state}."
         )
 
 
 class TokenExpiryNotProvided(Exception):
-    """ Token expiry was not provided. """
+    """Token expiry was not provided."""
 
     def __init__(self, token_body: dict):
         Exception.__init__(self, f"Expiry (exp) is not provided in {token_body}.")
```

### Comparing `requests_auth-6.0.0/requests_auth/oauth2_authentication_responses_server.py` & `requests_auth-7.0.0/requests_auth/oauth2_authentication_responses_server.py`

 * *Files identical despite different names*

### Comparing `requests_auth-6.0.0/requests_auth/oauth2_tokens.py` & `requests_auth-7.0.0/requests_auth/oauth2_tokens.py`

 * *Files identical despite different names*

### Comparing `requests_auth-6.0.0/requests_auth/testing.py` & `requests_auth-7.0.0/requests_auth/testing.py`

 * *Files identical despite different names*

### Comparing `requests_auth-6.0.0/setup.py` & `requests_auth-7.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-import os
-from setuptools import setup, find_packages
+[build-system]
+requires = ["setuptools", "setuptools_scm"]
+build-backend = "setuptools.build_meta"
 
-this_dir = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_dir, "README.md"), "r") as f:
-    long_description = f.read()
+[project]
+name = "requests_auth"
+description = "Authentication for Requests"
+readme = "README.md"
+requires-python = ">=3.7"
+license = {file = "LICENSE"}
+authors = [
+    {name = "Colin Bounouar", email = "colin.bounouar.dev@gmail.com" }
+]
+maintainers = [
+    {name = "Colin Bounouar", email = "colin.bounouar.dev@gmail.com" }
+]
+keywords = [
+    "authentication",
+    "ntlm",
+    "oauth2",
+    "azure-active-directory",
+    "azure-ad",
+    "okta",
+    "apikey",
+    "multiple",
+]
+classifiers=[
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Build Tools",
+]
+dependencies = [
+    "requests==2.*",
+]
+dynamic = ["version"]
 
-# More information on properties: https://packaging.python.org/distributing
-setup(
-    name="requests_auth",
-    version=open("requests_auth/version.py").readlines()[-1].split()[-1].strip("\"'"),
-    author="Colin Bounouar",
-    author_email="colin.bounouar.dev@gmail.com",
-    maintainer="Colin Bounouar",
-    maintainer_email="colin.bounouar.dev@gmail.com",
-    url="https://colin-b.github.io/requests_auth/",
-    description="Authentication for Requests",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    download_url="https://pypi.org/project/requests-auth/",
-    license="MIT",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Topic :: Software Development :: Build Tools",
-    ],
-    keywords=[
-        "authentication",
-        "ntlm",
-        "oauth2",
-        "azure-active-directory",
-        "azure-ad",
-        "okta",
-        "apikey",
-        "multiple",
-    ],
-    packages=find_packages(exclude=["tests*"]),
-    install_requires=[
-        # Used for Base Authentication and to communicate with OAuth2 servers
-        "requests==2.*"
-    ],
-    extras_require={
-        "testing": [
-            # Used to generate test tokens
-            "pyjwt==2.*",
-            # Used to mock responses to requests
-            "pytest-responses==0.5.*",
-            # Used to check coverage
-            "pytest-cov==3.*",
-        ]
-    },
-    python_requires=">=3.6",
-    project_urls={
-        "GitHub": "https://github.com/Colin-b/requests_auth",
-        "Changelog": "https://github.com/Colin-b/requests_auth/blob/master/CHANGELOG.md",
-        "Issues": "https://github.com/Colin-b/requests_auth/issues",
-    },
-    platforms=["Windows", "Linux"],
-)
+[project.urls]
+documentation = "https://colin-b.github.io/requests_auth/"
+repository = "https://github.com/Colin-b/requests_auth"
+changelog = "https://github.com/Colin-b/requests_auth/blob/master/CHANGELOG.md"
+issues = "https://github.com/Colin-b/requests_auth/issues"
+
+[project.optional-dependencies]
+testing = [
+    # Used to generate test tokens
+    "pyjwt==2.*",
+    # Used to mock requests
+    "pytest-responses==0.5.*",
+    # Used to check coverage
+    "pytest-cov==4.*",
+]
+
+[tool.setuptools.packages.find]
+exclude = ["tests*"]
+
+[tool.setuptools.dynamic]
+version = {attr = "requests_auth.version.__version__"}
```

