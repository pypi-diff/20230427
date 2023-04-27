# Comparing `tmp/lmk_python-0.0.5.tar.gz` & `tmp/lmk_python-0.0.7.tar.gz`

## Comparing `lmk_python-0.0.5.tar` & `lmk_python-0.0.7.tar`

### file list

```diff
@@ -1,124 +1,142 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lmk_python-0.0.5/.openapi-generator-ignore
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 lmk_python-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 lmk_python-0.0.5/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 lmk_python-0.0.5/babel.config.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 lmk_python-0.0.5/install.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk.json
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 lmk_python-0.0.5/npm.README.md
--rw-r--r--   0        0        0    27121 2020-02-02 00:00:00.000000 lmk_python-0.0.5/openapi.yaml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 lmk_python-0.0.5/openapitools.json
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 lmk_python-0.0.5/package.json
--rw-r--r--   0        0        0   263108 2020-02-02 00:00:00.000000 lmk_python-0.0.5/pnpm-lock.yaml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 lmk_python-0.0.5/setup.cfg
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 lmk_python-0.0.5/setup.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 lmk_python-0.0.5/tailwind-labextension.config.js
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 lmk_python-0.0.5/tailwind-nbextension.config.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lmk_python-0.0.5/tsconfig.build.json
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 lmk_python-0.0.5/tsconfig.json
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 lmk_python-0.0.5/webpack.config.js
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/__init__.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/api_client.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/auth.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/constants.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/exc.py
--rw-r--r--   0        0        0    17155 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/instance.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/methods.py
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/__init__.py
--rw-r--r--   0        0        0    29539 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api_client.py
--rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/configuration.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/exceptions.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/rest.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/__init__.py
--rw-r--r--   0        0        0    28903 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/app_api.py
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/auth_api.py
--rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/event_api.py
--rw-r--r--   0        0        0    37283 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/headless_auth_api.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/healthcheck_api.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/notification_api.py
--rw-r--r--   0        0        0    22115 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/oauth_api.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/session_api.py
--rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/api/user_api.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/__init__.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/access_token_request.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/access_token_response.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/actor_response.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/app_connection_response.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/app_response.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/create_app_request.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/create_headless_auth_session_request.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/create_notification_channel_request.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/create_notification_channel_request_payload.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/create_session_request.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/create_user_request.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/create_user_response.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/email_channel_payload.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/event_notification_configuration.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/event_request.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/event_response.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/events_response.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/headless_auth_refresh_token_request.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/headless_auth_session_response.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/initiate_oauth_request.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/initiate_oauth_response.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/list_connected_apps_item_response.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/list_connected_apps_response.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/login_request.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/notification_channel_info.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/notification_channel_response.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/notification_channels_response.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/oauth_error.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/owned_app_response.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/reorder_notification_channels_request.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/reorder_notification_channels_request_item.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/session_response.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/set_password_request.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/text_message_channel_payload.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/token_response.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/update_notification_channel_request.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/update_user_request.py
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/generated/models/user_response.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/constants.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/history.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/hooks.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/magics.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/methods.py
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/notebook_info.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/utils.py
--rw-r--r--   0        0        0    21310 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/widget.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/package.json
--rw-r--r--   0        0        0  1193411 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/399.49345c52b42d87d9afb9.js
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/399.49345c52b42d87d9afb9.js.LICENSE.txt
--rw-r--r--   0        0        0    24681 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/568.20579847b1912c2a38d6.js
--rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/582.2007fa97241e6df13205.js
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/875.e1becc2c9f68a75184b9.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/875.e1becc2c9f68a75184b9.js.LICENSE.txt
--rw-r--r--   0        0        0  1013150 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js.LICENSE.txt
--rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/remoteEntry.433f22a9050fe1c09832.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/style.js
--rw-r--r--   0        0        0    26613 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/third-party-licenses.json
--rw-r--r--   0        0        0  1460992 2020-02-02 00:00:00.000000 lmk_python-0.0.5/lmk/jupyter/nbextension/lmk-jupyter.js
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/extension.ts
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/globals.d.ts
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/index.ts
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/plugin.ts
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/version.ts
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/widget.ts
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/components/Auth.tsx
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/components/Layout.tsx
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/components/Loader.tsx
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/components/Navbar.tsx
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/components/Widget.tsx
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/components/WidgetContent.tsx
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/hooks/click-outside.ts
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/hooks/model.ts
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/hooks/now.ts
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 lmk_python-0.0.5/src/lib/widget-model.ts
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 lmk_python-0.0.5/styles/Loader.css
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 lmk_python-0.0.5/styles/tailwind.css
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lmk_python-0.0.5/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lmk_python-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 lmk_python-0.0.5/README.md
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 lmk_python-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 lmk_python-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lmk_python-0.0.7/.openapi-generator-ignore
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 lmk_python-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 lmk_python-0.0.7/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 lmk_python-0.0.7/babel.config.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 lmk_python-0.0.7/install.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk.json
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 lmk_python-0.0.7/npm.README.md
+-rw-r--r--   0        0        0    27121 2020-02-02 00:00:00.000000 lmk_python-0.0.7/openapi.yaml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 lmk_python-0.0.7/openapitools.json
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 lmk_python-0.0.7/package.json
+-rw-r--r--   0        0        0   263108 2020-02-02 00:00:00.000000 lmk_python-0.0.7/pnpm-lock.yaml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 lmk_python-0.0.7/setup.cfg
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 lmk_python-0.0.7/setup.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 lmk_python-0.0.7/tailwind-labextension.config.js
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 lmk_python-0.0.7/tailwind-nbextension.config.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lmk_python-0.0.7/tsconfig.build.json
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 lmk_python-0.0.7/tsconfig.json
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 lmk_python-0.0.7/webpack.config.js
+-rw-r--r--   0        0        0   253775 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/Extension Test.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/Untitled.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/Untitled1.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/Untitled2.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/Untitled3.ipynb
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/Untitled4.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/Untitled5.ipynb
+-rw-r--r--   0        0        0   150415 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/poetry.lock
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/untitled.md
+-rw-r--r--   0        0        0   254815 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/Extension Test-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/Untitled1-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/Untitled2-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/Untitled3-checkpoint.ipynb
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/Untitled4-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/Untitled5-checkpoint.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmk_python-0.0.7/examples/jupyter-example/.ipynb_checkpoints/untitled-checkpoint.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/__init__.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/api_client.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/auth.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/constants.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/exc.py
+-rw-r--r--   0        0        0    17155 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/instance.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/methods.py
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/__init__.py
+-rw-r--r--   0        0        0    29539 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api_client.py
+-rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/configuration.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/exceptions.py
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/rest.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/__init__.py
+-rw-r--r--   0        0        0    28903 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/app_api.py
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/auth_api.py
+-rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/event_api.py
+-rw-r--r--   0        0        0    37283 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/headless_auth_api.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/healthcheck_api.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/notification_api.py
+-rw-r--r--   0        0        0    22115 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/oauth_api.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/session_api.py
+-rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/api/user_api.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/__init__.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/access_token_request.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/access_token_response.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/actor_response.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/app_connection_response.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/app_response.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/create_app_request.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/create_headless_auth_session_request.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/create_notification_channel_request.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/create_notification_channel_request_payload.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/create_session_request.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/create_user_request.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/create_user_response.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/email_channel_payload.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/event_notification_configuration.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/event_request.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/event_response.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/events_response.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/headless_auth_refresh_token_request.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/headless_auth_session_response.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/initiate_oauth_request.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/initiate_oauth_response.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/list_connected_apps_item_response.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/list_connected_apps_response.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/login_request.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/notification_channel_info.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/notification_channel_response.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/notification_channels_response.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/oauth_error.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/owned_app_response.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/reorder_notification_channels_request.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/reorder_notification_channels_request_item.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/session_response.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/set_password_request.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/text_message_channel_payload.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/token_response.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/update_notification_channel_request.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/update_user_request.py
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/generated/models/user_response.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/constants.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/history.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/hooks.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/magics.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/methods.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/notebook_info.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/utils.py
+-rw-r--r--   0        0        0    21310 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/widget.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/package.json
+-rw-r--r--   0        0        0  1193411 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/399.c2165748a9b3b2c7908d.js
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/399.c2165748a9b3b2c7908d.js.LICENSE.txt
+-rw-r--r--   0        0        0    24681 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/568.12d21aceee689bf3ed6f.js
+-rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/582.2007fa97241e6df13205.js
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/875.e1becc2c9f68a75184b9.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/875.e1becc2c9f68a75184b9.js.LICENSE.txt
+-rw-r--r--   0        0        0  1013150 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js.LICENSE.txt
+-rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/remoteEntry.b02170963b4d89253004.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/style.js
+-rw-r--r--   0        0        0    26613 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/third-party-licenses.json
+-rw-r--r--   0        0        0  1460992 2020-02-02 00:00:00.000000 lmk_python-0.0.7/lmk/jupyter/nbextension/lmk-jupyter.js
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/extension.ts
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/globals.d.ts
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/index.ts
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/plugin.ts
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/version.ts
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/widget.ts
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/components/Auth.tsx
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/components/Layout.tsx
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/components/Loader.tsx
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/components/Navbar.tsx
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/components/Widget.tsx
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/components/WidgetContent.tsx
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/hooks/click-outside.ts
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/hooks/model.ts
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/hooks/now.ts
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 lmk_python-0.0.7/src/lib/widget-model.ts
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 lmk_python-0.0.7/styles/Loader.css
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 lmk_python-0.0.7/styles/tailwind.css
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lmk_python-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lmk_python-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 lmk_python-0.0.7/README.md
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 lmk_python-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 lmk_python-0.0.7/PKG-INFO
```

### Comparing `lmk_python-0.0.5/.openapi-generator-ignore` & `lmk_python-0.0.7/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/CHANGELOG.md` & `lmk_python-0.0.7/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.0.7] - 2023-04-19
+
+- Update plugin version spec to use a tilde because caret isn't working for some reason
+
+## [0.0.6] - 2023-04-19
+
+- Fix jupyter extension asset paths in `pyproject.toml`
+
 ## [0.0.5] - 2023-04-19
 
 - Add missing `typing_extensions` and `urllib3` dependencies
 
 ## [0.0.4] - 2023-04-19
 
 - Published package to pypi
```

### Comparing `lmk_python-0.0.5/MANIFEST.in` & `lmk_python-0.0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/openapi.yaml` & `lmk_python-0.0.7/openapi.yaml`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/openapitools.json` & `lmk_python-0.0.7/openapitools.json`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/package.json` & `lmk_python-0.0.7/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.0.7'"}*

```diff
@@ -130,9 +130,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w -p tsconfig.build.json",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.0.5"
+    "version": "0.0.7"
 }
```

### Comparing `lmk_python-0.0.5/pnpm-lock.yaml` & `lmk_python-0.0.7/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/tailwind-labextension.config.js` & `lmk_python-0.0.7/tailwind-labextension.config.js`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/tailwind-nbextension.config.js` & `lmk_python-0.0.7/tailwind-nbextension.config.js`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/tsconfig.json` & `lmk_python-0.0.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/webpack.config.js` & `lmk_python-0.0.7/webpack.config.js`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/__init__.py` & `lmk_python-0.0.7/lmk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from lmk import jupyter, methods
 from lmk.instance import get_instance, set_instance
 from lmk.jupyter import (
     _jupyter_labextension_paths,
     _jupyter_nbextension_paths,
 )
 
-__version__ = "0.0.5"
+__version__ = "0.0.7"
 
 __all__ = [
     "__version__",
     "jupyter",
     "get_instance",
     "set_instance",
     "_jupyter_labextension_paths",
```

### Comparing `lmk_python-0.0.5/lmk/api_client.py` & `lmk_python-0.0.7/lmk/api_client.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/exc.py` & `lmk_python-0.0.7/lmk/exc.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/instance.py` & `lmk_python-0.0.7/lmk/instance.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/__init__.py` & `lmk_python-0.0.7/lmk/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api_client.py` & `lmk_python-0.0.7/lmk/generated/api_client.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/configuration.py` & `lmk_python-0.0.7/lmk/generated/configuration.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/exceptions.py` & `lmk_python-0.0.7/lmk/generated/exceptions.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/rest.py` & `lmk_python-0.0.7/lmk/generated/rest.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/__init__.py` & `lmk_python-0.0.7/lmk/generated/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/app_api.py` & `lmk_python-0.0.7/lmk/generated/api/app_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/auth_api.py` & `lmk_python-0.0.7/lmk/generated/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/event_api.py` & `lmk_python-0.0.7/lmk/generated/api/event_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/headless_auth_api.py` & `lmk_python-0.0.7/lmk/generated/api/headless_auth_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/healthcheck_api.py` & `lmk_python-0.0.7/lmk/generated/api/healthcheck_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/notification_api.py` & `lmk_python-0.0.7/lmk/generated/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/oauth_api.py` & `lmk_python-0.0.7/lmk/generated/api/oauth_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/session_api.py` & `lmk_python-0.0.7/lmk/generated/api/session_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/api/user_api.py` & `lmk_python-0.0.7/lmk/generated/api/user_api.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/__init__.py` & `lmk_python-0.0.7/lmk/generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/access_token_request.py` & `lmk_python-0.0.7/lmk/generated/models/access_token_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/access_token_response.py` & `lmk_python-0.0.7/lmk/generated/models/access_token_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/actor_response.py` & `lmk_python-0.0.7/lmk/generated/models/actor_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/app_connection_response.py` & `lmk_python-0.0.7/lmk/generated/models/app_connection_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/app_response.py` & `lmk_python-0.0.7/lmk/generated/models/app_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/create_app_request.py` & `lmk_python-0.0.7/lmk/generated/models/create_app_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/create_headless_auth_session_request.py` & `lmk_python-0.0.7/lmk/generated/models/create_headless_auth_session_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/create_notification_channel_request.py` & `lmk_python-0.0.7/lmk/generated/models/create_notification_channel_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/create_notification_channel_request_payload.py` & `lmk_python-0.0.7/lmk/generated/models/create_notification_channel_request_payload.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/create_session_request.py` & `lmk_python-0.0.7/lmk/generated/models/create_session_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/create_user_request.py` & `lmk_python-0.0.7/lmk/generated/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/create_user_response.py` & `lmk_python-0.0.7/lmk/generated/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/email_channel_payload.py` & `lmk_python-0.0.7/lmk/generated/models/email_channel_payload.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/event_notification_configuration.py` & `lmk_python-0.0.7/lmk/generated/models/event_notification_configuration.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/event_request.py` & `lmk_python-0.0.7/lmk/generated/models/event_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/event_response.py` & `lmk_python-0.0.7/lmk/generated/models/event_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/events_response.py` & `lmk_python-0.0.7/lmk/generated/models/events_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/headless_auth_refresh_token_request.py` & `lmk_python-0.0.7/lmk/generated/models/headless_auth_refresh_token_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/headless_auth_session_response.py` & `lmk_python-0.0.7/lmk/generated/models/headless_auth_session_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/initiate_oauth_request.py` & `lmk_python-0.0.7/lmk/generated/models/initiate_oauth_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/initiate_oauth_response.py` & `lmk_python-0.0.7/lmk/generated/models/initiate_oauth_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/list_connected_apps_item_response.py` & `lmk_python-0.0.7/lmk/generated/models/list_connected_apps_item_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/list_connected_apps_response.py` & `lmk_python-0.0.7/lmk/generated/models/list_connected_apps_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/login_request.py` & `lmk_python-0.0.7/lmk/generated/models/login_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/notification_channel_info.py` & `lmk_python-0.0.7/lmk/generated/models/notification_channel_info.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/notification_channel_response.py` & `lmk_python-0.0.7/lmk/generated/models/notification_channel_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/notification_channels_response.py` & `lmk_python-0.0.7/lmk/generated/models/notification_channels_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/oauth_error.py` & `lmk_python-0.0.7/lmk/generated/models/oauth_error.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/owned_app_response.py` & `lmk_python-0.0.7/lmk/generated/models/owned_app_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/reorder_notification_channels_request.py` & `lmk_python-0.0.7/lmk/generated/models/reorder_notification_channels_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/reorder_notification_channels_request_item.py` & `lmk_python-0.0.7/lmk/generated/models/reorder_notification_channels_request_item.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/session_response.py` & `lmk_python-0.0.7/lmk/generated/models/session_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/set_password_request.py` & `lmk_python-0.0.7/lmk/generated/models/set_password_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/text_message_channel_payload.py` & `lmk_python-0.0.7/lmk/generated/models/text_message_channel_payload.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/token_response.py` & `lmk_python-0.0.7/lmk/generated/models/token_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/update_notification_channel_request.py` & `lmk_python-0.0.7/lmk/generated/models/update_notification_channel_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/update_user_request.py` & `lmk_python-0.0.7/lmk/generated/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/generated/models/user_response.py` & `lmk_python-0.0.7/lmk/generated/models/user_response.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/__init__.py` & `lmk_python-0.0.7/lmk/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/history.py` & `lmk_python-0.0.7/lmk/jupyter/history.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/hooks.py` & `lmk_python-0.0.7/lmk/jupyter/hooks.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/magics.py` & `lmk_python-0.0.7/lmk/jupyter/magics.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/notebook_info.py` & `lmk_python-0.0.7/lmk/jupyter/notebook_info.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/utils.py` & `lmk_python-0.0.7/lmk/jupyter/utils.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/widget.py` & `lmk_python-0.0.7/lmk/jupyter/widget.py`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/package.json` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b02170963b4d89253004.js'}}",*

 * * "'version'": "'0.0.7'"}*

```diff
@@ -70,15 +70,15 @@
         "dist/*.js",
         "styles/*.css"
     ],
     "homepage": "https://app.lmkapp.dev",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.433f22a9050fe1c09832.js"
+            "load": "static/remoteEntry.b02170963b4d89253004.js"
         },
         "extension": "dist/plugin",
         "outputDir": "lmk/jupyter/labextension/lmk-jupyter",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -134,9 +134,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w -p tsconfig.build.json",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.0.5"
+    "version": "0.0.7"
 }
```

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/399.49345c52b42d87d9afb9.js` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/399.c2165748a9b3b2c7908d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 399.49345c52b42d87d9afb9.js.LICENSE.txt */
+/*! For license information please see 399.c2165748a9b3b2c7908d.js.LICENSE.txt */
 (self.webpackChunklmk_jupyter = self.webpackChunklmk_jupyter || []).push([
     [399], {
         399: (c, e, a) => {
             (() => {
                 var e = {
                         5513: (c, e, a) => {
                             (e = a(1211)(!1)).push([c.id, '/*\n! tailwindcss v3.3.1 | MIT License | https://tailwindcss.com\n*//*\n1. Prevent padding and border from affecting element width. (https://github.com/mozdevs/cssremedy/issues/4)\n2. Allow adding a border to an element by just adding a border-width. (https://github.com/tailwindcss/tailwindcss/pull/116)\n*/\n\n*,\n::before,\n::after {\n  box-sizing: border-box; /* 1 */\n  border-width: 0; /* 2 */\n  border-style: solid; /* 2 */\n  border-color: currentColor; /* 2 */\n}\n\n::before,\n::after {\n  --tw-content: \'\';\n}\n\n/*\n1. Use a consistent sensible line-height in all browsers.\n2. Prevent adjustments of font size after orientation changes in iOS.\n3. Use a more readable tab size.\n4. Use the user\'s configured `sans` font-family by default.\n5. Use the user\'s configured `sans` font-feature-settings by default.\n6. Use the user\'s configured `sans` font-variation-settings by default.\n*/\n\nhtml {\n  line-height: 1.5; /* 1 */\n  -webkit-text-size-adjust: 100%; /* 2 */\n  -moz-tab-size: 4; /* 3 */\n  -o-tab-size: 4;\n     tab-size: 4; /* 3 */\n  font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, sans-serif, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"; /* 4 */\n  font-feature-settings: normal; /* 5 */\n  font-variation-settings: normal; /* 6 */\n}\n\n/*\n1. Remove the margin in all browsers.\n2. Inherit line-height from `html` so users can set them as a class directly on the `html` element.\n*/\n\nbody {\n  margin: 0; /* 1 */\n  line-height: inherit; /* 2 */\n}\n\n/*\n1. Add the correct height in Firefox.\n2. Correct the inheritance of border color in Firefox. (https://bugzilla.mozilla.org/show_bug.cgi?id=190655)\n3. Ensure horizontal rules are visible by default.\n*/\n\nhr {\n  height: 0; /* 1 */\n  color: inherit; /* 2 */\n  border-top-width: 1px; /* 3 */\n}\n\n/*\nAdd the correct text decoration in Chrome, Edge, and Safari.\n*/\n\nabbr:where([title]) {\n  text-decoration: underline;\n  -webkit-text-decoration: underline dotted;\n          text-decoration: underline dotted;\n}\n\n/*\nRemove the default font size and weight for headings.\n*/\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6 {\n  font-size: inherit;\n  font-weight: inherit;\n}\n\n/*\nReset links to optimize for opt-in styling instead of opt-out.\n*/\n\na {\n  color: inherit;\n  text-decoration: inherit;\n}\n\n/*\nAdd the correct font weight in Edge and Safari.\n*/\n\nb,\nstrong {\n  font-weight: bolder;\n}\n\n/*\n1. Use the user\'s configured `mono` font family by default.\n2. Correct the odd `em` font sizing in all browsers.\n*/\n\ncode,\nkbd,\nsamp,\npre {\n  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace; /* 1 */\n  font-size: 1em; /* 2 */\n}\n\n/*\nAdd the correct font size in all browsers.\n*/\n\nsmall {\n  font-size: 80%;\n}\n\n/*\nPrevent `sub` and `sup` elements from affecting the line height in all browsers.\n*/\n\nsub,\nsup {\n  font-size: 75%;\n  line-height: 0;\n  position: relative;\n  vertical-align: baseline;\n}\n\nsub {\n  bottom: -0.25em;\n}\n\nsup {\n  top: -0.5em;\n}\n\n/*\n1. Remove text indentation from table contents in Chrome and Safari. (https://bugs.chromium.org/p/chromium/issues/detail?id=999088, https://bugs.webkit.org/show_bug.cgi?id=201297)\n2. Correct table border color inheritance in all Chrome and Safari. (https://bugs.chromium.org/p/chromium/issues/detail?id=935729, https://bugs.webkit.org/show_bug.cgi?id=195016)\n3. Remove gaps between table borders by default.\n*/\n\ntable {\n  text-indent: 0; /* 1 */\n  border-color: inherit; /* 2 */\n  border-collapse: collapse; /* 3 */\n}\n\n/*\n1. Change the font styles in all browsers.\n2. Remove the margin in Firefox and Safari.\n3. Remove default padding in all browsers.\n*/\n\nbutton,\ninput,\noptgroup,\nselect,\ntextarea {\n  font-family: inherit; /* 1 */\n  font-size: 100%; /* 1 */\n  font-weight: inherit; /* 1 */\n  line-height: inherit; /* 1 */\n  color: inherit; /* 1 */\n  margin: 0; /* 2 */\n  padding: 0; /* 3 */\n}\n\n/*\nRemove the inheritance of text transform in Edge and Firefox.\n*/\n\nbutton,\nselect {\n  text-transform: none;\n}\n\n/*\n1. Correct the inability to style clickable types in iOS and Safari.\n2. Remove default button styles.\n*/\n\nbutton,\n[type=\'button\'],\n[type=\'reset\'],\n[type=\'submit\'] {\n  -webkit-appearance: button; /* 1 */\n  background-color: transparent; /* 2 */\n  background-image: none; /* 2 */\n}\n\n/*\nUse the modern Firefox focus style for all focusable elements.\n*/\n\n:-moz-focusring {\n  outline: auto;\n}\n\n/*\nRemove the additional `:invalid` styles in Firefox. (https://github.com/mozilla/gecko-dev/blob/2f9eacd9d3d995c937b4251a5557d95d494c9be1/layout/style/res/forms.css#L728-L737)\n*/\n\n:-moz-ui-invalid {\n  box-shadow: none;\n}\n\n/*\nAdd the correct vertical alignment in Chrome and Firefox.\n*/\n\nprogress {\n  vertical-align: baseline;\n}\n\n/*\nCorrect the cursor style of increment and decrement buttons in Safari.\n*/\n\n::-webkit-inner-spin-button,\n::-webkit-outer-spin-button {\n  height: auto;\n}\n\n/*\n1. Correct the odd appearance in Chrome and Safari.\n2. Correct the outline style in Safari.\n*/\n\n[type=\'search\'] {\n  -webkit-appearance: textfield; /* 1 */\n  outline-offset: -2px; /* 2 */\n}\n\n/*\nRemove the inner padding in Chrome and Safari on macOS.\n*/\n\n::-webkit-search-decoration {\n  -webkit-appearance: none;\n}\n\n/*\n1. Correct the inability to style clickable types in iOS and Safari.\n2. Change font properties to `inherit` in Safari.\n*/\n\n::-webkit-file-upload-button {\n  -webkit-appearance: button; /* 1 */\n  font: inherit; /* 2 */\n}\n\n/*\nAdd the correct display in Chrome and Safari.\n*/\n\nsummary {\n  display: list-item;\n}\n\n/*\nRemoves the default spacing and border for appropriate elements.\n*/\n\nblockquote,\ndl,\ndd,\nh1,\nh2,\nh3,\nh4,\nh5,\nh6,\nhr,\nfigure,\np,\npre {\n  margin: 0;\n}\n\nfieldset {\n  margin: 0;\n  padding: 0;\n}\n\nlegend {\n  padding: 0;\n}\n\nol,\nul,\nmenu {\n  list-style: none;\n  margin: 0;\n  padding: 0;\n}\n\n/*\nPrevent resizing textareas horizontally by default.\n*/\n\ntextarea {\n  resize: vertical;\n}\n\n/*\n1. Reset the default placeholder opacity in Firefox. (https://github.com/tailwindlabs/tailwindcss/issues/3300)\n2. Set the default placeholder color to the user\'s configured gray 400 color.\n*/\n\ninput::-moz-placeholder, textarea::-moz-placeholder {\n  opacity: 1; /* 1 */\n  color: #9ca3af; /* 2 */\n}\n\ninput::placeholder,\ntextarea::placeholder {\n  opacity: 1; /* 1 */\n  color: #9ca3af; /* 2 */\n}\n\n/*\nSet the default cursor for buttons.\n*/\n\nbutton,\n[role="button"] {\n  cursor: pointer;\n}\n\n/*\nMake sure disabled buttons don\'t get the pointer cursor.\n*/\n:disabled {\n  cursor: default;\n}\n\n/*\n1. Make replaced elements `display: block` by default. (https://github.com/mozdevs/cssremedy/issues/14)\n2. Add `vertical-align: middle` to align replaced elements more sensibly by default. (https://github.com/jensimmons/cssremedy/issues/14#issuecomment-634934210)\n   This can trigger a poorly considered lint error in some tools but is included by design.\n*/\n\nimg,\nsvg,\nvideo,\ncanvas,\naudio,\niframe,\nembed,\nobject {\n  display: block; /* 1 */\n  vertical-align: middle; /* 2 */\n}\n\n/*\nConstrain images and videos to the parent width and preserve their intrinsic aspect ratio. (https://github.com/mozdevs/cssremedy/issues/14)\n*/\n\nimg,\nvideo {\n  max-width: 100%;\n  height: auto;\n}\n\n/* Make elements with the HTML hidden attribute stay hidden by default */\n[hidden] {\n  display: none;\n}\n\n*, ::before, ::after {\n  --tw-border-spacing-x: 0;\n  --tw-border-spacing-y: 0;\n  --tw-translate-x: 0;\n  --tw-translate-y: 0;\n  --tw-rotate: 0;\n  --tw-skew-x: 0;\n  --tw-skew-y: 0;\n  --tw-scale-x: 1;\n  --tw-scale-y: 1;\n  --tw-pan-x:  ;\n  --tw-pan-y:  ;\n  --tw-pinch-zoom:  ;\n  --tw-scroll-snap-strictness: proximity;\n  --tw-ordinal:  ;\n  --tw-slashed-zero:  ;\n  --tw-numeric-figure:  ;\n  --tw-numeric-spacing:  ;\n  --tw-numeric-fraction:  ;\n  --tw-ring-inset:  ;\n  --tw-ring-offset-width: 0px;\n  --tw-ring-offset-color: #fff;\n  --tw-ring-color: rgba(59, 130, 246, 0.5);\n  --tw-ring-offset-shadow: 0 0 rgba(0,0,0,0);\n  --tw-ring-shadow: 0 0 rgba(0,0,0,0);\n  --tw-shadow: 0 0 rgba(0,0,0,0);\n  --tw-shadow-colored: 0 0 rgba(0,0,0,0);\n  --tw-blur:  ;\n  --tw-brightness:  ;\n  --tw-contrast:  ;\n  --tw-grayscale:  ;\n  --tw-hue-rotate:  ;\n  --tw-invert:  ;\n  --tw-saturate:  ;\n  --tw-sepia:  ;\n  --tw-drop-shadow:  ;\n  --tw-backdrop-blur:  ;\n  --tw-backdrop-brightness:  ;\n  --tw-backdrop-contrast:  ;\n  --tw-backdrop-grayscale:  ;\n  --tw-backdrop-hue-rotate:  ;\n  --tw-backdrop-invert:  ;\n  --tw-backdrop-opacity:  ;\n  --tw-backdrop-saturate:  ;\n  --tw-backdrop-sepia:  ;\n}\n\n::backdrop {\n  --tw-border-spacing-x: 0;\n  --tw-border-spacing-y: 0;\n  --tw-translate-x: 0;\n  --tw-translate-y: 0;\n  --tw-rotate: 0;\n  --tw-skew-x: 0;\n  --tw-skew-y: 0;\n  --tw-scale-x: 1;\n  --tw-scale-y: 1;\n  --tw-pan-x:  ;\n  --tw-pan-y:  ;\n  --tw-pinch-zoom:  ;\n  --tw-scroll-snap-strictness: proximity;\n  --tw-ordinal:  ;\n  --tw-slashed-zero:  ;\n  --tw-numeric-figure:  ;\n  --tw-numeric-spacing:  ;\n  --tw-numeric-fraction:  ;\n  --tw-ring-inset:  ;\n  --tw-ring-offset-width: 0px;\n  --tw-ring-offset-color: #fff;\n  --tw-ring-color: rgba(59, 130, 246, 0.5);\n  --tw-ring-offset-shadow: 0 0 rgba(0,0,0,0);\n  --tw-ring-shadow: 0 0 rgba(0,0,0,0);\n  --tw-shadow: 0 0 rgba(0,0,0,0);\n  --tw-shadow-colored: 0 0 rgba(0,0,0,0);\n  --tw-blur:  ;\n  --tw-brightness:  ;\n  --tw-contrast:  ;\n  --tw-grayscale:  ;\n  --tw-hue-rotate:  ;\n  --tw-invert:  ;\n  --tw-saturate:  ;\n  --tw-sepia:  ;\n  --tw-drop-shadow:  ;\n  --tw-backdrop-blur:  ;\n  --tw-backdrop-brightness:  ;\n  --tw-backdrop-contrast:  ;\n  --tw-backdrop-grayscale:  ;\n  --tw-backdrop-hue-rotate:  ;\n  --tw-backdrop-invert:  ;\n  --tw-backdrop-opacity:  ;\n  --tw-backdrop-saturate:  ;\n  --tw-backdrop-sepia:  ;\n}\n.jp-lmk-code {\n    font-size: var(--jp-code-font-size);\n    font-family: var(--jp-cell-prompt-font-family);\n  }\n.lmk-absolute {\n  position: absolute;\n}\n.lmk-right-0 {\n  right: 0px;\n}\n.lmk-z-10 {\n  z-index: 10;\n}\n.lmk-col-span-2 {\n  grid-column: span 2 / span 2;\n}\n.lmk-col-start-3 {\n  grid-column-start: 3;\n}\n.lmk-col-start-5 {\n  grid-column-start: 5;\n}\n.lmk-m-0 {\n  margin: 0px;\n}\n.lmk-m-2 {\n  margin: 0.5rem;\n}\n.lmk-mt-2 {\n  margin-top: 0.5rem;\n}\n.lmk-box-border {\n  box-sizing: border-box;\n}\n.lmk-flex {\n  display: flex;\n}\n.lmk-grid {\n  display: grid;\n}\n.lmk-hidden {\n  display: none;\n}\n.lmk-h-5 {\n  height: 1.25rem;\n}\n.lmk-h-\\[24px\\] {\n  height: 24px;\n}\n.lmk-h-full {\n  height: 100%;\n}\n.lmk-min-h-\\[100px\\] {\n  min-height: 100px;\n}\n.lmk-w-5 {\n  width: 1.25rem;\n}\n.lmk-w-6 {\n  width: 1.5rem;\n}\n.lmk-w-full {\n  width: 100%;\n}\n.lmk-grow {\n  flex-grow: 1;\n}\n.lmk-origin-top-right {\n  transform-origin: top right;\n}\n.lmk-cursor-pointer {\n  cursor: pointer;\n}\n.lmk-cursor-progress {\n  cursor: progress;\n}\n.lmk-grid-cols-1 {\n  grid-template-columns: repeat(1, minmax(0, 1fr));\n}\n.lmk-grid-cols-\\[max-content_1fr\\] {\n  grid-template-columns: max-content 1fr;\n}\n.lmk-grid-cols-\\[max-content_1fr_auto_1fr_max-content\\] {\n  grid-template-columns: max-content 1fr auto 1fr max-content;\n}\n.lmk-flex-row {\n  flex-direction: row;\n}\n.lmk-flex-col {\n  flex-direction: column;\n}\n.lmk-content-center {\n  align-content: center;\n}\n.lmk-items-center {\n  align-items: center;\n}\n.lmk-items-stretch {\n  align-items: stretch;\n}\n.lmk-gap-1 {\n  gap: 0.25rem;\n}\n.lmk-gap-2 {\n  gap: 0.5rem;\n}\n.lmk-gap-3 {\n  gap: 0.75rem;\n}\n.lmk-gap-4 {\n  gap: 1rem;\n}\n.lmk-rounded-md {\n  border-radius: 0.375rem;\n}\n.lmk-rounded-xl {\n  border-radius: 0.75rem;\n}\n.lmk-border {\n  border-width: 1px;\n}\n.lmk-border-solid {\n  border-style: solid;\n}\n.lmk-border-editorBorder {\n  border-color: var(--jp-cell-editor-border-color);\n}\n.lmk-bg-cellBg {\n  background-color: var(--jp-layout-color1);\n}\n.lmk-bg-transparent {\n  background-color: transparent;\n}\n.lmk-p-4 {\n  padding: 1rem;\n}\n.lmk-px-0 {\n  padding-left: 0px;\n  padding-right: 0px;\n}\n.lmk-px-4 {\n  padding-left: 1rem;\n  padding-right: 1rem;\n}\n.lmk-py-1 {\n  padding-top: 0.25rem;\n  padding-bottom: 0.25rem;\n}\n.lmk-py-2 {\n  padding-top: 0.5rem;\n  padding-bottom: 0.5rem;\n}\n.lmk-pt-2 {\n  padding-top: 0.5rem;\n}\n.lmk-font-jupyter {\n  font-family: var(--jp-ui-font-family);\n}\n.lmk-text-lg {\n  font-size: 1.125rem;\n  line-height: 1.75rem;\n}\n.lmk-text-sm {\n  font-size: 0.875rem;\n  line-height: 1.25rem;\n}\n.lmk-font-bold {\n  font-weight: 700;\n}\n.lmk-text-error {\n  color: var(--jp-error-color0);\n}\n.lmk-text-font {\n  color: var(--jp-ui-font-color0);\n}\n.lmk-text-success {\n  color: var(--jp-success-color0);\n}\n.lmk-text-warn {\n  color: var(--jp-warn-color0);\n}\n.lmk-shadow-lg {\n  --tw-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.1);\n  --tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);\n  box-shadow: 0 0 rgba(0,0,0,0), 0 0 rgba(0,0,0,0), 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.1);\n  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);\n}\n.lmk-ring-1 {\n  --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);\n  --tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);\n  box-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color), var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color), 0 0 rgba(0,0,0,0);\n  box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow), var(--tw-shadow, 0 0 #0000);\n}\n.lmk-ring-bgLight {\n  --tw-ring-color: var(--jp-layout-color2);\n}\n.lmk-ring-opacity-5 {\n  --tw-ring-opacity: 0.05;\n}\n.hover\\:lmk-bg-bgLight:hover {\n  background-color: var(--jp-layout-color2);\n}\n@media (min-width: 1024px) {\n\n  .lg\\:lmk-mr-1 {\n    margin-right: 0.25rem;\n  }\n\n  .lg\\:lmk-flex {\n    display: flex;\n  }\n\n  .lg\\:lmk-hidden {\n    display: none;\n  }\n\n  .lg\\:lmk-w-56 {\n    width: 14rem;\n  }\n\n  .lg\\:lmk-grid-cols-2 {\n    grid-template-columns: repeat(2, minmax(0, 1fr));\n  }\n\n  .lg\\:lmk-grid-rows-1 {\n    grid-template-rows: repeat(1, minmax(0, 1fr));\n  }\n}\n.\\[\\&\\>a\\]\\:lmk-text-link>a {\n  color: var(--jp-mirror-editor-variable-2-color);\n}\n.\\[\\&\\>a\\]\\:lmk-no-underline>a {\n  text-decoration-line: none;\n}\n.\\[\\&h3\\]\\:lmk-m-0h3 {\n  margin: 0px;\n}\n', ""]), c.exports = e
@@ -19281,15 +19281,15 @@
                         },
                         8459: c => {
                             "use strict";
                             c.exports = a(829)
                         },
                         4147: c => {
                             "use strict";
-                            c.exports = JSON.parse('{"name":"lmk-jupyter","version":"0.0.5","description":"Jupyter Widget for using LMK in a jupyter notebook","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.{d.ts,js}","dist/*.js","styles/*.css"],"homepage":"https://app.lmkapp.dev","bugs":{"url":"https://github.com/cfeenstra67/lmk-python/issues"},"license":"MIT","author":{"name":"Cam Feenstra","email":"me@camfeenstra.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cfeenstra67/lmk-python/blob/main/npm.README.md"},"scripts":{"build":"pnpm build:lib && pnpm build:nbextension && pnpm build:labextension:dev","build:prod":"pnpm run build:lib && NODE_ENV=production pnpm build:nbextension && NODE_ENV=production pnpm build:labextension","build:python":"pnpm clean && pnpm generate && venv/bin/python -m build .","build:publish":"pnpm clean && pnpm build:prod","build:labextension":"jupyter labextension build . && cd lmk/jupyter/labextension","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc -p tsconfig.build.json","build:nbextension":"webpack","clean":"pnpm clean:dist && pnpm run clean:lib && pnpm run clean:nbextension && pnpm run clean:labextension && pnpm run clean:generated && pnpm run clean:python","clean:dist":"rimraf dist","clean:lib":"rimraf lib","clean:labextension":"rimraf lmk/jupyter/labextension","clean:nbextension":"rimraf lmk/jupyter/nbextension","clean:generated":"rimraf lmk/generated","clean:python":"rm -rf lmk/**/__pycache__ lmk/**/*.pyc","format":"prettier --write \\"src/**/*.ts\\" && venv/bin/black lmk","generate":"openapi-generator-cli generate > /dev/null","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"pnpm run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w -p tsconfig.build.json","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","install-all":"pnpm install && venv/bin/pip install -e \'.[dev,publish,jupyter]\'","prepublishOnly":"pnpm readme:npm","postpack":"pnpm readme:git","readme:npm":"mv README.md git.README.md && mv npm.README.md README.md","readme:git":"mv README.md npm.README.md && mv git.README.md README.md","pypi-check":"twine check dist/lmk_*","pypi-upload-test":"twine upload --repository-url https://test.pypi.org/legacy/ dist/lmk_*","pypi-upload":"twine upload dist/lmk_*"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","classnames":"^2.3.2","uuid":"^9.0.0","yjs":"^13.5.17"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@fortawesome/fontawesome-svg-core":"^6.3.0","@fortawesome/free-solid-svg-icons":"^6.3.0","@fortawesome/react-fontawesome":"^0.2.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@jupyterlab/services":"^6.6.1","@jupyterlab/ui-components":"^3.6.1","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@openapitools/openapi-generator-cli":"^2.5.2","@swc/core":"^1.3.24","@types/backbone":"^1.4.15","@types/ms":"^0.7.31","@types/node":"^16.18.23","@types/react":"^17.0.2","@types/react-dom":"^17.0.2","@types/uuid":"^9.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","backbone":"^1.4.1","crypto":"1.0.1","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","esm":"^3.2.25","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","ms":"^2.1.3","npm-run-all":"^4.1.3","postcss":"^8.4.21","postcss-loader":"^7.2.4","postcss-preset-env":"^8.3.0","prettier":"^2.0.5","react":"^17.0.2","react-dom":"^17.0.2","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","tailwindcss":"^3.2.7","ts-loader":"^8.0.0","ts-node":"^10.9.1","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"dist/plugin","outputDir":"lmk/jupyter/labextension/lmk-jupyter","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/ui-components":{"bundled":false,"singleton":true}}}}')
+                            c.exports = JSON.parse('{"name":"lmk-jupyter","version":"0.0.7","description":"Jupyter Widget for using LMK in a jupyter notebook","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.{d.ts,js}","dist/*.js","styles/*.css"],"homepage":"https://app.lmkapp.dev","bugs":{"url":"https://github.com/cfeenstra67/lmk-python/issues"},"license":"MIT","author":{"name":"Cam Feenstra","email":"me@camfeenstra.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cfeenstra67/lmk-python/blob/main/npm.README.md"},"scripts":{"build":"pnpm build:lib && pnpm build:nbextension && pnpm build:labextension:dev","build:prod":"pnpm run build:lib && NODE_ENV=production pnpm build:nbextension && NODE_ENV=production pnpm build:labextension","build:python":"pnpm clean && pnpm generate && venv/bin/python -m build .","build:publish":"pnpm clean && pnpm build:prod","build:labextension":"jupyter labextension build . && cd lmk/jupyter/labextension","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc -p tsconfig.build.json","build:nbextension":"webpack","clean":"pnpm clean:dist && pnpm run clean:lib && pnpm run clean:nbextension && pnpm run clean:labextension && pnpm run clean:generated && pnpm run clean:python","clean:dist":"rimraf dist","clean:lib":"rimraf lib","clean:labextension":"rimraf lmk/jupyter/labextension","clean:nbextension":"rimraf lmk/jupyter/nbextension","clean:generated":"rimraf lmk/generated","clean:python":"rm -rf lmk/**/__pycache__ lmk/**/*.pyc","format":"prettier --write \\"src/**/*.ts\\" && venv/bin/black lmk","generate":"openapi-generator-cli generate > /dev/null","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"pnpm run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w -p tsconfig.build.json","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","install-all":"pnpm install && venv/bin/pip install -e \'.[dev,publish,jupyter]\'","prepublishOnly":"pnpm readme:npm","postpack":"pnpm readme:git","readme:npm":"mv README.md git.README.md && mv npm.README.md README.md","readme:git":"mv README.md npm.README.md && mv git.README.md README.md","pypi-check":"twine check dist/lmk_*","pypi-upload-test":"twine upload --repository-url https://test.pypi.org/legacy/ dist/lmk_*","pypi-upload":"twine upload dist/lmk_*"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","classnames":"^2.3.2","uuid":"^9.0.0","yjs":"^13.5.17"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@fortawesome/fontawesome-svg-core":"^6.3.0","@fortawesome/free-solid-svg-icons":"^6.3.0","@fortawesome/react-fontawesome":"^0.2.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@jupyterlab/services":"^6.6.1","@jupyterlab/ui-components":"^3.6.1","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@openapitools/openapi-generator-cli":"^2.5.2","@swc/core":"^1.3.24","@types/backbone":"^1.4.15","@types/ms":"^0.7.31","@types/node":"^16.18.23","@types/react":"^17.0.2","@types/react-dom":"^17.0.2","@types/uuid":"^9.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","backbone":"^1.4.1","crypto":"1.0.1","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","esm":"^3.2.25","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","ms":"^2.1.3","npm-run-all":"^4.1.3","postcss":"^8.4.21","postcss-loader":"^7.2.4","postcss-preset-env":"^8.3.0","prettier":"^2.0.5","react":"^17.0.2","react-dom":"^17.0.2","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","tailwindcss":"^3.2.7","ts-loader":"^8.0.0","ts-node":"^10.9.1","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"dist/plugin","outputDir":"lmk/jupyter/labextension/lmk-jupyter","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/ui-components":{"bundled":false,"singleton":true}}}}')
                         }
                     },
                     n = {};
 
                 function r(c) {
                     var a = n[c];
                     if (void 0 !== a) return a.exports;
```

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/399.49345c52b42d87d9afb9.js.LICENSE.txt` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/399.c2165748a9b3b2c7908d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/568.20579847b1912c2a38d6.js` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/568.12d21aceee689bf3ed6f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -784,11 +784,11 @@
             i(s, {
                 insert: "head",
                 singleton: !1
             }), e.exports = s.locals || {}
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"lmk-jupyter","version":"0.0.5","description":"Jupyter Widget for using LMK in a jupyter notebook","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.{d.ts,js}","dist/*.js","styles/*.css"],"homepage":"https://app.lmkapp.dev","bugs":{"url":"https://github.com/cfeenstra67/lmk-python/issues"},"license":"MIT","author":{"name":"Cam Feenstra","email":"me@camfeenstra.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cfeenstra67/lmk-python/blob/main/npm.README.md"},"scripts":{"build":"pnpm build:lib && pnpm build:nbextension && pnpm build:labextension:dev","build:prod":"pnpm run build:lib && NODE_ENV=production pnpm build:nbextension && NODE_ENV=production pnpm build:labextension","build:python":"pnpm clean && pnpm generate && venv/bin/python -m build .","build:publish":"pnpm clean && pnpm build:prod","build:labextension":"jupyter labextension build . && cd lmk/jupyter/labextension","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc -p tsconfig.build.json","build:nbextension":"webpack","clean":"pnpm clean:dist && pnpm run clean:lib && pnpm run clean:nbextension && pnpm run clean:labextension && pnpm run clean:generated && pnpm run clean:python","clean:dist":"rimraf dist","clean:lib":"rimraf lib","clean:labextension":"rimraf lmk/jupyter/labextension","clean:nbextension":"rimraf lmk/jupyter/nbextension","clean:generated":"rimraf lmk/generated","clean:python":"rm -rf lmk/**/__pycache__ lmk/**/*.pyc","format":"prettier --write \\"src/**/*.ts\\" && venv/bin/black lmk","generate":"openapi-generator-cli generate > /dev/null","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"pnpm run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w -p tsconfig.build.json","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","install-all":"pnpm install && venv/bin/pip install -e \'.[dev,publish,jupyter]\'","prepublishOnly":"pnpm readme:npm","postpack":"pnpm readme:git","readme:npm":"mv README.md git.README.md && mv npm.README.md README.md","readme:git":"mv README.md npm.README.md && mv git.README.md README.md","pypi-check":"twine check dist/lmk_*","pypi-upload-test":"twine upload --repository-url https://test.pypi.org/legacy/ dist/lmk_*","pypi-upload":"twine upload dist/lmk_*"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","classnames":"^2.3.2","uuid":"^9.0.0","yjs":"^13.5.17"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@fortawesome/fontawesome-svg-core":"^6.3.0","@fortawesome/free-solid-svg-icons":"^6.3.0","@fortawesome/react-fontawesome":"^0.2.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@jupyterlab/services":"^6.6.1","@jupyterlab/ui-components":"^3.6.1","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@openapitools/openapi-generator-cli":"^2.5.2","@swc/core":"^1.3.24","@types/backbone":"^1.4.15","@types/ms":"^0.7.31","@types/node":"^16.18.23","@types/react":"^17.0.2","@types/react-dom":"^17.0.2","@types/uuid":"^9.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","backbone":"^1.4.1","crypto":"1.0.1","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","esm":"^3.2.25","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","ms":"^2.1.3","npm-run-all":"^4.1.3","postcss":"^8.4.21","postcss-loader":"^7.2.4","postcss-preset-env":"^8.3.0","prettier":"^2.0.5","react":"^17.0.2","react-dom":"^17.0.2","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","tailwindcss":"^3.2.7","ts-loader":"^8.0.0","ts-node":"^10.9.1","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"dist/plugin","outputDir":"lmk/jupyter/labextension/lmk-jupyter","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/ui-components":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"lmk-jupyter","version":"0.0.7","description":"Jupyter Widget for using LMK in a jupyter notebook","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.{d.ts,js}","dist/*.js","styles/*.css"],"homepage":"https://app.lmkapp.dev","bugs":{"url":"https://github.com/cfeenstra67/lmk-python/issues"},"license":"MIT","author":{"name":"Cam Feenstra","email":"me@camfeenstra.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cfeenstra67/lmk-python/blob/main/npm.README.md"},"scripts":{"build":"pnpm build:lib && pnpm build:nbextension && pnpm build:labextension:dev","build:prod":"pnpm run build:lib && NODE_ENV=production pnpm build:nbextension && NODE_ENV=production pnpm build:labextension","build:python":"pnpm clean && pnpm generate && venv/bin/python -m build .","build:publish":"pnpm clean && pnpm build:prod","build:labextension":"jupyter labextension build . && cd lmk/jupyter/labextension","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc -p tsconfig.build.json","build:nbextension":"webpack","clean":"pnpm clean:dist && pnpm run clean:lib && pnpm run clean:nbextension && pnpm run clean:labextension && pnpm run clean:generated && pnpm run clean:python","clean:dist":"rimraf dist","clean:lib":"rimraf lib","clean:labextension":"rimraf lmk/jupyter/labextension","clean:nbextension":"rimraf lmk/jupyter/nbextension","clean:generated":"rimraf lmk/generated","clean:python":"rm -rf lmk/**/__pycache__ lmk/**/*.pyc","format":"prettier --write \\"src/**/*.ts\\" && venv/bin/black lmk","generate":"openapi-generator-cli generate > /dev/null","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"pnpm run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w -p tsconfig.build.json","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","install-all":"pnpm install && venv/bin/pip install -e \'.[dev,publish,jupyter]\'","prepublishOnly":"pnpm readme:npm","postpack":"pnpm readme:git","readme:npm":"mv README.md git.README.md && mv npm.README.md README.md","readme:git":"mv README.md npm.README.md && mv git.README.md README.md","pypi-check":"twine check dist/lmk_*","pypi-upload-test":"twine upload --repository-url https://test.pypi.org/legacy/ dist/lmk_*","pypi-upload":"twine upload dist/lmk_*"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","classnames":"^2.3.2","uuid":"^9.0.0","yjs":"^13.5.17"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@fortawesome/fontawesome-svg-core":"^6.3.0","@fortawesome/free-solid-svg-icons":"^6.3.0","@fortawesome/react-fontawesome":"^0.2.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@jupyterlab/services":"^6.6.1","@jupyterlab/ui-components":"^3.6.1","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@openapitools/openapi-generator-cli":"^2.5.2","@swc/core":"^1.3.24","@types/backbone":"^1.4.15","@types/ms":"^0.7.31","@types/node":"^16.18.23","@types/react":"^17.0.2","@types/react-dom":"^17.0.2","@types/uuid":"^9.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","backbone":"^1.4.1","crypto":"1.0.1","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","esm":"^3.2.25","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","ms":"^2.1.3","npm-run-all":"^4.1.3","postcss":"^8.4.21","postcss-loader":"^7.2.4","postcss-preset-env":"^8.3.0","prettier":"^2.0.5","react":"^17.0.2","react-dom":"^17.0.2","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","tailwindcss":"^3.2.7","ts-loader":"^8.0.0","ts-node":"^10.9.1","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"dist/plugin","outputDir":"lmk/jupyter/labextension/lmk-jupyter","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/ui-components":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/582.2007fa97241e6df13205.js` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/582.2007fa97241e6df13205.js`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/875.e1becc2c9f68a75184b9.js` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/875.e1becc2c9f68a75184b9.js`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js.LICENSE.txt` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/896.86af48f08490491b90eb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/remoteEntry.433f22a9050fe1c09832.js` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/remoteEntry.b02170963b4d89253004.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, f, l, s, d, c, p, h, v, b, m, g = {
+    var e, r, t, n, a, o, i, u, l, f, d, s, c, p, h, v, m, b, g = {
             888: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(896), t.e(829), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(829), t.e(399)]).then((() => () => t(399)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -42,23 +42,23 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        399: "49345c52b42d87d9afb9",
-        568: "20579847b1912c2a38d6",
+        399: "c2165748a9b3b2c7908d",
+        568: "12d21aceee689bf3ed6f",
         582: "2007fa97241e6df13205",
         829: "a875f185f4186af57d00",
         875: "e1becc2c9f68a75184b9",
         896: "86af48f08490491b90eb"
     } [e] + ".js?v=" + {
-        399: "49345c52b42d87d9afb9",
-        568: "20579847b1912c2a38d6",
+        399: "c2165748a9b3b2c7908d",
+        568: "12d21aceee689bf3ed6f",
         582: "2007fa97241e6df13205",
         829: "a875f185f4186af57d00",
         875: "e1becc2c9f68a75184b9",
         896: "86af48f08490491b90eb"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
@@ -67,32 +67,32 @@
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "lmk-jupyter:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
-                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
-                    var s = f[l];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var d = l[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
+            var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -113,16 +113,16 @@
                             u = a[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    f = [];
-                return "default" === t && (u("classnames", "2.3.2", (() => w.e(875).then((() => () => w(875))))), u("lmk-jupyter", "0.0.5", (() => Promise.all([w.e(896), w.e(829), w.e(568)]).then((() => () => w(568))))), u("uuid", "9.0.0", (() => w.e(582).then((() => () => w(582)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (u("classnames", "2.3.2", (() => w.e(875).then((() => () => w(875))))), u("lmk-jupyter", "0.0.7", (() => Promise.all([w.e(896), w.e(829), w.e(568)]).then((() => () => w(568))))), u("uuid", "9.0.0", (() => w.e(582).then((() => () => w(582)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -157,47 +157,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var u = e[o];
-            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
         }
-        return f();
+        return l();
 
-        function f() {
+        function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
-            for (var i = 0, u = 1, f = !0;; u++, i++) {
-                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !a : "" == d != a);
-                if ("u" == s) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
-                    if (d == s)
+            for (var i = 0, u = 1, l = !0;; u++, i++) {
+                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !a : "" == s != a);
+                if ("u" == d) {
+                    if (!l || "u" != s) return !1
+                } else if (l)
+                    if (s == d)
                         if (u <= n) {
-                            if (l != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (a ? l > e[u] : l < e[u]) return !1;
-                            l != e[u] && (f = !1)
+                            if (a ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != s && "n" != s) {
                     if (a || u <= n) return !1;
-                    f = !1, u--
+                    l = !1, u--
                 } else {
-                    if (u <= n || s < d != a) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, u--)
+                    if (u <= n || d < s != a) return !1;
+                    l = !1
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -206,56 +206,56 @@
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", l = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(f(e, t, a, n)), d(e[t][a])
-    }, s = (e, r, t) => {
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), s(e[t][a])
+    }, d = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, d = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
+    }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
-        var o = r && w.o(r, t) && s(r, t, n);
-        return o ? d(o) : a()
-    })), v = {}, b = {
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
+        var o = r && w.o(r, t) && d(r, t, n);
+        return o ? s(o) : a()
+    })), v = {}, m = {
         829: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ]),
         118: () => h("default", "classnames", [1, 2, 3, 2], (() => w.e(875).then((() => () => w(875))))),
         271: () => p("default", "react", [1, 17, 0, 1]),
         456: () => p("default", "react-dom", [1, 17, 0, 1]),
         698: () => h("default", "uuid", [1, 9, 0, 0], (() => w.e(582).then((() => () => w(582)))))
-    }, m = {
+    }, b = {
         568: [118, 271, 456, 698],
         829: [829]
     }, w.f.consumes = (e, r) => {
-        w.o(m, e) && m[e].forEach((e => {
+        w.o(b, e) && b[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var a = b[e]();
+                var a = m[e]();
                 a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
@@ -277,20 +277,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var n, a, [o, i, u] = t,
-                    f = 0;
+                    l = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (n in i) w.o(i, n) && (w.m[n] = i[n]);
                     u && u(w)
                 }
-                for (r && r(t); f < o.length; f++) a = o[f], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < o.length; l++) a = o[l], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunklmk_jupyter = self.webpackChunklmk_jupyter || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), w.nc = void 0;
     var k = w(888);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["lmk-jupyter"] = k
 })();
```

### Comparing `lmk_python-0.0.5/lmk/jupyter/labextension/lmk-jupyter/static/third-party-licenses.json` & `lmk_python-0.0.7/lmk/jupyter/labextension/lmk-jupyter/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/lmk/jupyter/nbextension/lmk-jupyter.js` & `lmk_python-0.0.7/lmk/jupyter/nbextension/lmk-jupyter.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25764,15 +25764,15 @@
 
             /***/
             4147:
                 /***/
                 ((module) => {
 
                     "use strict";
-                    module.exports = JSON.parse('{"name":"lmk-jupyter","version":"0.0.5","description":"Jupyter Widget for using LMK in a jupyter notebook","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.{d.ts,js}","dist/*.js","styles/*.css"],"homepage":"https://app.lmkapp.dev","bugs":{"url":"https://github.com/cfeenstra67/lmk-python/issues"},"license":"MIT","author":{"name":"Cam Feenstra","email":"me@camfeenstra.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cfeenstra67/lmk-python/blob/main/npm.README.md"},"scripts":{"build":"pnpm build:lib && pnpm build:nbextension && pnpm build:labextension:dev","build:prod":"pnpm run build:lib && NODE_ENV=production pnpm build:nbextension && NODE_ENV=production pnpm build:labextension","build:python":"pnpm clean && pnpm generate && venv/bin/python -m build .","build:publish":"pnpm clean && pnpm build:prod","build:labextension":"jupyter labextension build . && cd lmk/jupyter/labextension","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc -p tsconfig.build.json","build:nbextension":"webpack","clean":"pnpm clean:dist && pnpm run clean:lib && pnpm run clean:nbextension && pnpm run clean:labextension && pnpm run clean:generated && pnpm run clean:python","clean:dist":"rimraf dist","clean:lib":"rimraf lib","clean:labextension":"rimraf lmk/jupyter/labextension","clean:nbextension":"rimraf lmk/jupyter/nbextension","clean:generated":"rimraf lmk/generated","clean:python":"rm -rf lmk/**/__pycache__ lmk/**/*.pyc","format":"prettier --write \\"src/**/*.ts\\" && venv/bin/black lmk","generate":"openapi-generator-cli generate > /dev/null","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"pnpm run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w -p tsconfig.build.json","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","install-all":"pnpm install && venv/bin/pip install -e \'.[dev,publish,jupyter]\'","prepublishOnly":"pnpm readme:npm","postpack":"pnpm readme:git","readme:npm":"mv README.md git.README.md && mv npm.README.md README.md","readme:git":"mv README.md npm.README.md && mv git.README.md README.md","pypi-check":"twine check dist/lmk_*","pypi-upload-test":"twine upload --repository-url https://test.pypi.org/legacy/ dist/lmk_*","pypi-upload":"twine upload dist/lmk_*"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","classnames":"^2.3.2","uuid":"^9.0.0","yjs":"^13.5.17"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@fortawesome/fontawesome-svg-core":"^6.3.0","@fortawesome/free-solid-svg-icons":"^6.3.0","@fortawesome/react-fontawesome":"^0.2.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@jupyterlab/services":"^6.6.1","@jupyterlab/ui-components":"^3.6.1","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@openapitools/openapi-generator-cli":"^2.5.2","@swc/core":"^1.3.24","@types/backbone":"^1.4.15","@types/ms":"^0.7.31","@types/node":"^16.18.23","@types/react":"^17.0.2","@types/react-dom":"^17.0.2","@types/uuid":"^9.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","backbone":"^1.4.1","crypto":"1.0.1","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","esm":"^3.2.25","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","ms":"^2.1.3","npm-run-all":"^4.1.3","postcss":"^8.4.21","postcss-loader":"^7.2.4","postcss-preset-env":"^8.3.0","prettier":"^2.0.5","react":"^17.0.2","react-dom":"^17.0.2","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","tailwindcss":"^3.2.7","ts-loader":"^8.0.0","ts-node":"^10.9.1","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"dist/plugin","outputDir":"lmk/jupyter/labextension/lmk-jupyter","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/ui-components":{"bundled":false,"singleton":true}}}}');
+                    module.exports = JSON.parse('{"name":"lmk-jupyter","version":"0.0.7","description":"Jupyter Widget for using LMK in a jupyter notebook","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.{d.ts,js}","dist/*.js","styles/*.css"],"homepage":"https://app.lmkapp.dev","bugs":{"url":"https://github.com/cfeenstra67/lmk-python/issues"},"license":"MIT","author":{"name":"Cam Feenstra","email":"me@camfeenstra.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cfeenstra67/lmk-python/blob/main/npm.README.md"},"scripts":{"build":"pnpm build:lib && pnpm build:nbextension && pnpm build:labextension:dev","build:prod":"pnpm run build:lib && NODE_ENV=production pnpm build:nbextension && NODE_ENV=production pnpm build:labextension","build:python":"pnpm clean && pnpm generate && venv/bin/python -m build .","build:publish":"pnpm clean && pnpm build:prod","build:labextension":"jupyter labextension build . && cd lmk/jupyter/labextension","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc -p tsconfig.build.json","build:nbextension":"webpack","clean":"pnpm clean:dist && pnpm run clean:lib && pnpm run clean:nbextension && pnpm run clean:labextension && pnpm run clean:generated && pnpm run clean:python","clean:dist":"rimraf dist","clean:lib":"rimraf lib","clean:labextension":"rimraf lmk/jupyter/labextension","clean:nbextension":"rimraf lmk/jupyter/nbextension","clean:generated":"rimraf lmk/generated","clean:python":"rm -rf lmk/**/__pycache__ lmk/**/*.pyc","format":"prettier --write \\"src/**/*.ts\\" && venv/bin/black lmk","generate":"openapi-generator-cli generate > /dev/null","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"pnpm run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w -p tsconfig.build.json","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","install-all":"pnpm install && venv/bin/pip install -e \'.[dev,publish,jupyter]\'","prepublishOnly":"pnpm readme:npm","postpack":"pnpm readme:git","readme:npm":"mv README.md git.README.md && mv npm.README.md README.md","readme:git":"mv README.md npm.README.md && mv git.README.md README.md","pypi-check":"twine check dist/lmk_*","pypi-upload-test":"twine upload --repository-url https://test.pypi.org/legacy/ dist/lmk_*","pypi-upload":"twine upload dist/lmk_*"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","classnames":"^2.3.2","uuid":"^9.0.0","yjs":"^13.5.17"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@fortawesome/fontawesome-svg-core":"^6.3.0","@fortawesome/free-solid-svg-icons":"^6.3.0","@fortawesome/react-fontawesome":"^0.2.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@jupyterlab/services":"^6.6.1","@jupyterlab/ui-components":"^3.6.1","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@openapitools/openapi-generator-cli":"^2.5.2","@swc/core":"^1.3.24","@types/backbone":"^1.4.15","@types/ms":"^0.7.31","@types/node":"^16.18.23","@types/react":"^17.0.2","@types/react-dom":"^17.0.2","@types/uuid":"^9.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","backbone":"^1.4.1","crypto":"1.0.1","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","esm":"^3.2.25","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","ms":"^2.1.3","npm-run-all":"^4.1.3","postcss":"^8.4.21","postcss-loader":"^7.2.4","postcss-preset-env":"^8.3.0","prettier":"^2.0.5","react":"^17.0.2","react-dom":"^17.0.2","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","tailwindcss":"^3.2.7","ts-loader":"^8.0.0","ts-node":"^10.9.1","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"dist/plugin","outputDir":"lmk/jupyter/labextension/lmk-jupyter","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/ui-components":{"bundled":false,"singleton":true}}}}');
 
                     /***/
                 })
 
             /******/
         });
         /************************************************************************/
```

### Comparing `lmk_python-0.0.5/src/extension.ts` & `lmk_python-0.0.7/src/extension.ts`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/plugin.ts` & `lmk_python-0.0.7/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/version.ts` & `lmk_python-0.0.7/src/version.ts`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/components/Auth.tsx` & `lmk_python-0.0.7/src/components/Auth.tsx`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/components/Navbar.tsx` & `lmk_python-0.0.7/src/components/Navbar.tsx`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/components/Widget.tsx` & `lmk_python-0.0.7/src/components/Widget.tsx`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/components/WidgetContent.tsx` & `lmk_python-0.0.7/src/components/WidgetContent.tsx`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/hooks/click-outside.ts` & `lmk_python-0.0.7/src/hooks/click-outside.ts`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/hooks/model.ts` & `lmk_python-0.0.7/src/hooks/model.ts`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/src/lib/widget-model.ts` & `lmk_python-0.0.7/src/lib/widget-model.ts`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/styles/Loader.css` & `lmk_python-0.0.7/styles/Loader.css`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/LICENSE.txt` & `lmk_python-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/README.md` & `lmk_python-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lmk_python-0.0.5/pyproject.toml` & `lmk_python-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = ["pydantic", "blinker", "python-dateutil", "typing_extensions", "urllib3"]
-version = "0.0.5"
+version = "0.0.7"
 
 [project.optional-dependencies]
 jupyter = [
     "ipywidgets>=7.0.0",
     "ipython>=6.1.0"
 ]
 dev = ["black", "bump2version", "jupyterlab"]
@@ -49,16 +49,16 @@
 artifacts = [
     "lmk/generated",
     "lmk/jupyter/nbextension",
     "lmk/jupyter/labextension",
 ]
 
 [tool.hatch.build.targets.wheel.shared-data]
-"lmk/jupyter/nbextension/lmk-jupyter" = "share/jupyter/nbextensions/lmk-jupyter"
-"lmk/jupyter/labextension/lmk-jupyter.js" = "share/jupyter/labextensions/lmk-jupyter.js"
+"lmk/jupyter/labextension/lmk-jupyter" = "share/jupyter/labextensions/lmk-jupyter"
+"lmk/jupyter/nbextension/lmk-jupyter.js" = "share/jupyter/nbextensions/lmk-jupyter.js"
 "./install.json" = "share/jupyter/labextensions/lmk-jupyter/install.json"
 "./lmk.json" = "etc/jupyter/nbconfig/notebook.d/lmk.json"
 
 [tool.hatch.build.hooks.jupyter-builder]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
     "lmk/jupyter/nbextension/lmk-jupyter.js",
```

### Comparing `lmk_python-0.0.5/PKG-INFO` & `lmk_python-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmk-python
-Version: 0.0.5
+Version: 0.0.7
 Summary: Notifications you want, when you want them
 Project-URL: Homepage, https://github.com/cfeenstra67/lmk-python
 Author-email: Cam Feenstra <me@camfeenstra.com>
 License: Copyright 2023 Cameron Feenstra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

