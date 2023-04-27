# Comparing `tmp/ucloud-sdk-python3-0.9.3.tar.gz` & `tmp/ucloud-sdk-python3-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ucloud-sdk-python3-0.9.3.tar", last modified: Tue Sep 22 04:16:45 2020, max compression
+gzip compressed data, was "dist/ucloud-sdk-python3-0.9.4.tar", last modified: Fri Sep 25 12:31:28 2020, max compression
```

## Comparing `ucloud-sdk-python3-0.9.3.tar` & `ucloud-sdk-python3-0.9.4.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/
--rw-r--r--   0 root         (0)     1000     2183 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/PKG-INFO
--rw-r--r--   0 root         (0)     1000     1073 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/README.md
--rw-r--r--   0 root         (0)     1000       38 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/setup.cfg
--rw-r--r--   0 root         (0)     1000     3518 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/setup.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/__init__.py
--rw-r--r--   0 root         (0)     1000     3808 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/core/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/__init__.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/core/auth/
--rw-r--r--   0 root         (0)     1000       71 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/auth/__init__.py
--rw-r--r--   0 root         (0)     1000     2117 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/auth/_cfg.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/core/client/
--rw-r--r--   0 root         (0)     1000      137 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/client/__init__.py
--rw-r--r--   0 root         (0)     1000     3700 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/client/_cfg.py
--rw-r--r--   0 root         (0)     1000     5907 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/client/_client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/core/exc/
--rw-r--r--   0 root         (0)     1000      211 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/exc/__init__.py
--rw-r--r--   0 root         (0)     1000     2301 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/exc/_exc.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/core/transport/
--rw-r--r--   0 root         (0)     1000      223 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/transport/__init__.py
--rw-r--r--   0 root         (0)     1000     4489 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/transport/_requests.py
--rw-r--r--   0 root         (0)     1000     3185 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/transport/http.py
--rw-r--r--   0 root         (0)     1000     1448 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/transport/utils.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/__init__.py
--rw-r--r--   0 root         (0)     1000     1518 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/abstract.py
--rw-r--r--   0 root         (0)     1000      967 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/encoder.py
--rw-r--r--   0 root         (0)     1000     4090 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/fields.py
--rw-r--r--   0 root         (0)     1000     2665 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/schema.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/core/utils/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/utils/__init__.py
--rw-r--r--   0 root         (0)     1000      264 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/utils/compat.py
--rw-r--r--   0 root         (0)     1000      820 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/utils/deco.py
--rw-r--r--   0 root         (0)     1000      675 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/utils/log.py
--rw-r--r--   0 root         (0)     1000     2127 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/core/utils/middleware.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/helpers/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/helpers/__init__.py
--rw-r--r--   0 root         (0)     1000     2441 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/helpers/utils.py
--rw-r--r--   0 root         (0)     1000     3518 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/helpers/wait.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/__init__.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/__init__.py
--rw-r--r--   0 root         (0)     1000     5910 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000     2098 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     3914 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/pathx/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/pathx/__init__.py
--rw-r--r--   0 root         (0)     1000     7741 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/pathx/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/pathx/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/pathx/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000     5021 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/pathx/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     1270 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/pathx/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/__init__.py
--rw-r--r--   0 root         (0)     1000     4085 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000     2072 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     1271 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/__init__.py
--rw-r--r--   0 root         (0)     1000     6047 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000     2903 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     2644 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/__init__.py
--rw-r--r--   0 root         (0)     1000    35053 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    14628 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/schemas/apis.py
--rw-r--r--   0 root         (0)     1000    10892 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/__init__.py
--rw-r--r--   0 root         (0)     1000   135256 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    83272 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/schemas/apis.py
--rw-r--r--   0 root         (0)     1000    25113 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udb/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udb/__init__.py
--rw-r--r--   0 root         (0)     1000    84833 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udb/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udb/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udb/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    46085 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udb/schemas/apis.py
--rw-r--r--   0 root         (0)     1000    10173 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udb/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udisk/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udisk/__init__.py
--rw-r--r--   0 root         (0)     1000    27879 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udisk/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udisk/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udisk/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    14863 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udisk/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     4155 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udisk/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udpn/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udpn/__init__.py
--rw-r--r--   0 root         (0)     1000    10058 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udpn/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udpn/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udpn/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000     5265 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udpn/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     1119 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/udpn/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ufs/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ufs/__init__.py
--rw-r--r--   0 root         (0)     1000     6973 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ufs/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ufs/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ufs/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000     3447 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ufs/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     1229 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ufs/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhost/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhost/__init__.py
--rw-r--r--   0 root         (0)     1000    59508 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhost/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhost/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhost/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    32531 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhost/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     7017 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhost/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhub/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhub/__init__.py
--rw-r--r--   0 root         (0)     1000     8100 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhub/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhub/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhub/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000     4876 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhub/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     1432 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uhub/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ulb/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ulb/__init__.py
--rw-r--r--   0 root         (0)     1000    41231 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ulb/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ulb/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ulb/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    18026 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ulb/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     6130 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/ulb/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/umem/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/umem/__init__.py
--rw-r--r--   0 root         (0)     1000    40366 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/umem/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/umem/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/umem/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    21862 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/umem/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     7051 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/umem/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/unet/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/unet/__init__.py
--rw-r--r--   0 root         (0)     1000    50021 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/unet/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/unet/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/unet/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    26271 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/unet/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     8843 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/unet/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uphost/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uphost/__init__.py
--rw-r--r--   0 root         (0)     1000    19002 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uphost/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uphost/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uphost/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    10161 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uphost/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     4258 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/uphost/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/usms/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/usms/__init__.py
--rw-r--r--   0 root         (0)     1000    19819 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/usms/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/usms/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/usms/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    10803 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/usms/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     2066 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/usms/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/vpc/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/vpc/__init__.py
--rw-r--r--   0 root         (0)     1000    27332 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/vpc/client.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/services/vpc/schemas/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/vpc/schemas/__init__.py
--rw-r--r--   0 root         (0)     1000    14908 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/vpc/schemas/apis.py
--rw-r--r--   0 root         (0)     1000     4958 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/services/vpc/schemas/models.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/
--rw-r--r--   0 root         (0)     1000        0 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/__init__.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/driver/
--rw-r--r--   0 root         (0)     1000      122 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/driver/__init__.py
--rw-r--r--   0 root         (0)     1000     2585 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/driver/_scenario.py
--rw-r--r--   0 root         (0)     1000     1726 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/driver/_specification.py
--rw-r--r--   0 root         (0)     1000     5444 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/driver/_step.py
--rw-r--r--   0 root         (0)     1000      699 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/env.py
--rw-r--r--   0 root         (0)     1000      282 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/exc.py
--rw-r--r--   0 root         (0)     1000     1715 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/funcs.py
--rw-r--r--   0 root         (0)     1000      863 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/mock.py
--rw-r--r--   0 root         (0)     1000     4301 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/op.py
--rw-r--r--   0 root         (0)     1000     6121 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/testing/utest.py
--rw-r--r--   0 root         (0)     1000       18 2020-09-22 04:16:34.000000 ucloud-sdk-python3-0.9.3/ucloud/version.py
-drwxr-sr-x   0 root         (0)     1000        0 2020-09-22 04:16:45.000000 ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/
--rw-r--r--   0 root         (0)     1000     2183 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1000     4744 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1000        1 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1000        1 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1000      253 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1000        7 2020-09-22 04:16:44.000000 ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/
+-rw-r--r--   0 root         (0)     1000     2183 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/PKG-INFO
+-rw-r--r--   0 root         (0)     1000     1073 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/README.md
+-rw-r--r--   0 root         (0)     1000       38 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/setup.cfg
+-rw-r--r--   0 root         (0)     1000     3518 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/setup.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/__init__.py
+-rw-r--r--   0 root         (0)     1000     3808 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/core/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/__init__.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/core/auth/
+-rw-r--r--   0 root         (0)     1000       71 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/auth/__init__.py
+-rw-r--r--   0 root         (0)     1000     2115 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/auth/_cfg.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/core/client/
+-rw-r--r--   0 root         (0)     1000      137 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/client/__init__.py
+-rw-r--r--   0 root         (0)     1000     3700 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/client/_cfg.py
+-rw-r--r--   0 root         (0)     1000     5906 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/client/_client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/core/exc/
+-rw-r--r--   0 root         (0)     1000      211 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/exc/__init__.py
+-rw-r--r--   0 root         (0)     1000     2301 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/exc/_exc.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/core/transport/
+-rw-r--r--   0 root         (0)     1000      223 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/transport/__init__.py
+-rw-r--r--   0 root         (0)     1000     4486 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/transport/_requests.py
+-rw-r--r--   0 root         (0)     1000     3174 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/transport/http.py
+-rw-r--r--   0 root         (0)     1000     1447 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/transport/utils.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/__init__.py
+-rw-r--r--   0 root         (0)     1000     1518 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/abstract.py
+-rw-r--r--   0 root         (0)     1000      967 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/encoder.py
+-rw-r--r--   0 root         (0)     1000     4089 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/fields.py
+-rw-r--r--   0 root         (0)     1000     2665 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/schema.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/core/utils/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/utils/__init__.py
+-rw-r--r--   0 root         (0)     1000      264 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/utils/compat.py
+-rw-r--r--   0 root         (0)     1000      819 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/utils/deco.py
+-rw-r--r--   0 root         (0)     1000      675 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/utils/log.py
+-rw-r--r--   0 root         (0)     1000     2123 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/core/utils/middleware.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/helpers/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/helpers/__init__.py
+-rw-r--r--   0 root         (0)     1000     2438 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/helpers/utils.py
+-rw-r--r--   0 root         (0)     1000     3516 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/helpers/wait.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/__init__.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/__init__.py
+-rw-r--r--   0 root         (0)     1000     5820 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000     2074 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     3890 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/pathx/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/pathx/__init__.py
+-rw-r--r--   0 root         (0)     1000     7599 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/pathx/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/pathx/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/pathx/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000     4949 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/pathx/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     1256 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/pathx/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/__init__.py
+-rw-r--r--   0 root         (0)     1000     4012 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000     2044 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     1250 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/__init__.py
+-rw-r--r--   0 root         (0)     1000     5893 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000     2831 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     2623 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/__init__.py
+-rw-r--r--   0 root         (0)     1000    34481 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    14424 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000    10802 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/__init__.py
+-rw-r--r--   0 root         (0)     1000   133021 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    82078 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000    24933 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udb/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udb/__init__.py
+-rw-r--r--   0 root         (0)     1000    83758 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udb/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udb/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udb/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    45521 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udb/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000    10110 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udb/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udisk/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udisk/__init__.py
+-rw-r--r--   0 root         (0)     1000    27508 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udisk/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udisk/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udisk/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    14671 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udisk/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     4134 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udisk/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udpn/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udpn/__init__.py
+-rw-r--r--   0 root         (0)     1000     9892 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udpn/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udpn/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udpn/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000     5181 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udpn/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     1105 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/udpn/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ufs/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ufs/__init__.py
+-rw-r--r--   0 root         (0)     1000     6880 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ufs/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ufs/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ufs/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000     3399 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ufs/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     1223 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ufs/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhost/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhost/__init__.py
+-rw-r--r--   0 root         (0)     1000    58774 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhost/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhost/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhost/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    32177 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhost/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     6963 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhost/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhub/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhub/__init__.py
+-rw-r--r--   0 root         (0)     1000     7922 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhub/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhub/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhub/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000     4792 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhub/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     1414 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uhub/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ulb/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ulb/__init__.py
+-rw-r--r--   0 root         (0)     1000    40687 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ulb/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ulb/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ulb/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    17786 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ulb/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     6074 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/ulb/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/umem/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/umem/__init__.py
+-rw-r--r--   0 root         (0)     1000    53160 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/umem/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/umem/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/umem/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    28485 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/umem/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     9740 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/umem/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/unet/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/unet/__init__.py
+-rw-r--r--   0 root         (0)     1000    49175 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/unet/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/unet/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/unet/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    25887 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/unet/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     8741 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/unet/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uphost/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uphost/__init__.py
+-rw-r--r--   0 root         (0)     1000    18685 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uphost/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uphost/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uphost/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    10029 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uphost/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     4209 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/uphost/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/usms/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/usms/__init__.py
+-rw-r--r--   0 root         (0)     1000    19569 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/usms/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/usms/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/usms/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    10683 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/usms/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     2042 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/usms/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/vpc/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/vpc/__init__.py
+-rw-r--r--   0 root         (0)     1000    27312 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/vpc/client.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/services/vpc/schemas/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/vpc/schemas/__init__.py
+-rw-r--r--   0 root         (0)     1000    14668 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/vpc/schemas/apis.py
+-rw-r--r--   0 root         (0)     1000     4916 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/services/vpc/schemas/models.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/
+-rw-r--r--   0 root         (0)     1000        0 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/__init__.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/driver/
+-rw-r--r--   0 root         (0)     1000      122 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/driver/__init__.py
+-rw-r--r--   0 root         (0)     1000     2585 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/driver/_scenario.py
+-rw-r--r--   0 root         (0)     1000     1726 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/driver/_specification.py
+-rw-r--r--   0 root         (0)     1000     5443 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/driver/_step.py
+-rw-r--r--   0 root         (0)     1000      698 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/env.py
+-rw-r--r--   0 root         (0)     1000      282 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/exc.py
+-rw-r--r--   0 root         (0)     1000     1708 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/funcs.py
+-rw-r--r--   0 root         (0)     1000      863 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/mock.py
+-rw-r--r--   0 root         (0)     1000     4205 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/op.py
+-rw-r--r--   0 root         (0)     1000     6119 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/testing/utest.py
+-rw-r--r--   0 root         (0)     1000       18 2020-09-25 12:31:18.000000 ucloud-sdk-python3-0.9.4/ucloud/version.py
+drwxr-sr-x   0 root         (0)     1000        0 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/
+-rw-r--r--   0 root         (0)     1000     2183 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1000     4744 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1000        1 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1000        1 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1000      253 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1000        7 2020-09-25 12:31:28.000000 ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/top_level.txt
```

### Comparing `ucloud-sdk-python3-0.9.3/PKG-INFO` & `ucloud-sdk-python3-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucloud-sdk-python3
-Version: 0.9.3
+Version: 0.9.4
 Summary: UCloud Service Development Kit - Python
 Home-page: https://github.com/ucloud/ucloud-sdk-python3
 Author: ucloud
 Author-email: esl_ipdd@ucloud.cn
 License: Apache License 2.0
 Description: <p align="center">
             <img src="https://ucloud-sdk.dl.ufileos.com/logos%2Flogo-mini.png" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ucloud-sdk-python3 Version: 0.9.3 Summary: UCloud
+Metadata-Version: 2.1 Name: ucloud-sdk-python3 Version: 0.9.4 Summary: UCloud
 Service Development Kit - Python Home-page: https://github.com/ucloud/ucloud-
 sdk-python3 Author: ucloud Author-email: esl_ipdd@ucloud.cn License: Apache
 License 2.0 Description:
            [https://ucloud-sdk.dl.ufileos.com/logos%2Flogo-mini.png]
                        ****** UCloud SDK Python 3 ******
    [Latest_Stable_Version] [Travis_CI_Status] [Codecov_Status] [Doc_Status]
 UCloud SDK is a Python client library for accessing the UCloud API. This client
```

### Comparing `ucloud-sdk-python3-0.9.3/README.md` & `ucloud-sdk-python3-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/setup.py` & `ucloud-sdk-python3-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/client.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/auth/_cfg.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/auth/_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     fields = {
         "public_key": fields.Str(required=True),
         "private_key": fields.Str(required=True),
     }
 
 
 def verify_ac(private_key: str, params: dict) -> str:
-    """ calculate signature by private_key/public_key
+    """calculate signature by private_key/public_key
 
     the keys can be found on `APIKey documentation <https://console.ucloud.cn/uapi/apikey>`__
 
     >>> verify_ac("my_private_key", {"foo": "bar"})
     '634edc1bb957c0d65e5ab5494cf3b7784fbc87af'
 
     >>> verify_ac("my_private_key", {"foo": "bar"})
@@ -35,15 +35,15 @@
     hash_new = hashlib.sha1()
     hash_new.update(simplified.encode("utf-8"))
     hash_value = hash_new.hexdigest()
     return hash_value
 
 
 class Credential:
-    """ credential is the object to store credential information
+    """credential is the object to store credential information
 
     the keys can be found on `APIKey documentation <https://console.ucloud.cn/uapi/apikey>`__
 
     it can calculate signature for OpenAPI:
 
     >>> cred = Credential('my_public_key', 'my_private_key')
     >>> cred.verify_ac({"foo": "bar"})
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/client/_cfg.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/client/_cfg.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/client/_client.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/client/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             middleware = Middleware()
             middleware.response(self.logged_response_handler)
             middleware.request(self.logged_request_handler)
             middleware.exception(self.logged_exception_handler)
         self._middleware = middleware
 
     def invoke(self, action: str, args: dict = None, **options) -> dict:
-        """ invoke will invoke the action with arguments data and options
+        """invoke will invoke the action with arguments data and options
 
         :param str action: the api action, like `CreateUHostInstance`
         :param dict args: arguments of api(action), see doc: `UCloud API Documentation <https://docs.ucloud.cn/api>`__
         :return:
         """
         retries = 0
         max_retries = options.get("max_retries") or self.config.max_retries
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/exc/_exc.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/exc/_exc.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/transport/_requests.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/transport/_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ucloud.core.transport import http
 from ucloud.core.transport.http import Request, Response, SSLOption
 from ucloud.core.utils.middleware import Middleware
 from ucloud.core import exc
 
 
 class RequestsTransport(http.Transport):
-    """ transport is the implementation of http client, use for send a request and return a http response
+    """transport is the implementation of http client, use for send a request and return a http response
 
     :type max_retries: int
     :param max_retries: max retries is the max number of transport request when occur http error
     :type backoff_factor: float
     :param backoff_factor: backoff factor will calculate the backoff delay during retrying,
         the backoff delay = {backoff factor} * (2 ^ ({number of total retries} - 1))
     :type status_forcelist: tuple
@@ -31,15 +31,15 @@
         self.backoff_factor = backoff_factor
         self.status_forcelist = status_forcelist
 
         self._adapter = self._load_adapter(max_retries)
         self._middleware = Middleware()
 
     def send(self, req: Request, **options: typing.Any) -> http.Response:
-        """ send request and return the response
+        """send request and return the response
 
         :param req: the full http request descriptor
         :return: the response of http request
         """
         for handler in self.middleware.request_handlers:
             req = handler(req)
 
@@ -53,15 +53,15 @@
         for handler in self.middleware.response_handlers:
             resp = handler(resp)
 
         return resp
 
     @property
     def middleware(self) -> Middleware:
-        """ the middleware object, see :mod:
+        """the middleware object, see :mod:
 
         :return: the transport middleware
         """
         return self._middleware
 
     def _send(self, req: Request, **options: typing.Any) -> requests.Response:
         with requests.Session() as session:
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/transport/http.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/transport/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,29 +59,28 @@
         self.content = content
         self.encoding = encoding
         self.response_time = 0
         self.headers = headers or {}
         self.request_uuid = self.headers.get(REQUEST_UUID_HEADER_KEY)
 
     def json(self, **kwargs) -> typing.Optional[dict]:
-        """ json will return the bytes of content
-        """
+        """json will return the bytes of content"""
         if not self.content:
             return None
 
         try:
             return self._decode_json(**kwargs)
         except Exception as e:
             raise exc.InvalidResponseException(
                 self.content, str(e), request_uuid=self.request_uuid
             )
 
     @property
     def text(self):
-        """ text will return the unicode string of content,
+        """text will return the unicode string of content,
         see `requests.Response.text`
         """
         if not self.content:
             return str("")
 
         # Decode unicode from given encoding.
         try:
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/transport/utils.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/transport/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Null bytes; no need to recreate these on each call to guess_json_utf
 _null = "\x00".encode("ascii")  # encoding to ASCII for Python 3
 _null2 = _null * 2
 _null3 = _null * 3
 
 
 def guess_json_utf(data):
-    """ guess_json_utf will detect the encoding of bytes,
+    """guess_json_utf will detect the encoding of bytes,
     see `requests.utils.guess_json_utf`
 
     :rtype: str
     """
     # JSON always starts with two ASCII characters, so detection is as
     # easy as counting the nulls and from their location and count
     # determine the encoding. Also detect a BOM, if present.
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/abstract.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/abstract.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/encoder.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/encoder.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/fields.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ucloud.core.typesystem import abstract
 from ucloud.core.exc import ValidationException
 from ucloud.core.utils.compat import str
 
 
 class List(abstract.Field):
-    """ array param is the custom field to parse custom param such as:
+    """array param is the custom field to parse custom param such as:
 
     - IP.N
     - UDisk.N.Size
     - NetInterface.N.EIP.Bandwidth
     """
 
     def __init__(
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/typesystem/schema.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/typesystem/schema.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/utils/deco.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/utils/deco.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import logging
 
 logger = logging.getLogger("ucloud")
 
 
 def deprecated(instead_of="", message=""):
-    """ deprecated is a decorator to mark a function is deprecated.
+    """deprecated is a decorator to mark a function is deprecated.
     it will logging warning when this function called
 
     >>> @deprecated(instead_of="new_function")
     ... def an_old_function():
     ...     pass
     """
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/utils/log.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/core/utils/middleware.py` & `ucloud-sdk-python3-0.9.4/ucloud/core/utils/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 class Middleware:
-    """ middleware is the object to store request/response handlers
+    """middleware is the object to store request/response handlers
 
     >>> middleware = Middleware()
 
     Add a request handler to prepare the request
 
     >>> @middleware.request
     ... def prepare(req):
@@ -23,39 +23,39 @@
 
     def __init__(self):
         self.request_handlers = []
         self.response_handlers = []
         self.exception_handlers = []
 
     def request(self, handler, index=-1):
-        """ request is the request handler register to add request handler.
+        """request is the request handler register to add request handler.
 
         :param handler: request handler function, receive request object
                         and return a new request
         :param int index: the position of request in the handler list,
                           default is append it to end
         :return:
         """
         self.request_handlers.insert(index, handler)
         return handler
 
     def response(self, handler, index=-1):
-        """ response is the response handler register to add response handler.
+        """response is the response handler register to add response handler.
 
         :param handler: response handler function, receive response object
                         and return a new response
         :param int index: the position of response in the handler list,
                           default is append it to end
         :return:
         """
         self.response_handlers.insert(index, handler)
         return handler
 
     def exception(self, handler, index=-1):
-        """ exception is the exception handler register to add exception handler.
+        """exception is the exception handler register to add exception handler.
 
         :param handler: exception handler function, receive exception object
                         and raise a new exception or ignore it
         :param int index: the position of handler in the handler list,
                           default is append it to end
         :return:
         """
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/helpers/utils.py` & `ucloud-sdk-python3-0.9.4/ucloud/helpers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     number_letters: str = _numbers,
     special_letters: str = _specials,
     min_lower: int = 1,
     min_upper: int = 1,
     min_number: int = 1,
     min_specials: int = 1,
 ):
-    """ generate password for any resource
+    """generate password for any resource
 
     >>> len(gen_password(20))
     20
 
     :param int n: password total length
     :param str lower_letters: all lowercase letters
     :param str upper_letters: all uppercase letters
@@ -69,22 +69,22 @@
 def first(arr: typing.List[typing.Any]) -> typing.Any:
     if len(arr) == 0:
         return None
     return arr[0]
 
 
 def b64encode(s: str) -> str:
-    """ base64 encode
+    """base64 encode
 
     :param str s: input string
     :return: base64 string
     """
     return base64.b64encode(s.encode()).decode()
 
 
 def b64decode(s: str) -> str:
-    """ base64 decode
+    """base64 decode
 
     :param str s: base64 string
     :return: output string
     """
     return base64.b64decode(s.encode()).decode()
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/helpers/wait.py` & `ucloud-sdk-python3-0.9.4/ucloud/helpers/wait.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class WaitTimeoutException(exc.UCloudException):
     pass
 
 
 class StateConf:
-    """ StateConf is the utilities class to wait the state return by refresh function achieve the specific state,
+    """StateConf is the utilities class to wait the state return by refresh function achieve the specific state,
     the generally usage is wait the cloud resource, such as uhost, udb ... is
     ready after created.
     """
 
     def __init__(
         self,
         pending: typing.List[str],
@@ -73,15 +73,15 @@
     target: typing.List[str],
     refresh: typing.Callable,
     timeout: float,
     startup_delay: float = 0,
     min_backoff_interval: float = 0.1,
     max_backoff_interval: float = MAX_BACKOFF_INTERVAL,
 ):
-    """ wait_for_state is a utilities function to wait the state return by refresh function achieve the specific state,
+    """wait_for_state is a utilities function to wait the state return by refresh function achieve the specific state,
     the generally usage is wait the cloud resource, such as uhost, udb ... is
     ready after created.
 
     >>> wait_for_state(
     ...     pending=["pending"],
     ...     target=["running"],
     ...     refresh=lambda: "running",
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,34 +14,34 @@
         super(IPSecVPNClient, self).__init__(
             config, transport, middleware, logger
         )
 
     def describe_remote_vpn_gateway(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeRemoteVPNGateway - 获取客户VPN网关信息
+        """DescribeRemoteVPNGateway - 获取客户VPN网关信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 数据分页值, 默认为20
         - **Offset** (int) - 数据偏移量, 默认为0
         - **RemoteVPNGatewayIds** (list) - 客户VPN网关的资源ID，例如RemoteVPNGatewayIds.0代表希望获取客户VPN网关1的信息，RemoteVPNGatewayIds.1代表客户VPN网关2，如果为空，则返回当前Region中所有客户VPN网关实例的信息
         - **Tag** (str) - 业务组名称，若指定则返回业务组下所有客户VPN网关信息
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **RemoteVPNGatewayDataSet** 模型定义
         - **TotalCount** (int) - 符合条件的客户VPN网关总数
-        
+
         **Response Model**
-        
-        **RemoteVPNGatewayDataSet** 
-        
+
+        **RemoteVPNGatewayDataSet**
+
         - **ActiveTunnels** (str) - 活跃的隧道id
         - **CreateTime** (int) - 创建时间
         - **Remark** (str) - 备注
         - **RemoteVPNGatewayAddr** (str) - 客户网关IP地址
         - **RemoteVPNGatewayId** (str) - 客户网关ID
         - **RemoteVPNGatewayName** (str) - 客户网关名称
         - **Tag** (str) - 用户组
@@ -58,57 +58,57 @@
 
         resp = self.invoke("DescribeRemoteVPNGateway", d, **kwargs)
         return apis.DescribeRemoteVPNGatewayResponseSchema().loads(resp)
 
     def describe_vpn_tunnel(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeVPNTunnel - 获取VPN隧道信息
+        """DescribeVPNTunnel - 获取VPN隧道信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 数据分页值, 默认为20
         - **Offset** (int) - 数据偏移量, 默认为0
         - **Tag** (str) - 业务组名称，若指定则返回指定的业务组下的所有VPN网关的信息
         - **VPNTunnelIds** (list) - VPN隧道的资源ID，例如VPNTunnelIds.0代表希望获取信息的VPN隧道1，VPNTunneIds.1代表VPN隧道2，如果为空，则返回当前Region中所有的VPN隧道实例
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **VPNTunnelDataSet** 模型定义
         - **TotalCount** (int) - VPN隧道总数
-        
+
         **Response Model**
-        
-        **IPSecData** 
-        
+
+        **IPSecData**
+
         - **IPSecAuthenticationAlgorithm** (str) - IPSec通道中使用的认证算法
         - **IPSecEncryptionAlgorithm** (str) - IPSec通道中使用的加密算法
         - **IPSecLocalSubnetIds** (list) - 指定VPN连接的本地子网，用逗号分隔
         - **IPSecPFSDhGroup** (str) - 是否开启PFS功能,Disable表示关闭，数字表示DH组
         - **IPSecProtocol** (str) - 使用的安全协议，ESP或AH
         - **IPSecRemoteSubnets** (list) - 指定VPN连接的客户网段，用逗号分隔
         - **IPSecSALifetime** (str) - IPSec中SA的生存时间
         - **IPSecSALifetimeBytes** (str) - IPSec中SA的生存时间（以字节计）
 
-        **IKEData** 
-        
+        **IKEData**
+
         - **IKEAuthenticationAlgorithm** (str) - IKE认证算法
         - **IKEDhGroup** (str) - IKEDH组
         - **IKEEncryptionAlgorithm** (str) - IKE加密算法
         - **IKEExchangeMode** (str) - IKEv1协商模式
         - **IKELocalId** (str) - IKE本地ID标识
         - **IKEPreSharedKey** (str) - IKE预共享秘钥
         - **IKERemoteId** (str) - IKE对端ID标识
         - **IKESALifetime** (str) - IKE秘钥生存时间
         - **IKEVersion** (str) - IKE版本
 
-        **VPNTunnelDataSet** 
-        
+        **VPNTunnelDataSet**
+
         - **CreateTime** (int) - 创建时间
         - **IKEData** (dict) - 见 **IKEData** 模型定义
         - **IPSecData** (dict) - 见 **IPSecData** 模型定义
         - **Remark** (str) - 备注
         - **RemoteVPNGatewayId** (str) - 对端网关Id
         - **RemoteVPNGatewayName** (str) - 对端网关名字
         - **Tag** (str) - 用户组
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/schemas/apis.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 API: DescribeRemoteVPNGateway
 
 获取客户VPN网关信息
 """
 
 
 class DescribeRemoteVPNGatewayRequestSchema(schema.RequestSchema):
-    """ DescribeRemoteVPNGateway - 获取客户VPN网关信息
-    """
+    """DescribeRemoteVPNGateway - 获取客户VPN网关信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RemoteVPNGatewayIds": fields.List(fields.Str()),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class DescribeRemoteVPNGatewayResponseSchema(schema.ResponseSchema):
-    """ DescribeRemoteVPNGateway - 获取客户VPN网关信息
-    """
+    """DescribeRemoteVPNGateway - 获取客户VPN网关信息"""
 
     fields = {
         "DataSet": fields.List(
             models.RemoteVPNGatewayDataSetSchema(),
             required=False,
             load_from="DataSet",
         ),
@@ -47,30 +45,28 @@
 API: DescribeVPNTunnel
 
 获取VPN隧道信息
 """
 
 
 class DescribeVPNTunnelRequestSchema(schema.RequestSchema):
-    """ DescribeVPNTunnel - 获取VPN隧道信息
-    """
+    """DescribeVPNTunnel - 获取VPN隧道信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VPNTunnelIds": fields.List(fields.Str()),
     }
 
 
 class DescribeVPNTunnelResponseSchema(schema.ResponseSchema):
-    """ DescribeVPNTunnel - 获取VPN隧道信息
-    """
+    """DescribeVPNTunnel - 获取VPN隧道信息"""
 
     fields = {
         "DataSet": fields.List(
             models.VPNTunnelDataSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ipsecvpn/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ipsecvpn/schemas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class RemoteVPNGatewayDataSetSchema(schema.ResponseSchema):
-    """ RemoteVPNGatewayDataSet - DescribeRemoteVPNGateway返回参数
-    """
+    """RemoteVPNGatewayDataSet - DescribeRemoteVPNGateway返回参数"""
 
     fields = {
         "ActiveTunnels": fields.Str(required=False, load_from="ActiveTunnels"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Remark": fields.Str(required=False, load_from="Remark"),
         "RemoteVPNGatewayAddr": fields.Str(
             required=False, load_from="RemoteVPNGatewayAddr"
@@ -22,16 +21,15 @@
         ),
         "Tag": fields.Str(required=False, load_from="Tag"),
         "TunnelCount": fields.Int(required=False, load_from="TunnelCount"),
     }
 
 
 class IPSecDataSchema(schema.ResponseSchema):
-    """ IPSecData - IPSec参数
-    """
+    """IPSecData - IPSec参数"""
 
     fields = {
         "IPSecAuthenticationAlgorithm": fields.Str(
             required=False, load_from="IPSecAuthenticationAlgorithm"
         ),
         "IPSecEncryptionAlgorithm": fields.Str(
             required=False, load_from="IPSecEncryptionAlgorithm"
@@ -48,16 +46,15 @@
         "IPSecSALifetimeBytes": fields.Str(
             required=False, load_from="IPSecSALifetimeBytes"
         ),
     }
 
 
 class IKEDataSchema(schema.ResponseSchema):
-    """ IKEData - IKE信息
-    """
+    """IKEData - IKE信息"""
 
     fields = {
         "IKEAuthenticationAlgorithm": fields.Str(
             required=False, load_from="IKEAuthenticationAlgorithm"
         ),
         "IKEDhGroup": fields.Str(required=False, load_from="IKEDhGroup"),
         "IKEEncryptionAlgorithm": fields.Str(
@@ -73,16 +70,15 @@
         "IKERemoteId": fields.Str(required=False, load_from="IKERemoteId"),
         "IKESALifetime": fields.Str(required=False, load_from="IKESALifetime"),
         "IKEVersion": fields.Str(required=False, load_from="IKEVersion"),
     }
 
 
 class VPNTunnelDataSetSchema(schema.ResponseSchema):
-    """ VPNTunnelDataSet - DescribeVPNTunnel信息
-    """
+    """VPNTunnelDataSet - DescribeVPNTunnel信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "IKEData": IKEDataSchema(),
         "IPSecData": IPSecDataSchema(),
         "Remark": fields.Str(required=False, load_from="Remark"),
         "RemoteVPNGatewayId": fields.Str(
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/pathx/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/pathx/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,34 +12,34 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(PathXClient, self).__init__(config, transport, middleware, logger)
 
     def create_global_ssh_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateGlobalSSHInstance - 创建GlobalSSH实例
+        """CreateGlobalSSHInstance - 创建GlobalSSH实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID,如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID,如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Area** (str) - (Required) 填写支持SSH访问IP的地区名称，如“洛杉矶”，“新加坡”，“香港”，“东京”，“华盛顿”，“法兰克福”。Area和AreaCode两者必填一个
         - **AreaCode** (str) - (Required) AreaCode, 区域航空港国际通用代码。Area和AreaCode两者必填一个
         - **Port** (int) - (Required) SSH端口，1-65535且不能使用80，443端口
         - **TargetIP** (str) - (Required) 被SSH访问的IP
         - **ChargeType** (str) - 支付方式，如按月、按年、按时
         - **CouponId** (str) - 使用代金券可冲抵部分费用
         - **Quantity** (int) - 购买数量
         - **Remark** (str) - 备注信息
-        
+
         **Response**
 
         - **AcceleratingDomain** (str) - 加速域名，访问该域名可就近接入
         - **InstanceId** (str) - 实例ID，资源唯一标识
         - **Message** (str) - 提示信息
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.CreateGlobalSSHInstanceRequestSchema().dumps(d)
 
         # build options
@@ -47,53 +47,53 @@
 
         resp = self.invoke("CreateGlobalSSHInstance", d, **kwargs)
         return apis.CreateGlobalSSHInstanceResponseSchema().loads(resp)
 
     def delete_global_ssh_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteGlobalSSHInstance - 删除GlobalSSH实例
+        """DeleteGlobalSSHInstance - 删除GlobalSSH实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID,如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID,如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **InstanceId** (str) - (Required) 实例Id,资源的唯一标识
-        
+
         **Response**
 
         - **Message** (str) - 提示信息
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.DeleteGlobalSSHInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteGlobalSSHInstance", d, **kwargs)
         return apis.DeleteGlobalSSHInstanceResponseSchema().loads(resp)
 
     def describe_global_ssh_area(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeGlobalSSHArea - 获取GlobalSSH覆盖的地区列表 用于控制显示哪些机房地域可以使用SSH特性
+        """DescribeGlobalSSHArea - 获取GlobalSSH覆盖的地区列表 用于控制显示哪些机房地域可以使用SSH特性
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID,如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID,如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 机房地域代号，如hk、 us-ca、 us-ws等。不填默认为空，返回所有支持地区。
-        
+
         **Response**
 
         - **AreaSet** (list) - 见 **GlobalSSHArea** 模型定义
         - **Message** (str) - 提示信息
-        
+
         **Response Model**
-        
-        **GlobalSSHArea** 
-        
+
+        **GlobalSSHArea**
+
         - **Area** (str) - GlobalSSH覆盖的地区,如香港、东京、洛杉矶等
         - **AreaCode** (str) - 地区代号,以地区AirPort Code
         - **RegionSet** (list) - ucloud机房代号构成的数组，如["hk","us-ca"]
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
@@ -102,29 +102,29 @@
 
         resp = self.invoke("DescribeGlobalSSHArea", d, **kwargs)
         return apis.DescribeGlobalSSHAreaResponseSchema().loads(resp)
 
     def describe_global_ssh_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeGlobalSSHInstance - 获取GlobalSSH实例列表（传实例ID获取单个实例信息，不传获取项目下全部实例）
+        """DescribeGlobalSSHInstance - 获取GlobalSSH实例列表（传实例ID获取单个实例信息，不传获取项目下全部实例）
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID，如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID，如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **InstanceId** (str) - 实例ID，资源唯一标识
-        
+
         **Response**
 
         - **InstanceSet** (list) - 见 **GlobalSSHInfo** 模型定义
-        
+
         **Response Model**
-        
-        **GlobalSSHInfo** 
-        
+
+        **GlobalSSHInfo**
+
         - **AcceleratingDomain** (str) - 加速域名
         - **Area** (str) - 被SSH访问的IP所在地区
         - **ChargeType** (str) - 支付周期，如Month,Year等
         - **CreateTime** (int) - 资源创建时间戳
         - **ExpireTime** (int) - 资源过期时间戳
         - **InstanceId** (str) - 实例ID，资源唯一标识
         - **Port** (int) - SSH登陆端口
@@ -139,50 +139,50 @@
 
         resp = self.invoke("DescribeGlobalSSHInstance", d, **kwargs)
         return apis.DescribeGlobalSSHInstanceResponseSchema().loads(resp)
 
     def modify_global_ssh_port(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyGlobalSSHPort - 修改GlobalSSH端口
+        """ModifyGlobalSSHPort - 修改GlobalSSH端口
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID，如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID，如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **InstanceId** (str) - (Required) 实例ID,资源唯一标识
         - **Port** (int) - (Required) 调整后的SSH登陆端口
-        
+
         **Response**
 
         - **Message** (str) - 提示信息
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.ModifyGlobalSSHPortRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyGlobalSSHPort", d, **kwargs)
         return apis.ModifyGlobalSSHPortResponseSchema().loads(resp)
 
     def modify_global_ssh_remark(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyGlobalSSHRemark - 修改GlobalSSH备注
+        """ModifyGlobalSSHRemark - 修改GlobalSSH备注
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID，如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID，如org-xxxx。请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **InstanceId** (str) - (Required) 实例ID,资源唯一标识
         - **Remark** (str) - 备注信息，不填默认为空字符串
-        
+
         **Response**
 
         - **Message** (str) - 接口返回消息
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.ModifyGlobalSSHRemarkRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyGlobalSSHRemark", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/pathx/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/pathx/schemas/apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: CreateGlobalSSHInstance
 
 创建GlobalSSH实例
 """
 
 
 class CreateGlobalSSHInstanceRequestSchema(schema.RequestSchema):
-    """ CreateGlobalSSHInstance - 创建GlobalSSH实例
-    """
+    """CreateGlobalSSHInstance - 创建GlobalSSH实例"""
 
     fields = {
         "Area": fields.Str(required=True, dump_to="Area"),
         "AreaCode": fields.Str(required=True, dump_to="AreaCode"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Port": fields.Int(required=True, dump_to="Port"),
@@ -29,16 +28,15 @@
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "TargetIP": fields.Str(required=True, dump_to="TargetIP"),
     }
 
 
 class CreateGlobalSSHInstanceResponseSchema(schema.ResponseSchema):
-    """ CreateGlobalSSHInstance - 创建GlobalSSH实例
-    """
+    """CreateGlobalSSHInstance - 创建GlobalSSH实例"""
 
     fields = {
         "AcceleratingDomain": fields.Str(
             required=False, load_from="AcceleratingDomain"
         ),
         "InstanceId": fields.Str(required=True, load_from="InstanceId"),
         "Message": fields.Str(required=False, load_from="Message"),
@@ -49,50 +47,46 @@
 API: DeleteGlobalSSHInstance
 
 删除GlobalSSH实例
 """
 
 
 class DeleteGlobalSSHInstanceRequestSchema(schema.RequestSchema):
-    """ DeleteGlobalSSHInstance - 删除GlobalSSH实例
-    """
+    """DeleteGlobalSSHInstance - 删除GlobalSSH实例"""
 
     fields = {
         "InstanceId": fields.Str(required=True, dump_to="InstanceId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
     }
 
 
 class DeleteGlobalSSHInstanceResponseSchema(schema.ResponseSchema):
-    """ DeleteGlobalSSHInstance - 删除GlobalSSH实例
-    """
+    """DeleteGlobalSSHInstance - 删除GlobalSSH实例"""
 
     fields = {"Message": fields.Str(required=False, load_from="Message")}
 
 
 """
 API: DescribeGlobalSSHArea
 
 获取GlobalSSH覆盖的地区列表 用于控制显示哪些机房地域可以使用SSH特性
 """
 
 
 class DescribeGlobalSSHAreaRequestSchema(schema.RequestSchema):
-    """ DescribeGlobalSSHArea - 获取GlobalSSH覆盖的地区列表 用于控制显示哪些机房地域可以使用SSH特性
-    """
+    """DescribeGlobalSSHArea - 获取GlobalSSH覆盖的地区列表 用于控制显示哪些机房地域可以使用SSH特性"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
     }
 
 
 class DescribeGlobalSSHAreaResponseSchema(schema.ResponseSchema):
-    """ DescribeGlobalSSHArea - 获取GlobalSSH覆盖的地区列表 用于控制显示哪些机房地域可以使用SSH特性
-    """
+    """DescribeGlobalSSHArea - 获取GlobalSSH覆盖的地区列表 用于控制显示哪些机房地域可以使用SSH特性"""
 
     fields = {
         "AreaSet": fields.List(
             models.GlobalSSHAreaSchema(), required=False, load_from="AreaSet"
         ),
         "Message": fields.Str(required=False, load_from="Message"),
     }
@@ -102,26 +96,24 @@
 API: DescribeGlobalSSHInstance
 
 获取GlobalSSH实例列表（传实例ID获取单个实例信息，不传获取项目下全部实例）
 """
 
 
 class DescribeGlobalSSHInstanceRequestSchema(schema.RequestSchema):
-    """ DescribeGlobalSSHInstance - 获取GlobalSSH实例列表（传实例ID获取单个实例信息，不传获取项目下全部实例）
-    """
+    """DescribeGlobalSSHInstance - 获取GlobalSSH实例列表（传实例ID获取单个实例信息，不传获取项目下全部实例）"""
 
     fields = {
         "InstanceId": fields.Str(required=False, dump_to="InstanceId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
     }
 
 
 class DescribeGlobalSSHInstanceResponseSchema(schema.ResponseSchema):
-    """ DescribeGlobalSSHInstance - 获取GlobalSSH实例列表（传实例ID获取单个实例信息，不传获取项目下全部实例）
-    """
+    """DescribeGlobalSSHInstance - 获取GlobalSSH实例列表（传实例ID获取单个实例信息，不传获取项目下全部实例）"""
 
     fields = {
         "InstanceSet": fields.List(
             models.GlobalSSHInfoSchema(),
             required=False,
             load_from="InstanceSet",
         )
@@ -132,47 +124,43 @@
 API: ModifyGlobalSSHPort
 
 修改GlobalSSH端口
 """
 
 
 class ModifyGlobalSSHPortRequestSchema(schema.RequestSchema):
-    """ ModifyGlobalSSHPort - 修改GlobalSSH端口
-    """
+    """ModifyGlobalSSHPort - 修改GlobalSSH端口"""
 
     fields = {
         "InstanceId": fields.Str(required=True, dump_to="InstanceId"),
         "Port": fields.Int(required=True, dump_to="Port"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
     }
 
 
 class ModifyGlobalSSHPortResponseSchema(schema.ResponseSchema):
-    """ ModifyGlobalSSHPort - 修改GlobalSSH端口
-    """
+    """ModifyGlobalSSHPort - 修改GlobalSSH端口"""
 
     fields = {"Message": fields.Str(required=False, load_from="Message")}
 
 
 """
 API: ModifyGlobalSSHRemark
 
 修改GlobalSSH备注
 """
 
 
 class ModifyGlobalSSHRemarkRequestSchema(schema.RequestSchema):
-    """ ModifyGlobalSSHRemark - 修改GlobalSSH备注
-    """
+    """ModifyGlobalSSHRemark - 修改GlobalSSH备注"""
 
     fields = {
         "InstanceId": fields.Str(required=True, dump_to="InstanceId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
     }
 
 
 class ModifyGlobalSSHRemarkResponseSchema(schema.ResponseSchema):
-    """ ModifyGlobalSSHRemark - 修改GlobalSSH备注
-    """
+    """ModifyGlobalSSHRemark - 修改GlobalSSH备注"""
 
     fields = {"Message": fields.Str(required=False, load_from="Message")}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/pathx/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/pathx/schemas/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class GlobalSSHAreaSchema(schema.ResponseSchema):
-    """ GlobalSSHArea - GlobalSSH覆盖地区,包括关联的UCloud机房信息
-    """
+    """GlobalSSHArea - GlobalSSH覆盖地区,包括关联的UCloud机房信息"""
 
     fields = {
         "Area": fields.Str(required=True, load_from="Area"),
         "AreaCode": fields.Str(required=True, load_from="AreaCode"),
         "RegionSet": fields.List(fields.Str()),
     }
 
 
 class GlobalSSHInfoSchema(schema.ResponseSchema):
-    """ GlobalSSHInfo - GlobalSSH实例信息
-    """
+    """GlobalSSHInfo - GlobalSSH实例信息"""
 
     fields = {
         "AcceleratingDomain": fields.Str(
             required=True, load_from="AcceleratingDomain"
         ),
         "Area": fields.Str(required=True, load_from="Area"),
         "ChargeType": fields.Str(required=True, load_from="ChargeType"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,29 +14,29 @@
         super(StepFlowClient, self).__init__(
             config, transport, middleware, logger
         )
 
     def create_sf_workflow_from_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateSFWorkflowFromTemplate - 导入工作流定义
+        """CreateSFWorkflowFromTemplate - 导入工作流定义
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Namespace** (str) - (Required) 需要创建的工作流namespace
         - **Workflow** (str) - (Required) 描述工作流定义的base64字符串
         - **WorkflowName** (str) - (Required) 需要创建的工作流名称
-        
+
         **Response**
 
         - **Message** (str) - 返回消息
         - **Version** (int) - 创建的工作流版本号
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateSFWorkflowFromTemplateRequestSchema().dumps(d)
 
         # build options
@@ -44,50 +44,50 @@
 
         resp = self.invoke("CreateSFWorkflowFromTemplate", d, **kwargs)
         return apis.CreateSFWorkflowFromTemplateResponseSchema().loads(resp)
 
     def get_sf_workflow_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetSFWorkflowTemplate - 导出工作流定义
+        """GetSFWorkflowTemplate - 导出工作流定义
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **WorkflowId** (str) - (Required) 被导出工作流的Id
         - **WorkflowVersion** (int) - 被导出工作流的版本号。取值范围：WorkflowVersion >= 1；默认会获取发布版本对应的workflow；超过最大版本会返回错误
-        
+
         **Response**
 
         - **Message** (str) - 返回消息
         - **Version** (int) - 导出工作流的版本号
         - **Workflow** (dict) - 见 **WorkflowTemplate** 模型定义
         - **WorkflowId** (str) - 导出工作流的Id
-        
+
         **Response Model**
-        
-        **Param** 
-        
+
+        **Param**
+
         - **Name** (str) - 参数名称
         - **Type** (str) - 参数类型
         - **Value** (str) - 参数值
 
-        **ActivityTemplate** 
-        
+        **ActivityTemplate**
+
         - **Input** (dict) - Activity的输入
         - **Name** (str) - Activity的名字
         - **Next** (str) - 下一个Activity的名字
         - **Output** (list) - Activity的输出，详见Param
         - **RetryTimes** (str) - Activity的重试次数
         - **Timeout** (str) - Activity的超时时间
         - **Type** (str) - Activity的类型
 
-        **WorkflowTemplate** 
-        
+        **WorkflowTemplate**
+
         - **Activites** (list) - 见 **ActivityTemplate** 模型定义
         - **Input** (list) - 见 **Param** 模型定义
         - **Output** (list) - 见 **Param** 模型定义
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/schemas/apis.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 API: CreateSFWorkflowFromTemplate
 
 导入工作流定义
 """
 
 
 class CreateSFWorkflowFromTemplateRequestSchema(schema.RequestSchema):
-    """ CreateSFWorkflowFromTemplate - 导入工作流定义
-    """
+    """CreateSFWorkflowFromTemplate - 导入工作流定义"""
 
     fields = {
         "Namespace": fields.Str(required=True, dump_to="Namespace"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Workflow": fields.Base64(required=True, dump_to="Workflow"),
         "WorkflowName": fields.Str(required=True, dump_to="WorkflowName"),
     }
 
 
 class CreateSFWorkflowFromTemplateResponseSchema(schema.ResponseSchema):
-    """ CreateSFWorkflowFromTemplate - 导入工作流定义
-    """
+    """CreateSFWorkflowFromTemplate - 导入工作流定义"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "Version": fields.Int(required=True, load_from="Version"),
     }
 
 
@@ -42,30 +40,28 @@
 API: GetSFWorkflowTemplate
 
 导出工作流定义
 """
 
 
 class GetSFWorkflowTemplateRequestSchema(schema.RequestSchema):
-    """ GetSFWorkflowTemplate - 导出工作流定义
-    """
+    """GetSFWorkflowTemplate - 导出工作流定义"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "WorkflowId": fields.Str(required=True, dump_to="WorkflowId"),
         "WorkflowVersion": fields.Int(
             required=False, dump_to="WorkflowVersion"
         ),
     }
 
 
 class GetSFWorkflowTemplateResponseSchema(schema.ResponseSchema):
-    """ GetSFWorkflowTemplate - 导出工作流定义
-    """
+    """GetSFWorkflowTemplate - 导出工作流定义"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
         "Version": fields.Int(required=True, load_from="Version"),
         "Workflow": models.WorkflowTemplateSchema(),
         "WorkflowId": fields.Str(required=True, load_from="WorkflowId"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/stepflow/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/stepflow/schemas/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class ParamSchema(schema.ResponseSchema):
-    """ Param - 工作流参数
-    """
+    """Param - 工作流参数"""
 
     fields = {
         "Name": fields.Str(required=False, load_from="Name"),
         "Type": fields.Str(required=False, load_from="Type"),
         "Value": fields.Str(required=False, load_from="Value"),
     }
 
 
 class ActivityTemplateSchema(schema.ResponseSchema):
-    """ ActivityTemplate - 工作流的Activity定义
-    """
+    """ActivityTemplate - 工作流的Activity定义"""
 
     fields = {
         "Input": fields.Str(),
         "Name": fields.Str(required=False, load_from="Name"),
         "Next": fields.Str(required=False, load_from="Next"),
         "Output": fields.List(fields.Str()),
         "RetryTimes": fields.Str(required=False, load_from="RetryTimes"),
         "Timeout": fields.Str(required=False, load_from="Timeout"),
         "Type": fields.Str(required=False, load_from="Type"),
     }
 
 
 class WorkflowTemplateSchema(schema.ResponseSchema):
-    """ WorkflowTemplate - Workflow对象定义
-    """
+    """WorkflowTemplate - Workflow对象定义"""
 
     fields = {
         "Activites": fields.List(ActivityTemplateSchema()),
         "Input": fields.List(ParamSchema()),
         "Output": fields.List(ParamSchema()),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,24 @@
         super(UAccountClient, self).__init__(
             config, transport, middleware, logger
         )
 
     def create_project(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateProject - 创建项目
+        """CreateProject - 创建项目
 
         **Request**
 
         - **ProjectName** (str) - (Required) 项目名称
-        
+
         **Response**
 
         - **ProjectId** (str) - 所创建项目的Id
-        
+
         """
         # build request
         d = {}
         req and d.update(req)
         d = apis.CreateProjectRequestSchema().dumps(d)
 
         # build options
@@ -39,29 +39,29 @@
 
         resp = self.invoke("CreateProject", d, **kwargs)
         return apis.CreateProjectResponseSchema().loads(resp)
 
     def get_project_list(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetProjectList - 获取项目列表
+        """GetProjectList - 获取项目列表
 
         **Request**
 
         - **IsFinance** (str) - 是否是财务账号
-        
+
         **Response**
 
         - **ProjectCount** (int) - 项目总数
         - **ProjectSet** (list) - 见 **ProjectListInfo** 模型定义
-        
+
         **Response Model**
-        
-        **ProjectListInfo** 
-        
+
+        **ProjectListInfo**
+
         - **CreateTime** (int) - 创建时间(Unix时间戳)
         - **IsDefault** (bool) - 是否为默认项目
         - **MemberCount** (int) - 项目下成员数量
         - **ParentId** (str) - 父项目ID
         - **ParentName** (str) - 父项目名称
         - **ProjectId** (str) - 项目ID
         - **ProjectName** (str) - 项目名称
@@ -73,27 +73,27 @@
         req and d.update(req)
         d = apis.GetProjectListRequestSchema().dumps(d)
 
         resp = self.invoke("GetProjectList", d, **kwargs)
         return apis.GetProjectListResponseSchema().loads(resp)
 
     def get_region(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ GetRegion - 获取用户在各数据中心的权限等信息
+        """GetRegion - 获取用户在各数据中心的权限等信息
 
         **Request**
 
-        
+
         **Response**
 
         - **Regions** (list) - 见 **RegionInfo** 模型定义
-        
+
         **Response Model**
-        
-        **RegionInfo** 
-        
+
+        **RegionInfo**
+
         - **BitMaps** (str) - 用户在此数据中心的权限位
         - **IsDefault** (bool) - 是否用户当前默认数据中心
         - **Region** (str) - 地域名字，如cn-bj
         - **RegionId** (int) - 数据中心ID
         - **RegionName** (str) - 数据中心名称
         - **Zone** (str) - 可用区名字，如cn-bj-01
 
@@ -105,27 +105,27 @@
 
         resp = self.invoke("GetRegion", d, **kwargs)
         return apis.GetRegionResponseSchema().loads(resp)
 
     def get_user_info(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUserInfo - 获取用户信息
+        """GetUserInfo - 获取用户信息
 
         **Request**
 
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UserInfo** 模型定义
-        
+
         **Response Model**
-        
-        **UserInfo** 
-        
+
+        **UserInfo**
+
         - **Admin** (int) - 是否超级管理员 0:否 1:是
         - **Administrator** (str) - 管理员
         - **AuthState** (str) - 实名认证状态
         - **City** (str) - 城市
         - **CompanyName** (str) - 公司名称
         - **Finance** (int) - 是否有财务权限 0:否 1:是
         - **IndustryType** (int) - 所属行业
@@ -147,45 +147,45 @@
 
         resp = self.invoke("GetUserInfo", d, **kwargs)
         return apis.GetUserInfoResponseSchema().loads(resp)
 
     def modify_project(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyProject - 修改项目
+        """ModifyProject - 修改项目
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **ProjectName** (str) - (Required) 新的项目名称
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.ModifyProjectRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyProject", d, **kwargs)
         return apis.ModifyProjectResponseSchema().loads(resp)
 
     def terminate_project(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ TerminateProject - 删除项目
+        """TerminateProject - 删除项目
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.TerminateProjectRequestSchema().dumps(d)
 
         resp = self.invoke("TerminateProject", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/schemas/apis.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,44 +12,40 @@
 API: CreateProject
 
 创建项目
 """
 
 
 class CreateProjectRequestSchema(schema.RequestSchema):
-    """ CreateProject - 创建项目
-    """
+    """CreateProject - 创建项目"""
 
     fields = {"ProjectName": fields.Str(required=True, dump_to="ProjectName")}
 
 
 class CreateProjectResponseSchema(schema.ResponseSchema):
-    """ CreateProject - 创建项目
-    """
+    """CreateProject - 创建项目"""
 
     fields = {"ProjectId": fields.Str(required=True, load_from="ProjectId")}
 
 
 """
 API: GetProjectList
 
 获取项目列表
 """
 
 
 class GetProjectListRequestSchema(schema.RequestSchema):
-    """ GetProjectList - 获取项目列表
-    """
+    """GetProjectList - 获取项目列表"""
 
     fields = {"IsFinance": fields.Str(required=False, dump_to="IsFinance")}
 
 
 class GetProjectListResponseSchema(schema.ResponseSchema):
-    """ GetProjectList - 获取项目列表
-    """
+    """GetProjectList - 获取项目列表"""
 
     fields = {
         "ProjectCount": fields.Int(required=True, load_from="ProjectCount"),
         "ProjectSet": fields.List(
             models.ProjectListInfoSchema(),
             required=True,
             load_from="ProjectSet",
@@ -61,23 +57,21 @@
 API: GetRegion
 
 获取用户在各数据中心的权限等信息
 """
 
 
 class GetRegionRequestSchema(schema.RequestSchema):
-    """ GetRegion - 获取用户在各数据中心的权限等信息
-    """
+    """GetRegion - 获取用户在各数据中心的权限等信息"""
 
     fields = {}
 
 
 class GetRegionResponseSchema(schema.ResponseSchema):
-    """ GetRegion - 获取用户在各数据中心的权限等信息
-    """
+    """GetRegion - 获取用户在各数据中心的权限等信息"""
 
     fields = {
         "Regions": fields.List(
             models.RegionInfoSchema(), required=False, load_from="Regions"
         )
     }
 
@@ -86,23 +80,21 @@
 API: GetUserInfo
 
 获取用户信息
 """
 
 
 class GetUserInfoRequestSchema(schema.RequestSchema):
-    """ GetUserInfo - 获取用户信息
-    """
+    """GetUserInfo - 获取用户信息"""
 
     fields = {}
 
 
 class GetUserInfoResponseSchema(schema.ResponseSchema):
-    """ GetUserInfo - 获取用户信息
-    """
+    """GetUserInfo - 获取用户信息"""
 
     fields = {
         "DataSet": fields.List(
             models.UserInfoSchema(), required=True, load_from="DataSet"
         )
     }
 
@@ -111,42 +103,38 @@
 API: ModifyProject
 
 修改项目
 """
 
 
 class ModifyProjectRequestSchema(schema.RequestSchema):
-    """ ModifyProject - 修改项目
-    """
+    """ModifyProject - 修改项目"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "ProjectName": fields.Str(required=True, dump_to="ProjectName"),
     }
 
 
 class ModifyProjectResponseSchema(schema.ResponseSchema):
-    """ ModifyProject - 修改项目
-    """
+    """ModifyProject - 修改项目"""
 
     fields = {}
 
 
 """
 API: TerminateProject
 
 删除项目
 """
 
 
 class TerminateProjectRequestSchema(schema.RequestSchema):
-    """ TerminateProject - 删除项目
-    """
+    """TerminateProject - 删除项目"""
 
     fields = {"ProjectId": fields.Str(required=False, dump_to="ProjectId")}
 
 
 class TerminateProjectResponseSchema(schema.ResponseSchema):
-    """ TerminateProject - 删除项目
-    """
+    """TerminateProject - 删除项目"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uaccount/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uaccount/schemas/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class ProjectListInfoSchema(schema.ResponseSchema):
-    """ ProjectListInfo - 项目信息
-    """
+    """ProjectListInfo - 项目信息"""
 
     fields = {
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "IsDefault": fields.Bool(required=True, load_from="IsDefault"),
         "MemberCount": fields.Int(required=True, load_from="MemberCount"),
         "ParentId": fields.Str(required=True, load_from="ParentId"),
         "ParentName": fields.Str(required=True, load_from="ParentName"),
         "ProjectId": fields.Str(required=True, load_from="ProjectId"),
         "ProjectName": fields.Str(required=True, load_from="ProjectName"),
         "ResourceCount": fields.Int(required=True, load_from="ResourceCount"),
     }
 
 
 class RegionInfoSchema(schema.ResponseSchema):
-    """ RegionInfo - 数据中心信息
-    """
+    """RegionInfo - 数据中心信息"""
 
     fields = {
         "BitMaps": fields.Str(required=True, load_from="BitMaps"),
         "IsDefault": fields.Bool(required=True, load_from="IsDefault"),
         "Region": fields.Str(required=True, load_from="Region"),
         "RegionId": fields.Int(required=True, load_from="RegionId"),
         "RegionName": fields.Str(required=True, load_from="RegionName"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class UserInfoSchema(schema.ResponseSchema):
-    """ UserInfo - 用户信息
-    """
+    """UserInfo - 用户信息"""
 
     fields = {
         "Admin": fields.Int(required=True, load_from="Admin"),
         "Administrator": fields.Str(required=True, load_from="Administrator"),
         "AuthState": fields.Str(required=True, load_from="AuthState"),
         "City": fields.Str(required=True, load_from="City"),
         "CompanyName": fields.Str(required=True, load_from="CompanyName"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,53 +12,53 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UCDNClient, self).__init__(config, transport, middleware, logger)
 
     def batch_describe_new_ucdn_domain(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BatchDescribeNewUcdnDomain - 批量获取加速域名配置
+        """BatchDescribeNewUcdnDomain - 批量获取加速域名配置
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **ChannelType** (str) - 渠道ucdn、ufile、uvideo
         - **DomainId** (list) - 域名id，创建域名时生成的资源id，默认获取账号下的所有域名信息，n为自然数
         - **Limit** (int) - 返回数据长度，如果制定了Offset，则默认20，否则默认全部，非负整数
         - **Offset** (int) - 数据偏移量，默认0，非负整数
-        
+
         **Response**
 
         - **Arrearage** (list) - 标识欠费的数组，数组含有下列元素值， 1=国内流量有欠费 2=国外流量有欠费  3=国内带宽有欠费 4=国外带宽有欠费
         - **ChargeType** (int) - 当前计费方式，10=流量付费 20=带宽日峰值  30=按月后付费
         - **DomainSet** (list) - 见 **DomainInfo** 模型定义
         - **LastChargeType** (int) - 表示最后一次切换的计费方式，10=流量付费 20=带宽日峰值  30=按月后付费  40=未选择计费方式
         - **MaxDomainNum** (int) - 最大域名数量，默认20
         - **TotalCount** (int) - 满足条件的域名个数
         - **Vip** (str) - vip标示，yes-是  no-否
-        
+
         **Response Model**
-        
-        **CacheConf** 
-        
+
+        **CacheConf**
+
         - **CacheBehavior** (int) - 是否缓存，1为缓存，0为不缓存。为0的情况下，CacheTTL和CacheUnit强制不生效
         - **CacheTTL** (int) - 缓存时间
         - **CacheUnit** (str) - 缓存时间的单位。sec（秒），min（分钟），hour（小时），day（天）
         - **Description** (str) - 缓存规则描述
         - **FollowOriginRule** (int) - 是否优先遵循源站头部缓存策略，0为不优先遵循源站，1为优先遵循源站缓存头部。默认为0
         - **HttpCodePattern** (str) - 状态码默认情况只缓存200类状态码，支持正则
         - **IgnoreQueryString** (int) - 是否忽略参数缓存（0为不忽略，1为忽略，默认为0）
         - **PathPattern** (str) - 路径模式，支持正则
 
-        **AccessConf** 
-        
+        **AccessConf**
+
         - **IpBlacklist** (str) - 多个ip用逗号隔开
 
-        **DomainInfo** 
-        
+        **DomainInfo**
+
         - **AccessConf** (dict) - 见 **AccessConf** 模型定义
         - **AreaCode** (str) - 查询带宽区域 cn代表国内 abroad代表海外 不填默认为全部区域
         - **CacheConf** (list) - 见 **CacheConf** 模型定义
         - **CacheHost** (str) - 缓存Host，不同的域名可以配置为同一个CacheHost来实现缓存共享，默认为加速域名
         - **CdnProtocol** (str) - 加速类型http,http|https
         - **CdnType** (str) - 加速域名的业务类型，web代表网站，stream代表视频，download代表下载。
         - **CertName** (str) - 证书名称
@@ -89,43 +89,43 @@
 
         resp = self.invoke("BatchDescribeNewUcdnDomain", d, **kwargs)
         return apis.BatchDescribeNewUcdnDomainResponseSchema().loads(resp)
 
     def describe_new_ucdn_prefetch_cache_task(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeNewUcdnPrefetchCacheTask - 获取预取任务状态
+        """DescribeNewUcdnPrefetchCacheTask - 获取预取任务状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
         - **Limit** (int) - 返回数据长度,默认全部，自然数
         - **Offset** (int) - 数据偏移量，默认为0，自然数
         - **Status** (str) - 需要获取的内容预热的状态，枚举值：success：成功；wait：等待处理；process：正在处理；failure：失败； unknow：未知，默认选择所有状态
         - **TaskId** (list) - 提交任务时返回的任务ID
-        
+
         **Response**
 
         - **TaskList** (list) - 见 **TaskInfo** 模型定义
         - **TotalCount** (int) - 预热任务的总数
-        
+
         **Response Model**
-        
-        **UrlProgressInfo** 
-        
+
+        **UrlProgressInfo**
+
         - **CreateTime** (int) - 刷新任务创建的时间。格式为Unix Timestamp
         - **FinishTime** (int) - 任务完成时间。格式为Unix Timestamp
         - **Progress** (int) - 刷新进度，单位%
         - **Status** (str) - 刷新任务的当前状态，枚举值：success：成功；wait：排队中；process：处理中；failure：失败； unknow：未知
         - **Url** (str) - 刷新的单条url
 
-        **TaskInfo** 
-        
+        **TaskInfo**
+
         - **CreateTime** (int) - 刷新任务创建的时间。格式为Unix Timestamp
         - **Status** (str) - 刷新任务的当前状态，枚举值：success：成功；wait：排队中；process：处理中；failure：失败； unknow：未知
         - **TaskId** (str) - 提交任务时返回的任务ID
         - **Type** (str) - file/dir  刷新任务会返回Type，预取任务没有
         - **UrlLists** (list) - 见 **UrlProgressInfo** 模型定义
 
         """
@@ -136,43 +136,43 @@
 
         resp = self.invoke("DescribeNewUcdnPrefetchCacheTask", d, **kwargs)
         return apis.DescribeNewUcdnPrefetchCacheTaskResponseSchema().loads(resp)
 
     def describe_new_ucdn_refresh_cache_task(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeNewUcdnRefreshCacheTask - 获取域名刷新任务状态
+        """DescribeNewUcdnRefreshCacheTask - 获取域名刷新任务状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
         - **Limit** (int) - 返回数据长度,默认全部，自然数
         - **Offset** (int) - 数据偏移量，默认为0，自然数
         - **Status** (str) - 需要获取的内容刷新的状态，枚举值：success：成功；wait：等待处理；process：正在处理；failure：失败； unknow：未知，默认选择所有状态
         - **TaskId** (list) - 提交任务时返回的任务ID
-        
+
         **Response**
 
         - **TaskList** (list) - 见 **TaskInfo** 模型定义
         - **TotalCount** (int) - 刷新任务的总数
-        
+
         **Response Model**
-        
-        **UrlProgressInfo** 
-        
+
+        **UrlProgressInfo**
+
         - **CreateTime** (int) - 刷新任务创建的时间。格式为Unix Timestamp
         - **FinishTime** (int) - 任务完成时间。格式为Unix Timestamp
         - **Progress** (int) - 刷新进度，单位%
         - **Status** (str) - 刷新任务的当前状态，枚举值：success：成功；wait：排队中；process：处理中；failure：失败； unknow：未知
         - **Url** (str) - 刷新的单条url
 
-        **TaskInfo** 
-        
+        **TaskInfo**
+
         - **CreateTime** (int) - 刷新任务创建的时间。格式为Unix Timestamp
         - **Status** (str) - 刷新任务的当前状态，枚举值：success：成功；wait：排队中；process：处理中；failure：失败； unknow：未知
         - **TaskId** (str) - 提交任务时返回的任务ID
         - **Type** (str) - file/dir  刷新任务会返回Type，预取任务没有
         - **UrlLists** (list) - 见 **UrlProgressInfo** 模型定义
 
         """
@@ -183,34 +183,34 @@
 
         resp = self.invoke("DescribeNewUcdnRefreshCacheTask", d, **kwargs)
         return apis.DescribeNewUcdnRefreshCacheTaskResponseSchema().loads(resp)
 
     def get_new_ucdn_domain_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetNewUcdnDomainBandwidth - 获取域名带宽数据
+        """GetNewUcdnDomainBandwidth - 获取域名带宽数据
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Type** (int) - (Required) 时间粒度（0表示按照5分钟粒度，1表示按照1小时粒度，2表示按照一天的粒度）
         - **Areacode** (str) - 查询带宽区域 cn代表国内 abroad代表海外 不填默认为全部区域
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值。如没有赋值，则返回缺少参 数错误，如果没有EndTime，BeginTime也可以不赋值，EndTime默认当前时间，BeginTime 默认前一天的当前时间。
         - **DomainId** (list) - 域名id，创建域名时生成的id。默认全部域名
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
-        
+
         **Response**
 
         - **BandwidthList** (list) - 见 **BandwidthInfo** 模型定义
         - **Traffic** (str) - 从起始时间到结束时间内的所使用的CDN总流量，单位GB
-        
+
         **Response Model**
-        
-        **BandwidthInfo** 
-        
+
+        **BandwidthInfo**
+
         - **CdnBandwidth** (str) - 返回值返回指定时间区间内CDN的带宽峰值，单位Mbps（如果请求参数Type为0，则Value是五分钟粒度的带宽值，如果Type为1，则Value是1小时的带宽峰值，如果Type为2，则Value是一天内的带宽峰值）
         - **Time** (int) - 带宽获取的时间点。格式：时间戳
 
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
@@ -218,33 +218,33 @@
 
         resp = self.invoke("GetNewUcdnDomainBandwidth", d, **kwargs)
         return apis.GetNewUcdnDomainBandwidthResponseSchema().loads(resp)
 
     def get_new_ucdn_domain_hit_rate(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetNewUcdnDomainHitRate - 获取域名命中率
+        """GetNewUcdnDomainHitRate - 获取域名命中率
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Type** (int) - (Required) 时间粒度（0表示按照5分钟粒度，1表示按照1小时粒度，2表示按照一天的粒度）
         - **Areacode** (str) - 查询带宽区域 cn代表国内 abroad代表海外，只支持国内
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值。如没有赋值，则返回缺少参 数错误，如果没有EndTime，BeginTime也可以不赋值，EndTime默认当前时间，BeginTime 默认前一天的当前时间。
         - **DomainId** (list) - 域名id，创建域名时生成的id。默认全部域名
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
-        
+
         **Response**
 
         - **HitRateList** (list) - 见 **HitRateInfo** 模型定义
-        
+
         **Response Model**
-        
-        **HitRateInfo** 
-        
+
+        **HitRateInfo**
+
         - **FlowHitRate** (float) - 流量命中率，单位%
         - **RequestHitRate** (float) - 请求数命中率，单位%
         - **Time** (int) - 带宽获取的时间点。格式：时间戳
 
         """
         # build request
         d = {"ProjectId": self.config.project_id}
@@ -253,33 +253,33 @@
 
         resp = self.invoke("GetNewUcdnDomainHitRate", d, **kwargs)
         return apis.GetNewUcdnDomainHitRateResponseSchema().loads(resp)
 
     def get_new_ucdn_domain_http_code(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetNewUcdnDomainHttpCode - 获取域名状态码监控
+        """GetNewUcdnDomainHttpCode - 获取域名状态码监控
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Type** (int) - (Required) 时间粒度（0表示按照5分钟粒度，1表示按照1小时粒度，2表示按照一天的粒度）
         - **Areacode** (str) - 查询带宽区域 cn代表国内 abroad代表海外，只支持国内
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值。如没有赋值，则返回缺少参 数错误，如果没有EndTime，BeginTime也可以不赋值，EndTime默认当前时间，BeginTime 默认前一天的当前时间。
         - **DomainId** (list) - 域名id，创建域名时生成的id。默认全部域名
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
-        
+
         **Response**
 
         - **HttpCodeDetail** (list) - 见 **HttpCodeInfo** 模型定义
-        
+
         **Response Model**
-        
-        **HttpCodeInfo** 
-        
+
+        **HttpCodeInfo**
+
         - **HttpFiveXX** (int) - 5xx数量
         - **HttpFourXX** (int) - 4xx数量
         - **HttpOneXX** (int) - 1xx数量
         - **HttpThreeXX** (int) - 3xx数量
         - **HttpTwoXX** (int) - 2xx数量
         - **Time** (int) - 带宽获取的时间点。格式：时间戳
 
@@ -291,33 +291,33 @@
 
         resp = self.invoke("GetNewUcdnDomainHttpCode", d, **kwargs)
         return apis.GetNewUcdnDomainHttpCodeResponseSchema().loads(resp)
 
     def get_new_ucdn_domain_http_code_v2(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetNewUcdnDomainHttpCodeV2 - 获取域名详细状态码监控
+        """GetNewUcdnDomainHttpCodeV2 - 获取域名详细状态码监控
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **BeginTime** (int) - (Required) 查询的起始时间，格式为Unix Timestamp。
         - **EndTime** (int) - (Required) 查询的结束时间，格式为Unix Timestamp。
         - **Type** (int) - (Required) 时间粒度（0表示按照5分钟粒度，1表示按照1小时粒度，2表示按照一天粒度，3表示按照一分钟粒度）
         - **Areacode** (str) - 查询带宽区域 cn代表国内 abroad代表海外，只支持国内
         - **DomainId** (list) - 域名id，创建域名时生成的id。默认全部域名
-        
+
         **Response**
 
         - **HttpCodeV2Detail** (list) - 见 **HttpCodeV2Detail** 模型定义
-        
+
         **Response Model**
-        
-        **HttpCodeV2Detail** 
-        
+
+        **HttpCodeV2Detail**
+
         - **Http100** (int) - http100数量
         - **Http101** (int) - http101数量
         - **Http102** (int) - http102数量
         - **Http200** (int) - http200数量
         - **Http201** (int) - http201数量
         - **Http202** (int) - http202数量
         - **Http203** (int) - http203数量
@@ -380,33 +380,33 @@
 
         resp = self.invoke("GetNewUcdnDomainHttpCodeV2", d, **kwargs)
         return apis.GetNewUcdnDomainHttpCodeV2ResponseSchema().loads(resp)
 
     def get_new_ucdn_domain_request_num(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetNewUcdnDomainRequestNum - 获取域名请求数
+        """GetNewUcdnDomainRequestNum - 获取域名请求数
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Type** (int) - (Required) 时间粒度（0表示按照5分钟粒度，1表示按照1小时粒度，2表示按照一天的粒度）
         - **Areacode** (str) - 查询区域 cn代表国内 abroad代表海外，只支持国内
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值。如没有赋值，则返回缺少参 数错误，如果没有EndTime，BeginTime也可以不赋值，EndTime默认当前时间，BeginTime 默认前一天的当前时间。
         - **DomainId** (list) - 域名id，创建域名时生成的id。默认全部域名
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
-        
+
         **Response**
 
         - **RequestList** (list) - 见 **RequestInfo** 模型定义
-        
+
         **Response Model**
-        
-        **RequestInfo** 
-        
+
+        **RequestInfo**
+
         - **CdnRequest** (float) - 返回值返回指定时间区间内的cdn收到的请求次数之和
         - **OriginRequest** (float) - 返回值返回指定时间区间内的cdn回源的请求次数之和
         - **Time** (int) - 带宽获取的时间点。格式：时间戳
 
         """
         # build request
         d = {"ProjectId": self.config.project_id}
@@ -415,38 +415,38 @@
 
         resp = self.invoke("GetNewUcdnDomainRequestNum", d, **kwargs)
         return apis.GetNewUcdnDomainRequestNumResponseSchema().loads(resp)
 
     def get_ucdn_domain_log(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUcdnDomainLog - 获取加速域名原始日志
+        """GetUcdnDomainLog - 获取加速域名原始日志
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值。
         - **DomainId** (list) - 域名ID，创建加速域名时生成。默认全部域名
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
         - **Type** (int) - 查询粒度  0=default(没有粒度) 1=按小时  2=按天
-        
+
         **Response**
 
         - **LogSet** (list) - 见 **LogSetList** 模型定义
-        
+
         **Response Model**
-        
-        **LogSetInfo** 
-        
+
+        **LogSetInfo**
+
         - **AbroadLog** (list) - 国外日志url列表
         - **CnLog** (list) - 国内日志url列表
         - **Time** (int) - 日志时间UnixTime
 
-        **LogSetList** 
-        
+        **LogSetList**
+
         - **Domain** (str) - 域名
         - **Logs** (list) - 见 **LogSetInfo** 模型定义
 
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
@@ -454,56 +454,56 @@
 
         resp = self.invoke("GetUcdnDomainLog", d, **kwargs)
         return apis.GetUcdnDomainLogResponseSchema().loads(resp)
 
     def get_ucdn_domain_prefetch_enable(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUcdnDomainPrefetchEnable - 获取域名预取开启状态
+        """GetUcdnDomainPrefetchEnable - 获取域名预取开启状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **DomainId** (str) - (Required) 域名ID，创建加速域名时生成。
-        
+
         **Response**
 
         - **Enable** (int) - 0表示该域名未开启预取，1表示该域名已开启预取
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.GetUcdnDomainPrefetchEnableRequestSchema().dumps(d)
 
         resp = self.invoke("GetUcdnDomainPrefetchEnable", d, **kwargs)
         return apis.GetUcdnDomainPrefetchEnableResponseSchema().loads(resp)
 
     def get_ucdn_domain_request_num_v2(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUcdnDomainRequestNumV2 - 获取域名请求数
+        """GetUcdnDomainRequestNumV2 - 获取域名请求数
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **BeginTime** (int) - (Required) 查询的起始时间，格式为Unix Timestamp
         - **EndTime** (int) - (Required) 查询的结束时间，格式为Unix Timestamp
         - **Type** (int) - (Required) 时间粒度（0表示按照5分钟粒度，1表示按照1小时粒度，2表示按照一天的粒度, 3=按1分钟）
         - **Areacode** (str) - 查询区域 cn代表国内 abroad代表海外，只支持国内
         - **DomainId** (list) - 域名id，创建域名时生成的id。默认全部域名
-        
+
         **Response**
 
         - **RequestList** (list) - 见 **RequestInfo** 模型定义
-        
+
         **Response Model**
-        
-        **RequestInfo** 
-        
+
+        **RequestInfo**
+
         - **CdnRequest** (float) - 返回值返回指定时间区间内的cdn收到的请求次数之和
         - **OriginRequest** (float) - 返回值返回指定时间区间内的cdn回源的请求次数之和
         - **Time** (int) - 带宽获取的时间点。格式：时间戳
 
         """
         # build request
         d = {"ProjectId": self.config.project_id}
@@ -512,32 +512,32 @@
 
         resp = self.invoke("GetUcdnDomainRequestNumV2", d, **kwargs)
         return apis.GetUcdnDomainRequestNumV2ResponseSchema().loads(resp)
 
     def get_ucdn_domain_traffic(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUcdnDomainTraffic - 获取加速域名流量使用信息
+        """GetUcdnDomainTraffic - 获取加速域名流量使用信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Areacode** (str) - 查询流量区域 cn代表国内 abroad代表海外，默认全部区域。
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值。
         - **DomainId** (list) - 域名ID，创建加速域名时生成。默认全部域名
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
-        
+
         **Response**
 
         - **TrafficSet** (list) - 见 **UcdnDomainTrafficSet** 模型定义
-        
+
         **Response Model**
-        
-        **UcdnDomainTrafficSet** 
-        
+
+        **UcdnDomainTrafficSet**
+
         - **Time** (int) - 流量获取的时间点，格式为Unix Timestamp
         - **Value** (float) - 查询每日流量总值，单位：GB
 
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
@@ -545,33 +545,33 @@
 
         resp = self.invoke("GetUcdnDomainTraffic", d, **kwargs)
         return apis.GetUcdnDomainTrafficResponseSchema().loads(resp)
 
     def get_ucdn_pass_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUcdnPassBandwidth - 获取回源带宽数据（cdn回客户源站部分）
+        """GetUcdnPassBandwidth - 获取回源带宽数据（cdn回客户源站部分）
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Type** (int) - (Required) 时间粒度（0表示按照5分钟粒度，1表示按照1小时粒度，2表示按照一天的粒度）
         - **Areacode** (str) - 查询带宽区域 cn代表国内 abroad代表海外，只支持国内
         - **BeginTime** (int) - 查询的起始时间，格式为Unix Timestamp。如果有EndTime，BeginTime必须赋值。如没有赋值，则返回缺少参 数错误，如果没有EndTime，BeginTime也可以不赋值，EndTime默认当前时间，BeginTime 默认前一天的当前时间。
         - **DomainId** (list) - 域名id，创建域名时生成的id。默认全部域名
         - **EndTime** (int) - 查询的结束时间，格式为Unix Timestamp。EndTime默认为当前时间，BeginTime默认为当前时间前一天时间。
-        
+
         **Response**
 
         - **BandwidthDetail** (list) - 见 **BandwidthInfoDetail** 模型定义
-        
+
         **Response Model**
-        
-        **BandwidthInfoDetail** 
-        
+
+        **BandwidthInfoDetail**
+
         - **Bandwidth** (float) - 返回值带宽值数据。
         - **Time** (int) - 宽获取的时间点。格式：时间戳
 
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
@@ -579,28 +579,28 @@
 
         resp = self.invoke("GetUcdnPassBandwidth", d, **kwargs)
         return apis.GetUcdnPassBandwidthResponseSchema().loads(resp)
 
     def get_ucdn_traffic(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUcdnTraffic - 获取流量信息
+        """GetUcdnTraffic - 获取流量信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+
         **Response**
 
         - **TrafficSet** (list) - 见 **TrafficSet** 模型定义
-        
+
         **Response Model**
-        
-        **TrafficSet** 
-        
+
+        **TrafficSet**
+
         - **Areacode** (str) - 购买流量的区域, cn: 国内; abroad: 国外
         - **TrafficLeft** (str) - Areacode区域内总剩余流量, 单位GB
         - **TrafficTotal** (str) - Areacode区域内总购买流量, 单位GB
         - **TrafficUsed** (str) - Areacode区域内总使用流量, 单位GB
 
         """
         # build request
@@ -610,71 +610,71 @@
 
         resp = self.invoke("GetUcdnTraffic", d, **kwargs)
         return apis.GetUcdnTrafficResponseSchema().loads(resp)
 
     def prefetch_new_ucdn_domain_cache(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ PrefetchNewUcdnDomainCache - 提交预取任务
+        """PrefetchNewUcdnDomainCache - 提交预取任务
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **UrlList** (list) - (Required) 预热URL列表，n从自然数0开始。UrlList.n字段必须以”http://域名/”开始。目录要以”/”结尾， 如刷新目录a下所有文件，格式为：http://abc.ucloud.cn/a/；如刷新文件目录a下面img.png文件， 格式为http://abc.ucloud.cn/a/img.png。请正确提交需要刷新的域名
-        
+
         **Response**
 
         - **TaskId** (str) - 本次提交url对应的任务id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.PrefetchNewUcdnDomainCacheRequestSchema().dumps(d)
 
         resp = self.invoke("PrefetchNewUcdnDomainCache", d, **kwargs)
         return apis.PrefetchNewUcdnDomainCacheResponseSchema().loads(resp)
 
     def refresh_new_ucdn_domain_cache(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RefreshNewUcdnDomainCache - 刷新缓存
+        """RefreshNewUcdnDomainCache - 刷新缓存
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Type** (str) - (Required) 刷新类型，file代表文件刷新，dir 代表路径刷新
         - **UrlList** (list) - (Required) 刷新多个URL列表时，一次最多提交30个。必须以”http://域名/”开始。目录要以”/”结尾， 如刷新目录a下所有文件，格式为：http://abc.ucloud.cn/a/；如刷新文件目录a下面img.png文件， 格式为http://abc.ucloud.cn/a/img.png。请正确提交需要刷新的域名
-        
+
         **Response**
 
         - **TaskId** (str) - 本次提交url对应的任务id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.RefreshNewUcdnDomainCacheRequestSchema().dumps(d)
 
         resp = self.invoke("RefreshNewUcdnDomainCache", d, **kwargs)
         return apis.RefreshNewUcdnDomainCacheResponseSchema().loads(resp)
 
     def switch_ucdn_charge_type(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ SwitchUcdnChargeType - 切换账号计费方式
+        """SwitchUcdnChargeType - 切换账号计费方式
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **ChargeType** (str) - (Required) 计费方式。traffic代表按流量包计费，bandwidth按带宽付费
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.SwitchUcdnChargeTypeRequestSchema().dumps(d)
 
         resp = self.invoke("SwitchUcdnChargeType", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/schemas/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 API: BatchDescribeNewUcdnDomain
 
 批量获取加速域名配置
 """
 
 
 class BatchDescribeNewUcdnDomainRequestSchema(schema.RequestSchema):
-    """ BatchDescribeNewUcdnDomain - 批量获取加速域名配置
-    """
+    """BatchDescribeNewUcdnDomain - 批量获取加速域名配置"""
 
     fields = {
         "ChannelType": fields.Str(required=False, dump_to="ChannelType"),
         "DomainId": fields.List(fields.Str()),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
     }
 
 
 class BatchDescribeNewUcdnDomainResponseSchema(schema.ResponseSchema):
-    """ BatchDescribeNewUcdnDomain - 批量获取加速域名配置
-    """
+    """BatchDescribeNewUcdnDomain - 批量获取加速域名配置"""
 
     fields = {
         "Arrearage": fields.List(
             fields.Str(), required=False, load_from="Arrearage"
         ),
         "ChargeType": fields.Int(required=False, load_from="ChargeType"),
         "DomainSet": fields.List(
@@ -53,31 +51,29 @@
 API: DescribeNewUcdnPrefetchCacheTask
 
 获取预取任务状态
 """
 
 
 class DescribeNewUcdnPrefetchCacheTaskRequestSchema(schema.RequestSchema):
-    """ DescribeNewUcdnPrefetchCacheTask - 获取预取任务状态
-    """
+    """DescribeNewUcdnPrefetchCacheTask - 获取预取任务状态"""
 
     fields = {
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Status": fields.Str(required=False, dump_to="Status"),
         "TaskId": fields.List(fields.Str()),
     }
 
 
 class DescribeNewUcdnPrefetchCacheTaskResponseSchema(schema.ResponseSchema):
-    """ DescribeNewUcdnPrefetchCacheTask - 获取预取任务状态
-    """
+    """DescribeNewUcdnPrefetchCacheTask - 获取预取任务状态"""
 
     fields = {
         "TaskList": fields.List(
             models.TaskInfoSchema(), required=False, load_from="TaskList"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -87,31 +83,29 @@
 API: DescribeNewUcdnRefreshCacheTask
 
 获取域名刷新任务状态
 """
 
 
 class DescribeNewUcdnRefreshCacheTaskRequestSchema(schema.RequestSchema):
-    """ DescribeNewUcdnRefreshCacheTask - 获取域名刷新任务状态
-    """
+    """DescribeNewUcdnRefreshCacheTask - 获取域名刷新任务状态"""
 
     fields = {
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Status": fields.Str(required=False, dump_to="Status"),
         "TaskId": fields.List(fields.Str()),
     }
 
 
 class DescribeNewUcdnRefreshCacheTaskResponseSchema(schema.ResponseSchema):
-    """ DescribeNewUcdnRefreshCacheTask - 获取域名刷新任务状态
-    """
+    """DescribeNewUcdnRefreshCacheTask - 获取域名刷新任务状态"""
 
     fields = {
         "TaskList": fields.List(
             models.TaskInfoSchema(), required=False, load_from="TaskList"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -121,30 +115,28 @@
 API: GetNewUcdnDomainBandwidth
 
 获取域名带宽数据
 """
 
 
 class GetNewUcdnDomainBandwidthRequestSchema(schema.RequestSchema):
-    """ GetNewUcdnDomainBandwidth - 获取域名带宽数据
-    """
+    """GetNewUcdnDomainBandwidth - 获取域名带宽数据"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=True, dump_to="Type"),
     }
 
 
 class GetNewUcdnDomainBandwidthResponseSchema(schema.ResponseSchema):
-    """ GetNewUcdnDomainBandwidth - 获取域名带宽数据
-    """
+    """GetNewUcdnDomainBandwidth - 获取域名带宽数据"""
 
     fields = {
         "BandwidthList": fields.List(
             models.BandwidthInfoSchema(),
             required=False,
             load_from="BandwidthList",
         ),
@@ -156,30 +148,28 @@
 API: GetNewUcdnDomainHitRate
 
 获取域名命中率
 """
 
 
 class GetNewUcdnDomainHitRateRequestSchema(schema.RequestSchema):
-    """ GetNewUcdnDomainHitRate - 获取域名命中率
-    """
+    """GetNewUcdnDomainHitRate - 获取域名命中率"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=True, dump_to="Type"),
     }
 
 
 class GetNewUcdnDomainHitRateResponseSchema(schema.ResponseSchema):
-    """ GetNewUcdnDomainHitRate - 获取域名命中率
-    """
+    """GetNewUcdnDomainHitRate - 获取域名命中率"""
 
     fields = {
         "HitRateList": fields.List(
             models.HitRateInfoSchema(), required=False, load_from="HitRateList"
         )
     }
 
@@ -188,30 +178,28 @@
 API: GetNewUcdnDomainHttpCode
 
 获取域名状态码监控
 """
 
 
 class GetNewUcdnDomainHttpCodeRequestSchema(schema.RequestSchema):
-    """ GetNewUcdnDomainHttpCode - 获取域名状态码监控
-    """
+    """GetNewUcdnDomainHttpCode - 获取域名状态码监控"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=True, dump_to="Type"),
     }
 
 
 class GetNewUcdnDomainHttpCodeResponseSchema(schema.ResponseSchema):
-    """ GetNewUcdnDomainHttpCode - 获取域名状态码监控
-    """
+    """GetNewUcdnDomainHttpCode - 获取域名状态码监控"""
 
     fields = {
         "HttpCodeDetail": fields.List(
             models.HttpCodeInfoSchema(),
             required=False,
             load_from="HttpCodeDetail",
         )
@@ -222,30 +210,28 @@
 API: GetNewUcdnDomainHttpCodeV2
 
 获取域名详细状态码监控
 """
 
 
 class GetNewUcdnDomainHttpCodeV2RequestSchema(schema.RequestSchema):
-    """ GetNewUcdnDomainHttpCodeV2 - 获取域名详细状态码监控
-    """
+    """GetNewUcdnDomainHttpCodeV2 - 获取域名详细状态码监控"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=True, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=True, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=True, dump_to="Type"),
     }
 
 
 class GetNewUcdnDomainHttpCodeV2ResponseSchema(schema.ResponseSchema):
-    """ GetNewUcdnDomainHttpCodeV2 - 获取域名详细状态码监控
-    """
+    """GetNewUcdnDomainHttpCodeV2 - 获取域名详细状态码监控"""
 
     fields = {
         "HttpCodeV2Detail": fields.List(
             models.HttpCodeV2DetailSchema(),
             required=False,
             load_from="HttpCodeV2Detail",
         )
@@ -256,30 +242,28 @@
 API: GetNewUcdnDomainRequestNum
 
 获取域名请求数
 """
 
 
 class GetNewUcdnDomainRequestNumRequestSchema(schema.RequestSchema):
-    """ GetNewUcdnDomainRequestNum - 获取域名请求数
-    """
+    """GetNewUcdnDomainRequestNum - 获取域名请求数"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=True, dump_to="Type"),
     }
 
 
 class GetNewUcdnDomainRequestNumResponseSchema(schema.ResponseSchema):
-    """ GetNewUcdnDomainRequestNum - 获取域名请求数
-    """
+    """GetNewUcdnDomainRequestNum - 获取域名请求数"""
 
     fields = {
         "RequestList": fields.List(
             models.RequestInfoSchema(), required=False, load_from="RequestList"
         )
     }
 
@@ -288,29 +272,27 @@
 API: GetUcdnDomainLog
 
 获取加速域名原始日志
 """
 
 
 class GetUcdnDomainLogRequestSchema(schema.RequestSchema):
-    """ GetUcdnDomainLog - 获取加速域名原始日志
-    """
+    """GetUcdnDomainLog - 获取加速域名原始日志"""
 
     fields = {
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=False, dump_to="Type"),
     }
 
 
 class GetUcdnDomainLogResponseSchema(schema.ResponseSchema):
-    """ GetUcdnDomainLog - 获取加速域名原始日志
-    """
+    """GetUcdnDomainLog - 获取加速域名原始日志"""
 
     fields = {
         "LogSet": fields.List(
             models.LogSetListSchema(), required=False, load_from="LogSet"
         )
     }
 
@@ -319,54 +301,50 @@
 API: GetUcdnDomainPrefetchEnable
 
 获取域名预取开启状态
 """
 
 
 class GetUcdnDomainPrefetchEnableRequestSchema(schema.RequestSchema):
-    """ GetUcdnDomainPrefetchEnable - 获取域名预取开启状态
-    """
+    """GetUcdnDomainPrefetchEnable - 获取域名预取开启状态"""
 
     fields = {
         "DomainId": fields.Str(required=True, dump_to="DomainId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
     }
 
 
 class GetUcdnDomainPrefetchEnableResponseSchema(schema.ResponseSchema):
-    """ GetUcdnDomainPrefetchEnable - 获取域名预取开启状态
-    """
+    """GetUcdnDomainPrefetchEnable - 获取域名预取开启状态"""
 
     fields = {"Enable": fields.Int(required=False, load_from="Enable")}
 
 
 """
 API: GetUcdnDomainRequestNumV2
 
 获取域名请求数
 """
 
 
 class GetUcdnDomainRequestNumV2RequestSchema(schema.RequestSchema):
-    """ GetUcdnDomainRequestNumV2 - 获取域名请求数
-    """
+    """GetUcdnDomainRequestNumV2 - 获取域名请求数"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=True, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=True, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=True, dump_to="Type"),
     }
 
 
 class GetUcdnDomainRequestNumV2ResponseSchema(schema.ResponseSchema):
-    """ GetUcdnDomainRequestNumV2 - 获取域名请求数
-    """
+    """GetUcdnDomainRequestNumV2 - 获取域名请求数"""
 
     fields = {
         "RequestList": fields.List(
             models.RequestInfoSchema(), required=False, load_from="RequestList"
         )
     }
 
@@ -375,29 +353,27 @@
 API: GetUcdnDomainTraffic
 
 获取加速域名流量使用信息
 """
 
 
 class GetUcdnDomainTrafficRequestSchema(schema.RequestSchema):
-    """ GetUcdnDomainTraffic - 获取加速域名流量使用信息
-    """
+    """GetUcdnDomainTraffic - 获取加速域名流量使用信息"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
     }
 
 
 class GetUcdnDomainTrafficResponseSchema(schema.ResponseSchema):
-    """ GetUcdnDomainTraffic - 获取加速域名流量使用信息
-    """
+    """GetUcdnDomainTraffic - 获取加速域名流量使用信息"""
 
     fields = {
         "TrafficSet": fields.List(
             models.UcdnDomainTrafficSetSchema(),
             required=False,
             load_from="TrafficSet",
         )
@@ -408,30 +384,28 @@
 API: GetUcdnPassBandwidth
 
 获取回源带宽数据（cdn回客户源站部分）
 """
 
 
 class GetUcdnPassBandwidthRequestSchema(schema.RequestSchema):
-    """ GetUcdnPassBandwidth - 获取回源带宽数据（cdn回客户源站部分）
-    """
+    """GetUcdnPassBandwidth - 获取回源带宽数据（cdn回客户源站部分）"""
 
     fields = {
         "Areacode": fields.Str(required=False, dump_to="Areacode"),
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DomainId": fields.List(fields.Str()),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Int(required=True, dump_to="Type"),
     }
 
 
 class GetUcdnPassBandwidthResponseSchema(schema.ResponseSchema):
-    """ GetUcdnPassBandwidth - 获取回源带宽数据（cdn回客户源站部分）
-    """
+    """GetUcdnPassBandwidth - 获取回源带宽数据（cdn回客户源站部分）"""
 
     fields = {
         "BandwidthDetail": fields.List(
             models.BandwidthInfoDetailSchema(),
             required=False,
             load_from="BandwidthDetail",
         )
@@ -442,23 +416,21 @@
 API: GetUcdnTraffic
 
 获取流量信息
 """
 
 
 class GetUcdnTrafficRequestSchema(schema.RequestSchema):
-    """ GetUcdnTraffic - 获取流量信息
-    """
+    """GetUcdnTraffic - 获取流量信息"""
 
     fields = {"ProjectId": fields.Str(required=False, dump_to="ProjectId")}
 
 
 class GetUcdnTrafficResponseSchema(schema.ResponseSchema):
-    """ GetUcdnTraffic - 获取流量信息
-    """
+    """GetUcdnTraffic - 获取流量信息"""
 
     fields = {
         "TrafficSet": fields.List(
             models.TrafficSetSchema(), required=False, load_from="TrafficSet"
         )
     }
 
@@ -467,70 +439,64 @@
 API: PrefetchNewUcdnDomainCache
 
 提交预取任务
 """
 
 
 class PrefetchNewUcdnDomainCacheRequestSchema(schema.RequestSchema):
-    """ PrefetchNewUcdnDomainCache - 提交预取任务
-    """
+    """PrefetchNewUcdnDomainCache - 提交预取任务"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "UrlList": fields.List(fields.Str()),
     }
 
 
 class PrefetchNewUcdnDomainCacheResponseSchema(schema.ResponseSchema):
-    """ PrefetchNewUcdnDomainCache - 提交预取任务
-    """
+    """PrefetchNewUcdnDomainCache - 提交预取任务"""
 
     fields = {"TaskId": fields.Str(required=False, load_from="TaskId")}
 
 
 """
 API: RefreshNewUcdnDomainCache
 
 刷新缓存
 """
 
 
 class RefreshNewUcdnDomainCacheRequestSchema(schema.RequestSchema):
-    """ RefreshNewUcdnDomainCache - 刷新缓存
-    """
+    """RefreshNewUcdnDomainCache - 刷新缓存"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Str(required=True, dump_to="Type"),
         "UrlList": fields.List(fields.Str()),
     }
 
 
 class RefreshNewUcdnDomainCacheResponseSchema(schema.ResponseSchema):
-    """ RefreshNewUcdnDomainCache - 刷新缓存
-    """
+    """RefreshNewUcdnDomainCache - 刷新缓存"""
 
     fields = {"TaskId": fields.Str(required=False, load_from="TaskId")}
 
 
 """
 API: SwitchUcdnChargeType
 
 切换账号计费方式
 """
 
 
 class SwitchUcdnChargeTypeRequestSchema(schema.RequestSchema):
-    """ SwitchUcdnChargeType - 切换账号计费方式
-    """
+    """SwitchUcdnChargeType - 切换账号计费方式"""
 
     fields = {
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
     }
 
 
 class SwitchUcdnChargeTypeResponseSchema(schema.ResponseSchema):
-    """ SwitchUcdnChargeType - 切换账号计费方式
-    """
+    """SwitchUcdnChargeType - 切换账号计费方式"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ucdn/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ucdn/schemas/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class CacheConfSchema(schema.ResponseSchema):
-    """ CacheConf - 缓存配置
-    """
+    """CacheConf - 缓存配置"""
 
     fields = {
         "CacheBehavior": fields.Int(required=False, load_from="CacheBehavior"),
         "CacheTTL": fields.Int(required=False, load_from="CacheTTL"),
         "CacheUnit": fields.Str(required=False, load_from="CacheUnit"),
         "Description": fields.Str(required=False, load_from="Description"),
         "FollowOriginRule": fields.Int(
@@ -22,25 +21,23 @@
             required=False, load_from="IgnoreQueryString"
         ),
         "PathPattern": fields.Str(required=False, load_from="PathPattern"),
     }
 
 
 class AccessConfSchema(schema.ResponseSchema):
-    """ AccessConf - 访问控制
-    """
+    """AccessConf - 访问控制"""
 
     fields = {
         "IpBlacklist": fields.Str(required=False, load_from="IpBlacklist")
     }
 
 
 class DomainInfoSchema(schema.ResponseSchema):
-    """ DomainInfo - 域名配置
-    """
+    """DomainInfo - 域名配置"""
 
     fields = {
         "AccessConf": AccessConfSchema(),
         "AreaCode": fields.Str(required=False, load_from="AreaCode"),
         "CacheConf": fields.List(CacheConfSchema()),
         "CacheHost": fields.Str(required=False, load_from="CacheHost"),
         "CdnProtocol": fields.Str(required=False, load_from="CdnProtocol"),
@@ -68,79 +65,73 @@
         "Tag": fields.Str(required=False, load_from="Tag"),
         "TestUrl": fields.Str(required=True, load_from="TestUrl"),
         "ValidTime": fields.Int(required=False, load_from="ValidTime"),
     }
 
 
 class UrlProgressInfoSchema(schema.ResponseSchema):
-    """ UrlProgressInfo - UrlProgressInfo
-    """
+    """UrlProgressInfo - UrlProgressInfo"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "FinishTime": fields.Int(required=False, load_from="FinishTime"),
         "Progress": fields.Int(required=False, load_from="Progress"),
         "Status": fields.Str(required=False, load_from="Status"),
         "Url": fields.Str(required=False, load_from="Url"),
     }
 
 
 class TaskInfoSchema(schema.ResponseSchema):
-    """ TaskInfo - 预取刷新的任务信息
-    """
+    """TaskInfo - 预取刷新的任务信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Status": fields.Str(required=False, load_from="Status"),
         "TaskId": fields.Str(required=False, load_from="TaskId"),
         "Type": fields.Str(required=False, load_from="Type"),
         "UrlLists": fields.List(UrlProgressInfoSchema()),
     }
 
 
 class BandwidthInfoSchema(schema.ResponseSchema):
-    """ BandwidthInfo - BandwidthInfo
-    """
+    """BandwidthInfo - BandwidthInfo"""
 
     fields = {
         "CdnBandwidth": fields.Str(required=False, load_from="CdnBandwidth"),
         "Time": fields.Int(required=False, load_from="Time"),
     }
 
 
 class HitRateInfoSchema(schema.ResponseSchema):
-    """ HitRateInfo - HitRateInfo
-    """
+    """HitRateInfo - HitRateInfo"""
 
     fields = {
         "FlowHitRate": fields.Float(required=False, load_from="FlowHitRate"),
         "RequestHitRate": fields.Float(
             required=False, load_from="RequestHitRate"
         ),
         "Time": fields.Int(required=False, load_from="Time"),
     }
 
 
 class HttpCodeInfoSchema(schema.ResponseSchema):
-    """ HttpCodeInfo - HttpCodeInfo
-    """
+    """HttpCodeInfo - HttpCodeInfo"""
 
     fields = {
         "HttpFiveXX": fields.Int(required=False, load_from="HttpFiveXX"),
         "HttpFourXX": fields.Int(required=False, load_from="HttpFourXX"),
         "HttpOneXX": fields.Int(required=False, load_from="HttpOneXX"),
         "HttpThreeXX": fields.Int(required=False, load_from="HttpThreeXX"),
         "HttpTwoXX": fields.Int(required=False, load_from="HttpTwoXX"),
         "Time": fields.Int(required=False, load_from="Time"),
     }
 
 
 class HttpCodeV2DetailSchema(schema.ResponseSchema):
-    """ HttpCodeV2Detail - HTTP状态码详细信息
-    """
+    """HttpCodeV2Detail - HTTP状态码详细信息"""
 
     fields = {
         "Http100": fields.Int(required=False, load_from="Http100"),
         "Http101": fields.Int(required=False, load_from="Http101"),
         "Http102": fields.Int(required=False, load_from="Http102"),
         "Http200": fields.Int(required=False, load_from="Http200"),
         "Http201": fields.Int(required=False, load_from="Http201"),
@@ -196,70 +187,64 @@
         "Http509": fields.Int(required=False, load_from="Http509"),
         "Http510": fields.Int(required=False, load_from="Http510"),
         "Time": fields.Int(required=True, load_from="Time"),
     }
 
 
 class RequestInfoSchema(schema.ResponseSchema):
-    """ RequestInfo - RequestInfo
-    """
+    """RequestInfo - RequestInfo"""
 
     fields = {
         "CdnRequest": fields.Float(required=False, load_from="CdnRequest"),
         "OriginRequest": fields.Float(
             required=False, load_from="OriginRequest"
         ),
         "Time": fields.Int(required=False, load_from="Time"),
     }
 
 
 class LogSetInfoSchema(schema.ResponseSchema):
-    """ LogSetInfo - 日志信息
-    """
+    """LogSetInfo - 日志信息"""
 
     fields = {
         "AbroadLog": fields.List(fields.Str()),
         "CnLog": fields.List(fields.Str()),
         "Time": fields.Int(required=False, load_from="Time"),
     }
 
 
 class LogSetListSchema(schema.ResponseSchema):
-    """ LogSetList - 日志信息列表
-    """
+    """LogSetList - 日志信息列表"""
 
     fields = {
         "Domain": fields.Str(required=False, load_from="Domain"),
         "Logs": fields.List(LogSetInfoSchema()),
     }
 
 
 class UcdnDomainTrafficSetSchema(schema.ResponseSchema):
-    """ UcdnDomainTrafficSet - GetUcdnDomainTraffic
-    """
+    """UcdnDomainTrafficSet - GetUcdnDomainTraffic"""
 
     fields = {
         "Time": fields.Int(required=False, load_from="Time"),
         "Value": fields.Float(required=False, load_from="Value"),
     }
 
 
 class BandwidthInfoDetailSchema(schema.ResponseSchema):
-    """ BandwidthInfoDetail - 带宽值信息模型(时间-带宽)
-    """
+    """BandwidthInfoDetail - 带宽值信息模型(时间-带宽)"""
 
     fields = {
         "Bandwidth": fields.Float(required=True, load_from="Bandwidth"),
         "Time": fields.Int(required=True, load_from="Time"),
     }
 
 
 class TrafficSetSchema(schema.ResponseSchema):
-    """ TrafficSet - GetUcdnTraffic
-    """
+    """TrafficSet - GetUcdnTraffic"""
 
     fields = {
         "Areacode": fields.Str(required=False, load_from="Areacode"),
         "TrafficLeft": fields.Str(required=False, load_from="TrafficLeft"),
         "TrafficTotal": fields.Str(required=False, load_from="TrafficTotal"),
         "TrafficUsed": fields.Str(required=False, load_from="TrafficUsed"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,324 +12,324 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UCloudStackClient, self).__init__(
             config, transport, middleware, logger
         )
 
     def allocate_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ AllocateEIP - 申请外网IP
+        """AllocateEIP - 申请外网IP
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **Bandwidth** (int) - (Required) 带宽，默认值1，默认范围1~100
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **Name** (str) - (Required) 名称
         - **OperatorName** (str) - (Required) 线路。目前支持Bgp
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **IP** (str) - 指定IP
         - **IPVersion** (str) - IP版本，默认值IPv4，支持值：IPv4\IPv6
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
-        
+
         **Response**
 
         - **EIPID** (str) - 申请的EIP的ID
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.AllocateEIPRequestSchema().dumps(d)
 
         resp = self.invoke("AllocateEIP", d, **kwargs)
         return apis.AllocateEIPResponseSchema().loads(resp)
 
     def attach_disk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ AttachDisk - 绑定硬盘
+        """AttachDisk - 绑定硬盘
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **DiskID** (str) - (Required) 硬盘ID
         - **ResourceID** (str) - (Required) 绑定的资源ID
         - **ResourceType** (str) - (Required) 绑定的资源类型，枚举值：VM，标识虚拟机
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.AttachDiskRequestSchema().dumps(d)
 
         resp = self.invoke("AttachDisk", d, **kwargs)
         return apis.AttachDiskResponseSchema().loads(resp)
 
     def attach_nic(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ AttachNIC - 绑定UCloudStack网卡
+        """AttachNIC - 绑定UCloudStack网卡
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **NICID** (str) - (Required) 网卡ID
         - **ResourceID** (str) - (Required) 绑定的资源ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.AttachNICRequestSchema().dumps(d)
 
         resp = self.invoke("AttachNIC", d, **kwargs)
         return apis.AttachNICResponseSchema().loads(resp)
 
     def bind_alarm_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BindAlarmTemplate - 绑定告警模板
+        """BindAlarmTemplate - 绑定告警模板
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **AlarmTemplateID** (str) - (Required) 告警模板ID
         - **ResourceIDs** (list) - (Required) 【数组】告警模板ID。调用方式举例：ResourceIDs.0=“one-id”、ResourceIDs.1=“two-id”。
         - **ResourceType** (str) - (Required) 资源类型。VM：虚拟机, LB:负载均衡, NATGW：nat网关;EIP:弹性IP
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.BindAlarmTemplateRequestSchema().dumps(d)
 
         resp = self.invoke("BindAlarmTemplate", d, **kwargs)
         return apis.BindAlarmTemplateResponseSchema().loads(resp)
 
     def bind_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ BindEIP - 绑定外网 IP
+        """BindEIP - 绑定外网 IP
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；中国
         - **EIPID** (str) - (Required) 外网IP的ID
         - **ResourceID** (str) - (Required) 资源ID
         - **ResourceType** (str) - (Required) 资源类型。VM：虚拟机, LB:负载均衡, NATGW：nat网关
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.BindEIPRequestSchema().dumps(d)
 
         resp = self.invoke("BindEIP", d, **kwargs)
         return apis.BindEIPResponseSchema().loads(resp)
 
     def bind_physical_ip(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BindPhysicalIP - 绑定物理 IP ，被绑定的资源必须处于运行中或有效状态。
+        """BindPhysicalIP - 绑定物理 IP ，被绑定的资源必须处于运行中或有效状态。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **PhysicalIPID** (str) - (Required) 物理IP的ID
         - **ResourceID** (str) - (Required) 资源ID
         - **ResourceType** (str) - (Required) 资源类型。VM：虚拟机
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.BindPhysicalIPRequestSchema().dumps(d)
 
         resp = self.invoke("BindPhysicalIP", d, **kwargs)
         return apis.BindPhysicalIPResponseSchema().loads(resp)
 
     def bind_security_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BindSecurityGroup - 绑定安全组
+        """BindSecurityGroup - 绑定安全组
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **ResourceID** (str) - (Required) 绑定的资源ID。调用方式举例：ResourceID=“one-id”。
         - **SGID** (str) - (Required) 安全组ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **NICType** (str) - 网卡类型，玫举值：WAN，外网；LAN，内网，默认为WAN
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.BindSecurityGroupRequestSchema().dumps(d)
 
         resp = self.invoke("BindSecurityGroup", d, **kwargs)
         return apis.BindSecurityGroupResponseSchema().loads(resp)
 
     def clone_disk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CloneDisk - 克隆硬盘
+        """CloneDisk - 克隆硬盘
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **Name** (str) - (Required) 名称
         - **SrcID** (str) - (Required) 源硬盘ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
-        
+
         **Response**
 
         - **DiskID** (str) - 克隆出的硬盘ID
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CloneDiskRequestSchema().dumps(d)
 
         resp = self.invoke("CloneDisk", d, **kwargs)
         return apis.CloneDiskResponseSchema().loads(resp)
 
     def create_certificate(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateCertificate - 创建证书
+        """CreateCertificate - 创建证书
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Certificate** (str) - (Required) 证书内容
         - **CertificateType** (str) - (Required) 证书类型，枚举值["ServerCrt","CACrt"]。分别表示服务器证书和CA证书。只有在双向认证的时候才需要CA证书
         - **Name** (str) - (Required) 证书名称
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PrivateKey** (str) - 私钥内容,服务器证书必传,CA证书不用传递
         - **Remark** (str) - 证书描述
-        
+
         **Response**
 
         - **CertificateID** (str) - 证书ID
         - **Message** (str) - 错误描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateCertificateRequestSchema().dumps(d)
 
         resp = self.invoke("CreateCertificate", d, **kwargs)
         return apis.CreateCertificateResponseSchema().loads(resp)
 
     def create_custom_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateCustomImage - 创建自制镜像
+        """CreateCustomImage - 创建自制镜像
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **ImageName** (str) - (Required) 镜像名称
         - **VMID** (str) - (Required) 虚拟机ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **ImageDescription** (str) - 镜像描述。
-        
+
         **Response**
 
         - **ImageID** (str) - 创建的自制镜像ID
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateCustomImageRequestSchema().dumps(d)
 
         resp = self.invoke("CreateCustomImage", d, **kwargs)
         return apis.CreateCustomImageResponseSchema().loads(resp)
 
     def create_disk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateDisk - 创建硬盘
+        """CreateDisk - 创建硬盘
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **DiskSpace** (int) - (Required) 磁盘大小
         - **Name** (str) - (Required) 磁盘名称
         - **SetType** (str) - (Required) 磁盘类型。例如：Normal,SSD
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
-        
+
         **Response**
 
         - **DiskID** (str) - 创建的磁盘ID
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateDiskRequestSchema().dumps(d)
 
         resp = self.invoke("CreateDisk", d, **kwargs)
         return apis.CreateDiskResponseSchema().loads(resp)
 
     def create_lb(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateLB - 创建负载均衡
+        """CreateLB - 创建负载均衡
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **LBType** (str) - (Required) 枚举值。LAN：内网，WAN:外网
         - **Name** (str) - (Required) 名称。
@@ -337,322 +337,322 @@
         - **VMType** (str) - (Required) 运行负载均衡实例的主机机型。枚举值：如 Normal ，表示普通机型； SSD，表示 SSD 机型。（机型由平台管理员修改和指定，可参考获取主机机型接口）
         - **VPCID** (str) - (Required) LB实例所在的 VPC ID 。
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **EIPID** (str) - 外网IP的ID，创建外网LB时为必需
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
         - **Remark** (str) - 描述。
         - **SGID** (str) - 安全组ID，创建外网LB时为必需
-        
+
         **Response**
 
         - **LBID** (str) - 返回创建的负载均衡ID
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateLBRequestSchema().dumps(d)
 
         resp = self.invoke("CreateLB", d, **kwargs)
         return apis.CreateLBResponseSchema().loads(resp)
 
     def create_natgw(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateNATGW - 创建NAT网关
+        """CreateNATGW - 创建NAT网关
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **EIPID** (str) - (Required) 外网IP的ID
         - **Name** (str) - (Required) 名称。
         - **SGID** (str) - (Required) 安全组ID
         - **SubnetID** (str) - (Required) NAT网关实例所在的子网 ID
         - **VMType** (str) - (Required) 运行NAT网关实例的主机机型。枚举值：如 Normal ，表示普通机型； SSD，表示 SSD 机型。（机型由平台管理员修改和指定，可参考获取主机机型接口）
         - **VPCID** (str) - (Required) NAT网关实例所在的 VPC ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
         - **Remark** (str) - 描述
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
         - **NATGWID** (str) - 返回创建的NAT网关ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateNATGWRequestSchema().dumps(d)
 
         resp = self.invoke("CreateNATGW", d, **kwargs)
         return apis.CreateNATGWResponseSchema().loads(resp)
 
     def create_natgw_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateNATGWRule - 添加NAT网关白名单
+        """CreateNATGWRule - 添加NAT网关白名单
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **BindResourceID** (str) - (Required) 绑定的虚拟机资源ID
         - **NATGWID** (str) - (Required) NAT网关ID
         - **NATGWType** (str) - (Required) NAT的类型。枚举值：SNAT，DNAT
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
         - **RuleID** (str) - 白名单ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateNATGWRuleRequestSchema().dumps(d)
 
         resp = self.invoke("CreateNATGWRule", d, **kwargs)
         return apis.CreateNATGWRuleResponseSchema().loads(resp)
 
     def create_nic(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateNIC - 创建网卡
+        """CreateNIC - 创建网卡
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **Name** (str) - (Required) 名称
         - **SubnetID** (str) - (Required) Subnet ID
         - **VPCID** (str) - (Required) VPC ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **IP** (str) - 指定IP
         - **SGID** (str) - 安全组 ID
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
         - **NICID** (str) - 创建的网卡 ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateNICRequestSchema().dumps(d)
 
         resp = self.invoke("CreateNIC", d, **kwargs)
         return apis.CreateNICResponseSchema().loads(resp)
 
     def create_physical_ip(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreatePhysicalIP - 创建物理 IP ，需确保平台已配置物理 IP 线路相关信息及物理网络联通性。
+        """CreatePhysicalIP - 创建物理 IP ，需确保平台已配置物理 IP 线路相关信息及物理网络联通性。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **Name** (str) - (Required) 物理IP名称，限制字符长度30
         - **OperatorName** (str) - (Required) 物理IP线路
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Remark** (str) - 描述
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
         - **PhysicalIPID** (str) - 返回创建的物理IP的ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreatePhysicalIPRequestSchema().dumps(d)
 
         resp = self.invoke("CreatePhysicalIP", d, **kwargs)
         return apis.CreatePhysicalIPResponseSchema().loads(resp)
 
     def create_rs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateRS - 为负载均衡的 VServer 添加后端服务节点。
+        """CreateRS - 为负载均衡的 VServer 添加后端服务节点。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **BindResourceID** (str) - (Required) 服务节点的资源 ID ，仅支持添加与 LB 相同 VPC 的虚拟机资源
         - **LBID** (str) - (Required) 负载均衡ID
         - **Port** (int) - (Required) 服务节点暴露的服务端口号
         - **VSID** (str) - (Required) VServer的ID
         - **Weight** (int) - (Required) 服务节点的权重
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
         - **RSID** (str) - 返回创建的RSID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateRSRequestSchema().dumps(d)
 
         resp = self.invoke("CreateRS", d, **kwargs)
         return apis.CreateRSResponseSchema().loads(resp)
 
     def create_security_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateSecurityGroup - 创建安全组
+        """CreateSecurityGroup - 创建安全组
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Name** (str) - (Required) 名称;
         - **Rule** (list) - (Required) 【数组】安全组规则。输入有效的规则，调用方式举例：Rule.0=“TCP|23|0.0.0.0/0|ACCEPT|HIGH|1”、Rule.1=“TCP|55|0.0.0.0/0|ACCEPT|HIGH|1”
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Remark** (str) - 描述;
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
         - **SGID** (str) - 创建的安全组ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateSecurityGroupRequestSchema().dumps(d)
 
         resp = self.invoke("CreateSecurityGroup", d, **kwargs)
         return apis.CreateSecurityGroupResponseSchema().loads(resp)
 
     def create_security_group_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateSecurityGroupRule - 创建安全组规则
+        """CreateSecurityGroupRule - 创建安全组规则
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Rules** (list) - (Required) 【数组】安全组规则。输入有效的规则，调用方式举例：Rule.0=“TCP|23|0.0.0.0/0|ACCEPT|HIGH|1”、Rule.1=“TCP|55|0.0.0.0/0|ACCEPT|HIGH|1”
         - **SGID** (str) - (Required) 安全组ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
         - **SGRuleID** (str) - 创建的安全组规则ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateSecurityGroupRuleRequestSchema().dumps(d)
 
         resp = self.invoke("CreateSecurityGroupRule", d, **kwargs)
         return apis.CreateSecurityGroupRuleResponseSchema().loads(resp)
 
     def create_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateSnapshot - 创建硬盘快照
+        """CreateSnapshot - 创建硬盘快照
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：如 cn,表示中国。
         - **DiskID** (str) - (Required) 硬盘ID，输入“有效”状态的ID
         - **Name** (str) - (Required) 快照名称，限制字符长度30
         - **Zone** (str) - (Required) 可用区。枚举值：如 zone-01，表示可用区1。
         - **Remark** (str) - 描述，限制字符长度100
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
         - **SnapshotID** (str) - 创建的快照ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateSnapshotRequestSchema().dumps(d)
 
         resp = self.invoke("CreateSnapshot", d, **kwargs)
         return apis.CreateSnapshotResponseSchema().loads(resp)
 
     def create_subnet(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateSubnet - 创建子网
+        """CreateSubnet - 创建子网
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Name** (str) - (Required) 名称;
         - **Network** (str) - (Required) 网段。列如：10.0.0.0/16；
         - **VPCID** (str) - (Required) 所属VPCID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Remark** (str) - 描述;
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
         - **SubnetID** (str) - 创建Subnet的ID；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateSubnetRequestSchema().dumps(d)
 
         resp = self.invoke("CreateSubnet", d, **kwargs)
         return apis.CreateSubnetResponseSchema().loads(resp)
 
     def create_user(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateUser - 管理员添加账号
+        """CreateUser - 管理员添加账号
 
         **Request**
 
         - **PassWord** (str) - (Required) 账号密码。
         - **UserEmail** (str) - (Required) 账号邮箱。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
         - **UserID** (int) - 账户ID
-        
+
         """
         # build request
         d = {}
         req and d.update(req)
         d = apis.CreateUserRequestSchema().dumps(d)
 
         resp = self.invoke("CreateUser", d, **kwargs)
         return apis.CreateUserResponseSchema().loads(resp)
 
     def create_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateVMInstance - 创建虚拟机
+        """CreateVMInstance - 创建虚拟机
 
         **Request**
 
         - **Region** (str) - (Config) 地域或数据中心。枚举值：cn,表示中国；
         - **BootDiskSetType** (str) - (Required) 系统盘类型。枚举值：Normal，表示普通；SSD，表示SSD；
         - **CPU** (int) - (Required) CPU个数，如1，2，4，8，16，32，64等。
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
@@ -671,62 +671,62 @@
         - **GPU** (int) - GPU 卡核心的占用个数。枚举值：【1,2,4】。GPU与CPU、内存大小关系：CPU个数>=4*GPU个数，同时内存与CPU规格匹配.
         - **IPVersion** (str) - 创建虚拟机同时绑定外网 IP 的 IP 版本。枚举值：IPv4 & IPv6，默认为 IPv4
         - **InternalIP** (str) - 指定内网IP。输入有效的指定内网 IP，不指定时系统将自动从子网分配 IP 地址。
         - **InternetIP** (str) - 手动指定虚拟机绑定外网 IP 的地址，IP地址必须包含在网段内。
         - **LANSGID** (str) - 内网安全组 ID。输入“有效”状态的安全组的ID。
         - **OperatorName** (str) - 创建虚拟机同时绑定外网 IP 的网段，可由管理员自定义。
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
-        
+
         **Response**
 
         - **DiskID** (str) - 返回同时创建的数据盘 ID
         - **EIPID** (str) - 返回同时创建的外网IP ID
         - **Message** (str) - 返回信息描述。
         - **VMID** (str) - 返回创建的虚拟机 ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateVMInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("CreateVMInstance", d, **kwargs)
         return apis.CreateVMInstanceResponseSchema().loads(resp)
 
     def create_vpc(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateVPC - 创建VPC
+        """CreateVPC - 创建VPC
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Name** (str) - (Required) 名称;
         - **Network** (str) - (Required) 网段。例如：10.0.0.0/16；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Remark** (str) - 描述;
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
         - **VPCID** (str) - 创建的VPCID；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateVPCRequestSchema().dumps(d)
 
         resp = self.invoke("CreateVPC", d, **kwargs)
         return apis.CreateVPCResponseSchema().loads(resp)
 
     def create_vs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateVS - 创建负载均衡VServer
+        """CreateVS - 创建负载均衡VServer
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **HealthcheckType** (str) - (Required) 健康检查类型，枚举值，Port:端口,Path:域名。TCP和UDP协议只支持Port类型。
         - **LBID** (str) - (Required) 负载均衡ID
         - **Port** (int) - (Required) VServer 的监听端口。端口范围为 1~65535 ，其中 323、9102、9103、9104、9105、60909、60910 被系统占用。
@@ -737,531 +737,531 @@
         - **Domain** (str) - HTTP 健康检查时校验请求的 HOST 字段中的域名。当健康检查类型为端口检查时，该值为空。
         - **KeepaliveTimeout** (int) - 负载均衡的连接空闲超时时间，单位为秒，默认值为 60s 。
         - **Path** (str) - HTTP 健康检查的路径，健康检查类型为 HTTP 检查时为必填项。当健康检查类型为端口检查时，该值为空。
         - **PersistenceKey** (str) - 会话保持KEY，会话保持类型为Manual时为必填项，仅当 VServer 协议为 HTTP 时有效。
         - **PersistenceType** (str) - 会话保持类型。枚举值：None:关闭；Auto:自动生成；Manual:手动生成 。当协议为 TCP 时，该值不生效，会话保持和选择的调度算法相关；当协议为 UDP 时 Auto 表示开启会话保持 。
         - **SSLMode** (str) - SSL认证模式,HTTPS协议下必传,取值范围["simplex","duplex"]分别表示单向认证和双向认证。
         - **ServerCertificateID** (str) - 服务器证书ID，用于证明服务器的身份，仅当 VServer监听协议为 HTTPS时有效。
-        
+
         **Response**
 
         - **Action** (str) - 操作名称
         - **Message** (str) - 返回信息描述。
         - **RetCode** (int) - 返回码
         - **VSID** (str) - 返回创建的VSID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateVSRequestSchema().dumps(d)
 
         resp = self.invoke("CreateVS", d, **kwargs)
         return apis.CreateVSResponseSchema().loads(resp)
 
     def create_vs_policy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateVSPolicy - 创建七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
+        """CreateVSPolicy - 创建七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **RSIDs** (list) - (Required) 【数组】内容转发规则应用的服务节点的 ID，来源于 VServer 中添加的服务节点。调用方式举例：RSIDs.0=“one-id”、RSIDs.1=“two-id”。
         - **VSID** (str) - (Required) VServer的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Domain** (str) - 内容转发规则关联的请求域名，值可为空，即代表仅匹配路径。域名和路径至少需要指定一项，且域名和路径的组合在一个 VServer 中必须唯一。
         - **Path** (str) - 内容转发规则关联的请求访问路径，如 "/" 。域名和路径至少需要指定一项，且域名和路径的组合在一个 VServer 中必须唯一。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
         - **PolicyID** (str) - 返回创建的内容转发规则ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.CreateVSPolicyRequestSchema().dumps(d)
 
         resp = self.invoke("CreateVSPolicy", d, **kwargs)
         return apis.CreateVSPolicyResponseSchema().loads(resp)
 
     def delete_certificate(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteCertificate - 删除证书
+        """DeleteCertificate - 删除证书
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **CertificateID** (str) - (Required) 证书ID
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteCertificateRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteCertificate", d, **kwargs)
         return apis.DeleteCertificateResponseSchema().loads(resp)
 
     def delete_custom_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteCustomImage - 删除自制镜像
+        """DeleteCustomImage - 删除自制镜像
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **ImageID** (str) - (Required) 自制镜像ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteCustomImageRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteCustomImage", d, **kwargs)
         return apis.DeleteCustomImageResponseSchema().loads(resp)
 
     def delete_disk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteDisk - 删除硬盘
+        """DeleteDisk - 删除硬盘
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **DiskID** (str) - (Required) 被删除的硬盘ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteDiskRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteDisk", d, **kwargs)
         return apis.DeleteDiskResponseSchema().loads(resp)
 
     def delete_lb(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteLB - 删除负载均衡
+        """DeleteLB - 删除负载均衡
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteLBRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteLB", d, **kwargs)
         return apis.DeleteLBResponseSchema().loads(resp)
 
     def delete_natgw(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteNATGW - 删除NAT网关
+        """DeleteNATGW - 删除NAT网关
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **NATGWID** (str) - (Required) NAT网关ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteNATGWRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteNATGW", d, **kwargs)
         return apis.DeleteNATGWResponseSchema().loads(resp)
 
     def delete_natgw_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteNATGWRule - 删除NAT网关白名单
+        """DeleteNATGWRule - 删除NAT网关白名单
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **NATGWID** (str) - (Required) nat网关ID
         - **RuleID** (str) - (Required) 白名单ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteNATGWRuleRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteNATGWRule", d, **kwargs)
         return apis.DeleteNATGWRuleResponseSchema().loads(resp)
 
     def delete_nic(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteNIC - 删除网卡
+        """DeleteNIC - 删除网卡
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **NICID** (str) - (Required) 被删除的网卡 ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteNICRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteNIC", d, **kwargs)
         return apis.DeleteNICResponseSchema().loads(resp)
 
     def delete_physical_ip(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeletePhysicalIP - 删除物理IP
+        """DeletePhysicalIP - 删除物理IP
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **PhysicalIPID** (str) - (Required) 物理IP的ID
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回状态描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeletePhysicalIPRequestSchema().dumps(d)
 
         resp = self.invoke("DeletePhysicalIP", d, **kwargs)
         return apis.DeletePhysicalIPResponseSchema().loads(resp)
 
     def delete_rs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteRS - 移除负载均衡的单个服务节点
+        """DeleteRS - 移除负载均衡的单个服务节点
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **RSID** (str) - (Required) RServer的ID
         - **VSID** (str) - (Required) VServer的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteRSRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteRS", d, **kwargs)
         return apis.DeleteRSResponseSchema().loads(resp)
 
     def delete_security_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteSecurityGroup - 删除安全组
+        """DeleteSecurityGroup - 删除安全组
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **SGID** (str) - (Required) 安全组ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteSecurityGroupRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteSecurityGroup", d, **kwargs)
         return apis.DeleteSecurityGroupResponseSchema().loads(resp)
 
     def delete_security_group_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteSecurityGroupRule - 删除安全组规则
+        """DeleteSecurityGroupRule - 删除安全组规则
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **SGID** (str) - (Required) 安全组ID
         - **SGRuleID** (str) - (Required) 安全组规则ID
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteSecurityGroupRuleRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteSecurityGroupRule", d, **kwargs)
         return apis.DeleteSecurityGroupRuleResponseSchema().loads(resp)
 
     def delete_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteSnapshot - 删除快照，仅支持状态为正常的快照进行删除操作。
+        """DeleteSnapshot - 删除快照，仅支持状态为正常的快照进行删除操作。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：如 cn,表示中国。
         - **SnapshotID** (str) - (Required) 快照ID
         - **Zone** (str) - (Required) 可用区。枚举值：如 zone-01，表示可用区1。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteSnapshotRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteSnapshot", d, **kwargs)
         return apis.DeleteSnapshotResponseSchema().loads(resp)
 
     def delete_subnet(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteSubnet - 删除子网
+        """DeleteSubnet - 删除子网
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **SubnetID** (str) - (Required) SubnetID
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteSubnetRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteSubnet", d, **kwargs)
         return apis.DeleteSubnetResponseSchema().loads(resp)
 
     def delete_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteVMInstance - 删除虚拟机
+        """DeleteVMInstance - 删除虚拟机
 
         **Request**
 
         - **Region** (str) - (Config) 地域。 枚举值：cn，表示中国；
         - **VMID** (str) - (Required) 虚拟机 ID。输入有效的虚拟机 ID。
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteVMInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteVMInstance", d, **kwargs)
         return apis.DeleteVMInstanceResponseSchema().loads(resp)
 
     def delete_vpc(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteVPC - 删除VPC
+        """DeleteVPC - 删除VPC
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **VPCID** (str) - (Required) ID
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteVPCRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteVPC", d, **kwargs)
         return apis.DeleteVPCResponseSchema().loads(resp)
 
     def delete_vs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteVS - 删除VServer
+        """DeleteVS - 删除VServer
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) VServer 监听器所属的负载均衡 ID
         - **VSID** (str) - (Required) 负载均衡VServer监听器ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteVSRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteVS", d, **kwargs)
         return apis.DeleteVSResponseSchema().loads(resp)
 
     def delete_vs_policy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteVSPolicy - 删除七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
+        """DeleteVSPolicy - 删除七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **PolicyID** (str) - (Required) 内容转发规则ID
         - **VSID** (str) - (Required) VServer的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DeleteVSPolicyRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteVSPolicy", d, **kwargs)
         return apis.DeleteVSPolicyResponseSchema().loads(resp)
 
     def describe_certificate(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeCertificate - 查询证书
+        """DescribeCertificate - 查询证书
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **CertificateIDs** (list) - 证书ID列表
         - **CertificateType** (str) - 证书类型，枚举值["ServerCrt","CACrt"]。分别表示服务器证书和CA证书。
         - **Limit** (int) - 返回数据长度，默认为20，最大100
         - **Offset** (int) - 列表起始位置偏移量，默认为0
-        
+
         **Response**
 
         - **Infos** (list) - 见 **CertificateInfo** 模型定义
         - **Message** (str) - 返回信息描述
         - **TotalCount** (int) - 证书总个数
-        
+
         **Response Model**
-        
-        **BindVSInfo** 
-        
+
+        **BindVSInfo**
+
         - **LBID** (str) - LB ID
         - **LBName** (str) - LB名称
         - **Port** (int) - VS的端口
         - **Protocol** (str) - VS的协议
         - **VSID** (str) - VS ID
 
-        **CertificateInfo** 
-        
+        **CertificateInfo**
+
         - **CertificateContent** (str) - 证书内容
         - **CertificateID** (str) - 证书ID
         - **CertificateType** (str) - 证书类型，枚举值["ServerCrt","CACrt"]
         - **CommonName** (str) - 主域名
         - **CreateTime** (int) - 创建时间（平台创建时间）
         - **ExpireTime** (int) - 证书内容的过期时间
         - **Fingerprint** (str) - 证书指纹
@@ -1283,35 +1283,35 @@
 
         resp = self.invoke("DescribeCertificate", d, **kwargs)
         return apis.DescribeCertificateResponseSchema().loads(resp)
 
     def describe_disk(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeDisk - 获取硬盘信息
+        """DescribeDisk - 获取硬盘信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **DiskIDs** (list) - 【数组】磁盘的 ID。输入有效的 ID。调用方式举例：DiskIDs.0=“one-id”、DiskIDs.1=“two-id”。
         - **DiskType** (str) - 硬盘用途类型，默认空返回虚拟机所有硬盘，支持值：Boot（系统盘）、Data（数据盘）
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **DiskInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回磁盘总个数。
-        
+
         **Response Model**
-        
-        **DiskInfo** 
-        
+
+        **DiskInfo**
+
         - **AttachResourceID** (str) - 绑定资源ID
         - **ChargeType** (str) - 硬盘计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **CreateTime** (int) - 创建时间。时间戳
         - **DiskID** (str) - 硬盘ID
         - **DiskStatus** (str) - 硬盘状态。Creating：创建中,BeingCloned：正在被克隆中,Unbound：已解绑,Unbounding：解绑中,Bounding：绑定中,Bound：已绑定,Upgrading：升级中,Deleting：删除中,Deleted：已删除,Releasing：销毁中,Released：已销毁；Snapshoting（快照中）；Rollbacking（回滚中）
         - **DiskType** (str) - 硬盘用途类型，Boot（系统盘）、Data（数据盘）
         - **ExpireTime** (int) - 过期时间。时间戳
@@ -1330,36 +1330,36 @@
         req and d.update(req)
         d = apis.DescribeDiskRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeDisk", d, **kwargs)
         return apis.DescribeDiskResponseSchema().loads(resp)
 
     def describe_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeEIP - 获取外网IP的信息
+        """DescribeEIP - 获取外网IP的信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **BindResourceID** (str) - 绑定资源ID，查询该资源绑定的所有 EIP
         - **EIPIDs** (list) - 【数组】外网的 ID。输入有效的 ID。调用方式举例：EIPIDs.0=“one-id”、EIPIDs.1=“two-id”
         - **IPVersion** (str) - 版本，支持IPv4、IPv6
         - **Limit** (str) - 返回数据长度，默认为20，最大100。
         - **Offset** (str) - 列表起始位置偏移量，默认为0。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **EIPInfo** 模型定义
         - **Message** (str) - 返回信息描述
         - **Totalcount** (int) - 返回现有外网IP总数
-        
+
         **Response Model**
-        
-        **EIPInfo** 
-        
+
+        **EIPInfo**
+
         - **Bandwidth** (int) - 带宽大小
         - **BindResourceID** (str) - 绑定资源ID
         - **BindResourceType** (str) - 绑定资源类型
         - **CanDefaultGW** (int) - 所处线路是否为默认路由，1代表所处线路是默认路由；默认路由的可以设置成出口
         - **ChargeType** (str) - 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **CreateTime** (int) - 创建时间。时间戳
         - **EIPID** (str) - ID
@@ -1384,37 +1384,37 @@
 
         resp = self.invoke("DescribeEIP", d, **kwargs)
         return apis.DescribeEIPResponseSchema().loads(resp)
 
     def describe_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeImage - 获取镜像信息，包括默认镜像和自制镜像。
+        """DescribeImage - 获取镜像信息，包括默认镜像和自制镜像。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **ImageIDs** (list) - 【数组】镜像的 ID。输入有效的 ID。调用方式举例：ImageIDs.0=“one-id”、ImageIDs.1=“two-id”。
         - **ImageType** (str) - 镜像类型。枚举值：Base(基础镜像，平台默认提供的镜像)，Custom(自制镜像，通过虚拟机导出的镜像) 。若该值为空，默认查询所有镜像。
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
-        
+
         **Response**
 
         - **Action** (str) - 操作名称
         - **Infos** (list) - 见 **ImageInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **RetCode** (int) - 返回码
         - **TotalCount** (int) - 返回镜像的总个数。
-        
+
         **Response Model**
-        
-        **ImageInfo** 
-        
+
+        **ImageInfo**
+
         - **CreateTime** (int) - 创建时间。时间戳。
         - **ImageID** (str) - 镜像ID
         - **ImageStatus** (str) - 镜像状态。枚举类型：Making（创建中）,Terminating（销毁中）,Used（可用）,Deleting（删除中）,Deleted（已删除）, Uploading（导入中）, Failed（导入失败）
         - **ImageType** (str) - 镜像类型。枚举类型：Base(基础镜像),Custom（自制镜像）。
         - **Name** (str) - 镜像名称
         - **OSDistribution** (str) - 镜像系统发行版本。例如：Centos, Ubuntu, Windows等
         - **OSName** (str) - 系统名称。例如：CentOS 7.4 x86_64
@@ -1431,36 +1431,36 @@
         req and d.update(req)
         d = apis.DescribeImageRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeImage", d, **kwargs)
         return apis.DescribeImageResponseSchema().loads(resp)
 
     def describe_lb(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeLB - 获取负载均衡信息
+        """DescribeLB - 获取负载均衡信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **LBIDs** (list) - 【数组】负载均衡的 ID。调用方式举例：LBIDs.0=“one-id”、LBIDs.1=“two-id”。
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **SubnetID** (str) - 子网ID
         - **VPCID** (str) - VPCID
-        
+
         **Response**
 
         - **Infos** (list) - 见 **LBInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回负载均衡总个数。
-        
+
         **Response Model**
-        
-        **LBInfo** 
-        
+
+        **LBInfo**
+
         - **AlarmTemplateID** (str) - 告警模板ID
         - **ChargeType** (str) - 虚拟机计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **CreateTime** (int) - 创建时间，时间戳
         - **ExpireTime** (int) - 过期时间，时间戳
         - **LBID** (str) - 负载均衡ID
         - **LBStatus** (str) - 状态。Creating:创建中,Running:运行中,Deleting:删除中,Deleted:已删除
         - **LBType** (str) - 负载均衡类型，枚举值，WAN:外网负载均衡，LAN:内网负载均衡。
@@ -1485,41 +1485,41 @@
 
         resp = self.invoke("DescribeLB", d, **kwargs)
         return apis.DescribeLBResponseSchema().loads(resp)
 
     def describe_metric(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeMetric - 获取资源监控信息
+        """DescribeMetric - 获取资源监控信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn，表示中国；
         - **BeginTime** (str) - (Required) 开始时间。使用unix时间戳
         - **EndTime** (str) - (Required) 结束时间。使用Unix时间戳
         - **MetricName** (list) - (Required) 监控指标。1. 获取虚拟机监控信息调用举例，MetricName.0="CPUUtilization"、MetricName.0="MemUsage"。虚拟机监控指标枚举值：BlockProcessCount，表示阻塞进程数；CPUUtilization，表示CPU使用率；DiskReadOps，表示磁盘读次数；DiskWriteOps，表示磁盘写次数；IORead，表示磁盘读吞吐；IOWrite，表示磁盘写吞吐；LoadAvg，表示平均负载1分钟；MemUsage，表示内存使用率；NetPacketIn，表示网卡入包量；NetPacketOut，表示网卡出包量；NICIn，表示网卡入带宽；NICOut，表示网卡出带宽；SpaceUsage，表示空间使用率；TCPConnectCount，表示TCP连接数；2. EIP监控指标：NetPacketIn：入包量；NetPacketOut：出包量；NICIn：入带宽；NICOut：出带宽；NICOutUsage：出带宽使用率；
         - **ResourceID** (str) - (Required) 资源ID
         - **ResourceType** (str) - (Required) 资源类型。VM：虚拟机；EIP：弹性IP
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，中国；
-        
+
         **Response**
 
         - **Infos** (list) - 见 **MetricInfo** 模型定义
         - **Message** (str) - 返回信息描述
         - **TotalCount** (int) - 返回监控信息条数
-        
+
         **Response Model**
-        
-        **MetricSet** 
-        
+
+        **MetricSet**
+
         - **Timestamp** (int) - 监控时间
         - **Value** (float) - 监控值
 
-        **MetricInfo** 
-        
+        **MetricInfo**
+
         - **Infos** (list) - 见 **MetricSet** 模型定义
         - **MetricName** (str) - 监控指标。虚拟机的监控指标枚举值为：BlockProcessCount，表示阻塞进程数；CPUUtilization，表示CPU使用率；DiskReadOps，表示磁盘读次数；DiskWriteOps，表示磁盘写次数；IORead，表示磁盘读吞吐；IOWrite，表示磁盘写吞吐；LoadAvg，表示平均负载1分钟；MemUsage，表示内存使用率；NetPacketIn，表示网卡入包量；NetPacketOut，表示网卡出包量；NICIn，表示网卡入带宽；NICOut，表示网卡出带宽；SpaceUsage，表示空间使用率；TCPConnectCount，表示TCP连接数；
 
         """
         # build request
         d = {
             "Region": self.config.region,
@@ -1529,34 +1529,34 @@
 
         resp = self.invoke("DescribeMetric", d, **kwargs)
         return apis.DescribeMetricResponseSchema().loads(resp)
 
     def describe_natgw(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeNATGW - 获取NAT网关信息
+        """DescribeNATGW - 获取NAT网关信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **NATGWIDs** (list) - 【数组】NAT网关的 ID。调用方式举例：NATGWIDs.0=“one-id”、NATGWIDs.1=“two-id”。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **NATGWInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回NAT网关总个数
-        
+
         **Response Model**
-        
-        **NATGWInfo** 
-        
+
+        **NATGWInfo**
+
         - **AlarmTemplateID** (str) - 告警模板ID
         - **ChargeType** (str) - 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **CreateTime** (int) - 创建时间，时间戳
         - **EIP** (str) - 虚拟IP
         - **ExpireTime** (int) - 过期时间，时间戳
         - **NATGWID** (str) - NAT网关ID
         - **NATGWStatus** (str) - 状态。Creating:创建中, Running:运行中, Deleting:删除中, Deleted:已删除
@@ -1578,37 +1578,37 @@
 
         resp = self.invoke("DescribeNATGW", d, **kwargs)
         return apis.DescribeNATGWResponseSchema().loads(resp)
 
     def describe_natgw_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeNATGWRule - 获取NAT网关白名单信息
+        """DescribeNATGWRule - 获取NAT网关白名单信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **NATGWID** (str) - (Required) NAT网关ID
         - **NATGWType** (str) - (Required) NAT类型。枚举值：SNAT，DNAT
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **BindResourceIDs** (list) - 【数组】NAT网关白名单资源ID。调用方式举例：NATGWRules.0=“one-id”、NATGWRules.1=“two-id”。
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **RuleIDs** (list) - 【数组】NAT网关白名单ID。调用方式举例：NATGWRules.0=“one-id”、NATGWRules.1=“two-id”。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **NATGWRuleInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回NAT网关白名单资源总个数。
-        
+
         **Response Model**
-        
-        **NATGWRuleInfo** 
-        
+
+        **NATGWRuleInfo**
+
         - **BindResourceID** (str) - 绑定的资源ID
         - **BindResourceType** (str) - 绑定资源的类型
         - **CreateTime** (int) - 创建时间，时间戳。
         - **IP** (str) - 白名单资源的内网IP地址
         - **NATGWID** (str) - NAT网关ID
         - **NATGWType** (str) - nat网关类型
         - **Name** (str) - 添加的白名单资源名称
@@ -1623,34 +1623,34 @@
         req and d.update(req)
         d = apis.DescribeNATGWRuleRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeNATGWRule", d, **kwargs)
         return apis.DescribeNATGWRuleResponseSchema().loads(resp)
 
     def describe_nic(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeNIC - 获取网卡信息
+        """DescribeNIC - 获取网卡信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **NICIDs** (list) - 【数组】网卡的 ID。输入有效的 ID。调用方式举例：NICIDs.0=“one-id”、NICIDs.1=“two-id”。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **NICInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回网卡总个数。
-        
+
         **Response Model**
-        
-        **NICInfo** 
-        
+
+        **NICInfo**
+
         - **BindResourceID** (str) - 绑定资源ID
         - **CreateTime** (int) - 创建时间。时间戳
         - **IP** (str) - IP
         - **MAC** (str) - mac 地址
         - **NICID** (str) - 网卡ID
         - **NICStatus** (str) - 网卡状态。枚举值。Creating：创建中,Free：未绑定,Unbounding：解绑中,Bounding：绑定中,Bound：已绑定,BindSGing：绑定安全组中,UnbindSGing：解绑安全组中,UpdateSGing：更新安全组中,Deleting：删除中,Deleted：已删除,Releasing：销毁中,Released：已销毁
         - **Name** (str) - 名称
@@ -1671,50 +1671,50 @@
 
         resp = self.invoke("DescribeNIC", d, **kwargs)
         return apis.DescribeNICResponseSchema().loads(resp)
 
     def describe_op_logs(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeOPLogs - 查询操作日志
+        """DescribeOPLogs - 查询操作日志
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BeginTime** (int) - (Required) 开始时间
         - **EndTime** (int) - (Required) 结束时间
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **IsSuccess** (str) - 是否操作成功
-        - **Limit** (int) - 
-        - **Offset** (int) - 
+        - **Limit** (int) -
+        - **Offset** (int) -
         - **ResourceID** (str) - 资源ID
         - **ResourceType** (str) - 资源类型
-        
+
         **Response**
 
         - **Infos** (list) - 见 **OPLogInfo** 模型定义
         - **Message** (str) - 错误信息
         - **TotalCount** (int) - 总数
-        
+
         **Response Model**
-        
-        **OPLogInfo** 
-        
+
+        **OPLogInfo**
+
         - **CreateTime** (int) - 创建时间
         - **IsSuccess** (str) - 是否操作成功， Yes, No
         - **OPLogsID** (str) - 日志ID
         - **OPName** (str) - API
         - **OPTime** (int) - 操作时间
         - **OpMessage** (str) - 错误信息
-        - **Region** (str) - 
+        - **Region** (str) -
         - **ResourceID** (str) - 资源ID
         - **ResourceType** (int) - 资源类型
         - **RetCode** (int) - 状态码
         - **UserEmail** (str) - 账号邮箱
-        - **Zone** (str) - 
+        - **Zone** (str) -
 
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
@@ -1722,34 +1722,34 @@
 
         resp = self.invoke("DescribeOPLogs", d, **kwargs)
         return apis.DescribeOPLogsResponseSchema().loads(resp)
 
     def describe_physical_ip(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribePhysicalIP - 获取物理IP信息
+        """DescribePhysicalIP - 获取物理IP信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (str) - 返回数据长度，默认为20，最大100。
         - **Offset** (str) - 列表起始位置偏移量，默认为0。
         - **PhysicalIPIDs** (list) - 【数组】物理IP的 ID。输入有效的 ID。调用方式举例：PhysicalIPIDs.0=“one-id”、PhysicalIPIDs.1=“two-id”
-        
+
         **Response**
 
         - **Infos** (list) - 见 **PhysicalIPInfo** 模型定义
         - **Message** (str) - 返回信息描述
         - **TotalCount** (int) - 返回现有物理IP总数
-        
+
         **Response Model**
-        
-        **PhysicalIPInfo** 
-        
+
+        **PhysicalIPInfo**
+
         - **BindResourceID** (str) - 绑定资源ID
         - **BindResourceType** (str) - 绑定资源类型
         - **CreateTime** (int) - 创建时间。时间戳
         - **IP** (str) - 物理IP
         - **Name** (str) - 名称
         - **OperatorName** (str) - 线路
         - **PhysicalIPID** (str) - 物理IP的ID
@@ -1767,36 +1767,36 @@
         req and d.update(req)
         d = apis.DescribePhysicalIPRequestSchema().dumps(d)
 
         resp = self.invoke("DescribePhysicalIP", d, **kwargs)
         return apis.DescribePhysicalIPResponseSchema().loads(resp)
 
     def describe_rs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeRS - 获取负载均衡服务的服务节点信息
+        """DescribeRS - 获取负载均衡服务的服务节点信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **RSIDs** (list) - 【数组】RServer的 ID。调用方式举例：RSIDs.0=“one-id”、RSIDs.1=“two-id”。
         - **VSID** (str) - VServer的ID
-        
+
         **Response**
 
         - **Infos** (list) - 见 **RSInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回该负载均衡下VServer的总个数。
-        
+
         **Response Model**
-        
-        **RSInfo** 
-        
+
+        **RSInfo**
+
         - **BindResourceID** (str) - 绑定的资源ID
         - **CreateTime** (int) - 创建时间，时间戳
         - **IP** (str) - 服务节点的内网 IP 地址
         - **LBID** (str) - 服务节点所属的负载均衡 ID
         - **Name** (str) - 服务节点的资源名称
         - **Port** (int) - 服务节点暴露的服务端口号
         - **RSID** (str) - 服务节点的 ID
@@ -1816,33 +1816,33 @@
 
         resp = self.invoke("DescribeRS", d, **kwargs)
         return apis.DescribeRSResponseSchema().loads(resp)
 
     def describe_recycled_resource(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeRecycledResource - 查询回收站资源
+        """DescribeRecycledResource - 查询回收站资源
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：如 cn,表示中国。
         - **Zone** (str) - (Required) 可用区。枚举值：如 zone-01，表示可用区1。
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **ResourceIDs** (list) - 【数组】资源ID，输入“有效”的ID。调用方式举例：ResourceIDs.0=“one-id”、ResourceIDs.1=“two-id”。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **RecycledResourceInfo** 模型定义
         - **TotalCount** (int) - 返回回收站资源的总个数
-        
+
         **Response Model**
-        
-        **RecycledResourceInfo** 
-        
+
+        **RecycledResourceInfo**
+
         - **CreateTime** (int) - 创建时间
         - **DeleteTime** (int) - 删除时间
         - **Description** (str) - 描述
         - **ExpireTime** (int) - 过期时间
         - **IsAutoTerminated** (bool) - 是否自动销户
         - **Name** (str) - 名称
         - **Region** (str) - 地域
@@ -1862,44 +1862,44 @@
 
         resp = self.invoke("DescribeRecycledResource", d, **kwargs)
         return apis.DescribeRecycledResourceResponseSchema().loads(resp)
 
     def describe_security_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeSecurityGroup - 查询安全组信息
+        """DescribeSecurityGroup - 查询安全组信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **Zone** (str) - (Required) 可用区。
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **SGIDs** (list) - 【数组】安全组的 ID。输入有效的 ID。调用方式举例：SGIDs.0=“one-id”、SGIDs.1=“two-id”
-        
+
         **Response**
 
         - **Infos** (list) - 见 **SGInfo** 模型定义
         - **Message** (str) - 返回信息描述；
         - **TotalCount** (int) - 安全组的总数
-        
+
         **Response Model**
-        
-        **SGRuleInfo** 
-        
+
+        **SGRuleInfo**
+
         - **DstPort** (str) - 端口号
         - **IsIn** (str) - 方向。1：入，0：出
         - **Priority** (str) - 优先级。HIGH:高，MEDIUM:中，LOW:低
         - **ProtocolType** (str) - 协议
         - **RuleAction** (str) - 动作。ACCEPT：接受，DROP：拒绝
         - **RuleID** (str) - 规则ID
         - **SrcIP** (str) - IP或者掩码/段形式。10.0.0.2,10.0.10.10/16
 
-        **SGInfo** 
-        
+        **SGInfo**
+
         - **CreateTime** (int) - 创建时间，时间戳
         - **Name** (str) - 名称
         - **Region** (str) - 地域
         - **Remark** (str) - 描述
         - **ResourceCount** (int) - 资源绑定数量
         - **Rule** (list) - 见 **SGRuleInfo** 模型定义
         - **RuleCount** (int) - 规则数量
@@ -1918,34 +1918,34 @@
 
         resp = self.invoke("DescribeSecurityGroup", d, **kwargs)
         return apis.DescribeSecurityGroupResponseSchema().loads(resp)
 
     def describe_security_group_resource(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeSecurityGroupResource - 查询安全组绑定的资源信息
+        """DescribeSecurityGroupResource - 查询安全组绑定的资源信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **SGID** (str) - (Required) 安全组ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **SGResourceInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回资源总个数。
-        
+
         **Response Model**
-        
-        **SGResourceInfo** 
-        
+
+        **SGResourceInfo**
+
         - **Name** (str) - 资源名称
         - **Region** (str) - 地域
         - **ResourceID** (str) - 资源ID
         - **ResourceType** (str) - 资源类型
         - **Zone** (str) - 可用区
 
         """
@@ -1958,35 +1958,35 @@
 
         resp = self.invoke("DescribeSecurityGroupResource", d, **kwargs)
         return apis.DescribeSecurityGroupResourceResponseSchema().loads(resp)
 
     def describe_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeSnapshot - 查询硬盘快照信息
+        """DescribeSnapshot - 查询硬盘快照信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **DiskID** (str) - 硬盘ID，输入“有效”状态的ID
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **SnapshotIDs** (list) - 【数组】快照ID，输入“有效”的ID。调用方式举例：SnapshotIDs.0=“one-id”、SnapshotIDs.1=“two-id”。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **SnapshotInfo** 模型定义
         - **Message** (str) - 返回信息描述
         - **TotalCount** (int) - 返回快照总个数
-        
+
         **Response Model**
-        
-        **SnapshotInfo** 
-        
+
+        **SnapshotInfo**
+
         - **CreateTime** (int) - 快照创建时间
         - **DiskID** (str) - 快照对应的硬盘 ID
         - **DiskType** (str) - 硬盘类型。枚举值：Boot，表示系统盘；Data，表示数据盘；
         - **Name** (str) - 快照名称
         - **Region** (str) - 地域。枚举值： cn，表示中国；
         - **Remark** (str) - 描述
         - **SnapshotID** (str) - 快照ID
@@ -2003,31 +2003,31 @@
 
         resp = self.invoke("DescribeSnapshot", d, **kwargs)
         return apis.DescribeSnapshotResponseSchema().loads(resp)
 
     def describe_storage_type(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeStorageType - 查询存储类型
+        """DescribeStorageType - 查询存储类型
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **StorageTypeInfo** 模型定义
         - **Message** (str) - 返回信息描述；
         - **TotalCount** (int) - 存储类型的总数
-        
+
         **Response Model**
-        
-        **StorageTypeInfo** 
-        
+
+        **StorageTypeInfo**
+
         - **Region** (str) - 地域
         - **SetArch** (str) - 架构
         - **StorageType** (str) - 存储类型
         - **StorageTypeAlias** (str) - 存储类型别名
         - **Zone** (str) - 可用区
 
         """
@@ -2040,35 +2040,35 @@
 
         resp = self.invoke("DescribeStorageType", d, **kwargs)
         return apis.DescribeStorageTypeResponseSchema().loads(resp)
 
     def describe_subnet(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeSubnet - 查询子网信息
+        """DescribeSubnet - 查询子网信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **Zone** (str) - (Required) 可用区。
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **SubnetIDs** (list) - 【数组】子网 ID。调用方式举例：SubnetIDs.0=“one-id”、SubnetIDs.1=“two-id”
         - **VPCID** (str) - VPCID
-        
+
         **Response**
 
         - **Infos** (list) - 见 **SubnetInfo** 模型定义
         - **Message** (str) - 返回信息描述；
         - **TotalCount** (int) - 子网的总数
-        
+
         **Response Model**
-        
-        **SubnetInfo** 
-        
+
+        **SubnetInfo**
+
         - **CreateTime** (int) - 创建时间，时间戳
         - **Name** (str) - 名称
         - **Network** (str) - 网段
         - **Region** (str) - 地域
         - **Remark** (str) - 描述
         - **State** (str) - 状态；Allocating：申请中,Available：有效,Deleting：删除中,Deleted：已删除
         - **SubnetID** (str) - ID
@@ -2085,32 +2085,32 @@
 
         resp = self.invoke("DescribeSubnet", d, **kwargs)
         return apis.DescribeSubnetResponseSchema().loads(resp)
 
     def describe_user(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUser - 查询租户信息
+        """DescribeUser - 查询租户信息
 
         **Request**
 
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **UserIDs** (list) - 【数组】租户的 ID。输入有效的 ID。调用方式举例：UserIDs.0=123”、UserIDs.1=456
-        
+
         **Response**
 
         - **Infos** (list) - 见 **UserInfo** 模型定义
         - **Message** (str) - 返回信息描述
         - **TotalCount** (int) - 返回现有租户总数
-        
+
         **Response Model**
-        
-        **UserInfo** 
-        
+
+        **UserInfo**
+
         - **Amount** (float) - 账户余额
         - **CreateTime** (int) - 账户创建时间。时间戳
         - **Email** (str) - 租户名称
         - **PrivateKey** (str) - 私钥
         - **PublicKey** (str) - 公钥
         - **Status** (str) - 用户状态。USER_STATUS_AVAILABLE：正常，USER_STATUS_FREEZE：冻结
         - **UpdateTime** (int) - 更新时间。时间戳
@@ -2124,60 +2124,60 @@
 
         resp = self.invoke("DescribeUser", d, **kwargs)
         return apis.DescribeUserResponseSchema().loads(resp)
 
     def describe_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeVMInstance - 查询虚拟机
+        """DescribeVMInstance - 查询虚拟机
 
         **Request**
 
         - **Region** (str) - (Config) 地域或数据中心。枚举值： cn，表示中国；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **SubnetID** (str) - 子网 ID。输入“有效”状态的子网 ID。
         - **VMIDs** (list) - 【数组】虚拟机的 ID。输入有效的 ID。调用方式举例：PrivateIp.0=“one-id”、PrivateIp.1=“two-id”。
         - **VPCID** (str) - VPC ID。输入“有效”状态的VPC ID。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **VMInstanceInfo** 模型定义
         - **Message** (str) - 返回信息描述
         - **TotalCount** (int) - 返回虚拟机总个数
-        
+
         **Response Model**
-        
-        **VMDiskInfo** 
-        
+
+        **VMDiskInfo**
+
         - **DiskID** (str) - 磁盘 ID
         - **Drive** (str) - 磁盘盘符
         - **IsElastic** (str) - 是否是弹性磁盘。枚举值为：Y，表示是；N，表示否；
         - **Name** (str) - 磁盘名称
         - **Size** (int) - 磁盘大小，单位 GB
         - **Type** (str) - 磁盘类型。枚举值：Boot，表示系统盘；Data，表示数据盘；
 
-        **VMIPInfo** 
-        
+        **VMIPInfo**
+
         - **IP** (str) - IP 值
         - **IPVersion** (str) - IP版本,支持值：IPv4\IPv6
         - **InterfaceID** (str) - 网卡 ID，IP 地址绑定的网卡 ID
         - **IsElastic** (str) - 是否是弹性网卡。枚举值：Y，表示是；N，表示否；
         - **MAC** (str) - MAC 地址值
         - **SGID** (str) - 安全组 ID
         - **SGName** (str) - 安全组名称
         - **SubnetID** (str) - 子网 ID，IP 为外网 IP 时为空；
         - **SubnetName** (str) - 子网名称，IP 为外网 IP 时为空；
         - **Type** (str) - IP 类型。枚举值：Private，表示内网；Public，表示外网。
         - **VPCID** (str) - VPC ID，IP 为外网 IP 时为空；
         - **VPCName** (str) - VPC 名称，IP 为外网 IP 时为空；
 
-        **VMInstanceInfo** 
-        
+        **VMInstanceInfo**
+
         - **CPU** (int) - CPU 个数
         - **ChargeType** (str) - 虚拟机计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **CreateTime** (int) - 虚拟机创建时间
         - **DiskInfos** (list) - 见 **VMDiskInfo** 模型定义
         - **ExpireTime** (int) - 虚拟机过期时间
         - **IPInfos** (list) - 见 **VMIPInfo** 模型定义
         - **ImageID** (str) - 镜像 ID
@@ -2207,31 +2207,31 @@
 
         resp = self.invoke("DescribeVMInstance", d, **kwargs)
         return apis.DescribeVMInstanceResponseSchema().loads(resp)
 
     def describe_vm_type(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeVMType - 查询主机机型
+        """DescribeVMType - 查询主机机型
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **VMTypeInfo** 模型定义
         - **Message** (str) - 返回信息描述；
         - **TotalCount** (int) - 主机机型的总数
-        
+
         **Response Model**
-        
-        **VMTypeInfo** 
-        
+
+        **VMTypeInfo**
+
         - **Region** (str) - 地域
         - **SetArch** (str) - 架构
         - **VMType** (str) - 机型
         - **VMTypeAlias** (str) - 机型别名
         - **Zone** (str) - 可用区
 
         """
@@ -2242,46 +2242,46 @@
         req and d.update(req)
         d = apis.DescribeVMTypeRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeVMType", d, **kwargs)
         return apis.DescribeVMTypeResponseSchema().loads(resp)
 
     def describe_vpc(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeVPC - 查询VPC信息
+        """DescribeVPC - 查询VPC信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **Zone** (str) - (Required) 可用区。
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **VPCIDs** (list) - 【数组】VPC的 ID。调用方式举例：VPCIDs.0=“one-id”、VPCIDs.1=“two-id”
-        
+
         **Response**
 
         - **Infos** (list) - 见 **VPCInfo** 模型定义
         - **Message** (str) - 返回信息描述；
         - **TotalCount** (int) - VPC的总数
-        
+
         **Response Model**
-        
-        **SubnetInfo** 
-        
+
+        **SubnetInfo**
+
         - **CreateTime** (int) - 创建时间，时间戳
         - **Name** (str) - 名称
         - **Network** (str) - 网段
         - **Region** (str) - 地域
         - **Remark** (str) - 描述
         - **State** (str) - 状态；Allocating：申请中,Available：有效,Deleting：删除中,Deleted：已删除
         - **SubnetID** (str) - ID
         - **UpdateTime** (int) - 更新时间，时间戳
         - **Zone** (str) - 可用区
 
-        **VPCInfo** 
-        
+        **VPCInfo**
+
         - **CreateTime** (int) - 创建时间，时间戳
         - **Name** (str) - 名称
         - **Network** (str) - 网段，比如10.0.0.0/16
         - **Region** (str) - 地域。
         - **Remark** (str) - 描述
         - **State** (str) - 状态；Allocating：申请中,Available：有效,Terminating：销毁中,Terminated：已销毁
         - **SubnetCount** (int) - 该VPC下拥有的子网数目
@@ -2298,62 +2298,62 @@
         req and d.update(req)
         d = apis.DescribeVPCRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeVPC", d, **kwargs)
         return apis.DescribeVPCResponseSchema().loads(resp)
 
     def describe_vs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeVS - 获取负载均衡 VServer 信息
+        """DescribeVS - 获取负载均衡 VServer 信息
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **VSIDs** (list) - 【数组】VServer的 ID。调用方式举例：VSIDs.0=“one-id”、VSIDs.1=“two-id”。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **VSInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回当前负载均衡 VServer 总个数。
-        
+
         **Response Model**
-        
-        **VSPolicyInfo** 
-        
+
+        **VSPolicyInfo**
+
         - **CreateTime** (int) - 创建时间，时间戳
         - **Domain** (str) - 内容转发规则关联的请求域名，值可为空，即代表仅匹配路径。
         - **LBID** (str) - 负载均衡ID
         - **Path** (str) - 内容转发规则关联的请求访问路径，如 "/" 。
         - **PolicyID** (str) - 内容转发规则ID
         - **PolicyStatus** (str) - 状态，枚举值，Available:有效,Deleted:已删除
         - **RSInfos** (list) - 见 **RSInfo** 模型定义
         - **UpdateTime** (int) - 更新时间，时间戳
         - **VSID** (str) - VServerID
 
-        **RSInfo** 
-        
+        **RSInfo**
+
         - **BindResourceID** (str) - 绑定的资源ID
         - **CreateTime** (int) - 创建时间，时间戳
         - **IP** (str) - 服务节点的内网 IP 地址
         - **LBID** (str) - 服务节点所属的负载均衡 ID
         - **Name** (str) - 服务节点的资源名称
         - **Port** (int) - 服务节点暴露的服务端口号
         - **RSID** (str) - 服务节点的 ID
         - **RSMode** (str) - 节点模式。枚举值，Enabling:开启中,Enable:已启用,Disabling:禁用中,Disable:已禁用
         - **RSStatus** (str) - RSStatus 的描述修改为：状态，枚举值，Creating:创建中,Inactive:无效,Active:有效,Updating:更新中,Deleting:删除中,Deleted:已删除。其中有效代表节点服务健康，无效代表节点服务异常。
         - **UpdateTime** (int) - 更新时间，时间戳
         - **VSID** (str) - 服务节点所属的 VServer ID
         - **Weight** (int) - 服务节点的权重
 
-        **VSInfo** 
-        
+        **VSInfo**
+
         - **AlarmTemplateID** (str) - 告警模板ID
         - **CACertificateID** (str) - CA证书ID，用于验证客户端证书的签名。仅当VServer监听协议为 HTTPS 且 SSLMode 为双向认证时有效。
         - **CreateTime** (int) - 创建时间，时间戳
         - **Domain** (str) - HTTP 健康检查时校验请求的 HOST 字段中的域名。当健康检查类型为端口检查时，该值为空。
         - **HealthcheckType** (str) - 负载均衡的健康检查类型。枚举值：Port:端口检查；Path: HTTP检查 。
         - **KeepaliveTimeout** (int) - 负载均衡的连接空闲超时时间，单位为秒，默认值为 60s 。当 VServer 协议为 UDP 时，该值为空。
         - **LBID** (str) - VServer 所属的负载均衡 ID
@@ -2382,51 +2382,51 @@
 
         resp = self.invoke("DescribeVS", d, **kwargs)
         return apis.DescribeVSResponseSchema().loads(resp)
 
     def describe_vs_policy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeVSPolicy - 获取七层负载均衡内容转发规则信息，仅当 VServer 的监听协议为 HTTP 时有效。
+        """DescribeVSPolicy - 获取七层负载均衡内容转发规则信息，仅当 VServer 的监听协议为 HTTP 时有效。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Limit** (int) - 返回数据长度，默认为20，最大100。
         - **Offset** (int) - 列表起始位置偏移量，默认为0。
         - **PolicyIDs** (list) - 【数组】七层负载均衡内容转发规则的 ID。调用方式举例：PolicyIDs.0=“one-id”、PolicyIDs.1=“two-id”
         - **VSID** (str) - VServerID
-        
+
         **Response**
 
         - **Infos** (list) - 见 **VSPolicyInfo** 模型定义
         - **Message** (str) - 返回信息描述。
         - **TotalCount** (int) - 返回内容转发规则的总个数。
-        
+
         **Response Model**
-        
-        **RSInfo** 
-        
+
+        **RSInfo**
+
         - **BindResourceID** (str) - 绑定的资源ID
         - **CreateTime** (int) - 创建时间，时间戳
         - **IP** (str) - 服务节点的内网 IP 地址
         - **LBID** (str) - 服务节点所属的负载均衡 ID
         - **Name** (str) - 服务节点的资源名称
         - **Port** (int) - 服务节点暴露的服务端口号
         - **RSID** (str) - 服务节点的 ID
         - **RSMode** (str) - 节点模式。枚举值，Enabling:开启中,Enable:已启用,Disabling:禁用中,Disable:已禁用
         - **RSStatus** (str) - RSStatus 的描述修改为：状态，枚举值，Creating:创建中,Inactive:无效,Active:有效,Updating:更新中,Deleting:删除中,Deleted:已删除。其中有效代表节点服务健康，无效代表节点服务异常。
         - **UpdateTime** (int) - 更新时间，时间戳
         - **VSID** (str) - 服务节点所属的 VServer ID
         - **Weight** (int) - 服务节点的权重
 
-        **VSPolicyInfo** 
-        
+        **VSPolicyInfo**
+
         - **CreateTime** (int) - 创建时间，时间戳
         - **Domain** (str) - 内容转发规则关联的请求域名，值可为空，即代表仅匹配路径。
         - **LBID** (str) - 负载均衡ID
         - **Path** (str) - 内容转发规则关联的请求访问路径，如 "/" 。
         - **PolicyID** (str) - 内容转发规则ID
         - **PolicyStatus** (str) - 状态，枚举值，Available:有效,Deleted:已删除
         - **RSInfos** (list) - 见 **RSInfo** 模型定义
@@ -2441,138 +2441,138 @@
         req and d.update(req)
         d = apis.DescribeVSPolicyRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeVSPolicy", d, **kwargs)
         return apis.DescribeVSPolicyResponseSchema().loads(resp)
 
     def detach_disk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DetachDisk - 解绑硬盘
+        """DetachDisk - 解绑硬盘
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **DiskID** (str) - (Required) 硬盘ID
         - **ResourceID** (str) - (Required) 绑定的资源ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DetachDiskRequestSchema().dumps(d)
 
         resp = self.invoke("DetachDisk", d, **kwargs)
         return apis.DetachDiskResponseSchema().loads(resp)
 
     def detach_nic(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DetachNIC - 解绑UClouStack网卡
+        """DetachNIC - 解绑UClouStack网卡
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **NICID** (str) - (Required) 网卡ID
         - **ResourceID** (str) - (Required) 绑定的资源ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DetachNICRequestSchema().dumps(d)
 
         resp = self.invoke("DetachNIC", d, **kwargs)
         return apis.DetachNICResponseSchema().loads(resp)
 
     def disable_rs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DisableRS - 禁用负载均衡的单个服务节点
+        """DisableRS - 禁用负载均衡的单个服务节点
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **RSID** (str) - (Required) RServer的ID
         - **VSID** (str) - (Required) VServer的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.DisableRSRequestSchema().dumps(d)
 
         resp = self.invoke("DisableRS", d, **kwargs)
         return apis.DisableRSResponseSchema().loads(resp)
 
     def enable_rs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ EnableRS - 启用负载均衡的单个服务节点
+        """EnableRS - 启用负载均衡的单个服务节点
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **RSID** (str) - (Required) RServer的ID
         - **VSID** (str) - (Required) VServer的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.EnableRSRequestSchema().dumps(d)
 
         resp = self.invoke("EnableRS", d, **kwargs)
         return apis.EnableRSResponseSchema().loads(resp)
 
     def get_disk_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetDiskPrice - 获取硬盘价格
+        """GetDiskPrice - 获取硬盘价格
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **DiskSpace** (int) - (Required) 磁盘大小
         - **SetType** (str) - (Required) 磁盘类型
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **PriceInfo** 模型定义
         - **Message** (str) - 返回信息描述。
-        
+
         **Response Model**
-        
-        **PriceInfo** 
-        
+
+        **PriceInfo**
+
         - **ChargeType** (str) - 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **Price** (float) - 价格
 
         """
         # build request
         d = {
             "Region": self.config.region,
@@ -2582,34 +2582,34 @@
 
         resp = self.invoke("GetDiskPrice", d, **kwargs)
         return apis.GetDiskPriceResponseSchema().loads(resp)
 
     def get_eip_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetEIPPrice - 获取外网IP价格
+        """GetEIPPrice - 获取外网IP价格
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **Bandwidth** (int) - (Required) 带宽，默认值1，默认范围1~100
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **OpertatorName** (str) - (Required) 线路。目前支持Bgp
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **PriceInfo** 模型定义
         - **Message** (str) - 返回信息描述
-        
+
         **Response Model**
-        
-        **PriceInfo** 
-        
+
+        **PriceInfo**
+
         - **ChargeType** (str) - 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **Price** (float) - 价格
 
         """
         # build request
         d = {
             "Region": self.config.region,
@@ -2619,15 +2619,15 @@
 
         resp = self.invoke("GetEIPPrice", d, **kwargs)
         return apis.GetEIPPriceResponseSchema().loads(resp)
 
     def get_vm_instance_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetVMInstancePrice - 获取虚拟机价格
+        """GetVMInstancePrice - 获取虚拟机价格
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **BootDiskSetType** (str) - (Required) 系统盘类型。枚举值：Normal，表示普通；SSD，表示SSD；
         - **CPU** (int) - (Required) CPU 个数，目前只能输入数据库配置指定规格参数，如：1核2048M、2核4096M、4核8192M、8核16384M、16核32768M。
         - **ChargeType** (str) - (Required) 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
@@ -2636,24 +2636,24 @@
         - **ImageID** (str) - (Required) 镜像 ID。基础镜像 ID 或者自制镜像 ID。如：cn-image-centos-74。
         - **Memory** (int) - (Required) 内存大小，单位 M。目前只能输入数据库配置指定规格参数，如：1核2048M、2核4096M、4核8192M、8核16384M、16核32768M。
         - **OSType** (str) - (Required) 系统类型。
         - **VMType** (str) - (Required) 机型。枚举值：Normal，表示普通；SSD，表示SSD；
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **GPU** (int) - GPU 卡核心的占用个数。枚举值：【1,2,4】。GPU与CPU、内存大小关系：CPU个数>=4*GPU个数，同时内存与CPU规格匹配.
         - **Quantity** (int) - 购买时长。默认值1。小时不生效，月范围【1，11】，年范围【1，5】。
-        
+
         **Response**
 
         - **Infos** (list) - 见 **PriceInfo** 模型定义
         - **Message** (str) - 返回信息描述。
-        
+
         **Response Model**
-        
-        **PriceInfo** 
-        
+
+        **PriceInfo**
+
         - **ChargeType** (str) - 计费模式。枚举值：Dynamic，表示小时；Month，表示月；Year，表示年；
         - **Price** (float) - 价格
 
         """
         # build request
         d = {
             "Region": self.config.region,
@@ -2663,606 +2663,606 @@
 
         resp = self.invoke("GetVMInstancePrice", d, **kwargs)
         return apis.GetVMInstancePriceResponseSchema().loads(resp)
 
     def modify_eip_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyEIPBandwidth - 调整外网IP带宽
+        """ModifyEIPBandwidth - 调整外网IP带宽
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **Bandwidth** (int) - (Required) 调整后的带宽
         - **EIPID** (str) - (Required) 外网IP的ID
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.ModifyEIPBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyEIPBandwidth", d, **kwargs)
         return apis.ModifyEIPBandwidthResponseSchema().loads(resp)
 
     def modify_name_and_remark(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyNameAndRemark - 修改资源名称和备注
+        """ModifyNameAndRemark - 修改资源名称和备注
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Name** (str) - (Required) 名称;
         - **ResourceID** (str) - (Required) 资源ID;
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Remark** (str) - 描述;
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.ModifyNameAndRemarkRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyNameAndRemark", d, **kwargs)
         return apis.ModifyNameAndRemarkResponseSchema().loads(resp)
 
     def poweroff_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ PoweroffVMInstance - 断电虚拟机，可能导致丢失数据甚至损坏操作系统，仅适用于虚拟机死机及级端测试场景。
+        """PoweroffVMInstance - 断电虚拟机，可能导致丢失数据甚至损坏操作系统，仅适用于虚拟机死机及级端测试场景。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：如 cn,表示中国。
         - **VMID** (str) - (Required) 虚拟机ID
         - **Zone** (str) - (Required) 可用区。枚举值：如 zone-01，表示可用区1。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.PoweroffVMInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("PoweroffVMInstance", d, **kwargs)
         return apis.PoweroffVMInstanceResponseSchema().loads(resp)
 
     def recharge(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ Recharge - 管理员给租户充值
+        """Recharge - 管理员给租户充值
 
         **Request**
 
         - **Amount** (int) - (Required) 充值金额。最少100,最大500000
         - **FromType** (str) - (Required) 充值来源。INPOUR_FROM_ALIPAY：支付宝，INPOUR_FROM_OFFLINE：银行转账，INPOUR_FROM_SINPAY：新浪支付，INPOUR_FROM_WECHAT_PAY：微信转账。
         - **SerialNo** (str) - (Required) 充值单号。充值方式为“账户余额”时为必要参数。
         - **UserID** (int) - (Required) 租户的账户ID。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {}
         req and d.update(req)
         d = apis.RechargeRequestSchema().dumps(d)
 
         resp = self.invoke("Recharge", d, **kwargs)
         return apis.RechargeResponseSchema().loads(resp)
 
     def reinstall_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ReinstallVMInstance - 重装系统，关机的虚拟机才可以重装系统
+        """ReinstallVMInstance - 重装系统，关机的虚拟机才可以重装系统
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **ImageID** (str) - (Required) 镜像ID
         - **VMID** (str) - (Required) 虚拟机ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.ReinstallVMInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("ReinstallVMInstance", d, **kwargs)
         return apis.ReinstallVMInstanceResponseSchema().loads(resp)
 
     def release_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ ReleaseEIP - 删除外网IP
+        """ReleaseEIP - 删除外网IP
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；中国
         - **EIPID** (str) - (Required) 外网IP的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国
-        
+
         **Response**
 
         - **Message** (str) - 返回状态描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.ReleaseEIPRequestSchema().dumps(d)
 
         resp = self.invoke("ReleaseEIP", d, **kwargs)
         return apis.ReleaseEIPResponseSchema().loads(resp)
 
     def renew_resource(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RenewResource - 续费回收站资源
+        """RenewResource - 续费回收站资源
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：如 cn,表示中国。
         - **ResourceID** (str) - (Required) 待续续的资源ID
         - **Zone** (str) - (Required) 可用区。枚举值：如 zone-01，表示可用区1。
         - **Quantity** (int) - 购买时长，默认为 1。按小时(Dynamic)付费的资源无需此参数，按月付费的资源传 0 时，代表购买至月末。
-        
+
         **Response**
 
         - **Message** (str) - 返回描述信息
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.RenewResourceRequestSchema().dumps(d)
 
         resp = self.invoke("RenewResource", d, **kwargs)
         return apis.RenewResourceResponseSchema().loads(resp)
 
     def reset_vm_instance_password(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResetVMInstancePassword - 重置虚拟机密码，主机必须开机才可以重置密码
+        """ResetVMInstancePassword - 重置虚拟机密码，主机必须开机才可以重置密码
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Password** (str) - (Required) 密码
         - **VMID** (str) - (Required) 虚拟机ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.ResetVMInstancePasswordRequestSchema().dumps(d)
 
         resp = self.invoke("ResetVMInstancePassword", d, **kwargs)
         return apis.ResetVMInstancePasswordResponseSchema().loads(resp)
 
     def resize_vm_config(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeVMConfig - 修改虚拟机配置
+        """ResizeVMConfig - 修改虚拟机配置
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **CPU** (int) - (Required) CPU 个数，如 1、2、4、8、16、32、64。
         - **Memory** (int) - (Required) 内存容量，如 2048、4096、8192、16384、32768、65536、131072。
         - **VMID** (str) - (Required) 虚拟机ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.ResizeVMConfigRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeVMConfig", d, **kwargs)
         return apis.ResizeVMConfigResponseSchema().loads(resp)
 
     def restart_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RestartVMInstance - 重启虚拟机
+        """RestartVMInstance - 重启虚拟机
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **VMID** (str) - (Required) 虚拟机ID;
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.RestartVMInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("RestartVMInstance", d, **kwargs)
         return apis.RestartVMInstanceResponseSchema().loads(resp)
 
     def rollback_resource(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RollbackResource - 恢复回收站资源
+        """RollbackResource - 恢复回收站资源
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：如 cn,表示中国。
         - **ResourceID** (str) - (Required) 待恢复的资源ID
         - **Zone** (str) - (Required) 可用区。枚举值：如 zone-01，表示可用区1。
-        
+
         **Response**
 
         - **Message** (str) - 返回描述信息
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.RollbackResourceRequestSchema().dumps(d)
 
         resp = self.invoke("RollbackResource", d, **kwargs)
         return apis.RollbackResourceResponseSchema().loads(resp)
 
     def rollback_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RollbackSnapshot - 将某个快照内的数据回滚到原云硬盘，仅支持正常状态的快照进行回滚操作，回滚时硬盘必须处于未绑定或其挂载的主机为关机状态。
+        """RollbackSnapshot - 将某个快照内的数据回滚到原云硬盘，仅支持正常状态的快照进行回滚操作，回滚时硬盘必须处于未绑定或其挂载的主机为关机状态。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：如 cn,表示中国。
         - **DiskID** (str) - (Required) 对应的云硬盘 ID；
         - **SnapshotID** (str) - (Required) 快照ID
         - **Zone** (str) - (Required) 可用区。枚举值：如 zone-01，表示可用区1。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.RollbackSnapshotRequestSchema().dumps(d)
 
         resp = self.invoke("RollbackSnapshot", d, **kwargs)
         return apis.RollbackSnapshotResponseSchema().loads(resp)
 
     def start_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ StartVMInstance - 开启虚拟机
+        """StartVMInstance - 开启虚拟机
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn，表示中国；
         - **VMID** (str) - (Required) 虚拟机 ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.StartVMInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("StartVMInstance", d, **kwargs)
         return apis.StartVMInstanceResponseSchema().loads(resp)
 
     def stop_vm_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ StopVMInstance - 关闭虚拟机
+        """StopVMInstance - 关闭虚拟机
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn，表示中国；
         - **VMID** (str) - (Required) 虚拟机 ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
         - **VMID** (str) - 虚拟机 ID
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.StopVMInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("StopVMInstance", d, **kwargs)
         return apis.StopVMInstanceResponseSchema().loads(resp)
 
     def terminate_resource(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ TerminateResource - 销毁资源
+        """TerminateResource - 销毁资源
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **ResourceID** (str) - (Required) 资源id
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回描述信息
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.TerminateResourceRequestSchema().dumps(d)
 
         resp = self.invoke("TerminateResource", d, **kwargs)
         return apis.TerminateResourceResponseSchema().loads(resp)
 
     def un_bind_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ UnBindEIP - 解绑外网IP
+        """UnBindEIP - 解绑外网IP
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；中国
         - **EIPID** (str) - (Required) 外网IP的ID
         - **ResourceID** (str) - (Required) 资源ID
         - **ResourceType** (str) - (Required) 资源类型。VM：虚拟机, LB:负载均衡, NATGW：nat网关
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UnBindEIPRequestSchema().dumps(d)
 
         resp = self.invoke("UnBindEIP", d, **kwargs)
         return apis.UnBindEIPResponseSchema().loads(resp)
 
     def un_bind_security_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UnBindSecurityGroup - 解绑安全组
+        """UnBindSecurityGroup - 解绑安全组
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **ResourceID** (str) - (Required) 解绑的资源ID。调用方式举例：ResourceID=“one-id”。
         - **SGID** (str) - (Required) 安全组ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UnBindSecurityGroupRequestSchema().dumps(d)
 
         resp = self.invoke("UnBindSecurityGroup", d, **kwargs)
         return apis.UnBindSecurityGroupResponseSchema().loads(resp)
 
     def unbind_alarm_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UnbindAlarmTemplate - 解绑告警模板
+        """UnbindAlarmTemplate - 解绑告警模板
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **AlarmTemplateID** (str) - (Required) 告警模板ID
         - **ResourceIDs** (list) - (Required) 【数组】资源的 ID。调用方式举例：ResourceIDs.0=“one-id”、ResourceIDs.1=“two-id”。
         - **ResourceType** (str) - (Required) 资源类型。VM：虚拟机, LB:负载均衡, NATGW：nat网关;EIP:弹性网卡
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UnbindAlarmTemplateRequestSchema().dumps(d)
 
         resp = self.invoke("UnbindAlarmTemplate", d, **kwargs)
         return apis.UnbindAlarmTemplateResponseSchema().loads(resp)
 
     def unbind_physical_ip(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UnbindPhysicalIP - 解绑物理IP
+        """UnbindPhysicalIP - 解绑物理IP
 
         **Request**
 
         - **Region** (str) - (Config) 地域。
         - **PhysicalIPID** (str) - (Required) 物理IP的ID
         - **ResourceID** (str) - (Required) 资源ID
         - **ResourceType** (str) - (Required) 资源类型。VM：虚拟机
         - **Zone** (str) - (Required) 可用区。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UnbindPhysicalIPRequestSchema().dumps(d)
 
         resp = self.invoke("UnbindPhysicalIP", d, **kwargs)
         return apis.UnbindPhysicalIPResponseSchema().loads(resp)
 
     def update_alarm_template_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateAlarmTemplateRule - 更新告警模板规则
+        """UpdateAlarmTemplateRule - 更新告警模板规则
 
         **Request**
 
         - **Region** (str) - (Config) 地域
         - **AlarmStrategy** (str) - (Required) 瘦脸策略
         - **AlarmTemplateID** (str) - (Required) 告警模板ID
         - **AlarmTemplateRuleID** (str) - (Required) 告警规则ID
         - **Compare** (str) - (Required) 对比方式
         - **ContactGroupID** (str) - (Required) 通知组ID
         - **MetricName** (str) - (Required) 监控指标名称
         - **ResourceType** (str) - (Required) 资源类型
         - **Threshold** (str) - (Required) 告警阈值
         - **TriggerCount** (str) - (Required) 连续触发次数
         - **Zone** (str) - (Required) 可用区
-        
+
         **Response**
 
         - **Message** (str) - 返回描述信息
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UpdateAlarmTemplateRuleRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateAlarmTemplateRule", d, **kwargs)
         return apis.UpdateAlarmTemplateRuleResponseSchema().loads(resp)
 
     def update_rs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ UpdateRS - 修改负载均衡的服务节点
+        """UpdateRS - 修改负载均衡的服务节点
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) VServer 监听器所属的负载均衡 ID
         - **RSID** (str) - (Required) RServer的ID
         - **VSID** (str) - (Required) RServer所属的VServer的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Port** (int) - 端口号
         - **Weight** (int) - 权重
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UpdateRSRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateRS", d, **kwargs)
         return apis.UpdateRSResponseSchema().loads(resp)
 
     def update_security_group_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateSecurityGroupRule - 修改安全组规则
+        """UpdateSecurityGroupRule - 修改安全组规则
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值： cn，表示中国；
         - **Rules** (list) - (Required) 【数组】规则。输入有效的 规则。调用方式举例：Rules.0=“TCP|23|0.0.0.0/0|ACCEPT|HIGH|1|sg_rule-wefvg34f”、Rules.1=“TCP|55|0.0.0.0/0|ACCEPT|HIGH|1|sg_rule-wefvggf”
         - **SGID** (str) - (Required) 安全组ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述；
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UpdateSecurityGroupRuleRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateSecurityGroupRule", d, **kwargs)
         return apis.UpdateSecurityGroupRuleResponseSchema().loads(resp)
 
     def update_vs(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ UpdateVS - 修改负载均衡VServer
+        """UpdateVS - 修改负载均衡VServer
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) VServer 监听器所属的负载均衡 ID
         - **VSID** (str) - (Required) 需要更新的VSID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
@@ -3273,77 +3273,77 @@
         - **Path** (str) - HTTP 健康检查的路径，健康检查类型为 HTTP 检查时为必填项。当健康检查类型为端口检查时，该值为空。
         - **PersistenceKey** (str) - 会话保持KEY，会话保持类型为Manual时为必填项，仅当 VServer 协议为 HTTP 时有效。
         - **PersistenceType** (str) - 会话保持类型。枚举值：None:关闭；Auto:自动生成；Manual:手动生成 。当协议为 TCP 时，该值不生效，会话保持和选择的调度算法相关；当协议为 UDP 时 Auto 表示开启会话保持 。
         - **Port** (int) - VServer 监听端口
         - **SSLMode** (str) - SSL认证模式,HTTPS协议下必传,取值范围["simplex","duplex"]分别表示单向认证和双向认证。
         - **Scheduler** (str) - 负载均衡的调度算法。枚举值：wrr:加权轮训；least_conn:最小连接数；hash:原地址,四层lb使用。ip_hash:七层lb使用
         - **ServerCertificateID** (str) - 服务器证书ID，用于证明服务器的身份，仅当 VServer监听协议为 HTTPS 时有效。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UpdateVSRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateVS", d, **kwargs)
         return apis.UpdateVSResponseSchema().loads(resp)
 
     def update_vs_policy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateVSPolicy - 更新七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
+        """UpdateVSPolicy - 更新七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **LBID** (str) - (Required) 负载均衡ID
         - **PolicyID** (str) - (Required) 内容转发规则ID
         - **VSID** (str) - (Required) VServer的ID
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
         - **Domain** (str) - 内容转发规则关联的请求域名，值可为空，即代表仅匹配路径。
         - **Path** (str) - 内容转发规则关联的请求访问路径，如 "/" 。
         - **RSIDs** (list) - 【数组】RServer的 ID。调用方式举例：RSIDs.0=“one-id”、RSIDs.1=“two-id”。
-        
+
         **Response**
 
         - **Message** (str) - 返回信息描述。
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UpdateVSPolicyRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateVSPolicy", d, **kwargs)
         return apis.UpdateVSPolicyResponseSchema().loads(resp)
 
     def upgrade_disk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ UpgradeDisk - 扩容硬盘，为保证数据完整性，容量扩容前建议暂停对当前硬盘的所有文件系统读写操作，并进入操作系统进行 `umount ` 或`脱机` 操作。
+        """UpgradeDisk - 扩容硬盘，为保证数据完整性，容量扩容前建议暂停对当前硬盘的所有文件系统读写操作，并进入操作系统进行 `umount ` 或`脱机` 操作。
 
         **Request**
 
         - **Region** (str) - (Config) 地域。枚举值：cn,表示中国；
         - **DiskID** (str) - (Required) 硬盘ID
         - **DiskSpace** (int) - (Required) 硬盘升级后的容量， 不能小于原硬盘容量，单位为 GB 。
         - **Zone** (str) - (Required) 可用区。枚举值：zone-01，表示中国；
-        
+
         **Response**
 
         - **Action** (str) - 操作名称
         - **Message** (str) - 返回信息描述。
         - **RetCode** (int) - 返回码
-        
+
         """
         # build request
         d = {
             "Region": self.config.region,
         }
         req and d.update(req)
         d = apis.UpgradeDiskRequestSchema().dumps(d)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/schemas/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: AllocateEIP
 
 申请外网IP
 """
 
 
 class AllocateEIPRequestSchema(schema.RequestSchema):
-    """ AllocateEIP - 申请外网IP
-    """
+    """AllocateEIP - 申请外网IP"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "IP": fields.Str(required=False, dump_to="IP"),
         "IPVersion": fields.Str(required=False, dump_to="IPVersion"),
         "Name": fields.Str(required=True, dump_to="Name"),
@@ -29,16 +28,15 @@
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class AllocateEIPResponseSchema(schema.ResponseSchema):
-    """ AllocateEIP - 申请外网IP
-    """
+    """AllocateEIP - 申请外网IP"""
 
     fields = {
         "EIPID": fields.Str(required=True, load_from="EIPID"),
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
@@ -46,203 +44,189 @@
 API: AttachDisk
 
 绑定硬盘
 """
 
 
 class AttachDiskRequestSchema(schema.RequestSchema):
-    """ AttachDisk - 绑定硬盘
-    """
+    """AttachDisk - 绑定硬盘"""
 
     fields = {
         "DiskID": fields.Str(required=True, dump_to="DiskID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class AttachDiskResponseSchema(schema.ResponseSchema):
-    """ AttachDisk - 绑定硬盘
-    """
+    """AttachDisk - 绑定硬盘"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: AttachNIC
 
 绑定UCloudStack网卡
 """
 
 
 class AttachNICRequestSchema(schema.RequestSchema):
-    """ AttachNIC - 绑定UCloudStack网卡
-    """
+    """AttachNIC - 绑定UCloudStack网卡"""
 
     fields = {
         "NICID": fields.Str(required=True, dump_to="NICID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class AttachNICResponseSchema(schema.ResponseSchema):
-    """ AttachNIC - 绑定UCloudStack网卡
-    """
+    """AttachNIC - 绑定UCloudStack网卡"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: BindAlarmTemplate
 
 绑定告警模板
 """
 
 
 class BindAlarmTemplateRequestSchema(schema.RequestSchema):
-    """ BindAlarmTemplate - 绑定告警模板
-    """
+    """BindAlarmTemplate - 绑定告警模板"""
 
     fields = {
         "AlarmTemplateID": fields.Str(required=True, dump_to="AlarmTemplateID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceIDs": fields.List(fields.Str()),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class BindAlarmTemplateResponseSchema(schema.ResponseSchema):
-    """ BindAlarmTemplate - 绑定告警模板
-    """
+    """BindAlarmTemplate - 绑定告警模板"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: BindEIP
 
 绑定外网 IP
 """
 
 
 class BindEIPRequestSchema(schema.RequestSchema):
-    """ BindEIP - 绑定外网 IP
-    """
+    """BindEIP - 绑定外网 IP"""
 
     fields = {
         "EIPID": fields.Str(required=True, dump_to="EIPID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class BindEIPResponseSchema(schema.ResponseSchema):
-    """ BindEIP - 绑定外网 IP
-    """
+    """BindEIP - 绑定外网 IP"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: BindPhysicalIP
 
 绑定物理 IP ，被绑定的资源必须处于运行中或有效状态。
 """
 
 
 class BindPhysicalIPRequestSchema(schema.RequestSchema):
-    """ BindPhysicalIP - 绑定物理 IP ，被绑定的资源必须处于运行中或有效状态。
-    """
+    """BindPhysicalIP - 绑定物理 IP ，被绑定的资源必须处于运行中或有效状态。"""
 
     fields = {
         "PhysicalIPID": fields.Str(required=True, dump_to="PhysicalIPID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class BindPhysicalIPResponseSchema(schema.ResponseSchema):
-    """ BindPhysicalIP - 绑定物理 IP ，被绑定的资源必须处于运行中或有效状态。
-    """
+    """BindPhysicalIP - 绑定物理 IP ，被绑定的资源必须处于运行中或有效状态。"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: BindSecurityGroup
 
 绑定安全组
 """
 
 
 class BindSecurityGroupRequestSchema(schema.RequestSchema):
-    """ BindSecurityGroup - 绑定安全组
-    """
+    """BindSecurityGroup - 绑定安全组"""
 
     fields = {
         "NICType": fields.Str(required=False, dump_to="NICType"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "SGID": fields.Str(required=True, dump_to="SGID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class BindSecurityGroupResponseSchema(schema.ResponseSchema):
-    """ BindSecurityGroup - 绑定安全组
-    """
+    """BindSecurityGroup - 绑定安全组"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: CloneDisk
 
 克隆硬盘
 """
 
 
 class CloneDiskRequestSchema(schema.RequestSchema):
-    """ CloneDisk - 克隆硬盘
-    """
+    """CloneDisk - 克隆硬盘"""
 
     fields = {
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SrcID": fields.Str(required=True, dump_to="SrcID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CloneDiskResponseSchema(schema.ResponseSchema):
-    """ CloneDisk - 克隆硬盘
-    """
+    """CloneDisk - 克隆硬盘"""
 
     fields = {
         "DiskID": fields.Str(required=True, load_from="DiskID"),
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
@@ -250,31 +234,29 @@
 API: CreateCertificate
 
 创建证书
 """
 
 
 class CreateCertificateRequestSchema(schema.RequestSchema):
-    """ CreateCertificate - 创建证书
-    """
+    """CreateCertificate - 创建证书"""
 
     fields = {
         "Certificate": fields.Str(required=True, dump_to="Certificate"),
         "CertificateType": fields.Str(required=True, dump_to="CertificateType"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "PrivateKey": fields.Str(required=False, dump_to="PrivateKey"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateCertificateResponseSchema(schema.ResponseSchema):
-    """ CreateCertificate - 创建证书
-    """
+    """CreateCertificate - 创建证书"""
 
     fields = {
         "CertificateID": fields.Str(required=True, load_from="CertificateID"),
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
@@ -282,31 +264,29 @@
 API: CreateCustomImage
 
 创建自制镜像
 """
 
 
 class CreateCustomImageRequestSchema(schema.RequestSchema):
-    """ CreateCustomImage - 创建自制镜像
-    """
+    """CreateCustomImage - 创建自制镜像"""
 
     fields = {
         "ImageDescription": fields.Str(
             required=False, dump_to="ImageDescription"
         ),
         "ImageName": fields.Str(required=True, dump_to="ImageName"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateCustomImageResponseSchema(schema.ResponseSchema):
-    """ CreateCustomImage - 创建自制镜像
-    """
+    """CreateCustomImage - 创建自制镜像"""
 
     fields = {
         "ImageID": fields.Str(required=True, load_from="ImageID"),
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
@@ -314,31 +294,29 @@
 API: CreateDisk
 
 创建硬盘
 """
 
 
 class CreateDiskRequestSchema(schema.RequestSchema):
-    """ CreateDisk - 创建硬盘
-    """
+    """CreateDisk - 创建硬盘"""
 
     fields = {
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SetType": fields.Str(required=True, dump_to="SetType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateDiskResponseSchema(schema.ResponseSchema):
-    """ CreateDisk - 创建硬盘
-    """
+    """CreateDisk - 创建硬盘"""
 
     fields = {
         "DiskID": fields.Str(required=True, load_from="DiskID"),
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
@@ -346,16 +324,15 @@
 API: CreateLB
 
 创建负载均衡
 """
 
 
 class CreateLBRequestSchema(schema.RequestSchema):
-    """ CreateLB - 创建负载均衡
-    """
+    """CreateLB - 创建负载均衡"""
 
     fields = {
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "EIPID": fields.Str(required=False, dump_to="EIPID"),
         "LBType": fields.Str(required=True, dump_to="LBType"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
@@ -366,16 +343,15 @@
         "VMType": fields.Str(required=True, dump_to="VMType"),
         "VPCID": fields.Str(required=True, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateLBResponseSchema(schema.ResponseSchema):
-    """ CreateLB - 创建负载均衡
-    """
+    """CreateLB - 创建负载均衡"""
 
     fields = {
         "LBID": fields.Str(required=False, load_from="LBID"),
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
@@ -383,16 +359,15 @@
 API: CreateNATGW
 
 创建NAT网关
 """
 
 
 class CreateNATGWRequestSchema(schema.RequestSchema):
-    """ CreateNATGW - 创建NAT网关
-    """
+    """CreateNATGW - 创建NAT网关"""
 
     fields = {
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "EIPID": fields.Str(required=True, dump_to="EIPID"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
@@ -402,16 +377,15 @@
         "VMType": fields.Str(required=True, dump_to="VMType"),
         "VPCID": fields.Str(required=True, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateNATGWResponseSchema(schema.ResponseSchema):
-    """ CreateNATGW - 创建NAT网关
-    """
+    """CreateNATGW - 创建NAT网关"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
         "NATGWID": fields.Str(required=False, load_from="NATGWID"),
     }
 
 
@@ -419,29 +393,27 @@
 API: CreateNATGWRule
 
 添加NAT网关白名单
 """
 
 
 class CreateNATGWRuleRequestSchema(schema.RequestSchema):
-    """ CreateNATGWRule - 添加NAT网关白名单
-    """
+    """CreateNATGWRule - 添加NAT网关白名单"""
 
     fields = {
         "BindResourceID": fields.Str(required=True, dump_to="BindResourceID"),
         "NATGWID": fields.Str(required=True, dump_to="NATGWID"),
         "NATGWType": fields.Str(required=True, dump_to="NATGWType"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateNATGWRuleResponseSchema(schema.ResponseSchema):
-    """ CreateNATGWRule - 添加NAT网关白名单
-    """
+    """CreateNATGWRule - 添加NAT网关白名单"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "RuleID": fields.Str(required=False, load_from="RuleID"),
     }
 
 
@@ -449,31 +421,29 @@
 API: CreateNIC
 
 创建网卡
 """
 
 
 class CreateNICRequestSchema(schema.RequestSchema):
-    """ CreateNIC - 创建网卡
-    """
+    """CreateNIC - 创建网卡"""
 
     fields = {
         "IP": fields.Str(required=False, dump_to="IP"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SGID": fields.Str(required=False, dump_to="SGID"),
         "SubnetID": fields.Str(required=True, dump_to="SubnetID"),
         "VPCID": fields.Str(required=True, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateNICResponseSchema(schema.ResponseSchema):
-    """ CreateNIC - 创建网卡
-    """
+    """CreateNIC - 创建网卡"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "NICID": fields.Str(required=True, load_from="NICID"),
     }
 
 
@@ -481,29 +451,27 @@
 API: CreatePhysicalIP
 
 创建物理 IP ，需确保平台已配置物理 IP 线路相关信息及物理网络联通性。
 """
 
 
 class CreatePhysicalIPRequestSchema(schema.RequestSchema):
-    """ CreatePhysicalIP - 创建物理 IP ，需确保平台已配置物理 IP 线路相关信息及物理网络联通性。
-    """
+    """CreatePhysicalIP - 创建物理 IP ，需确保平台已配置物理 IP 线路相关信息及物理网络联通性。"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "OperatorName": fields.Str(required=True, dump_to="OperatorName"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreatePhysicalIPResponseSchema(schema.ResponseSchema):
-    """ CreatePhysicalIP - 创建物理 IP ，需确保平台已配置物理 IP 线路相关信息及物理网络联通性。
-    """
+    """CreatePhysicalIP - 创建物理 IP ，需确保平台已配置物理 IP 线路相关信息及物理网络联通性。"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
         "PhysicalIPID": fields.Str(required=True, load_from="PhysicalIPID"),
     }
 
 
@@ -511,31 +479,29 @@
 API: CreateRS
 
 为负载均衡的 VServer 添加后端服务节点。
 """
 
 
 class CreateRSRequestSchema(schema.RequestSchema):
-    """ CreateRS - 为负载均衡的 VServer 添加后端服务节点。
-    """
+    """CreateRS - 为负载均衡的 VServer 添加后端服务节点。"""
 
     fields = {
         "BindResourceID": fields.Str(required=True, dump_to="BindResourceID"),
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Port": fields.Int(required=True, dump_to="Port"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Weight": fields.Int(required=True, dump_to="Weight"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateRSResponseSchema(schema.ResponseSchema):
-    """ CreateRS - 为负载均衡的 VServer 添加后端服务节点。
-    """
+    """CreateRS - 为负载均衡的 VServer 添加后端服务节点。"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
         "RSID": fields.Str(required=False, load_from="RSID"),
     }
 
 
@@ -543,29 +509,27 @@
 API: CreateSecurityGroup
 
 创建安全组
 """
 
 
 class CreateSecurityGroupRequestSchema(schema.RequestSchema):
-    """ CreateSecurityGroup - 创建安全组
-    """
+    """CreateSecurityGroup - 创建安全组"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Rule": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateSecurityGroupResponseSchema(schema.ResponseSchema):
-    """ CreateSecurityGroup - 创建安全组
-    """
+    """CreateSecurityGroup - 创建安全组"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "SGID": fields.Str(required=False, load_from="SGID"),
     }
 
 
@@ -573,28 +537,26 @@
 API: CreateSecurityGroupRule
 
 创建安全组规则
 """
 
 
 class CreateSecurityGroupRuleRequestSchema(schema.RequestSchema):
-    """ CreateSecurityGroupRule - 创建安全组规则
-    """
+    """CreateSecurityGroupRule - 创建安全组规则"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "Rules": fields.List(fields.Str()),
         "SGID": fields.Str(required=True, dump_to="SGID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateSecurityGroupRuleResponseSchema(schema.ResponseSchema):
-    """ CreateSecurityGroupRule - 创建安全组规则
-    """
+    """CreateSecurityGroupRule - 创建安全组规则"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "SGRuleID": fields.Str(required=False, load_from="SGRuleID"),
     }
 
 
@@ -602,29 +564,27 @@
 API: CreateSnapshot
 
 创建硬盘快照
 """
 
 
 class CreateSnapshotRequestSchema(schema.RequestSchema):
-    """ CreateSnapshot - 创建硬盘快照
-    """
+    """CreateSnapshot - 创建硬盘快照"""
 
     fields = {
         "DiskID": fields.Str(required=True, dump_to="DiskID"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateSnapshotResponseSchema(schema.ResponseSchema):
-    """ CreateSnapshot - 创建硬盘快照
-    """
+    """CreateSnapshot - 创建硬盘快照"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "SnapshotID": fields.Str(required=True, load_from="SnapshotID"),
     }
 
 
@@ -632,30 +592,28 @@
 API: CreateSubnet
 
 创建子网
 """
 
 
 class CreateSubnetRequestSchema(schema.RequestSchema):
-    """ CreateSubnet - 创建子网
-    """
+    """CreateSubnet - 创建子网"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "Network": fields.Str(required=True, dump_to="Network"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "VPCID": fields.Str(required=True, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateSubnetResponseSchema(schema.ResponseSchema):
-    """ CreateSubnet - 创建子网
-    """
+    """CreateSubnet - 创建子网"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "SubnetID": fields.Str(required=False, load_from="SubnetID"),
     }
 
 
@@ -663,26 +621,24 @@
 API: CreateUser
 
 管理员添加账号
 """
 
 
 class CreateUserRequestSchema(schema.RequestSchema):
-    """ CreateUser - 管理员添加账号
-    """
+    """CreateUser - 管理员添加账号"""
 
     fields = {
         "PassWord": fields.Str(required=True, dump_to="PassWord"),
         "UserEmail": fields.Str(required=True, dump_to="UserEmail"),
     }
 
 
 class CreateUserResponseSchema(schema.ResponseSchema):
-    """ CreateUser - 管理员添加账号
-    """
+    """CreateUser - 管理员添加账号"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "UserID": fields.Int(required=False, load_from="UserID"),
     }
 
 
@@ -690,16 +646,15 @@
 API: CreateVMInstance
 
 创建虚拟机
 """
 
 
 class CreateVMInstanceRequestSchema(schema.RequestSchema):
-    """ CreateVMInstance - 创建虚拟机
-    """
+    """CreateVMInstance - 创建虚拟机"""
 
     fields = {
         "Bandwidth": fields.Str(required=False, dump_to="Bandwidth"),
         "BootDiskSetType": fields.Str(required=True, dump_to="BootDiskSetType"),
         "CPU": fields.Int(required=True, dump_to="CPU"),
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "DataDiskSetType": fields.Str(required=True, dump_to="DataDiskSetType"),
@@ -721,16 +676,15 @@
         "VPCID": fields.Str(required=True, dump_to="VPCID"),
         "WANSGID": fields.Str(required=True, dump_to="WANSGID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateVMInstanceResponseSchema(schema.ResponseSchema):
-    """ CreateVMInstance - 创建虚拟机
-    """
+    """CreateVMInstance - 创建虚拟机"""
 
     fields = {
         "DiskID": fields.Str(required=False, load_from="DiskID"),
         "EIPID": fields.Str(required=False, load_from="EIPID"),
         "Message": fields.Str(required=False, load_from="Message"),
         "VMID": fields.Str(required=False, load_from="VMID"),
     }
@@ -740,29 +694,27 @@
 API: CreateVPC
 
 创建VPC
 """
 
 
 class CreateVPCRequestSchema(schema.RequestSchema):
-    """ CreateVPC - 创建VPC
-    """
+    """CreateVPC - 创建VPC"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "Network": fields.Str(required=True, dump_to="Network"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateVPCResponseSchema(schema.ResponseSchema):
-    """ CreateVPC - 创建VPC
-    """
+    """CreateVPC - 创建VPC"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "VPCID": fields.Str(required=False, load_from="VPCID"),
     }
 
 
@@ -770,16 +722,15 @@
 API: CreateVS
 
 创建负载均衡VServer
 """
 
 
 class CreateVSRequestSchema(schema.RequestSchema):
-    """ CreateVS - 创建负载均衡VServer
-    """
+    """CreateVS - 创建负载均衡VServer"""
 
     fields = {
         "CACertificateID": fields.Str(
             required=False, dump_to="CACertificateID"
         ),
         "Domain": fields.Str(required=False, dump_to="Domain"),
         "HealthcheckType": fields.Str(required=True, dump_to="HealthcheckType"),
@@ -801,16 +752,15 @@
             required=False, dump_to="ServerCertificateID"
         ),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateVSResponseSchema(schema.ResponseSchema):
-    """ CreateVS - 创建负载均衡VServer
-    """
+    """CreateVS - 创建负载均衡VServer"""
 
     fields = {
         "Action": fields.Str(required=True, load_from="Action"),
         "Message": fields.Str(required=False, load_from="Message"),
         "RetCode": fields.Int(required=True, load_from="RetCode"),
         "VSID": fields.Str(required=False, load_from="VSID"),
     }
@@ -820,31 +770,29 @@
 API: CreateVSPolicy
 
 创建七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
 """
 
 
 class CreateVSPolicyRequestSchema(schema.RequestSchema):
-    """ CreateVSPolicy - 创建七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """CreateVSPolicy - 创建七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "Domain": fields.Str(required=False, dump_to="Domain"),
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Path": fields.Str(required=False, dump_to="Path"),
         "RSIDs": fields.List(fields.Str()),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateVSPolicyResponseSchema(schema.ResponseSchema):
-    """ CreateVSPolicy - 创建七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """CreateVSPolicy - 创建七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
         "PolicyID": fields.Str(required=False, load_from="PolicyID"),
     }
 
 
@@ -852,498 +800,462 @@
 API: DeleteCertificate
 
 删除证书
 """
 
 
 class DeleteCertificateRequestSchema(schema.RequestSchema):
-    """ DeleteCertificate - 删除证书
-    """
+    """DeleteCertificate - 删除证书"""
 
     fields = {
         "CertificateID": fields.Str(required=True, dump_to="CertificateID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteCertificateResponseSchema(schema.ResponseSchema):
-    """ DeleteCertificate - 删除证书
-    """
+    """DeleteCertificate - 删除证书"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteCustomImage
 
 删除自制镜像
 """
 
 
 class DeleteCustomImageRequestSchema(schema.RequestSchema):
-    """ DeleteCustomImage - 删除自制镜像
-    """
+    """DeleteCustomImage - 删除自制镜像"""
 
     fields = {
         "ImageID": fields.Str(required=True, dump_to="ImageID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteCustomImageResponseSchema(schema.ResponseSchema):
-    """ DeleteCustomImage - 删除自制镜像
-    """
+    """DeleteCustomImage - 删除自制镜像"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteDisk
 
 删除硬盘
 """
 
 
 class DeleteDiskRequestSchema(schema.RequestSchema):
-    """ DeleteDisk - 删除硬盘
-    """
+    """DeleteDisk - 删除硬盘"""
 
     fields = {
         "DiskID": fields.Str(required=True, dump_to="DiskID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteDiskResponseSchema(schema.ResponseSchema):
-    """ DeleteDisk - 删除硬盘
-    """
+    """DeleteDisk - 删除硬盘"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteLB
 
 删除负载均衡
 """
 
 
 class DeleteLBRequestSchema(schema.RequestSchema):
-    """ DeleteLB - 删除负载均衡
-    """
+    """DeleteLB - 删除负载均衡"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteLBResponseSchema(schema.ResponseSchema):
-    """ DeleteLB - 删除负载均衡
-    """
+    """DeleteLB - 删除负载均衡"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteNATGW
 
 删除NAT网关
 """
 
 
 class DeleteNATGWRequestSchema(schema.RequestSchema):
-    """ DeleteNATGW - 删除NAT网关
-    """
+    """DeleteNATGW - 删除NAT网关"""
 
     fields = {
         "NATGWID": fields.Str(required=True, dump_to="NATGWID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteNATGWResponseSchema(schema.ResponseSchema):
-    """ DeleteNATGW - 删除NAT网关
-    """
+    """DeleteNATGW - 删除NAT网关"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteNATGWRule
 
 删除NAT网关白名单
 """
 
 
 class DeleteNATGWRuleRequestSchema(schema.RequestSchema):
-    """ DeleteNATGWRule - 删除NAT网关白名单
-    """
+    """DeleteNATGWRule - 删除NAT网关白名单"""
 
     fields = {
         "NATGWID": fields.Str(required=True, dump_to="NATGWID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RuleID": fields.Str(required=True, dump_to="RuleID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteNATGWRuleResponseSchema(schema.ResponseSchema):
-    """ DeleteNATGWRule - 删除NAT网关白名单
-    """
+    """DeleteNATGWRule - 删除NAT网关白名单"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteNIC
 
 删除网卡
 """
 
 
 class DeleteNICRequestSchema(schema.RequestSchema):
-    """ DeleteNIC - 删除网卡
-    """
+    """DeleteNIC - 删除网卡"""
 
     fields = {
         "NICID": fields.Str(required=True, dump_to="NICID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteNICResponseSchema(schema.ResponseSchema):
-    """ DeleteNIC - 删除网卡
-    """
+    """DeleteNIC - 删除网卡"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeletePhysicalIP
 
 删除物理IP
 """
 
 
 class DeletePhysicalIPRequestSchema(schema.RequestSchema):
-    """ DeletePhysicalIP - 删除物理IP
-    """
+    """DeletePhysicalIP - 删除物理IP"""
 
     fields = {
         "PhysicalIPID": fields.Str(required=True, dump_to="PhysicalIPID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeletePhysicalIPResponseSchema(schema.ResponseSchema):
-    """ DeletePhysicalIP - 删除物理IP
-    """
+    """DeletePhysicalIP - 删除物理IP"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteRS
 
 移除负载均衡的单个服务节点
 """
 
 
 class DeleteRSRequestSchema(schema.RequestSchema):
-    """ DeleteRS - 移除负载均衡的单个服务节点
-    """
+    """DeleteRS - 移除负载均衡的单个服务节点"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "RSID": fields.Str(required=True, dump_to="RSID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteRSResponseSchema(schema.ResponseSchema):
-    """ DeleteRS - 移除负载均衡的单个服务节点
-    """
+    """DeleteRS - 移除负载均衡的单个服务节点"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteSecurityGroup
 
 删除安全组
 """
 
 
 class DeleteSecurityGroupRequestSchema(schema.RequestSchema):
-    """ DeleteSecurityGroup - 删除安全组
-    """
+    """DeleteSecurityGroup - 删除安全组"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "SGID": fields.Str(required=True, dump_to="SGID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteSecurityGroupResponseSchema(schema.ResponseSchema):
-    """ DeleteSecurityGroup - 删除安全组
-    """
+    """DeleteSecurityGroup - 删除安全组"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteSecurityGroupRule
 
 删除安全组规则
 """
 
 
 class DeleteSecurityGroupRuleRequestSchema(schema.RequestSchema):
-    """ DeleteSecurityGroupRule - 删除安全组规则
-    """
+    """DeleteSecurityGroupRule - 删除安全组规则"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "SGID": fields.Str(required=True, dump_to="SGID"),
         "SGRuleID": fields.Str(required=True, dump_to="SGRuleID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteSecurityGroupRuleResponseSchema(schema.ResponseSchema):
-    """ DeleteSecurityGroupRule - 删除安全组规则
-    """
+    """DeleteSecurityGroupRule - 删除安全组规则"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteSnapshot
 
 删除快照，仅支持状态为正常的快照进行删除操作。
 """
 
 
 class DeleteSnapshotRequestSchema(schema.RequestSchema):
-    """ DeleteSnapshot - 删除快照，仅支持状态为正常的快照进行删除操作。
-    """
+    """DeleteSnapshot - 删除快照，仅支持状态为正常的快照进行删除操作。"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "SnapshotID": fields.Str(required=True, dump_to="SnapshotID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteSnapshotResponseSchema(schema.ResponseSchema):
-    """ DeleteSnapshot - 删除快照，仅支持状态为正常的快照进行删除操作。
-    """
+    """DeleteSnapshot - 删除快照，仅支持状态为正常的快照进行删除操作。"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteSubnet
 
 删除子网
 """
 
 
 class DeleteSubnetRequestSchema(schema.RequestSchema):
-    """ DeleteSubnet - 删除子网
-    """
+    """DeleteSubnet - 删除子网"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetID": fields.Str(required=True, dump_to="SubnetID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteSubnetResponseSchema(schema.ResponseSchema):
-    """ DeleteSubnet - 删除子网
-    """
+    """DeleteSubnet - 删除子网"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteVMInstance
 
 删除虚拟机
 """
 
 
 class DeleteVMInstanceRequestSchema(schema.RequestSchema):
-    """ DeleteVMInstance - 删除虚拟机
-    """
+    """DeleteVMInstance - 删除虚拟机"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteVMInstanceResponseSchema(schema.ResponseSchema):
-    """ DeleteVMInstance - 删除虚拟机
-    """
+    """DeleteVMInstance - 删除虚拟机"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: DeleteVPC
 
 删除VPC
 """
 
 
 class DeleteVPCRequestSchema(schema.RequestSchema):
-    """ DeleteVPC - 删除VPC
-    """
+    """DeleteVPC - 删除VPC"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCID": fields.Str(required=True, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteVPCResponseSchema(schema.ResponseSchema):
-    """ DeleteVPC - 删除VPC
-    """
+    """DeleteVPC - 删除VPC"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteVS
 
 删除VServer
 """
 
 
 class DeleteVSRequestSchema(schema.RequestSchema):
-    """ DeleteVS - 删除VServer
-    """
+    """DeleteVS - 删除VServer"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteVSResponseSchema(schema.ResponseSchema):
-    """ DeleteVS - 删除VServer
-    """
+    """DeleteVS - 删除VServer"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DeleteVSPolicy
 
 删除七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
 """
 
 
 class DeleteVSPolicyRequestSchema(schema.RequestSchema):
-    """ DeleteVSPolicy - 删除七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """DeleteVSPolicy - 删除七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "PolicyID": fields.Str(required=True, dump_to="PolicyID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteVSPolicyResponseSchema(schema.ResponseSchema):
-    """ DeleteVSPolicy - 删除七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """DeleteVSPolicy - 删除七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: DescribeCertificate
 
 查询证书
 """
 
 
 class DescribeCertificateRequestSchema(schema.RequestSchema):
-    """ DescribeCertificate - 查询证书
-    """
+    """DescribeCertificate - 查询证书"""
 
     fields = {
         "CertificateIDs": fields.List(fields.Str()),
         "CertificateType": fields.Str(
             required=False, dump_to="CertificateType"
         ),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeCertificateResponseSchema(schema.ResponseSchema):
-    """ DescribeCertificate - 查询证书
-    """
+    """DescribeCertificate - 查询证书"""
 
     fields = {
         "Infos": fields.List(
             models.CertificateInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1354,30 +1266,28 @@
 API: DescribeDisk
 
 获取硬盘信息
 """
 
 
 class DescribeDiskRequestSchema(schema.RequestSchema):
-    """ DescribeDisk - 获取硬盘信息
-    """
+    """DescribeDisk - 获取硬盘信息"""
 
     fields = {
         "DiskIDs": fields.List(fields.Str()),
         "DiskType": fields.Str(required=False, dump_to="DiskType"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeDiskResponseSchema(schema.ResponseSchema):
-    """ DescribeDisk - 获取硬盘信息
-    """
+    """DescribeDisk - 获取硬盘信息"""
 
     fields = {
         "Infos": fields.List(
             models.DiskInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1388,31 +1298,29 @@
 API: DescribeEIP
 
 获取外网IP的信息
 """
 
 
 class DescribeEIPRequestSchema(schema.RequestSchema):
-    """ DescribeEIP - 获取外网IP的信息
-    """
+    """DescribeEIP - 获取外网IP的信息"""
 
     fields = {
         "BindResourceID": fields.Str(required=False, dump_to="BindResourceID"),
         "EIPIDs": fields.List(fields.Str()),
         "IPVersion": fields.Str(required=False, dump_to="IPVersion"),
         "Limit": fields.Str(required=False, dump_to="Limit"),
         "Offset": fields.Str(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeEIPResponseSchema(schema.ResponseSchema):
-    """ DescribeEIP - 获取外网IP的信息
-    """
+    """DescribeEIP - 获取外网IP的信息"""
 
     fields = {
         "Infos": fields.List(
             models.EIPInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "Totalcount": fields.Int(required=False, load_from="Totalcount"),
@@ -1423,30 +1331,28 @@
 API: DescribeImage
 
 获取镜像信息，包括默认镜像和自制镜像。
 """
 
 
 class DescribeImageRequestSchema(schema.RequestSchema):
-    """ DescribeImage - 获取镜像信息，包括默认镜像和自制镜像。
-    """
+    """DescribeImage - 获取镜像信息，包括默认镜像和自制镜像。"""
 
     fields = {
         "ImageIDs": fields.List(fields.Str()),
         "ImageType": fields.Str(required=False, dump_to="ImageType"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeImageResponseSchema(schema.ResponseSchema):
-    """ DescribeImage - 获取镜像信息，包括默认镜像和自制镜像。
-    """
+    """DescribeImage - 获取镜像信息，包括默认镜像和自制镜像。"""
 
     fields = {
         "Action": fields.Str(required=True, load_from="Action"),
         "Infos": fields.List(
             models.ImageInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
@@ -1459,31 +1365,29 @@
 API: DescribeLB
 
 获取负载均衡信息
 """
 
 
 class DescribeLBRequestSchema(schema.RequestSchema):
-    """ DescribeLB - 获取负载均衡信息
-    """
+    """DescribeLB - 获取负载均衡信息"""
 
     fields = {
         "LBIDs": fields.List(fields.Str()),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetID": fields.Str(required=False, dump_to="SubnetID"),
         "VPCID": fields.Str(required=False, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeLBResponseSchema(schema.ResponseSchema):
-    """ DescribeLB - 获取负载均衡信息
-    """
+    """DescribeLB - 获取负载均衡信息"""
 
     fields = {
         "Infos": fields.List(
             models.LBInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1494,31 +1398,29 @@
 API: DescribeMetric
 
 获取资源监控信息
 """
 
 
 class DescribeMetricRequestSchema(schema.RequestSchema):
-    """ DescribeMetric - 获取资源监控信息
-    """
+    """DescribeMetric - 获取资源监控信息"""
 
     fields = {
         "BeginTime": fields.Str(required=True, dump_to="BeginTime"),
         "EndTime": fields.Str(required=True, dump_to="EndTime"),
         "MetricName": fields.List(fields.Str()),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeMetricResponseSchema(schema.ResponseSchema):
-    """ DescribeMetric - 获取资源监控信息
-    """
+    """DescribeMetric - 获取资源监控信息"""
 
     fields = {
         "Infos": fields.List(
             models.MetricInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=False, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -1529,29 +1431,27 @@
 API: DescribeNATGW
 
 获取NAT网关信息
 """
 
 
 class DescribeNATGWRequestSchema(schema.RequestSchema):
-    """ DescribeNATGW - 获取NAT网关信息
-    """
+    """DescribeNATGW - 获取NAT网关信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "NATGWIDs": fields.List(fields.Str()),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeNATGWResponseSchema(schema.ResponseSchema):
-    """ DescribeNATGW - 获取NAT网关信息
-    """
+    """DescribeNATGW - 获取NAT网关信息"""
 
     fields = {
         "Infos": fields.List(
             models.NATGWInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1562,32 +1462,30 @@
 API: DescribeNATGWRule
 
 获取NAT网关白名单信息 
 """
 
 
 class DescribeNATGWRuleRequestSchema(schema.RequestSchema):
-    """ DescribeNATGWRule - 获取NAT网关白名单信息 
-    """
+    """DescribeNATGWRule - 获取NAT网关白名单信息"""
 
     fields = {
         "BindResourceIDs": fields.List(fields.Str()),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "NATGWID": fields.Str(required=True, dump_to="NATGWID"),
         "NATGWType": fields.Str(required=True, dump_to="NATGWType"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RuleIDs": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeNATGWRuleResponseSchema(schema.ResponseSchema):
-    """ DescribeNATGWRule - 获取NAT网关白名单信息 
-    """
+    """DescribeNATGWRule - 获取NAT网关白名单信息"""
 
     fields = {
         "Infos": fields.List(
             models.NATGWRuleInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1598,29 +1496,27 @@
 API: DescribeNIC
 
 获取网卡信息
 """
 
 
 class DescribeNICRequestSchema(schema.RequestSchema):
-    """ DescribeNIC - 获取网卡信息
-    """
+    """DescribeNIC - 获取网卡信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "NICIDs": fields.List(fields.Str()),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeNICResponseSchema(schema.ResponseSchema):
-    """ DescribeNIC - 获取网卡信息
-    """
+    """DescribeNIC - 获取网卡信息"""
 
     fields = {
         "Infos": fields.List(
             models.NICInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1631,16 +1527,15 @@
 API: DescribeOPLogs
 
 查询操作日志
 """
 
 
 class DescribeOPLogsRequestSchema(schema.RequestSchema):
-    """ DescribeOPLogs - 查询操作日志
-    """
+    """DescribeOPLogs - 查询操作日志"""
 
     fields = {
         "BeginTime": fields.Int(required=True, dump_to="BeginTime"),
         "EndTime": fields.Int(required=True, dump_to="EndTime"),
         "IsSuccess": fields.Str(required=False, dump_to="IsSuccess"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
@@ -1648,16 +1543,15 @@
         "ResourceID": fields.Str(required=False, dump_to="ResourceID"),
         "ResourceType": fields.Str(required=False, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeOPLogsResponseSchema(schema.ResponseSchema):
-    """ DescribeOPLogs - 查询操作日志
-    """
+    """DescribeOPLogs - 查询操作日志"""
 
     fields = {
         "Infos": fields.List(
             models.OPLogInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1668,29 +1562,27 @@
 API: DescribePhysicalIP
 
 获取物理IP信息 
 """
 
 
 class DescribePhysicalIPRequestSchema(schema.RequestSchema):
-    """ DescribePhysicalIP - 获取物理IP信息 
-    """
+    """DescribePhysicalIP - 获取物理IP信息"""
 
     fields = {
         "Limit": fields.Str(required=False, dump_to="Limit"),
         "Offset": fields.Str(required=False, dump_to="Offset"),
         "PhysicalIPIDs": fields.List(fields.Str()),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribePhysicalIPResponseSchema(schema.ResponseSchema):
-    """ DescribePhysicalIP - 获取物理IP信息 
-    """
+    """DescribePhysicalIP - 获取物理IP信息"""
 
     fields = {
         "Infos": fields.List(
             models.PhysicalIPInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -1701,31 +1593,29 @@
 API: DescribeRS
 
 获取负载均衡服务的服务节点信息
 """
 
 
 class DescribeRSRequestSchema(schema.RequestSchema):
-    """ DescribeRS - 获取负载均衡服务的服务节点信息
-    """
+    """DescribeRS - 获取负载均衡服务的服务节点信息"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "RSIDs": fields.List(fields.Str()),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=False, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeRSResponseSchema(schema.ResponseSchema):
-    """ DescribeRS - 获取负载均衡服务的服务节点信息
-    """
+    """DescribeRS - 获取负载均衡服务的服务节点信息"""
 
     fields = {
         "Infos": fields.List(
             models.RSInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1736,29 +1626,27 @@
 API: DescribeRecycledResource
 
 查询回收站资源
 """
 
 
 class DescribeRecycledResourceRequestSchema(schema.RequestSchema):
-    """ DescribeRecycledResource - 查询回收站资源
-    """
+    """DescribeRecycledResource - 查询回收站资源"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceIDs": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeRecycledResourceResponseSchema(schema.ResponseSchema):
-    """ DescribeRecycledResource - 查询回收站资源
-    """
+    """DescribeRecycledResource - 查询回收站资源"""
 
     fields = {
         "Infos": fields.List(
             models.RecycledResourceInfoSchema(),
             required=True,
             load_from="Infos",
         ),
@@ -1770,29 +1658,27 @@
 API: DescribeSecurityGroup
 
 查询安全组信息
 """
 
 
 class DescribeSecurityGroupRequestSchema(schema.RequestSchema):
-    """ DescribeSecurityGroup - 查询安全组信息
-    """
+    """DescribeSecurityGroup - 查询安全组信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SGIDs": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeSecurityGroupResponseSchema(schema.ResponseSchema):
-    """ DescribeSecurityGroup - 查询安全组信息
-    """
+    """DescribeSecurityGroup - 查询安全组信息"""
 
     fields = {
         "Infos": fields.List(
             models.SGInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -1803,29 +1689,27 @@
 API: DescribeSecurityGroupResource
 
 查询安全组绑定的资源信息
 """
 
 
 class DescribeSecurityGroupResourceRequestSchema(schema.RequestSchema):
-    """ DescribeSecurityGroupResource - 查询安全组绑定的资源信息
-    """
+    """DescribeSecurityGroupResource - 查询安全组绑定的资源信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SGID": fields.Str(required=True, dump_to="SGID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeSecurityGroupResourceResponseSchema(schema.ResponseSchema):
-    """ DescribeSecurityGroupResource - 查询安全组绑定的资源信息
-    """
+    """DescribeSecurityGroupResource - 查询安全组绑定的资源信息"""
 
     fields = {
         "Infos": fields.List(
             models.SGResourceInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1836,30 +1720,28 @@
 API: DescribeSnapshot
 
 查询硬盘快照信息
 """
 
 
 class DescribeSnapshotRequestSchema(schema.RequestSchema):
-    """ DescribeSnapshot - 查询硬盘快照信息
-    """
+    """DescribeSnapshot - 查询硬盘快照信息"""
 
     fields = {
         "DiskID": fields.Str(required=False, dump_to="DiskID"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SnapshotIDs": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeSnapshotResponseSchema(schema.ResponseSchema):
-    """ DescribeSnapshot - 查询硬盘快照信息
-    """
+    """DescribeSnapshot - 查询硬盘快照信息"""
 
     fields = {
         "Infos": fields.List(
             models.SnapshotInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1870,26 +1752,24 @@
 API: DescribeStorageType
 
 查询存储类型
 """
 
 
 class DescribeStorageTypeRequestSchema(schema.RequestSchema):
-    """ DescribeStorageType - 查询存储类型
-    """
+    """DescribeStorageType - 查询存储类型"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeStorageTypeResponseSchema(schema.ResponseSchema):
-    """ DescribeStorageType - 查询存储类型
-    """
+    """DescribeStorageType - 查询存储类型"""
 
     fields = {
         "Infos": fields.List(
             models.StorageTypeInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -1900,30 +1780,28 @@
 API: DescribeSubnet
 
 查询子网信息
 """
 
 
 class DescribeSubnetRequestSchema(schema.RequestSchema):
-    """ DescribeSubnet - 查询子网信息
-    """
+    """DescribeSubnet - 查询子网信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetIDs": fields.List(fields.Str()),
         "VPCID": fields.Str(required=False, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeSubnetResponseSchema(schema.ResponseSchema):
-    """ DescribeSubnet - 查询子网信息
-    """
+    """DescribeSubnet - 查询子网信息"""
 
     fields = {
         "Infos": fields.List(
             models.SubnetInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -1934,27 +1812,25 @@
 API: DescribeUser
 
 查询租户信息
 """
 
 
 class DescribeUserRequestSchema(schema.RequestSchema):
-    """ DescribeUser - 查询租户信息
-    """
+    """DescribeUser - 查询租户信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "UserIDs": fields.List(fields.Int()),
     }
 
 
 class DescribeUserResponseSchema(schema.ResponseSchema):
-    """ DescribeUser - 查询租户信息
-    """
+    """DescribeUser - 查询租户信息"""
 
     fields = {
         "Infos": fields.List(
             models.UserInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -1965,31 +1841,29 @@
 API: DescribeVMInstance
 
 查询虚拟机
 """
 
 
 class DescribeVMInstanceRequestSchema(schema.RequestSchema):
-    """ DescribeVMInstance - 查询虚拟机
-    """
+    """DescribeVMInstance - 查询虚拟机"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetID": fields.Str(required=False, dump_to="SubnetID"),
         "VMIDs": fields.List(fields.Str()),
         "VPCID": fields.Str(required=False, dump_to="VPCID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeVMInstanceResponseSchema(schema.ResponseSchema):
-    """ DescribeVMInstance - 查询虚拟机
-    """
+    """DescribeVMInstance - 查询虚拟机"""
 
     fields = {
         "Infos": fields.List(
             models.VMInstanceInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=False, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -2000,26 +1874,24 @@
 API: DescribeVMType
 
 查询主机机型
 """
 
 
 class DescribeVMTypeRequestSchema(schema.RequestSchema):
-    """ DescribeVMType - 查询主机机型
-    """
+    """DescribeVMType - 查询主机机型"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeVMTypeResponseSchema(schema.ResponseSchema):
-    """ DescribeVMType - 查询主机机型
-    """
+    """DescribeVMType - 查询主机机型"""
 
     fields = {
         "Infos": fields.List(
             models.VMTypeInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -2030,29 +1902,27 @@
 API: DescribeVPC
 
 查询VPC信息
 """
 
 
 class DescribeVPCRequestSchema(schema.RequestSchema):
-    """ DescribeVPC - 查询VPC信息
-    """
+    """DescribeVPC - 查询VPC信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCIDs": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeVPCResponseSchema(schema.ResponseSchema):
-    """ DescribeVPC - 查询VPC信息
-    """
+    """DescribeVPC - 查询VPC信息"""
 
     fields = {
         "Infos": fields.List(
             models.VPCInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
@@ -2063,30 +1933,28 @@
 API: DescribeVS
 
 获取负载均衡 VServer 信息
 """
 
 
 class DescribeVSRequestSchema(schema.RequestSchema):
-    """ DescribeVS - 获取负载均衡 VServer 信息
-    """
+    """DescribeVS - 获取负载均衡 VServer 信息"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSIDs": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeVSResponseSchema(schema.ResponseSchema):
-    """ DescribeVS - 获取负载均衡 VServer 信息
-    """
+    """DescribeVS - 获取负载均衡 VServer 信息"""
 
     fields = {
         "Infos": fields.List(
             models.VSInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -2097,31 +1965,29 @@
 API: DescribeVSPolicy
 
 获取七层负载均衡内容转发规则信息，仅当 VServer 的监听协议为 HTTP 时有效。
 """
 
 
 class DescribeVSPolicyRequestSchema(schema.RequestSchema):
-    """ DescribeVSPolicy - 获取七层负载均衡内容转发规则信息，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """DescribeVSPolicy - 获取七层负载均衡内容转发规则信息，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "PolicyIDs": fields.List(fields.Str()),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=False, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeVSPolicyResponseSchema(schema.ResponseSchema):
-    """ DescribeVSPolicy - 获取七层负载均衡内容转发规则信息，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """DescribeVSPolicy - 获取七层负载均衡内容转发规则信息，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "Infos": fields.List(
             models.VSPolicyInfoSchema(), required=True, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
@@ -2132,144 +1998,134 @@
 API: DetachDisk
 
 解绑硬盘
 """
 
 
 class DetachDiskRequestSchema(schema.RequestSchema):
-    """ DetachDisk - 解绑硬盘
-    """
+    """DetachDisk - 解绑硬盘"""
 
     fields = {
         "DiskID": fields.Str(required=True, dump_to="DiskID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DetachDiskResponseSchema(schema.ResponseSchema):
-    """ DetachDisk - 解绑硬盘
-    """
+    """DetachDisk - 解绑硬盘"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DetachNIC
 
 解绑UClouStack网卡
 """
 
 
 class DetachNICRequestSchema(schema.RequestSchema):
-    """ DetachNIC - 解绑UClouStack网卡
-    """
+    """DetachNIC - 解绑UClouStack网卡"""
 
     fields = {
         "NICID": fields.Str(required=True, dump_to="NICID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DetachNICResponseSchema(schema.ResponseSchema):
-    """ DetachNIC - 解绑UClouStack网卡
-    """
+    """DetachNIC - 解绑UClouStack网卡"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: DisableRS
 
 禁用负载均衡的单个服务节点
 """
 
 
 class DisableRSRequestSchema(schema.RequestSchema):
-    """ DisableRS - 禁用负载均衡的单个服务节点
-    """
+    """DisableRS - 禁用负载均衡的单个服务节点"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "RSID": fields.Str(required=True, dump_to="RSID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DisableRSResponseSchema(schema.ResponseSchema):
-    """ DisableRS - 禁用负载均衡的单个服务节点
-    """
+    """DisableRS - 禁用负载均衡的单个服务节点"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: EnableRS
 
 启用负载均衡的单个服务节点
 """
 
 
 class EnableRSRequestSchema(schema.RequestSchema):
-    """ EnableRS - 启用负载均衡的单个服务节点
-    """
+    """EnableRS - 启用负载均衡的单个服务节点"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "RSID": fields.Str(required=True, dump_to="RSID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class EnableRSResponseSchema(schema.ResponseSchema):
-    """ EnableRS - 启用负载均衡的单个服务节点
-    """
+    """EnableRS - 启用负载均衡的单个服务节点"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: GetDiskPrice
 
 获取硬盘价格
 """
 
 
 class GetDiskPriceRequestSchema(schema.RequestSchema):
-    """ GetDiskPrice - 获取硬盘价格
-    """
+    """GetDiskPrice - 获取硬盘价格"""
 
     fields = {
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SetType": fields.Str(required=True, dump_to="SetType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class GetDiskPriceResponseSchema(schema.ResponseSchema):
-    """ GetDiskPrice - 获取硬盘价格
-    """
+    """GetDiskPrice - 获取硬盘价格"""
 
     fields = {
         "Infos": fields.List(
             models.PriceInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
     }
@@ -2279,30 +2135,28 @@
 API: GetEIPPrice
 
 获取外网IP价格
 """
 
 
 class GetEIPPriceRequestSchema(schema.RequestSchema):
-    """ GetEIPPrice - 获取外网IP价格
-    """
+    """GetEIPPrice - 获取外网IP价格"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "OpertatorName": fields.Str(required=True, dump_to="OpertatorName"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class GetEIPPriceResponseSchema(schema.ResponseSchema):
-    """ GetEIPPrice - 获取外网IP价格
-    """
+    """GetEIPPrice - 获取外网IP价格"""
 
     fields = {
         "Infos": fields.List(
             models.PriceInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
     }
@@ -2312,16 +2166,15 @@
 API: GetVMInstancePrice
 
 获取虚拟机价格
 """
 
 
 class GetVMInstancePriceRequestSchema(schema.RequestSchema):
-    """ GetVMInstancePrice - 获取虚拟机价格
-    """
+    """GetVMInstancePrice - 获取虚拟机价格"""
 
     fields = {
         "BootDiskSetType": fields.Str(required=True, dump_to="BootDiskSetType"),
         "CPU": fields.Int(required=True, dump_to="CPU"),
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "DataDiskSetType": fields.Str(required=True, dump_to="DataDiskSetType"),
         "DataDiskSpace": fields.Int(required=True, dump_to="DataDiskSpace"),
@@ -2333,16 +2186,15 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMType": fields.Str(required=True, dump_to="VMType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class GetVMInstancePriceResponseSchema(schema.ResponseSchema):
-    """ GetVMInstancePrice - 获取虚拟机价格
-    """
+    """GetVMInstancePrice - 获取虚拟机价格"""
 
     fields = {
         "Infos": fields.List(
             models.PriceInfoSchema(), required=False, load_from="Infos"
         ),
         "Message": fields.Str(required=False, load_from="Message"),
     }
@@ -2352,388 +2204,360 @@
 API: ModifyEIPBandwidth
 
 调整外网IP带宽
 """
 
 
 class ModifyEIPBandwidthRequestSchema(schema.RequestSchema):
-    """ ModifyEIPBandwidth - 调整外网IP带宽
-    """
+    """ModifyEIPBandwidth - 调整外网IP带宽"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "EIPID": fields.Str(required=True, dump_to="EIPID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ModifyEIPBandwidthResponseSchema(schema.ResponseSchema):
-    """ ModifyEIPBandwidth - 调整外网IP带宽
-    """
+    """ModifyEIPBandwidth - 调整外网IP带宽"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: ModifyNameAndRemark
 
 修改资源名称和备注
 """
 
 
 class ModifyNameAndRemarkRequestSchema(schema.RequestSchema):
-    """ ModifyNameAndRemark - 修改资源名称和备注
-    """
+    """ModifyNameAndRemark - 修改资源名称和备注"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ModifyNameAndRemarkResponseSchema(schema.ResponseSchema):
-    """ ModifyNameAndRemark - 修改资源名称和备注
-    """
+    """ModifyNameAndRemark - 修改资源名称和备注"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: PoweroffVMInstance
 
 断电虚拟机，可能导致丢失数据甚至损坏操作系统，仅适用于虚拟机死机及级端测试场景。
 """
 
 
 class PoweroffVMInstanceRequestSchema(schema.RequestSchema):
-    """ PoweroffVMInstance - 断电虚拟机，可能导致丢失数据甚至损坏操作系统，仅适用于虚拟机死机及级端测试场景。
-    """
+    """PoweroffVMInstance - 断电虚拟机，可能导致丢失数据甚至损坏操作系统，仅适用于虚拟机死机及级端测试场景。"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class PoweroffVMInstanceResponseSchema(schema.ResponseSchema):
-    """ PoweroffVMInstance - 断电虚拟机，可能导致丢失数据甚至损坏操作系统，仅适用于虚拟机死机及级端测试场景。
-    """
+    """PoweroffVMInstance - 断电虚拟机，可能导致丢失数据甚至损坏操作系统，仅适用于虚拟机死机及级端测试场景。"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: Recharge
 
 管理员给租户充值
 """
 
 
 class RechargeRequestSchema(schema.RequestSchema):
-    """ Recharge - 管理员给租户充值
-    """
+    """Recharge - 管理员给租户充值"""
 
     fields = {
         "Amount": fields.Int(required=True, dump_to="Amount"),
         "FromType": fields.Str(required=True, dump_to="FromType"),
         "SerialNo": fields.Str(required=True, dump_to="SerialNo"),
         "UserID": fields.Int(required=True, dump_to="UserID"),
     }
 
 
 class RechargeResponseSchema(schema.ResponseSchema):
-    """ Recharge - 管理员给租户充值
-    """
+    """Recharge - 管理员给租户充值"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: ReinstallVMInstance
 
 重装系统，关机的虚拟机才可以重装系统
 """
 
 
 class ReinstallVMInstanceRequestSchema(schema.RequestSchema):
-    """ ReinstallVMInstance - 重装系统，关机的虚拟机才可以重装系统
-    """
+    """ReinstallVMInstance - 重装系统，关机的虚拟机才可以重装系统"""
 
     fields = {
         "ImageID": fields.Str(required=True, dump_to="ImageID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ReinstallVMInstanceResponseSchema(schema.ResponseSchema):
-    """ ReinstallVMInstance - 重装系统，关机的虚拟机才可以重装系统
-    """
+    """ReinstallVMInstance - 重装系统，关机的虚拟机才可以重装系统"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: ReleaseEIP
 
 删除外网IP
 """
 
 
 class ReleaseEIPRequestSchema(schema.RequestSchema):
-    """ ReleaseEIP - 删除外网IP
-    """
+    """ReleaseEIP - 删除外网IP"""
 
     fields = {
         "EIPID": fields.Str(required=True, dump_to="EIPID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ReleaseEIPResponseSchema(schema.ResponseSchema):
-    """ ReleaseEIP - 删除外网IP
-    """
+    """ReleaseEIP - 删除外网IP"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: RenewResource
 
 续费回收站资源 
 """
 
 
 class RenewResourceRequestSchema(schema.RequestSchema):
-    """ RenewResource - 续费回收站资源 
-    """
+    """RenewResource - 续费回收站资源"""
 
     fields = {
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class RenewResourceResponseSchema(schema.ResponseSchema):
-    """ RenewResource - 续费回收站资源 
-    """
+    """RenewResource - 续费回收站资源"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: ResetVMInstancePassword
 
 重置虚拟机密码，主机必须开机才可以重置密码
 """
 
 
 class ResetVMInstancePasswordRequestSchema(schema.RequestSchema):
-    """ ResetVMInstancePassword - 重置虚拟机密码，主机必须开机才可以重置密码
-    """
+    """ResetVMInstancePassword - 重置虚拟机密码，主机必须开机才可以重置密码"""
 
     fields = {
         "Password": fields.Str(required=True, dump_to="Password"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ResetVMInstancePasswordResponseSchema(schema.ResponseSchema):
-    """ ResetVMInstancePassword - 重置虚拟机密码，主机必须开机才可以重置密码
-    """
+    """ResetVMInstancePassword - 重置虚拟机密码，主机必须开机才可以重置密码"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: ResizeVMConfig
 
 修改虚拟机配置
 """
 
 
 class ResizeVMConfigRequestSchema(schema.RequestSchema):
-    """ ResizeVMConfig - 修改虚拟机配置
-    """
+    """ResizeVMConfig - 修改虚拟机配置"""
 
     fields = {
         "CPU": fields.Int(required=True, dump_to="CPU"),
         "Memory": fields.Int(required=True, dump_to="Memory"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ResizeVMConfigResponseSchema(schema.ResponseSchema):
-    """ ResizeVMConfig - 修改虚拟机配置
-    """
+    """ResizeVMConfig - 修改虚拟机配置"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: RestartVMInstance
 
 重启虚拟机
 """
 
 
 class RestartVMInstanceRequestSchema(schema.RequestSchema):
-    """ RestartVMInstance - 重启虚拟机
-    """
+    """RestartVMInstance - 重启虚拟机"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class RestartVMInstanceResponseSchema(schema.ResponseSchema):
-    """ RestartVMInstance - 重启虚拟机
-    """
+    """RestartVMInstance - 重启虚拟机"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: RollbackResource
 
 恢复回收站资源
 """
 
 
 class RollbackResourceRequestSchema(schema.RequestSchema):
-    """ RollbackResource - 恢复回收站资源
-    """
+    """RollbackResource - 恢复回收站资源"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class RollbackResourceResponseSchema(schema.ResponseSchema):
-    """ RollbackResource - 恢复回收站资源
-    """
+    """RollbackResource - 恢复回收站资源"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: RollbackSnapshot
 
 将某个快照内的数据回滚到原云硬盘，仅支持正常状态的快照进行回滚操作，回滚时硬盘必须处于未绑定或其挂载的主机为关机状态。
 """
 
 
 class RollbackSnapshotRequestSchema(schema.RequestSchema):
-    """ RollbackSnapshot - 将某个快照内的数据回滚到原云硬盘，仅支持正常状态的快照进行回滚操作，回滚时硬盘必须处于未绑定或其挂载的主机为关机状态。
-    """
+    """RollbackSnapshot - 将某个快照内的数据回滚到原云硬盘，仅支持正常状态的快照进行回滚操作，回滚时硬盘必须处于未绑定或其挂载的主机为关机状态。"""
 
     fields = {
         "DiskID": fields.Str(required=True, dump_to="DiskID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SnapshotID": fields.Str(required=True, dump_to="SnapshotID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class RollbackSnapshotResponseSchema(schema.ResponseSchema):
-    """ RollbackSnapshot - 将某个快照内的数据回滚到原云硬盘，仅支持正常状态的快照进行回滚操作，回滚时硬盘必须处于未绑定或其挂载的主机为关机状态。
-    """
+    """RollbackSnapshot - 将某个快照内的数据回滚到原云硬盘，仅支持正常状态的快照进行回滚操作，回滚时硬盘必须处于未绑定或其挂载的主机为关机状态。"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: StartVMInstance
 
 开启虚拟机
 """
 
 
 class StartVMInstanceRequestSchema(schema.RequestSchema):
-    """ StartVMInstance - 开启虚拟机
-    """
+    """StartVMInstance - 开启虚拟机"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class StartVMInstanceResponseSchema(schema.ResponseSchema):
-    """ StartVMInstance - 开启虚拟机
-    """
+    """StartVMInstance - 开启虚拟机"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: StopVMInstance
 
 关闭虚拟机
 """
 
 
 class StopVMInstanceRequestSchema(schema.RequestSchema):
-    """ StopVMInstance - 关闭虚拟机
-    """
+    """StopVMInstance - 关闭虚拟机"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "VMID": fields.Str(required=True, dump_to="VMID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class StopVMInstanceResponseSchema(schema.ResponseSchema):
-    """ StopVMInstance - 关闭虚拟机
-    """
+    """StopVMInstance - 关闭虚拟机"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
         "VMID": fields.Str(required=False, load_from="VMID"),
     }
 
 
@@ -2741,158 +2565,147 @@
 API: TerminateResource
 
 销毁资源
 """
 
 
 class TerminateResourceRequestSchema(schema.RequestSchema):
-    """ TerminateResource - 销毁资源
-    """
+    """TerminateResource - 销毁资源"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class TerminateResourceResponseSchema(schema.ResponseSchema):
-    """ TerminateResource - 销毁资源
-    """
+    """TerminateResource - 销毁资源"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: UnBindEIP
 
 解绑外网IP
 """
 
 
 class UnBindEIPRequestSchema(schema.RequestSchema):
-    """ UnBindEIP - 解绑外网IP
-    """
+    """UnBindEIP - 解绑外网IP"""
 
     fields = {
         "EIPID": fields.Str(required=True, dump_to="EIPID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UnBindEIPResponseSchema(schema.ResponseSchema):
-    """ UnBindEIP - 解绑外网IP
-    """
+    """UnBindEIP - 解绑外网IP"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: UnBindSecurityGroup
 
 解绑安全组
 """
 
 
 class UnBindSecurityGroupRequestSchema(schema.RequestSchema):
-    """ UnBindSecurityGroup - 解绑安全组
-    """
+    """UnBindSecurityGroup - 解绑安全组"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "SGID": fields.Str(required=True, dump_to="SGID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UnBindSecurityGroupResponseSchema(schema.ResponseSchema):
-    """ UnBindSecurityGroup - 解绑安全组
-    """
+    """UnBindSecurityGroup - 解绑安全组"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: UnbindAlarmTemplate
 
 解绑告警模板
 """
 
 
 class UnbindAlarmTemplateRequestSchema(schema.RequestSchema):
-    """ UnbindAlarmTemplate - 解绑告警模板
-    """
+    """UnbindAlarmTemplate - 解绑告警模板"""
 
     fields = {
         "AlarmTemplateID": fields.Str(required=True, dump_to="AlarmTemplateID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceIDs": fields.List(fields.Str()),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UnbindAlarmTemplateResponseSchema(schema.ResponseSchema):
-    """ UnbindAlarmTemplate - 解绑告警模板
-    """
+    """UnbindAlarmTemplate - 解绑告警模板"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: UnbindPhysicalIP
 
 解绑物理IP
 """
 
 
 class UnbindPhysicalIPRequestSchema(schema.RequestSchema):
-    """ UnbindPhysicalIP - 解绑物理IP
-    """
+    """UnbindPhysicalIP - 解绑物理IP"""
 
     fields = {
         "PhysicalIPID": fields.Str(required=True, dump_to="PhysicalIPID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceID": fields.Str(required=True, dump_to="ResourceID"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UnbindPhysicalIPResponseSchema(schema.ResponseSchema):
-    """ UnbindPhysicalIP - 解绑物理IP
-    """
+    """UnbindPhysicalIP - 解绑物理IP"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: UpdateAlarmTemplateRule
 
 更新告警模板规则
 """
 
 
 class UpdateAlarmTemplateRuleRequestSchema(schema.RequestSchema):
-    """ UpdateAlarmTemplateRule - 更新告警模板规则
-    """
+    """UpdateAlarmTemplateRule - 更新告警模板规则"""
 
     fields = {
         "AlarmStrategy": fields.Str(required=True, dump_to="AlarmStrategy"),
         "AlarmTemplateID": fields.Str(required=True, dump_to="AlarmTemplateID"),
         "AlarmTemplateRuleID": fields.Str(
             required=True, dump_to="AlarmTemplateRuleID"
         ),
@@ -2904,91 +2717,85 @@
         "Threshold": fields.Str(required=True, dump_to="Threshold"),
         "TriggerCount": fields.Str(required=True, dump_to="TriggerCount"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpdateAlarmTemplateRuleResponseSchema(schema.ResponseSchema):
-    """ UpdateAlarmTemplateRule - 更新告警模板规则
-    """
+    """UpdateAlarmTemplateRule - 更新告警模板规则"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: UpdateRS
 
 修改负载均衡的服务节点
 """
 
 
 class UpdateRSRequestSchema(schema.RequestSchema):
-    """ UpdateRS - 修改负载均衡的服务节点
-    """
+    """UpdateRS - 修改负载均衡的服务节点"""
 
     fields = {
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Port": fields.Int(required=False, dump_to="Port"),
         "RSID": fields.Str(required=True, dump_to="RSID"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Weight": fields.Int(required=False, dump_to="Weight"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpdateRSResponseSchema(schema.ResponseSchema):
-    """ UpdateRS - 修改负载均衡的服务节点
-    """
+    """UpdateRS - 修改负载均衡的服务节点"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: UpdateSecurityGroupRule
 
 修改安全组规则
 """
 
 
 class UpdateSecurityGroupRuleRequestSchema(schema.RequestSchema):
-    """ UpdateSecurityGroupRule - 修改安全组规则
-    """
+    """UpdateSecurityGroupRule - 修改安全组规则"""
 
     fields = {
         "Region": fields.Str(required=True, dump_to="Region"),
         "Rules": fields.List(fields.Str()),
         "SGID": fields.Str(required=True, dump_to="SGID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpdateSecurityGroupRuleResponseSchema(schema.ResponseSchema):
-    """ UpdateSecurityGroupRule - 修改安全组规则
-    """
+    """UpdateSecurityGroupRule - 修改安全组规则"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
 """
 API: UpdateVS
 
 修改负载均衡VServer
 """
 
 
 class UpdateVSRequestSchema(schema.RequestSchema):
-    """ UpdateVS - 修改负载均衡VServer
-    """
+    """UpdateVS - 修改负载均衡VServer"""
 
     fields = {
         "CACertificateID": fields.Str(
             required=False, dump_to="CACertificateID"
         ),
         "Domain": fields.Str(required=False, dump_to="Domain"),
         "HealthcheckType": fields.Str(
@@ -3012,75 +2819,70 @@
         ),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpdateVSResponseSchema(schema.ResponseSchema):
-    """ UpdateVS - 修改负载均衡VServer
-    """
+    """UpdateVS - 修改负载均衡VServer"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: UpdateVSPolicy
 
 更新七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
 """
 
 
 class UpdateVSPolicyRequestSchema(schema.RequestSchema):
-    """ UpdateVSPolicy - 更新七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """UpdateVSPolicy - 更新七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "Domain": fields.Str(required=False, dump_to="Domain"),
         "LBID": fields.Str(required=True, dump_to="LBID"),
         "Path": fields.Str(required=False, dump_to="Path"),
         "PolicyID": fields.Str(required=True, dump_to="PolicyID"),
         "RSIDs": fields.List(fields.Str()),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VSID": fields.Str(required=True, dump_to="VSID"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpdateVSPolicyResponseSchema(schema.ResponseSchema):
-    """ UpdateVSPolicy - 更新七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。
-    """
+    """UpdateVSPolicy - 更新七层负载均衡内容转发规则，仅当 VServer 的监听协议为 HTTP 时有效。"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: UpgradeDisk
 
 扩容硬盘，为保证数据完整性，容量扩容前建议暂停对当前硬盘的所有文件系统读写操作，并进入操作系统进行 `umount ` 或`脱机` 操作。
 """
 
 
 class UpgradeDiskRequestSchema(schema.RequestSchema):
-    """ UpgradeDisk - 扩容硬盘，为保证数据完整性，容量扩容前建议暂停对当前硬盘的所有文件系统读写操作，并进入操作系统进行 `umount ` 或`脱机` 操作。
-    """
+    """UpgradeDisk - 扩容硬盘，为保证数据完整性，容量扩容前建议暂停对当前硬盘的所有文件系统读写操作，并进入操作系统进行 `umount ` 或`脱机` 操作。"""
 
     fields = {
         "DiskID": fields.Str(required=True, dump_to="DiskID"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpgradeDiskResponseSchema(schema.ResponseSchema):
-    """ UpgradeDisk - 扩容硬盘，为保证数据完整性，容量扩容前建议暂停对当前硬盘的所有文件系统读写操作，并进入操作系统进行 `umount ` 或`脱机` 操作。
-    """
+    """UpgradeDisk - 扩容硬盘，为保证数据完整性，容量扩容前建议暂停对当前硬盘的所有文件系统读写操作，并进入操作系统进行 `umount ` 或`脱机` 操作。"""
 
     fields = {
         "Action": fields.Str(required=True, load_from="Action"),
         "Message": fields.Str(required=True, load_from="Message"),
         "RetCode": fields.Int(required=True, load_from="RetCode"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ucloudstack/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ucloudstack/schemas/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class BindVSInfoSchema(schema.ResponseSchema):
-    """ BindVSInfo - 证书绑定的vs信息
-    """
+    """BindVSInfo - 证书绑定的vs信息"""
 
     fields = {
         "LBID": fields.Str(required=False, load_from="LBID"),
         "LBName": fields.Str(required=False, load_from="LBName"),
         "Port": fields.Int(required=False, load_from="Port"),
         "Protocol": fields.Str(required=False, load_from="Protocol"),
         "VSID": fields.Str(required=False, load_from="VSID"),
     }
 
 
 class CertificateInfoSchema(schema.ResponseSchema):
-    """ CertificateInfo - 证书信息
-    """
+    """CertificateInfo - 证书信息"""
 
     fields = {
         "CertificateContent": fields.Str(
             required=False, load_from="CertificateContent"
         ),
         "CertificateID": fields.Str(required=False, load_from="CertificateID"),
         "CertificateType": fields.Str(
@@ -39,16 +37,15 @@
         "SubjectAlternativeNames": fields.List(fields.Str()),
         "VSInfos": fields.List(BindVSInfoSchema()),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class DiskInfoSchema(schema.ResponseSchema):
-    """ DiskInfo - 磁盘信息
-    """
+    """DiskInfo - 磁盘信息"""
 
     fields = {
         "AttachResourceID": fields.Str(
             required=True, load_from="AttachResourceID"
         ),
         "ChargeType": fields.Str(required=True, load_from="ChargeType"),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
@@ -62,16 +59,15 @@
         "SetType": fields.Str(required=True, load_from="SetType"),
         "Size": fields.Int(required=True, load_from="Size"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class EIPInfoSchema(schema.ResponseSchema):
-    """ EIPInfo - 外网IP信息
-    """
+    """EIPInfo - 外网IP信息"""
 
     fields = {
         "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
         "BindResourceID": fields.Str(
             required=False, load_from="BindResourceID"
         ),
         "BindResourceType": fields.Str(
@@ -91,16 +87,15 @@
         "Remark": fields.Str(required=False, load_from="Remark"),
         "Status": fields.Str(required=False, load_from="Status"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class ImageInfoSchema(schema.ResponseSchema):
-    """ ImageInfo - 镜像信息
-    """
+    """ImageInfo - 镜像信息"""
 
     fields = {
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "ImageID": fields.Str(required=True, load_from="ImageID"),
         "ImageStatus": fields.Str(required=True, load_from="ImageStatus"),
         "ImageType": fields.Str(required=True, load_from="ImageType"),
         "Name": fields.Str(required=True, load_from="Name"),
@@ -110,16 +105,15 @@
         "Region": fields.Str(required=True, load_from="Region"),
         "SetArch": fields.Str(required=True, load_from="SetArch"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class LBInfoSchema(schema.ResponseSchema):
-    """ LBInfo - 负载均衡信息
-    """
+    """LBInfo - 负载均衡信息"""
 
     fields = {
         "AlarmTemplateID": fields.Str(
             required=True, load_from="AlarmTemplateID"
         ),
         "ChargeType": fields.Str(required=True, load_from="ChargeType"),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
@@ -137,36 +131,33 @@
         "VPCID": fields.Str(required=True, load_from="VPCID"),
         "VSCount": fields.Int(required=True, load_from="VSCount"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class MetricSetSchema(schema.ResponseSchema):
-    """ MetricSet - 监控值
-    """
+    """MetricSet - 监控值"""
 
     fields = {
         "Timestamp": fields.Int(required=False, load_from="Timestamp"),
         "Value": fields.Float(required=False, load_from="Value"),
     }
 
 
 class MetricInfoSchema(schema.ResponseSchema):
-    """ MetricInfo - 监控信息
-    """
+    """MetricInfo - 监控信息"""
 
     fields = {
         "Infos": fields.List(MetricSetSchema()),
         "MetricName": fields.Str(required=False, load_from="MetricName"),
     }
 
 
 class NATGWInfoSchema(schema.ResponseSchema):
-    """ NATGWInfo - NAT网关信息
-    """
+    """NATGWInfo - NAT网关信息"""
 
     fields = {
         "AlarmTemplateID": fields.Str(
             required=True, load_from="AlarmTemplateID"
         ),
         "ChargeType": fields.Str(required=True, load_from="ChargeType"),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
@@ -181,16 +172,15 @@
         "SubnetID": fields.Str(required=True, load_from="SubnetID"),
         "VPCID": fields.Str(required=True, load_from="VPCID"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class NATGWRuleInfoSchema(schema.ResponseSchema):
-    """ NATGWRuleInfo - NAT网关关联的白名单资源信息
-    """
+    """NATGWRuleInfo - NAT网关关联的白名单资源信息"""
 
     fields = {
         "BindResourceID": fields.Str(required=True, load_from="BindResourceID"),
         "BindResourceType": fields.Str(
             required=True, load_from="BindResourceType"
         ),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
@@ -200,16 +190,15 @@
         "Name": fields.Str(required=True, load_from="Name"),
         "RuleID": fields.Str(required=True, load_from="RuleID"),
         "RuleStatus": fields.Str(required=True, load_from="RuleStatus"),
     }
 
 
 class NICInfoSchema(schema.ResponseSchema):
-    """ NICInfo - 网卡信息
-    """
+    """NICInfo - 网卡信息"""
 
     fields = {
         "BindResourceID": fields.Str(required=True, load_from="BindResourceID"),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "IP": fields.Str(required=True, load_from="IP"),
         "MAC": fields.Str(required=True, load_from="MAC"),
         "NICID": fields.Str(required=True, load_from="NICID"),
@@ -221,16 +210,15 @@
         "SubnetID": fields.Str(required=True, load_from="SubnetID"),
         "VPCID": fields.Str(required=True, load_from="VPCID"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class OPLogInfoSchema(schema.ResponseSchema):
-    """ OPLogInfo - 操作日志
-    """
+    """OPLogInfo - 操作日志"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "IsSuccess": fields.Str(required=False, load_from="IsSuccess"),
         "OPLogsID": fields.Str(required=False, load_from="OPLogsID"),
         "OPName": fields.Str(required=False, load_from="OPName"),
         "OPTime": fields.Int(required=False, load_from="OPTime"),
@@ -241,16 +229,15 @@
         "RetCode": fields.Int(required=False, load_from="RetCode"),
         "UserEmail": fields.Str(required=False, load_from="UserEmail"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class PhysicalIPInfoSchema(schema.ResponseSchema):
-    """ PhysicalIPInfo - 物理IP信息
-    """
+    """PhysicalIPInfo - 物理IP信息"""
 
     fields = {
         "BindResourceID": fields.Str(required=True, load_from="BindResourceID"),
         "BindResourceType": fields.Str(
             required=True, load_from="BindResourceType"
         ),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
@@ -263,16 +250,15 @@
         "Status": fields.Str(required=True, load_from="Status"),
         "UpdateTime": fields.Int(required=True, load_from="UpdateTime"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class RSInfoSchema(schema.ResponseSchema):
-    """ RSInfo - 转发规则关联的服务节点信息
-    """
+    """RSInfo - 转发规则关联的服务节点信息"""
 
     fields = {
         "BindResourceID": fields.Str(required=True, load_from="BindResourceID"),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "IP": fields.Str(required=True, load_from="IP"),
         "LBID": fields.Str(required=True, load_from="LBID"),
         "Name": fields.Str(required=True, load_from="Name"),
@@ -283,16 +269,15 @@
         "UpdateTime": fields.Int(required=True, load_from="UpdateTime"),
         "VSID": fields.Str(required=True, load_from="VSID"),
         "Weight": fields.Int(required=True, load_from="Weight"),
     }
 
 
 class RecycledResourceInfoSchema(schema.ResponseSchema):
-    """ RecycledResourceInfo - 回收站资源信息
-    """
+    """RecycledResourceInfo - 回收站资源信息"""
 
     fields = {
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "DeleteTime": fields.Int(required=True, load_from="DeleteTime"),
         "Description": fields.Str(required=True, load_from="Description"),
         "ExpireTime": fields.Int(required=True, load_from="ExpireTime"),
         "IsAutoTerminated": fields.Bool(
@@ -307,31 +292,29 @@
             required=True, load_from="WillTerminateTime"
         ),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class SGRuleInfoSchema(schema.ResponseSchema):
-    """ SGRuleInfo - 安全组规则信息
-    """
+    """SGRuleInfo - 安全组规则信息"""
 
     fields = {
         "DstPort": fields.Str(required=False, load_from="DstPort"),
         "IsIn": fields.Str(required=False, load_from="IsIn"),
         "Priority": fields.Str(required=False, load_from="Priority"),
         "ProtocolType": fields.Str(required=False, load_from="ProtocolType"),
         "RuleAction": fields.Str(required=False, load_from="RuleAction"),
         "RuleID": fields.Str(required=False, load_from="RuleID"),
         "SrcIP": fields.Str(required=False, load_from="SrcIP"),
     }
 
 
 class SGInfoSchema(schema.ResponseSchema):
-    """ SGInfo - 安全组信息
-    """
+    """SGInfo - 安全组信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Region": fields.Str(required=False, load_from="Region"),
         "Remark": fields.Str(required=False, load_from="Remark"),
         "ResourceCount": fields.Int(required=False, load_from="ResourceCount"),
@@ -341,29 +324,27 @@
         "Status": fields.Str(required=False, load_from="Status"),
         "UpdateTime": fields.Int(required=False, load_from="UpdateTime"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class SGResourceInfoSchema(schema.ResponseSchema):
-    """ SGResourceInfo - 安全组绑定的资源信息
-    """
+    """SGResourceInfo - 安全组绑定的资源信息"""
 
     fields = {
         "Name": fields.Str(required=True, load_from="Name"),
         "Region": fields.Str(required=True, load_from="Region"),
         "ResourceID": fields.Str(required=True, load_from="ResourceID"),
         "ResourceType": fields.Str(required=True, load_from="ResourceType"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class SnapshotInfoSchema(schema.ResponseSchema):
-    """ SnapshotInfo - 快照的详细信息
-    """
+    """SnapshotInfo - 快照的详细信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "DiskID": fields.Str(required=False, load_from="DiskID"),
         "DiskType": fields.Str(required=False, load_from="DiskType"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Region": fields.Str(required=False, load_from="Region"),
@@ -373,31 +354,29 @@
             required=False, load_from="SnapshotStatus"
         ),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class StorageTypeInfoSchema(schema.ResponseSchema):
-    """ StorageTypeInfo - 存储类型信息
-    """
+    """StorageTypeInfo - 存储类型信息"""
 
     fields = {
         "Region": fields.Str(required=True, load_from="Region"),
         "SetArch": fields.Str(required=True, load_from="SetArch"),
         "StorageType": fields.Str(required=True, load_from="StorageType"),
         "StorageTypeAlias": fields.Str(
             required=True, load_from="StorageTypeAlias"
         ),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class SubnetInfoSchema(schema.ResponseSchema):
-    """ SubnetInfo - 子网信息
-    """
+    """SubnetInfo - 子网信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Network": fields.Str(required=False, load_from="Network"),
         "Region": fields.Str(required=False, load_from="Region"),
         "Remark": fields.Str(required=False, load_from="Remark"),
@@ -405,46 +384,43 @@
         "SubnetID": fields.Str(required=False, load_from="SubnetID"),
         "UpdateTime": fields.Int(required=False, load_from="UpdateTime"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UserInfoSchema(schema.ResponseSchema):
-    """ UserInfo - 租户信息
-    """
+    """UserInfo - 租户信息"""
 
     fields = {
         "Amount": fields.Float(required=False, load_from="Amount"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Email": fields.Str(required=False, load_from="Email"),
         "PrivateKey": fields.Str(required=False, load_from="PrivateKey"),
         "PublicKey": fields.Str(required=False, load_from="PublicKey"),
         "Status": fields.Str(required=False, load_from="Status"),
         "UpdateTime": fields.Int(required=False, load_from="UpdateTime"),
         "UserID": fields.Int(required=False, load_from="UserID"),
     }
 
 
 class VMDiskInfoSchema(schema.ResponseSchema):
-    """ VMDiskInfo - 虚拟机磁盘信息
-    """
+    """VMDiskInfo - 虚拟机磁盘信息"""
 
     fields = {
         "DiskID": fields.Str(required=False, load_from="DiskID"),
         "Drive": fields.Str(required=False, load_from="Drive"),
         "IsElastic": fields.Str(required=False, load_from="IsElastic"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Size": fields.Int(required=False, load_from="Size"),
         "Type": fields.Str(required=False, load_from="Type"),
     }
 
 
 class VMIPInfoSchema(schema.ResponseSchema):
-    """ VMIPInfo - 虚拟机IP信息
-    """
+    """VMIPInfo - 虚拟机IP信息"""
 
     fields = {
         "IP": fields.Str(required=False, load_from="IP"),
         "IPVersion": fields.Str(required=False, load_from="IPVersion"),
         "InterfaceID": fields.Str(required=False, load_from="InterfaceID"),
         "IsElastic": fields.Str(required=False, load_from="IsElastic"),
         "MAC": fields.Str(required=False, load_from="MAC"),
@@ -455,16 +431,15 @@
         "Type": fields.Str(required=False, load_from="Type"),
         "VPCID": fields.Str(required=False, load_from="VPCID"),
         "VPCName": fields.Str(required=False, load_from="VPCName"),
     }
 
 
 class VMInstanceInfoSchema(schema.ResponseSchema):
-    """ VMInstanceInfo - UCloudStack虚拟机信息
-    """
+    """VMInstanceInfo - UCloudStack虚拟机信息"""
 
     fields = {
         "CPU": fields.Int(required=False, load_from="CPU"),
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "DiskInfos": fields.List(VMDiskInfoSchema()),
         "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
@@ -485,29 +460,27 @@
         "VPCID": fields.Str(required=False, load_from="VPCID"),
         "VPCName": fields.Str(required=False, load_from="VPCName"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class VMTypeInfoSchema(schema.ResponseSchema):
-    """ VMTypeInfo - 主机机型信息
-    """
+    """VMTypeInfo - 主机机型信息"""
 
     fields = {
         "Region": fields.Str(required=True, load_from="Region"),
         "SetArch": fields.Str(required=True, load_from="SetArch"),
         "VMType": fields.Str(required=True, load_from="VMType"),
         "VMTypeAlias": fields.Str(required=True, load_from="VMTypeAlias"),
         "Zone": fields.Str(required=True, load_from="Zone"),
     }
 
 
 class VPCInfoSchema(schema.ResponseSchema):
-    """ VPCInfo - VPC信息
-    """
+    """VPCInfo - VPC信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Network": fields.Str(required=False, load_from="Network"),
         "Region": fields.Str(required=False, load_from="Region"),
         "Remark": fields.Str(required=False, load_from="Remark"),
@@ -517,16 +490,15 @@
         "UpdateTime": fields.Int(required=False, load_from="UpdateTime"),
         "VPCID": fields.Str(required=False, load_from="VPCID"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class VSPolicyInfoSchema(schema.ResponseSchema):
-    """ VSPolicyInfo - 内容转发规则信息
-    """
+    """VSPolicyInfo - 内容转发规则信息"""
 
     fields = {
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "Domain": fields.Str(required=True, load_from="Domain"),
         "LBID": fields.Str(required=True, load_from="LBID"),
         "Path": fields.Str(required=True, load_from="Path"),
         "PolicyID": fields.Str(required=True, load_from="PolicyID"),
@@ -534,16 +506,15 @@
         "RSInfos": fields.List(RSInfoSchema()),
         "UpdateTime": fields.Int(required=True, load_from="UpdateTime"),
         "VSID": fields.Str(required=True, load_from="VSID"),
     }
 
 
 class VSInfoSchema(schema.ResponseSchema):
-    """ VSInfo - VServer信息
-    """
+    """VSInfo - VServer信息"""
 
     fields = {
         "AlarmTemplateID": fields.Str(
             required=True, load_from="AlarmTemplateID"
         ),
         "CACertificateID": fields.Str(
             required=False, load_from="CACertificateID"
@@ -577,14 +548,13 @@
         "VSID": fields.Str(required=True, load_from="VSID"),
         "VSPolicyInfos": fields.List(VSPolicyInfoSchema()),
         "VSStatus": fields.Str(required=True, load_from="VSStatus"),
     }
 
 
 class PriceInfoSchema(schema.ResponseSchema):
-    """ PriceInfo - 价格信息
-    """
+    """PriceInfo - 价格信息"""
 
     fields = {
         "ChargeType": fields.Str(required=True, load_from="ChargeType"),
         "Price": fields.Float(required=True, load_from="Price"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udb/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udb/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,31 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UDBClient, self).__init__(config, transport, middleware, logger)
 
     def backup_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BackupUDBInstance - 备份UDB实例
+        """BackupUDBInstance - 备份UDB实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupName** (str) - (Required) 备份名称
         - **DBId** (str) - (Required) DB实例Id,该值可以通过DescribeUDBInstance获取
         - **BackupMethod** (str) - 使用的备份方式。（快照备份即物理备份。注意只有SSD版本的mysql实例支持设置为snapshot）
         - **Blacklist** (str) - 备份黑名单列表，以 ; 分隔。注意：只有逻辑备份下备份黑名单才生效，快照备份备份黑名单下无效
         - **ForceBackup** (bool) - true表示逻辑备份时是使用 --force 参数，false表示不使用 --force 参数。物理备份此参数无效。
         - **UseBlacklist** (bool) - 是否使用黑名单备份，默认false
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.BackupUDBInstanceRequestSchema().dumps(d)
 
         # build options
@@ -44,186 +44,186 @@
 
         resp = self.invoke("BackupUDBInstance", d, **kwargs)
         return apis.BackupUDBInstanceResponseSchema().loads(resp)
 
     def backup_udb_instance_binlog(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BackupUDBInstanceBinlog - 备份UDB指定时间段的binlog列表
+        """BackupUDBInstanceBinlog - 备份UDB指定时间段的binlog列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupFile** (str) - (Required) 需要备份文件,可通过DescribeUDBInstanceBinlog获得 如果要传入多个文件名，以空格键分割,用单引号包含.
         - **DBId** (str) - (Required) DB实例Id,该值可以通过DescribeUDBInstance获取
         - **BackupName** (str) - DB备份文件名称
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.BackupUDBInstanceBinlogRequestSchema().dumps(d)
 
         resp = self.invoke("BackupUDBInstanceBinlog", d, **kwargs)
         return apis.BackupUDBInstanceBinlogResponseSchema().loads(resp)
 
     def backup_udb_instance_error_log(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BackupUDBInstanceErrorLog - 备份UDB指定时间段的errorlog
+        """BackupUDBInstanceErrorLog - 备份UDB指定时间段的errorlog
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupName** (str) - (Required) 备份名称
         - **DBId** (str) - (Required) DB实例Id,该值可以通过DescribeUDBInstance获取
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.BackupUDBInstanceErrorLogRequestSchema().dumps(d)
 
         resp = self.invoke("BackupUDBInstanceErrorLog", d, **kwargs)
         return apis.BackupUDBInstanceErrorLogResponseSchema().loads(resp)
 
     def backup_udb_instance_slow_log(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ BackupUDBInstanceSlowLog - 备份UDB指定时间段的slowlog分析结果
+        """BackupUDBInstanceSlowLog - 备份UDB指定时间段的slowlog分析结果
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupName** (str) - (Required) 备份文件名称
         - **BeginTime** (int) - (Required) 过滤条件:起始时间(时间戳)
         - **DBId** (str) - (Required) DB实例Id,该值可以通过DescribeUDBInstance获取
         - **EndTime** (int) - (Required) 过滤条件:结束时间(时间戳)
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.BackupUDBInstanceSlowLogRequestSchema().dumps(d)
 
         resp = self.invoke("BackupUDBInstanceSlowLog", d, **kwargs)
         return apis.BackupUDBInstanceSlowLogResponseSchema().loads(resp)
 
     def check_recover_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CheckRecoverUDBInstance - 核查db是否可以使用回档功能
+        """CheckRecoverUDBInstance - 核查db是否可以使用回档功能
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SrcDBId** (str) - (Required) 源实例的Id(只支持普通版DB不支持高可用)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **LastestTime** (int) - 核查成功返回值为可以回档到的最近时刻,核查失败不返回
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CheckRecoverUDBInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("CheckRecoverUDBInstance", d, **kwargs)
         return apis.CheckRecoverUDBInstanceResponseSchema().loads(resp)
 
     def check_udb_instance_to_ha_allowance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CheckUDBInstanceToHAAllowance - 核查db是否可以升级为高可用
+        """CheckUDBInstanceToHAAllowance - 核查db是否可以升级为高可用
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
-        
+
         **Response**
 
         - **Allowance** (str) - Yes ，No ，Yes即可以升级，No为不可以升级
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CheckUDBInstanceToHAAllowanceRequestSchema().dumps(d)
 
         resp = self.invoke("CheckUDBInstanceToHAAllowance", d, **kwargs)
         return apis.CheckUDBInstanceToHAAllowanceResponseSchema().loads(resp)
 
     def clear_udb_log(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ClearUDBLog - 清除UDB实例的log
+        """ClearUDBLog - 清除UDB实例的log
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) DB实例的id,该值可以通过DescribeUDBInstance获取
         - **LogType** (int) - (Required) 日志类型，10-error（暂不支持）、20-slow（暂不支持 ）、30-binlog
         - **BeforeTime** (int) - 删除时间点(至少前一天)之前log，采用时间戳(秒)，默认当 前时间点前一天
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ClearUDBLogRequestSchema().dumps(d)
 
         resp = self.invoke("ClearUDBLog", d, **kwargs)
         return apis.ClearUDBLogResponseSchema().loads(resp)
 
     def create_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUDBInstance - 创建UDB实例（包括创建mysql master节点、mongodb primary/configsvr节点和从备份恢复实例）
+        """CreateUDBInstance - 创建UDB实例（包括创建mysql master节点、mongodb primary/configsvr节点和从备份恢复实例）
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **AdminPassword** (str) - (Required) 管理员密码
         - **DBTypeId** (str) - (Required) DB类型id，mysql/mongodb/postgesql按版本细分 1：mysql-5.1，2：mysql-5.5，3：percona-5.5，4：mysql-5.6，5：percona-5.6，6：mysql-5.7，7：percona-5.7，8：mariadb-10.0，9：mongodb-2.4，10：mongodb-2.6，11：mongodb-3.0，12：mongodb-3.2,13：postgresql-9.4，14：postgresql-9.6，14：postgresql-10.4
         - **DiskSpace** (int) - (Required) 磁盘空间(GB), 暂时支持20G - 3000G
         - **MemoryLimit** (int) - (Required) 内存限制(MB)，目前支持以下几档 1000M/2000M/4000M/ 6000M/8000M/12000M/16000M/ 24000M/32000M/48000M/ 64000M/96000M
         - **Name** (str) - (Required) 实例名称，至少6位
         - **ParamGroupId** (int) - (Required) DB实例使用的配置参数组id
         - **Port** (int) - (Required) 端口号，mysql默认3306，mongodb默认27017，postgresql默认5432
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **AdminUser** (str) - 管理员帐户名，默认root
         - **BackupCount** (int) - 备份策略，每周备份数量，默认7次
         - **BackupDuration** (int) - 备份策略，备份时间间隔，单位小时计，默认24小时
         - **BackupId** (int) - 备份id，如果指定，则表明从备份恢复实例
         - **BackupTime** (int) - 备份策略，备份开始时间，单位小时计，默认1点
-        - **BackupZone** (str) - 跨可用区高可用备库所在可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **BackupZone** (str) - 跨可用区高可用备库所在可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **CPU** (int) - cpu核数
         - **ChargeType** (str) - Year， Month， Dynamic，Trial，默认: Month
         - **ClusterRole** (str) - 当DB类型(DBTypeId)为mongodb时，需要指定mongo的角色，可选值为configsrv (配置节点)，shardsrv (数据节点)
         - **CouponId** (str) - 使用的代金券id
         - **DisableSemisync** (bool) - 是否开启异步高可用，默认不填，可置为true
         - **HAArch** (str) - 高可用架构:1） haproxy（默认）: 当前仅支持mysql。2） sentinel: 基于vip和哨兵节点的架构，当前支持mysql和pg。
         - **InstanceMode** (str) - UDB实例模式类型, 可选值如下: "Normal": 普通版UDB实例 "HA": 高可用版UDB实例 默认是"Normal"
@@ -231,19 +231,19 @@
         - **Quantity** (int) - 购买时长，默认值1
         - **SSDType** (str) - SSD类型，可选值为"SATA"、"PCI-E"，如果UseSSD为true ，则必选
         - **SubnetId** (str) - 子网ID
         - **Tag** (str) - 实例所在的业务组名称
         - **UDBCId** (str) - 专区ID信息（如果这个参数存在这说明是在专区中创建DB）
         - **UseSSD** (bool) - 是否使用SSD，默认为false。目前主要可用区、海外机房、新机房只提供SSD资源，非SSD资源不再提供。
         - **VPCId** (str) - VPC的ID
-        
+
         **Response**
 
         - **DBId** (str) - BD实例id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDBInstanceRequestSchema().dumps(d)
 
         # build options
@@ -251,36 +251,36 @@
 
         resp = self.invoke("CreateUDBInstance", d, **kwargs)
         return apis.CreateUDBInstanceResponseSchema().loads(resp)
 
     def create_udb_instance_by_recovery(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUDBInstanceByRecovery - 创建db，将新创建的db恢复到指定db某个指定时间点
+        """CreateUDBInstanceByRecovery - 创建db，将新创建的db恢复到指定db某个指定时间点
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 实例名称，至少6位
         - **RecoveryTime** (int) - (Required) 恢复到某个时间点的时间戳(UTC时间格式，默认单位秒)
         - **SrcDBId** (str) - (Required) 源实例的Id
         - **ChargeType** (str) - Year， Month， Dynamic，Trial，默认: Dynamic
         - **CouponId** (str) - 使用的代金券id
         - **Quantity** (int) - 购买时长，默认值1
         - **SubnetId** (str) - 子网ID
         - **UDBCId** (str) - 专区的Id
         - **UseSSD** (bool) - 指定是否是否使用SSD，默认使用主库的配置
         - **VPCId** (str) - VPC的ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DBId** (str) - db实例id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDBInstanceByRecoveryRequestSchema().dumps(d)
 
         # build options
@@ -288,31 +288,31 @@
 
         resp = self.invoke("CreateUDBInstanceByRecovery", d, **kwargs)
         return apis.CreateUDBInstanceByRecoveryResponseSchema().loads(resp)
 
     def create_udb_param_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUDBParamGroup - 从已有配置文件创建新配置文件
+        """CreateUDBParamGroup - 从已有配置文件创建新配置文件
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBTypeId** (str) - (Required) DB类型id，mysql/mongodb/postgesql按版本细分 1：mysql-5.1，2：mysql-5.5，3：percona-5.5，4：mysql-5.6，5：percona-5.6，6：mysql-5.7，7：percona-5.7，8：mariadb-10.0，9：mongodb-2.4，10：mongodb-2.6，11：mongodb-3.0，12：mongodb-3.2,13：postgresql-9.4，14：postgresql-9.6
         - **Description** (str) - (Required) 参数组描述
         - **GroupName** (str) - (Required) 新配置参数组名称
         - **SrcGroupId** (int) - (Required) 源参数组id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **RegionFlag** (bool) - 是否是地域级别的配置文件，默认是false
-        
+
         **Response**
 
         - **GroupId** (int) - 新配置参数组id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDBParamGroupRequestSchema().dumps(d)
 
         # build options
@@ -320,32 +320,32 @@
 
         resp = self.invoke("CreateUDBParamGroup", d, **kwargs)
         return apis.CreateUDBParamGroupResponseSchema().loads(resp)
 
     def create_udb_replication_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUDBReplicationInstance - 创建MongoDB的副本节点（包括仲裁）
+        """CreateUDBReplicationInstance - 创建MongoDB的副本节点（包括仲裁）
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 实例名称，至少6位
         - **SrcId** (str) - (Required) primary节点的DBId,该值可以通过DescribeUDBInstance获取
         - **CouponId** (str) - 使用的代金券id
         - **IsArbiter** (bool) - 是否是仲裁节点，默认false，仲裁节点按最小机型创建
         - **Port** (int) - 端口号，默认27017，取值范围3306至65535。
         - **UseSSD** (bool) - 是否使用SSD，默认不使用
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DBId** (str) - 创建从节点的DBId
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDBReplicationInstanceRequestSchema().dumps(d)
 
         # build options
@@ -353,37 +353,37 @@
 
         resp = self.invoke("CreateUDBReplicationInstance", d, **kwargs)
         return apis.CreateUDBReplicationInstanceResponseSchema().loads(resp)
 
     def create_udb_route_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUDBRouteInstance - 创建mongos实例
+        """CreateUDBRouteInstance - 创建mongos实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ConfigsvrId** (list) - (Required) 配置服务器的dbid，允许一个或者三个。
         - **DBTypeId** (str) - (Required) DB类型id，mongodb按版本细分有1：mongodb-2.4，2：mongodb-2.6,3：mongodb-3.0，4：mongodb-3.2
         - **DiskSpace** (int) - (Required) 磁盘空间(GB), 暂时支持20G - 500G
         - **MemoryLimit** (int) - (Required) 内存限制(MB)，目前支持以下几档 600M/1500M/3000M /6000M/15000M/30000M
         - **Name** (str) - (Required) 实例名称，至少6位
         - **ParamGroupId** (int) - (Required) DB实例使用的配置参数组id
         - **Port** (int) - (Required) 端口号，mongodb默认27017
         - **ChargeType** (str) - Year， Month， Dynamic，Trial，默认: Month
         - **CouponId** (str) - 使用的代金券id
         - **Quantity** (int) - 购买时长，默认值1
         - **UseSSD** (bool) - 是否使用SSD，默认为false
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DBId** (str) - db实例id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDBRouteInstanceRequestSchema().dumps(d)
 
         # build options
@@ -391,37 +391,37 @@
 
         resp = self.invoke("CreateUDBRouteInstance", d, **kwargs)
         return apis.CreateUDBRouteInstanceResponseSchema().loads(resp)
 
     def create_udb_slave(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUDBSlave - 创建UDB实例的slave
+        """CreateUDBSlave - 创建UDB实例的slave
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 实例名称，至少6位
         - **SrcId** (str) - (Required) master实例的DBId,该值可以通过DescribeUDBInstance获取
         - **CouponId** (str) - 使用的代金券id
         - **DiskSpace** (int) - 磁盘空间(GB), 暂时支持20G - 3000G（API支持，前端暂时只开放内存定制）
         - **InstanceMode** (str) - UDB实例部署模式，可选值如下：Normal: 普通单点实例HA: 高可用部署实例
         - **InstanceType** (str) - UDB实例类型：Normal和SATA_SSD
         - **IsLock** (bool) - 是否锁主库，默认为true
         - **MemoryLimit** (int) - 内存限制(MB)，目前支持以下几档 1000M/2000M/4000M/ 6000M/8000M/12000M/16000M/ 24000M/32000M/48000M/ 64000M/96000M
         - **Port** (int) - 端口号，mysql默认3306
         - **SSDType** (str) - SSD类型，可选值为"SATA"、"PCI-E"，如果UseSSD为true ，则必选
         - **UseSSD** (bool) - 是否使用SSD，默认为false
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DBId** (str) - 创建slave的DBId
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDBSlaveRequestSchema().dumps(d)
 
         # build options
@@ -429,139 +429,139 @@
 
         resp = self.invoke("CreateUDBSlave", d, **kwargs)
         return apis.CreateUDBSlaveResponseSchema().loads(resp)
 
     def delete_udb_backup(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUDBBackup - 删除UDB实例备份
+        """DeleteUDBBackup - 删除UDB实例备份
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (int) - (Required) 备份id，可通过DescribeUDBBackup获得
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupZone** (str) - 跨可用区高可用备库所在可用区，参见［可用区列表］
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteUDBBackupRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUDBBackup", d, **kwargs)
         return apis.DeleteUDBBackupResponseSchema().loads(resp)
 
     def delete_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUDBInstance - 删除UDB实例
+        """DeleteUDBInstance - 删除UDB实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) DB实例的id,该值可以通过DescribeUDBInstance获取
         - **UDBCId** (str) - 专区ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteUDBInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUDBInstance", d, **kwargs)
         return apis.DeleteUDBInstanceResponseSchema().loads(resp)
 
     def delete_udb_log_package(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUDBLogPackage - 删除UDB日志包
+        """DeleteUDBLogPackage - 删除UDB日志包
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (int) - (Required) 日志包id，可通过DescribeUDBLogPackage获得
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupZone** (str) - 跨可用区高可用备库所在可用区
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteUDBLogPackageRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUDBLogPackage", d, **kwargs)
         return apis.DeleteUDBLogPackageResponseSchema().loads(resp)
 
     def delete_udb_param_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUDBParamGroup - 删除配置参数组
+        """DeleteUDBParamGroup - 删除配置参数组
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (int) - (Required) 参数组id,可通过DescribeUDBParamGroup获取
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **RegionFlag** (bool) - 是否属于地域级别
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteUDBParamGroupRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUDBParamGroup", d, **kwargs)
         return apis.DeleteUDBParamGroupResponseSchema().loads(resp)
 
     def describe_udb_backup(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBBackup - 列表UDB实例备份信息.Zone不填表示多可用区，填代表单可用区
+        """DescribeUDBBackup - 列表UDB实例备份信息.Zone不填表示多可用区，填代表单可用区
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - (Required) 分页显示的条目数，列表操作则指定
         - **Offset** (int) - (Required) 分页显示的起始偏移，列表操作则指定
         - **BackupId** (int) - 如果填了BackupId, 那么只拉取这个备份的记录
         - **BackupType** (int) - 备份类型,取值为0或1，0表示自动，1表示手动
         - **BeginTime** (int) - 过滤条件:起始时间(Unix时间戳)
         - **ClassType** (str) - 如果未指定GroupId，则可选是否选取特定DB类型的配置(sql, nosql, postgresql, sqlserver)
         - **DBId** (str) - DB实例Id，如果指定，则只获取该db的备份信息 该值可以通过DescribeUDBInstance获取
         - **EndTime** (int) - 过滤条件:结束时间(Unix时间戳)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UDBBackupSet** 模型定义
         - **TotalCount** (int) - 满足条件备份总数，如果指定dbid，则是该db备份总数
-        
+
         **Response Model**
-        
-        **UDBBackupSet** 
-        
+
+        **UDBBackupSet**
+
         - **BackupEndTime** (int) - 备份完成时间(Unix时间戳)
         - **BackupId** (int) - 备份id
         - **BackupName** (str) - 备份名称
         - **BackupSize** (int) - 备份文件大小(字节)
         - **BackupTime** (int) - 备份时间(Unix时间戳)
         - **BackupType** (int) - 备份类型,取值为0或1,0表示自动，1表示手动
         - **BackupZone** (str) - 跨机房高可用备库所在可用区
@@ -579,89 +579,89 @@
 
         resp = self.invoke("DescribeUDBBackup", d, **kwargs)
         return apis.DescribeUDBBackupResponseSchema().loads(resp)
 
     def describe_udb_backup_blacklist(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBBackupBlacklist - 获取UDB实例的备份黑名单
+        """DescribeUDBBackupBlacklist - 获取UDB实例的备份黑名单
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) DB实例Id,该值可以通过DescribeUDBInstance获取
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Blacklist** (str) - DB的黑名单列表, db.%为指定库 dbname.tablename为指定表
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBBackupBlacklistRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBBackupBlacklist", d, **kwargs)
         return apis.DescribeUDBBackupBlacklistResponseSchema().loads(resp)
 
     def describe_udb_binlog_backup_url(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBBinlogBackupURL - 获取UDB的Binlog备份地址
+        """DescribeUDBBinlogBackupURL - 获取UDB的Binlog备份地址
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (int) - (Required) DB实例binlog备份ID，可以从DescribeUDBLogPackage结果当中获得
         - **DBId** (str) - (Required) DB实例Id
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **BackupPath** (str) - DB实例备份文件的公网地址
         - **InnerBackupPath** (str) - DB实例备份文件的内网地址
-        
+
         """
         # build request
         d = {"Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBBinlogBackupURLRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBBinlogBackupURL", d, **kwargs)
         return apis.DescribeUDBBinlogBackupURLResponseSchema().loads(resp)
 
     def describe_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstance - 获取UDB实例信息，支持两类操作：（1）指定DBId用于获取该db的信息；（2）指定ClassType、Offset、Limit用于列表操作，查询某一个类型db。
+        """DescribeUDBInstance - 获取UDB实例信息，支持两类操作：（1）指定DBId用于获取该db的信息；（2）指定ClassType、Offset、Limit用于列表操作，查询某一个类型db。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ClassType** (str) - DB种类，如果是列表操作，则需要指定,不区分大小写，其取值如下：mysql: SQL；mongo: NOSQL；postgresql: postgresql
         - **DBId** (str) - DB实例id，如果指定则获取单个db实例的描述，否则为列表操作。 指定DBId时无需填写ClassType、Offset、Limit
         - **IncludeSlaves** (bool) - 当只获取这个特定DBId的信息时，如果有该选项，那么把这个DBId实例的所有从库信息一起拉取并返回
         - **IsInUDBC** (bool) - 是否查看专区里面DB
         - **Limit** (int) - 分页显示数量，列表操作时必填
         - **Offset** (int) - 分页显示起始偏移位置，列表操作时必填
         - **UDBCId** (str) - IsInUDBC为True,UDBCId为空，说明查看整个可用区的专区的db，如果UDBId不为空则只查看此专区下面的db
-        - **Zone** (str) - 可用区，不填时默认全部可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区，不填时默认全部可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UDBInstanceSet** 模型定义
         - **TotalCount** (int) - 用户db组的数量，对于 mysql: 主从结对数量，没有slave，则只有master mongodb: 副本集数量
-        
+
         **Response Model**
-        
-        **UDBSlaveInstanceSet** 
-        
+
+        **UDBSlaveInstanceSet**
+
         - **AdminUser** (str) - 管理员帐户名，默认root
         - **BackupBeginTime** (int) - 备份策略，不可修改，开始时间，单位小时计，默认3点
         - **BackupBlacklist** (str) - 备份策略，备份黑名单，mongodb则不适用
         - **BackupCount** (int) - 备份策略，不可修改，备份文件保留的数量，默认7次
         - **BackupDate** (str) - 备份日期标记位。共7位,每一位为一周中一天的备份情况 0表示关闭当天备份,1表示打开当天备份。最右边的一位 为星期天的备份开关，其余从右到左依次为星期一到星期 六的备份配置开关，每周必须至少设置两天备份。 例如：1100000 表示打开星期六和星期五的自动备份功能
         - **BackupDuration** (int) - 备份策略，一天内备份时间间隔，单位小时，默认24小时
         - **ChargeType** (str) - Year， Month， Dynamic，Trial，默认: Dynamic
@@ -691,16 +691,16 @@
         - **Tag** (str) - 获取资源其他信息
         - **UseSSD** (bool) - 是否使用SSD
         - **VPCId** (str) - VPC的ID
         - **VirtualIP** (str) - DB实例虚ip
         - **VirtualIPMac** (str) - DB实例虚ip的mac地址
         - **Zone** (str) - 可用区
 
-        **UDBInstanceSet** 
-        
+        **UDBInstanceSet**
+
         - **AdminUser** (str) - 管理员帐户名，默认root
         - **BackupBeginTime** (int) - 备份策略，不可修改，开始时间，单位小时计，默认3点
         - **BackupBlacklist** (str) - 备份策略，备份黑名单，mongodb则不适用
         - **BackupCount** (int) - 备份策略，不可修改，备份文件保留的数量，默认7次
         - **BackupDate** (str) - 备份日期标记位。共7位,每一位为一周中一天的备份情况 0表示关闭当天备份,1表示打开当天备份。最右边的一位 为星期天的备份开关，其余从右到左依次为星期一到星期 六的备份配置开关，每周必须至少设置两天备份。 例如：1100000 表示打开星期六和星期五的自动备份功能
         - **BackupDuration** (int) - 备份策略，一天内备份时间间隔，单位小时，默认24小时
         - **BackupZone** (str) - 跨可用区高可用备库所在可用区
@@ -744,88 +744,88 @@
 
         resp = self.invoke("DescribeUDBInstance", d, **kwargs)
         return apis.DescribeUDBInstanceResponseSchema().loads(resp)
 
     def describe_udb_instance_backup_state(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstanceBackupState - 获取UDB实例备份状态
+        """DescribeUDBInstanceBackupState - 获取UDB实例备份状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (int) - (Required) 备份记录ID
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupZone** (str) - 跨可用区高可用备库所在可用区，参见［可用区列表］
-        
+
         **Response**
 
-        - **BackupEndTime** (int) - 
-        - **BackupSize** (int) - 
+        - **BackupEndTime** (int) -
+        - **BackupSize** (int) -
         - **State** (str) - 备份状态 0 Backuping // 备份中 1 Success // 备份成功 2 Failed // 备份失败 3 Expired // 备份过期
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBInstanceBackupStateRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBInstanceBackupState", d, **kwargs)
         return apis.DescribeUDBInstanceBackupStateResponseSchema().loads(resp)
 
     def describe_udb_instance_backup_url(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstanceBackupURL - 获取UDB备份下载地址
+        """DescribeUDBInstanceBackupURL - 获取UDB备份下载地址
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (int) - (Required) DB实例备份ID,该值可以通过DescribeUDBBackup获取
         - **DBId** (str) - (Required) DB实例Id,该值可通过DescribeUDBInstance获取
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **BackupPath** (str) - DB实例备份文件公网的地址
         - **InnerBackupPath** (str) - DB实例备份文件内网的地址
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBInstanceBackupURLRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBInstanceBackupURL", d, **kwargs)
         return apis.DescribeUDBInstanceBackupURLResponseSchema().loads(resp)
 
     def describe_udb_instance_binlog(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstanceBinlog - 获取UDB指定时间段的binlog列表
+        """DescribeUDBInstanceBinlog - 获取UDB指定时间段的binlog列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BeginTime** (int) - (Required) 过滤条件:起始时间(时间戳)
         - **DBId** (str) - (Required) DB实例Id
         - **EndTime** (int) - (Required) 过滤条件:结束时间(时间戳)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UDBInstanceBinlogSet** 模型定义
-        
+
         **Response Model**
-        
-        **UDBInstanceBinlogSet** 
-        
+
+        **UDBInstanceBinlogSet**
+
         - **BeginTime** (int) - Binlog文件生成时间(时间戳)
         - **EndTime** (int) - Binlog文件结束时间(时间戳)
         - **Name** (str) - Binlog文件名
         - **Size** (int) - Binlog文件大小
 
         """
         # build request
@@ -835,67 +835,67 @@
 
         resp = self.invoke("DescribeUDBInstanceBinlog", d, **kwargs)
         return apis.DescribeUDBInstanceBinlogResponseSchema().loads(resp)
 
     def describe_udb_instance_binlog_backup_state(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstanceBinlogBackupState - 获取udb实例备份状态
+        """DescribeUDBInstanceBinlogBackupState - 获取udb实例备份状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (int) - (Required) 备份记录ID
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupZone** (str) - 跨可用区高可用备库所在可用区
-        
+
         **Response**
 
         - **BackupSize** (int) - 备份文件大小(字节)
         - **State** (str) - 备份状态 0 Backuping // 备份中 1 Success // 备份成功 2 Failed // 备份失败 3 Expired // 备份过期
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBInstanceBinlogBackupStateRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBInstanceBinlogBackupState", d, **kwargs)
         return apis.DescribeUDBInstanceBinlogBackupStateResponseSchema().loads(
             resp
         )
 
     def describe_udb_instance_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstancePrice - 获取UDB实例价格信息
+        """DescribeUDBInstancePrice - 获取UDB实例价格信息
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBTypeId** (str) - (Required) UDB实例的DB版本字符串
         - **DiskSpace** (int) - (Required) 磁盘空间(GB),暂时支持20(GB) - 3000(GB), 输入不带单位
         - **MemoryLimit** (int) - (Required) 内存限制(MB)，单位为MB.目前支持：1000-96000
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - Year，按年付费； Month，按月付费 Dynamic，按需付费（需开启权限) Trial，试用（需开启权限）默认为月付
         - **Count** (int) - 购买DB实例数量,最大数量为10台, 默认为1台
         - **InstanceMode** (str) - 实例的部署类型。可选值为：Normal: 普通单点实例，Slave: 从库实例,HA: 高可用部署实例，默认是Normal
         - **Quantity** (int) - DB购买多少个"计费时间单位"，默认值为1。比如：买2个月，Quantity就是2。如果计费单位是“按月”，并且Quantity为0，表示“购买到月底”
         - **SSDType** (str) - SSD类型，可选值为"SATA"、"PCI-E"，如果UseSSD为true ，则必填
         - **UseSSD** (str) - 是否使用SSD，只能填true或false，默认为false
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UDBInstancePriceSet** 模型定义
-        
+
         **Response Model**
-        
-        **UDBInstancePriceSet** 
-        
+
+        **UDBInstancePriceSet**
+
         - **ChargeType** (str) - Year， Month， Dynamic，Trial
         - **Price** (int) - 价格，单位为分
 
         """
         # build request
         d = {"Region": self.config.region}
         req and d.update(req)
@@ -903,118 +903,118 @@
 
         resp = self.invoke("DescribeUDBInstancePrice", d, **kwargs)
         return apis.DescribeUDBInstancePriceResponseSchema().loads(resp)
 
     def describe_udb_instance_state(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstanceState - 获取UDB实例状态
+        """DescribeUDBInstanceState - 获取UDB实例状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **State** (str) - DB状态标记 Init：初始化中；Fail：安装失败； Starting：启动中； Running ： 运行 ；Shutdown：关闭中； Shutoff ：已关闭； Delete：已删除； Upgrading：升级中； Promoting： 提升为独库进行中； Recovering： 恢复中； Recover fail：恢复失败。
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBInstanceStateRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBInstanceState", d, **kwargs)
         return apis.DescribeUDBInstanceStateResponseSchema().loads(resp)
 
     def describe_udb_instance_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBInstanceUpgradePrice - 获取UDB实例升降级价格信息
+        """DescribeUDBInstanceUpgradePrice - 获取UDB实例升降级价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id
         - **DiskSpace** (int) - (Required) 磁盘空间(GB), 暂时支持20G - 500G
         - **MemoryLimit** (int) - (Required) 内存限制(MB)
         - **SSDType** (str) - SSD类型，可选值为"SATA"、"PCI-E"，如果UseSSD为true ，则必选
         - **UseSSD** (bool) - 是否使用SSD，默认为false
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Price** (int) - 价格，单位为分
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBInstanceUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBInstanceUpgradePrice", d, **kwargs)
         return apis.DescribeUDBInstanceUpgradePriceResponseSchema().loads(resp)
 
     def describe_udb_log_backup_url(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBLogBackupURL - 获取UDB的slowlog备份地址
+        """DescribeUDBLogBackupURL - 获取UDB的slowlog备份地址
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (int) - (Required) DB实例备份ID
         - **DBId** (str) - (Required) DB实例Id
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **BackupPath** (str) - 备份外网URL
         - **UsernetPath** (str) - 备份用户网URL
-        
+
         """
         # build request
         d = {"Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBLogBackupURLRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBLogBackupURL", d, **kwargs)
         return apis.DescribeUDBLogBackupURLResponseSchema().loads(resp)
 
     def describe_udb_log_package(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBLogPackage - 列表UDB实例binlog或slowlog或errorlog备份信息
+        """DescribeUDBLogPackage - 列表UDB实例binlog或slowlog或errorlog备份信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - (Required) 分页显示的条目数，列表操作则指定
         - **Offset** (int) - (Required) 分页显示的起始偏移，列表操作则指定
         - **BeginTime** (int) - 过滤条件:起始时间(时间戳)
         - **DBId** (str) - DB实例Id，如果指定，则只获取该db的备份信息
         - **EndTime** (int) - 过滤条件:结束时间(时间戳)
         - **Type** (int) - 需要列出的备份文件类型，每种文件的值如下 2 : BINLOG\_BACKUP 3 : SLOW\_QUERY\_BACKUP 4 : ERRORLOG\_BACKUP
         - **Types** (list) - Types作为Type的补充，支持多值传入，可以获取多个类型的日志记录，如：Types.0=2&Types.1=3
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **LogPackageDataSet** 模型定义
         - **TotalCount** (int) - 备份总数，如果指定dbid，则是该db备份总数
-        
+
         **Response Model**
-        
-        **LogPackageDataSet** 
-        
+
+        **LogPackageDataSet**
+
         - **BackupId** (int) - 备份id
         - **BackupName** (str) - 备份名称
         - **BackupSize** (int) - 备份文件大小
         - **BackupTime** (int) - 备份时间
         - **BackupType** (int) - 备份类型，包括2-binlog备份，3-slowlog备份
         - **BackupZone** (str) - 跨可用区高可用备库所在可用区
         - **DBId** (str) - dbid
@@ -1030,490 +1030,490 @@
 
         resp = self.invoke("DescribeUDBLogPackage", d, **kwargs)
         return apis.DescribeUDBLogPackageResponseSchema().loads(resp)
 
     def describe_udb_param_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBParamGroup - 获取参数组详细参数信息
+        """DescribeUDBParamGroup - 获取参数组详细参数信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - (Required) 分页显示的条目数，列表操作则指定
         - **Offset** (int) - (Required) 分页显示的起始偏移，列表操作则指定
         - **ClassType** (str) - 如果未指定GroupId，则可选是否选取特定DB类型的配置(sql, nosql, postgresql, sqlserver)
         - **GroupId** (int) - 参数组id，如果指定则获取描述，否则是列表操作，需要 指定Offset/Limit
         - **IsInUDBC** (bool) - 是否选取专区中配置
         - **RegionFlag** (bool) - 当请求没有填写Zone时，如果指定为true，表示只拉取跨可用区的相关配置文件，否则，拉取所有机房的配置文件（包括每个单可用区和跨可用区）
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UDBParamGroupSet** 模型定义
         - **TotalCount** (int) - 参数组总数，列表操作时才会有该参数
-        
+
         **Response Model**
-        
-        **UDBParamMemberSet** 
-        
+
+        **UDBParamMemberSet**
+
         - **AllowedVal** (str) - 允许的值(根据参数类型，用分隔符表示)
         - **ApplyType** (int) - 参数值应用类型,取值范围为{0,10,20}，各值代表 意义为0-unknown、10-static、20-dynamic
         - **FormatType** (int) - 允许值的格式类型，取值范围为{0,10,20}，意义分 别为PVFT_UNKOWN=0,PVFT_RANGE=10, PVFT_ENUM=20
         - **Key** (str) - 参数名称
         - **Modifiable** (bool) - 是否可更改，默认为false
         - **Value** (str) - 参数值
         - **ValueType** (int) - 参数值应用类型，取值范围为{0,10,20,30},各值 代表意义为 0-unknown、10-int、20-string、 30-bool
 
-        **UDBParamGroupSet** 
-        
+        **UDBParamGroupSet**
+
         - **DBTypeId** (str) - DB类型id，mysql/mongodb按版本细分各有一个id 目前id的取值范围为[1,7],数值对应的版本如下 1：mysql-5.5，2：mysql-5.1，3：percona-5.5 4：mongodb-2.4，5：mongodb-2.6，6：mysql-5.6 7：percona-5.6
         - **Description** (str) - 参数组描述
         - **GroupId** (int) - 参数组id
         - **GroupName** (str) - 参数组名称
         - **Modifiable** (bool) - 参数组是否可修改
         - **ParamMember** (list) - 见 **UDBParamMemberSet** 模型定义
-        - **RegionFlag** (bool) - 
-        - **Zone** (str) - 
+        - **RegionFlag** (bool) -
+        - **Zone** (str) -
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBParamGroupRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBParamGroup", d, **kwargs)
         return apis.DescribeUDBParamGroupResponseSchema().loads(resp)
 
     def describe_udb_type(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDBType - 获取UDB支持的类型信息
+        """DescribeUDBType - 获取UDB支持的类型信息
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **BackupZone** (str) - 跨可用区高可用DB的备库所在区域，仅当该可用区支持跨可用区高可用时填入。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **BackupZone** (str) - 跨可用区高可用DB的备库所在区域，仅当该可用区支持跨可用区高可用时填入。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBClusterType** (str) - DB实例类型，如mysql，sqlserver，mongo，postgresql
         - **DiskType** (str) - 返回支持某种磁盘类型的DB类型。如果没传，则表示任何磁盘类型均可。
         - **InstanceMode** (str) - 返回支持某种实例类型的DB类型。如果没传，则表示任何实例类型均可。normal:单点,ha:高可用,sharded_cluster:分片集群
-        
+
         **Response**
 
         - **Action** (str) - 操作名称
         - **DataSet** (list) - 见 **UDBTypeSet** 模型定义
         - **RetCode** (int) - 返回码
-        
+
         **Response Model**
-        
-        **UDBTypeSet** 
-        
+
+        **UDBTypeSet**
+
         - **DBTypeId** (str) - DB类型id，mysql/mongodb按版本细分各有一个id, 目前id的取值范围为[1,7],数值对应的版本如下： 1：mysql-5.5，2：mysql-5.1，3：percona-5.5 4：mongodb-2.4，5：mongodb-2.6，6：mysql-5.6， 7：percona-5.6
 
         """
         # build request
         d = {"Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDBTypeRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDBType", d, **kwargs)
         return apis.DescribeUDBTypeResponseSchema().loads(resp)
 
     def edit_udb_backup_blacklist(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ EditUDBBackupBlacklist - 编辑UDB实例的备份黑名单
+        """EditUDBBackupBlacklist - 编辑UDB实例的备份黑名单
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Blacklist** (str) - (Required) 黑名单，规范示例,指定库mysql.%;test.%; 指定表city.address;
         - **DBId** (str) - (Required) DB实例Id,该值可以通过DescribeUDBInstance获取
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.EditUDBBackupBlacklistRequestSchema().dumps(d)
 
         resp = self.invoke("EditUDBBackupBlacklist", d, **kwargs)
         return apis.EditUDBBackupBlacklistResponseSchema().loads(resp)
 
     def fetch_udb_instance_earliest_recover_time(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ FetchUDBInstanceEarliestRecoverTime - 获取UDB最早可回档的时间点
+        """FetchUDBInstanceEarliestRecoverTime - 获取UDB最早可回档的时间点
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) DB实例Id
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **EarliestTime** (int) - 获取最早可回档时间点
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.FetchUDBInstanceEarliestRecoverTimeRequestSchema().dumps(d)
 
         resp = self.invoke("FetchUDBInstanceEarliestRecoverTime", d, **kwargs)
         return apis.FetchUDBInstanceEarliestRecoverTimeResponseSchema().loads(
             resp
         )
 
     def modify_udb_instance_name(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyUDBInstanceName - 重命名UDB实例
+        """ModifyUDBInstanceName - 重命名UDB实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
         - **Name** (str) - (Required) 实例的新名字, 长度要求为6~63位
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyUDBInstanceNameRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyUDBInstanceName", d, **kwargs)
         return apis.ModifyUDBInstanceNameResponseSchema().loads(resp)
 
     def modify_udb_instance_password(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyUDBInstancePassword - 修改DB实例的管理员密码
+        """ModifyUDBInstancePassword - 修改DB实例的管理员密码
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的ID,该值可以通过DescribeUDBInstance获取
         - **Password** (str) - (Required) 实例的新密码
         - **AccountName** (str) - sqlserver帐号，仅在sqlserver的情况下填该参数
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyUDBInstancePasswordRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyUDBInstancePassword", d, **kwargs)
         return apis.ModifyUDBInstancePasswordResponseSchema().loads(resp)
 
     def promote_udb_instance_to_ha(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ PromoteUDBInstanceToHA - 普通db升级为高可用(只针对mysql5.5及以上版本)
+        """PromoteUDBInstanceToHA - 普通db升级为高可用(只针对mysql5.5及以上版本)
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.PromoteUDBInstanceToHARequestSchema().dumps(d)
 
         resp = self.invoke("PromoteUDBInstanceToHA", d, **kwargs)
         return apis.PromoteUDBInstanceToHAResponseSchema().loads(resp)
 
     def promote_udb_slave(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ PromoteUDBSlave - 从库提升为独立库
+        """PromoteUDBSlave - 从库提升为独立库
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
         - **IsForce** (bool) - 是否强制(如果从库落后可能会禁止提升)，默认false 如果落后情况下，强制提升丢失数据
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.PromoteUDBSlaveRequestSchema().dumps(d)
 
         resp = self.invoke("PromoteUDBSlave", d, **kwargs)
         return apis.PromoteUDBSlaveResponseSchema().loads(resp)
 
     def resize_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeUDBInstance - 修改（升级和降级）UDB实例的配置，包括内存和磁盘的配置，对于内存升级无需关闭实例，其他场景需要事先关闭实例。两套参数可以配置升降机：1.配置UseSSD和SSDType  2.配置InstanceType，不需要配置InstanceMode。这两套第二套参数的优先级更高
+        """ResizeUDBInstance - 修改（升级和降级）UDB实例的配置，包括内存和磁盘的配置，对于内存升级无需关闭实例，其他场景需要事先关闭实例。两套参数可以配置升降机：1.配置UseSSD和SSDType  2.配置InstanceType，不需要配置InstanceMode。这两套第二套参数的优先级更高
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id
         - **DiskSpace** (int) - (Required) 磁盘空间(GB), 暂时支持20G-3000G
         - **MemoryLimit** (int) - (Required) 内存限制(MB)，目前支持以下几档 1000M/2000M/4000M/ 6000M/8000M/ 12000M/16000M/ 24000M/32000M/ 48000M/64000M/96000M。
         - **CouponId** (str) - 使用的代金券id
         - **InstanceMode** (str) - UDB实例模式类型, 可选值如下: "Normal": 普通版UDB实例 "HA": 高可用版UDB实例 默认是"Normal"
         - **InstanceType** (str) - UDB数据库机型: "Normal": "标准机型" ,  "SATA_SSD": "SSD机型" , "PCIE_SSD": "SSD高性能机型" ,  "Normal_Volume": "标准大容量机型",  "SATA_SSD_Volume": "SSD大容量机型" ,  "PCIE_SSD_Volume": "SSD高性能大容量机型"
         - **SSDType** (str) - SSD类型，可选值为"SATA"、"PCI-E"，如果UseSSD为true ，则必选
         - **StartAfterUpgrade** (bool) - DB关闭状态下升降级，升降级后是否启动DB，默认为false
         - **UDBCId** (str) - 专区的ID，如果有值表示专区中的DB配置升降级
         - **UseSSD** (bool) - 是否使用SSD，默认为false
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ResizeUDBInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeUDBInstance", d, **kwargs)
         return apis.ResizeUDBInstanceResponseSchema().loads(resp)
 
     def restart_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RestartUDBInstance - 重启UDB实例
+        """RestartUDBInstance - 重启UDB实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.RestartUDBInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("RestartUDBInstance", d, **kwargs)
         return apis.RestartUDBInstanceResponseSchema().loads(resp)
 
     def start_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ StartUDBInstance - 启动UDB实例
+        """StartUDBInstance - 启动UDB实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.StartUDBInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("StartUDBInstance", d, **kwargs)
         return apis.StartUDBInstanceResponseSchema().loads(resp)
 
     def stop_udb_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ StopUDBInstance - 关闭UDB实例
+        """StopUDBInstance - 关闭UDB实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
         - **ForceToKill** (bool) - 是否使用强制手段关闭DB，默认是false
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.StopUDBInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("StopUDBInstance", d, **kwargs)
         return apis.StopUDBInstanceResponseSchema().loads(resp)
 
     def switch_udb_instance_to_ha(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ SwitchUDBInstanceToHA - 普通UDB切换为高可用，原db状态为WaitForSwitch时，调用该api
+        """SwitchUDBInstanceToHA - 普通UDB切换为高可用，原db状态为WaitForSwitch时，调用该api
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 实例的Id,该值可以通过DescribeUDBInstance获取
         - **ChargeType** (str) - Year， Month， Dynamic，Trial，不填则按现在单点计费执行
         - **Quantity** (str) - 购买时长，需要和 ChargeType 搭配使用，否则使用单点计费策略的值
         - **Tag** (str) - 业务组
-        
+
         **Response**
 
         - **DBId** (str) - 切换后高可用db实例的Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.SwitchUDBInstanceToHARequestSchema().dumps(d)
 
         resp = self.invoke("SwitchUDBInstanceToHA", d, **kwargs)
         return apis.SwitchUDBInstanceToHAResponseSchema().loads(resp)
 
     def update_udb_instance_backup_strategy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateUDBInstanceBackupStrategy - 修改UDB自动备份策略
+        """UpdateUDBInstanceBackupStrategy - 修改UDB自动备份策略
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DBId** (str) - (Required) 主节点的Id
         - **BackupDate** (str) - 备份时期标记位。共7位，每一位为一周中一天的备份情况，0表示关闭当天备份，1表示打开当天备份。最右边的一位为星期天的备份开关，其余从右到左依次为星期一到星期六的备份配置开关，每周必须至少设置两天备份。例如：1100000表示打开星期六和星期五的备份功能
         - **BackupMethod** (str) - 选择默认的备份方式，可选 snapshot 表示使用快照/物理备份，填 logic 表示使用逻辑备份。需要同时设置BackupDate字段。（注意现在只有SSD 版本的 MySQL实例支持物理备份）
         - **BackupTime** (int) - 备份的整点时间，范围[0,23]
         - **ForceDump** (bool) - 当导出某些数据遇到问题后，是否强制导出其他剩余数据默认是false需要同时设置BackupDate字段
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateUDBInstanceBackupStrategyRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateUDBInstanceBackupStrategy", d, **kwargs)
         return apis.UpdateUDBInstanceBackupStrategyResponseSchema().loads(resp)
 
     def update_udb_instance_slave_backup_switch(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateUDBInstanceSlaveBackupSwitch - 开启或者关闭UDB从库备份
+        """UpdateUDBInstanceSlaveBackupSwitch - 开启或者关闭UDB从库备份
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupSwitch** (int) - (Required) 从库的备份开关，范围[0,1],0表示从库备份功能关闭,1 表示从库备份开关打开。
         - **MasterDBId** (str) - (Required) 主库的Id
         - **SlaveDBId** (str) - 从库的Id,如果从库备份开关设定为打开，则必须赋值。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateUDBInstanceSlaveBackupSwitchRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateUDBInstanceSlaveBackupSwitch", d, **kwargs)
         return apis.UpdateUDBInstanceSlaveBackupSwitchResponseSchema().loads(
             resp
         )
 
     def update_udb_param_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateUDBParamGroup - 更新UDB配置参数项
+        """UpdateUDBParamGroup - 更新UDB配置参数项
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (int) - (Required) 配置参数组id，使用DescribeUDBParamGroup获得
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Description** (str) - 配置文件的描述，不传时认为不修改
         - **Key** (str) - 参数名称（与Value配合使用）
         - **Name** (str) - 配置文件的名字，不传时认为不修改名字，传了则不能为空
         - **RegionFlag** (bool) - 该配置文件是否是地域级别配置文件，默认是false
         - **Value** (str) - 参数值（与Key配合使用）
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateUDBParamGroupRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateUDBParamGroup", d, **kwargs)
         return apis.UpdateUDBParamGroupResponseSchema().loads(resp)
 
     def upload_udb_param_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UploadUDBParamGroup - 导入UDB配置
+        """UploadUDBParamGroup - 导入UDB配置
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Content** (str) - (Required) 配置内容，导入的配置内容采用base64编码
         - **DBTypeId** (str) - (Required) DB类型id，DB类型id，mysql/mongodb/postgesql按版本细分 1：mysql-5.1，2：mysql-5.5，3：percona-5.5，4：mysql-5.6，5：percona-5.6，6：mysql-5.7，7：percona-5.7，8：mariadb-10.0，9：mongodb-2.4，10：mongodb-2.6，11：mongodb-3.0，12：mongodb-3.2,13：postgresql-9.4，14：postgresql-9.6
         - **Description** (str) - (Required) 参数组描述
         - **GroupName** (str) - (Required) 配置参数组名称
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ParamGroupTypeId** (int) - 配置文件子类型 0-未知, 1-Shardsvr-MMAPv1, 2-Shardsvr-WiredTiger, 3-Configsvr-MMAPv1, 4-Configsvr-WiredTiger, 5-Mongos
         - **RegionFlag** (bool) - 该配置文件是否是地域级别配置文件，默认是false
-        
+
         **Response**
 
         - **GroupId** (int) - 配置参数组id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UploadUDBParamGroupRequestSchema().dumps(d)
 
         # build options
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udb/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udb/schemas/apis.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: BackupUDBInstance
 
 备份UDB实例
 """
 
 
 class BackupUDBInstanceRequestSchema(schema.RequestSchema):
-    """ BackupUDBInstance - 备份UDB实例
-    """
+    """BackupUDBInstance - 备份UDB实例"""
 
     fields = {
         "BackupMethod": fields.Str(required=False, dump_to="BackupMethod"),
         "BackupName": fields.Str(required=True, dump_to="BackupName"),
         "Blacklist": fields.Str(required=False, dump_to="Blacklist"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ForceBackup": fields.Bool(required=False, dump_to="ForceBackup"),
@@ -29,194 +28,180 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "UseBlacklist": fields.Bool(required=False, dump_to="UseBlacklist"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class BackupUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ BackupUDBInstance - 备份UDB实例
-    """
+    """BackupUDBInstance - 备份UDB实例"""
 
     fields = {}
 
 
 """
 API: BackupUDBInstanceBinlog
 
 备份UDB指定时间段的binlog列表
 """
 
 
 class BackupUDBInstanceBinlogRequestSchema(schema.RequestSchema):
-    """ BackupUDBInstanceBinlog - 备份UDB指定时间段的binlog列表
-    """
+    """BackupUDBInstanceBinlog - 备份UDB指定时间段的binlog列表"""
 
     fields = {
         "BackupFile": fields.Str(required=True, dump_to="BackupFile"),
         "BackupName": fields.Str(required=False, dump_to="BackupName"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class BackupUDBInstanceBinlogResponseSchema(schema.ResponseSchema):
-    """ BackupUDBInstanceBinlog - 备份UDB指定时间段的binlog列表
-    """
+    """BackupUDBInstanceBinlog - 备份UDB指定时间段的binlog列表"""
 
     fields = {}
 
 
 """
 API: BackupUDBInstanceErrorLog
 
 备份UDB指定时间段的errorlog
 """
 
 
 class BackupUDBInstanceErrorLogRequestSchema(schema.RequestSchema):
-    """ BackupUDBInstanceErrorLog - 备份UDB指定时间段的errorlog
-    """
+    """BackupUDBInstanceErrorLog - 备份UDB指定时间段的errorlog"""
 
     fields = {
         "BackupName": fields.Str(required=True, dump_to="BackupName"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class BackupUDBInstanceErrorLogResponseSchema(schema.ResponseSchema):
-    """ BackupUDBInstanceErrorLog - 备份UDB指定时间段的errorlog
-    """
+    """BackupUDBInstanceErrorLog - 备份UDB指定时间段的errorlog"""
 
     fields = {}
 
 
 """
 API: BackupUDBInstanceSlowLog
 
 备份UDB指定时间段的slowlog分析结果
 """
 
 
 class BackupUDBInstanceSlowLogRequestSchema(schema.RequestSchema):
-    """ BackupUDBInstanceSlowLog - 备份UDB指定时间段的slowlog分析结果
-    """
+    """BackupUDBInstanceSlowLog - 备份UDB指定时间段的slowlog分析结果"""
 
     fields = {
         "BackupName": fields.Str(required=True, dump_to="BackupName"),
         "BeginTime": fields.Int(required=True, dump_to="BeginTime"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "EndTime": fields.Int(required=True, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class BackupUDBInstanceSlowLogResponseSchema(schema.ResponseSchema):
-    """ BackupUDBInstanceSlowLog - 备份UDB指定时间段的slowlog分析结果
-    """
+    """BackupUDBInstanceSlowLog - 备份UDB指定时间段的slowlog分析结果"""
 
     fields = {}
 
 
 """
 API: CheckRecoverUDBInstance
 
 核查db是否可以使用回档功能
 """
 
 
 class CheckRecoverUDBInstanceRequestSchema(schema.RequestSchema):
-    """ CheckRecoverUDBInstance - 核查db是否可以使用回档功能
-    """
+    """CheckRecoverUDBInstance - 核查db是否可以使用回档功能"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SrcDBId": fields.Str(required=True, dump_to="SrcDBId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CheckRecoverUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ CheckRecoverUDBInstance - 核查db是否可以使用回档功能
-    """
+    """CheckRecoverUDBInstance - 核查db是否可以使用回档功能"""
 
     fields = {
         "LastestTime": fields.Int(required=False, load_from="LastestTime")
     }
 
 
 """
 API: CheckUDBInstanceToHAAllowance
 
 核查db是否可以升级为高可用
 """
 
 
 class CheckUDBInstanceToHAAllowanceRequestSchema(schema.RequestSchema):
-    """ CheckUDBInstanceToHAAllowance - 核查db是否可以升级为高可用
-    """
+    """CheckUDBInstanceToHAAllowance - 核查db是否可以升级为高可用"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class CheckUDBInstanceToHAAllowanceResponseSchema(schema.ResponseSchema):
-    """ CheckUDBInstanceToHAAllowance - 核查db是否可以升级为高可用
-    """
+    """CheckUDBInstanceToHAAllowance - 核查db是否可以升级为高可用"""
 
     fields = {"Allowance": fields.Str(required=False, load_from="Allowance")}
 
 
 """
 API: ClearUDBLog
 
 清除UDB实例的log
 """
 
 
 class ClearUDBLogRequestSchema(schema.RequestSchema):
-    """ ClearUDBLog - 清除UDB实例的log
-    """
+    """ClearUDBLog - 清除UDB实例的log"""
 
     fields = {
         "BeforeTime": fields.Int(required=False, dump_to="BeforeTime"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "LogType": fields.Int(required=True, dump_to="LogType"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ClearUDBLogResponseSchema(schema.ResponseSchema):
-    """ ClearUDBLog - 清除UDB实例的log
-    """
+    """ClearUDBLog - 清除UDB实例的log"""
 
     fields = {}
 
 
 """
 API: CreateUDBInstance
 
 创建UDB实例（包括创建mysql master节点、mongodb primary/configsvr节点和从备份恢复实例）
 """
 
 
 class CreateUDBInstanceRequestSchema(schema.RequestSchema):
-    """ CreateUDBInstance - 创建UDB实例（包括创建mysql master节点、mongodb primary/configsvr节点和从备份恢复实例）
-    """
+    """CreateUDBInstance - 创建UDB实例（包括创建mysql master节点、mongodb primary/configsvr节点和从备份恢复实例）"""
 
     fields = {
         "AdminPassword": fields.Str(required=True, dump_to="AdminPassword"),
         "AdminUser": fields.Str(required=False, dump_to="AdminUser"),
         "BackupCount": fields.Int(required=False, dump_to="BackupCount"),
         "BackupDuration": fields.Int(required=False, dump_to="BackupDuration"),
         "BackupId": fields.Int(required=False, dump_to="BackupId"),
@@ -248,30 +233,28 @@
         "UseSSD": fields.Bool(required=False, dump_to="UseSSD"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ CreateUDBInstance - 创建UDB实例（包括创建mysql master节点、mongodb primary/configsvr节点和从备份恢复实例）
-    """
+    """CreateUDBInstance - 创建UDB实例（包括创建mysql master节点、mongodb primary/configsvr节点和从备份恢复实例）"""
 
     fields = {"DBId": fields.Str(required=False, load_from="DBId")}
 
 
 """
 API: CreateUDBInstanceByRecovery
 
 创建db，将新创建的db恢复到指定db某个指定时间点
 """
 
 
 class CreateUDBInstanceByRecoveryRequestSchema(schema.RequestSchema):
-    """ CreateUDBInstanceByRecovery - 创建db，将新创建的db恢复到指定db某个指定时间点
-    """
+    """CreateUDBInstanceByRecovery - 创建db，将新创建的db恢复到指定db某个指定时间点"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
@@ -283,60 +266,56 @@
         "UseSSD": fields.Bool(required=False, dump_to="UseSSD"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CreateUDBInstanceByRecoveryResponseSchema(schema.ResponseSchema):
-    """ CreateUDBInstanceByRecovery - 创建db，将新创建的db恢复到指定db某个指定时间点
-    """
+    """CreateUDBInstanceByRecovery - 创建db，将新创建的db恢复到指定db某个指定时间点"""
 
     fields = {"DBId": fields.Str(required=False, load_from="DBId")}
 
 
 """
 API: CreateUDBParamGroup
 
 从已有配置文件创建新配置文件
 """
 
 
 class CreateUDBParamGroupRequestSchema(schema.RequestSchema):
-    """ CreateUDBParamGroup - 从已有配置文件创建新配置文件
-    """
+    """CreateUDBParamGroup - 从已有配置文件创建新配置文件"""
 
     fields = {
         "DBTypeId": fields.Str(required=True, dump_to="DBTypeId"),
         "Description": fields.Str(required=True, dump_to="Description"),
         "GroupName": fields.Str(required=True, dump_to="GroupName"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
         "SrcGroupId": fields.Int(required=True, dump_to="SrcGroupId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateUDBParamGroupResponseSchema(schema.ResponseSchema):
-    """ CreateUDBParamGroup - 从已有配置文件创建新配置文件
-    """
+    """CreateUDBParamGroup - 从已有配置文件创建新配置文件"""
 
     fields = {"GroupId": fields.Int(required=False, load_from="GroupId")}
 
 
 """
 API: CreateUDBReplicationInstance
 
 创建MongoDB的副本节点（包括仲裁）
 """
 
 
 class CreateUDBReplicationInstanceRequestSchema(schema.RequestSchema):
-    """ CreateUDBReplicationInstance - 创建MongoDB的副本节点（包括仲裁）
-    """
+    """CreateUDBReplicationInstance - 创建MongoDB的副本节点（包括仲裁）"""
 
     fields = {
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "IsArbiter": fields.Bool(required=False, dump_to="IsArbiter"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Port": fields.Int(required=False, dump_to="Port"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -344,30 +323,28 @@
         "SrcId": fields.Str(required=True, dump_to="SrcId"),
         "UseSSD": fields.Bool(required=False, dump_to="UseSSD"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CreateUDBReplicationInstanceResponseSchema(schema.ResponseSchema):
-    """ CreateUDBReplicationInstance - 创建MongoDB的副本节点（包括仲裁）
-    """
+    """CreateUDBReplicationInstance - 创建MongoDB的副本节点（包括仲裁）"""
 
     fields = {"DBId": fields.Str(required=False, load_from="DBId")}
 
 
 """
 API: CreateUDBRouteInstance
 
 创建mongos实例
 """
 
 
 class CreateUDBRouteInstanceRequestSchema(schema.RequestSchema):
-    """ CreateUDBRouteInstance - 创建mongos实例
-    """
+    """CreateUDBRouteInstance - 创建mongos实例"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "ConfigsvrId": fields.List(fields.Str()),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "DBTypeId": fields.Str(required=True, dump_to="DBTypeId"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
@@ -380,30 +357,28 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "UseSSD": fields.Bool(required=False, dump_to="UseSSD"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CreateUDBRouteInstanceResponseSchema(schema.ResponseSchema):
-    """ CreateUDBRouteInstance - 创建mongos实例
-    """
+    """CreateUDBRouteInstance - 创建mongos实例"""
 
     fields = {"DBId": fields.Str(required=False, load_from="DBId")}
 
 
 """
 API: CreateUDBSlave
 
 创建UDB实例的slave
 """
 
 
 class CreateUDBSlaveRequestSchema(schema.RequestSchema):
-    """ CreateUDBSlave - 创建UDB实例的slave
-    """
+    """CreateUDBSlave - 创建UDB实例的slave"""
 
     fields = {
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "DiskSpace": fields.Int(required=False, dump_to="DiskSpace"),
         "InstanceMode": fields.Str(required=False, dump_to="InstanceMode"),
         "InstanceType": fields.Str(required=False, dump_to="InstanceType"),
         "IsLock": fields.Bool(required=False, dump_to="IsLock"),
@@ -416,138 +391,128 @@
         "SrcId": fields.Str(required=True, dump_to="SrcId"),
         "UseSSD": fields.Bool(required=False, dump_to="UseSSD"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CreateUDBSlaveResponseSchema(schema.ResponseSchema):
-    """ CreateUDBSlave - 创建UDB实例的slave
-    """
+    """CreateUDBSlave - 创建UDB实例的slave"""
 
     fields = {"DBId": fields.Str(required=False, load_from="DBId")}
 
 
 """
 API: DeleteUDBBackup
 
 删除UDB实例备份
 """
 
 
 class DeleteUDBBackupRequestSchema(schema.RequestSchema):
-    """ DeleteUDBBackup - 删除UDB实例备份
-    """
+    """DeleteUDBBackup - 删除UDB实例备份"""
 
     fields = {
         "BackupId": fields.Int(required=True, dump_to="BackupId"),
         "BackupZone": fields.Str(required=False, dump_to="BackupZone"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteUDBBackupResponseSchema(schema.ResponseSchema):
-    """ DeleteUDBBackup - 删除UDB实例备份
-    """
+    """DeleteUDBBackup - 删除UDB实例备份"""
 
     fields = {}
 
 
 """
 API: DeleteUDBInstance
 
 删除UDB实例
 """
 
 
 class DeleteUDBInstanceRequestSchema(schema.RequestSchema):
-    """ DeleteUDBInstance - 删除UDB实例
-    """
+    """DeleteUDBInstance - 删除UDB实例"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDBCId": fields.Str(required=False, dump_to="UDBCId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DeleteUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ DeleteUDBInstance - 删除UDB实例
-    """
+    """DeleteUDBInstance - 删除UDB实例"""
 
     fields = {}
 
 
 """
 API: DeleteUDBLogPackage
 
 删除UDB日志包
 """
 
 
 class DeleteUDBLogPackageRequestSchema(schema.RequestSchema):
-    """ DeleteUDBLogPackage - 删除UDB日志包
-    """
+    """DeleteUDBLogPackage - 删除UDB日志包"""
 
     fields = {
         "BackupId": fields.Int(required=True, dump_to="BackupId"),
         "BackupZone": fields.Str(required=False, dump_to="BackupZone"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteUDBLogPackageResponseSchema(schema.ResponseSchema):
-    """ DeleteUDBLogPackage - 删除UDB日志包
-    """
+    """DeleteUDBLogPackage - 删除UDB日志包"""
 
     fields = {}
 
 
 """
 API: DeleteUDBParamGroup
 
 删除配置参数组
 """
 
 
 class DeleteUDBParamGroupRequestSchema(schema.RequestSchema):
-    """ DeleteUDBParamGroup - 删除配置参数组
-    """
+    """DeleteUDBParamGroup - 删除配置参数组"""
 
     fields = {
         "GroupId": fields.Int(required=True, dump_to="GroupId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteUDBParamGroupResponseSchema(schema.ResponseSchema):
-    """ DeleteUDBParamGroup - 删除配置参数组
-    """
+    """DeleteUDBParamGroup - 删除配置参数组"""
 
     fields = {}
 
 
 """
 API: DescribeUDBBackup
 
 列表UDB实例备份信息.Zone不填表示多可用区，填代表单可用区
 """
 
 
 class DescribeUDBBackupRequestSchema(schema.RequestSchema):
-    """ DescribeUDBBackup - 列表UDB实例备份信息.Zone不填表示多可用区，填代表单可用区
-    """
+    """DescribeUDBBackup - 列表UDB实例备份信息.Zone不填表示多可用区，填代表单可用区"""
 
     fields = {
         "BackupId": fields.Int(required=False, dump_to="BackupId"),
         "BackupType": fields.Int(required=False, dump_to="BackupType"),
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "ClassType": fields.Str(required=False, dump_to="ClassType"),
         "DBId": fields.Str(required=False, dump_to="DBId"),
@@ -557,16 +522,15 @@
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBBackupResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBBackup - 列表UDB实例备份信息.Zone不填表示多可用区，填代表单可用区
-    """
+    """DescribeUDBBackup - 列表UDB实例备份信息.Zone不填表示多可用区，填代表单可用区"""
 
     fields = {
         "DataSet": fields.List(
             models.UDBBackupSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -576,54 +540,50 @@
 API: DescribeUDBBackupBlacklist
 
 获取UDB实例的备份黑名单
 """
 
 
 class DescribeUDBBackupBlacklistRequestSchema(schema.RequestSchema):
-    """ DescribeUDBBackupBlacklist - 获取UDB实例的备份黑名单
-    """
+    """DescribeUDBBackupBlacklist - 获取UDB实例的备份黑名单"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBBackupBlacklistResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBBackupBlacklist - 获取UDB实例的备份黑名单
-    """
+    """DescribeUDBBackupBlacklist - 获取UDB实例的备份黑名单"""
 
     fields = {"Blacklist": fields.Str(required=False, load_from="Blacklist")}
 
 
 """
 API: DescribeUDBBinlogBackupURL
 
 获取UDB的Binlog备份地址
 """
 
 
 class DescribeUDBBinlogBackupURLRequestSchema(schema.RequestSchema):
-    """ DescribeUDBBinlogBackupURL - 获取UDB的Binlog备份地址
-    """
+    """DescribeUDBBinlogBackupURL - 获取UDB的Binlog备份地址"""
 
     fields = {
         "BackupId": fields.Int(required=True, dump_to="BackupId"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBBinlogBackupURLResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBBinlogBackupURL - 获取UDB的Binlog备份地址
-    """
+    """DescribeUDBBinlogBackupURL - 获取UDB的Binlog备份地址"""
 
     fields = {
         "BackupPath": fields.Str(required=False, load_from="BackupPath"),
         "InnerBackupPath": fields.Str(
             required=False, load_from="InnerBackupPath"
         ),
     }
@@ -633,16 +593,15 @@
 API: DescribeUDBInstance
 
 获取UDB实例信息，支持两类操作：（1）指定DBId用于获取该db的信息；（2）指定ClassType、Offset、Limit用于列表操作，查询某一个类型db。
 """
 
 
 class DescribeUDBInstanceRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstance - 获取UDB实例信息，支持两类操作：（1）指定DBId用于获取该db的信息；（2）指定ClassType、Offset、Limit用于列表操作，查询某一个类型db。
-    """
+    """DescribeUDBInstance - 获取UDB实例信息，支持两类操作：（1）指定DBId用于获取该db的信息；（2）指定ClassType、Offset、Limit用于列表操作，查询某一个类型db。"""
 
     fields = {
         "ClassType": fields.Str(required=False, dump_to="ClassType"),
         "DBId": fields.Str(required=False, dump_to="DBId"),
         "IncludeSlaves": fields.Bool(required=False, dump_to="IncludeSlaves"),
         "IsInUDBC": fields.Bool(required=False, dump_to="IsInUDBC"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
@@ -651,16 +610,15 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDBCId": fields.Str(required=False, dump_to="UDBCId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstance - 获取UDB实例信息，支持两类操作：（1）指定DBId用于获取该db的信息；（2）指定ClassType、Offset、Limit用于列表操作，查询某一个类型db。
-    """
+    """DescribeUDBInstance - 获取UDB实例信息，支持两类操作：（1）指定DBId用于获取该db的信息；（2）指定ClassType、Offset、Limit用于列表操作，查询某一个类型db。"""
 
     fields = {
         "DataSet": fields.List(
             models.UDBInstanceSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -670,29 +628,27 @@
 API: DescribeUDBInstanceBackupState
 
 获取UDB实例备份状态
 """
 
 
 class DescribeUDBInstanceBackupStateRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstanceBackupState - 获取UDB实例备份状态
-    """
+    """DescribeUDBInstanceBackupState - 获取UDB实例备份状态"""
 
     fields = {
         "BackupId": fields.Int(required=True, dump_to="BackupId"),
         "BackupZone": fields.Str(required=False, dump_to="BackupZone"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstanceBackupStateResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstanceBackupState - 获取UDB实例备份状态
-    """
+    """DescribeUDBInstanceBackupState - 获取UDB实例备份状态"""
 
     fields = {
         "BackupEndTime": fields.Int(required=False, load_from="BackupEndTime"),
         "BackupSize": fields.Int(required=False, load_from="BackupSize"),
         "State": fields.Str(required=False, load_from="State"),
     }
 
@@ -701,29 +657,27 @@
 API: DescribeUDBInstanceBackupURL
 
 获取UDB备份下载地址
 """
 
 
 class DescribeUDBInstanceBackupURLRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstanceBackupURL - 获取UDB备份下载地址
-    """
+    """DescribeUDBInstanceBackupURL - 获取UDB备份下载地址"""
 
     fields = {
         "BackupId": fields.Int(required=True, dump_to="BackupId"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstanceBackupURLResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstanceBackupURL - 获取UDB备份下载地址
-    """
+    """DescribeUDBInstanceBackupURL - 获取UDB备份下载地址"""
 
     fields = {
         "BackupPath": fields.Str(required=False, load_from="BackupPath"),
         "InnerBackupPath": fields.Str(
             required=False, load_from="InnerBackupPath"
         ),
     }
@@ -733,30 +687,28 @@
 API: DescribeUDBInstanceBinlog
 
 获取UDB指定时间段的binlog列表
 """
 
 
 class DescribeUDBInstanceBinlogRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstanceBinlog - 获取UDB指定时间段的binlog列表
-    """
+    """DescribeUDBInstanceBinlog - 获取UDB指定时间段的binlog列表"""
 
     fields = {
         "BeginTime": fields.Int(required=True, dump_to="BeginTime"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "EndTime": fields.Int(required=True, dump_to="EndTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstanceBinlogResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstanceBinlog - 获取UDB指定时间段的binlog列表
-    """
+    """DescribeUDBInstanceBinlog - 获取UDB指定时间段的binlog列表"""
 
     fields = {
         "DataSet": fields.List(
             models.UDBInstanceBinlogSetSchema(),
             required=False,
             load_from="DataSet",
         )
@@ -767,29 +719,27 @@
 API: DescribeUDBInstanceBinlogBackupState
 
 获取udb实例备份状态
 """
 
 
 class DescribeUDBInstanceBinlogBackupStateRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstanceBinlogBackupState - 获取udb实例备份状态
-    """
+    """DescribeUDBInstanceBinlogBackupState - 获取udb实例备份状态"""
 
     fields = {
         "BackupId": fields.Int(required=True, dump_to="BackupId"),
         "BackupZone": fields.Str(required=False, dump_to="BackupZone"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstanceBinlogBackupStateResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstanceBinlogBackupState - 获取udb实例备份状态
-    """
+    """DescribeUDBInstanceBinlogBackupState - 获取udb实例备份状态"""
 
     fields = {
         "BackupSize": fields.Int(required=False, load_from="BackupSize"),
         "State": fields.Str(required=False, load_from="State"),
     }
 
 
@@ -797,16 +747,15 @@
 API: DescribeUDBInstancePrice
 
 获取UDB实例价格信息
 """
 
 
 class DescribeUDBInstancePriceRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstancePrice - 获取UDB实例价格信息
-    """
+    """DescribeUDBInstancePrice - 获取UDB实例价格信息"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "Count": fields.Int(required=False, dump_to="Count"),
         "DBTypeId": fields.Str(required=True, dump_to="DBTypeId"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
         "InstanceMode": fields.Str(required=False, dump_to="InstanceMode"),
@@ -816,16 +765,15 @@
         "SSDType": fields.Str(required=False, dump_to="SSDType"),
         "UseSSD": fields.Str(required=False, dump_to="UseSSD"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstancePriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstancePrice - 获取UDB实例价格信息
-    """
+    """DescribeUDBInstancePrice - 获取UDB实例价格信息"""
 
     fields = {
         "DataSet": fields.List(
             models.UDBInstancePriceSetSchema(),
             required=False,
             load_from="DataSet",
         )
@@ -836,84 +784,78 @@
 API: DescribeUDBInstanceState
 
 获取UDB实例状态
 """
 
 
 class DescribeUDBInstanceStateRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstanceState - 获取UDB实例状态
-    """
+    """DescribeUDBInstanceState - 获取UDB实例状态"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstanceStateResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstanceState - 获取UDB实例状态
-    """
+    """DescribeUDBInstanceState - 获取UDB实例状态"""
 
     fields = {"State": fields.Str(required=False, load_from="State")}
 
 
 """
 API: DescribeUDBInstanceUpgradePrice
 
 获取UDB实例升降级价格信息
 """
 
 
 class DescribeUDBInstanceUpgradePriceRequestSchema(schema.RequestSchema):
-    """ DescribeUDBInstanceUpgradePrice - 获取UDB实例升降级价格信息
-    """
+    """DescribeUDBInstanceUpgradePrice - 获取UDB实例升降级价格信息"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
         "MemoryLimit": fields.Int(required=True, dump_to="MemoryLimit"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SSDType": fields.Str(required=False, dump_to="SSDType"),
         "UseSSD": fields.Bool(required=False, dump_to="UseSSD"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBInstanceUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBInstanceUpgradePrice - 获取UDB实例升降级价格信息
-    """
+    """DescribeUDBInstanceUpgradePrice - 获取UDB实例升降级价格信息"""
 
     fields = {"Price": fields.Int(required=False, load_from="Price")}
 
 
 """
 API: DescribeUDBLogBackupURL
 
 获取UDB的slowlog备份地址
 """
 
 
 class DescribeUDBLogBackupURLRequestSchema(schema.RequestSchema):
-    """ DescribeUDBLogBackupURL - 获取UDB的slowlog备份地址
-    """
+    """DescribeUDBLogBackupURL - 获取UDB的slowlog备份地址"""
 
     fields = {
         "BackupId": fields.Int(required=True, dump_to="BackupId"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBLogBackupURLResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBLogBackupURL - 获取UDB的slowlog备份地址
-    """
+    """DescribeUDBLogBackupURL - 获取UDB的slowlog备份地址"""
 
     fields = {
         "BackupPath": fields.Str(required=False, load_from="BackupPath"),
         "UsernetPath": fields.Str(required=False, load_from="UsernetPath"),
     }
 
 
@@ -921,16 +863,15 @@
 API: DescribeUDBLogPackage
 
 列表UDB实例binlog或slowlog或errorlog备份信息
 """
 
 
 class DescribeUDBLogPackageRequestSchema(schema.RequestSchema):
-    """ DescribeUDBLogPackage - 列表UDB实例binlog或slowlog或errorlog备份信息
-    """
+    """DescribeUDBLogPackage - 列表UDB实例binlog或slowlog或errorlog备份信息"""
 
     fields = {
         "BeginTime": fields.Int(required=False, dump_to="BeginTime"),
         "DBId": fields.Str(required=False, dump_to="DBId"),
         "EndTime": fields.Int(required=False, dump_to="EndTime"),
         "Limit": fields.Int(required=True, dump_to="Limit"),
         "Offset": fields.Int(required=True, dump_to="Offset"),
@@ -939,16 +880,15 @@
         "Type": fields.Int(required=False, dump_to="Type"),
         "Types": fields.List(fields.Int()),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBLogPackageResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBLogPackage - 列表UDB实例binlog或slowlog或errorlog备份信息
-    """
+    """DescribeUDBLogPackage - 列表UDB实例binlog或slowlog或errorlog备份信息"""
 
     fields = {
         "DataSet": fields.List(
             models.LogPackageDataSetSchema(),
             required=False,
             load_from="DataSet",
         ),
@@ -960,16 +900,15 @@
 API: DescribeUDBParamGroup
 
 获取参数组详细参数信息
 """
 
 
 class DescribeUDBParamGroupRequestSchema(schema.RequestSchema):
-    """ DescribeUDBParamGroup - 获取参数组详细参数信息
-    """
+    """DescribeUDBParamGroup - 获取参数组详细参数信息"""
 
     fields = {
         "ClassType": fields.Str(required=False, dump_to="ClassType"),
         "GroupId": fields.Int(required=False, dump_to="GroupId"),
         "IsInUDBC": fields.Bool(required=False, dump_to="IsInUDBC"),
         "Limit": fields.Int(required=True, dump_to="Limit"),
         "Offset": fields.Int(required=True, dump_to="Offset"),
@@ -977,16 +916,15 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDBParamGroupResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBParamGroup - 获取参数组详细参数信息
-    """
+    """DescribeUDBParamGroup - 获取参数组详细参数信息"""
 
     fields = {
         "DataSet": fields.List(
             models.UDBParamGroupSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -996,30 +934,28 @@
 API: DescribeUDBType
 
 获取UDB支持的类型信息
 """
 
 
 class DescribeUDBTypeRequestSchema(schema.RequestSchema):
-    """ DescribeUDBType - 获取UDB支持的类型信息
-    """
+    """DescribeUDBType - 获取UDB支持的类型信息"""
 
     fields = {
         "BackupZone": fields.Str(required=False, dump_to="BackupZone"),
         "DBClusterType": fields.Str(required=False, dump_to="DBClusterType"),
         "DiskType": fields.Str(required=False, dump_to="DiskType"),
         "InstanceMode": fields.Str(required=False, dump_to="InstanceMode"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUDBTypeResponseSchema(schema.ResponseSchema):
-    """ DescribeUDBType - 获取UDB支持的类型信息
-    """
+    """DescribeUDBType - 获取UDB支持的类型信息"""
 
     fields = {
         "Action": fields.Str(required=True, load_from="Action"),
         "DataSet": fields.List(
             models.UDBTypeSetSchema(), required=False, load_from="DataSet"
         ),
         "RetCode": fields.Int(required=True, load_from="RetCode"),
@@ -1030,178 +966,165 @@
 API: EditUDBBackupBlacklist
 
 编辑UDB实例的备份黑名单
 """
 
 
 class EditUDBBackupBlacklistRequestSchema(schema.RequestSchema):
-    """ EditUDBBackupBlacklist - 编辑UDB实例的备份黑名单
-    """
+    """EditUDBBackupBlacklist - 编辑UDB实例的备份黑名单"""
 
     fields = {
         "Blacklist": fields.Str(required=True, dump_to="Blacklist"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class EditUDBBackupBlacklistResponseSchema(schema.ResponseSchema):
-    """ EditUDBBackupBlacklist - 编辑UDB实例的备份黑名单
-    """
+    """EditUDBBackupBlacklist - 编辑UDB实例的备份黑名单"""
 
     fields = {}
 
 
 """
 API: FetchUDBInstanceEarliestRecoverTime
 
 获取UDB最早可回档的时间点
 """
 
 
 class FetchUDBInstanceEarliestRecoverTimeRequestSchema(schema.RequestSchema):
-    """ FetchUDBInstanceEarliestRecoverTime - 获取UDB最早可回档的时间点
-    """
+    """FetchUDBInstanceEarliestRecoverTime - 获取UDB最早可回档的时间点"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class FetchUDBInstanceEarliestRecoverTimeResponseSchema(schema.ResponseSchema):
-    """ FetchUDBInstanceEarliestRecoverTime - 获取UDB最早可回档的时间点
-    """
+    """FetchUDBInstanceEarliestRecoverTime - 获取UDB最早可回档的时间点"""
 
     fields = {
         "EarliestTime": fields.Int(required=False, load_from="EarliestTime")
     }
 
 
 """
 API: ModifyUDBInstanceName
 
 重命名UDB实例
 """
 
 
 class ModifyUDBInstanceNameRequestSchema(schema.RequestSchema):
-    """ ModifyUDBInstanceName - 重命名UDB实例
-    """
+    """ModifyUDBInstanceName - 重命名UDB实例"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyUDBInstanceNameResponseSchema(schema.ResponseSchema):
-    """ ModifyUDBInstanceName - 重命名UDB实例
-    """
+    """ModifyUDBInstanceName - 重命名UDB实例"""
 
     fields = {}
 
 
 """
 API: ModifyUDBInstancePassword
 
 修改DB实例的管理员密码
 """
 
 
 class ModifyUDBInstancePasswordRequestSchema(schema.RequestSchema):
-    """ ModifyUDBInstancePassword - 修改DB实例的管理员密码
-    """
+    """ModifyUDBInstancePassword - 修改DB实例的管理员密码"""
 
     fields = {
         "AccountName": fields.Str(required=False, dump_to="AccountName"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "Password": fields.Str(required=True, dump_to="Password"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyUDBInstancePasswordResponseSchema(schema.ResponseSchema):
-    """ ModifyUDBInstancePassword - 修改DB实例的管理员密码
-    """
+    """ModifyUDBInstancePassword - 修改DB实例的管理员密码"""
 
     fields = {}
 
 
 """
 API: PromoteUDBInstanceToHA
 
 普通db升级为高可用(只针对mysql5.5及以上版本)
 """
 
 
 class PromoteUDBInstanceToHARequestSchema(schema.RequestSchema):
-    """ PromoteUDBInstanceToHA - 普通db升级为高可用(只针对mysql5.5及以上版本)
-    """
+    """PromoteUDBInstanceToHA - 普通db升级为高可用(只针对mysql5.5及以上版本)"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class PromoteUDBInstanceToHAResponseSchema(schema.ResponseSchema):
-    """ PromoteUDBInstanceToHA - 普通db升级为高可用(只针对mysql5.5及以上版本)
-    """
+    """PromoteUDBInstanceToHA - 普通db升级为高可用(只针对mysql5.5及以上版本)"""
 
     fields = {}
 
 
 """
 API: PromoteUDBSlave
 
 从库提升为独立库
 """
 
 
 class PromoteUDBSlaveRequestSchema(schema.RequestSchema):
-    """ PromoteUDBSlave - 从库提升为独立库
-    """
+    """PromoteUDBSlave - 从库提升为独立库"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "IsForce": fields.Bool(required=False, dump_to="IsForce"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class PromoteUDBSlaveResponseSchema(schema.ResponseSchema):
-    """ PromoteUDBSlave - 从库提升为独立库
-    """
+    """PromoteUDBSlave - 从库提升为独立库"""
 
     fields = {}
 
 
 """
 API: ResizeUDBInstance
 
 修改（升级和降级）UDB实例的配置，包括内存和磁盘的配置，对于内存升级无需关闭实例，其他场景需要事先关闭实例。两套参数可以配置升降机：1.配置UseSSD和SSDType  2.配置InstanceType，不需要配置InstanceMode。这两套第二套参数的优先级更高
 """
 
 
 class ResizeUDBInstanceRequestSchema(schema.RequestSchema):
-    """ ResizeUDBInstance - 修改（升级和降级）UDB实例的配置，包括内存和磁盘的配置，对于内存升级无需关闭实例，其他场景需要事先关闭实例。两套参数可以配置升降机：1.配置UseSSD和SSDType  2.配置InstanceType，不需要配置InstanceMode。这两套第二套参数的优先级更高
-    """
+    """ResizeUDBInstance - 修改（升级和降级）UDB实例的配置，包括内存和磁盘的配置，对于内存升级无需关闭实例，其他场景需要事先关闭实例。两套参数可以配置升降机：1.配置UseSSD和SSDType  2.配置InstanceType，不需要配置InstanceMode。这两套第二套参数的优先级更高"""
 
     fields = {
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
         "InstanceMode": fields.Str(required=False, dump_to="InstanceMode"),
         "InstanceType": fields.Str(required=False, dump_to="InstanceType"),
@@ -1215,195 +1138,181 @@
         "UDBCId": fields.Str(required=False, dump_to="UDBCId"),
         "UseSSD": fields.Bool(required=False, dump_to="UseSSD"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ResizeUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ ResizeUDBInstance - 修改（升级和降级）UDB实例的配置，包括内存和磁盘的配置，对于内存升级无需关闭实例，其他场景需要事先关闭实例。两套参数可以配置升降机：1.配置UseSSD和SSDType  2.配置InstanceType，不需要配置InstanceMode。这两套第二套参数的优先级更高
-    """
+    """ResizeUDBInstance - 修改（升级和降级）UDB实例的配置，包括内存和磁盘的配置，对于内存升级无需关闭实例，其他场景需要事先关闭实例。两套参数可以配置升降机：1.配置UseSSD和SSDType  2.配置InstanceType，不需要配置InstanceMode。这两套第二套参数的优先级更高"""
 
     fields = {}
 
 
 """
 API: RestartUDBInstance
 
 重启UDB实例
 """
 
 
 class RestartUDBInstanceRequestSchema(schema.RequestSchema):
-    """ RestartUDBInstance - 重启UDB实例
-    """
+    """RestartUDBInstance - 重启UDB实例"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class RestartUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ RestartUDBInstance - 重启UDB实例
-    """
+    """RestartUDBInstance - 重启UDB实例"""
 
     fields = {}
 
 
 """
 API: StartUDBInstance
 
 启动UDB实例
 """
 
 
 class StartUDBInstanceRequestSchema(schema.RequestSchema):
-    """ StartUDBInstance - 启动UDB实例
-    """
+    """StartUDBInstance - 启动UDB实例"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class StartUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ StartUDBInstance - 启动UDB实例
-    """
+    """StartUDBInstance - 启动UDB实例"""
 
     fields = {}
 
 
 """
 API: StopUDBInstance
 
 关闭UDB实例
 """
 
 
 class StopUDBInstanceRequestSchema(schema.RequestSchema):
-    """ StopUDBInstance - 关闭UDB实例
-    """
+    """StopUDBInstance - 关闭UDB实例"""
 
     fields = {
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ForceToKill": fields.Bool(required=False, dump_to="ForceToKill"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class StopUDBInstanceResponseSchema(schema.ResponseSchema):
-    """ StopUDBInstance - 关闭UDB实例
-    """
+    """StopUDBInstance - 关闭UDB实例"""
 
     fields = {}
 
 
 """
 API: SwitchUDBInstanceToHA
 
 普通UDB切换为高可用，原db状态为WaitForSwitch时，调用该api
 """
 
 
 class SwitchUDBInstanceToHARequestSchema(schema.RequestSchema):
-    """ SwitchUDBInstanceToHA - 普通UDB切换为高可用，原db状态为WaitForSwitch时，调用该api
-    """
+    """SwitchUDBInstanceToHA - 普通UDB切换为高可用，原db状态为WaitForSwitch时，调用该api"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Str(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class SwitchUDBInstanceToHAResponseSchema(schema.ResponseSchema):
-    """ SwitchUDBInstanceToHA - 普通UDB切换为高可用，原db状态为WaitForSwitch时，调用该api
-    """
+    """SwitchUDBInstanceToHA - 普通UDB切换为高可用，原db状态为WaitForSwitch时，调用该api"""
 
     fields = {"DBId": fields.Str(required=False, load_from="DBId")}
 
 
 """
 API: UpdateUDBInstanceBackupStrategy
 
 修改UDB自动备份策略
 """
 
 
 class UpdateUDBInstanceBackupStrategyRequestSchema(schema.RequestSchema):
-    """ UpdateUDBInstanceBackupStrategy - 修改UDB自动备份策略
-    """
+    """UpdateUDBInstanceBackupStrategy - 修改UDB自动备份策略"""
 
     fields = {
         "BackupDate": fields.Str(required=False, dump_to="BackupDate"),
         "BackupMethod": fields.Str(required=False, dump_to="BackupMethod"),
         "BackupTime": fields.Int(required=False, dump_to="BackupTime"),
         "DBId": fields.Str(required=True, dump_to="DBId"),
         "ForceDump": fields.Bool(required=False, dump_to="ForceDump"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class UpdateUDBInstanceBackupStrategyResponseSchema(schema.ResponseSchema):
-    """ UpdateUDBInstanceBackupStrategy - 修改UDB自动备份策略
-    """
+    """UpdateUDBInstanceBackupStrategy - 修改UDB自动备份策略"""
 
     fields = {}
 
 
 """
 API: UpdateUDBInstanceSlaveBackupSwitch
 
 开启或者关闭UDB从库备份
 """
 
 
 class UpdateUDBInstanceSlaveBackupSwitchRequestSchema(schema.RequestSchema):
-    """ UpdateUDBInstanceSlaveBackupSwitch - 开启或者关闭UDB从库备份
-    """
+    """UpdateUDBInstanceSlaveBackupSwitch - 开启或者关闭UDB从库备份"""
 
     fields = {
         "BackupSwitch": fields.Int(required=True, dump_to="BackupSwitch"),
         "MasterDBId": fields.Str(required=True, dump_to="MasterDBId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SlaveDBId": fields.Str(required=False, dump_to="SlaveDBId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class UpdateUDBInstanceSlaveBackupSwitchResponseSchema(schema.ResponseSchema):
-    """ UpdateUDBInstanceSlaveBackupSwitch - 开启或者关闭UDB从库备份
-    """
+    """UpdateUDBInstanceSlaveBackupSwitch - 开启或者关闭UDB从库备份"""
 
     fields = {}
 
 
 """
 API: UpdateUDBParamGroup
 
 更新UDB配置参数项
 """
 
 
 class UpdateUDBParamGroupRequestSchema(schema.RequestSchema):
-    """ UpdateUDBParamGroup - 更新UDB配置参数项
-    """
+    """UpdateUDBParamGroup - 更新UDB配置参数项"""
 
     fields = {
         "Description": fields.Str(required=False, dump_to="Description"),
         "GroupId": fields.Int(required=True, dump_to="GroupId"),
         "Key": fields.Str(required=False, dump_to="Key"),
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -1411,30 +1320,28 @@
         "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
         "Value": fields.Str(required=False, dump_to="Value"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpdateUDBParamGroupResponseSchema(schema.ResponseSchema):
-    """ UpdateUDBParamGroup - 更新UDB配置参数项
-    """
+    """UpdateUDBParamGroup - 更新UDB配置参数项"""
 
     fields = {}
 
 
 """
 API: UploadUDBParamGroup
 
 导入UDB配置
 """
 
 
 class UploadUDBParamGroupRequestSchema(schema.RequestSchema):
-    """ UploadUDBParamGroup - 导入UDB配置
-    """
+    """UploadUDBParamGroup - 导入UDB配置"""
 
     fields = {
         "Content": fields.Str(required=True, dump_to="Content"),
         "DBTypeId": fields.Str(required=True, dump_to="DBTypeId"),
         "Description": fields.Str(required=True, dump_to="Description"),
         "GroupName": fields.Str(required=True, dump_to="GroupName"),
         "ParamGroupTypeId": fields.Int(
@@ -1444,11 +1351,10 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UploadUDBParamGroupResponseSchema(schema.ResponseSchema):
-    """ UploadUDBParamGroup - 导入UDB配置
-    """
+    """UploadUDBParamGroup - 导入UDB配置"""
 
     fields = {"GroupId": fields.Int(required=False, load_from="GroupId")}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udb/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udb/schemas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class UDBBackupSetSchema(schema.ResponseSchema):
-    """ UDBBackupSet - DescribeUDBBackup
-    """
+    """UDBBackupSet - DescribeUDBBackup"""
 
     fields = {
         "BackupEndTime": fields.Int(required=False, load_from="BackupEndTime"),
         "BackupId": fields.Int(required=False, load_from="BackupId"),
         "BackupName": fields.Str(required=False, load_from="BackupName"),
         "BackupSize": fields.Int(required=False, load_from="BackupSize"),
         "BackupTime": fields.Int(required=False, load_from="BackupTime"),
@@ -20,16 +19,15 @@
         "ErrorInfo": fields.Str(required=False, load_from="ErrorInfo"),
         "State": fields.Str(required=False, load_from="State"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UDBSlaveInstanceSetSchema(schema.ResponseSchema):
-    """ UDBSlaveInstanceSet - DescribeUDBSlaveInstance
-    """
+    """UDBSlaveInstanceSet - DescribeUDBSlaveInstance"""
 
     fields = {
         "AdminUser": fields.Str(required=False, load_from="AdminUser"),
         "BackupBeginTime": fields.Int(
             required=False, load_from="BackupBeginTime"
         ),
         "BackupBlacklist": fields.Str(
@@ -74,16 +72,15 @@
         "VirtualIP": fields.Str(required=False, load_from="VirtualIP"),
         "VirtualIPMac": fields.Str(required=False, load_from="VirtualIPMac"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UDBInstanceSetSchema(schema.ResponseSchema):
-    """ UDBInstanceSet - DescribeUDBInstance
-    """
+    """UDBInstanceSet - DescribeUDBInstance"""
 
     fields = {
         "AdminUser": fields.Str(required=False, load_from="AdminUser"),
         "BackupBeginTime": fields.Int(
             required=False, load_from="BackupBeginTime"
         ),
         "BackupBlacklist": fields.Str(
@@ -130,38 +127,35 @@
         "VirtualIP": fields.Str(required=False, load_from="VirtualIP"),
         "VirtualIPMac": fields.Str(required=False, load_from="VirtualIPMac"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UDBInstanceBinlogSetSchema(schema.ResponseSchema):
-    """ UDBInstanceBinlogSet - DescribeUDBInstanceBinlog
-    """
+    """UDBInstanceBinlogSet - DescribeUDBInstanceBinlog"""
 
     fields = {
         "BeginTime": fields.Int(required=False, load_from="BeginTime"),
         "EndTime": fields.Int(required=False, load_from="EndTime"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Size": fields.Int(required=False, load_from="Size"),
     }
 
 
 class UDBInstancePriceSetSchema(schema.ResponseSchema):
-    """ UDBInstancePriceSet - DescribeUDBInstancePrice
-    """
+    """UDBInstancePriceSet - DescribeUDBInstancePrice"""
 
     fields = {
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
         "Price": fields.Int(required=False, load_from="Price"),
     }
 
 
 class LogPackageDataSetSchema(schema.ResponseSchema):
-    """ LogPackageDataSet - DescribeUDBLogPackage
-    """
+    """LogPackageDataSet - DescribeUDBLogPackage"""
 
     fields = {
         "BackupId": fields.Int(required=False, load_from="BackupId"),
         "BackupName": fields.Str(required=False, load_from="BackupName"),
         "BackupSize": fields.Int(required=False, load_from="BackupSize"),
         "BackupTime": fields.Int(required=False, load_from="BackupTime"),
         "BackupType": fields.Int(required=False, load_from="BackupType"),
@@ -170,42 +164,39 @@
         "DBName": fields.Str(required=False, load_from="DBName"),
         "State": fields.Str(required=False, load_from="State"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UDBParamMemberSetSchema(schema.ResponseSchema):
-    """ UDBParamMemberSet - DescribeUDBParamGroup
-    """
+    """UDBParamMemberSet - DescribeUDBParamGroup"""
 
     fields = {
         "AllowedVal": fields.Str(required=False, load_from="AllowedVal"),
         "ApplyType": fields.Int(required=False, load_from="ApplyType"),
         "FormatType": fields.Int(required=False, load_from="FormatType"),
         "Key": fields.Str(required=False, load_from="Key"),
         "Modifiable": fields.Bool(required=False, load_from="Modifiable"),
         "Value": fields.Str(required=False, load_from="Value"),
         "ValueType": fields.Int(required=False, load_from="ValueType"),
     }
 
 
 class UDBParamGroupSetSchema(schema.ResponseSchema):
-    """ UDBParamGroupSet - DescribeUDBParamGroup
-    """
+    """UDBParamGroupSet - DescribeUDBParamGroup"""
 
     fields = {
         "DBTypeId": fields.Str(required=False, load_from="DBTypeId"),
         "Description": fields.Str(required=False, load_from="Description"),
         "GroupId": fields.Int(required=False, load_from="GroupId"),
         "GroupName": fields.Str(required=False, load_from="GroupName"),
         "Modifiable": fields.Bool(required=False, load_from="Modifiable"),
         "ParamMember": fields.List(UDBParamMemberSetSchema()),
         "RegionFlag": fields.Bool(required=False, load_from="RegionFlag"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UDBTypeSetSchema(schema.ResponseSchema):
-    """ UDBTypeSet - DescribeUDBType
-    """
+    """UDBTypeSet - DescribeUDBType"""
 
     fields = {"DBTypeId": fields.Str(required=False, load_from="DBTypeId")}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udisk/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udisk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,59 +10,59 @@
 class UDiskClient(Client):
     def __init__(
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UDiskClient, self).__init__(config, transport, middleware, logger)
 
     def attach_udisk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ AttachUDisk - 将一个可用的UDisk挂载到某台主机上，当UDisk挂载成功后，还需要在主机内部进行文件系统操作
+        """AttachUDisk - 将一个可用的UDisk挂载到某台主机上，当UDisk挂载成功后，还需要在主机内部进行文件系统操作
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UDiskId** (str) - (Required) 需要挂载的UDisk实例ID.
         - **UHostId** (str) - (Required) UHost实例ID
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **MultiAttach** (str) - 是否允许多点挂载（Yes: 允许多点挂载， No: 不允许多点挂载， 不填默认Yes ）
-        
+
         **Response**
 
         - **UDiskId** (str) - 挂载的UDisk实例ID
         - **UHostId** (str) - 挂载的UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.AttachUDiskRequestSchema().dumps(d)
 
         resp = self.invoke("AttachUDisk", d, **kwargs)
         return apis.AttachUDiskResponseSchema().loads(resp)
 
     def clone_udisk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CloneUDisk - 从UDisk创建UDisk克隆
+        """CloneUDisk - 从UDisk创建UDisk克隆
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 实例名称
         - **SourceId** (str) - (Required) 克隆父Disk的Id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - Year , Month, Dynamic，Postpay 默认: Dynamic
         - **Comment** (str) - Disk注释
         - **CouponId** (str) - 使用的代金券id
         - **Quantity** (int) - 购买时长 默认: 1
         - **UDataArkMode** (str) - 方舟是否开启，"Yes":开启，"No":关闭；默认为"No"
-        
+
         **Response**
 
         - **UDiskId** (list) - 创建UDisk Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CloneUDiskRequestSchema().dumps(d)
 
         # build options
@@ -70,69 +70,69 @@
 
         resp = self.invoke("CloneUDisk", d, **kwargs)
         return apis.CloneUDiskResponseSchema().loads(resp)
 
     def clone_udisk_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CloneUDiskSnapshot - 从快照创建UDisk克隆
+        """CloneUDiskSnapshot - 从快照创建UDisk克隆
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 实例名称
         - **Size** (int) - (Required) 购买UDisk大小,单位:GB,范围[1~2000], 权限位控制可达8T,若需要请申请开通相关权限。
         - **SourceId** (str) - (Required) 克隆父Snapshot的Id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - Year , Month, Dynamic，Postpay 默认: Dynamic
         - **Comment** (str) - Disk注释
         - **CouponId** (str) - 使用的代金券id
         - **Quantity** (int) - 购买时长 默认: 1
         - **UDataArkMode** (str) - 是否开启数据方舟   默认:No
-        
+
         **Response**
 
         - **UDiskId** (list) - 创建UDisk Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CloneUDiskSnapshotRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CloneUDiskSnapshot", d, **kwargs)
         return apis.CloneUDiskSnapshotResponseSchema().loads(resp)
 
     def create_udisk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateUDisk - 创建UDisk磁盘
+        """CreateUDisk - 创建UDisk磁盘
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 实例名称
         - **Size** (int) - (Required) 购买UDisk大小,单位:GB,普通盘: 范围[1~2000], 权限位控制可达8T,若需要请申请开通相关权限;SSD盘： 范围[1~4000]。
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - Year , Month, Dynamic, Postpay, Trial 默认: Dynamic
         - **CmkId** (str) - 加密需要的cmk id，UKmsMode为Yes时，必填
         - **CouponId** (str) - 使用的代金券id
         - **DiskType** (str) - UDisk 类型: DataDisk（普通数据盘），SSDDataDisk（SSD数据盘），RSSDDataDisk（RSSD数据盘），默认值（DataDisk）
         - **Quantity** (int) - 购买时长 默认: 1
         - **Tag** (str) - 业务组 默认：Default
         - **UDataArkMode** (str) - 是否开启数据方舟
         - **UKmsMode** (str) - 是否加密。Yes：加密，No：不加密，默认值（No）
-        
+
         **Response**
 
         - **UDiskId** (list) - UDisk实例Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDiskRequestSchema().dumps(d)
 
         # build options
@@ -140,116 +140,116 @@
 
         resp = self.invoke("CreateUDisk", d, **kwargs)
         return apis.CreateUDiskResponseSchema().loads(resp)
 
     def create_udisk_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUDiskSnapshot - 创建snapshot快照
+        """CreateUDiskSnapshot - 创建snapshot快照
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 快照名称
         - **UDiskId** (str) - (Required) 快照的UDisk的Id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - Year , Month, Dynamic 默认: Dynamic
         - **Comment** (str) - 快照描述
         - **Quantity** (int) - 购买时长 默认: 1
-        
+
         **Response**
 
         - **SnapshotId** (list) - 快照Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUDiskSnapshotRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreateUDiskSnapshot", d, **kwargs)
         return apis.CreateUDiskSnapshotResponseSchema().loads(resp)
 
     def delete_udisk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteUDisk - 删除UDisk
+        """DeleteUDisk - 删除UDisk
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UDiskId** (str) - (Required) 要删除的UDisk的Id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteUDiskRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUDisk", d, **kwargs)
         return apis.DeleteUDiskResponseSchema().loads(resp)
 
     def delete_udisk_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUDiskSnapshot - 删除Snapshot
+        """DeleteUDiskSnapshot - 删除Snapshot
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SnapshotId** (str) - 快照Id(填写后不能填写UDisk Id)
         - **UDiskId** (str) - UDisk Id,删除该盘所创建出来的所有快照(填写后不能填写SnapshotId)
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteUDiskSnapshotRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUDiskSnapshot", d, **kwargs)
         return apis.DeleteUDiskSnapshotResponseSchema().loads(resp)
 
     def describe_udisk(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDisk - 获取UDisk实例
+        """DescribeUDisk - 获取UDisk实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DiskType** (str) - ProtocolVersion字段为1时，需结合IsBoot确定具体磁盘类型:普通数据盘：DiskType:"CLOUD_NORMAL",IsBoot:"False"； 普通系统盘：DiskType:"CLOUD_NORMAL",IsBoot:"True"；SSD数据盘：DiskType:"CLOUD_SSD",IsBoot:"False"；SSD系统盘：DiskType:"CLOUD_SSD",IsBoot:"True"；RSSD数据盘：DiskType:"CLOUD_RSSD",IsBoot:"False"；为空拉取所有。ProtocolVersion字段为0或没有该字段时，可设为以下几个值:普通数据盘：DataDisk；普通系统盘；SystemDisk；SSD数据盘：SSDDataDisk；SSD系统盘：SSDSystemDisk；RSSD数据盘：RSSDDataDisk；为空拉取所有。
         - **IsBoot** (str) - ProtocolVersion字段为1且DiskType不为空时，必须设置，设置规则请参照DiskType；ProtocolVersion字段为1且DiskType为空时，该字段无效。ProtocolVersion字段为0或没有该字段时，该字段无效。
         - **Limit** (int) - 返回数据长度, 默认为20
         - **Offset** (int) - 数据偏移量, 默认为0
         - **ProtocolVersion** (int) - 请求协议版本，建议升级为1，为1时DiskType与UHost磁盘类型定义一致；默认为0
         - **UDiskId** (str) - UDisk Id(留空返回全部)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UDiskDataSet** 模型定义
         - **TotalCount** (int) - 根据过滤条件得到的总数
-        
+
         **Response Model**
-        
-        **UDiskDataSet** 
-        
+
+        **UDiskDataSet**
+
         - **ArkSwitchEnable** (int) - 是否支持开启方舟，1支持 ，0不支持
         - **ChargeType** (str) - Year,Month,Dynamic,Trial,Postpay
         - **CloneEnable** (int) - 是否支持克隆，1支持 ，0不支持
         - **CmkId** (str) - 该盘的cmk id
         - **CmkIdAlias** (str) - cmk id 别名
         - **CmkIdStatus** (str) - 该盘cmk的状态, Enabled(正常)，Disabled(失效)，Deleted(删除)，NoCmkId(非加密盘)
         - **CreateTime** (int) - 创建时间
@@ -283,35 +283,35 @@
 
         resp = self.invoke("DescribeUDisk", d, **kwargs)
         return apis.DescribeUDiskResponseSchema().loads(resp)
 
     def describe_udisk_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDiskPrice - 获取UDisk实例价格信息
+        """DescribeUDiskPrice - 获取UDisk实例价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 购买UDisk大小,单位:GB,范围[1~1000]
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - Year， Month， Dynamic，Trial，默认: Dynamic
         - **DiskType** (str) - UDisk 类型: DataDisk（普通数据盘），SSDDataDisk（SSD数据盘），SystemDisk（普通系统盘），SSDSystemDisk（SSD系统盘），RSSDDataDisk（RSSD数据盘），默认值（DataDisk）
         - **Quantity** (int) - 购买UDisk的时长，默认值为1
         - **UDataArkMode** (str) - 是否打开数据方舟, 打开"Yes",关闭"No", 默认关闭
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UDiskPriceDataSet** 模型定义
-        
+
         **Response Model**
-        
-        **UDiskPriceDataSet** 
-        
+
+        **UDiskPriceDataSet**
+
         - **ChargeName** (str) - "UDataArk","UDisk"
         - **ChargeType** (str) - Year， Month， Dynamic，Trial
         - **OriginalPrice** (int) - 用户折后价
         - **Price** (int) - 价格 (单位: 分)
 
         """
         # build request
@@ -321,35 +321,35 @@
 
         resp = self.invoke("DescribeUDiskPrice", d, **kwargs)
         return apis.DescribeUDiskPriceResponseSchema().loads(resp)
 
     def describe_udisk_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDiskSnapshot - 获取UDisk快照
+        """DescribeUDiskSnapshot - 获取UDisk快照
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 返回数据长度, 默认为20
         - **Offset** (int) - 数据偏移量, 默认为0
         - **SnapshotId** (str) - 快照id，SnapshotId , UDiskId 同时传SnapshotId优先
         - **UDiskId** (str) - UDiskId,返回该盘所做快照.(必须同时传Zone)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UDiskSnapshotSet** 模型定义
         - **TotalCount** (int) - 根据过滤条件得到的总数
-        
+
         **Response Model**
-        
-        **UDiskSnapshotSet** 
-        
+
+        **UDiskSnapshotSet**
+
         - **CmkId** (str) - 该快照的cmk id
         - **CmkIdAlias** (str) - cmk id 别名
         - **CmkIdStatus** (str) - 该快照cmk的状态, Enabled(正常)，Disabled(失效)，Deleted(删除)，NoCmkId(非加密盘)
         - **Comment** (str) - 快照描述
         - **CreateTime** (int) - 创建时间
         - **DataKey** (str) - 该快照的密文密钥
         - **DiskType** (int) - 磁盘类型，0:数据盘，1:系统盘
@@ -373,154 +373,154 @@
 
         resp = self.invoke("DescribeUDiskSnapshot", d, **kwargs)
         return apis.DescribeUDiskSnapshotResponseSchema().loads(resp)
 
     def describe_udisk_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDiskUpgradePrice - 获取UDisk升级价格信息
+        """DescribeUDiskUpgradePrice - 获取UDisk升级价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 购买UDisk大小,单位:GB,范围[1~2000], 权限位控制可达8T,若需要请申请开通相关权限。
         - **SourceId** (str) - (Required) 升级目标UDisk ID
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DiskType** (str) - 磁盘类型，SSDDataDisk:ssd数据盘,DataDisk:普通数据盘,SystemDisk:普通系统盘,SSDSystemDisk:ssd系统盘。默认为DataDisk
         - **UDataArkMode** (str) - 是否打开数据方舟, 打开"Yes",关闭"No", 默认关闭
-        
+
         **Response**
 
         - **OriginalPrice** (int) - 用户折后价
         - **Price** (int) - 价格
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUDiskUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUDiskUpgradePrice", d, **kwargs)
         return apis.DescribeUDiskUpgradePriceResponseSchema().loads(resp)
 
     def detach_udisk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DetachUDisk - 卸载某个已经挂载在指定UHost实例上的UDisk
+        """DetachUDisk - 卸载某个已经挂载在指定UHost实例上的UDisk
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UDiskId** (str) - (Required) 需要卸载的UDisk实例ID
         - **UHostId** (str) - (Required) UHost实例ID
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UDiskId** (str) - 卸载的UDisk实例ID
         - **UHostId** (str) - 卸载的UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DetachUDiskRequestSchema().dumps(d)
 
         resp = self.invoke("DetachUDisk", d, **kwargs)
         return apis.DetachUDiskResponseSchema().loads(resp)
 
     def rename_udisk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ RenameUDisk - 重命名UDisk
+        """RenameUDisk - 重命名UDisk
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UDiskId** (str) - (Required) 重命名的UDisk的Id
         - **UDiskName** (str) - (Required) 重命名UDisk的name
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.RenameUDiskRequestSchema().dumps(d)
 
         resp = self.invoke("RenameUDisk", d, **kwargs)
         return apis.RenameUDiskResponseSchema().loads(resp)
 
     def resize_udisk(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ ResizeUDisk - 调整UDisk容量
+        """ResizeUDisk - 调整UDisk容量
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 调整后大小, 单位:GB, 范围[1~2000],权限位控制可达8000,若需要请申请开通相关权限。
         - **UDiskId** (str) - (Required) UDisk Id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **CouponId** (str) - 使用的代金券id
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ResizeUDiskRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeUDisk", d, **kwargs)
         return apis.ResizeUDiskResponseSchema().loads(resp)
 
     def restore_udisk(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RestoreUDisk - 从备份恢复数据至UDisk
+        """RestoreUDisk - 从备份恢复数据至UDisk
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UDiskId** (str) - (Required) 需要恢复的盘id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SnapshotId** (str) - 从指定的快照恢复
         - **SnapshotTime** (int) - 指定从方舟恢复的备份时间点
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.RestoreUDiskRequestSchema().dumps(d)
 
         resp = self.invoke("RestoreUDisk", d, **kwargs)
         return apis.RestoreUDiskResponseSchema().loads(resp)
 
     def set_udisk__udataark_mode(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ SetUDiskUDataArkMode - 设置UDisk数据方舟的状态
+        """SetUDiskUDataArkMode - 设置UDisk数据方舟的状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UDataArkMode** (str) - (Required) 是否开启数据方舟，开启:"Yes", 不支持:"No"
         - **UDiskId** (str) - (Required) 需要设置数据方舟的UDisk的Id
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.SetUDiskUDataArkModeRequestSchema().dumps(d)
 
         resp = self.invoke("SetUDiskUDataArkMode", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udisk/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udisk/schemas/apis.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 API: AttachUDisk
 
 将一个可用的UDisk挂载到某台主机上，当UDisk挂载成功后，还需要在主机内部进行文件系统操作
 """
 
 
 class AttachUDiskRequestSchema(schema.RequestSchema):
-    """ AttachUDisk - 将一个可用的UDisk挂载到某台主机上，当UDisk挂载成功后，还需要在主机内部进行文件系统操作
-    """
+    """AttachUDisk - 将一个可用的UDisk挂载到某台主机上，当UDisk挂载成功后，还需要在主机内部进行文件系统操作"""
 
     fields = {
         "MultiAttach": fields.Str(required=False, dump_to="MultiAttach"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class AttachUDiskResponseSchema(schema.ResponseSchema):
-    """ AttachUDisk - 将一个可用的UDisk挂载到某台主机上，当UDisk挂载成功后，还需要在主机内部进行文件系统操作
-    """
+    """AttachUDisk - 将一个可用的UDisk挂载到某台主机上，当UDisk挂载成功后，还需要在主机内部进行文件系统操作"""
 
     fields = {
         "UDiskId": fields.Str(required=False, load_from="UDiskId"),
         "UHostId": fields.Str(required=False, load_from="UHostId"),
     }
 
 
@@ -43,16 +41,15 @@
 API: CloneUDisk
 
 从UDisk创建UDisk克隆
 """
 
 
 class CloneUDiskRequestSchema(schema.RequestSchema):
-    """ CloneUDisk - 从UDisk创建UDisk克隆
-    """
+    """CloneUDisk - 从UDisk创建UDisk克隆"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "Comment": fields.Str(required=False, dump_to="Comment"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -61,16 +58,15 @@
         "SourceId": fields.Str(required=True, dump_to="SourceId"),
         "UDataArkMode": fields.Str(required=False, dump_to="UDataArkMode"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CloneUDiskResponseSchema(schema.ResponseSchema):
-    """ CloneUDisk - 从UDisk创建UDisk克隆
-    """
+    """CloneUDisk - 从UDisk创建UDisk克隆"""
 
     fields = {
         "UDiskId": fields.List(
             fields.Str(), required=False, load_from="UDiskId"
         )
     }
 
@@ -79,16 +75,15 @@
 API: CloneUDiskSnapshot
 
 从快照创建UDisk克隆
 """
 
 
 class CloneUDiskSnapshotRequestSchema(schema.RequestSchema):
-    """ CloneUDiskSnapshot - 从快照创建UDisk克隆
-    """
+    """CloneUDiskSnapshot - 从快照创建UDisk克隆"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "Comment": fields.Str(required=False, dump_to="Comment"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -98,16 +93,15 @@
         "SourceId": fields.Str(required=True, dump_to="SourceId"),
         "UDataArkMode": fields.Str(required=False, dump_to="UDataArkMode"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CloneUDiskSnapshotResponseSchema(schema.ResponseSchema):
-    """ CloneUDiskSnapshot - 从快照创建UDisk克隆
-    """
+    """CloneUDiskSnapshot - 从快照创建UDisk克隆"""
 
     fields = {
         "UDiskId": fields.List(
             fields.Str(), required=False, load_from="UDiskId"
         )
     }
 
@@ -116,16 +110,15 @@
 API: CreateUDisk
 
 创建UDisk磁盘
 """
 
 
 class CreateUDiskRequestSchema(schema.RequestSchema):
-    """ CreateUDisk - 创建UDisk磁盘
-    """
+    """CreateUDisk - 创建UDisk磁盘"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CmkId": fields.Str(required=False, dump_to="CmkId"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "DiskType": fields.Str(required=False, dump_to="DiskType"),
         "Name": fields.Str(required=True, dump_to="Name"),
@@ -137,16 +130,15 @@
         "UDataArkMode": fields.Str(required=False, dump_to="UDataArkMode"),
         "UKmsMode": fields.Str(required=False, dump_to="UKmsMode"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateUDiskResponseSchema(schema.ResponseSchema):
-    """ CreateUDisk - 创建UDisk磁盘
-    """
+    """CreateUDisk - 创建UDisk磁盘"""
 
     fields = {
         "UDiskId": fields.List(
             fields.Str(), required=False, load_from="UDiskId"
         )
     }
 
@@ -155,32 +147,30 @@
 API: CreateUDiskSnapshot
 
 创建snapshot快照
 """
 
 
 class CreateUDiskSnapshotRequestSchema(schema.RequestSchema):
-    """ CreateUDiskSnapshot - 创建snapshot快照
-    """
+    """CreateUDiskSnapshot - 创建snapshot快照"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "Comment": fields.Str(required=False, dump_to="Comment"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateUDiskSnapshotResponseSchema(schema.ResponseSchema):
-    """ CreateUDiskSnapshot - 创建snapshot快照
-    """
+    """CreateUDiskSnapshot - 创建snapshot快照"""
 
     fields = {
         "SnapshotId": fields.List(
             fields.Str(), required=True, load_from="SnapshotId"
         )
     }
 
@@ -189,69 +179,64 @@
 API: DeleteUDisk
 
 删除UDisk
 """
 
 
 class DeleteUDiskRequestSchema(schema.RequestSchema):
-    """ DeleteUDisk - 删除UDisk
-    """
+    """DeleteUDisk - 删除UDisk"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteUDiskResponseSchema(schema.ResponseSchema):
-    """ DeleteUDisk - 删除UDisk
-    """
+    """DeleteUDisk - 删除UDisk"""
 
     fields = {}
 
 
 """
 API: DeleteUDiskSnapshot
 
 删除Snapshot
 """
 
 
 class DeleteUDiskSnapshotRequestSchema(schema.RequestSchema):
-    """ DeleteUDiskSnapshot - 删除Snapshot
-    """
+    """DeleteUDiskSnapshot - 删除Snapshot"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SnapshotId": fields.Str(required=False, dump_to="SnapshotId"),
         "UDiskId": fields.Str(required=False, dump_to="UDiskId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DeleteUDiskSnapshotResponseSchema(schema.ResponseSchema):
-    """ DeleteUDiskSnapshot - 删除Snapshot
-    """
+    """DeleteUDiskSnapshot - 删除Snapshot"""
 
     fields = {}
 
 
 """
 API: DescribeUDisk
 
 获取UDisk实例
 """
 
 
 class DescribeUDiskRequestSchema(schema.RequestSchema):
-    """ DescribeUDisk - 获取UDisk实例
-    """
+    """DescribeUDisk - 获取UDisk实例"""
 
     fields = {
         "DiskType": fields.Str(required=False, dump_to="DiskType"),
         "IsBoot": fields.Str(required=False, dump_to="IsBoot"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -261,16 +246,15 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDiskId": fields.Str(required=False, dump_to="UDiskId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDiskResponseSchema(schema.ResponseSchema):
-    """ DescribeUDisk - 获取UDisk实例
-    """
+    """DescribeUDisk - 获取UDisk实例"""
 
     fields = {
         "DataSet": fields.List(
             models.UDiskDataSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -280,32 +264,30 @@
 API: DescribeUDiskPrice
 
 获取UDisk实例价格信息
 """
 
 
 class DescribeUDiskPriceRequestSchema(schema.RequestSchema):
-    """ DescribeUDiskPrice - 获取UDisk实例价格信息
-    """
+    """DescribeUDiskPrice - 获取UDisk实例价格信息"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "DiskType": fields.Str(required=False, dump_to="DiskType"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "UDataArkMode": fields.Str(required=False, dump_to="UDataArkMode"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUDiskPriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUDiskPrice - 获取UDisk实例价格信息
-    """
+    """DescribeUDiskPrice - 获取UDisk实例价格信息"""
 
     fields = {
         "DataSet": fields.List(
             models.UDiskPriceDataSetSchema(),
             required=False,
             load_from="DataSet",
         )
@@ -316,31 +298,29 @@
 API: DescribeUDiskSnapshot
 
 获取UDisk快照
 """
 
 
 class DescribeUDiskSnapshotRequestSchema(schema.RequestSchema):
-    """ DescribeUDiskSnapshot - 获取UDisk快照
-    """
+    """DescribeUDiskSnapshot - 获取UDisk快照"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SnapshotId": fields.Str(required=False, dump_to="SnapshotId"),
         "UDiskId": fields.Str(required=False, dump_to="UDiskId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUDiskSnapshotResponseSchema(schema.ResponseSchema):
-    """ DescribeUDiskSnapshot - 获取UDisk快照
-    """
+    """DescribeUDiskSnapshot - 获取UDisk快照"""
 
     fields = {
         "DataSet": fields.List(
             models.UDiskSnapshotSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -350,31 +330,29 @@
 API: DescribeUDiskUpgradePrice
 
 获取UDisk升级价格信息
 """
 
 
 class DescribeUDiskUpgradePriceRequestSchema(schema.RequestSchema):
-    """ DescribeUDiskUpgradePrice - 获取UDisk升级价格信息
-    """
+    """DescribeUDiskUpgradePrice - 获取UDisk升级价格信息"""
 
     fields = {
         "DiskType": fields.Str(required=False, dump_to="DiskType"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "SourceId": fields.Str(required=True, dump_to="SourceId"),
         "UDataArkMode": fields.Str(required=False, dump_to="UDataArkMode"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUDiskUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUDiskUpgradePrice - 获取UDisk升级价格信息
-    """
+    """DescribeUDiskUpgradePrice - 获取UDisk升级价格信息"""
 
     fields = {
         "OriginalPrice": fields.Int(required=False, load_from="OriginalPrice"),
         "Price": fields.Int(required=False, load_from="Price"),
     }
 
 
@@ -382,29 +360,27 @@
 API: DetachUDisk
 
 卸载某个已经挂载在指定UHost实例上的UDisk
 """
 
 
 class DetachUDiskRequestSchema(schema.RequestSchema):
-    """ DetachUDisk - 卸载某个已经挂载在指定UHost实例上的UDisk
-    """
+    """DetachUDisk - 卸载某个已经挂载在指定UHost实例上的UDisk"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DetachUDiskResponseSchema(schema.ResponseSchema):
-    """ DetachUDisk - 卸载某个已经挂载在指定UHost实例上的UDisk
-    """
+    """DetachUDisk - 卸载某个已经挂载在指定UHost实例上的UDisk"""
 
     fields = {
         "UDiskId": fields.Str(required=False, load_from="UDiskId"),
         "UHostId": fields.Str(required=False, load_from="UHostId"),
     }
 
 
@@ -412,107 +388,99 @@
 API: RenameUDisk
 
 重命名UDisk
 """
 
 
 class RenameUDiskRequestSchema(schema.RequestSchema):
-    """ RenameUDisk - 重命名UDisk
-    """
+    """RenameUDisk - 重命名UDisk"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "UDiskName": fields.Str(required=True, dump_to="UDiskName"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class RenameUDiskResponseSchema(schema.ResponseSchema):
-    """ RenameUDisk - 重命名UDisk
-    """
+    """RenameUDisk - 重命名UDisk"""
 
     fields = {}
 
 
 """
 API: ResizeUDisk
 
 调整UDisk容量
 """
 
 
 class ResizeUDiskRequestSchema(schema.RequestSchema):
-    """ ResizeUDisk - 调整UDisk容量
-    """
+    """ResizeUDisk - 调整UDisk容量"""
 
     fields = {
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ResizeUDiskResponseSchema(schema.ResponseSchema):
-    """ ResizeUDisk - 调整UDisk容量
-    """
+    """ResizeUDisk - 调整UDisk容量"""
 
     fields = {}
 
 
 """
 API: RestoreUDisk
 
 从备份恢复数据至UDisk
 """
 
 
 class RestoreUDiskRequestSchema(schema.RequestSchema):
-    """ RestoreUDisk - 从备份恢复数据至UDisk
-    """
+    """RestoreUDisk - 从备份恢复数据至UDisk"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SnapshotId": fields.Str(required=False, dump_to="SnapshotId"),
         "SnapshotTime": fields.Int(required=False, dump_to="SnapshotTime"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class RestoreUDiskResponseSchema(schema.ResponseSchema):
-    """ RestoreUDisk - 从备份恢复数据至UDisk
-    """
+    """RestoreUDisk - 从备份恢复数据至UDisk"""
 
     fields = {}
 
 
 """
 API: SetUDiskUDataArkMode
 
 设置UDisk数据方舟的状态
 """
 
 
 class SetUDiskUDataArkModeRequestSchema(schema.RequestSchema):
-    """ SetUDiskUDataArkMode - 设置UDisk数据方舟的状态
-    """
+    """SetUDiskUDataArkMode - 设置UDisk数据方舟的状态"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UDataArkMode": fields.Str(required=True, dump_to="UDataArkMode"),
         "UDiskId": fields.Str(required=True, dump_to="UDiskId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class SetUDiskUDataArkModeResponseSchema(schema.ResponseSchema):
-    """ SetUDiskUDataArkMode - 设置UDisk数据方舟的状态
-    """
+    """SetUDiskUDataArkMode - 设置UDisk数据方舟的状态"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udisk/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udisk/schemas/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class UDiskDataSetSchema(schema.ResponseSchema):
-    """ UDiskDataSet - DescribeUDisk
-    """
+    """UDiskDataSet - DescribeUDisk"""
 
     fields = {
         "ArkSwitchEnable": fields.Int(
             required=False, load_from="ArkSwitchEnable"
         ),
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
         "CloneEnable": fields.Int(required=False, load_from="CloneEnable"),
@@ -38,28 +37,26 @@
         "UKmsMode": fields.Str(required=False, load_from="UKmsMode"),
         "Version": fields.Str(required=False, load_from="Version"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UDiskPriceDataSetSchema(schema.ResponseSchema):
-    """ UDiskPriceDataSet - DescribeUDiskPrice
-    """
+    """UDiskPriceDataSet - DescribeUDiskPrice"""
 
     fields = {
         "ChargeName": fields.Str(required=False, load_from="ChargeName"),
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
         "OriginalPrice": fields.Int(required=False, load_from="OriginalPrice"),
         "Price": fields.Int(required=False, load_from="Price"),
     }
 
 
 class UDiskSnapshotSetSchema(schema.ResponseSchema):
-    """ UDiskSnapshotSet - DescribeUDiskSnapshot
-    """
+    """UDiskSnapshotSet - DescribeUDiskSnapshot"""
 
     fields = {
         "CmkId": fields.Str(required=False, load_from="CmkId"),
         "CmkIdAlias": fields.Str(required=False, load_from="CmkIdAlias"),
         "CmkIdStatus": fields.Str(required=False, load_from="CmkIdStatus"),
         "Comment": fields.Str(required=False, load_from="Comment"),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udpn/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udpn/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,31 +12,31 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UDPNClient, self).__init__(config, transport, middleware, logger)
 
     def allocate_udpn(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ AllocateUDPN - 分配一条 UDPN 专线
+        """AllocateUDPN - 分配一条 UDPN 专线
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 带宽
         - **Peer1** (str) - (Required) 专线可用区1，支持地域：北京二：cn-bj2, 上海二：cn-sh2, 广东：cn-gd, 亚太： hk, 上海一：cn-sh1, 法兰克福：ge-fra, 新加坡：sg,  洛杉矶：us-la， 华盛顿：us-ws， 东京：jpn-tky
         - **Peer2** (str) - (Required) 专线可用区2，支持地域：北京二：cn-bj2, 上海二：cn-sh2, 广东：cn-gd, 亚太： hk, 上海一：cn-sh1, 法兰克福：ge-fra, 新加坡：sg,  洛杉矶：us-la， 华盛顿：us-ws， 东京：jpn-tky
         - **ChargeType** (str) - 计费类型，枚举值为： Year，按年付费； Month，按月付费； Dynamic，按需付费
         - **CouponId** (str) - 代金劵
         - **Quantity** (int) - 计费时长，默认 1
-        
+
         **Response**
 
         - **UDPNId** (str) - 资源名称
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.AllocateUDPNRequestSchema().dumps(d)
 
         # build options
@@ -44,33 +44,33 @@
 
         resp = self.invoke("AllocateUDPN", d, **kwargs)
         return apis.AllocateUDPNResponseSchema().loads(resp)
 
     def describe_udpn(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUDPN - 描述 UDPN
+        """DescribeUDPN - 描述 UDPN
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 返回数据长度，默认为 20
         - **Offset** (int) - 列表起始位置偏移量，默认为 0
         - **UDPNId** (str) - 申请到的 UDPN 资源 ID。若为空，则查询该用户在机房所有的专线信息。非默认项目资源，需填写ProjectId
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UDPNData** 模型定义
         - **TotalCount** (int) - 查询到的总数量
-        
+
         **Response Model**
-        
-        **UDPNData** 
-        
+
+        **UDPNData**
+
         - **Bandwidth** (int) - 带宽
         - **ChargeType** (str) - 计费类型
         - **CreateTime** (int) - unix 时间戳 创建时间
         - **ExpireTime** (int) - unix 时间戳 到期时间
         - **Peer1** (str) - 可用区域 1
         - **Peer2** (str) - 可用区域 2
         - **UDPNId** (str) - UDPN 资源短 ID
@@ -83,30 +83,30 @@
 
         resp = self.invoke("DescribeUDPN", d, **kwargs)
         return apis.DescribeUDPNResponseSchema().loads(resp)
 
     def get_udpn_line_list(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUDPNLineList - 获取当前支持的专线线路列表
+        """GetUDPNLineList - 获取当前支持的专线线路列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config)
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UDPNLineSet** 模型定义
         - **TotalCount** (int) - DataSet中的元素个数
-        
+
         **Response Model**
-        
-        **UDPNLineSet** 
-        
+
+        **UDPNLineSet**
+
         - **BandwidthUpperLimit** (int) - 线路带宽上限,单位 M
         - **LocalRegion** (str) - 支持UDPN的地域之一，北京二：cn-bj2, 上海二：cn-sh2, 广东：cn-gd, 亚太： hk, 上海一：cn-sh1, 法兰克福：ge-fra, 新加坡：sg, 华盛顿：us-ws, 洛杉矶：us-la， 东京：jpn-tky
         - **RemoteRegion** (str) - 支持UDPN的地域之一，北京二：cn-bj2, 上海二：cn-sh2, 广东：cn-gd, 亚太： hk, 上海一：cn-sh1, 法兰克福：ge-fra, 新加坡：sg, 华盛顿：us-ws, 洛杉矶：us-la， 东京：jpn-tky
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
@@ -115,101 +115,101 @@
 
         resp = self.invoke("GetUDPNLineList", d, **kwargs)
         return apis.GetUDPNLineListResponseSchema().loads(resp)
 
     def get_udpn_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUDPNPrice - 获取 UDPN 价格
+        """GetUDPNPrice - 获取 UDPN 价格
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 带宽信息
         - **Peer1** (str) - (Required) 专线可用区1，支持地域：北京二：cn-bj2, 上海二：cn-sh2, 广东：cn-gd, 亚太： hk, 上海一：cn-sh1, 法兰克福：ge-fra, 新加坡：sg, 洛杉矶：us-la， 华盛顿：us-ws， 东京：jpn-tky
         - **Peer2** (str) - (Required) 专线可用区2，支持地域：北京二：cn-bj2, 上海二：cn-sh2, 广东：cn-gd, 亚太： hk, 上海一：cn-sh1, 法兰克福：ge-fra, 新加坡：sg, 洛杉矶：us-la， 华盛顿：us-ws， 东京：jpn-tky
         - **ChargeType** (str) - 计费类型
         - **Quantity** (int) - 购买时长
-        
+
         **Response**
 
         - **Price** (float) - 专线价格
         - **PurchaseValue** (int) - 资源有效期 unix 时间戳
-        
+
         """
         # build request
         d = {"Region": self.config.region}
         req and d.update(req)
         d = apis.GetUDPNPriceRequestSchema().dumps(d)
 
         resp = self.invoke("GetUDPNPrice", d, **kwargs)
         return apis.GetUDPNPriceResponseSchema().loads(resp)
 
     def get_udpn_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUDPNUpgradePrice - 获取专线升级价格
+        """GetUDPNUpgradePrice - 获取专线升级价格
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 带宽
         - **UDPNId** (str) - (Required) 专线带宽资源 Id
-        
+
         **Response**
 
         - **Price** (float) - 升级后的价格
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.GetUDPNUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("GetUDPNUpgradePrice", d, **kwargs)
         return apis.GetUDPNUpgradePriceResponseSchema().loads(resp)
 
     def modify_udpn_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyUDPNBandwidth - 修改带宽值
+        """ModifyUDPNBandwidth - 修改带宽值
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 调整后专线带宽, 单位为Mbps，取值范围为大于等于2且小于等于1000([2-1000])的整数
         - **UDPNId** (str) - (Required) UDPN Id
         - **CouponId** (str) - 代金劵 ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyUDPNBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyUDPNBandwidth", d, **kwargs)
         return apis.ModifyUDPNBandwidthResponseSchema().loads(resp)
 
     def release_udpn(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ ReleaseUDPN - 释放 UDPN
+        """ReleaseUDPN - 释放 UDPN
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UDPNId** (str) - (Required) UDPN 资源 Id
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ReleaseUDPNRequestSchema().dumps(d)
 
         resp = self.invoke("ReleaseUDPN", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udpn/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udpn/schemas/apis.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,59 +12,55 @@
 API: AllocateUDPN
 
 分配一条 UDPN 专线
 """
 
 
 class AllocateUDPNRequestSchema(schema.RequestSchema):
-    """ AllocateUDPN - 分配一条 UDPN 专线
-    """
+    """AllocateUDPN - 分配一条 UDPN 专线"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Peer1": fields.Str(required=True, dump_to="Peer1"),
         "Peer2": fields.Str(required=True, dump_to="Peer2"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=False, dump_to="Region"),
     }
 
 
 class AllocateUDPNResponseSchema(schema.ResponseSchema):
-    """ AllocateUDPN - 分配一条 UDPN 专线
-    """
+    """AllocateUDPN - 分配一条 UDPN 专线"""
 
     fields = {"UDPNId": fields.Str(required=True, load_from="UDPNId")}
 
 
 """
 API: DescribeUDPN
 
 描述 UDPN
 """
 
 
 class DescribeUDPNRequestSchema(schema.RequestSchema):
-    """ DescribeUDPN - 描述 UDPN
-    """
+    """DescribeUDPN - 描述 UDPN"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "UDPNId": fields.Str(required=False, dump_to="UDPNId"),
     }
 
 
 class DescribeUDPNResponseSchema(schema.ResponseSchema):
-    """ DescribeUDPN - 描述 UDPN
-    """
+    """DescribeUDPN - 描述 UDPN"""
 
     fields = {
         "DataSet": fields.List(
             models.UDPNDataSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
@@ -74,26 +70,24 @@
 API: GetUDPNLineList
 
 获取当前支持的专线线路列表
 """
 
 
 class GetUDPNLineListRequestSchema(schema.RequestSchema):
-    """ GetUDPNLineList - 获取当前支持的专线线路列表
-    """
+    """GetUDPNLineList - 获取当前支持的专线线路列表"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
     }
 
 
 class GetUDPNLineListResponseSchema(schema.ResponseSchema):
-    """ GetUDPNLineList - 获取当前支持的专线线路列表
-    """
+    """GetUDPNLineList - 获取当前支持的专线线路列表"""
 
     fields = {
         "DataSet": fields.List(
             models.UDPNLineSetSchema(), required=True, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
@@ -103,30 +97,28 @@
 API: GetUDPNPrice
 
 获取 UDPN 价格
 """
 
 
 class GetUDPNPriceRequestSchema(schema.RequestSchema):
-    """ GetUDPNPrice - 获取 UDPN 价格
-    """
+    """GetUDPNPrice - 获取 UDPN 价格"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "Peer1": fields.Str(required=True, dump_to="Peer1"),
         "Peer2": fields.Str(required=True, dump_to="Peer2"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=False, dump_to="Region"),
     }
 
 
 class GetUDPNPriceResponseSchema(schema.ResponseSchema):
-    """ GetUDPNPrice - 获取 UDPN 价格
-    """
+    """GetUDPNPrice - 获取 UDPN 价格"""
 
     fields = {
         "Price": fields.Float(required=True, load_from="Price"),
         "PurchaseValue": fields.Int(required=True, load_from="PurchaseValue"),
     }
 
 
@@ -134,75 +126,69 @@
 API: GetUDPNUpgradePrice
 
 获取专线升级价格
 """
 
 
 class GetUDPNUpgradePriceRequestSchema(schema.RequestSchema):
-    """ GetUDPNUpgradePrice - 获取专线升级价格
-    """
+    """GetUDPNUpgradePrice - 获取专线升级价格"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "UDPNId": fields.Str(required=True, dump_to="UDPNId"),
     }
 
 
 class GetUDPNUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ GetUDPNUpgradePrice - 获取专线升级价格
-    """
+    """GetUDPNUpgradePrice - 获取专线升级价格"""
 
     fields = {"Price": fields.Float(required=True, load_from="Price")}
 
 
 """
 API: ModifyUDPNBandwidth
 
 修改带宽值
 """
 
 
 class ModifyUDPNBandwidthRequestSchema(schema.RequestSchema):
-    """ ModifyUDPNBandwidth - 修改带宽值
-    """
+    """ModifyUDPNBandwidth - 修改带宽值"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "UDPNId": fields.Str(required=True, dump_to="UDPNId"),
     }
 
 
 class ModifyUDPNBandwidthResponseSchema(schema.ResponseSchema):
-    """ ModifyUDPNBandwidth - 修改带宽值
-    """
+    """ModifyUDPNBandwidth - 修改带宽值"""
 
     fields = {}
 
 
 """
 API: ReleaseUDPN
 
 释放 UDPN
 """
 
 
 class ReleaseUDPNRequestSchema(schema.RequestSchema):
-    """ ReleaseUDPN - 释放 UDPN
-    """
+    """ReleaseUDPN - 释放 UDPN"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "UDPNId": fields.Str(required=True, dump_to="UDPNId"),
     }
 
 
 class ReleaseUDPNResponseSchema(schema.ResponseSchema):
-    """ ReleaseUDPN - 释放 UDPN
-    """
+    """ReleaseUDPN - 释放 UDPN"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/udpn/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/udpn/schemas/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class UDPNDataSchema(schema.ResponseSchema):
-    """ UDPNData - UDPN 详细信息
-    """
+    """UDPNData - UDPN 详细信息"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, load_from="Bandwidth"),
         "ChargeType": fields.Str(required=True, load_from="ChargeType"),
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "ExpireTime": fields.Int(required=True, load_from="ExpireTime"),
         "Peer1": fields.Str(required=True, load_from="Peer1"),
         "Peer2": fields.Str(required=True, load_from="Peer2"),
         "UDPNId": fields.Str(required=True, load_from="UDPNId"),
     }
 
 
 class UDPNLineSetSchema(schema.ResponseSchema):
-    """ UDPNLineSet - GetUDPNLineList
-    """
+    """UDPNLineSet - GetUDPNLineList"""
 
     fields = {
         "BandwidthUpperLimit": fields.Int(
             required=True, load_from="BandwidthUpperLimit"
         ),
         "LocalRegion": fields.Str(required=True, load_from="LocalRegion"),
         "RemoteRegion": fields.Str(required=True, load_from="RemoteRegion"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ufs/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ufs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,36 +12,36 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UFSClient, self).__init__(config, transport, middleware, logger)
 
     def create_ufs_volume(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUFSVolume - 创建文件系统
+        """CreateUFSVolume - 创建文件系统
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ProtocolType** (str) - (Required) 文件系统协议，枚举值，NFSv3表示NFS V3协议，NFSv4表示NFS V4协议
         - **Size** (int) - (Required) 文件系统大小，单位为GB，最大不超过20T，香港容量型必须为100的整数倍，Size最小为500GB，北京，上海，广州的容量型必须为1024的整数倍，Size最小为1024GB。性能型文件系统Size最小为100GB
         - **StorageType** (str) - (Required) 文件系统存储类型，枚举值，Basic表示容量型，Advanced表示性能型
         - **ChargeType** (str) - 计费模式，枚举值为： Year，按年付费； Month，按月付费； Dynamic，按需付费（需开启权限）； Trial，试用（需开启权限） 默认为Dynamic
         - **CouponId** (str) - 使用的代金券id
         - **Quantity** (int) - 购买时长 默认: 1
         - **Remark** (str) - 备注
         - **Tag** (str) - 文件系统所属业务组
         - **VolumeName** (str) - 文件系统名称
-        
+
         **Response**
 
         - **VolumeId** (str) - 文件系统ID
         - **VolumeName** (str) - 文件系统名称
         - **VolumeStatus** (str) - 文件系统挂载点状态
-        
+
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
             "Region": self.config.region,
         }
         req and d.update(req)
@@ -52,33 +52,33 @@
 
         resp = self.invoke("CreateUFSVolume", d, **kwargs)
         return apis.CreateUFSVolumeResponseSchema().loads(resp)
 
     def describe_ufs_volume_2(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUFSVolume2 - 获取文件系统列表
+        """DescribeUFSVolume2 - 获取文件系统列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 文件列表长度
         - **Offset** (int) - 文件列表起始
         - **VolumeId** (str) - 文件系统ID
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UFSVolumeInfo2** 模型定义
         - **TotalCount** (int) - 文件系统总数
-        
+
         **Response Model**
-        
-        **UFSVolumeInfo2** 
-        
+
+        **UFSVolumeInfo2**
+
         - **CreateTime** (int) - 文件系统创建时间（unix时间戳）
         - **ExpiredTime** (int) - 文件系统过期时间（unix时间戳）
         - **IsExpired** (str) - 是否过期
         - **MaxMountPointNum** (int) - 文件系统允许创建的最大挂载点数目
         - **ProtocolType** (str) - 文件系统协议，枚举值，NFSv3表示NFS V3协议，NFSv4表示NFS V4协议
         - **Remark** (str) - 文件系统备注信息
         - **Size** (int) - 文件系统大小，单位GB
@@ -100,26 +100,26 @@
 
         resp = self.invoke("DescribeUFSVolume2", d, **kwargs)
         return apis.DescribeUFSVolume2ResponseSchema().loads(resp)
 
     def extend_ufs_volume(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ExtendUFSVolume - 文件系统扩容
+        """ExtendUFSVolume - 文件系统扩容
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 文件系统大小，单位为GB，最大不超过20T，香港容量型必须为100的整数倍，Size最小为500GB，北京，上海，广州的容量型必须为1024的整数倍，Size最小为1024GB。性能型文件系统Size最小为100GB
         - **VolumeId** (str) - (Required) 文件系统ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
             "Region": self.config.region,
         }
         req and d.update(req)
@@ -127,25 +127,25 @@
 
         resp = self.invoke("ExtendUFSVolume", d, **kwargs)
         return apis.ExtendUFSVolumeResponseSchema().loads(resp)
 
     def remove_ufs_volume(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RemoveUFSVolume - 删除UFS文件系统
+        """RemoveUFSVolume - 删除UFS文件系统
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **VolumeId** (str) - (Required) 文件系统ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
             "Region": self.config.region,
         }
         req and d.update(req)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ufs/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ufs/schemas/apis.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: CreateUFSVolume
 
 创建文件系统
 """
 
 
 class CreateUFSVolumeRequestSchema(schema.RequestSchema):
-    """ CreateUFSVolume - 创建文件系统
-    """
+    """CreateUFSVolume - 创建文件系统"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "ProtocolType": fields.Str(required=True, dump_to="ProtocolType"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
@@ -31,16 +30,15 @@
         "StorageType": fields.Str(required=True, dump_to="StorageType"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VolumeName": fields.Str(required=False, dump_to="VolumeName"),
     }
 
 
 class CreateUFSVolumeResponseSchema(schema.ResponseSchema):
-    """ CreateUFSVolume - 创建文件系统
-    """
+    """CreateUFSVolume - 创建文件系统"""
 
     fields = {
         "VolumeId": fields.Str(required=True, load_from="VolumeId"),
         "VolumeName": fields.Str(required=True, load_from="VolumeName"),
         "VolumeStatus": fields.Str(required=True, load_from="VolumeStatus"),
     }
 
@@ -49,29 +47,27 @@
 API: DescribeUFSVolume2
 
 获取文件系统列表
 """
 
 
 class DescribeUFSVolume2RequestSchema(schema.RequestSchema):
-    """ DescribeUFSVolume2 - 获取文件系统列表
-    """
+    """DescribeUFSVolume2 - 获取文件系统列表"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VolumeId": fields.Str(required=False, dump_to="VolumeId"),
     }
 
 
 class DescribeUFSVolume2ResponseSchema(schema.ResponseSchema):
-    """ DescribeUFSVolume2 - 获取文件系统列表
-    """
+    """DescribeUFSVolume2 - 获取文件系统列表"""
 
     fields = {
         "DataSet": fields.List(
             models.UFSVolumeInfo2Schema(), required=True, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
@@ -81,48 +77,44 @@
 API: ExtendUFSVolume
 
 文件系统扩容
 """
 
 
 class ExtendUFSVolumeRequestSchema(schema.RequestSchema):
-    """ ExtendUFSVolume - 文件系统扩容
-    """
+    """ExtendUFSVolume - 文件系统扩容"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "VolumeId": fields.Str(required=True, dump_to="VolumeId"),
     }
 
 
 class ExtendUFSVolumeResponseSchema(schema.ResponseSchema):
-    """ ExtendUFSVolume - 文件系统扩容
-    """
+    """ExtendUFSVolume - 文件系统扩容"""
 
     fields = {}
 
 
 """
 API: RemoveUFSVolume
 
 删除UFS文件系统
 """
 
 
 class RemoveUFSVolumeRequestSchema(schema.RequestSchema):
-    """ RemoveUFSVolume - 删除UFS文件系统
-    """
+    """RemoveUFSVolume - 删除UFS文件系统"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VolumeId": fields.Str(required=True, dump_to="VolumeId"),
     }
 
 
 class RemoveUFSVolumeResponseSchema(schema.ResponseSchema):
-    """ RemoveUFSVolume - 删除UFS文件系统
-    """
+    """RemoveUFSVolume - 删除UFS文件系统"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ufs/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ufs/schemas/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class UFSVolumeInfo2Schema(schema.ResponseSchema):
-    """ UFSVolumeInfo2 - 文件系统信息
-    """
+    """UFSVolumeInfo2 - 文件系统信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "ExpiredTime": fields.Int(required=False, load_from="ExpiredTime"),
         "IsExpired": fields.Str(required=False, load_from="IsExpired"),
         "MaxMountPointNum": fields.Int(
             required=True, load_from="MaxMountPointNum"
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uhost/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uhost/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,31 +12,31 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UHostClient, self).__init__(config, transport, middleware, logger)
 
     def copy_custom_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CopyCustomImage - 复制自制镜像
+        """CopyCustomImage - 复制自制镜像
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SourceImageId** (str) - (Required) 源镜像Id, 参见 DescribeImage
         - **TargetProjectId** (str) - (Required) 目标项目Id, 参见 GetProjectList
         - **TargetImageDescription** (str) - 目标镜像描述
         - **TargetImageName** (str) - 目标镜像名称
         - **TargetRegion** (str) - 目标地域，不跨地域不用填
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **TargetImageId** (str) - 目标镜像Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CopyCustomImageRequestSchema().dumps(d)
 
         # build options
@@ -44,29 +44,29 @@
 
         resp = self.invoke("CopyCustomImage", d, **kwargs)
         return apis.CopyCustomImageResponseSchema().loads(resp)
 
     def create_custom_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateCustomImage - 从指定UHost实例，生成自定义镜像。
+        """CreateCustomImage - 从指定UHost实例，生成自定义镜像。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ImageName** (str) - (Required) 镜像名称
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **ImageDescription** (str) - 镜像描述
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **ImageId** (str) - 镜像Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateCustomImageRequestSchema().dumps(d)
 
         # build options
@@ -74,24 +74,24 @@
 
         resp = self.invoke("CreateCustomImage", d, **kwargs)
         return apis.CreateCustomImageResponseSchema().loads(resp)
 
     def create_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUHostInstance - 创建UHost实例。
+        """CreateUHostInstance - 创建UHost实例。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ImageId** (str) - (Required) 镜像ID。 请通过  `DescribeImage <https://docs.ucloud.cn/api/uhost-api/describe_image.html>`_ 获取
         - **LoginMode** (str) - (Required) 主机登陆模式。密码（默认选项）: Password。
         - **Password** (str) - (Required) UHost密码。请遵照 `字段规范 <https://docs.ucloud.cn/api/uhost-api/specification>`_ 设定密码。密码需使用base64进行编码，举例如下：# echo -n Password1 | base64UGFzc3dvcmQx。
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **AlarmTemplateId** (int) - 告警模板id，如果传了告警模板id，且告警模板id正确，则绑定告警模板。绑定告警模板失败只会在后台有日志，不会影响创建主机流程，也不会在前端报错。
         - **BootDiskSpace** (int) - 【待废弃，不建议调用】系统盘大小。 单位：GB， 范围[20,100]， 步长：10
         - **CPU** (int) - 虚拟CPU核数。可选参数：1-64（具体机型与CPU的对应关系参照控制台）。默认值: 4。
         - **ChargeType** (str) - 计费模式。枚举值为： \\ > Year，按年付费； \\ > Month，按月付费；\\ > Dynamic，按小时预付费 \\ > Postpay，按小时后付费（支持关机不收费，目前仅部分可用区支持，请联系您的客户经理） \\ 默认为月付
         - **CouponId** (str) - 主机代金券ID。请通过DescribeCoupon接口查询，或登录用户中心查看
         - **DiskPassword** (str) - 【待废弃，不建议调用】加密盘的密码。若输入此字段，自动选择加密盘。加密盘需要权限位。
         - **DiskSpace** (int) - 【待废弃，不建议调用】数据盘大小。 单位：GB， 范围[0,8000]， 步长：10， 默认值：20，云盘支持0-8000；本地普通盘支持0-2000；本地SSD盘（包括所有GPU机型）支持100-1000
@@ -122,54 +122,54 @@
         - **SubnetId** (str) - 子网 ID。默认为当前地域的默认子网。
         - **Tag** (str) - 业务组。默认：Default（Default即为未分组）。请遵照 `字段规范 <https://docs.ucloud.cn/api/uhost-api/specification>`_ 设定业务组。
         - **TimemachineFeature** (str) - 【待废弃，不建议调用】是否开启方舟特性。Yes为开启方舟，No为关闭方舟。目前仅选择普通本地盘+普通本地盘 或 SSD云盘+普通云盘的组合支持开启方舟。
         - **UHostType** (str) - 【建议后续不再使用】云主机机型（V1.0），在本字段和字段MachineType中，仅需要其中1个字段即可。参考 `云主机机型说明 <https://docs.ucloud.cn/api/uhost-api/uhost_type>`_ 。
         - **UserData** (str) - 【即将支持】用户自定义数据。当镜像支持Cloud-init Feature时可填写此字段。注意：1、总数据量大小不超多16K；2、使用base64编码
         - **UserDataScript** (str) - 【暂不支持】cloudinit方式下，用户初始化脚本
         - **VPCId** (str) - VPC ID。默认为当前地域的默认VPC。
-        
+
         **Response**
 
         - **IPs** (list) - 【批量创建不会返回】IP信息
         - **UHostIds** (list) - UHost实例Id集合
-        
+
         **Request Model**
-        
-        **CreateUHostInstanceParamNetworkInterfaceEIPGlobalSSH** 
-        
+
+        **CreateUHostInstanceParamNetworkInterfaceEIPGlobalSSH**
+
         - **Area** (str) - 填写支持SSH访问IP的地区名称，如“洛杉矶”，“新加坡”，“香港”，“东京”，“华盛顿”，“法兰克福”。Area和AreaCode两者必填其中之一。
         - **AreaCode** (str) - GlobalSSH的地区编码，格式为区域航空港国际通用代码。Area和AreaCode两者必填其中之一。
         - **Port** (int) - SSH端口，1-65535且不能使用80，443端口
 
-        **CreateUHostInstanceParamNetworkInterfaceEIP** 
-        
+        **CreateUHostInstanceParamNetworkInterfaceEIP**
+
         - **Bandwidth** (int) - 【若绑定EIP，此参数必填】弹性IP的外网带宽, 单位为Mbps. 共享带宽模式必须指定0M带宽, 非共享带宽模式必须指定非0Mbps带宽. 各地域非共享带宽的带宽范围如下： 流量计费[1-300]，带宽计费[1-800]
         - **CouponId** (str) - 当前EIP代金券id。请通过DescribeCoupon接口查询，或登录用户中心查看。
         - **GlobalSSH** (dict) - 见 **CreateUHostInstanceParamNetworkInterfaceEIPGlobalSSH** 模型定义
         - **OperatorName** (str) - 【若绑定EIP，此参数必填】弹性IP的线路。枚举值: 国际: International BGP: Bgp 各地域允许的线路参数如下: cn-sh1: Bgp cn-sh2: Bgp cn-gd: Bgp cn-bj1: Bgp cn-bj2: Bgp hk: International us-ca: International th-bkk: International kr-seoul:International us-ws:International ge-fra:International sg:International tw-kh:International.其他海外线路均为 International
         - **PayMode** (str) - 弹性IP的计费模式. 枚举值: "Traffic", 流量计费; "Bandwidth", 带宽计费; "ShareBandwidth",共享带宽模式. "Free":免费带宽模式.默认为 "Bandwidth".
         - **ShareBandwidthId** (str) - 绑定的共享带宽Id，仅当PayMode为ShareBandwidth时有效
 
-        **CreateUHostInstanceParamNetworkInterfaceIPv6** 
-        
+        **CreateUHostInstanceParamNetworkInterfaceIPv6**
+
         - **Adress** (str) - 第N个网卡对应的IPv6地址，默认不分配IPv6，“Auto”自动分配，不为空的其他字符串为实际要分配的IPv6地址
         - **ShareBandwidthId** (str) - 第N块网卡中IPv6对应的共享带宽id，默认不带外网
 
-        **CreateUHostInstanceParamDisks** 
-        
-        - **BackupType** (str) - 磁盘备份方案。枚举值：\\ > NONE，无备份 \\ > DATAARK，数据方舟 \\ 当前磁盘支持的备份模式参考  `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 
+        **CreateUHostInstanceParamDisks**
+
+        - **BackupType** (str) - 磁盘备份方案。枚举值：\\ > NONE，无备份 \\ > DATAARK，数据方舟 \\ 当前磁盘支持的备份模式参考  `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_
         - **CouponId** (str) - 云盘代金券id。不适用于系统盘/本地盘。请通过DescribeCoupon接口查询，或登录用户中心查看
         - **Encrypted** (bool) - 【功能仅部分可用区开放，详询技术支持】磁盘是否加密。加密：true, 不加密: false加密必须传入对应的的KmsKeyId
         - **IsBoot** (str) - 是否是系统盘。枚举值：\\ > True，是系统盘 \\ > False，是数据盘（默认）。Disks数组中有且只能有一块盘是系统盘。
         - **KmsKeyId** (str) - 【功能仅部分可用区开放，详询技术支持】kms key id。选择加密盘时必填。
         - **Size** (int) - 磁盘大小，单位GB，必须是10GB的整数倍。请参考 `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 。
         - **Type** (str) - 磁盘类型。请参考 `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 。
 
-        **CreateUHostInstanceParamNetworkInterface** 
-        
+        **CreateUHostInstanceParamNetworkInterface**
+
         - **EIP** (dict) - 见 **CreateUHostInstanceParamNetworkInterfaceEIP** 模型定义
         - **IPv6** (dict) - 见 **CreateUHostInstanceParamNetworkInterfaceIPv6** 模型定义
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
@@ -180,37 +180,37 @@
 
         resp = self.invoke("CreateUHostInstance", d, **kwargs)
         return apis.CreateUHostInstanceResponseSchema().loads(resp)
 
     def describe_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeImage - 获取指定数据中心镜像列表，用户可通过指定操作系统类型，镜像Id进行过滤。
+        """DescribeImage - 获取指定数据中心镜像列表，用户可通过指定操作系统类型，镜像Id进行过滤。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ImageId** (str) - 镜像Id
         - **ImageType** (str) - 镜像类型。标准镜像：Base，镜像市场：Business， 自定义镜像：Custom，默认返回所有类型
         - **Limit** (int) - 返回数据长度，默认为20
         - **Offset** (int) - 列表起始位置偏移量，默认为0
         - **OsType** (str) - 操作系统类型：Linux， Windows 默认返回所有类型
         - **PriceSet** (int) - 是否返回价格：1返回，0不返回；默认不返回
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **ImageSet** (list) - 见 **UHostImageSet** 模型定义
         - **TotalCount** (int) - 满足条件的镜像总数
-        
+
         **Response Model**
-        
-        **UHostImageSet** 
-        
+
+        **UHostImageSet**
+
         - **CreateTime** (int) - 创建时间，格式为Unix时间戳
         - **Features** (list) - 特殊状态标识， 目前包含NetEnhnced（网络增强1.0）, NetEnhanced_Ultra]（网络增强2.0）,HotPlug(热升级),CloudInit
         - **FuncType** (str) - 行业镜像类型（仅行业镜像将返回这个值）
         - **ImageDescription** (str) - 镜像描述
         - **ImageId** (str) - 镜像ID
         - **ImageName** (str) - 镜像名称
         - **ImageSize** (int) - 镜像大小
@@ -218,51 +218,51 @@
         - **IntegratedSoftware** (str) - 集成软件名称（仅行业镜像将返回这个值）
         - **Links** (str) - 介绍链接（仅行业镜像将返回这个值）
         - **MinimalCPU** (str) - 默认值为空'''。当CentOS 7.3/7.4/7.5等镜像会标记为“Broadwell”
         - **OsName** (str) - 操作系统名称
         - **OsType** (str) - 操作系统类型：Liunx，Windows
         - **State** (str) - 镜像状态， 可用：Available，制作中：Making， 不可用：Unavailable
         - **Vendor** (str) - 供应商（仅行业镜像将返回这个值）
-        - **Zone** (str) - 可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - 可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeImageRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeImage", d, **kwargs)
         return apis.DescribeImageResponseSchema().loads(resp)
 
     def describe_isolation_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeIsolationGroup - 查询硬件隔离组列表。
+        """DescribeIsolationGroup - 查询硬件隔离组列表。
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目id
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - 待查的硬件隔离组id
         - **Limit** (int) - 返回数据长度，默认为20，最大100
         - **Offset** (int) - 列表起始位置偏移量，默认为0
-        
+
         **Response**
 
         - **IsolationGroupSet** (list) - 见 **IsolationGroup** 模型定义
-        
+
         **Response Model**
-        
-        **SpreadInfo** 
-        
+
+        **SpreadInfo**
+
         - **UHostCount** (int) - 可用区中硬件隔离组中云主机的数量，不超过7。
         - **Zone** (str) - 可用区信息
 
-        **IsolationGroup** 
-        
+        **IsolationGroup**
+
         - **GroupId** (str) - 硬件隔离组id
         - **GroupName** (str) - 硬件隔离组名称
         - **Remark** (str) - 备注
         - **SpreadInfoSet** (list) - 见 **SpreadInfo** 模型定义
 
         """
         # build request
@@ -272,65 +272,65 @@
 
         resp = self.invoke("DescribeIsolationGroup", d, **kwargs)
         return apis.DescribeIsolationGroupResponseSchema().loads(resp)
 
     def describe_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUHostInstance - 获取主机或主机列表信息，并可根据数据中心，主机ID等参数进行过滤。
+        """DescribeUHostInstance - 获取主机或主机列表信息，并可根据数据中心，主机ID等参数进行过滤。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **IsolationGroup** (str) - 硬件隔离组id。通过硬件隔离组筛选主机。
         - **LifeCycle** (int) - 1：普通云主机；2：抢占型云主机；如不传此参数，默认全部获取
         - **Limit** (int) - 返回数据长度，默认为20，最大100
         - **Offset** (int) - 列表起始位置偏移量，默认为0
         - **SubnetId** (str) - 子网id。通过子网筛选主机。北京一地域无效。
         - **Tag** (str) - 要查询的业务组名称
         - **UHostIds** (list) - 【数组】UHost主机的资源ID，例如UHostIds.0代表希望获取信息 的主机1，UHostIds.1代表主机2。 如果不传入，则返回当前Region 所有符合条件的UHost实例。
         - **VPCId** (str) - vpc id。通过VPC筛选主机。北京一地域无效。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Action** (str) - 操作名称
         - **RetCode** (int) - 返回码
         - **TotalCount** (int) - UHostInstance总数
         - **UHostSet** (list) - 见 **UHostInstanceSet** 模型定义
-        
+
         **Response Model**
-        
-        **UHostDiskSet** 
-        
+
+        **UHostDiskSet**
+
         - **BackupType** (str) - 备份方案。若开通了数据方舟，则为DataArk
         - **DiskId** (str) - 磁盘ID
         - **DiskType** (str) - 磁盘类型。请参考 `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 。
         - **Drive** (str) - 磁盘盘符
         - **Encrypted** (bool) - true: 加密盘 false：非加密盘
         - **IsBoot** (str) - 是否是系统盘。枚举值：\\ > True，是系统盘 \\ > False，是数据盘（默认）。Disks数组中有且只能有一块盘是系统盘。
         - **Name** (str) - UDisk名字（仅当磁盘是UDisk时返回）
         - **Size** (int) - 磁盘大小，单位: GB
         - **Type** (str) - 【建议不再使用】磁盘类型。系统盘: Boot，数据盘: Data,网络盘：Udisk
 
-        **UHostIPSet** 
-        
+        **UHostIPSet**
+
         - **Bandwidth** (int) - IP对应的带宽, 单位: Mb  (内网IP不显示带宽信息)
         - **Default** (str) - 【暂未支持】是否为默认网卡。True: 是默认网卡；其他值：不是。
         - **IP** (str) - IP地址
         - **IPId** (str) - 外网IP资源ID 。(内网IP无对应的资源ID)
         - **Mac** (str) - 当前网卡的Mac。
         - **SubnetId** (str) - IP地址对应的子网 ID。（北京一不支持，字段返回为空）
         - **Type** (str) - 国际: Internation，BGP: Bgp，内网: Private
         - **VPCId** (str) - IP地址对应的VPC ID。（北京一不支持，字段返回为空）
         - **Weight** (int) - 当前EIP的权重。权重最大的为当前的出口IP。
 
-        **UHostInstanceSet** 
-        
+        **UHostInstanceSet**
+
         - **AutoRenew** (str) - 是否自动续费，自动续费：“Yes”，不自动续费：“No”
         - **BasicImageId** (str) - 基础镜像ID（指当前自定义镜像的来源镜像）
         - **BasicImageName** (str) - 基础镜像名称（指当前自定义镜像的来源镜像）
         - **BootDiskState** (str) - 系统盘状态 Normal表示初始化完成；Initializing表示在初始化。仍在初始化的系统盘无法制作镜像。
         - **CPU** (int) - 虚拟CPU核数，单位: 个
         - **ChargeType** (str) - 计费模式，枚举值为： Year，按年付费； Month，按月付费； Dynamic，按需付费（需开启权限）；
         - **CreateTime** (int) - 创建时间，格式为Unix时间戳
@@ -355,46 +355,46 @@
         - **StorageType** (str) - 【建议不再使用】主机磁盘类型。 枚举值为：\\ > LocalDisk，本地磁盘; \\ > UDisk 云盘。\\只要有一块磁盘为本地盘，即返回LocalDisk。
         - **SubnetType** (str) - 【建议不再使用】仅北京A的云主机会返回此字段。基础网络模式：Default；子网模式：Private
         - **Tag** (str) - 业务组名称
         - **TimemachineFeature** (str) - 【建议不再使用】数据方舟模式。枚举值：\\ > Yes: 开启方舟； \\ > no，未开启方舟
         - **TotalDiskSpace** (int) - 总的数据盘存储空间。
         - **UHostId** (str) - UHost实例ID
         - **UHostType** (str) - 【建议不再使用】云主机机型（旧）。参考 `云主机机型说明 <https://docs.ucloud.cn/api/uhost-api/uhost_type>`_ 。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUHostInstance", d, **kwargs)
         return apis.DescribeUHostInstanceResponseSchema().loads(resp)
 
     def describe_uhost_instance_snapshot(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUHostInstanceSnapshot - 获取已经存在的UHost实例的存储快照列表。
+        """DescribeUHostInstanceSnapshot - 获取已经存在的UHost实例的存储快照列表。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **SnapshotSet** (list) - 见 **UHostSnapshotSet** 模型定义
         - **UhostId** (str) - UHost实例ID
-        
+
         **Response Model**
-        
-        **UHostSnapshotSet** 
-        
+
+        **UHostSnapshotSet**
+
         - **SnapshotName** (str) - 快照名称
         - **SnapshotState** (str) - 快照状态, 制作中:Capturing 制作成功:Success 制作失败:Fail
         - **SnapshotTime** (str) - 快照制作时间
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
@@ -403,31 +403,31 @@
 
         resp = self.invoke("DescribeUHostInstanceSnapshot", d, **kwargs)
         return apis.DescribeUHostInstanceSnapshotResponseSchema().loads(resp)
 
     def describe_uhost_tags(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUHostTags - 获取指定数据中心的业务组列表。
+        """DescribeUHostTags - 获取指定数据中心的业务组列表。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **TagSet** (list) - 见 **UHostTagSet** 模型定义
         - **TotalCount** (int) - 已有主机的业务组总个数
-        
+
         **Response Model**
-        
-        **UHostTagSet** 
-        
+
+        **UHostTagSet**
+
         - **Tag** (str) - 业务组名称
         - **TotalCount** (int) - 该业务组中包含的主机个数
         - **Zone** (str) - 可用区
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
@@ -436,20 +436,20 @@
 
         resp = self.invoke("DescribeUHostTags", d, **kwargs)
         return apis.DescribeUHostTagsResponseSchema().loads(resp)
 
     def get_uhost_instance_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUHostInstancePrice - 根据UHost实例配置，获取UHost实例的价格。
+        """GetUHostInstancePrice - 根据UHost实例配置，获取UHost实例的价格。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **CPU** (int) - (Required) CPU核数。可选参数：1-64。可选范围参照控制台。默认值: 4
         - **Count** (int) - (Required) 购买台数，范围[1,5]
         - **ImageId** (str) - (Required) 镜像Id，可通过  `DescribeImage <https://docs.ucloud.cn/api/uhost-api/describe_image.html>`_  获取镜像ID
         - **Memory** (int) - (Required) 内存大小。单位：MB。范围 ：[1024, 262144]，取值为1024的倍数（可选范围参照好控制台）。默认值：8192
         - **ChargeType** (str) - 计费模式。枚举值为： \\ > Year，按年付费； \\ > Month，按月付费；\\ > Dynamic，按小时付费 \\ 默认为月付。
         - **DiskSpace** (int) - 【待废弃】数据盘大小，单位: GB，范围[0,1000]，步长: 10，默认值: 0
         - **Disks** (list) - 见 **GetUHostInstancePriceParamDisks** 模型定义
@@ -458,33 +458,33 @@
         - **LifeCycle** (int) - 【未支持】1：普通云主机；2：抢占性云主机；默认普通
         - **MachineType** (str) - 云主机机型（V2版本概念）。枚举值["N", "C", "G", "O"]。参考 `云主机机型说明 <https://docs.ucloud.cn/api/uhost-api/uhost_type>`_ 。
         - **NetCapability** (str) - 网络增强。枚举值：Normal，不开启; Super，开启网络增强1.0。 默认值为Normal。
         - **Quantity** (int) - 购买时长。默认: 1。按小时购买(Dynamic)时无需此参数。 月付时，此参数传0，代表了购买至月末。
         - **StorageType** (str) - 【待废弃】磁盘类型，同时设定系统盘和数据盘， 枚举值为：LocalDisk，本地磁盘; UDisk，云硬盘; 默认为LocalDisk 仅部分可用区支持云硬盘方式的主机存储方式，具体请查询控制台。
         - **TimemachineFeature** (str) - 【待废弃】方舟机型。No，Yes。默认是No。
         - **UHostType** (str) - 【待废弃】云主机机型（V1版本概念）。参考 `云主机机型说明 <https://docs.ucloud.cn/api/uhost-api/uhost_type>`_ 。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PriceSet** (list) - 见 **UHostPriceSet** 模型定义
-        
+
         **Request Model**
-        
-        **GetUHostInstancePriceParamDisks** 
-        
-        - **BackupType** (str) - 磁盘备份方案。枚举值：\\ > NONE，无备份 \\ > DATAARK，数据方舟 \\ 当前磁盘支持的备份模式参考  `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 
+
+        **GetUHostInstancePriceParamDisks**
+
+        - **BackupType** (str) - 磁盘备份方案。枚举值：\\ > NONE，无备份 \\ > DATAARK，数据方舟 \\ 当前磁盘支持的备份模式参考  `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_
         - **IsBoot** (str) - 是否是系统盘。枚举值：\\ > True，是系统盘 \\ > False，是数据盘（默认）。Disks数组中有且只能有一块盘是系统盘。
         - **Size** (int) - 磁盘大小，单位GB。请参考 `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 。
         - **Type** (str) - 磁盘类型。请参考 `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 。
 
         **Response Model**
-        
-        **UHostPriceSet** 
-        
+
+        **UHostPriceSet**
+
         - **ChargeType** (str) - 计费类型。Year，Month，Dynamic
         - **Price** (float) - 价格，单位: 元，保留小数点后两位有效数字
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
@@ -492,92 +492,92 @@
 
         resp = self.invoke("GetUHostInstancePrice", d, **kwargs)
         return apis.GetUHostInstancePriceResponseSchema().loads(resp)
 
     def get_uhost_instance_vnc_info(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUHostInstanceVncInfo - 获取指定UHost实例的管理VNC配置详细信息。
+        """GetUHostInstanceVncInfo - 获取指定UHost实例的管理VNC配置详细信息。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
         - **VncIP** (str) - Vnc登录IP
         - **VncPassword** (str) - Vnc 登录密码
         - **VncPort** (int) - Vnc登录端口
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.GetUHostInstanceVncInfoRequestSchema().dumps(d)
 
         resp = self.invoke("GetUHostInstanceVncInfo", d, **kwargs)
         return apis.GetUHostInstanceVncInfoResponseSchema().loads(resp)
 
     def get_uhost_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUHostUpgradePrice - 获取UHost实例升级配置的价格。可选配置范围请参考 `云主机机型说明 <https://docs.ucloud.cn/api/uhost-api/uhost_type>`_ 。
+        """GetUHostUpgradePrice - 获取UHost实例升级配置的价格。可选配置范围请参考 `云主机机型说明 <https://docs.ucloud.cn/api/uhost-api/uhost_type>`_ 。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UHostId** (str) - (Required) UHost实例ID。 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 。
         - **BootDiskSpace** (int) - 【待废弃】系统大小，单位: GB，范围[20,100]，步长: 10。
         - **CPU** (int) - 虚拟CPU核数。可选参数：1-64（可选范围参考控制台）。默认值为当前实例的CPU核数。
         - **DiskSpace** (int) - 【待废弃】数据盘大小，单位: GB，范围[0,1000]，步长: 10， 默认值是该主机当前数据盘大小。
         - **HostType** (str) - 【待废弃】主机系列，目前支持N1,N2
         - **Memory** (int) - 内存大小。单位：MB。范围 ：[1024, 262144]，取值为1024的倍数（可选范围参考控制台）。默认值为当前实例的内存大小。
         - **NetCapValue** (int) - 网卡升降级（1，表示升级，2表示降级，0表示不变）
         - **TimemachineFeature** (str) - 方舟机型。No，Yes。默认是No。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Price** (float) - 规格调整差价。精确到小数点后2位。
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.GetUHostUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("GetUHostUpgradePrice", d, **kwargs)
         return apis.GetUHostUpgradePriceResponseSchema().loads(resp)
 
     def import_custom_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ImportCustomImage - 把UFile的镜像文件导入到UHost，生成自定义镜像
+        """ImportCustomImage - 把UFile的镜像文件导入到UHost，生成自定义镜像
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Auth** (bool) - (Required) 是否授权。必须填true
         - **Format** (str) - (Required) 镜像格式，可选RAW、VHD、VMDK、qcow2
         - **ImageName** (str) - (Required) 镜像名称
         - **OsName** (str) - (Required) 操作系统详细版本，请参考控制台的镜像版本；OsType为Other时，输入参数为Other
         - **OsType** (str) - (Required) 操作系统平台，比如CentOS、Ubuntu、Windows、RedHat等，请参考控制台的镜像版本；若导入控制台上没有的操作系统，参数为Other
         - **UFileUrl** (str) - (Required) UFile私有空间地址
         - **ImageDescription** (str) - 镜像描述
-        
+
         **Response**
 
         - **ImageId** (str) - 镜像Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ImportCustomImageRequestSchema().dumps(d)
 
         # build options
@@ -585,374 +585,374 @@
 
         resp = self.invoke("ImportCustomImage", d, **kwargs)
         return apis.ImportCustomImageResponseSchema().loads(resp)
 
     def modify_uhost_instance_name(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyUHostInstanceName - 修改指定UHost实例名称，需要给出数据中心，UHostId，及新的实例名称。
+        """ModifyUHostInstanceName - 修改指定UHost实例名称，需要给出数据中心，UHostId，及新的实例名称。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **Name** (str) - UHost实例名称
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyUHostInstanceNameRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyUHostInstanceName", d, **kwargs)
         return apis.ModifyUHostInstanceNameResponseSchema().loads(resp)
 
     def modify_uhost_instance_remark(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyUHostInstanceRemark - 修改指定UHost实例备注信息。
+        """ModifyUHostInstanceRemark - 修改指定UHost实例备注信息。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **Remark** (str) - 备注
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyUHostInstanceRemarkRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyUHostInstanceRemark", d, **kwargs)
         return apis.ModifyUHostInstanceRemarkResponseSchema().loads(resp)
 
     def modify_uhost_instance_tag(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyUHostInstanceTag - 修改指定UHost实例业务组标识。
+        """ModifyUHostInstanceTag - 修改指定UHost实例业务组标识。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **Tag** (str) - 业务组名称
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyUHostInstanceTagRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyUHostInstanceTag", d, **kwargs)
         return apis.ModifyUHostInstanceTagResponseSchema().loads(resp)
 
     def poweroff_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ PoweroffUHostInstance - 直接关闭UHost实例电源，无需等待实例正常关闭。
+        """PoweroffUHostInstance - 直接关闭UHost实例电源，无需等待实例正常关闭。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.PoweroffUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("PoweroffUHostInstance", d, **kwargs)
         return apis.PoweroffUHostInstanceResponseSchema().loads(resp)
 
     def reboot_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RebootUHostInstance - 重新启动UHost实例，需要指定数据中心及UHostID两个参数的值。
+        """RebootUHostInstance - 重新启动UHost实例，需要指定数据中心及UHostID两个参数的值。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **DiskPassword** (str) - 加密盘密码
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.RebootUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("RebootUHostInstance", d, **kwargs)
         return apis.RebootUHostInstanceResponseSchema().loads(resp)
 
     def reinstall_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ReinstallUHostInstance - 重新安装指定UHost实例的操作系统
+        """ReinstallUHostInstance - 重新安装指定UHost实例的操作系统
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例资源ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例资源ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **DNSServers** (list) - 针对非私有子网主机，可自定义DNS。n可为0-2
-        - **ImageId** (str) - 镜像Id，默认使用原镜像 参见  `DescribeImage <https://docs.ucloud.cn/api/uhost-api/describe_image.html>`_ 
+        - **ImageId** (str) - 镜像Id，默认使用原镜像 参见  `DescribeImage <https://docs.ucloud.cn/api/uhost-api/describe_image.html>`_
         - **Password** (str) - 如果创建UHost实例时LoginMode为Password，则必须填写，如果LoginMode为KeyPair，不需要填写 （密码格式使用BASE64编码；LoginMode不可变更）
         - **ReserveDisk** (str) - 是否保留数据盘，保留：Yes，不报留：No， 默认：Yes
         - **ResourceType** (int) - 云灾备指明191
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ReinstallUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("ReinstallUHostInstance", d, **kwargs)
         return apis.ReinstallUHostInstanceResponseSchema().loads(resp)
 
     def reset_uhost_instance_password(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResetUHostInstancePassword - 重置UHost实例的管理员密码。
+        """ResetUHostInstancePassword - 重置UHost实例的管理员密码。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Password** (str) - (Required) UHost新密码（密码格式使用BASE64编码）
         - **UHostId** (str) - (Required) UHost实例ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ResetUHostInstancePasswordRequestSchema().dumps(d)
 
         resp = self.invoke("ResetUHostInstancePassword", d, **kwargs)
         return apis.ResetUHostInstancePasswordResponseSchema().loads(resp)
 
     def resize_attached_disk(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeAttachedDisk - 修改挂载的磁盘大小，包含系统盘和数据盘
+        """ResizeAttachedDisk - 修改挂载的磁盘大小，包含系统盘和数据盘
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DiskId** (str) - (Required) 磁盘ID。参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 返回值中的DiskSet。
         - **DiskSpace** (int) - (Required) 磁盘大小，单位GB，步长为10。取值范围需大于当前磁盘大小，最大值请参考 `磁盘类型 <https://docs.ucloud.cn/api/uhost-api/disk_type>`_ 。
         - **UHostId** (str) - (Required) UHost实例ID。 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 。
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DiskId** (str) - 改配成功的磁盘id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ResizeAttachedDiskRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeAttachedDisk", d, **kwargs)
         return apis.ResizeAttachedDiskResponseSchema().loads(resp)
 
     def resize_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeUHostInstance - 修改指定UHost实例的资源配置，如CPU核心数，内存容量大小，磁盘空间大小,网络增强等。
+        """ResizeUHostInstance - 修改指定UHost实例的资源配置，如CPU核心数，内存容量大小，磁盘空间大小,网络增强等。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **BootDiskSpace** (int) - 系统盘大小，单位：GB，范围[20,100]，步长：10，系统盘不支持缩容，因此不允许输入比当前实例系统盘小的值
         - **CPU** (int) - 虚拟CPU核数，单位：个，范围：[1,16]，最小值为1，其他值是2的倍数，默认值为当前实例的CPU核数（*windows CPU>=2）
         - **DiskSpace** (int) - 数据盘大小，单位：GB，范围[10,1000]； SSD机型，单位：GB，范围[100,500]；步长：10，默认值为当前实例的数据盘大小，数据盘不支持缩容，因此不允许输入比当前实例数据盘大小的值
         - **Memory** (int) - 内存大小，单位：MB，范围[2048,65536]，步长：2048，默认值为当前实例的内存大小（BGP-C数据中心最小支持1024，限Linux系统）
         - **NetCapValue** (int) - 网卡升降级（1，表示升级，2表示降级，0表示不变）
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ResizeUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeUHostInstance", d, **kwargs)
         return apis.ResizeUHostInstanceResponseSchema().loads(resp)
 
     def start_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ StartUHostInstance - 启动处于关闭状态的UHost实例，需要指定数据中心及UHostID两个参数的值。
+        """StartUHostInstance - 启动处于关闭状态的UHost实例，需要指定数据中心及UHostID两个参数的值。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **DiskPassword** (str) - 加密盘密码
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.StartUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("StartUHostInstance", d, **kwargs)
         return apis.StartUHostInstanceResponseSchema().loads(resp)
 
     def stop_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ StopUHostInstance - 指停止处于运行状态的UHost实例，需指定数据中心及UhostID。
+        """StopUHostInstance - 指停止处于运行状态的UHost实例，需指定数据中心及UhostID。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost实例ID 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **UhostId** (str) - UHost实例ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.StopUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("StopUHostInstance", d, **kwargs)
         return apis.StopUHostInstanceResponseSchema().loads(resp)
 
     def terminate_custom_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ TerminateCustomImage - 删除用户自定义镜像
+        """TerminateCustomImage - 删除用户自定义镜像
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **ImageId** (str) - (Required) 自制镜像ID 参见  `DescribeImage <https://docs.ucloud.cn/api/uhost-api/describe_image.html>`_ 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **ImageId** (str) - (Required) 自制镜像ID 参见  `DescribeImage <https://docs.ucloud.cn/api/uhost-api/describe_image.html>`_
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **ImageId** (str) - 自制镜像Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.TerminateCustomImageRequestSchema().dumps(d)
 
         resp = self.invoke("TerminateCustomImage", d, **kwargs)
         return apis.TerminateCustomImageResponseSchema().loads(resp)
 
     def terminate_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ TerminateUHostInstance - 删除指定数据中心的UHost实例。
+        """TerminateUHostInstance - 删除指定数据中心的UHost实例。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **UHostId** (str) - (Required) UHost资源Id 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **UHostId** (str) - (Required) UHost资源Id 参见  `DescribeUHostInstance <https://docs.ucloud.cn/api/uhost-api/describe_uhost_instance.html>`_
         - **Destroy** (int) - 是否直接删除，0表示按照原来的逻辑（有回收站权限，则进入回收站），1表示直接删除
         - **ReleaseEIP** (bool) - 是否释放绑定的EIP。true: 解绑EIP后，并释放；其他值或不填：解绑EIP。
         - **ReleaseUDisk** (bool) - 是否删除挂载的数据盘。true删除，其他不删除。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **InRecycle** (str) - 放入回收站:"Yes", 彻底删除：“No”
         - **UHostId** (str) - UHost 实例 Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.TerminateUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("TerminateUHostInstance", d, **kwargs)
         return apis.TerminateUHostInstanceResponseSchema().loads(resp)
 
     def upgrade_to_ark_uhost_instance(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpgradeToArkUHostInstance - 普通升级为方舟机型
+        """UpgradeToArkUHostInstance - 普通升级为方舟机型
 
         **Request**
 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **UHostIds** (list) - (Required) UHost主机的资源ID，例如UHostIds.0代表希望升级的主机1，UHostIds.1代表主机2。
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **CouponId** (str) - 代金券ID 请参考DescribeCoupon接口
-        
+
         **Response**
 
         - **UHostSet** (list) - UHost主机的资源ID数组
-        
+
         """
         # build request
         d = {"Region": self.config.region}
         req and d.update(req)
         d = apis.UpgradeToArkUHostInstanceRequestSchema().dumps(d)
 
         resp = self.invoke("UpgradeToArkUHostInstance", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uhost/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uhost/schemas/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: CopyCustomImage
 
 复制自制镜像
 """
 
 
 class CopyCustomImageRequestSchema(schema.RequestSchema):
-    """ CopyCustomImage - 复制自制镜像
-    """
+    """CopyCustomImage - 复制自制镜像"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SourceImageId": fields.Str(required=True, dump_to="SourceImageId"),
         "TargetImageDescription": fields.Str(
             required=False, dump_to="TargetImageDescription"
@@ -32,87 +31,81 @@
         "TargetProjectId": fields.Str(required=True, dump_to="TargetProjectId"),
         "TargetRegion": fields.Str(required=False, dump_to="TargetRegion"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CopyCustomImageResponseSchema(schema.ResponseSchema):
-    """ CopyCustomImage - 复制自制镜像
-    """
+    """CopyCustomImage - 复制自制镜像"""
 
     fields = {
         "TargetImageId": fields.Str(required=False, load_from="TargetImageId")
     }
 
 
 """
 API: CreateCustomImage
 
 从指定UHost实例，生成自定义镜像。
 """
 
 
 class CreateCustomImageRequestSchema(schema.RequestSchema):
-    """ CreateCustomImage - 从指定UHost实例，生成自定义镜像。
-    """
+    """CreateCustomImage - 从指定UHost实例，生成自定义镜像。"""
 
     fields = {
         "ImageDescription": fields.Str(
             required=False, dump_to="ImageDescription"
         ),
         "ImageName": fields.Str(required=True, dump_to="ImageName"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CreateCustomImageResponseSchema(schema.ResponseSchema):
-    """ CreateCustomImage - 从指定UHost实例，生成自定义镜像。
-    """
+    """CreateCustomImage - 从指定UHost实例，生成自定义镜像。"""
 
     fields = {"ImageId": fields.Str(required=False, load_from="ImageId")}
 
 
 """
 API: CreateUHostInstance
 
 创建UHost实例。
 """
 
 
 class CreateUHostInstanceParamNetworkInterfaceEIPGlobalSSHSchema(
     schema.RequestSchema
 ):
-    """ CreateUHostInstanceParamNetworkInterfaceEIPGlobalSSH - 
-    """
+    """CreateUHostInstanceParamNetworkInterfaceEIPGlobalSSH -"""
 
     fields = {
         "Area": fields.Str(required=False, dump_to="Area"),
         "AreaCode": fields.Str(required=False, dump_to="AreaCode"),
         "Port": fields.Int(required=False, dump_to="Port"),
     }
 
 
 class CreateUHostInstanceParamNetworkInterfaceIPv6Schema(schema.RequestSchema):
-    """ CreateUHostInstanceParamNetworkInterfaceIPv6 - 
-    """
+    """CreateUHostInstanceParamNetworkInterfaceIPv6 -"""
 
     fields = {
         "Adress": fields.Str(required=False, dump_to="Adress"),
         "ShareBandwidthId": fields.Str(
             required=False, dump_to="ShareBandwidthId"
         ),
     }
 
 
 class CreateUHostInstanceParamNetworkInterfaceEIPSchema(schema.RequestSchema):
-    """ CreateUHostInstanceParamNetworkInterfaceEIP - 
-    """
+    """CreateUHostInstanceParamNetworkInterfaceEIP -"""
 
     fields = {
         "Bandwidth": fields.Int(required=False, dump_to="Bandwidth"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "GlobalSSH": CreateUHostInstanceParamNetworkInterfaceEIPGlobalSSHSchema(
             required=False, dump_to="GlobalSSH"
         ),
@@ -121,45 +114,42 @@
         "ShareBandwidthId": fields.Str(
             required=False, dump_to="ShareBandwidthId"
         ),
     }
 
 
 class CreateUHostInstanceParamNetworkInterfaceSchema(schema.RequestSchema):
-    """ CreateUHostInstanceParamNetworkInterface - 
-    """
+    """CreateUHostInstanceParamNetworkInterface -"""
 
     fields = {
         "EIP": CreateUHostInstanceParamNetworkInterfaceEIPSchema(
             required=False, dump_to="EIP"
         ),
         "IPv6": CreateUHostInstanceParamNetworkInterfaceIPv6Schema(
             required=False, dump_to="IPv6"
         ),
     }
 
 
 class CreateUHostInstanceParamDisksSchema(schema.RequestSchema):
-    """ CreateUHostInstanceParamDisks - 
-    """
+    """CreateUHostInstanceParamDisks -"""
 
     fields = {
         "BackupType": fields.Str(required=False, dump_to="BackupType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Encrypted": fields.Bool(required=False, dump_to="Encrypted"),
         "IsBoot": fields.Str(required=True, dump_to="IsBoot"),
         "KmsKeyId": fields.Str(required=False, dump_to="KmsKeyId"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "Type": fields.Str(required=True, dump_to="Type"),
     }
 
 
 class CreateUHostInstanceRequestSchema(schema.RequestSchema):
-    """ CreateUHostInstance - 创建UHost实例。
-    """
+    """CreateUHostInstance - 创建UHost实例。"""
 
     fields = {
         "AlarmTemplateId": fields.Int(
             required=False, dump_to="AlarmTemplateId"
         ),
         "BootDiskSpace": fields.Int(required=False, dump_to="BootDiskSpace"),
         "CPU": fields.Int(required=False, dump_to="CPU"),
@@ -212,16 +202,15 @@
         "UserDataScript": fields.Str(required=False, dump_to="UserDataScript"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ CreateUHostInstance - 创建UHost实例。
-    """
+    """CreateUHostInstance - 创建UHost实例。"""
 
     fields = {
         "IPs": fields.List(fields.Str(), required=False, load_from="IPs"),
         "UHostIds": fields.List(
             fields.Str(), required=False, load_from="UHostIds"
         ),
     }
@@ -231,16 +220,15 @@
 API: DescribeImage
 
 获取指定数据中心镜像列表，用户可通过指定操作系统类型，镜像Id进行过滤。
 """
 
 
 class DescribeImageRequestSchema(schema.RequestSchema):
-    """ DescribeImage - 获取指定数据中心镜像列表，用户可通过指定操作系统类型，镜像Id进行过滤。
-    """
+    """DescribeImage - 获取指定数据中心镜像列表，用户可通过指定操作系统类型，镜像Id进行过滤。"""
 
     fields = {
         "ImageId": fields.Str(required=False, dump_to="ImageId"),
         "ImageType": fields.Str(required=False, dump_to="ImageType"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "OsType": fields.Str(required=False, dump_to="OsType"),
@@ -248,16 +236,15 @@
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeImageResponseSchema(schema.ResponseSchema):
-    """ DescribeImage - 获取指定数据中心镜像列表，用户可通过指定操作系统类型，镜像Id进行过滤。
-    """
+    """DescribeImage - 获取指定数据中心镜像列表，用户可通过指定操作系统类型，镜像Id进行过滤。"""
 
     fields = {
         "ImageSet": fields.List(
             models.UHostImageSetSchema(), required=False, load_from="ImageSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -267,29 +254,27 @@
 API: DescribeIsolationGroup
 
 查询硬件隔离组列表。
 """
 
 
 class DescribeIsolationGroupRequestSchema(schema.RequestSchema):
-    """ DescribeIsolationGroup - 查询硬件隔离组列表。
-    """
+    """DescribeIsolationGroup - 查询硬件隔离组列表。"""
 
     fields = {
         "GroupId": fields.Str(required=False, dump_to="GroupId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DescribeIsolationGroupResponseSchema(schema.ResponseSchema):
-    """ DescribeIsolationGroup - 查询硬件隔离组列表。
-    """
+    """DescribeIsolationGroup - 查询硬件隔离组列表。"""
 
     fields = {
         "IsolationGroupSet": fields.List(
             models.IsolationGroupSchema(),
             required=False,
             load_from="IsolationGroupSet",
         )
@@ -300,16 +285,15 @@
 API: DescribeUHostInstance
 
 获取主机或主机列表信息，并可根据数据中心，主机ID等参数进行过滤。
 """
 
 
 class DescribeUHostInstanceRequestSchema(schema.RequestSchema):
-    """ DescribeUHostInstance - 获取主机或主机列表信息，并可根据数据中心，主机ID等参数进行过滤。
-    """
+    """DescribeUHostInstance - 获取主机或主机列表信息，并可根据数据中心，主机ID等参数进行过滤。"""
 
     fields = {
         "IsolationGroup": fields.Str(required=False, dump_to="IsolationGroup"),
         "LifeCycle": fields.Int(required=False, dump_to="LifeCycle"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -319,16 +303,15 @@
         "UHostIds": fields.List(fields.Str()),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ DescribeUHostInstance - 获取主机或主机列表信息，并可根据数据中心，主机ID等参数进行过滤。
-    """
+    """DescribeUHostInstance - 获取主机或主机列表信息，并可根据数据中心，主机ID等参数进行过滤。"""
 
     fields = {
         "Action": fields.Str(required=True, load_from="Action"),
         "RetCode": fields.Int(required=True, load_from="RetCode"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
         "UHostSet": fields.List(
             models.UHostInstanceSetSchema(),
@@ -342,28 +325,26 @@
 API: DescribeUHostInstanceSnapshot
 
 获取已经存在的UHost实例的存储快照列表。
 """
 
 
 class DescribeUHostInstanceSnapshotRequestSchema(schema.RequestSchema):
-    """ DescribeUHostInstanceSnapshot - 获取已经存在的UHost实例的存储快照列表。
-    """
+    """DescribeUHostInstanceSnapshot - 获取已经存在的UHost实例的存储快照列表。"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUHostInstanceSnapshotResponseSchema(schema.ResponseSchema):
-    """ DescribeUHostInstanceSnapshot - 获取已经存在的UHost实例的存储快照列表。
-    """
+    """DescribeUHostInstanceSnapshot - 获取已经存在的UHost实例的存储快照列表。"""
 
     fields = {
         "SnapshotSet": fields.List(
             models.UHostSnapshotSetSchema(),
             required=False,
             load_from="SnapshotSet",
         ),
@@ -375,27 +356,25 @@
 API: DescribeUHostTags
 
 获取指定数据中心的业务组列表。
 """
 
 
 class DescribeUHostTagsRequestSchema(schema.RequestSchema):
-    """ DescribeUHostTags - 获取指定数据中心的业务组列表。
-    """
+    """DescribeUHostTags - 获取指定数据中心的业务组列表。"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUHostTagsResponseSchema(schema.ResponseSchema):
-    """ DescribeUHostTags - 获取指定数据中心的业务组列表。
-    """
+    """DescribeUHostTags - 获取指定数据中心的业务组列表。"""
 
     fields = {
         "TagSet": fields.List(
             models.UHostTagSetSchema(), required=False, load_from="TagSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -405,28 +384,26 @@
 API: GetUHostInstancePrice
 
 根据UHost实例配置，获取UHost实例的价格。
 """
 
 
 class GetUHostInstancePriceParamDisksSchema(schema.RequestSchema):
-    """ GetUHostInstancePriceParamDisks - 
-    """
+    """GetUHostInstancePriceParamDisks -"""
 
     fields = {
         "BackupType": fields.Str(required=False, dump_to="BackupType"),
         "IsBoot": fields.Str(required=True, dump_to="IsBoot"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "Type": fields.Str(required=True, dump_to="Type"),
     }
 
 
 class GetUHostInstancePriceRequestSchema(schema.RequestSchema):
-    """ GetUHostInstancePrice - 根据UHost实例配置，获取UHost实例的价格。
-    """
+    """GetUHostInstancePrice - 根据UHost实例配置，获取UHost实例的价格。"""
 
     fields = {
         "CPU": fields.Int(required=True, dump_to="CPU"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "Count": fields.Int(required=True, dump_to="Count"),
         "DiskSpace": fields.Int(required=False, dump_to="DiskSpace"),
         "Disks": fields.List(GetUHostInstancePriceParamDisksSchema()),
@@ -446,16 +423,15 @@
         ),
         "UHostType": fields.Str(required=False, dump_to="UHostType"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class GetUHostInstancePriceResponseSchema(schema.ResponseSchema):
-    """ GetUHostInstancePrice - 根据UHost实例配置，获取UHost实例的价格。
-    """
+    """GetUHostInstancePrice - 根据UHost实例配置，获取UHost实例的价格。"""
 
     fields = {
         "PriceSet": fields.List(
             models.UHostPriceSetSchema(), required=False, load_from="PriceSet"
         )
     }
 
@@ -464,28 +440,26 @@
 API: GetUHostInstanceVncInfo
 
 获取指定UHost实例的管理VNC配置详细信息。
 """
 
 
 class GetUHostInstanceVncInfoRequestSchema(schema.RequestSchema):
-    """ GetUHostInstanceVncInfo - 获取指定UHost实例的管理VNC配置详细信息。
-    """
+    """GetUHostInstanceVncInfo - 获取指定UHost实例的管理VNC配置详细信息。"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class GetUHostInstanceVncInfoResponseSchema(schema.ResponseSchema):
-    """ GetUHostInstanceVncInfo - 获取指定UHost实例的管理VNC配置详细信息。
-    """
+    """GetUHostInstanceVncInfo - 获取指定UHost实例的管理VNC配置详细信息。"""
 
     fields = {
         "UhostId": fields.Str(required=False, load_from="UhostId"),
         "VncIP": fields.Str(required=False, load_from="VncIP"),
         "VncPassword": fields.Str(required=False, load_from="VncPassword"),
         "VncPort": fields.Int(required=False, load_from="VncPort"),
     }
@@ -495,16 +469,15 @@
 API: GetUHostUpgradePrice
 
 获取UHost实例升级配置的价格。可选配置范围请参考[[api:uhost-api:uhost_type|云主机机型说明]]。
 """
 
 
 class GetUHostUpgradePriceRequestSchema(schema.RequestSchema):
-    """ GetUHostUpgradePrice - 获取UHost实例升级配置的价格。可选配置范围请参考[[api:uhost-api:uhost_type|云主机机型说明]]。
-    """
+    """GetUHostUpgradePrice - 获取UHost实例升级配置的价格。可选配置范围请参考[[api:uhost-api:uhost_type|云主机机型说明]]。"""
 
     fields = {
         "BootDiskSpace": fields.Int(required=False, dump_to="BootDiskSpace"),
         "CPU": fields.Int(required=False, dump_to="CPU"),
         "DiskSpace": fields.Int(required=False, dump_to="DiskSpace"),
         "HostType": fields.Str(required=False, dump_to="HostType"),
         "Memory": fields.Int(required=False, dump_to="Memory"),
@@ -516,30 +489,28 @@
         ),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class GetUHostUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ GetUHostUpgradePrice - 获取UHost实例升级配置的价格。可选配置范围请参考[[api:uhost-api:uhost_type|云主机机型说明]]。
-    """
+    """GetUHostUpgradePrice - 获取UHost实例升级配置的价格。可选配置范围请参考[[api:uhost-api:uhost_type|云主机机型说明]]。"""
 
     fields = {"Price": fields.Float(required=False, load_from="Price")}
 
 
 """
 API: ImportCustomImage
 
 把UFile的镜像文件导入到UHost，生成自定义镜像
 """
 
 
 class ImportCustomImageRequestSchema(schema.RequestSchema):
-    """ ImportCustomImage - 把UFile的镜像文件导入到UHost，生成自定义镜像
-    """
+    """ImportCustomImage - 把UFile的镜像文件导入到UHost，生成自定义镜像"""
 
     fields = {
         "Auth": fields.Bool(required=True, dump_to="Auth"),
         "Format": fields.Str(required=True, dump_to="Format"),
         "ImageDescription": fields.Str(
             required=False, dump_to="ImageDescription"
         ),
@@ -549,164 +520,152 @@
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UFileUrl": fields.Str(required=True, dump_to="UFileUrl"),
     }
 
 
 class ImportCustomImageResponseSchema(schema.ResponseSchema):
-    """ ImportCustomImage - 把UFile的镜像文件导入到UHost，生成自定义镜像
-    """
+    """ImportCustomImage - 把UFile的镜像文件导入到UHost，生成自定义镜像"""
 
     fields = {"ImageId": fields.Str(required=False, load_from="ImageId")}
 
 
 """
 API: ModifyUHostInstanceName
 
 修改指定UHost实例名称，需要给出数据中心，UHostId，及新的实例名称。
 """
 
 
 class ModifyUHostInstanceNameRequestSchema(schema.RequestSchema):
-    """ ModifyUHostInstanceName - 修改指定UHost实例名称，需要给出数据中心，UHostId，及新的实例名称。
-    """
+    """ModifyUHostInstanceName - 修改指定UHost实例名称，需要给出数据中心，UHostId，及新的实例名称。"""
 
     fields = {
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyUHostInstanceNameResponseSchema(schema.ResponseSchema):
-    """ ModifyUHostInstanceName - 修改指定UHost实例名称，需要给出数据中心，UHostId，及新的实例名称。
-    """
+    """ModifyUHostInstanceName - 修改指定UHost实例名称，需要给出数据中心，UHostId，及新的实例名称。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: ModifyUHostInstanceRemark
 
 修改指定UHost实例备注信息。
 """
 
 
 class ModifyUHostInstanceRemarkRequestSchema(schema.RequestSchema):
-    """ ModifyUHostInstanceRemark - 修改指定UHost实例备注信息。
-    """
+    """ModifyUHostInstanceRemark - 修改指定UHost实例备注信息。"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyUHostInstanceRemarkResponseSchema(schema.ResponseSchema):
-    """ ModifyUHostInstanceRemark - 修改指定UHost实例备注信息。
-    """
+    """ModifyUHostInstanceRemark - 修改指定UHost实例备注信息。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: ModifyUHostInstanceTag
 
 修改指定UHost实例业务组标识。
 """
 
 
 class ModifyUHostInstanceTagRequestSchema(schema.RequestSchema):
-    """ ModifyUHostInstanceTag - 修改指定UHost实例业务组标识。
-    """
+    """ModifyUHostInstanceTag - 修改指定UHost实例业务组标识。"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyUHostInstanceTagResponseSchema(schema.ResponseSchema):
-    """ ModifyUHostInstanceTag - 修改指定UHost实例业务组标识。
-    """
+    """ModifyUHostInstanceTag - 修改指定UHost实例业务组标识。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: PoweroffUHostInstance
 
 直接关闭UHost实例电源，无需等待实例正常关闭。
 """
 
 
 class PoweroffUHostInstanceRequestSchema(schema.RequestSchema):
-    """ PoweroffUHostInstance - 直接关闭UHost实例电源，无需等待实例正常关闭。
-    """
+    """PoweroffUHostInstance - 直接关闭UHost实例电源，无需等待实例正常关闭。"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class PoweroffUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ PoweroffUHostInstance - 直接关闭UHost实例电源，无需等待实例正常关闭。
-    """
+    """PoweroffUHostInstance - 直接关闭UHost实例电源，无需等待实例正常关闭。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: RebootUHostInstance
 
 重新启动UHost实例，需要指定数据中心及UHostID两个参数的值。
 """
 
 
 class RebootUHostInstanceRequestSchema(schema.RequestSchema):
-    """ RebootUHostInstance - 重新启动UHost实例，需要指定数据中心及UHostID两个参数的值。
-    """
+    """RebootUHostInstance - 重新启动UHost实例，需要指定数据中心及UHostID两个参数的值。"""
 
     fields = {
         "DiskPassword": fields.Str(required=False, dump_to="DiskPassword"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class RebootUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ RebootUHostInstance - 重新启动UHost实例，需要指定数据中心及UHostID两个参数的值。
-    """
+    """RebootUHostInstance - 重新启动UHost实例，需要指定数据中心及UHostID两个参数的值。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: ReinstallUHostInstance
 
 重新安装指定UHost实例的操作系统
 """
 
 
 class ReinstallUHostInstanceRequestSchema(schema.RequestSchema):
-    """ ReinstallUHostInstance - 重新安装指定UHost实例的操作系统
-    """
+    """ReinstallUHostInstance - 重新安装指定UHost实例的操作系统"""
 
     fields = {
         "DNSServers": fields.List(fields.Str()),
         "ImageId": fields.Str(required=False, dump_to="ImageId"),
         "Password": fields.Base64(required=False, dump_to="Password"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
@@ -714,85 +673,79 @@
         "ResourceType": fields.Int(required=False, dump_to="ResourceType"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ReinstallUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ ReinstallUHostInstance - 重新安装指定UHost实例的操作系统
-    """
+    """ReinstallUHostInstance - 重新安装指定UHost实例的操作系统"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: ResetUHostInstancePassword
 
 重置UHost实例的管理员密码。
 """
 
 
 class ResetUHostInstancePasswordRequestSchema(schema.RequestSchema):
-    """ ResetUHostInstancePassword - 重置UHost实例的管理员密码。
-    """
+    """ResetUHostInstancePassword - 重置UHost实例的管理员密码。"""
 
     fields = {
         "Password": fields.Base64(required=True, dump_to="Password"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ResetUHostInstancePasswordResponseSchema(schema.ResponseSchema):
-    """ ResetUHostInstancePassword - 重置UHost实例的管理员密码。
-    """
+    """ResetUHostInstancePassword - 重置UHost实例的管理员密码。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: ResizeAttachedDisk
 
 修改挂载的磁盘大小，包含系统盘和数据盘
 """
 
 
 class ResizeAttachedDiskRequestSchema(schema.RequestSchema):
-    """ ResizeAttachedDisk - 修改挂载的磁盘大小，包含系统盘和数据盘
-    """
+    """ResizeAttachedDisk - 修改挂载的磁盘大小，包含系统盘和数据盘"""
 
     fields = {
         "DiskId": fields.Str(required=True, dump_to="DiskId"),
         "DiskSpace": fields.Int(required=True, dump_to="DiskSpace"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ResizeAttachedDiskResponseSchema(schema.ResponseSchema):
-    """ ResizeAttachedDisk - 修改挂载的磁盘大小，包含系统盘和数据盘
-    """
+    """ResizeAttachedDisk - 修改挂载的磁盘大小，包含系统盘和数据盘"""
 
     fields = {"DiskId": fields.Str(required=False, load_from="DiskId")}
 
 
 """
 API: ResizeUHostInstance
 
 修改指定UHost实例的资源配置，如CPU核心数，内存容量大小，磁盘空间大小,网络增强等。
 """
 
 
 class ResizeUHostInstanceRequestSchema(schema.RequestSchema):
-    """ ResizeUHostInstance - 修改指定UHost实例的资源配置，如CPU核心数，内存容量大小，磁盘空间大小,网络增强等。
-    """
+    """ResizeUHostInstance - 修改指定UHost实例的资源配置，如CPU核心数，内存容量大小，磁盘空间大小,网络增强等。"""
 
     fields = {
         "BootDiskSpace": fields.Int(required=False, dump_to="BootDiskSpace"),
         "CPU": fields.Int(required=False, dump_to="CPU"),
         "DiskSpace": fields.Int(required=False, dump_to="DiskSpace"),
         "Memory": fields.Int(required=False, dump_to="Memory"),
         "NetCapValue": fields.Int(required=False, dump_to="NetCapValue"),
@@ -800,124 +753,115 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ResizeUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ ResizeUHostInstance - 修改指定UHost实例的资源配置，如CPU核心数，内存容量大小，磁盘空间大小,网络增强等。
-    """
+    """ResizeUHostInstance - 修改指定UHost实例的资源配置，如CPU核心数，内存容量大小，磁盘空间大小,网络增强等。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: StartUHostInstance
 
 启动处于关闭状态的UHost实例，需要指定数据中心及UHostID两个参数的值。
 """
 
 
 class StartUHostInstanceRequestSchema(schema.RequestSchema):
-    """ StartUHostInstance - 启动处于关闭状态的UHost实例，需要指定数据中心及UHostID两个参数的值。
-    """
+    """StartUHostInstance - 启动处于关闭状态的UHost实例，需要指定数据中心及UHostID两个参数的值。"""
 
     fields = {
         "DiskPassword": fields.Str(required=False, dump_to="DiskPassword"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class StartUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ StartUHostInstance - 启动处于关闭状态的UHost实例，需要指定数据中心及UHostID两个参数的值。
-    """
+    """StartUHostInstance - 启动处于关闭状态的UHost实例，需要指定数据中心及UHostID两个参数的值。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: StopUHostInstance
 
 指停止处于运行状态的UHost实例，需指定数据中心及UhostID。
 """
 
 
 class StopUHostInstanceRequestSchema(schema.RequestSchema):
-    """ StopUHostInstance - 指停止处于运行状态的UHost实例，需指定数据中心及UhostID。
-    """
+    """StopUHostInstance - 指停止处于运行状态的UHost实例，需指定数据中心及UhostID。"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class StopUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ StopUHostInstance - 指停止处于运行状态的UHost实例，需指定数据中心及UhostID。
-    """
+    """StopUHostInstance - 指停止处于运行状态的UHost实例，需指定数据中心及UhostID。"""
 
     fields = {"UhostId": fields.Str(required=False, load_from="UhostId")}
 
 
 """
 API: TerminateCustomImage
 
 删除用户自定义镜像
 """
 
 
 class TerminateCustomImageRequestSchema(schema.RequestSchema):
-    """ TerminateCustomImage - 删除用户自定义镜像
-    """
+    """TerminateCustomImage - 删除用户自定义镜像"""
 
     fields = {
         "ImageId": fields.Str(required=True, dump_to="ImageId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class TerminateCustomImageResponseSchema(schema.ResponseSchema):
-    """ TerminateCustomImage - 删除用户自定义镜像
-    """
+    """TerminateCustomImage - 删除用户自定义镜像"""
 
     fields = {"ImageId": fields.Str(required=False, load_from="ImageId")}
 
 
 """
 API: TerminateUHostInstance
 
 删除指定数据中心的UHost实例。
 """
 
 
 class TerminateUHostInstanceRequestSchema(schema.RequestSchema):
-    """ TerminateUHostInstance - 删除指定数据中心的UHost实例。
-    """
+    """TerminateUHostInstance - 删除指定数据中心的UHost实例。"""
 
     fields = {
         "Destroy": fields.Int(required=False, dump_to="Destroy"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ReleaseEIP": fields.Bool(required=False, dump_to="ReleaseEIP"),
         "ReleaseUDisk": fields.Bool(required=False, dump_to="ReleaseUDisk"),
         "UHostId": fields.Str(required=True, dump_to="UHostId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class TerminateUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ TerminateUHostInstance - 删除指定数据中心的UHost实例。
-    """
+    """TerminateUHostInstance - 删除指定数据中心的UHost实例。"""
 
     fields = {
         "InRecycle": fields.Str(required=True, load_from="InRecycle"),
         "UHostId": fields.Str(required=False, load_from="UHostId"),
     }
 
 
@@ -925,27 +869,25 @@
 API: UpgradeToArkUHostInstance
 
 普通升级为方舟机型
 """
 
 
 class UpgradeToArkUHostInstanceRequestSchema(schema.RequestSchema):
-    """ UpgradeToArkUHostInstance - 普通升级为方舟机型
-    """
+    """UpgradeToArkUHostInstance - 普通升级为方舟机型"""
 
     fields = {
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "UHostIds": fields.List(fields.Str()),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class UpgradeToArkUHostInstanceResponseSchema(schema.ResponseSchema):
-    """ UpgradeToArkUHostInstance - 普通升级为方舟机型
-    """
+    """UpgradeToArkUHostInstance - 普通升级为方舟机型"""
 
     fields = {
         "UHostSet": fields.List(
             fields.Str(), required=False, load_from="UHostSet"
         )
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uhost/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uhost/schemas/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class UHostImageSetSchema(schema.ResponseSchema):
-    """ UHostImageSet - DescribeImage
-    """
+    """UHostImageSet - DescribeImage"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Features": fields.List(fields.Str()),
         "FuncType": fields.Str(required=False, load_from="FuncType"),
         "ImageDescription": fields.Str(
             required=False, load_from="ImageDescription"
@@ -28,38 +27,35 @@
         "State": fields.Str(required=False, load_from="State"),
         "Vendor": fields.Str(required=False, load_from="Vendor"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class SpreadInfoSchema(schema.ResponseSchema):
-    """ SpreadInfo - 每个可用区中硬件隔离组信息
-    """
+    """SpreadInfo - 每个可用区中硬件隔离组信息"""
 
     fields = {
         "UHostCount": fields.Int(required=False, load_from="UHostCount"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class IsolationGroupSchema(schema.ResponseSchema):
-    """ IsolationGroup - 硬件隔离组信息
-    """
+    """IsolationGroup - 硬件隔离组信息"""
 
     fields = {
         "GroupId": fields.Str(required=False, load_from="GroupId"),
         "GroupName": fields.Str(required=False, load_from="GroupName"),
         "Remark": fields.Str(required=False, load_from="Remark"),
         "SpreadInfoSet": fields.List(SpreadInfoSchema()),
     }
 
 
 class UHostDiskSetSchema(schema.ResponseSchema):
-    """ UHostDiskSet - DescribeUHostInstance
-    """
+    """UHostDiskSet - DescribeUHostInstance"""
 
     fields = {
         "BackupType": fields.Str(required=False, load_from="BackupType"),
         "DiskId": fields.Str(required=False, load_from="DiskId"),
         "DiskType": fields.Str(required=True, load_from="DiskType"),
         "Drive": fields.Str(required=False, load_from="Drive"),
         "Encrypted": fields.Bool(required=False, load_from="Encrypted"),
@@ -67,16 +63,15 @@
         "Name": fields.Str(required=False, load_from="Name"),
         "Size": fields.Int(required=False, load_from="Size"),
         "Type": fields.Str(required=False, load_from="Type"),
     }
 
 
 class UHostIPSetSchema(schema.ResponseSchema):
-    """ UHostIPSet - DescribeUHostInstance
-    """
+    """UHostIPSet - DescribeUHostInstance"""
 
     fields = {
         "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
         "Default": fields.Str(required=True, load_from="Default"),
         "IP": fields.Str(required=False, load_from="IP"),
         "IPId": fields.Str(required=False, load_from="IPId"),
         "Mac": fields.Str(required=True, load_from="Mac"),
@@ -84,16 +79,15 @@
         "Type": fields.Str(required=False, load_from="Type"),
         "VPCId": fields.Str(required=False, load_from="VPCId"),
         "Weight": fields.Int(required=True, load_from="Weight"),
     }
 
 
 class UHostInstanceSetSchema(schema.ResponseSchema):
-    """ UHostInstanceSet - DescribeUHostInstance
-    """
+    """UHostInstanceSet - DescribeUHostInstance"""
 
     fields = {
         "AutoRenew": fields.Str(required=False, load_from="AutoRenew"),
         "BasicImageId": fields.Str(required=False, load_from="BasicImageId"),
         "BasicImageName": fields.Str(
             required=False, load_from="BasicImageName"
         ),
@@ -135,36 +129,33 @@
         "UHostId": fields.Str(required=False, load_from="UHostId"),
         "UHostType": fields.Str(required=False, load_from="UHostType"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UHostSnapshotSetSchema(schema.ResponseSchema):
-    """ UHostSnapshotSet - DescribeUHostInstanceSnapshot
-    """
+    """UHostSnapshotSet - DescribeUHostInstanceSnapshot"""
 
     fields = {
         "SnapshotName": fields.Str(required=False, load_from="SnapshotName"),
         "SnapshotState": fields.Str(required=False, load_from="SnapshotState"),
         "SnapshotTime": fields.Str(required=False, load_from="SnapshotTime"),
     }
 
 
 class UHostTagSetSchema(schema.ResponseSchema):
-    """ UHostTagSet - DescribeUHostTags
-    """
+    """UHostTagSet - DescribeUHostTags"""
 
     fields = {
         "Tag": fields.Str(required=False, load_from="Tag"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class UHostPriceSetSchema(schema.ResponseSchema):
-    """ UHostPriceSet - 主机价格
-    """
+    """UHostPriceSet - 主机价格"""
 
     fields = {
         "ChargeType": fields.Str(required=True, load_from="ChargeType"),
         "Price": fields.Float(required=True, load_from="Price"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uhub/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uhub/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 class UHubClient(Client):
     def __init__(
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UHubClient, self).__init__(config, transport, middleware, logger)
 
     def create_repo(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateRepo - 创建镜像仓库
+        """CreateRepo - 创建镜像仓库
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **RepoName** (str) - (Required) 仓库名称，不可修改
         - **Description** (str) - 仓库备注
         - **IsShared** (bool) - 镜像仓库是否公开，公开为true、不公开为false;默认为false
-        
+
         **Response**
 
         - **Message** (str) - 有错误时返回内容
-        
+
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
         }
         req and d.update(req)
         d = apis.CreateRepoRequestSchema().dumps(d)
@@ -38,84 +38,84 @@
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreateRepo", d, **kwargs)
         return apis.CreateRepoResponseSchema().loads(resp)
 
     def delete_repo(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteRepo - 删除镜像仓库
+        """DeleteRepo - 删除镜像仓库
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **RepoName** (str) - (Required) 镜像仓库名称
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
         }
         req and d.update(req)
         d = apis.DeleteRepoRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteRepo", d, **kwargs)
         return apis.DeleteRepoResponseSchema().loads(resp)
 
     def delete_repo_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteRepoImage - 删除镜像
+        """DeleteRepoImage - 删除镜像
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **ImageName** (str) - (Required) 镜像名称
         - **RepoName** (str) - (Required) 镜像仓库名称
         - **TagName** (str) - 不指定tag则删除全部tag
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
         }
         req and d.update(req)
         d = apis.DeleteRepoImageRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteRepoImage", d, **kwargs)
         return apis.DeleteRepoImageResponseSchema().loads(resp)
 
     def get_image_tag(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetImageTag - 获取镜像tag
+        """GetImageTag - 获取镜像tag
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **ImageName** (str) - (Required) 镜像名称
         - **RepoName** (str) - (Required) 镜像仓库名称
         - **Limit** (int) - 每次获取数量，默认为20
         - **Offset** (int) - 偏移量，默认0
         - **TagName** (str) - 默认不写，如果填写，代表查询该tag，否则查全部tag
-        
+
         **Response**
 
         - **TagSet** (list) - 见 **TagSet** 模型定义
         - **TotalCount** (int) - tag总数
-        
+
         **Response Model**
-        
-        **TagSet** 
-        
+
+        **TagSet**
+
         - **TagName** (str) - Tag名称
         - **UpdateTime** (str) - 镜像更新时间
 
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
@@ -123,32 +123,32 @@
         req and d.update(req)
         d = apis.GetImageTagRequestSchema().dumps(d)
 
         resp = self.invoke("GetImageTag", d, **kwargs)
         return apis.GetImageTagResponseSchema().loads(resp)
 
     def get_repo(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ GetRepo - 获取镜像仓库
+        """GetRepo - 获取镜像仓库
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Limit** (int) - 数量，默认20
         - **Offset** (int) - 偏移量，默认0
         - **Type** (str) - private私有仓库，public公共仓库，默认public
-        
+
         **Response**
 
         - **RepoSet** (list) - 见 **RepoSet** 模型定义
         - **TotalCount** (int) - 总的仓库数量
-        
+
         **Response Model**
-        
-        **RepoSet** 
-        
+
+        **RepoSet**
+
         - **CreateTime** (str) - 仓库创建时间
         - **Description** (str) - 镜像仓库描述
         - **IsOutSide** (str) - 镜像仓库是否外网可以访问，可以为ture,不可以为false
         - **IsShared** (str) - 镜像仓库类型,false为私有；true为公有
         - **RepoName** (str) - 镜像仓库名称
         - **UpdateTime** (str) - 仓库更新时间
 
@@ -162,32 +162,32 @@
 
         resp = self.invoke("GetRepo", d, **kwargs)
         return apis.GetRepoResponseSchema().loads(resp)
 
     def get_repo_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetRepoImage - 获取镜像仓库下的镜像
+        """GetRepoImage - 获取镜像仓库下的镜像
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **RepoName** (str) - (Required) 镜像仓库名称
         - **Limit** (int) - 显示数量，默认为20
         - **Offset** (int) - 偏移量，默认0
-        
+
         **Response**
 
         - **ImageSet** (list) - 见 **ImageSet** 模型定义
-        - **TotalCount** (int) - 
-        
+        - **TotalCount** (int) -
+
         **Response Model**
-        
-        **ImageSet** 
-        
+
+        **ImageSet**
+
         - **CreateTime** (str) - 创建时间
         - **ImageName** (str) - 镜像名称
         - **LatestTag** (str) - 最新push的Tag
         - **PullCount** (int) - 镜像被下载次数
         - **RepoName** (str) - 镜像仓库名称
         - **UpdateTime** (str) - 修改时间
 
@@ -199,27 +199,27 @@
         req and d.update(req)
         d = apis.GetRepoImageRequestSchema().dumps(d)
 
         resp = self.invoke("GetRepoImage", d, **kwargs)
         return apis.GetRepoImageResponseSchema().loads(resp)
 
     def update_repo(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ UpdateRepo - 更新镜像仓库
+        """UpdateRepo - 更新镜像仓库
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **RepoName** (str) - (Required) 镜像仓库名称，不可修改
         - **Description** (str) - 备注
         - **IsShared** (str) - false设置为私有；true设置为公有。默认false
-        
+
         **Response**
 
         - **Message** (str) - 错误的时候返回
-        
+
         """
         # build request
         d = {
             "ProjectId": self.config.project_id,
         }
         req and d.update(req)
         d = apis.UpdateRepoRequestSchema().dumps(d)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uhub/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uhub/schemas/apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,108 +12,100 @@
 API: CreateRepo
 
 创建镜像仓库
 """
 
 
 class CreateRepoRequestSchema(schema.RequestSchema):
-    """ CreateRepo - 创建镜像仓库
-    """
+    """CreateRepo - 创建镜像仓库"""
 
     fields = {
         "Description": fields.Str(required=False, dump_to="Description"),
         "IsShared": fields.Bool(required=False, dump_to="IsShared"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "RepoName": fields.Str(required=True, dump_to="RepoName"),
     }
 
 
 class CreateRepoResponseSchema(schema.ResponseSchema):
-    """ CreateRepo - 创建镜像仓库
-    """
+    """CreateRepo - 创建镜像仓库"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
 """
 API: DeleteRepo
 
 删除镜像仓库
 """
 
 
 class DeleteRepoRequestSchema(schema.RequestSchema):
-    """ DeleteRepo - 删除镜像仓库
-    """
+    """DeleteRepo - 删除镜像仓库"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "RepoName": fields.Str(required=True, dump_to="RepoName"),
     }
 
 
 class DeleteRepoResponseSchema(schema.ResponseSchema):
-    """ DeleteRepo - 删除镜像仓库
-    """
+    """DeleteRepo - 删除镜像仓库"""
 
     fields = {}
 
 
 """
 API: DeleteRepoImage
 
 删除镜像
 """
 
 
 class DeleteRepoImageRequestSchema(schema.RequestSchema):
-    """ DeleteRepoImage - 删除镜像
-    """
+    """DeleteRepoImage - 删除镜像"""
 
     fields = {
         "ImageName": fields.Str(required=True, dump_to="ImageName"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "RepoName": fields.Str(required=True, dump_to="RepoName"),
         "TagName": fields.Str(required=False, dump_to="TagName"),
     }
 
 
 class DeleteRepoImageResponseSchema(schema.ResponseSchema):
-    """ DeleteRepoImage - 删除镜像
-    """
+    """DeleteRepoImage - 删除镜像"""
 
     fields = {}
 
 
 """
 API: GetImageTag
 
 获取镜像tag
 """
 
 
 class GetImageTagRequestSchema(schema.RequestSchema):
-    """ GetImageTag - 获取镜像tag
-    """
+    """GetImageTag - 获取镜像tag"""
 
     fields = {
         "ImageName": fields.Str(required=True, dump_to="ImageName"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "RepoName": fields.Str(required=True, dump_to="RepoName"),
         "TagName": fields.Str(required=False, dump_to="TagName"),
     }
 
 
 class GetImageTagResponseSchema(schema.ResponseSchema):
-    """ GetImageTag - 获取镜像tag
-    """
+    """GetImageTag - 获取镜像tag"""
 
     fields = {
         "TagSet": fields.List(
             models.TagSetSchema(), required=True, load_from="TagSet"
         ),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
@@ -123,28 +115,26 @@
 API: GetRepo
 
 获取镜像仓库
 """
 
 
 class GetRepoRequestSchema(schema.RequestSchema):
-    """ GetRepo - 获取镜像仓库
-    """
+    """GetRepo - 获取镜像仓库"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Type": fields.Str(required=False, dump_to="Type"),
     }
 
 
 class GetRepoResponseSchema(schema.ResponseSchema):
-    """ GetRepo - 获取镜像仓库
-    """
+    """GetRepo - 获取镜像仓库"""
 
     fields = {
         "RepoSet": fields.List(
             models.RepoSetSchema(), required=True, load_from="RepoSet"
         ),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
@@ -154,28 +144,26 @@
 API: GetRepoImage
 
 获取镜像仓库下的镜像
 """
 
 
 class GetRepoImageRequestSchema(schema.RequestSchema):
-    """ GetRepoImage - 获取镜像仓库下的镜像
-    """
+    """GetRepoImage - 获取镜像仓库下的镜像"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "RepoName": fields.Str(required=True, dump_to="RepoName"),
     }
 
 
 class GetRepoImageResponseSchema(schema.ResponseSchema):
-    """ GetRepoImage - 获取镜像仓库下的镜像
-    """
+    """GetRepoImage - 获取镜像仓库下的镜像"""
 
     fields = {
         "ImageSet": fields.List(
             models.ImageSetSchema(), required=True, load_from="ImageSet"
         ),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
@@ -185,25 +173,23 @@
 API: UpdateRepo
 
 更新镜像仓库
 """
 
 
 class UpdateRepoRequestSchema(schema.RequestSchema):
-    """ UpdateRepo - 更新镜像仓库
-    """
+    """UpdateRepo - 更新镜像仓库"""
 
     fields = {
         "Description": fields.Str(required=False, dump_to="Description"),
         "IsShared": fields.Str(required=False, dump_to="IsShared"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "RepoName": fields.Str(required=True, dump_to="RepoName"),
     }
 
 
 class UpdateRepoResponseSchema(schema.ResponseSchema):
-    """ UpdateRepo - 更新镜像仓库
-    """
+    """UpdateRepo - 更新镜像仓库"""
 
     fields = {
         "Message": fields.Str(required=False, load_from="Message"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uhub/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uhub/schemas/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class TagSetSchema(schema.ResponseSchema):
-    """ TagSet - Tag详细信息
-    """
+    """TagSet - Tag详细信息"""
 
     fields = {
         "TagName": fields.Str(required=True, load_from="TagName"),
         "UpdateTime": fields.Str(required=True, load_from="UpdateTime"),
     }
 
 
 class RepoSetSchema(schema.ResponseSchema):
-    """ RepoSet - 镜像仓库
-    """
+    """RepoSet - 镜像仓库"""
 
     fields = {
         "CreateTime": fields.Str(required=True, load_from="CreateTime"),
         "Description": fields.Str(required=True, load_from="Description"),
         "IsOutSide": fields.Str(required=True, load_from="IsOutSide"),
         "IsShared": fields.Str(required=True, load_from="IsShared"),
         "RepoName": fields.Str(required=True, load_from="RepoName"),
         "UpdateTime": fields.Str(required=True, load_from="UpdateTime"),
     }
 
 
 class ImageSetSchema(schema.ResponseSchema):
-    """ ImageSet - 镜像信息
-    """
+    """ImageSet - 镜像信息"""
 
     fields = {
         "CreateTime": fields.Str(required=True, load_from="CreateTime"),
         "ImageName": fields.Str(required=True, load_from="ImageName"),
         "LatestTag": fields.Str(required=True, load_from="LatestTag"),
         "PullCount": fields.Int(required=True, load_from="PullCount"),
         "RepoName": fields.Str(required=True, load_from="RepoName"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ulb/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ulb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,183 +12,183 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(ULBClient, self).__init__(config, transport, middleware, logger)
 
     def allocate_backend(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ AllocateBackend - 添加ULB后端资源实例
+        """AllocateBackend - 添加ULB后端资源实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ResourceId** (str) - (Required) 所添加的后端资源的资源ID
         - **ResourceType** (str) - (Required) 所添加的后端资源的类型，枚举值：UHost -> 云主机；UPM -> 物理云主机； UDHost -> 私有专区主机；UDocker -> 容器，默认值为“UHost”
         - **ULBId** (str) - (Required) 负载均衡实例的ID
         - **VServerId** (str) - (Required) VServer实例的ID
         - **Enabled** (int) - 后端实例状态开关，枚举值： 1：启用； 0：禁用 默认为启用
         - **Port** (int) - 所添加的后端资源服务端口，取值范围[1-65535]，默认80
         - **Weight** (int) - 所添加的后端RS权重（在加权轮询算法下有效），取值范围[0-100]，默认为1
-        
+
         **Response**
 
         - **BackendId** (str) - 所添加的后端资源在ULB中的对象ID，（为ULB系统中使用，与资源自身ID无关），可用于 UpdateBackendAttribute/UpdateBackendAttributeBatch/ReleaseBackend
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.AllocateBackendRequestSchema().dumps(d)
 
         resp = self.invoke("AllocateBackend", d, **kwargs)
         return apis.AllocateBackendResponseSchema().loads(resp)
 
     def allocate_backend_batch(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ AllocateBackendBatch - 批量添加VServer后端节点
+        """AllocateBackendBatch - 批量添加VServer后端节点
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Backends** (list) - (Required) 用| 分割字段，格式：ResourceId| ResourceType| Port| Enabled|IP| Weight。ResourceId:所添加的后端资源的资源ID；ResourceType:所添加的后端资源的类型，枚举值：UHost -> 云主机；UPM -> 物理云主机； UDHost -> 私有专区主机；UDocker -> 容器，默认值为“UHost”；Port:所添加的后端资源服务端口，取值范围[1-65535]；Enabled:后端实例状态开关，枚举值： 1：启用； 0：禁用；IP:后端资源内网ip；Weight：所添加的后端RS权重（在加权轮询算法下有效），取值范围[0-100]，默认为1
         - **ULBId** (str) - (Required) 负载均衡实例的ID
         - **VServerId** (str) - (Required) VServer实例的ID
-        - **ApiVersion** (int) - 
-        
+        - **ApiVersion** (int) -
+
         **Response**
 
         - **BackendSet** (list) - 见 **BackendSet** 模型定义
-        
+
         **Response Model**
-        
-        **BackendSet** 
-        
+
+        **BackendSet**
+
         - **BackendId** (str) - rs的资源ID
         - **ResourceId** (str) - rs对应的UHost ID
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.AllocateBackendBatchRequestSchema().dumps(d)
 
         resp = self.invoke("AllocateBackendBatch", d, **kwargs)
         return apis.AllocateBackendBatchResponseSchema().loads(resp)
 
     def bind_ssl(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ BindSSL - 将SSL证书绑定到VServer
+        """BindSSL - 将SSL证书绑定到VServer
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SSLId** (str) - (Required) SSL证书的Id
         - **ULBId** (str) - (Required) 所绑定ULB实例ID
         - **VServerId** (str) - (Required) 所绑定VServer实例ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.BindSSLRequestSchema().dumps(d)
 
         resp = self.invoke("BindSSL", d, **kwargs)
         return apis.BindSSLResponseSchema().loads(resp)
 
     def create_policy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreatePolicy - 创建VServer内容转发策略
+        """CreatePolicy - 创建VServer内容转发策略
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackendId** (list) - (Required) 内容转发策略应用的后端资源实例的ID，来源于 AllocateBackend 返回的 BackendId
         - **Match** (str) - (Required) 内容转发匹配字段
         - **ULBId** (str) - (Required) 需要添加内容转发策略的负载均衡实例ID
         - **VServerId** (str) - (Required) 需要添加内容转发策略的VServer实例ID
         - **Type** (str) - 内容转发匹配字段的类型
-        
+
         **Response**
 
         - **PolicyId** (str) - 内容转发策略ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreatePolicyRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreatePolicy", d, **kwargs)
         return apis.CreatePolicyResponseSchema().loads(resp)
 
     def create_ssl(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateSSL - 创建SSL证书，可以把整个 Pem 证书内容传过来，或者把证书、私钥、CA证书分别传过来
+        """CreateSSL - 创建SSL证书，可以把整个 Pem 证书内容传过来，或者把证书、私钥、CA证书分别传过来
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SSLName** (str) - (Required) SSL证书的名字，默认值为空
         - **CaCert** (str) - CA证书
         - **PrivateKey** (str) - 加密证书的私钥
         - **SSLContent** (str) - SSL证书的完整内容，包括用户证书、加密证书的私钥、CA证书
         - **SSLType** (str) - 所添加的SSL证书类型，目前只支持Pem格式
         - **UserCert** (str) - 用户的证书
-        
+
         **Response**
 
         - **SSLId** (str) - SSL证书的Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateSSLRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreateSSL", d, **kwargs)
         return apis.CreateSSLResponseSchema().loads(resp)
 
     def create_ulb(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateULB - 创建负载均衡实例，可以选择内网或者外网
+        """CreateULB - 创建负载均衡实例，可以选择内网或者外网
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BusinessId** (str) - ULB 所属的业务组ID，如果不传则使用默认的业务组
         - **ChargeType** (str) - 付费方式
         - **IPVersion** (str) - ULB ip类型，枚举值：IPv6 / IPv4 （内部测试，暂未对外开放）
         - **InnerMode** (str) - 创建的ULB是否为内网模式
         - **ListenType** (str) - ULB 监听器类型，枚举值：RequestProxy / PacketsTransmit （内部测试，暂未对外开放）
         - **OuterMode** (str) - 创建的ULB是否为外网模式，默认即为外网模式
         - **PrivateIp** (str) - 创建内网ULB时指定内网IP。若不传值，则随机分配当前子网下的IP（暂时不对外开放，创建外网ULB该字段会忽略）
         - **Remark** (str) - 备注
         - **SubnetId** (str) - 内网ULB 所属的子网ID，如果不传则使用默认的子网
         - **Tag** (str) - 业务组
         - **ULBName** (str) - 负载均衡的名字，默认值为“ULB”
         - **VPCId** (str) - ULB所在的VPC的ID, 如果不传则使用默认的VPC
-        
+
         **Response**
 
         - **ULBId** (str) - 负载均衡实例的Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateULBRequestSchema().dumps(d)
 
         # build options
@@ -196,37 +196,37 @@
 
         resp = self.invoke("CreateULB", d, **kwargs)
         return apis.CreateULBResponseSchema().loads(resp)
 
     def create_vserver(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateVServer - 创建VServer实例，定义监听的协议和端口以及负载均衡算法
+        """CreateVServer - 创建VServer实例，定义监听的协议和端口以及负载均衡算法
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ULBId** (str) - (Required) 负载均衡实例ID
         - **ClientTimeout** (int) - ListenType为RequestProxy时表示空闲连接的回收时间，单位：秒，取值范围：时(0，86400]，默认值为60；ListenType为PacketsTransmit时表示连接保持的时间，单位：秒，取值范围：[60，900]，0 表示禁用连接保持
         - **Domain** (str) - 根据MonitorType确认； 当MonitorType为Port时，此字段无意义。当MonitorType为Path时，代表HTTP检查域名
         - **FrontendPort** (int) - VServer后端端口，取值范围[1-65535]；默认值为80
         - **ListenType** (str) - 监听器类型，枚举值为：RequestProxy -> 请求代理；PacketsTransmit -> 报文转发；默认为"RequestProxy"
         - **Method** (str) - VServer负载均衡模式，枚举值：Roundrobin -> 轮询;Source -> 源地址；ConsistentHash -> 一致性哈希；SourcePort -> 源地址（计算端口）；ConsistentHashPort -> 一致性哈希（计算端口）; WeightRoundrobin -> 加权轮询; Leastconn -> 最小连接数。ConsistentHash，SourcePort，ConsistentHashPort 只在报文转发中使用；Leastconn只在请求代理中使用；Roundrobin、Source和WeightRoundrobin在请求代理和报文转发中使用。默认为："Roundrobin"
         - **MonitorType** (str) - 健康检查类型，枚举值：Port -> 端口检查；Path -> 路径检查；
         - **Path** (str) - 根据MonitorType确认； 当MonitorType为Port时，此字段无意义。当MonitorType为Path时，代表HTTP检查路径
         - **PersistenceInfo** (str) - 根据PersistenceType确认； None和ServerInsert： 此字段无意义； UserDefined：此字段传入自定义会话保持String
         - **PersistenceType** (str) - VServer会话保持方式，默认关闭会话保持。枚举值：None -> 关闭；ServerInsert -> 自动生成KEY；UserDefined -> 用户自定义KEY。
         - **Protocol** (str) - VServer实例的协议，请求代理模式下有 HTTP、HTTPS、TCP，报文转发下有 TCP，UDP。默认为“HTTP"
         - **VServerName** (str) - VServer实例名称，默认为"VServer"
-        
+
         **Response**
 
         - **VServerId** (str) - VServer实例的Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateVServerRequestSchema().dumps(d)
 
         # build options
@@ -234,200 +234,200 @@
 
         resp = self.invoke("CreateVServer", d, **kwargs)
         return apis.CreateVServerResponseSchema().loads(resp)
 
     def delete_policy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeletePolicy - 删除内容转发策略
+        """DeletePolicy - 删除内容转发策略
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PolicyId** (str) - (Required) 内容转发策略ID
         - **GroupId** (str) - 内容转发策略组ID
         - **VServerId** (str) - VServer 资源ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeletePolicyRequestSchema().dumps(d)
 
         resp = self.invoke("DeletePolicy", d, **kwargs)
         return apis.DeletePolicyResponseSchema().loads(resp)
 
     def delete_ssl(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteSSL - 删除SSL证书
+        """DeleteSSL - 删除SSL证书
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SSLId** (str) - (Required) SSL证书的ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteSSLRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteSSL", d, **kwargs)
         return apis.DeleteSSLResponseSchema().loads(resp)
 
     def delete_ulb(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteULB - 删除负载均衡实例
+        """DeleteULB - 删除负载均衡实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ULBId** (str) - (Required) 负载均衡实例的ID
         - **ReleaseEip** (bool) - 删除ulb时是否释放绑定的EIP，false标识只解绑EIP，true表示会释放绑定的EIP，默认是false
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteULBRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteULB", d, **kwargs)
         return apis.DeleteULBResponseSchema().loads(resp)
 
     def delete_vserver(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteVServer - 删除VServer实例
+        """DeleteVServer - 删除VServer实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ULBId** (str) - (Required) 负载均衡实例的ID
         - **VServerId** (str) - (Required) VServer实例的ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteVServerRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteVServer", d, **kwargs)
         return apis.DeleteVServerResponseSchema().loads(resp)
 
     def describe_ssl(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeSSL - 获取SSL证书信息
+        """DescribeSSL - 获取SSL证书信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 数据分页值，默认为20
         - **Offset** (int) - 数据偏移量，默认值为0
         - **SSLId** (str) - SSL证书的Id
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **ULBSSLSet** 模型定义
         - **TotalCount** (int) - 满足条件的SSL证书总数
-        
+
         **Response Model**
-        
-        **ULBSSLSet** 
-        
-        - **HashValue** (str) - 
+
+        **ULBSSLSet**
+
+        - **HashValue** (str) -
         - **SSLId** (str) - SSL证书的Id
         - **SSLName** (str) - SSL证书的名字
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeSSLRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeSSL", d, **kwargs)
         return apis.DescribeSSLResponseSchema().loads(resp)
 
     def describe_ulb(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeULB - 获取ULB详细信息
+        """DescribeULB - 获取ULB详细信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BusinessId** (str) - ULB所属的业务组ID
         - **Limit** (int) - 数据分页值，默认为20
         - **Offset** (int) - 数据偏移量，默认为0
         - **SubnetId** (str) - ULB所属的子网ID
         - **ULBId** (str) - 负载均衡实例的Id。 若指定则返回指定的负载均衡实例的信息； 若不指定则返回当前数据中心中所有的负载均衡实例的信息
         - **VPCId** (str) - ULB所属的VPC
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **ULBSet** 模型定义
         - **TotalCount** (int) - 满足条件的ULB总数
-        
+
         **Response Model**
-        
-        **PolicyBackendSet** 
-        
+
+        **PolicyBackendSet**
+
         - **BackendId** (str) - 所添加的后端资源在ULB中的对象ID，（为ULB系统中使用，与资源自身ID无关
         - **ObjectId** (str) - 后端资源的对象ID
         - **Port** (int) - 所添加的后端资源服务端口
         - **PrivateIP** (str) - 后端资源的内网IP
         - **ResourceName** (str) - 后端资源的实例名称
 
-        **ULBPolicySet** 
-        
+        **ULBPolicySet**
+
         - **BackendSet** (list) - 见 **PolicyBackendSet** 模型定义
         - **Match** (str) - 内容转发匹配字段;默认内容转发类型下为空。
         - **PolicyId** (str) - 内容转发Id，默认内容转发类型下为空。
         - **PolicyPriority** (int) - 内容转发优先级，范围[1,9999]，数字越大优先级越高。默认内容转发规则下为0。
         - **PolicyType** (str) - 内容类型，枚举值：Custom -> 客户自定义；Default -> 默认内容转发
         - **TotalCount** (int) - 默认内容转发类型下返回当前rs总数
         - **Type** (str) - 内容转发匹配字段的类型，枚举值：Domain -> 域名；Path -> 路径； 默认内容转发类型下为空
         - **VServerId** (str) - 所属VServerId
 
-        **ULBBackendSet** 
-        
+        **ULBBackendSet**
+
         - **BackendId** (str) - 后端资源实例的Id
         - **Enabled** (int) - 后端提供服务的实例启用与否，枚举值：0 禁用 1 启用
         - **Port** (int) - 后端提供服务的端口
         - **PrivateIP** (str) - 后端提供服务的内网IP
         - **ResourceId** (str) - 资源实例的资源Id
         - **ResourceName** (str) - 资源实例的资源名称
         - **ResourceType** (str) - 资源实例的类型
         - **Status** (int) - 后端提供服务的实例运行状态，枚举值：0健康检查健康状态 1 健康检查异常
         - **SubResourceId** (str) - 资源绑定的虚拟网卡实例的资源Id
         - **SubResourceName** (str) - 资源绑定的虚拟网卡实例的资源名称
         - **SubResourceType** (str) - 资源绑定的虚拟网卡实例的类型
         - **SubnetId** (str) - 后端提供服务的资源所在的子网的ID
-        - **Weight** (int) - 
+        - **Weight** (int) -
+
+        **ULBSSLSet**
 
-        **ULBSSLSet** 
-        
-        - **HashValue** (str) - 
+        - **HashValue** (str) -
         - **SSLId** (str) - SSL证书的Id
         - **SSLName** (str) - SSL证书的名字
 
-        **ULBVServerSet** 
-        
+        **ULBVServerSet**
+
         - **BackendSet** (list) - 见 **ULBBackendSet** 模型定义
         - **ClientTimeout** (int) - 空闲连接的回收时间，单位：秒。
         - **Domain** (str) - 根据MonitorType确认； 当MonitorType为Port时，此字段无意义。当MonitorType为Path时，代表HTTP检查域名
         - **FrontendPort** (int) - VServer服务端口
         - **ListenType** (str) - 监听器类型，枚举值为: RequestProxy -> 请求代理；PacketsTransmit -> 报文转发
         - **Method** (str) - VServer负载均衡的模式，枚举值：Roundrobin -> 轮询;Source -> 源地址；ConsistentHash -> 一致性哈希；SourcePort -> 源地址（计算端口）；ConsistentHashPort -> 一致性哈希（计算端口）。
         - **MonitorType** (str) - 健康检查类型，枚举值：Port -> 端口检查；Path -> 路径检查；
@@ -437,24 +437,24 @@
         - **PolicySet** (list) - 见 **ULBPolicySet** 模型定义
         - **Protocol** (str) - VServer实例的协议。 枚举值为：HTTP，TCP，UDP，HTTPS。
         - **SSLSet** (list) - 见 **ULBSSLSet** 模型定义
         - **Status** (int) - VServer的运行状态。枚举值： 0 -> rs全部运行正常;1 -> rs全部运行异常；2 -> rs部分运行异常。
         - **VServerId** (str) - VServer实例的Id
         - **VServerName** (str) - VServer实例的名字
 
-        **ULBIPSet** 
-        
+        **ULBIPSet**
+
         - **Bandwidth** (int) - 弹性IP的带宽值（暂未对外开放）
         - **BandwidthType** (int) - 弹性IP的带宽类型，枚举值：1 表示是共享带宽，0 普通带宽类型（暂未对外开放）
         - **EIP** (str) - 弹性IP地址
         - **EIPId** (str) - 弹性IP的ID
         - **OperatorName** (str) - 弹性IP的运营商信息，枚举值为：  Bgp：BGP IP International：国际IP
 
-        **ULBSet** 
-        
+        **ULBSet**
+
         - **Bandwidth** (int) - 带宽
         - **BandwidthType** (int) - 带宽类型，枚举值为： 0，非共享带宽； 1，共享带宽
         - **BusinessId** (str) - ULB 所属的业务组ID
         - **CreateTime** (int) - ULB的创建时间，格式为Unix Timestamp
         - **ExpireTime** (int) - ULB的到期时间，格式为Unix Timestamp
         - **IPSet** (list) - 见 **ULBIPSet** 模型定义
         - **Name** (str) - 负载均衡的资源名称（资源系统中），缺省值“ULB”
@@ -477,75 +477,75 @@
 
         resp = self.invoke("DescribeULB", d, **kwargs)
         return apis.DescribeULBResponseSchema().loads(resp)
 
     def describe_vserver(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeVServer - 获取ULB下的VServer的详细信息
+        """DescribeVServer - 获取ULB下的VServer的详细信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ULBId** (str) - (Required) 负载均衡实例的Id
         - **Limit** (int) - 数据分页值
         - **Offset** (int) - 数据偏移量
         - **VServerId** (str) - VServer实例的Id；若指定则返回指定的VServer实例的信息； 若不指定则返回当前负载均衡实例下所有VServer的信息
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **ULBVServerSet** 模型定义
         - **TotalCount** (int) - 满足条件的VServer总数
-        
+
         **Response Model**
-        
-        **PolicyBackendSet** 
-        
+
+        **PolicyBackendSet**
+
         - **BackendId** (str) - 所添加的后端资源在ULB中的对象ID，（为ULB系统中使用，与资源自身ID无关
         - **ObjectId** (str) - 后端资源的对象ID
         - **Port** (int) - 所添加的后端资源服务端口
         - **PrivateIP** (str) - 后端资源的内网IP
         - **ResourceName** (str) - 后端资源的实例名称
 
-        **ULBSSLSet** 
-        
-        - **HashValue** (str) - 
+        **ULBSSLSet**
+
+        - **HashValue** (str) -
         - **SSLId** (str) - SSL证书的Id
         - **SSLName** (str) - SSL证书的名字
 
-        **ULBPolicySet** 
-        
+        **ULBPolicySet**
+
         - **BackendSet** (list) - 见 **PolicyBackendSet** 模型定义
         - **Match** (str) - 内容转发匹配字段;默认内容转发类型下为空。
         - **PolicyId** (str) - 内容转发Id，默认内容转发类型下为空。
         - **PolicyPriority** (int) - 内容转发优先级，范围[1,9999]，数字越大优先级越高。默认内容转发规则下为0。
         - **PolicyType** (str) - 内容类型，枚举值：Custom -> 客户自定义；Default -> 默认内容转发
         - **TotalCount** (int) - 默认内容转发类型下返回当前rs总数
         - **Type** (str) - 内容转发匹配字段的类型，枚举值：Domain -> 域名；Path -> 路径； 默认内容转发类型下为空
         - **VServerId** (str) - 所属VServerId
 
-        **ULBBackendSet** 
-        
+        **ULBBackendSet**
+
         - **BackendId** (str) - 后端资源实例的Id
         - **Enabled** (int) - 后端提供服务的实例启用与否，枚举值：0 禁用 1 启用
         - **Port** (int) - 后端提供服务的端口
         - **PrivateIP** (str) - 后端提供服务的内网IP
         - **ResourceId** (str) - 资源实例的资源Id
         - **ResourceName** (str) - 资源实例的资源名称
         - **ResourceType** (str) - 资源实例的类型
         - **Status** (int) - 后端提供服务的实例运行状态，枚举值：0健康检查健康状态 1 健康检查异常
         - **SubResourceId** (str) - 资源绑定的虚拟网卡实例的资源Id
         - **SubResourceName** (str) - 资源绑定的虚拟网卡实例的资源名称
         - **SubResourceType** (str) - 资源绑定的虚拟网卡实例的类型
         - **SubnetId** (str) - 后端提供服务的资源所在的子网的ID
-        - **Weight** (int) - 
+        - **Weight** (int) -
+
+        **ULBVServerSet**
 
-        **ULBVServerSet** 
-        
         - **BackendSet** (list) - 见 **ULBBackendSet** 模型定义
         - **ClientTimeout** (int) - 空闲连接的回收时间，单位：秒。
         - **Domain** (str) - 根据MonitorType确认； 当MonitorType为Port时，此字段无意义。当MonitorType为Path时，代表HTTP检查域名
         - **FrontendPort** (int) - VServer服务端口
         - **ListenType** (str) - 监听器类型，枚举值为: RequestProxy -> 请求代理；PacketsTransmit -> 报文转发
         - **Method** (str) - VServer负载均衡的模式，枚举值：Roundrobin -> 轮询;Source -> 源地址；ConsistentHash -> 一致性哈希；SourcePort -> 源地址（计算端口）；ConsistentHashPort -> 一致性哈希（计算端口）。
         - **MonitorType** (str) - 健康检查类型，枚举值：Port -> 端口检查；Path -> 路径检查；
@@ -567,164 +567,164 @@
 
         resp = self.invoke("DescribeVServer", d, **kwargs)
         return apis.DescribeVServerResponseSchema().loads(resp)
 
     def release_backend(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ReleaseBackend - 从VServer释放后端资源实例
+        """ReleaseBackend - 从VServer释放后端资源实例
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackendId** (str) - (Required) 后端资源实例的ID(ULB后端ID，非资源自身ID)
         - **ULBId** (str) - (Required) 负载均衡实例的ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ReleaseBackendRequestSchema().dumps(d)
 
         resp = self.invoke("ReleaseBackend", d, **kwargs)
         return apis.ReleaseBackendResponseSchema().loads(resp)
 
     def unbind_ssl(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ UnbindSSL - 从VServer解绑SSL证书
+        """UnbindSSL - 从VServer解绑SSL证书
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SSLId** (str) - (Required) SSL证书的Id
         - **ULBId** (str) - (Required) 所绑定ULB实例ID
         - **VServerId** (str) - (Required) 所绑定VServer实例ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UnbindSSLRequestSchema().dumps(d)
 
         resp = self.invoke("UnbindSSL", d, **kwargs)
         return apis.UnbindSSLResponseSchema().loads(resp)
 
     def update_backend_attribute(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateBackendAttribute - 更新ULB后端资源实例(服务节点)属性
+        """UpdateBackendAttribute - 更新ULB后端资源实例(服务节点)属性
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackendId** (str) - (Required) 后端资源实例的ID(ULB后端ID，非资源自身ID)
         - **ULBId** (str) - (Required) 负载均衡资源ID
         - **Enabled** (int) - 后端实例状态开关
         - **Port** (int) - 后端资源服务端口，取值范围[1-65535]
         - **Weight** (int) - 所添加的后端RS权重（在加权轮询算法下有效），取值范围[0-100]，默认为1
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateBackendAttributeRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateBackendAttribute", d, **kwargs)
         return apis.UpdateBackendAttributeResponseSchema().loads(resp)
 
     def update_policy(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdatePolicy - 更新内容转发规则，包括转发规则后的服务节点
+        """UpdatePolicy - 更新内容转发规则，包括转发规则后的服务节点
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackendId** (list) - (Required) 内容转发策略应用的后端资源实例的ID，来源于 AllocateBackend 返回的 BackendId
         - **Match** (str) - (Required) 内容转发匹配字段
         - **PolicyId** (str) - (Required) 转发规则的ID
         - **ULBId** (str) - (Required) 需要添加内容转发策略的负载均衡实例ID
         - **VServerId** (str) - (Required) 需要添加内容转发策略的VServer实例ID
         - **Type** (str) - 内容转发匹配字段的类型
-        
+
         **Response**
 
         - **PolicyId** (str) - 转发规则的ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdatePolicyRequestSchema().dumps(d)
 
         resp = self.invoke("UpdatePolicy", d, **kwargs)
         return apis.UpdatePolicyResponseSchema().loads(resp)
 
     def update_ulb_attribute(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateULBAttribute - 更新ULB名字业务组备注等属性字段
+        """UpdateULBAttribute - 更新ULB名字业务组备注等属性字段
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ULBId** (str) - (Required) ULB资源ID
         - **Name** (str) - 名字
         - **Remark** (str) - 备注
         - **Tag** (str) - 业务
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateULBAttributeRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateULBAttribute", d, **kwargs)
         return apis.UpdateULBAttributeResponseSchema().loads(resp)
 
     def update_vserver_attribute(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateVServerAttribute - 更新VServer实例属性
+        """UpdateVServerAttribute - 更新VServer实例属性
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ULBId** (str) - (Required) 负载均衡实例ID
         - **VServerId** (str) - (Required) VServer实例ID
         - **ClientTimeout** (int) - 请求代理的VServer下表示空闲连接的回收时间，单位：秒，取值范围：时(0，86400]，默认值为60；报文转发的VServer下表示回话保持的时间，单位：秒，取值范围：[60，900]，0 表示禁用连接保持
         - **Domain** (str) - MonitorType 为 Path 时指定健康检查发送请求时HTTP HEADER 里的域名
         - **Method** (str) - VServer负载均衡模式，枚举值：Roundrobin -> 轮询;Source -> 源地址；ConsistentHash -> 一致性哈希；SourcePort -> 源地址（计算端口）；ConsistentHashPort -> 一致性哈希（计算端口）; WeightRoundrobin -> 加权轮询; Leastconn -> 最小连接数。ConsistentHash，SourcePort，ConsistentHashPort 只在报文转发中使用；Leastconn只在请求代理中使用；Roundrobin、Source和WeightRoundrobin在请求代理和报文转发中使用。默认为："Roundrobin"
         - **MonitorType** (str) - 健康检查的类型，Port:端口,Path:路径
         - **Path** (str) - MonitorType 为 Path 时指定健康检查发送请求时的路径，默认为 /
         - **PersistenceInfo** (str) - 根据PersistenceType确定: None或ServerInsert, 此字段无意义; UserDefined, 则此字段传入用户自定义会话保持String. 若无此字段则不做修改
         - **PersistenceType** (str) - VServer会话保持模式，若无此字段则不做修改。枚举值：None：关闭；ServerInsert：自动生成KEY；UserDefined：用户自定义KEY。
         - **Protocol** (str) - VServer协议类型，请求代理只支持修改为 HTTP/HTTPS，报文转发VServer只支持修改为 TCP/UDP
         - **VServerName** (str) - VServer实例名称，若无此字段则不做修改
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateVServerAttributeRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateVServerAttribute", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ulb/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ulb/schemas/apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: AllocateBackend
 
 添加ULB后端资源实例
 """
 
 
 class AllocateBackendRequestSchema(schema.RequestSchema):
-    """ AllocateBackend - 添加ULB后端资源实例
-    """
+    """AllocateBackend - 添加ULB后端资源实例"""
 
     fields = {
         "Enabled": fields.Int(required=False, dump_to="Enabled"),
         "Port": fields.Int(required=False, dump_to="Port"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceId": fields.Str(required=True, dump_to="ResourceId"),
@@ -29,44 +28,41 @@
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
         "Weight": fields.Int(required=False, dump_to="Weight"),
     }
 
 
 class AllocateBackendResponseSchema(schema.ResponseSchema):
-    """ AllocateBackend - 添加ULB后端资源实例
-    """
+    """AllocateBackend - 添加ULB后端资源实例"""
 
     fields = {"BackendId": fields.Str(required=False, load_from="BackendId")}
 
 
 """
 API: AllocateBackendBatch
 
 批量添加VServer后端节点
 """
 
 
 class AllocateBackendBatchRequestSchema(schema.RequestSchema):
-    """ AllocateBackendBatch - 批量添加VServer后端节点
-    """
+    """AllocateBackendBatch - 批量添加VServer后端节点"""
 
     fields = {
         "ApiVersion": fields.Int(required=False, dump_to="ApiVersion"),
         "Backends": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
     }
 
 
 class AllocateBackendBatchResponseSchema(schema.ResponseSchema):
-    """ AllocateBackendBatch - 批量添加VServer后端节点
-    """
+    """AllocateBackendBatch - 批量添加VServer后端节点"""
 
     fields = {
         "BackendSet": fields.List(
             models.BackendSetSchema(), required=False, load_from="BackendSet"
         )
     }
 
@@ -75,102 +71,95 @@
 API: BindSSL
 
 将SSL证书绑定到VServer
 """
 
 
 class BindSSLRequestSchema(schema.RequestSchema):
-    """ BindSSL - 将SSL证书绑定到VServer
-    """
+    """BindSSL - 将SSL证书绑定到VServer"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SSLId": fields.Str(required=True, dump_to="SSLId"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
     }
 
 
 class BindSSLResponseSchema(schema.ResponseSchema):
-    """ BindSSL - 将SSL证书绑定到VServer
-    """
+    """BindSSL - 将SSL证书绑定到VServer"""
 
     fields = {}
 
 
 """
 API: CreatePolicy
 
 创建VServer内容转发策略
 """
 
 
 class CreatePolicyRequestSchema(schema.RequestSchema):
-    """ CreatePolicy - 创建VServer内容转发策略
-    """
+    """CreatePolicy - 创建VServer内容转发策略"""
 
     fields = {
         "BackendId": fields.List(fields.Str()),
         "Match": fields.Str(required=True, dump_to="Match"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Type": fields.Str(required=False, dump_to="Type"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
     }
 
 
 class CreatePolicyResponseSchema(schema.ResponseSchema):
-    """ CreatePolicy - 创建VServer内容转发策略
-    """
+    """CreatePolicy - 创建VServer内容转发策略"""
 
     fields = {"PolicyId": fields.Str(required=False, load_from="PolicyId")}
 
 
 """
 API: CreateSSL
 
 创建SSL证书，可以把整个 Pem 证书内容传过来，或者把证书、私钥、CA证书分别传过来
 """
 
 
 class CreateSSLRequestSchema(schema.RequestSchema):
-    """ CreateSSL - 创建SSL证书，可以把整个 Pem 证书内容传过来，或者把证书、私钥、CA证书分别传过来
-    """
+    """CreateSSL - 创建SSL证书，可以把整个 Pem 证书内容传过来，或者把证书、私钥、CA证书分别传过来"""
 
     fields = {
         "CaCert": fields.Str(required=False, dump_to="CaCert"),
         "PrivateKey": fields.Str(required=False, dump_to="PrivateKey"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SSLContent": fields.Str(required=False, dump_to="SSLContent"),
         "SSLName": fields.Str(required=True, dump_to="SSLName"),
         "SSLType": fields.Str(required=False, dump_to="SSLType"),
         "UserCert": fields.Str(required=False, dump_to="UserCert"),
     }
 
 
 class CreateSSLResponseSchema(schema.ResponseSchema):
-    """ CreateSSL - 创建SSL证书，可以把整个 Pem 证书内容传过来，或者把证书、私钥、CA证书分别传过来
-    """
+    """CreateSSL - 创建SSL证书，可以把整个 Pem 证书内容传过来，或者把证书、私钥、CA证书分别传过来"""
 
     fields = {"SSLId": fields.Str(required=False, load_from="SSLId")}
 
 
 """
 API: CreateULB
 
 创建负载均衡实例，可以选择内网或者外网
 """
 
 
 class CreateULBRequestSchema(schema.RequestSchema):
-    """ CreateULB - 创建负载均衡实例，可以选择内网或者外网
-    """
+    """CreateULB - 创建负载均衡实例，可以选择内网或者外网"""
 
     fields = {
         "BusinessId": fields.Str(required=False, dump_to="BusinessId"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "IPVersion": fields.Str(required=False, dump_to="IPVersion"),
         "InnerMode": fields.Str(required=False, dump_to="InnerMode"),
         "ListenType": fields.Str(required=False, dump_to="ListenType"),
@@ -183,30 +172,28 @@
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "ULBName": fields.Str(required=False, dump_to="ULBName"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
     }
 
 
 class CreateULBResponseSchema(schema.ResponseSchema):
-    """ CreateULB - 创建负载均衡实例，可以选择内网或者外网
-    """
+    """CreateULB - 创建负载均衡实例，可以选择内网或者外网"""
 
     fields = {"ULBId": fields.Str(required=False, load_from="ULBId")}
 
 
 """
 API: CreateVServer
 
 创建VServer实例，定义监听的协议和端口以及负载均衡算法
 """
 
 
 class CreateVServerRequestSchema(schema.RequestSchema):
-    """ CreateVServer - 创建VServer实例，定义监听的协议和端口以及负载均衡算法
-    """
+    """CreateVServer - 创建VServer实例，定义监听的协议和端口以及负载均衡算法"""
 
     fields = {
         "ClientTimeout": fields.Int(required=False, dump_to="ClientTimeout"),
         "Domain": fields.Str(required=False, dump_to="Domain"),
         "FrontendPort": fields.Int(required=False, dump_to="FrontendPort"),
         "ListenType": fields.Str(required=False, dump_to="ListenType"),
         "Method": fields.Str(required=False, dump_to="Method"),
@@ -223,147 +210,136 @@
         "Region": fields.Str(required=True, dump_to="Region"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerName": fields.Str(required=False, dump_to="VServerName"),
     }
 
 
 class CreateVServerResponseSchema(schema.ResponseSchema):
-    """ CreateVServer - 创建VServer实例，定义监听的协议和端口以及负载均衡算法
-    """
+    """CreateVServer - 创建VServer实例，定义监听的协议和端口以及负载均衡算法"""
 
     fields = {"VServerId": fields.Str(required=False, load_from="VServerId")}
 
 
 """
 API: DeletePolicy
 
 删除内容转发策略
 """
 
 
 class DeletePolicyRequestSchema(schema.RequestSchema):
-    """ DeletePolicy - 删除内容转发策略
-    """
+    """DeletePolicy - 删除内容转发策略"""
 
     fields = {
         "GroupId": fields.Str(required=False, dump_to="GroupId"),
         "PolicyId": fields.Str(required=True, dump_to="PolicyId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VServerId": fields.Str(required=False, dump_to="VServerId"),
     }
 
 
 class DeletePolicyResponseSchema(schema.ResponseSchema):
-    """ DeletePolicy - 删除内容转发策略
-    """
+    """DeletePolicy - 删除内容转发策略"""
 
     fields = {}
 
 
 """
 API: DeleteSSL
 
 删除SSL证书
 """
 
 
 class DeleteSSLRequestSchema(schema.RequestSchema):
-    """ DeleteSSL - 删除SSL证书
-    """
+    """DeleteSSL - 删除SSL证书"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SSLId": fields.Str(required=True, dump_to="SSLId"),
     }
 
 
 class DeleteSSLResponseSchema(schema.ResponseSchema):
-    """ DeleteSSL - 删除SSL证书
-    """
+    """DeleteSSL - 删除SSL证书"""
 
     fields = {}
 
 
 """
 API: DeleteULB
 
 删除负载均衡实例
 """
 
 
 class DeleteULBRequestSchema(schema.RequestSchema):
-    """ DeleteULB - 删除负载均衡实例
-    """
+    """DeleteULB - 删除负载均衡实例"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ReleaseEip": fields.Bool(required=False, dump_to="ReleaseEip"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
     }
 
 
 class DeleteULBResponseSchema(schema.ResponseSchema):
-    """ DeleteULB - 删除负载均衡实例
-    """
+    """DeleteULB - 删除负载均衡实例"""
 
     fields = {}
 
 
 """
 API: DeleteVServer
 
 删除VServer实例
 """
 
 
 class DeleteVServerRequestSchema(schema.RequestSchema):
-    """ DeleteVServer - 删除VServer实例
-    """
+    """DeleteVServer - 删除VServer实例"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
     }
 
 
 class DeleteVServerResponseSchema(schema.ResponseSchema):
-    """ DeleteVServer - 删除VServer实例
-    """
+    """DeleteVServer - 删除VServer实例"""
 
     fields = {}
 
 
 """
 API: DescribeSSL
 
 获取SSL证书信息
 """
 
 
 class DescribeSSLRequestSchema(schema.RequestSchema):
-    """ DescribeSSL - 获取SSL证书信息
-    """
+    """DescribeSSL - 获取SSL证书信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SSLId": fields.Str(required=False, dump_to="SSLId"),
     }
 
 
 class DescribeSSLResponseSchema(schema.ResponseSchema):
-    """ DescribeSSL - 获取SSL证书信息
-    """
+    """DescribeSSL - 获取SSL证书信息"""
 
     fields = {
         "DataSet": fields.List(
             models.ULBSSLSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -373,32 +349,30 @@
 API: DescribeULB
 
 获取ULB详细信息
 """
 
 
 class DescribeULBRequestSchema(schema.RequestSchema):
-    """ DescribeULB - 获取ULB详细信息
-    """
+    """DescribeULB - 获取ULB详细信息"""
 
     fields = {
         "BusinessId": fields.Str(required=False, dump_to="BusinessId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetId": fields.Str(required=False, dump_to="SubnetId"),
         "ULBId": fields.Str(required=False, dump_to="ULBId"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
     }
 
 
 class DescribeULBResponseSchema(schema.ResponseSchema):
-    """ DescribeULB - 获取ULB详细信息
-    """
+    """DescribeULB - 获取ULB详细信息"""
 
     fields = {
         "DataSet": fields.List(
             models.ULBSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -408,30 +382,28 @@
 API: DescribeVServer
 
 获取ULB下的VServer的详细信息
 """
 
 
 class DescribeVServerRequestSchema(schema.RequestSchema):
-    """ DescribeVServer - 获取ULB下的VServer的详细信息
-    """
+    """DescribeVServer - 获取ULB下的VServer的详细信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=False, dump_to="VServerId"),
     }
 
 
 class DescribeVServerResponseSchema(schema.ResponseSchema):
-    """ DescribeVServer - 获取ULB下的VServer的详细信息
-    """
+    """DescribeVServer - 获取ULB下的VServer的详细信息"""
 
     fields = {
         "DataSet": fields.List(
             models.ULBVServerSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -441,156 +413,145 @@
 API: ReleaseBackend
 
 从VServer释放后端资源实例
 """
 
 
 class ReleaseBackendRequestSchema(schema.RequestSchema):
-    """ ReleaseBackend - 从VServer释放后端资源实例
-    """
+    """ReleaseBackend - 从VServer释放后端资源实例"""
 
     fields = {
         "BackendId": fields.Str(required=True, dump_to="BackendId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
     }
 
 
 class ReleaseBackendResponseSchema(schema.ResponseSchema):
-    """ ReleaseBackend - 从VServer释放后端资源实例
-    """
+    """ReleaseBackend - 从VServer释放后端资源实例"""
 
     fields = {}
 
 
 """
 API: UnbindSSL
 
 从VServer解绑SSL证书
 """
 
 
 class UnbindSSLRequestSchema(schema.RequestSchema):
-    """ UnbindSSL - 从VServer解绑SSL证书
-    """
+    """UnbindSSL - 从VServer解绑SSL证书"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SSLId": fields.Str(required=True, dump_to="SSLId"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
     }
 
 
 class UnbindSSLResponseSchema(schema.ResponseSchema):
-    """ UnbindSSL - 从VServer解绑SSL证书
-    """
+    """UnbindSSL - 从VServer解绑SSL证书"""
 
     fields = {}
 
 
 """
 API: UpdateBackendAttribute
 
 更新ULB后端资源实例(服务节点)属性
 """
 
 
 class UpdateBackendAttributeRequestSchema(schema.RequestSchema):
-    """ UpdateBackendAttribute - 更新ULB后端资源实例(服务节点)属性
-    """
+    """UpdateBackendAttribute - 更新ULB后端资源实例(服务节点)属性"""
 
     fields = {
         "BackendId": fields.Str(required=True, dump_to="BackendId"),
         "Enabled": fields.Int(required=False, dump_to="Enabled"),
         "Port": fields.Int(required=False, dump_to="Port"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "Weight": fields.Int(required=False, dump_to="Weight"),
     }
 
 
 class UpdateBackendAttributeResponseSchema(schema.ResponseSchema):
-    """ UpdateBackendAttribute - 更新ULB后端资源实例(服务节点)属性
-    """
+    """UpdateBackendAttribute - 更新ULB后端资源实例(服务节点)属性"""
 
     fields = {}
 
 
 """
 API: UpdatePolicy
 
 更新内容转发规则，包括转发规则后的服务节点
 """
 
 
 class UpdatePolicyRequestSchema(schema.RequestSchema):
-    """ UpdatePolicy - 更新内容转发规则，包括转发规则后的服务节点
-    """
+    """UpdatePolicy - 更新内容转发规则，包括转发规则后的服务节点"""
 
     fields = {
         "BackendId": fields.List(fields.Str()),
         "Match": fields.Str(required=True, dump_to="Match"),
         "PolicyId": fields.Str(required=True, dump_to="PolicyId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Type": fields.Str(required=False, dump_to="Type"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
     }
 
 
 class UpdatePolicyResponseSchema(schema.ResponseSchema):
-    """ UpdatePolicy - 更新内容转发规则，包括转发规则后的服务节点
-    """
+    """UpdatePolicy - 更新内容转发规则，包括转发规则后的服务节点"""
 
     fields = {"PolicyId": fields.Str(required=False, load_from="PolicyId")}
 
 
 """
 API: UpdateULBAttribute
 
 更新ULB名字业务组备注等属性字段
 """
 
 
 class UpdateULBAttributeRequestSchema(schema.RequestSchema):
-    """ UpdateULBAttribute - 更新ULB名字业务组备注等属性字段
-    """
+    """UpdateULBAttribute - 更新ULB名字业务组备注等属性字段"""
 
     fields = {
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
     }
 
 
 class UpdateULBAttributeResponseSchema(schema.ResponseSchema):
-    """ UpdateULBAttribute - 更新ULB名字业务组备注等属性字段
-    """
+    """UpdateULBAttribute - 更新ULB名字业务组备注等属性字段"""
 
     fields = {}
 
 
 """
 API: UpdateVServerAttribute
 
 更新VServer实例属性
 """
 
 
 class UpdateVServerAttributeRequestSchema(schema.RequestSchema):
-    """ UpdateVServerAttribute - 更新VServer实例属性
-    """
+    """UpdateVServerAttribute - 更新VServer实例属性"""
 
     fields = {
         "ClientTimeout": fields.Int(required=False, dump_to="ClientTimeout"),
         "Domain": fields.Str(required=False, dump_to="Domain"),
         "Method": fields.Str(required=False, dump_to="Method"),
         "MonitorType": fields.Str(required=False, dump_to="MonitorType"),
         "Path": fields.Str(required=False, dump_to="Path"),
@@ -606,11 +567,10 @@
         "ULBId": fields.Str(required=True, dump_to="ULBId"),
         "VServerId": fields.Str(required=True, dump_to="VServerId"),
         "VServerName": fields.Str(required=False, dump_to="VServerName"),
     }
 
 
 class UpdateVServerAttributeResponseSchema(schema.ResponseSchema):
-    """ UpdateVServerAttribute - 更新VServer实例属性
-    """
+    """UpdateVServerAttribute - 更新VServer实例属性"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/ulb/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/ulb/schemas/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class BackendSetSchema(schema.ResponseSchema):
-    """ BackendSet - ulb添加rs时返回的信息
-    """
+    """BackendSet - ulb添加rs时返回的信息"""
 
     fields = {
         "BackendId": fields.Str(required=True, load_from="BackendId"),
         "ResourceId": fields.Str(required=True, load_from="ResourceId"),
     }
 
 
 class ULBSSLSetSchema(schema.ResponseSchema):
-    """ ULBSSLSet - DescribeULB
-    """
+    """ULBSSLSet - DescribeULB"""
 
     fields = {
         "HashValue": fields.Str(required=False, load_from="HashValue"),
         "SSLId": fields.Str(required=False, load_from="SSLId"),
         "SSLName": fields.Str(required=False, load_from="SSLName"),
     }
 
 
 class PolicyBackendSetSchema(schema.ResponseSchema):
-    """ PolicyBackendSet - 内容转发下rs详细信息
-    """
+    """PolicyBackendSet - 内容转发下rs详细信息"""
 
     fields = {
         "BackendId": fields.Str(required=False, load_from="BackendId"),
         "ObjectId": fields.Str(required=False, load_from="ObjectId"),
         "Port": fields.Int(required=False, load_from="Port"),
         "PrivateIP": fields.Str(required=False, load_from="PrivateIP"),
         "ResourceName": fields.Str(required=False, load_from="ResourceName"),
     }
 
 
 class ULBBackendSetSchema(schema.ResponseSchema):
-    """ ULBBackendSet - DescribeULB
-    """
+    """ULBBackendSet - DescribeULB"""
 
     fields = {
         "BackendId": fields.Str(required=False, load_from="BackendId"),
         "Enabled": fields.Int(required=False, load_from="Enabled"),
         "Port": fields.Int(required=False, load_from="Port"),
         "PrivateIP": fields.Str(required=False, load_from="PrivateIP"),
         "ResourceId": fields.Str(required=False, load_from="ResourceId"),
@@ -59,16 +55,15 @@
         ),
         "SubnetId": fields.Str(required=False, load_from="SubnetId"),
         "Weight": fields.Int(required=False, load_from="Weight"),
     }
 
 
 class ULBPolicySetSchema(schema.ResponseSchema):
-    """ ULBPolicySet - 内容转发详细列表
-    """
+    """ULBPolicySet - 内容转发详细列表"""
 
     fields = {
         "BackendSet": fields.List(PolicyBackendSetSchema()),
         "Match": fields.Str(required=False, load_from="Match"),
         "PolicyId": fields.Str(required=False, load_from="PolicyId"),
         "PolicyPriority": fields.Int(
             required=False, load_from="PolicyPriority"
@@ -77,16 +72,15 @@
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
         "Type": fields.Str(required=False, load_from="Type"),
         "VServerId": fields.Str(required=False, load_from="VServerId"),
     }
 
 
 class ULBVServerSetSchema(schema.ResponseSchema):
-    """ ULBVServerSet - DescribeULB
-    """
+    """ULBVServerSet - DescribeULB"""
 
     fields = {
         "BackendSet": fields.List(ULBBackendSetSchema()),
         "ClientTimeout": fields.Int(required=False, load_from="ClientTimeout"),
         "Domain": fields.Str(required=True, load_from="Domain"),
         "FrontendPort": fields.Int(required=False, load_from="FrontendPort"),
         "ListenType": fields.Str(required=False, load_from="ListenType"),
@@ -105,29 +99,27 @@
         "Status": fields.Int(required=False, load_from="Status"),
         "VServerId": fields.Str(required=False, load_from="VServerId"),
         "VServerName": fields.Str(required=False, load_from="VServerName"),
     }
 
 
 class ULBIPSetSchema(schema.ResponseSchema):
-    """ ULBIPSet - DescribeULB
-    """
+    """ULBIPSet - DescribeULB"""
 
     fields = {
         "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
         "BandwidthType": fields.Int(required=False, load_from="BandwidthType"),
         "EIP": fields.Str(required=False, load_from="EIP"),
         "EIPId": fields.Str(required=False, load_from="EIPId"),
         "OperatorName": fields.Str(required=False, load_from="OperatorName"),
     }
 
 
 class ULBSetSchema(schema.ResponseSchema):
-    """ ULBSet - DescribeULB
-    """
+    """ULBSet - DescribeULB"""
 
     fields = {
         "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
         "BandwidthType": fields.Int(required=False, load_from="BandwidthType"),
         "BusinessId": fields.Str(required=False, load_from="BusinessId"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/umem/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/umem/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,545 +9,800 @@
 
 class UMemClient(Client):
     def __init__(
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UMemClient, self).__init__(config, transport, middleware, logger)
 
+    def create_umem_backup(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """CreateUMemBackup - 创建分布式redis备份
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **BackupName** (str) - (Required) 请求创建备份的名称 (范围[6-63],只能包含英文、数字以及符号-和_)
+        - **SpaceId** (str) - (Required) 资源id
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
+        **Response**
+
+        - **BackupId** (str) - 备份Id
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.CreateUMemBackupRequestSchema().dumps(d)
+
+        # build options
+        kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
+
+        resp = self.invoke("CreateUMemBackup", d, **kwargs)
+        return apis.CreateUMemBackupResponseSchema().loads(resp)
+
     def create_umem_space(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUMemSpace - 创建UMem内存空间
+        """CreateUMemSpace - 创建UMem内存空间
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 空间名称,长度(6<=size<=63)
         - **Size** (int) - (Required) 内存大小, 单位:GB, 范围[1~1024]
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - Year , Month, Dynamic, Trial 默认: Month
         - **CouponId** (str) - 使用的代金券id
-        - **Password** (str) - URedis密码。请遵照 `字段规范 <https://docs.ucloud.cn/api/uhost-api/specification>`_ 设定密码。密码需使用base64进行编码，举例如下：# echo -n Password1 | base64UGFzc3dvcmQx。
         - **Protocol** (str) - 协议:memcache, redis (默认redis).注意:redis无single类型
         - **Quantity** (int) - 购买时长 默认: 1
-        - **SubnetId** (str) - 
-        - **Tag** (str) - 
+        - **SubnetId** (str) -
         - **Type** (str) - 空间类型:single(无热备),double(热备)(默认: double)
-        - **VPCId** (str) - 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **VPCId** (str) -
+
         **Response**
 
         - **SpaceId** (str) - 创建内存空间ID列表
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.CreateUMemSpaceRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreateUMemSpace", d, **kwargs)
         return apis.CreateUMemSpaceResponseSchema().loads(resp)
 
     def create_umem_cache_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUMemcacheGroup - 创建单机Memcache
+        """CreateUMemcacheGroup - 创建单机Memcache
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 请求创建组的名称 范围[6-60]
         - **ChargeType** (str) - 计费模式，Year , Month, Dynamic 默认: Month
         - **ConfigId** (str) - 配置ID,目前仅支持默认配置id 默认配置id:"9a891891-c245-4b66-bce8-67e59430d67c"
         - **CouponId** (str) - 代金券ID
-        - **Protocol** (str) - 
+        - **Protocol** (str) -
         - **Quantity** (int) - 购买时长，默认为1
         - **Size** (int) - 每个节点的内存大小,单位GB,默认1GB 目前仅支持1/2/4/8/16/32这几档
-        - **SubnetId** (str) - 
+        - **SubnetId** (str) -
         - **Tag** (str) - 业务组 默认：Default
-        - **VPCId** (str) - 
+        - **VPCId** (str) -
         - **Version** (str) - Memcache版本信息,默认为1.4.31
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **GroupId** (str) - 创建的组ID
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.CreateUMemcacheGroupRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreateUMemcacheGroup", d, **kwargs)
         return apis.CreateUMemcacheGroupResponseSchema().loads(resp)
 
+    def create_uredis_backup(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """CreateURedisBackup - 创建主备Redis备份
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **BackupName** (str) - (Required) 请求创建组的名称 (范围[6-63],只能包含英文、数字以及符号-和_)
+        - **GroupId** (str) - (Required) 资源id
+        - **SlaveZone** (str) - 跨机房URedis，slave所在可用区（必须和Zone在同一Region，且不可相同）
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
+        **Response**
+
+        - **BackupId** (str) - 备份id
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.CreateURedisBackupRequestSchema().dumps(d)
+
+        # build options
+        kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
+
+        resp = self.invoke("CreateURedisBackup", d, **kwargs)
+        return apis.CreateURedisBackupResponseSchema().loads(resp)
+
     def create_uredis_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateURedisGroup - 创建主备redis
+        """CreateURedisGroup - 创建主备redis
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **HighAvailability** (str) - (Required) 是否开启高可用,enable或disable
         - **Name** (str) - (Required) 请求创建组的名称 (范围[6-63],只能包含英文、数字以及符号-和_)
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **AutoBackup** (str) - 是否自动备份,enable或disable，默认disable
         - **BackupId** (str) - 有此项代表从备份中创建，无代表正常创建
         - **BackupTime** (int) - 自动备份开始时间,范围[0-23],默认3点
         - **ChargeType** (str) - 计费模式，Year , Month, Dynamic 默认: Month
         - **ConfigId** (str) - 配置ID,目前支持 3.0版本配置ID:"03f58ca9-b64d-4bdd-abc7-c6b9a46fd801",3.2版本配置ID:"3e45ac48-f8a2-a9q2-261d-l342dab130gf", 4.0版本配置ID:"6c9298a3-9d7f-428c-b1d0-e87ab3b8a1ea",默认版本3.0,从备份创建为必传项
         - **CouponId** (str) - 代金券ID
+        - **EnableIpV6** (bool) - 是否创建使用ipv6 资源， 默认为false， 或者不填， 创建ipv6为true
         - **MasterGroupId** (str) - Master Redis Group的ID，创建只读Slave时，必须填写
         - **Password** (str) - 初始化密码,需要 base64 编码
         - **Quantity** (int) - 购买时长，默认为1
         - **Size** (int) - 每个节点的内存大小,单位GB,默认1GB,目前仅支持1/2/4/8/16/32,六种
         - **SlaveZone** (str) - 跨机房URedis，slave所在可用区（必须和Zone在同一Region，且不可相同）
-        - **SubnetId** (str) - 
+        - **SubnetId** (str) - 子网ID
         - **Tag** (str) - 业务组名称
-        - **VPCId** (str) - 
+        - **VPCId** (str) - VPC的ID
         - **Version** (str) - Redis版本信息(详见DescribeURedisVersion返回结果),默认版本3.0
-        
+
         **Response**
 
         - **GroupId** (str) - 创建的组ID
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.CreateURedisGroupRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreateURedisGroup", d, **kwargs)
         return apis.CreateURedisGroupResponseSchema().loads(resp)
 
     def delete_umem_space(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUMemSpace - 删除UMem内存空间
+        """DeleteUMemSpace - 删除UMem内存空间
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SpaceId** (str) - (Required) UMem内存空间ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DeleteUMemSpaceRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUMemSpace", d, **kwargs)
         return apis.DeleteUMemSpaceResponseSchema().loads(resp)
 
     def delete_umem_cache_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUMemcacheGroup - 删除单机Memcache
+        """DeleteUMemcacheGroup - 删除单机Memcache
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - (Required) 组ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DeleteUMemcacheGroupRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUMemcacheGroup", d, **kwargs)
         return apis.DeleteUMemcacheGroupResponseSchema().loads(resp)
 
     def delete_uredis_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteURedisGroup - 删除主备redis
+        """DeleteURedisGroup - 删除主备redis
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - (Required) 组ID
-        
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DeleteURedisGroupRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteURedisGroup", d, **kwargs)
         return apis.DeleteURedisGroupResponseSchema().loads(resp)
 
+    def describe_umem_backup(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """DescribeUMemBackup - 查询分布式redis备份
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **SpaceId** (str) - (Required) 资源id
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Limit** (int) - 分页显示的条目数, 默认值为10
+        - **Offset** (int) - 分页显示的起始偏移, 默认值为0
+
+        **Response**
+
+        - **DataSet** (list) - 见 **UMemBackupSet** 模型定义
+
+        **Response Model**
+
+        **UMemBackupSet**
+
+        - **BackupId** (str) - 空间的备份ID
+        - **BackupName** (str) - 备份名称
+        - **BackupType** (str) - 备份类型: auto(自动) ,manual(手动)
+        - **BlockCount** (int) - 本次备份，分片的数量
+        - **CreateTime** (int) - 创建时间
+        - **State** (str) - Starting:备份中 Done:完成
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.DescribeUMemBackupRequestSchema().dumps(d)
+
+        resp = self.invoke("DescribeUMemBackup", d, **kwargs)
+        return apis.DescribeUMemBackupResponseSchema().loads(resp)
+
+    def describe_umem_backup_url(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """DescribeUMemBackupURL - 获取分布式redis 备份下载链接
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **BackupId** (str) - (Required) 备份Id
+        - **SpaceId** (str) - (Required) 资源id
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **BlockId** (str) - 分片id
+
+        **Response**
+
+        - **BackupURL** (list) - 备份url，每个分片一个下载URL
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.DescribeUMemBackupURLRequestSchema().dumps(d)
+
+        resp = self.invoke("DescribeUMemBackupURL", d, **kwargs)
+        return apis.DescribeUMemBackupURLResponseSchema().loads(resp)
+
+    def describe_umem_block_info(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """DescribeUMemBlockInfo - 拉取UDRedis分片信息
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Limit** (int) - (Required) 分页显示的条目数, 默认值为10
+        - **Offset** (int) - (Required) 分页显示的起始偏移, 默认值为0
+        - **SpaceId** (str) - (Required) UMem内存资源ID
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
+        **Response**
+
+        - **DataSet** (list) - 见 **UMemBlockInfo** 模型定义
+
+        **Response Model**
+
+        **UMemBlockInfo**
+
+        - **BlockId** (str) - 分片id
+        - **BlockPort** (int) - 分片端口
+        - **BlockSize** (int) - 容量单位GB
+        - **BlockSlotBegin** (int) - 分片维护的键槽起始值
+        - **BlockSlotEnd** (int) - 分片维护的键槽结束值
+        - **BlockState** (str) - 实例状态 Starting // 创建中 Creating // 初始化中 CreateFail // 创建失败 Fail // 创建失败 Deleting // 删除中 DeleteFail // 删除失败 Running // 运行 Resizing // 容量调整中 ResizeFail // 容量调整失败 Configing // 配置中 ConfigFail // 配置失败Restarting // 重启中 SetPasswordFail //设置密码失败
+        - **BlockUsedSize** (int) - 使用量单位MB
+        - **BlockVip** (str) - 分片ip
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.DescribeUMemBlockInfoRequestSchema().dumps(d)
+
+        resp = self.invoke("DescribeUMemBlockInfo", d, **kwargs)
+        return apis.DescribeUMemBlockInfoResponseSchema().loads(resp)
+
     def describe_umem_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUMemPrice - 获取UMem实例价格信息
+        """DescribeUMemPrice - 获取UMem实例价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 购买umem大小,单位:GB,范围[1~1024]
         - **Type** (str) - (Required) 空间类型:single(无热备),double(热备)(默认: double)
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **ChargeType** (str) - Year， Month， Dynamic，Trial 如果不指定，则一次性获取三种计费
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **ChargeType** (str) - Year， Month， Dynamic 如果不指定，则一次性获取三种计费
         - **Quantity** (int) - 购买UMem的时长，默认值为1
-        - **RegionFlag** (bool) - 
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UMemPriceSet** 模型定义
-        
+
         **Response Model**
-        
-        **UMemPriceSet** 
-        
+
+        **UMemPriceSet**
+
         - **ChargeType** (str) - Year， Month， Dynamic，Trial
+        - **ListPrice** (int) - 产品列表价
         - **OriginalPrice** (int) - 原价
-        - **Price** (int) - 现价，单位: 元，保留小数点后两位有效数字
+        - **Price** (int) - 现价
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeUMemPriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUMemPrice", d, **kwargs)
         return apis.DescribeUMemPriceResponseSchema().loads(resp)
 
     def describe_umem_space(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUMemSpace - 获取UMem内存空间列表
+        """DescribeUMemSpace - 获取UMem内存空间列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 返回数据长度, 默认为20
         - **Offset** (int) - 数据偏移量, 默认为0
+        - **Protocol** (str) - 协议类型: memcache, redis
         - **SpaceId** (str) - 内存空间ID (无ID，则获取所有)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UMemSpaceSet** 模型定义
         - **TotalCount** (int) - 根据过滤条件得到的总数
-        
+
         **Response Model**
-        
-        **UMemSpaceAddressSet** 
-        
+
+        **UMemSpaceAddressSet**
+
         - **IP** (str) - UMem实例访问IP
         - **Port** (int) - UMem实例访问Port
 
-        **UMemSpaceSet** 
-        
+        **UMemSpaceSet**
+
         - **Address** (list) - 见 **UMemSpaceAddressSet** 模型定义
         - **ChargeType** (str) - Year, Month, Dynamic, Trial
         - **CreateTime** (int) - 创建时间
         - **ExpireTime** (int) - 到期时间
         - **Name** (str) - 内存空间名称
         - **Protocol** (str) - 协议类型: memcache, redis
         - **RewriteTime** (int) - 运维时间0   //0点1   //1点依次类推
         - **Size** (int) - 容量单位GB
         - **SpaceId** (str) - 内存空间ID
         - **State** (str) - Starting:创建中 Running:运行中 Fail:失败
-        - **SubnetId** (str) - 
-        - **Tag** (str) - 
+        - **SubnetId** (str) -
+        - **Tag** (str) -
         - **Type** (str) - 空间类型:single(无热备),double(热备)
         - **UsedSize** (int) - 使用量单位MB
-        - **VPCId** (str) - 
-        - **Zone** (str) - 可用区，参见 `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **VPCId** (str) -
+        - **Zone** (str) - 可用区，参见 `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeUMemSpaceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUMemSpace", d, **kwargs)
         return apis.DescribeUMemSpaceResponseSchema().loads(resp)
 
     def describe_umem_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUMemUpgradePrice - 获取UMem升级价格信息
+        """DescribeUMemUpgradePrice - 获取UMem升级价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 购买UMem大小,单位:GB
         - **SpaceId** (str) - (Required) 需要升级的空间的SpaceId
         - **Type** (str) - (Required) 空间类型:single(无热备),double(热备)(默认: double)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (dict) - 见 **PriceDataSet** 模型定义
         - **Price** (int) - 价格(兼容老版本)
-        
+
         **Response Model**
-        
-        **PriceDataSet** 
-        
+
+        **PriceDataSet**
+
         - **CustomPrice** (int) - 用户折后价
         - **PurchaseValue** (int) - 资源有效期
         - **TotalPrice** (int) - 升降级资源的价格
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeUMemUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUMemUpgradePrice", d, **kwargs)
         return apis.DescribeUMemUpgradePriceResponseSchema().loads(resp)
 
     def describe_umem_cache_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUMemcacheGroup - 显示Memcache
+        """DescribeUMemcacheGroup - 显示Memcache
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - 组的ID,如果指定则获取描述，否则为列表操 作,需指定Offset/Limit
         - **Limit** (int) - 分页显示的条目数, 默认值为20
         - **Offset** (int) - 分页显示的起始偏移, 默认值为0
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **UMemcacheGroupSet** 模型定义
         - **TotalCount** (int) - 组的总的节点个数
-        
+
         **Response Model**
-        
-        **UMemcacheGroupSet** 
-        
+
+        **UMemcacheGroupSet**
+
         - **ChargeType** (str) - 计费类型:Year,Month,Dynamic 默认Dynamic
         - **ConfigId** (str) - 节点的配置ID
         - **CreateTime** (int) - 创建时间 (UNIX时间戳)
         - **ExpireTime** (int) - 过期时间 (UNIX时间戳)
         - **GroupId** (str) - 组ID
         - **ModifyTime** (int) - 修改时间 (UNIX时间戳)
         - **Name** (str) - 组名称
         - **Port** (int) - 节点分配的服务端口
         - **Size** (int) - 容量单位GB
         - **State** (str) - 状态标记 Creating // 初始化中 CreateFail // 创建失败 Deleting // 删除中 DeleteFail // 删除失败 Running // 运行 Resizing // 容量调整中 ResizeFail // 容量调整失败 Configing // 配置中 ConfigFail // 配置失败Restarting // 重启中
-        - **SubnetId** (str) - 
+        - **SubnetId** (str) -
         - **Tag** (str) - 业务组名称
         - **UsedSize** (int) - 使用量单位MB
-        - **VPCId** (str) - 
+        - **VPCId** (str) -
         - **Version** (str) - Memcache版本信息,默认为1.4.31
         - **VirtualIP** (str) - 节点的虚拟IP地址
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeUMemcacheGroupRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUMemcacheGroup", d, **kwargs)
         return apis.DescribeUMemcacheGroupResponseSchema().loads(resp)
 
     def describe_umem_cache_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUMemcachePrice - 获取umemcache组价格信息
+        """DescribeUMemcachePrice - 获取umemcache组价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 容量大小,单位:GB 取值范围[1-32]
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - 计费模式，Year， Month， Dynamic，默认: Dynamic 默认: 获取所有计费模式的价格
         - **Quantity** (int) - 购买umemcache的时长，默认值为1
         - **Type** (str) - 空间类型:single(无热备),double(热备)(默认: double)
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UMemcachePriceSet** 模型定义
-        
+
         **Response Model**
-        
-        **UMemcachePriceSet** 
-        
+
+        **UMemcachePriceSet**
+
         - **ChargeType** (str) - 计费模式，Year, Month, Dynamic
+        - **ListPrice** (int) - 产品列表价
         - **OriginalPrice** (int) - 原价
-        - **Price** (int) - 总价格，单位: 元，保留小数点后两位有效数字
+        - **Price** (int) - 总价格
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeUMemcachePriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUMemcachePrice", d, **kwargs)
         return apis.DescribeUMemcachePriceResponseSchema().loads(resp)
 
     def describe_umem_cache_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeUMemcacheUpgradePrice - 获取umemcache升级价格信息
+        """DescribeUMemcacheUpgradePrice - 获取umemcache升级价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
         - **GroupId** (str) - (Required) 需要升级的空间的GroupId,请参考DescribeUMemcacheGroup接口
         - **Size** (int) - (Required) 购买umemcache大小,单位:GB
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+
         **Response**
 
-        - **DataSet** (dict) - 见 **PriceDataSet** 模型定义
-        - **Price** (int) - 价格，单位：元
-        
-        **Response Model**
-        
-        **PriceDataSet** 
-        
-        - **CustomPrice** (int) - 用户折后价
-        - **PurchaseValue** (int) - 资源有效期
-        - **TotalPrice** (int) - 升降级资源的价格
+        - **Price** (float) - 价格，单位：元
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {}
         req and d.update(req)
         d = apis.DescribeUMemcacheUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeUMemcacheUpgradePrice", d, **kwargs)
         return apis.DescribeUMemcacheUpgradePriceResponseSchema().loads(resp)
 
     def describe_uredis_backup(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeURedisBackup - 查询主备redis备份
+        """DescribeURedisBackup - 查询主备redis备份
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - 组的ID
         - **Limit** (int) - 分页显示的条目数, 默认值为10
         - **Offset** (int) - 分页显示的起始偏移, 默认值为0
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **URedisBackupSet** 模型定义
         - **TotalCount** (int) - 用户名下总的备份个数
-        
+
         **Response Model**
-        
-        **URedisBackupSet** 
-        
+
+        **URedisBackupSet**
+
         - **BackupId** (str) - 备份ID
         - **BackupName** (str) - 备份的名称
         - **BackupSize** (int) - 备份文件大小, 以字节为单位
         - **BackupTime** (int) - 备份时间 (UNIX时间戳)
         - **BackupType** (str) - 备份类型: Manual 手动 Auto 自动
         - **GroupId** (str) - 对应的实例ID
         - **GroupName** (str) - 组名称
         - **State** (str) - 备份的状态: Backuping 备份中 Success 备份成功 Error 备份失败 Expired 备份过期
-        - **Zone** (str) - 可用区，参见 `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - 可用区，参见 `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeURedisBackupRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeURedisBackup", d, **kwargs)
         return apis.DescribeURedisBackupResponseSchema().loads(resp)
 
     def describe_uredis_backup_url(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeURedisBackupURL - 获取主备Redis备份下载链接
+        """DescribeURedisBackupURL - 获取主备Redis备份下载链接
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BackupId** (str) - (Required) 备份ID
         - **GroupId** (str) - 实例名称
         - **RegionFlag** (bool) - 是否是跨机房URedis(默认false)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **SlaveZone** (str) - 跨机房URedis，slave所在可用区（必须和Zone在同一Region，且不可相同）
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **BackupPath** (str) - 备份文件公网的地址
         - **BackupURL** (str) - 备份文件公网的地址
-        - **InnerBackupPath** (str) - 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeURedisBackupURLRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeURedisBackupURL", d, **kwargs)
         return apis.DescribeURedisBackupURLResponseSchema().loads(resp)
 
+    def describe_uredis_config(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """DescribeURedisConfig - 查询主备Redis所有配置文件
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **RegionFlag** (bool) - (Required) 是否是跨机房URedis(默认false)
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **ConfigId** (str) - 配置文件ID
+        - **Limit** (int) - 页显示的条目数, 默认值为10
+        - **Offset** (int) - 页显示的起始偏移, 默认值为0
+        - **Version** (str) - Redis版本号
+
+        **Response**
+
+        - **DataSet** (list) - 见 **URedisConfigSet** 模型定义
+        - **TotalCount** (int) - 根据过滤条件得到的总数
+
+        **Response Model**
+
+        **URedisConfigSet**
+
+        - **ConfigId** (str) - 配置ID
+        - **CreateTime** (int) - 创建时间 (UNIX时间戳)
+        - **Description** (str) - 配置描述
+        - **IsModify** (str) - 置是否可以修改
+        - **ModifyTime** (int) - 修改时间 (UNIX时间戳)
+        - **Name** (str) - 配置名称
+        - **RegionFlag** (bool) - 是否是跨机房URedis(默认false)
+        - **State** (str) - 配置所处的状态
+        - **Version** (str) - 配置对应的Redis版本
+        - **Zone** (str) - Zone
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.DescribeURedisConfigRequestSchema().dumps(d)
+
+        resp = self.invoke("DescribeURedisConfig", d, **kwargs)
+        return apis.DescribeURedisConfigResponseSchema().loads(resp)
+
     def describe_uredis_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeURedisGroup - 查询主备Redis
+        """DescribeURedisGroup - 查询主备Redis
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - 组的ID,如果指定则获取描述，否则为列表操 作,需指定Offset/Limit
         - **Limit** (int) - 分页显示的条目数, 默认值为20
         - **Offset** (int) - 分页显示的起始偏移, 默认值为0
-        - **Zone** (str) - 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 见 **URedisGroupSet** 模型定义
         - **TotalCount** (int) - 组的总的节点个数
-        
+
         **Response Model**
-        
-        **URedisGroupSet** 
-        
+
+        **URedisGroupSet**
+
         - **AutoBackup** (str) - 是否需要自动备份,enable,disable
         - **BackupTime** (int) - 组自动备份开始时间,单位小时计,范围[0-23]
         - **ChargeType** (str) - 计费类型:Year,Month,Dynamic 默认Dynamic
         - **ConfigId** (str) - 节点的配置ID
         - **CreateTime** (int) - 创建时间 (UNIX时间戳)
         - **ExpireTime** (int) - 过期时间 (UNIX时间戳)
         - **GroupId** (str) - 组ID
@@ -555,282 +810,397 @@
         - **HighAvailability** (str) - 是否开启高可用,enable,disable
         - **MemorySize** (int) - 容量单位GB
         - **ModifyTime** (int) - 修改时间 (UNIX时间戳)
         - **Name** (str) - 组名称
         - **Port** (int) - 节点分配的服务端口
         - **Protocol** (str) - 协议
         - **RewriteTime** (int) - 返回运维时间 0 //0点 1 //1点 以此类推
+        - **Role** (str) - 实例类型
         - **Size** (int) - 容量单位GB
-        - **SlaveZone** (str) - 跨机房URedis，slave redis所在可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **SlaveZone** (str) - 跨机房URedis，slave redis所在可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **State** (str) - 状态标记 Creating // 初始化中 CreateFail // 创建失败 Deleting // 删除中 DeleteFail // 删除失败 Running // 运行 Resizing // 容量调整中 ResizeFail // 容量调整失败 Configing // 配置中 ConfigFail // 配置失败
-        - **SubnetId** (str) - 
+        - **SubnetId** (str) - 子网
         - **Tag** (str) - 业务组名称
-        - **Type** (str) - 
+        - **Type** (str) - 空间类型:single(无热备),double(热备)
         - **UsedSize** (int) - 使用量单位MB
-        - **VPCId** (str) - 
+        - **VPCId** (str) - VPCId
         - **Version** (str) - Redis版本信息
         - **VirtualIP** (str) - 节点的虚拟IP地址
-        - **Zone** (str) - 实例所在可用区，或者master redis所在可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - 实例所在可用区，或者master redis所在可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeURedisGroupRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeURedisGroup", d, **kwargs)
         return apis.DescribeURedisGroupResponseSchema().loads(resp)
 
     def describe_uredis_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeURedisPrice - 取uredis价格信息
+        """DescribeURedisPrice - 取uredis价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 量大小,单位:GB  取值范围[1-32]
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - 计费模式，Year， Month， Dynamic；如果不指定，则一次性获取三种计费
         - **ProductType** (str) - 产品类型：MS_Redis（标准主备版），S_Redis（从库），默认为MS_Redis
         - **Quantity** (int) - 计费模式为Dynamic时，购买的时长, 默认为1
         - **RegionFlag** (bool) - 是否是跨机房URedis(默认false)
-        - **Type** (str) - 
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **URedisPriceSet** 模型定义
-        
+
         **Response Model**
-        
-        **URedisPriceSet** 
-        
+
+        **URedisPriceSet**
+
         - **ChargeType** (str) - Year， Month， Dynamic，Trial
+        - **ListPrice** (int) - 产品列表价
         - **OriginalPrice** (int) - 原价
-        - **Price** (int) - 总价格，单位: 元，保留小数点后两位有效数字
+        - **Price** (int) - 总价格
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeURedisPriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeURedisPrice", d, **kwargs)
         return apis.DescribeURedisPriceResponseSchema().loads(resp)
 
+    def describe_uredis_slowlog(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """DescribeURedisSlowlog - 查询URedis慢日志
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **GroupId** (str) - (Required) 资源ID
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Limit** (int) - 分页显示的条目数，默认为10
+
+        **Response**
+
+        - **DataSet** (list) - 见 **URedisSlowlogSet** 模型定义
+        - **TotalCount** (int) - 总条目数
+
+        **Response Model**
+
+        **URedisSlowlogSet**
+
+        - **Command** (str) - 查询命令
+        - **SpendTime** (int) - 查询消耗的时间
+        - **StartTime** (int) - 查询发生的时间
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.DescribeURedisSlowlogRequestSchema().dumps(d)
+
+        resp = self.invoke("DescribeURedisSlowlog", d, **kwargs)
+        return apis.DescribeURedisSlowlogResponseSchema().loads(resp)
+
     def describe_uredis_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeURedisUpgradePrice - 获取uredis升级价格信息
+        """DescribeURedisUpgradePrice - 获取uredis升级价格信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - (Required) 要升级的空间的GroupId,请参考DescribeURedisGroup接口
         - **Size** (int) - (Required) 购买uredis大小,单位:GB,范围是[1-32]
-        - **Type** (str) - 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        - **DataSet** (dict) - 见 **PriceDataSet** 模型定义
-        - **Price** (int) - 扩容差价，单位: 元，保留小数点后两位有效数字(兼容老版本)
-        
-        **Response Model**
-        
-        **PriceDataSet** 
-        
-        - **CustomPrice** (int) - 用户折后价
-        - **PurchaseValue** (int) - 资源有效期
-        - **TotalPrice** (int) - 升降级资源的价格
+        - **Price** (float) - 扩容差价，单位: 元，保留小数点后两位有效数字
 
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.DescribeURedisUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeURedisUpgradePrice", d, **kwargs)
         return apis.DescribeURedisUpgradePriceResponseSchema().loads(resp)
 
+    def describe_uredis_version(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """DescribeURedisVersion - 获取主Redis可用版本
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
+        **Response**
+
+        - **DataSet** (list) - 见 **URedisVersionSet** 模型定义
+        - **TotalCount** (int) - 总版本个数
+
+        **Response Model**
+
+        **URedisVersionSet**
+
+        - **Version** (str) - Redis版本
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.DescribeURedisVersionRequestSchema().dumps(d)
+
+        resp = self.invoke("DescribeURedisVersion", d, **kwargs)
+        return apis.DescribeURedisVersionResponseSchema().loads(resp)
+
     def get_umem_space_state(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUMemSpaceState - 获取UMem内存空间列表
+        """GetUMemSpaceState - 获取UMem内存空间列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SpaceId** (str) - (Required) 内存空间ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **State** (str) - Starting:创建中 Running:运行中 Fail:失败
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.GetUMemSpaceStateRequestSchema().dumps(d)
 
         resp = self.invoke("GetUMemSpaceState", d, **kwargs)
         return apis.GetUMemSpaceStateResponseSchema().loads(resp)
 
     def modify_umem_space_name(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyUMemSpaceName - 修改UMem内存空间名称
+        """ModifyUMemSpaceName - 修改UMem内存空间名称
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) 新的名称,长度(6<=size<=63)
         - **SpaceId** (str) - (Required) UMem内存空间ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.ModifyUMemSpaceNameRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyUMemSpaceName", d, **kwargs)
         return apis.ModifyUMemSpaceNameResponseSchema().loads(resp)
 
     def modify_uredis_group_name(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyURedisGroupName - 修改主备redis名称
+        """ModifyURedisGroupName - 修改主备redis名称
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - (Required) 组的ID
         - **Name** (str) - (Required) Redis组名称 (范围[6-63],只能包含英文、数字以及符号-和_)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.ModifyURedisGroupNameRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyURedisGroupName", d, **kwargs)
         return apis.ModifyURedisGroupNameResponseSchema().loads(resp)
 
-    def resize_udredis_space(
+    def modify_uredis_group_password(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeUDredisSpace - 调整内存空间容量
+        """ModifyURedisGroupPassword - 修改主备密码/重置密码
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **Size** (int) - (Required) 内存大小, 单位:GB (需要大于原size,<= 1024)
-        - **SpaceId** (str) - (Required) 高性能UMem 内存空间Id
-        - **CouponId** (str) - 使用的代金券Id
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **GroupId** (str) - (Required) 组的ID
+        - **Password** (str) - (Required) 新密码字符串，要求长度为6~36个字符,且只能包含英文、数字以及-和下划线；并且需要base64加密；如要取消密码，此值为空字符串，
+        - **ResourceType** (str) -
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
-        d = apis.ResizeUDredisSpaceRequestSchema().dumps(d)
+        d = apis.ModifyURedisGroupPasswordRequestSchema().dumps(d)
 
-        resp = self.invoke("ResizeUDredisSpace", d, **kwargs)
-        return apis.ResizeUDredisSpaceResponseSchema().loads(resp)
+        resp = self.invoke("ModifyURedisGroupPassword", d, **kwargs)
+        return apis.ModifyURedisGroupPasswordResponseSchema().loads(resp)
 
     def resize_umem_space(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeUMemSpace - 调整内存空间容量
+        """ResizeUMemSpace - 调整内存空间容量
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Size** (int) - (Required) 内存大小, 单位:GB (需要大于原size,<= 1024)
         - **SpaceId** (str) - (Required) UMem 内存空间Id
-        - **ChargeType** (str) - 
         - **CouponId** (str) - 使用的代金券Id
-        - **Type** (str) - 空间类型:single(无热备),double(热备)(默认: double)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.ResizeUMemSpaceRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeUMemSpace", d, **kwargs)
         return apis.ResizeUMemSpaceResponseSchema().loads(resp)
 
     def resize_uredis_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeURedisGroup - 调整主备redis容量
+        """ResizeURedisGroup - 调整主备redis容量
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - (Required) 组ID
         - **Size** (int) - (Required) 内存大小, 单位:GB (需要大于原size,且小于等于32) 目前仅支持1/2/4/8/16/32 G 六种容量规格
-        - **ChargeType** (str) - 
         - **CouponId** (int) - 代金券ID 请参考DescribeCoupon接口
-        - **Type** (str) - 空间类型:single(无热备),double(热备)(默认: double)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.ResizeURedisGroupRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeURedisGroup", d, **kwargs)
         return apis.ResizeURedisGroupResponseSchema().loads(resp)
 
     def restart_umem_cache_group(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ RestartUMemcacheGroup - 重启单机Memcache
+        """RestartUMemcacheGroup - 重启单机Memcache
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **GroupId** (str) - (Required) 组的ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
-        
+
         """
         # build request
-        d = {"ProjectId": self.config.project_id, "Region": self.config.region}
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
         req and d.update(req)
         d = apis.RestartUMemcacheGroupRequestSchema().dumps(d)
 
         resp = self.invoke("RestartUMemcacheGroup", d, **kwargs)
         return apis.RestartUMemcacheGroupResponseSchema().loads(resp)
+
+    def update_uredis_backup_strategy(
+        self, req: typing.Optional[dict] = None, **kwargs
+    ) -> dict:
+        """UpdateURedisBackupStrategy - URedisBackupStrategy
+
+        **Request**
+
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **BackupTime** (str) - (Required) 备份时间，默认为0
+        - **GroupId** (str) - (Required) 组的ID
+        - **AutoBackup** (str) - 是否打开默认备份功能。enable(打开)，disable(关闭)，默认enable
+        - **SlaveZone** (str) - 跨机房URedis，slave所在可用区（必须和Zone在同一Region，且不可相同）
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
+        **Response**
+
+
+        """
+        # build request
+        d = {
+            "ProjectId": self.config.project_id,
+            "Region": self.config.region,
+        }
+        req and d.update(req)
+        d = apis.UpdateURedisBackupStrategyRequestSchema().dumps(d)
+
+        resp = self.invoke("UpdateURedisBackupStrategy", d, **kwargs)
+        return apis.UpdateURedisBackupStrategyResponseSchema().loads(resp)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/umem/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/umem/schemas/apis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,87 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
+
 from ucloud.core.typesystem import schema, fields
 from ucloud.services.umem.schemas import models
 
-
 """ UMem API Schema
 """
 
 
 """
+API: CreateUMemBackup
+
+创建分布式redis备份
+"""
+
+
+class CreateUMemBackupRequestSchema(schema.RequestSchema):
+    """CreateUMemBackup - 创建分布式redis备份"""
+
+    fields = {
+        "BackupName": fields.Str(required=True, dump_to="BackupName"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
+    }
+
+
+class CreateUMemBackupResponseSchema(schema.ResponseSchema):
+    """CreateUMemBackup - 创建分布式redis备份"""
+
+    fields = {
+        "BackupId": fields.Str(required=False, load_from="BackupId"),
+    }
+
+
+"""
 API: CreateUMemSpace
 
 创建UMem内存空间
 """
 
 
 class CreateUMemSpaceRequestSchema(schema.RequestSchema):
-    """ CreateUMemSpace - 创建UMem内存空间
-    """
+    """CreateUMemSpace - 创建UMem内存空间"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Name": fields.Str(required=True, dump_to="Name"),
-        "Password": fields.Base64(required=False, dump_to="Password"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Protocol": fields.Str(required=False, dump_to="Protocol"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "SubnetId": fields.Str(required=False, dump_to="SubnetId"),
-        "Tag": fields.Str(required=False, dump_to="Tag"),
         "Type": fields.Str(required=False, dump_to="Type"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
-        "Zone": fields.Str(required=False, dump_to="Zone"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateUMemSpaceResponseSchema(schema.ResponseSchema):
-    """ CreateUMemSpace - 创建UMem内存空间
-    """
+    """CreateUMemSpace - 创建UMem内存空间"""
 
-    fields = {"SpaceId": fields.Str(required=False, load_from="SpaceId")}
+    fields = {
+        "SpaceId": fields.Str(required=False, load_from="SpaceId"),
+    }
 
 
 """
 API: CreateUMemcacheGroup
 
 创建单机Memcache
 """
 
 
 class CreateUMemcacheGroupRequestSchema(schema.RequestSchema):
-    """ CreateUMemcacheGroup - 创建单机Memcache
-    """
+    """CreateUMemcacheGroup - 创建单机Memcache"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "ConfigId": fields.Str(required=False, dump_to="ConfigId"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -70,38 +94,67 @@
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Version": fields.Str(required=False, dump_to="Version"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CreateUMemcacheGroupResponseSchema(schema.ResponseSchema):
-    """ CreateUMemcacheGroup - 创建单机Memcache
-    """
+    """CreateUMemcacheGroup - 创建单机Memcache"""
 
-    fields = {"GroupId": fields.Str(required=False, load_from="GroupId")}
+    fields = {
+        "GroupId": fields.Str(required=False, load_from="GroupId"),
+    }
+
+
+"""
+API: CreateURedisBackup
+
+创建主备Redis备份
+"""
+
+
+class CreateURedisBackupRequestSchema(schema.RequestSchema):
+    """CreateURedisBackup - 创建主备Redis备份"""
+
+    fields = {
+        "BackupName": fields.Str(required=True, dump_to="BackupName"),
+        "GroupId": fields.Str(required=True, dump_to="GroupId"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "SlaveZone": fields.Str(required=False, dump_to="SlaveZone"),
+        "Zone": fields.Str(required=False, dump_to="Zone"),
+    }
+
+
+class CreateURedisBackupResponseSchema(schema.ResponseSchema):
+    """CreateURedisBackup - 创建主备Redis备份"""
+
+    fields = {
+        "BackupId": fields.Str(required=True, load_from="BackupId"),
+    }
 
 
 """
 API: CreateURedisGroup
 
 创建主备redis
 """
 
 
 class CreateURedisGroupRequestSchema(schema.RequestSchema):
-    """ CreateURedisGroup - 创建主备redis
-    """
+    """CreateURedisGroup - 创建主备redis"""
 
     fields = {
         "AutoBackup": fields.Str(required=False, dump_to="AutoBackup"),
         "BackupId": fields.Str(required=False, dump_to="BackupId"),
         "BackupTime": fields.Int(required=False, dump_to="BackupTime"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "ConfigId": fields.Str(required=False, dump_to="ConfigId"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
+        "EnableIpV6": fields.Bool(required=False, dump_to="EnableIpV6"),
         "HighAvailability": fields.Str(
             required=True, dump_to="HighAvailability"
         ),
         "MasterGroupId": fields.Str(required=False, dump_to="MasterGroupId"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "Password": fields.Base64(required=False, dump_to="Password"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -114,155 +167,236 @@
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Version": fields.Str(required=False, dump_to="Version"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreateURedisGroupResponseSchema(schema.ResponseSchema):
-    """ CreateURedisGroup - 创建主备redis
-    """
+    """CreateURedisGroup - 创建主备redis"""
 
-    fields = {"GroupId": fields.Str(required=False, load_from="GroupId")}
+    fields = {
+        "GroupId": fields.Str(required=False, load_from="GroupId"),
+    }
 
 
 """
 API: DeleteUMemSpace
 
 删除UMem内存空间
 """
 
 
 class DeleteUMemSpaceRequestSchema(schema.RequestSchema):
-    """ DeleteUMemSpace - 删除UMem内存空间
-    """
+    """DeleteUMemSpace - 删除UMem内存空间"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DeleteUMemSpaceResponseSchema(schema.ResponseSchema):
-    """ DeleteUMemSpace - 删除UMem内存空间
-    """
+    """DeleteUMemSpace - 删除UMem内存空间"""
 
     fields = {}
 
 
 """
 API: DeleteUMemcacheGroup
 
 删除单机Memcache
 """
 
 
 class DeleteUMemcacheGroupRequestSchema(schema.RequestSchema):
-    """ DeleteUMemcacheGroup - 删除单机Memcache
-    """
+    """DeleteUMemcacheGroup - 删除单机Memcache"""
 
     fields = {
         "GroupId": fields.Str(required=True, dump_to="GroupId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DeleteUMemcacheGroupResponseSchema(schema.ResponseSchema):
-    """ DeleteUMemcacheGroup - 删除单机Memcache
-    """
+    """DeleteUMemcacheGroup - 删除单机Memcache"""
 
     fields = {}
 
 
 """
 API: DeleteURedisGroup
 
 删除主备redis
 """
 
 
 class DeleteURedisGroupRequestSchema(schema.RequestSchema):
-    """ DeleteURedisGroup - 删除主备redis
-    """
+    """DeleteURedisGroup - 删除主备redis"""
 
     fields = {
         "GroupId": fields.Str(required=True, dump_to="GroupId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DeleteURedisGroupResponseSchema(schema.ResponseSchema):
-    """ DeleteURedisGroup - 删除主备redis
-    """
+    """DeleteURedisGroup - 删除主备redis"""
 
     fields = {}
 
 
 """
+API: DescribeUMemBackup
+
+查询分布式redis备份
+"""
+
+
+class DescribeUMemBackupRequestSchema(schema.RequestSchema):
+    """DescribeUMemBackup - 查询分布式redis备份"""
+
+    fields = {
+        "Limit": fields.Int(required=False, dump_to="Limit"),
+        "Offset": fields.Int(required=False, dump_to="Offset"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
+    }
+
+
+class DescribeUMemBackupResponseSchema(schema.ResponseSchema):
+    """DescribeUMemBackup - 查询分布式redis备份"""
+
+    fields = {
+        "DataSet": fields.List(
+            models.UMemBackupSetSchema(), required=False, load_from="DataSet"
+        ),
+    }
+
+
+"""
+API: DescribeUMemBackupURL
+
+获取分布式redis 备份下载链接
+"""
+
+
+class DescribeUMemBackupURLRequestSchema(schema.RequestSchema):
+    """DescribeUMemBackupURL - 获取分布式redis 备份下载链接"""
+
+    fields = {
+        "BackupId": fields.Str(required=True, dump_to="BackupId"),
+        "BlockId": fields.Str(required=False, dump_to="BlockId"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
+    }
+
+
+class DescribeUMemBackupURLResponseSchema(schema.ResponseSchema):
+    """DescribeUMemBackupURL - 获取分布式redis 备份下载链接"""
+
+    fields = {
+        "BackupURL": fields.List(
+            fields.Str(), required=True, load_from="BackupURL"
+        ),
+    }
+
+
+"""
+API: DescribeUMemBlockInfo
+
+拉取UDRedis分片信息
+"""
+
+
+class DescribeUMemBlockInfoRequestSchema(schema.RequestSchema):
+    """DescribeUMemBlockInfo - 拉取UDRedis分片信息"""
+
+    fields = {
+        "Limit": fields.Int(required=True, dump_to="Limit"),
+        "Offset": fields.Int(required=True, dump_to="Offset"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
+    }
+
+
+class DescribeUMemBlockInfoResponseSchema(schema.ResponseSchema):
+    """DescribeUMemBlockInfo - 拉取UDRedis分片信息"""
+
+    fields = {
+        "DataSet": fields.List(
+            models.UMemBlockInfoSchema(), required=False, load_from="DataSet"
+        ),
+    }
+
+
+"""
 API: DescribeUMemPrice
 
 获取UMem实例价格信息
 """
 
 
 class DescribeUMemPriceRequestSchema(schema.RequestSchema):
-    """ DescribeUMemPrice - 获取UMem实例价格信息
-    """
+    """DescribeUMemPrice - 获取UMem实例价格信息"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
-        "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "Type": fields.Str(required=True, dump_to="Type"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUMemPriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUMemPrice - 获取UMem实例价格信息
-    """
+    """DescribeUMemPrice - 获取UMem实例价格信息"""
 
     fields = {
         "DataSet": fields.List(
             models.UMemPriceSetSchema(), required=False, load_from="DataSet"
-        )
+        ),
     }
 
 
 """
 API: DescribeUMemSpace
 
 获取UMem内存空间列表
 """
 
 
 class DescribeUMemSpaceRequestSchema(schema.RequestSchema):
-    """ DescribeUMemSpace - 获取UMem内存空间列表
-    """
+    """DescribeUMemSpace - 获取UMem内存空间列表"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Protocol": fields.Str(required=False, dump_to="Protocol"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SpaceId": fields.Str(required=False, dump_to="SpaceId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUMemSpaceResponseSchema(schema.ResponseSchema):
-    """ DescribeUMemSpace - 获取UMem内存空间列表
-    """
+    """DescribeUMemSpace - 获取UMem内存空间列表"""
 
     fields = {
         "DataSet": fields.List(
             models.UMemSpaceSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -272,30 +406,28 @@
 API: DescribeUMemUpgradePrice
 
 获取UMem升级价格信息
 """
 
 
 class DescribeUMemUpgradePriceRequestSchema(schema.RequestSchema):
-    """ DescribeUMemUpgradePrice - 获取UMem升级价格信息
-    """
+    """DescribeUMemUpgradePrice - 获取UMem升级价格信息"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
         "Type": fields.Str(required=True, dump_to="Type"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUMemUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUMemUpgradePrice - 获取UMem升级价格信息
-    """
+    """DescribeUMemUpgradePrice - 获取UMem升级价格信息"""
 
     fields = {
         "DataSet": models.PriceDataSetSchema(),
         "Price": fields.Int(required=False, load_from="Price"),
     }
 
 
@@ -303,30 +435,28 @@
 API: DescribeUMemcacheGroup
 
 显示Memcache
 """
 
 
 class DescribeUMemcacheGroupRequestSchema(schema.RequestSchema):
-    """ DescribeUMemcacheGroup - 显示Memcache
-    """
+    """DescribeUMemcacheGroup - 显示Memcache"""
 
     fields = {
         "GroupId": fields.Str(required=False, dump_to="GroupId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUMemcacheGroupResponseSchema(schema.ResponseSchema):
-    """ DescribeUMemcacheGroup - 显示Memcache
-    """
+    """DescribeUMemcacheGroup - 显示Memcache"""
 
     fields = {
         "DataSet": fields.List(
             models.UMemcacheGroupSetSchema(),
             required=False,
             load_from="DataSet",
         ),
@@ -338,94 +468,84 @@
 API: DescribeUMemcachePrice
 
 获取umemcache组价格信息
 """
 
 
 class DescribeUMemcachePriceRequestSchema(schema.RequestSchema):
-    """ DescribeUMemcachePrice - 获取umemcache组价格信息
-    """
+    """DescribeUMemcachePrice - 获取umemcache组价格信息"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "Type": fields.Str(required=False, dump_to="Type"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeUMemcachePriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUMemcachePrice - 获取umemcache组价格信息
-    """
+    """DescribeUMemcachePrice - 获取umemcache组价格信息"""
 
     fields = {
         "DataSet": fields.List(
             models.UMemcachePriceSetSchema(),
             required=False,
             load_from="DataSet",
-        )
+        ),
     }
 
 
 """
 API: DescribeUMemcacheUpgradePrice
 
 获取umemcache升级价格信息
 """
 
 
 class DescribeUMemcacheUpgradePriceRequestSchema(schema.RequestSchema):
-    """ DescribeUMemcacheUpgradePrice - 获取umemcache升级价格信息
-    """
+    """DescribeUMemcacheUpgradePrice - 获取umemcache升级价格信息"""
 
     fields = {
         "GroupId": fields.Str(required=True, dump_to="GroupId"),
-        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
-        "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
-        "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeUMemcacheUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ DescribeUMemcacheUpgradePrice - 获取umemcache升级价格信息
-    """
+    """DescribeUMemcacheUpgradePrice - 获取umemcache升级价格信息"""
 
     fields = {
-        "DataSet": models.PriceDataSetSchema(),
-        "Price": fields.Int(required=False, load_from="Price"),
+        "Price": fields.Float(required=False, load_from="Price"),
     }
 
 
 """
 API: DescribeURedisBackup
 
 查询主备redis备份
 """
 
 
 class DescribeURedisBackupRequestSchema(schema.RequestSchema):
-    """ DescribeURedisBackup - 查询主备redis备份
-    """
+    """DescribeURedisBackup - 查询主备redis备份"""
 
     fields = {
         "GroupId": fields.Str(required=False, dump_to="GroupId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DescribeURedisBackupResponseSchema(schema.ResponseSchema):
-    """ DescribeURedisBackup - 查询主备redis备份
-    """
+    """DescribeURedisBackup - 查询主备redis备份"""
 
     fields = {
         "DataSet": fields.List(
             models.URedisBackupSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -435,64 +555,91 @@
 API: DescribeURedisBackupURL
 
 获取主备Redis备份下载链接
 """
 
 
 class DescribeURedisBackupURLRequestSchema(schema.RequestSchema):
-    """ DescribeURedisBackupURL - 获取主备Redis备份下载链接
-    """
+    """DescribeURedisBackupURL - 获取主备Redis备份下载链接"""
 
     fields = {
         "BackupId": fields.Str(required=True, dump_to="BackupId"),
         "GroupId": fields.Str(required=False, dump_to="GroupId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
+        "SlaveZone": fields.Str(required=False, dump_to="SlaveZone"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeURedisBackupURLResponseSchema(schema.ResponseSchema):
-    """ DescribeURedisBackupURL - 获取主备Redis备份下载链接
-    """
+    """DescribeURedisBackupURL - 获取主备Redis备份下载链接"""
 
     fields = {
         "BackupPath": fields.Str(required=False, load_from="BackupPath"),
         "BackupURL": fields.Str(required=False, load_from="BackupURL"),
-        "InnerBackupPath": fields.Str(
-            required=False, load_from="InnerBackupPath"
+    }
+
+
+"""
+API: DescribeURedisConfig
+
+查询主备Redis所有配置文件
+"""
+
+
+class DescribeURedisConfigRequestSchema(schema.RequestSchema):
+    """DescribeURedisConfig - 查询主备Redis所有配置文件"""
+
+    fields = {
+        "ConfigId": fields.Str(required=False, dump_to="ConfigId"),
+        "Limit": fields.Int(required=False, dump_to="Limit"),
+        "Offset": fields.Int(required=False, dump_to="Offset"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "RegionFlag": fields.Bool(required=True, dump_to="RegionFlag"),
+        "Version": fields.Str(required=False, dump_to="Version"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
+    }
+
+
+class DescribeURedisConfigResponseSchema(schema.ResponseSchema):
+    """DescribeURedisConfig - 查询主备Redis所有配置文件"""
+
+    fields = {
+        "DataSet": fields.List(
+            models.URedisConfigSetSchema(), required=False, load_from="DataSet"
         ),
+        "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
 
 
 """
 API: DescribeURedisGroup
 
 查询主备Redis
 """
 
 
 class DescribeURedisGroupRequestSchema(schema.RequestSchema):
-    """ DescribeURedisGroup - 查询主备Redis
-    """
+    """DescribeURedisGroup - 查询主备Redis"""
 
     fields = {
         "GroupId": fields.Str(required=False, dump_to="GroupId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeURedisGroupResponseSchema(schema.ResponseSchema):
-    """ DescribeURedisGroup - 查询主备Redis
-    """
+    """DescribeURedisGroup - 查询主备Redis"""
 
     fields = {
         "DataSet": fields.List(
             models.URedisGroupSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -502,257 +649,316 @@
 API: DescribeURedisPrice
 
 取uredis价格信息
 """
 
 
 class DescribeURedisPriceRequestSchema(schema.RequestSchema):
-    """ DescribeURedisPrice - 取uredis价格信息
-    """
+    """DescribeURedisPrice - 取uredis价格信息"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "ProductType": fields.Str(required=False, dump_to="ProductType"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RegionFlag": fields.Bool(required=False, dump_to="RegionFlag"),
         "Size": fields.Int(required=True, dump_to="Size"),
-        "Type": fields.Str(required=False, dump_to="Type"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribeURedisPriceResponseSchema(schema.ResponseSchema):
-    """ DescribeURedisPrice - 取uredis价格信息
-    """
+    """DescribeURedisPrice - 取uredis价格信息"""
 
     fields = {
         "DataSet": fields.List(
             models.URedisPriceSetSchema(), required=False, load_from="DataSet"
-        )
+        ),
+    }
+
+
+"""
+API: DescribeURedisSlowlog
+
+查询URedis慢日志
+"""
+
+
+class DescribeURedisSlowlogRequestSchema(schema.RequestSchema):
+    """DescribeURedisSlowlog - 查询URedis慢日志"""
+
+    fields = {
+        "GroupId": fields.Str(required=True, dump_to="GroupId"),
+        "Limit": fields.Int(required=False, dump_to="Limit"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
+    }
+
+
+class DescribeURedisSlowlogResponseSchema(schema.ResponseSchema):
+    """DescribeURedisSlowlog - 查询URedis慢日志"""
+
+    fields = {
+        "DataSet": fields.List(
+            models.URedisSlowlogSetSchema(), required=False, load_from="DataSet"
+        ),
+        "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
 
 
 """
 API: DescribeURedisUpgradePrice
 
 获取uredis升级价格信息
 """
 
 
 class DescribeURedisUpgradePriceRequestSchema(schema.RequestSchema):
-    """ DescribeURedisUpgradePrice - 获取uredis升级价格信息
-    """
+    """DescribeURedisUpgradePrice - 获取uredis升级价格信息"""
 
     fields = {
         "GroupId": fields.Str(required=True, dump_to="GroupId"),
-        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
-        "Type": fields.Str(required=False, dump_to="Type"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeURedisUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ DescribeURedisUpgradePrice - 获取uredis升级价格信息
-    """
+    """DescribeURedisUpgradePrice - 获取uredis升级价格信息"""
 
     fields = {
-        "DataSet": models.PriceDataSetSchema(),
-        "Price": fields.Int(required=False, load_from="Price"),
+        "Price": fields.Float(required=False, load_from="Price"),
+    }
+
+
+"""
+API: DescribeURedisVersion
+
+获取主Redis可用版本
+"""
+
+
+class DescribeURedisVersionRequestSchema(schema.RequestSchema):
+    """DescribeURedisVersion - 获取主Redis可用版本"""
+
+    fields = {
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
+    }
+
+
+class DescribeURedisVersionResponseSchema(schema.ResponseSchema):
+    """DescribeURedisVersion - 获取主Redis可用版本"""
+
+    fields = {
+        "DataSet": fields.List(
+            models.URedisVersionSetSchema(), required=False, load_from="DataSet"
+        ),
+        "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
 
 
 """
 API: GetUMemSpaceState
 
 获取UMem内存空间列表
 """
 
 
 class GetUMemSpaceStateRequestSchema(schema.RequestSchema):
-    """ GetUMemSpaceState - 获取UMem内存空间列表
-    """
+    """GetUMemSpaceState - 获取UMem内存空间列表"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class GetUMemSpaceStateResponseSchema(schema.ResponseSchema):
-    """ GetUMemSpaceState - 获取UMem内存空间列表
-    """
+    """GetUMemSpaceState - 获取UMem内存空间列表"""
 
-    fields = {"State": fields.Str(required=False, load_from="State")}
+    fields = {
+        "State": fields.Str(required=False, load_from="State"),
+    }
 
 
 """
 API: ModifyUMemSpaceName
 
 修改UMem内存空间名称
 """
 
 
 class ModifyUMemSpaceNameRequestSchema(schema.RequestSchema):
-    """ ModifyUMemSpaceName - 修改UMem内存空间名称
-    """
+    """ModifyUMemSpaceName - 修改UMem内存空间名称"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyUMemSpaceNameResponseSchema(schema.ResponseSchema):
-    """ ModifyUMemSpaceName - 修改UMem内存空间名称
-    """
+    """ModifyUMemSpaceName - 修改UMem内存空间名称"""
 
     fields = {}
 
 
 """
 API: ModifyURedisGroupName
 
 修改主备redis名称
 """
 
 
 class ModifyURedisGroupNameRequestSchema(schema.RequestSchema):
-    """ ModifyURedisGroupName - 修改主备redis名称
-    """
+    """ModifyURedisGroupName - 修改主备redis名称"""
 
     fields = {
         "GroupId": fields.Str(required=True, dump_to="GroupId"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
-        "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyURedisGroupNameResponseSchema(schema.ResponseSchema):
-    """ ModifyURedisGroupName - 修改主备redis名称
-    """
+    """ModifyURedisGroupName - 修改主备redis名称"""
 
     fields = {}
 
 
 """
-API: ResizeUDredisSpace
+API: ModifyURedisGroupPassword
 
-调整内存空间容量
+修改主备密码/重置密码
 """
 
 
-class ResizeUDredisSpaceRequestSchema(schema.RequestSchema):
-    """ ResizeUDredisSpace - 调整内存空间容量
-    """
+class ModifyURedisGroupPasswordRequestSchema(schema.RequestSchema):
+    """ModifyURedisGroupPassword - 修改主备密码/重置密码"""
 
     fields = {
-        "CouponId": fields.Str(required=False, dump_to="CouponId"),
+        "GroupId": fields.Str(required=True, dump_to="GroupId"),
+        "Password": fields.Str(required=True, dump_to="Password"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
-        "Size": fields.Int(required=True, dump_to="Size"),
-        "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
+        "ResourceType": fields.Str(required=False, dump_to="ResourceType"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
-class ResizeUDredisSpaceResponseSchema(schema.ResponseSchema):
-    """ ResizeUDredisSpace - 调整内存空间容量
-    """
+class ModifyURedisGroupPasswordResponseSchema(schema.ResponseSchema):
+    """ModifyURedisGroupPassword - 修改主备密码/重置密码"""
 
     fields = {}
 
 
 """
 API: ResizeUMemSpace
 
 调整内存空间容量
 """
 
 
 class ResizeUMemSpaceRequestSchema(schema.RequestSchema):
-    """ ResizeUMemSpace - 调整内存空间容量
-    """
+    """ResizeUMemSpace - 调整内存空间容量"""
 
     fields = {
-        "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
         "SpaceId": fields.Str(required=True, dump_to="SpaceId"),
-        "Type": fields.Str(required=False, dump_to="Type"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ResizeUMemSpaceResponseSchema(schema.ResponseSchema):
-    """ ResizeUMemSpace - 调整内存空间容量
-    """
+    """ResizeUMemSpace - 调整内存空间容量"""
 
     fields = {}
 
 
 """
 API: ResizeURedisGroup
 
 调整主备redis容量
 """
 
 
 class ResizeURedisGroupRequestSchema(schema.RequestSchema):
-    """ ResizeURedisGroup - 调整主备redis容量
-    """
+    """ResizeURedisGroup - 调整主备redis容量"""
 
     fields = {
-        "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Int(required=False, dump_to="CouponId"),
         "GroupId": fields.Str(required=True, dump_to="GroupId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Size": fields.Int(required=True, dump_to="Size"),
-        "Type": fields.Str(required=False, dump_to="Type"),
-        "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ResizeURedisGroupResponseSchema(schema.ResponseSchema):
-    """ ResizeURedisGroup - 调整主备redis容量
-    """
+    """ResizeURedisGroup - 调整主备redis容量"""
 
     fields = {}
 
 
 """
 API: RestartUMemcacheGroup
 
 重启单机Memcache
 """
 
 
 class RestartUMemcacheGroupRequestSchema(schema.RequestSchema):
-    """ RestartUMemcacheGroup - 重启单机Memcache
-    """
+    """RestartUMemcacheGroup - 重启单机Memcache"""
 
     fields = {
         "GroupId": fields.Str(required=True, dump_to="GroupId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
-        "Zone": fields.Str(required=False, dump_to="Zone"),
+        "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class RestartUMemcacheGroupResponseSchema(schema.ResponseSchema):
-    """ RestartUMemcacheGroup - 重启单机Memcache
-    """
+    """RestartUMemcacheGroup - 重启单机Memcache"""
+
+    fields = {}
+
+
+"""
+API: UpdateURedisBackupStrategy
+
+URedisBackupStrategy
+"""
+
+
+class UpdateURedisBackupStrategyRequestSchema(schema.RequestSchema):
+    """UpdateURedisBackupStrategy - URedisBackupStrategy"""
+
+    fields = {
+        "AutoBackup": fields.Str(required=False, dump_to="AutoBackup"),
+        "BackupTime": fields.Str(required=True, dump_to="BackupTime"),
+        "GroupId": fields.Str(required=True, dump_to="GroupId"),
+        "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
+        "Region": fields.Str(required=True, dump_to="Region"),
+        "SlaveZone": fields.Str(required=False, dump_to="SlaveZone"),
+        "Zone": fields.Str(required=False, dump_to="Zone"),
+    }
+
+
+class UpdateURedisBackupStrategyResponseSchema(schema.ResponseSchema):
+    """UpdateURedisBackupStrategy - URedisBackupStrategy"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/umem/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/unet/schemas/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,158 +1,234 @@
-""" Code is generated by ucloud-model, DO NOT EDIT IT. """
-
-from ucloud.core.typesystem import schema, fields
-
-
-class UMemPriceSetSchema(schema.ResponseSchema):
-    """ UMemPriceSet - DescribeUMemPrice
-    """
-
-    fields = {
-        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
-        "OriginalPrice": fields.Int(required=False, load_from="OriginalPrice"),
-        "Price": fields.Int(required=False, load_from="Price"),
-    }
-
-
-class UMemSpaceAddressSetSchema(schema.ResponseSchema):
-    """ UMemSpaceAddressSet - DescribeUMemSpace
-    """
-
-    fields = {
-        "IP": fields.Str(required=False, load_from="IP"),
-        "Port": fields.Int(required=False, load_from="Port"),
-    }
-
-
-class UMemSpaceSetSchema(schema.ResponseSchema):
-    """ UMemSpaceSet - DescribeUMemSpace
-    """
-
-    fields = {
-        "Address": fields.List(UMemSpaceAddressSetSchema()),
-        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
-        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
-        "Name": fields.Str(required=False, load_from="Name"),
-        "Protocol": fields.Str(required=False, load_from="Protocol"),
-        "RewriteTime": fields.Int(required=True, load_from="RewriteTime"),
-        "Size": fields.Int(required=False, load_from="Size"),
-        "SpaceId": fields.Str(required=False, load_from="SpaceId"),
-        "State": fields.Str(required=False, load_from="State"),
-        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
-        "Tag": fields.Str(required=True, load_from="Tag"),
-        "Type": fields.Str(required=False, load_from="Type"),
-        "UsedSize": fields.Int(required=False, load_from="UsedSize"),
-        "VPCId": fields.Str(required=False, load_from="VPCId"),
-        "Zone": fields.Str(required=False, load_from="Zone"),
-    }
-
-
-class PriceDataSetSchema(schema.ResponseSchema):
-    """ PriceDataSet - 升降级价格
-    """
-
-    fields = {
-        "CustomPrice": fields.Int(required=False, load_from="CustomPrice"),
-        "PurchaseValue": fields.Int(required=False, load_from="PurchaseValue"),
-        "TotalPrice": fields.Int(required=False, load_from="TotalPrice"),
-    }
-
-
-class UMemcacheGroupSetSchema(schema.ResponseSchema):
-    """ UMemcacheGroupSet - DescribeUMemcacheGroup
-    """
-
-    fields = {
-        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
-        "ConfigId": fields.Str(required=False, load_from="ConfigId"),
-        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
-        "GroupId": fields.Str(required=False, load_from="GroupId"),
-        "ModifyTime": fields.Int(required=False, load_from="ModifyTime"),
-        "Name": fields.Str(required=False, load_from="Name"),
-        "Port": fields.Int(required=False, load_from="Port"),
-        "Size": fields.Int(required=False, load_from="Size"),
-        "State": fields.Str(required=False, load_from="State"),
-        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
-        "Tag": fields.Str(required=False, load_from="Tag"),
-        "UsedSize": fields.Int(required=False, load_from="UsedSize"),
-        "VPCId": fields.Str(required=False, load_from="VPCId"),
-        "Version": fields.Str(required=False, load_from="Version"),
-        "VirtualIP": fields.Str(required=False, load_from="VirtualIP"),
-    }
-
-
-class UMemcachePriceSetSchema(schema.ResponseSchema):
-    """ UMemcachePriceSet - DescribeUMemcachePrice
-    """
-
-    fields = {
-        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
-        "OriginalPrice": fields.Int(required=False, load_from="OriginalPrice"),
-        "Price": fields.Int(required=False, load_from="Price"),
-    }
-
-
-class URedisBackupSetSchema(schema.ResponseSchema):
-    """ URedisBackupSet - DescribeURedisBackup
-    """
-
-    fields = {
-        "BackupId": fields.Str(required=False, load_from="BackupId"),
-        "BackupName": fields.Str(required=False, load_from="BackupName"),
-        "BackupSize": fields.Int(required=False, load_from="BackupSize"),
-        "BackupTime": fields.Int(required=False, load_from="BackupTime"),
-        "BackupType": fields.Str(required=False, load_from="BackupType"),
-        "GroupId": fields.Str(required=False, load_from="GroupId"),
-        "GroupName": fields.Str(required=False, load_from="GroupName"),
-        "State": fields.Str(required=False, load_from="State"),
-        "Zone": fields.Str(required=False, load_from="Zone"),
-    }
-
-
-class URedisGroupSetSchema(schema.ResponseSchema):
-    """ URedisGroupSet - DescribeURedisGroup
-    """
-
-    fields = {
-        "AutoBackup": fields.Str(required=False, load_from="AutoBackup"),
-        "BackupTime": fields.Int(required=False, load_from="BackupTime"),
-        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
-        "ConfigId": fields.Str(required=False, load_from="ConfigId"),
-        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
-        "GroupId": fields.Str(required=False, load_from="GroupId"),
-        "GroupName": fields.Str(required=False, load_from="GroupName"),
-        "HighAvailability": fields.Str(
-            required=False, load_from="HighAvailability"
-        ),
-        "MemorySize": fields.Int(required=False, load_from="MemorySize"),
-        "ModifyTime": fields.Int(required=False, load_from="ModifyTime"),
-        "Name": fields.Str(required=False, load_from="Name"),
-        "Port": fields.Int(required=False, load_from="Port"),
-        "Protocol": fields.Str(required=False, load_from="Protocol"),
-        "RewriteTime": fields.Int(required=True, load_from="RewriteTime"),
-        "Size": fields.Int(required=False, load_from="Size"),
-        "SlaveZone": fields.Str(required=False, load_from="SlaveZone"),
-        "State": fields.Str(required=False, load_from="State"),
-        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
-        "Tag": fields.Str(required=False, load_from="Tag"),
-        "Type": fields.Str(required=False, load_from="Type"),
-        "UsedSize": fields.Int(required=False, load_from="UsedSize"),
-        "VPCId": fields.Str(required=True, load_from="VPCId"),
-        "Version": fields.Str(required=False, load_from="Version"),
-        "VirtualIP": fields.Str(required=False, load_from="VirtualIP"),
-        "Zone": fields.Str(required=False, load_from="Zone"),
-    }
-
-
-class URedisPriceSetSchema(schema.ResponseSchema):
-    """ URedisPriceSet - 主备Redis价格
-    """
-
-    fields = {
-        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
-        "OriginalPrice": fields.Int(required=True, load_from="OriginalPrice"),
-        "Price": fields.Int(required=False, load_from="Price"),
-    }
+""" Code is generated by ucloud-model, DO NOT EDIT IT. """
+
+from ucloud.core.typesystem import schema, fields
+
+
+class UnetEIPAddrSetSchema(schema.ResponseSchema):
+    """UnetEIPAddrSet - DescribeEIP"""
+
+    fields = {
+        "IP": fields.Str(required=False, load_from="IP"),
+        "OperatorName": fields.Str(required=False, load_from="OperatorName"),
+    }
+
+
+class UnetAllocateEIPSetSchema(schema.ResponseSchema):
+    """UnetAllocateEIPSet - AllocateEIP"""
+
+    fields = {
+        "EIPAddr": fields.List(UnetEIPAddrSetSchema()),
+        "EIPId": fields.Str(required=False, load_from="EIPId"),
+    }
+
+
+class VIPSetSchema(schema.ResponseSchema):
+    """VIPSet - VIPSet"""
+
+    fields = {
+        "VIP": fields.Str(required=False, load_from="VIP"),
+        "VIPId": fields.Str(required=False, load_from="VIPId"),
+        "VPCId": fields.Str(required=False, load_from="VPCId"),
+    }
+
+
+class EIPAddrSetSchema(schema.ResponseSchema):
+    """EIPAddrSet - DescribeShareBandwidth"""
+
+    fields = {
+        "IP": fields.Str(required=False, load_from="IP"),
+        "OperatorName": fields.Str(required=False, load_from="OperatorName"),
+    }
+
+
+class UnetBandwidthPackageSetSchema(schema.ResponseSchema):
+    """UnetBandwidthPackageSet - DescribeBandwidthPackage"""
+
+    fields = {
+        "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
+        "BandwidthPackageId": fields.Str(
+            required=False, load_from="BandwidthPackageId"
+        ),
+        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
+        "DisableTime": fields.Int(required=False, load_from="DisableTime"),
+        "EIPAddr": fields.List(EIPAddrSetSchema()),
+        "EIPId": fields.Str(required=False, load_from="EIPId"),
+        "EnableTime": fields.Int(required=False, load_from="EnableTime"),
+    }
+
+
+class UnetBandwidthUsageEIPSetSchema(schema.ResponseSchema):
+    """UnetBandwidthUsageEIPSet - DescribeBandwidthUsage"""
+
+    fields = {
+        "CurBandwidth": fields.Float(required=False, load_from="CurBandwidth"),
+        "EIPId": fields.Str(required=False, load_from="EIPId"),
+    }
+
+
+class ShareBandwidthSetSchema(schema.ResponseSchema):
+    """ShareBandwidthSet - DescribeEIP"""
+
+    fields = {
+        "ShareBandwidth": fields.Int(
+            required=False, load_from="ShareBandwidth"
+        ),
+        "ShareBandwidthId": fields.Str(
+            required=False, load_from="ShareBandwidthId"
+        ),
+        "ShareBandwidthName": fields.Str(
+            required=False, load_from="ShareBandwidthName"
+        ),
+    }
+
+
+class UnetEIPResourceSetSchema(schema.ResponseSchema):
+    """UnetEIPResourceSet - DescribeEIP"""
+
+    fields = {
+        "EIPId": fields.Str(required=False, load_from="EIPId"),
+        "ResourceId": fields.Str(required=False, load_from="ResourceId"),
+        "ResourceName": fields.Str(required=False, load_from="ResourceName"),
+        "ResourceType": fields.Str(required=False, load_from="ResourceType"),
+        "SubResourceId": fields.Str(required=False, load_from="SubResourceId"),
+        "SubResourceName": fields.Str(
+            required=False, load_from="SubResourceName"
+        ),
+        "SubResourceType": fields.Str(
+            required=False, load_from="SubResourceType"
+        ),
+    }
+
+
+class UnetEIPSetSchema(schema.ResponseSchema):
+    """UnetEIPSet - DescribeEIP"""
+
+    fields = {
+        "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
+        "BandwidthType": fields.Int(required=False, load_from="BandwidthType"),
+        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
+        "EIPAddr": fields.List(UnetEIPAddrSetSchema()),
+        "EIPId": fields.Str(required=False, load_from="EIPId"),
+        "Expire": fields.Bool(required=False, load_from="Expire"),
+        "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
+        "Name": fields.Str(required=False, load_from="Name"),
+        "PayMode": fields.Str(required=False, load_from="PayMode"),
+        "Remark": fields.Str(required=False, load_from="Remark"),
+        "Resource": UnetEIPResourceSetSchema(),
+        "ShareBandwidthSet": ShareBandwidthSetSchema(),
+        "Status": fields.Str(required=False, load_from="Status"),
+        "Tag": fields.Str(required=False, load_from="Tag"),
+        "Weight": fields.Int(required=False, load_from="Weight"),
+    }
+
+
+class FirewallRuleSetSchema(schema.ResponseSchema):
+    """FirewallRuleSet - DescribeFirewall"""
+
+    fields = {
+        "DstPort": fields.Str(required=False, load_from="DstPort"),
+        "Priority": fields.Str(required=False, load_from="Priority"),
+        "ProtocolType": fields.Str(required=False, load_from="ProtocolType"),
+        "Remark": fields.Str(required=False, load_from="Remark"),
+        "RuleAction": fields.Str(required=False, load_from="RuleAction"),
+        "SrcIP": fields.Str(required=False, load_from="SrcIP"),
+    }
+
+
+class FirewallDataSetSchema(schema.ResponseSchema):
+    """FirewallDataSet - DescribeFirewall"""
+
+    fields = {
+        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
+        "FWId": fields.Str(required=True, load_from="FWId"),
+        "GroupId": fields.Str(required=True, load_from="GroupId"),
+        "Name": fields.Str(required=False, load_from="Name"),
+        "Remark": fields.Str(required=False, load_from="Remark"),
+        "ResourceCount": fields.Int(required=False, load_from="ResourceCount"),
+        "Rule": fields.List(FirewallRuleSetSchema()),
+        "Tag": fields.Str(required=False, load_from="Tag"),
+        "Type": fields.Str(required=False, load_from="Type"),
+    }
+
+
+class ResourceSetSchema(schema.ResponseSchema):
+    """ResourceSet - 资源信息"""
+
+    fields = {
+        "Name": fields.Str(required=False, load_from="Name"),
+        "PrivateIP": fields.Str(required=False, load_from="PrivateIP"),
+        "Remark": fields.Str(required=False, load_from="Remark"),
+        "ResourceID": fields.Str(required=False, load_from="ResourceID"),
+        "ResourceType": fields.Str(required=False, load_from="ResourceType"),
+        "Status": fields.Int(required=False, load_from="Status"),
+        "Tag": fields.Str(required=False, load_from="Tag"),
+        "Zone": fields.Int(required=False, load_from="Zone"),
+    }
+
+
+class EIPSetDataSchema(schema.ResponseSchema):
+    """EIPSetData - describeShareBandwidth"""
+
+    fields = {
+        "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
+        "EIPAddr": fields.List(EIPAddrSetSchema()),
+        "EIPId": fields.Str(required=False, load_from="EIPId"),
+    }
+
+
+class UnetShareBandwidthSetSchema(schema.ResponseSchema):
+    """UnetShareBandwidthSet - DescribeShareBandwidth"""
+
+    fields = {
+        "BandwidthGuarantee": fields.Int(
+            required=False, load_from="BandwidthGuarantee"
+        ),
+        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
+        "EIPSet": fields.List(EIPSetDataSchema()),
+        "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
+        "Name": fields.Str(required=False, load_from="Name"),
+        "PostPayStartTime": fields.Int(
+            required=False, load_from="PostPayStartTime"
+        ),
+        "ShareBandwidth": fields.Int(
+            required=False, load_from="ShareBandwidth"
+        ),
+        "ShareBandwidthId": fields.Str(
+            required=False, load_from="ShareBandwidthId"
+        ),
+    }
+
+
+class VIPDetailSetSchema(schema.ResponseSchema):
+    """VIPDetailSet - VIPDetailSet"""
+
+    fields = {
+        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
+        "Name": fields.Str(required=False, load_from="Name"),
+        "RealIp": fields.Str(required=False, load_from="RealIp"),
+        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
+        "VIP": fields.Str(required=False, load_from="VIP"),
+        "VIPId": fields.Str(required=False, load_from="VIPId"),
+        "VPCId": fields.Str(required=False, load_from="VPCId"),
+        "Zone": fields.Str(required=False, load_from="Zone"),
+    }
+
+
+class EIPPayModeSetSchema(schema.ResponseSchema):
+    """EIPPayModeSet - GetEIPPayModeEIP"""
+
+    fields = {
+        "EIPId": fields.Str(required=False, load_from="EIPId"),
+        "EIPPayMode": fields.Str(required=False, load_from="EIPPayMode"),
+    }
+
+
+class EIPPriceDetailSetSchema(schema.ResponseSchema):
+    """EIPPriceDetailSet - GetEIPPrice"""
+
+    fields = {
+        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "Price": fields.Float(required=False, load_from="Price"),
+        "PurchaseValue": fields.Int(required=False, load_from="PurchaseValue"),
+    }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/unet/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/unet/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class UNetClient(Client):
     def __init__(
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UNetClient, self).__init__(config, transport, middleware, logger)
 
     def allocate_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ AllocateEIP - 根据提供信息, 申请弹性IP
+        """AllocateEIP - 根据提供信息, 申请弹性IP
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。
         - **Region** (str) - (Config) 地域。
         - **Bandwidth** (int) - (Required) 弹性IP的外网带宽, 单位为Mbps. 共享带宽模式必须指定0M带宽, 非共享带宽模式必须指定非0Mbps带宽. 各地域非共享带宽的带宽范围如下： 流量计费[1-200]，带宽计费[1-800]
         - **OperatorName** (str) - (Required) 弹性IP的线路如下: 国际: International BGP: Bgp  各地域允许的线路参数如下:  cn-sh1: Bgp cn-sh2: Bgp cn-gd: Bgp cn-bj1: Bgp cn-bj2: Bgp hk: International us-ca: International th-bkk: International  kr-seoul:International  us-ws:International  ge-fra:International  sg:International  tw-kh:International.其他海外线路均为 International
@@ -25,28 +25,28 @@
         - **CouponId** (str) - 代金券ID, 默认不使用
         - **Name** (str) - 弹性IP的名称, 默认为 "EIP"
         - **PayMode** (str) - 弹性IP的计费模式. 枚举值: "Traffic", 流量计费; "Bandwidth", 带宽计费; "ShareBandwidth",共享带宽模式. 默认为 "Bandwidth".
         - **Quantity** (int) - 购买时长, 默认: 1
         - **Remark** (str) - 弹性IP的备注, 默认为空
         - **ShareBandwidthId** (str) - 绑定的共享带宽Id，仅当PayMode为ShareBandwidth时有效
         - **Tag** (str) - 业务组名称, 默认为 "Default"
-        
+
         **Response**
 
         - **EIPSet** (list) - 见 **UnetAllocateEIPSet** 模型定义
-        
+
         **Response Model**
-        
-        **UnetEIPAddrSet** 
-        
+
+        **UnetEIPAddrSet**
+
         - **IP** (str) - IP地址
         - **OperatorName** (str) - 运营商信息如: 电信: Telecom, 联通: Unicom, 国际: International, Duplet: 双线IP（电信+联通), BGP: Bgp
 
-        **UnetAllocateEIPSet** 
-        
+        **UnetAllocateEIPSet**
+
         - **EIPAddr** (list) - 见 **UnetEIPAddrSet** 模型定义
         - **EIPId** (str) - 申请到的EIP资源ID
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
@@ -57,69 +57,69 @@
 
         resp = self.invoke("AllocateEIP", d, **kwargs)
         return apis.AllocateEIPResponseSchema().loads(resp)
 
     def allocate_share_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ AllocateShareBandwidth - 开通共享带宽
+        """AllocateShareBandwidth - 开通共享带宽
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - (Required) 付费方式:Year 按年,Month 按月,Dynamic 按时;
         - **Name** (str) - (Required) 共享带宽名字
         - **ShareBandwidth** (int) - (Required) 共享带宽值
         - **BwType** (str) - 共享带宽类型，ipv4或者ipv6，不传默认ipv4
         - **Quantity** (int) - 购买时长
         - **ShareBandwidthGuarantee** (int) - 共享带宽保底值(后付费)
-        
+
         **Response**
 
         - **ShareBandwidthId** (str) - 共享带宽资源Id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.AllocateShareBandwidthRequestSchema().dumps(d)
 
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("AllocateShareBandwidth", d, **kwargs)
         return apis.AllocateShareBandwidthResponseSchema().loads(resp)
 
     def allocate_vip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ AllocateVIP - 根据提供信息，申请内网VIP(Virtual IP），多用于高可用程序作为漂移IP。
+        """AllocateVIP - 根据提供信息，申请内网VIP(Virtual IP），多用于高可用程序作为漂移IP。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域
         - **SubnetId** (str) - (Required) 子网id
         - **VPCId** (str) - (Required) 指定vip所属的VPC
         - **BusinessId** (str) - 业务组
         - **Count** (int) - 申请数量，默认: 1
         - **Ip** (str) - 指定ip
         - **Name** (str) - vip名，默认为VIP
         - **Remark** (str) - 备注
         - **Tag** (str) - 业务组名称，默认为Default
         - **Zone** (str) - 可用区
-        
+
         **Response**
 
         - **DataSet** (list) - 申请到的VIP地址
         - **VIPSet** (list) - 见 **VIPSet** 模型定义
-        
+
         **Response Model**
-        
-        **VIPSet** 
-        
+
+        **VIPSet**
+
         - **VIP** (str) - 虚拟ip
         - **VIPId** (str) - 虚拟ip id
         - **VPCId** (str) - VPC id
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
@@ -131,77 +131,77 @@
 
         resp = self.invoke("AllocateVIP", d, **kwargs)
         return apis.AllocateVIPResponseSchema().loads(resp)
 
     def associate_eip_with_share_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ AssociateEIPWithShareBandwidth - 将EIP加入共享带宽
+        """AssociateEIPWithShareBandwidth - 将EIP加入共享带宽
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。
         - **Region** (str) - (Config) 地域。
         - **EIPIds** (list) - (Required) 要加入共享带宽的EIP的资源Id
         - **ShareBandwidthId** (str) - (Required) 共享带宽ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.AssociateEIPWithShareBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("AssociateEIPWithShareBandwidth", d, **kwargs)
         return apis.AssociateEIPWithShareBandwidthResponseSchema().loads(resp)
 
     def bind_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ BindEIP - 将尚未使用的弹性IP绑定到指定的资源
+        """BindEIP - 将尚未使用的弹性IP绑定到指定的资源
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **EIPId** (str) - (Required) 弹性IP的资源Id
         - **ResourceId** (str) - (Required) 弹性IP请求绑定的资源ID
         - **ResourceType** (str) - (Required) 弹性IP请求绑定的资源类型, 枚举值为: uhost: 云主机; ulb, 负载均衡器 upm: 物理机; hadoophost: 大数据集群;fortresshost：堡垒机；udockhost：容器；udhost：私有专区主机；natgw：natgw；udb：udb；vpngw：ipsec vpn；ucdr：云灾备；dbaudit：数据库审计；uni：虚拟网卡。
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.BindEIPRequestSchema().dumps(d)
 
         resp = self.invoke("BindEIP", d, **kwargs)
         return apis.BindEIPResponseSchema().loads(resp)
 
     def create_bandwidth_package(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateBandwidthPackage - 为非共享带宽模式下, 已绑定资源实例的带宽计费弹性IP附加临时带宽包
+        """CreateBandwidthPackage - 为非共享带宽模式下, 已绑定资源实例的带宽计费弹性IP附加临时带宽包
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。
         - **Region** (str) - (Config) 地域
         - **Bandwidth** (int) - (Required) 带宽大小(单位Mbps), 取值范围[2,800] (最大值受地域限制)
         - **EIPId** (str) - (Required) 所绑定弹性IP的资源ID
         - **TimeRange** (int) - (Required) 带宽包有效时长, 取值范围为大于0的整数, 即该带宽包在EnableTime到 EnableTime+TimeRange时间段内生效
         - **CouponId** (str) - 代金券ID
         - **EnableTime** (int) - 生效时间, 格式为 Unix timestamp, 默认为立即开通
-        
+
         **Response**
 
         - **BandwidthPackageId** (str) - 所创建带宽包的资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateBandwidthPackageRequestSchema().dumps(d)
 
         # build options
@@ -209,29 +209,29 @@
 
         resp = self.invoke("CreateBandwidthPackage", d, **kwargs)
         return apis.CreateBandwidthPackageResponseSchema().loads(resp)
 
     def create_firewall(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateFirewall - 创建防火墙
+        """CreateFirewall - 创建防火墙
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **Name** (str) - (Required) 防火墙名称
         - **Rule** (list) - (Required) 防火墙规则，例如：TCP|22|192.168.1.1/22|DROP|LOW|禁用22端口，第一个参数代表协议：第二个参数代表端口号，第三个参数为ip，第四个参数为ACCEPT（接受）和DROP（拒绝），第五个参数优先级：HIGH（高），MEDIUM（中），LOW（低），第六个参数为该条规则的自定义备注
         - **Remark** (str) - 防火墙描述，默认为空
         - **Tag** (str) - 防火墙业务组，默认为Default
-        
+
         **Response**
 
         - **FWId** (str) - 防火墙ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateFirewallRequestSchema().dumps(d)
 
         # build options
@@ -239,83 +239,83 @@
 
         resp = self.invoke("CreateFirewall", d, **kwargs)
         return apis.CreateFirewallResponseSchema().loads(resp)
 
     def delete_bandwidth_package(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteBandwidthPackage - 删除弹性IP上已附加带宽包
+        """DeleteBandwidthPackage - 删除弹性IP上已附加带宽包
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **BandwidthPackageId** (str) - (Required) 带宽包资源ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteBandwidthPackageRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteBandwidthPackage", d, **kwargs)
         return apis.DeleteBandwidthPackageResponseSchema().loads(resp)
 
     def delete_firewall(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteFirewall - 删除防火墙
+        """DeleteFirewall - 删除防火墙
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **FWId** (str) - (Required) 防火墙资源ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteFirewallRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteFirewall", d, **kwargs)
         return apis.DeleteFirewallResponseSchema().loads(resp)
 
     def describe_bandwidth_package(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeBandwidthPackage - 获取某地域下的带宽包信息
+        """DescribeBandwidthPackage - 获取某地域下的带宽包信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 返回数据分页值, 取值范围为 [0,10000000] 之间的整数, 默认为20
         - **Offset** (int) - 返回数据偏移量, 默认为0
-        
+
         **Response**
 
         - **DataSets** (list) - 见 **UnetBandwidthPackageSet** 模型定义
         - **TotalCount** (int) - 满足条件的带宽包总数
-        
+
         **Response Model**
-        
-        **EIPAddrSet** 
-        
+
+        **EIPAddrSet**
+
         - **IP** (str) - 弹性IP地址
         - **OperatorName** (str) - 运营商信息, 枚举值为: Telecom 电信; Unicom: 联通; Duplet: 双线; Bgp: BGP; International: 国际.
 
-        **UnetBandwidthPackageSet** 
-        
+        **UnetBandwidthPackageSet**
+
         - **Bandwidth** (int) - 带宽包的临时带宽值, 单位Mbps
         - **BandwidthPackageId** (str) - 带宽包的资源ID
         - **CreateTime** (int) - 创建时间, 格式为 Unix Timestamp
         - **DisableTime** (int) - 失效时间, 格式为 Unix Timestamp
         - **EIPAddr** (list) - 见 **EIPAddrSet** 模型定义
         - **EIPId** (str) - 带宽包所绑定弹性IP的资源ID
         - **EnableTime** (int) - 生效时间, 格式为 Unix Timestamp
@@ -328,87 +328,87 @@
 
         resp = self.invoke("DescribeBandwidthPackage", d, **kwargs)
         return apis.DescribeBandwidthPackageResponseSchema().loads(resp)
 
     def describe_bandwidth_usage(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeBandwidthUsage - 获取带宽用量信息
+        """DescribeBandwidthUsage - 获取带宽用量信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **EIPIds** (list) - 弹性IP的资源Id. 如果为空, 则返回当前 Region中符合条件的所有EIP的带宽用量, n为自然数
         - **Limit** (int) - 返回数据分页值, 取值范围为 [0,10000000] 之间的整数, 默认为20
         - **OffSet** (int) - 返回数据偏移量, 默认为0
-        
+
         **Response**
 
         - **EIPSet** (list) - 见 **UnetBandwidthUsageEIPSet** 模型定义
         - **TotalCount** (int) - EIPSet中的元素个数
-        
+
         **Response Model**
-        
-        **UnetBandwidthUsageEIPSet** 
-        
+
+        **UnetBandwidthUsageEIPSet**
+
         - **CurBandwidth** (float) - 最近5分钟带宽用量, 单位Mbps
         - **EIPId** (str) - 弹性IP资源ID
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribeBandwidthUsageRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeBandwidthUsage", d, **kwargs)
         return apis.DescribeBandwidthUsageResponseSchema().loads(resp)
 
     def describe_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeEIP - 获取弹性IP信息
+        """DescribeEIP - 获取弹性IP信息
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **EIPIds** (list) - 弹性IP的资源ID如果为空, 则返回当前 Region中符合条件的的所有EIP
         - **Limit** (int) - 数据分页值, 默认为20
         - **Offset** (int) - 数据偏移量, 默认为0
-        
+
         **Response**
 
         - **EIPSet** (list) - 见 **UnetEIPSet** 模型定义
         - **TotalBandwidth** (int) - 满足条件的弹性IP带宽总和, 单位Mbps
         - **TotalCount** (int) - 满足条件的弹性IP总数
-        
+
         **Response Model**
-        
-        **ShareBandwidthSet** 
-        
+
+        **ShareBandwidthSet**
+
         - **ShareBandwidth** (int) - 共享带宽带宽值
         - **ShareBandwidthId** (str) - 共享带宽ID
         - **ShareBandwidthName** (str) - 共享带宽的资源名称
 
-        **UnetEIPAddrSet** 
-        
+        **UnetEIPAddrSet**
+
         - **IP** (str) - IP地址
         - **OperatorName** (str) - 运营商信息如: 电信: Telecom, 联通: Unicom, 国际: International, Duplet: 双线IP（电信+联通), BGP: Bgp
 
-        **UnetEIPResourceSet** 
-        
+        **UnetEIPResourceSet**
+
         - **EIPId** (str) - 弹性IP的资源ID
         - **ResourceId** (str) - 已绑定资源的资源ID
         - **ResourceName** (str) - 已绑定的资源名称
         - **ResourceType** (str) - 已绑定的资源类型, 枚举值为: uhost, 云主机；natgw：NAT网关；ulb：负载均衡器；upm: 物理机; hadoophost: 大数据集群;fortresshost：堡垒机；udockhost：容器；udhost：私有专区主机；vpngw：IPSec VPN；ucdr：云灾备；dbaudit：数据库审计，uni：虚拟网卡。
         - **SubResourceId** (str) - 资源绑定的虚拟网卡的ID
         - **SubResourceName** (str) - 资源绑定的虚拟网卡的名称
         - **SubResourceType** (str) - 资源绑定的虚拟网卡的类型。uni，虚拟网卡。
 
-        **UnetEIPSet** 
-        
+        **UnetEIPSet**
+
         - **Bandwidth** (int) - 弹性IP的带宽, 单位为Mbps, 当BandwidthType=1时, 该处显示为共享带宽值. 当BandwidthType=0时, 该处显示这个弹性IP的带宽.
         - **BandwidthType** (int) - 带宽模式, 枚举值为: 0: 非共享带宽模式, 1: 共享带宽模式
         - **ChargeType** (str) - 付费方式, 枚举值为: Year, 按年付费; Month, 按月付费; Dynamic, 按小时付费; Trial, 试用. 按小时付费和试用这两种付费模式需要开通权限.
         - **CreateTime** (int) - 弹性IP的创建时间, 格式为Unix Timestamp
         - **EIPAddr** (list) - 见 **UnetEIPAddrSet** 模型定义
         - **EIPId** (str) - 弹性IP的资源ID
         - **Expire** (bool) - 弹性IP是否到期
@@ -430,44 +430,44 @@
 
         resp = self.invoke("DescribeEIP", d, **kwargs)
         return apis.DescribeEIPResponseSchema().loads(resp)
 
     def describe_firewall(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeFirewall - 获取防火墙组信息
+        """DescribeFirewall - 获取防火墙组信息
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **FWId** (str) - 防火墙ID，默认为返回所有防火墙
         - **Limit** (int) - 返回数据长度，默认为20，最大10000000
         - **Offset** (int) - 列表起始位置偏移量，默认为0
         - **ResourceId** (str) - 绑定防火墙组的资源ID
         - **ResourceType** (str) - 绑定防火墙组的资源类型，默认为全部资源类型。枚举值为："unatgw"，NAT网关； "uhost"，云主机； "upm"，物理云主机； "hadoophost"，hadoop节点； "fortresshost"，堡垒机； "udhost"，私有专区主机；"udockhost"，容器；"dbaudit"，数据库审计.
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **FirewallDataSet** 模型定义
-        - **TotalCount** (int) - 
-        
+        - **TotalCount** (int) -
+
         **Response Model**
-        
-        **FirewallRuleSet** 
-        
+
+        **FirewallRuleSet**
+
         - **DstPort** (str) - 目标端口
         - **Priority** (str) - 优先级
         - **ProtocolType** (str) - 协议类型
         - **Remark** (str) - 防火墙规则备注
         - **RuleAction** (str) - 防火墙动作
         - **SrcIP** (str) - 源地址
 
-        **FirewallDataSet** 
-        
+        **FirewallDataSet**
+
         - **CreateTime** (int) - 防火墙组创建时间，格式为Unix Timestamp
         - **FWId** (str) - 防火墙ID
         - **GroupId** (str) - 安全组ID（即将废弃）
         - **Name** (str) - 防火墙名称
         - **Remark** (str) - 防火墙备注
         - **ResourceCount** (int) - 防火墙绑定资源数量
         - **Rule** (list) - 见 **FirewallRuleSet** 模型定义
@@ -482,33 +482,33 @@
 
         resp = self.invoke("DescribeFirewall", d, **kwargs)
         return apis.DescribeFirewallResponseSchema().loads(resp)
 
     def describe_firewall_resource(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeFirewallResource - 获取防火墙组所绑定资源的外网IP
+        """DescribeFirewallResource - 获取防火墙组所绑定资源的外网IP
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **FWId** (str) - (Required) 防火墙ID
         - **Limit** (int) - 返回数据长度，默认为20，最大10000000
         - **Offset** (int) - 列表起始位置偏移量，默认为0
-        
+
         **Response**
 
         - **ResourceSet** (list) - 见 **ResourceSet** 模型定义
         - **TotalCount** (int) - 绑定资源总数
-        
+
         **Response Model**
-        
-        **ResourceSet** 
-        
+
+        **ResourceSet**
+
         - **Name** (str) - 名称
         - **PrivateIP** (str) - 内网IP
         - **Remark** (str) - 备注
         - **ResourceID** (str) - 绑定该防火墙的资源id
         - **ResourceType** (str) - 绑定资源的资源类型，如"uhost","upm","umem","uhive","uvip","uredis","uhadoop","ufortress","dbaudit","udw","udocker", "umemcache"
         - **Status** (int) - 状态
         - **Tag** (str) - 业务组
@@ -522,42 +522,42 @@
 
         resp = self.invoke("DescribeFirewallResource", d, **kwargs)
         return apis.DescribeFirewallResourceResponseSchema().loads(resp)
 
     def describe_share_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeShareBandwidth - 获取共享带宽信息
+        """DescribeShareBandwidth - 获取共享带宽信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ShareBandwidthIds** (list) - 需要返回的共享带宽Id
-        
+
         **Response**
 
         - **DataSet** (list) - 见 **UnetShareBandwidthSet** 模型定义
         - **TotalCount** (int) - 符合条件的共享带宽总数，大于等于返回DataSet长度
-        
+
         **Response Model**
-        
-        **EIPAddrSet** 
-        
+
+        **EIPAddrSet**
+
         - **IP** (str) - 弹性IP地址
         - **OperatorName** (str) - 运营商信息, 枚举值为: Telecom 电信; Unicom: 联通; Duplet: 双线; Bgp: BGP; International: 国际.
 
-        **EIPSetData** 
-        
+        **EIPSetData**
+
         - **Bandwidth** (int) - EIP带宽值
         - **EIPAddr** (list) - 见 **EIPAddrSet** 模型定义
         - **EIPId** (str) - EIP资源Id
 
-        **UnetShareBandwidthSet** 
-        
+        **UnetShareBandwidthSet**
+
         - **BandwidthGuarantee** (int) - 共享带宽保底值(后付费)
         - **ChargeType** (str) - 付费方式, 预付费:Year 按年,Month 按月,Dynamic 按需;后付费:PostPay(按月)
         - **CreateTime** (int) - 创建时间, 格式为Unix Timestamp
         - **EIPSet** (list) - 见 **EIPSetData** 模型定义
         - **ExpireTime** (int) - 过期时间, 格式为Unix Timestamp
         - **Name** (str) - 共享带宽名称
         - **PostPayStartTime** (int) - 共享带宽后付费开始计费时间(后付费)
@@ -570,38 +570,38 @@
         req and d.update(req)
         d = apis.DescribeShareBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeShareBandwidth", d, **kwargs)
         return apis.DescribeShareBandwidthResponseSchema().loads(resp)
 
     def describe_vip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeVIP - 获取内网VIP详细信息
+        """DescribeVIP - 获取内网VIP详细信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BusinessId** (str) - 业务组
         - **SubnetId** (str) - 子网id，不指定则获取VPCId下的所有vip
         - **Tag** (str) - 业务组名称, 默认为 Default
         - **VPCId** (str) - vpc的id,指定SubnetId时必填
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **DataSet** (list) - 内网VIP地址列表
         - **TotalCount** (int) - vip数量
         - **VIPSet** (list) - 见 **VIPDetailSet** 模型定义
-        
+
         **Response Model**
-        
-        **VIPDetailSet** 
-        
+
+        **VIPDetailSet**
+
         - **CreateTime** (int) - 创建时间
-        - **Name** (str) - 
+        - **Name** (str) -
         - **RealIp** (str) - 真实主机ip
         - **SubnetId** (str) - 子网id
         - **VIP** (str) - 虚拟ip
         - **VIPId** (str) - 虚拟ip id
         - **VPCId** (str) - VPC id
         - **Zone** (str) - 地域
 
@@ -613,58 +613,58 @@
 
         resp = self.invoke("DescribeVIP", d, **kwargs)
         return apis.DescribeVIPResponseSchema().loads(resp)
 
     def disassociate_eip_with_share_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DisassociateEIPWithShareBandwidth - 将EIP移出共享带宽
+        """DisassociateEIPWithShareBandwidth - 将EIP移出共享带宽
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 移出共享带宽后，EIP的外网带宽, 单位为Mbps. 各地域带宽范围如下：  流量计费[1-200],带宽计费[1-800]
         - **ShareBandwidthId** (str) - (Required) 共享带宽ID
         - **EIPIds** (list) - EIP的资源Id；默认移出该共享带宽下所有的EIP
         - **PayMode** (str) - 移出共享带宽后，EIP的计费模式. 枚举值: "Traffic", 流量计费; "Bandwidth", 带宽计费;  默认为 "Bandwidth".
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DisassociateEIPWithShareBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("DisassociateEIPWithShareBandwidth", d, **kwargs)
         return apis.DisassociateEIPWithShareBandwidthResponseSchema().loads(
             resp
         )
 
     def get_eip_pay_mode(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetEIPPayMode - 获取弹性IP计费模式
+        """GetEIPPayMode - 获取弹性IP计费模式
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **EIPId** (list) - (Required) 弹性IP的资源Id
-        
+
         **Response**
 
         - **EIPPayMode** (list) - 见 **EIPPayModeSet** 模型定义
-        
+
         **Response Model**
-        
-        **EIPPayModeSet** 
-        
+
+        **EIPPayModeSet**
+
         - **EIPId** (str) - EIP的资源ID
         - **EIPPayMode** (str) - EIP的计费模式. 枚举值为：Bandwidth, 带宽计费;Traffic, 流量计费; "ShareBandwidth",共享带宽模式
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
@@ -672,34 +672,34 @@
 
         resp = self.invoke("GetEIPPayMode", d, **kwargs)
         return apis.GetEIPPayModeResponseSchema().loads(resp)
 
     def get_eip_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetEIPPrice - 获取弹性IP价格
+        """GetEIPPrice - 获取弹性IP价格
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 弹性IP的外网带宽, 单位为Mbps, 范围 [0-800]
         - **OperatorName** (str) - (Required) 弹性IP的线路如下: 国际: International BGP: Bgp 各地域允许的线路参数如下: cn-sh1: Bgp cn-sh2: Bgp cn-gd: Bgp cn-bj1: Bgp cn-bj2: Bgp hk: International us-ca: International th-bkk: International kr-seoul:International us-ws:International ge-fra:International sg:International tw-kh:International.其他海外线路均为 International,泉州为移动单线cn-qz:ChinaMobile
         - **ChargeType** (str) - 付费方式, 枚举值为: Year, 按年付费; Month, 按月付费; Dynamic, 按时付费; 默认为获取三种价格
         - **PayMode** (str) - 弹性IP计费方式r. 枚举值为: Traffic, 流量计费; Bandwidth, 带宽计费; "ShareBandwidth",共享带宽模式. 默认为Bandwidth
         - **Quantity** (int) - 购买时长。默认: 1。按小时购买(Dynamic)时无需此参数。 月付时，此参数传0，代表了购买至月末
-        
+
         **Response**
 
         - **PriceSet** (list) - 见 **EIPPriceDetailSet** 模型定义
-        
+
         **Response Model**
-        
-        **EIPPriceDetailSet** 
-        
+
+        **EIPPriceDetailSet**
+
         - **ChargeType** (str) - 弹性IP付费方式
         - **Price** (float) - 弹性IP价格, 单位"元"
         - **PurchaseValue** (int) - 资源有效期, 以Unix Timestamp表示
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
@@ -708,317 +708,317 @@
 
         resp = self.invoke("GetEIPPrice", d, **kwargs)
         return apis.GetEIPPriceResponseSchema().loads(resp)
 
     def get_eip_upgrade_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetEIPUpgradePrice - 获取弹性IP带宽改动价格
+        """GetEIPUpgradePrice - 获取弹性IP带宽改动价格
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 弹性IP的外网带宽, 单位为Mbps, 范围 [1-800]
         - **EIPId** (str) - (Required) 弹性IP的资源ID
-        
+
         **Response**
 
         - **Price** (float) - 调整带宽后的EIP价格, 单位为"元", 如需退费此处为负值
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.GetEIPUpgradePriceRequestSchema().dumps(d)
 
         resp = self.invoke("GetEIPUpgradePrice", d, **kwargs)
         return apis.GetEIPUpgradePriceResponseSchema().loads(resp)
 
     def grant_firewall(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GrantFirewall - 将防火墙应用到资源上
+        """GrantFirewall - 将防火墙应用到资源上
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **FWId** (str) - (Required) 防火墙资源ID
         - **ResourceId** (str) - (Required) 所应用资源ID
         - **ResourceType** (str) - (Required) 绑定防火墙组的资源类型，默认为全部资源类型。枚举值为："unatgw"，NAT网关； "uhost"，云主机； "upm"，物理云主机； "hadoophost"，hadoop节点； "fortresshost"，堡垒机； "udhost"，私有专区主机；"udockhost"，容器；"dbaudit"，数据库审计，”uni“，虚拟网卡。
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.GrantFirewallRequestSchema().dumps(d)
 
         resp = self.invoke("GrantFirewall", d, **kwargs)
         return apis.GrantFirewallResponseSchema().loads(resp)
 
     def modify_eip_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyEIPBandwidth - 调整弹性IP的外网带宽
+        """ModifyEIPBandwidth - 调整弹性IP的外网带宽
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 弹性IP的外网带宽, 单位为Mbps. 各地域的带宽值范围如下：流量计费[1-200],带宽计费[1-800]
         - **EIPId** (str) - (Required) 弹性IP的资源ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyEIPBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyEIPBandwidth", d, **kwargs)
         return apis.ModifyEIPBandwidthResponseSchema().loads(resp)
 
     def modify_eip_weight(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyEIPWeight - 修改弹性IP的外网出口权重
+        """ModifyEIPWeight - 修改弹性IP的外网出口权重
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **EIPId** (str) - (Required) 弹性IP的资源ID
         - **Weight** (int) - (Required) 外网出口权重, 范围[0-100] 取值为0时, 该弹性IP不会被使用. 取值为100时, 同主机下只会使用这个弹性IP，其他弹性IP不会被使用 请勿将多个绑定在同一资源的弹性IP设置为相同权重
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyEIPWeightRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyEIPWeight", d, **kwargs)
         return apis.ModifyEIPWeightResponseSchema().loads(resp)
 
     def release_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ ReleaseEIP - 释放弹性IP资源, 所释放弹性IP必须为非绑定状态.
+        """ReleaseEIP - 释放弹性IP资源, 所释放弹性IP必须为非绑定状态.
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **EIPId** (str) - (Required) 弹性IP的资源ID
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ReleaseEIPRequestSchema().dumps(d)
 
         resp = self.invoke("ReleaseEIP", d, **kwargs)
         return apis.ReleaseEIPResponseSchema().loads(resp)
 
     def release_share_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ReleaseShareBandwidth - 关闭共享带宽
+        """ReleaseShareBandwidth - 关闭共享带宽
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **EIPBandwidth** (int) - (Required) 关闭共享带宽后，各EIP恢复为的带宽值
         - **ShareBandwidthId** (str) - (Required) 共享带宽ID
         - **PayMode** (str) - Bandwidth 带宽计费, Traffic 转流量计费
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ReleaseShareBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("ReleaseShareBandwidth", d, **kwargs)
         return apis.ReleaseShareBandwidthResponseSchema().loads(resp)
 
     def release_vip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ ReleaseVIP - 释放VIP资源
+        """ReleaseVIP - 释放VIP资源
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写
         - **Region** (str) - (Config) 地域
         - **VIPId** (str) - (Required) 内网VIP的id
         - **Zone** (str) - 可用区
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ReleaseVIPRequestSchema().dumps(d)
 
         resp = self.invoke("ReleaseVIP", d, **kwargs)
         return apis.ReleaseVIPResponseSchema().loads(resp)
 
     def resize_share_bandwidth(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ResizeShareBandwidth - 调整共享带宽的带宽值
+        """ResizeShareBandwidth - 调整共享带宽的带宽值
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ShareBandwidth** (int) - (Required) 带宽值，单位为Mb，范围 [20-5000] (最大值受地域限制)
         - **ShareBandwidthId** (str) - (Required) 共享带宽的Id
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ResizeShareBandwidthRequestSchema().dumps(d)
 
         resp = self.invoke("ResizeShareBandwidth", d, **kwargs)
         return apis.ResizeShareBandwidthResponseSchema().loads(resp)
 
     def set_eip_pay_mode(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ SetEIPPayMode - 设置弹性IP计费模式, 切换时会涉及付费/退费.
+        """SetEIPPayMode - 设置弹性IP计费模式, 切换时会涉及付费/退费.
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Bandwidth** (int) - (Required) 调整的目标带宽值, 单位Mbps. 各地域的带宽值范围如下: 流量计费[1-200],其余情况[1-800]
         - **EIPId** (str) - (Required) 弹性IP的资源Id
         - **PayMode** (str) - (Required) 计费模式. 枚举值："Traffic", 流量计费模式; "Bandwidth", 带宽计费模式
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.SetEIPPayModeRequestSchema().dumps(d)
 
         resp = self.invoke("SetEIPPayMode", d, **kwargs)
         return apis.SetEIPPayModeResponseSchema().loads(resp)
 
     def un_bind_eip(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ UnBindEIP - 将弹性IP从资源上解绑
+        """UnBindEIP - 将弹性IP从资源上解绑
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **EIPId** (str) - (Required) 弹性IP的资源Id
         - **ResourceId** (str) - (Required) 弹性IP请求解绑的资源ID
         - **ResourceType** (str) - (Required) 弹性IP请求解绑的资源类型, 枚举值为: uhost: 云主机; ulb, 负载均衡器 upm: 物理机; hadoophost: 大数据集群;fortresshost：堡垒机；udockhost：容器；udhost：私有专区主机；natgw：NAT网关；udb：udb；vpngw：ipsec vpn；ucdr：云灾备；dbaudit：数据库审计；uni，虚拟网卡。
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UnBindEIPRequestSchema().dumps(d)
 
         resp = self.invoke("UnBindEIP", d, **kwargs)
         return apis.UnBindEIPResponseSchema().loads(resp)
 
     def update_eip_attribute(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateEIPAttribute - 更新弹性IP名称，业务组，备注等属性字段
+        """UpdateEIPAttribute - 更新弹性IP名称，业务组，备注等属性字段
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **EIPId** (str) - (Required) EIP资源ID
         - **Name** (str) - 名字（Name Tag Remark都为空则报错）
         - **Remark** (str) - 备注
         - **Tag** (str) - 业务
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateEIPAttributeRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateEIPAttribute", d, **kwargs)
         return apis.UpdateEIPAttributeResponseSchema().loads(resp)
 
     def update_firewall(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateFirewall - 更新防火墙规则
+        """UpdateFirewall - 更新防火墙规则
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **FWId** (str) - (Required) 防火墙资源ID
         - **Rule** (list) - (Required) 防火墙规则，例如：TCP|22|192.168.1.1/22|DROP|LOW|禁用22端口，第一个参数代表协议：第二个参数代表端口号，第三个参数为ip，第四个参数为ACCEPT（接受）和DROP（拒绝），第五个参数优先级：HIGH（高），MEDIUM（中），LOW（低），第六个参数为该条规则的自定义备注
-        
+
         **Response**
 
         - **FWId** (str) - 防火墙id
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateFirewallRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateFirewall", d, **kwargs)
         return apis.UpdateFirewallResponseSchema().loads(resp)
 
     def update_firewall_attribute(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateFirewallAttribute - 更新防火墙规则
+        """UpdateFirewallAttribute - 更新防火墙规则
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **FWId** (str) - (Required) 防火墙资源ID
         - **Name** (str) - 防火墙名称，默认为空，为空则不做修改。Name,Tag,Remark必须填写1个及以上
         - **Remark** (str) - 防火墙备注，默认为空，为空则不做修改。Name,Tag,Remark必须填写1个及以上
         - **Tag** (str) - 防火墙业务组，默认为空，为空则不做修改。Name,Tag,Remark必须填写1个及以上
-        
+
         **Response**
 
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateFirewallAttributeRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateFirewallAttribute", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/unet/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/unet/schemas/apis.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: AllocateEIP
 
 根据提供信息, 申请弹性IP
 """
 
 
 class AllocateEIPRequestSchema(schema.RequestSchema):
-    """ AllocateEIP - 根据提供信息, 申请弹性IP
-    """
+    """AllocateEIP - 根据提供信息, 申请弹性IP"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "Name": fields.Str(required=False, dump_to="Name"),
         "OperatorName": fields.Str(required=True, dump_to="OperatorName"),
@@ -34,16 +33,15 @@
             required=False, dump_to="ShareBandwidthId"
         ),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class AllocateEIPResponseSchema(schema.ResponseSchema):
-    """ AllocateEIP - 根据提供信息, 申请弹性IP
-    """
+    """AllocateEIP - 根据提供信息, 申请弹性IP"""
 
     fields = {
         "EIPSet": fields.List(
             models.UnetAllocateEIPSetSchema(),
             required=False,
             load_from="EIPSet",
         )
@@ -54,16 +52,15 @@
 API: AllocateShareBandwidth
 
 开通共享带宽
 """
 
 
 class AllocateShareBandwidthRequestSchema(schema.RequestSchema):
-    """ AllocateShareBandwidth - 开通共享带宽
-    """
+    """AllocateShareBandwidth - 开通共享带宽"""
 
     fields = {
         "BwType": fields.Str(required=False, dump_to="BwType"),
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
@@ -72,16 +69,15 @@
         "ShareBandwidthGuarantee": fields.Int(
             required=False, dump_to="ShareBandwidthGuarantee"
         ),
     }
 
 
 class AllocateShareBandwidthResponseSchema(schema.ResponseSchema):
-    """ AllocateShareBandwidth - 开通共享带宽
-    """
+    """AllocateShareBandwidth - 开通共享带宽"""
 
     fields = {
         "ShareBandwidthId": fields.Str(
             required=False, load_from="ShareBandwidthId"
         )
     }
 
@@ -90,16 +86,15 @@
 API: AllocateVIP
 
 根据提供信息，申请内网VIP(Virtual IP），多用于高可用程序作为漂移IP。
 """
 
 
 class AllocateVIPRequestSchema(schema.RequestSchema):
-    """ AllocateVIP - 根据提供信息，申请内网VIP(Virtual IP），多用于高可用程序作为漂移IP。
-    """
+    """AllocateVIP - 根据提供信息，申请内网VIP(Virtual IP），多用于高可用程序作为漂移IP。"""
 
     fields = {
         "BusinessId": fields.Str(required=False, dump_to="BusinessId"),
         "Count": fields.Int(required=False, dump_to="Count"),
         "Ip": fields.Str(required=False, dump_to="Ip"),
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -109,16 +104,15 @@
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class AllocateVIPResponseSchema(schema.ResponseSchema):
-    """ AllocateVIP - 根据提供信息，申请内网VIP(Virtual IP），多用于高可用程序作为漂移IP。
-    """
+    """AllocateVIP - 根据提供信息，申请内网VIP(Virtual IP），多用于高可用程序作为漂移IP。"""
 
     fields = {
         "DataSet": fields.List(
             fields.Str(), required=False, load_from="DataSet"
         ),
         "VIPSet": fields.List(
             models.VIPSetSchema(), required=False, load_from="VIPSet"
@@ -130,86 +124,80 @@
 API: AssociateEIPWithShareBandwidth
 
 将EIP加入共享带宽
 """
 
 
 class AssociateEIPWithShareBandwidthRequestSchema(schema.RequestSchema):
-    """ AssociateEIPWithShareBandwidth - 将EIP加入共享带宽
-    """
+    """AssociateEIPWithShareBandwidth - 将EIP加入共享带宽"""
 
     fields = {
         "EIPIds": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ShareBandwidthId": fields.Str(
             required=True, dump_to="ShareBandwidthId"
         ),
     }
 
 
 class AssociateEIPWithShareBandwidthResponseSchema(schema.ResponseSchema):
-    """ AssociateEIPWithShareBandwidth - 将EIP加入共享带宽
-    """
+    """AssociateEIPWithShareBandwidth - 将EIP加入共享带宽"""
 
     fields = {}
 
 
 """
 API: BindEIP
 
 将尚未使用的弹性IP绑定到指定的资源
 """
 
 
 class BindEIPRequestSchema(schema.RequestSchema):
-    """ BindEIP - 将尚未使用的弹性IP绑定到指定的资源
-    """
+    """BindEIP - 将尚未使用的弹性IP绑定到指定的资源"""
 
     fields = {
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceId": fields.Str(required=True, dump_to="ResourceId"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
     }
 
 
 class BindEIPResponseSchema(schema.ResponseSchema):
-    """ BindEIP - 将尚未使用的弹性IP绑定到指定的资源
-    """
+    """BindEIP - 将尚未使用的弹性IP绑定到指定的资源"""
 
     fields = {}
 
 
 """
 API: CreateBandwidthPackage
 
 为非共享带宽模式下, 已绑定资源实例的带宽计费弹性IP附加临时带宽包
 """
 
 
 class CreateBandwidthPackageRequestSchema(schema.RequestSchema):
-    """ CreateBandwidthPackage - 为非共享带宽模式下, 已绑定资源实例的带宽计费弹性IP附加临时带宽包
-    """
+    """CreateBandwidthPackage - 为非共享带宽模式下, 已绑定资源实例的带宽计费弹性IP附加临时带宽包"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "EnableTime": fields.Int(required=False, dump_to="EnableTime"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "TimeRange": fields.Int(required=True, dump_to="TimeRange"),
     }
 
 
 class CreateBandwidthPackageResponseSchema(schema.ResponseSchema):
-    """ CreateBandwidthPackage - 为非共享带宽模式下, 已绑定资源实例的带宽计费弹性IP附加临时带宽包
-    """
+    """CreateBandwidthPackage - 为非共享带宽模式下, 已绑定资源实例的带宽计费弹性IP附加临时带宽包"""
 
     fields = {
         "BandwidthPackageId": fields.Str(
             required=False, load_from="BandwidthPackageId"
         )
     }
 
@@ -218,108 +206,100 @@
 API: CreateFirewall
 
 创建防火墙
 """
 
 
 class CreateFirewallRequestSchema(schema.RequestSchema):
-    """ CreateFirewall - 创建防火墙
-    """
+    """CreateFirewall - 创建防火墙"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Rule": fields.List(fields.Str()),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class CreateFirewallResponseSchema(schema.ResponseSchema):
-    """ CreateFirewall - 创建防火墙
-    """
+    """CreateFirewall - 创建防火墙"""
 
     fields = {"FWId": fields.Str(required=False, load_from="FWId")}
 
 
 """
 API: DeleteBandwidthPackage
 
 删除弹性IP上已附加带宽包
 """
 
 
 class DeleteBandwidthPackageRequestSchema(schema.RequestSchema):
-    """ DeleteBandwidthPackage - 删除弹性IP上已附加带宽包
-    """
+    """DeleteBandwidthPackage - 删除弹性IP上已附加带宽包"""
 
     fields = {
         "BandwidthPackageId": fields.Str(
             required=True, dump_to="BandwidthPackageId"
         ),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DeleteBandwidthPackageResponseSchema(schema.ResponseSchema):
-    """ DeleteBandwidthPackage - 删除弹性IP上已附加带宽包
-    """
+    """DeleteBandwidthPackage - 删除弹性IP上已附加带宽包"""
 
     fields = {}
 
 
 """
 API: DeleteFirewall
 
 删除防火墙
 """
 
 
 class DeleteFirewallRequestSchema(schema.RequestSchema):
-    """ DeleteFirewall - 删除防火墙
-    """
+    """DeleteFirewall - 删除防火墙"""
 
     fields = {
         "FWId": fields.Str(required=True, dump_to="FWId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DeleteFirewallResponseSchema(schema.ResponseSchema):
-    """ DeleteFirewall - 删除防火墙
-    """
+    """DeleteFirewall - 删除防火墙"""
 
     fields = {}
 
 
 """
 API: DescribeBandwidthPackage
 
 获取某地域下的带宽包信息
 """
 
 
 class DescribeBandwidthPackageRequestSchema(schema.RequestSchema):
-    """ DescribeBandwidthPackage - 获取某地域下的带宽包信息
-    """
+    """DescribeBandwidthPackage - 获取某地域下的带宽包信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DescribeBandwidthPackageResponseSchema(schema.ResponseSchema):
-    """ DescribeBandwidthPackage - 获取某地域下的带宽包信息
-    """
+    """DescribeBandwidthPackage - 获取某地域下的带宽包信息"""
 
     fields = {
         "DataSets": fields.List(
             models.UnetBandwidthPackageSetSchema(),
             required=False,
             load_from="DataSets",
         ),
@@ -331,29 +311,27 @@
 API: DescribeBandwidthUsage
 
 获取带宽用量信息
 """
 
 
 class DescribeBandwidthUsageRequestSchema(schema.RequestSchema):
-    """ DescribeBandwidthUsage - 获取带宽用量信息
-    """
+    """DescribeBandwidthUsage - 获取带宽用量信息"""
 
     fields = {
         "EIPIds": fields.List(fields.Str()),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "OffSet": fields.Int(required=False, dump_to="OffSet"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DescribeBandwidthUsageResponseSchema(schema.ResponseSchema):
-    """ DescribeBandwidthUsage - 获取带宽用量信息
-    """
+    """DescribeBandwidthUsage - 获取带宽用量信息"""
 
     fields = {
         "EIPSet": fields.List(
             models.UnetBandwidthUsageEIPSetSchema(),
             required=False,
             load_from="EIPSet",
         ),
@@ -365,29 +343,27 @@
 API: DescribeEIP
 
 获取弹性IP信息
 """
 
 
 class DescribeEIPRequestSchema(schema.RequestSchema):
-    """ DescribeEIP - 获取弹性IP信息
-    """
+    """DescribeEIP - 获取弹性IP信息"""
 
     fields = {
         "EIPIds": fields.List(fields.Str()),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DescribeEIPResponseSchema(schema.ResponseSchema):
-    """ DescribeEIP - 获取弹性IP信息
-    """
+    """DescribeEIP - 获取弹性IP信息"""
 
     fields = {
         "EIPSet": fields.List(
             models.UnetEIPSetSchema(), required=False, load_from="EIPSet"
         ),
         "TotalBandwidth": fields.Int(
             required=False, load_from="TotalBandwidth"
@@ -400,31 +376,29 @@
 API: DescribeFirewall
 
 获取防火墙组信息
 """
 
 
 class DescribeFirewallRequestSchema(schema.RequestSchema):
-    """ DescribeFirewall - 获取防火墙组信息
-    """
+    """DescribeFirewall - 获取防火墙组信息"""
 
     fields = {
         "FWId": fields.Str(required=False, dump_to="FWId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceId": fields.Str(required=False, dump_to="ResourceId"),
         "ResourceType": fields.Str(required=False, dump_to="ResourceType"),
     }
 
 
 class DescribeFirewallResponseSchema(schema.ResponseSchema):
-    """ DescribeFirewall - 获取防火墙组信息
-    """
+    """DescribeFirewall - 获取防火墙组信息"""
 
     fields = {
         "DataSet": fields.List(
             models.FirewallDataSetSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -434,29 +408,27 @@
 API: DescribeFirewallResource
 
 获取防火墙组所绑定资源的外网IP
 """
 
 
 class DescribeFirewallResourceRequestSchema(schema.RequestSchema):
-    """ DescribeFirewallResource - 获取防火墙组所绑定资源的外网IP
-    """
+    """DescribeFirewallResource - 获取防火墙组所绑定资源的外网IP"""
 
     fields = {
         "FWId": fields.Str(required=True, dump_to="FWId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class DescribeFirewallResourceResponseSchema(schema.ResponseSchema):
-    """ DescribeFirewallResource - 获取防火墙组所绑定资源的外网IP
-    """
+    """DescribeFirewallResource - 获取防火墙组所绑定资源的外网IP"""
 
     fields = {
         "ResourceSet": fields.List(
             models.ResourceSetSchema(), required=False, load_from="ResourceSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -466,27 +438,25 @@
 API: DescribeShareBandwidth
 
 获取共享带宽信息
 """
 
 
 class DescribeShareBandwidthRequestSchema(schema.RequestSchema):
-    """ DescribeShareBandwidth - 获取共享带宽信息
-    """
+    """DescribeShareBandwidth - 获取共享带宽信息"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ShareBandwidthIds": fields.List(fields.Str()),
     }
 
 
 class DescribeShareBandwidthResponseSchema(schema.ResponseSchema):
-    """ DescribeShareBandwidth - 获取共享带宽信息
-    """
+    """DescribeShareBandwidth - 获取共享带宽信息"""
 
     fields = {
         "DataSet": fields.List(
             models.UnetShareBandwidthSetSchema(),
             required=False,
             load_from="DataSet",
         ),
@@ -498,31 +468,29 @@
 API: DescribeVIP
 
 获取内网VIP详细信息
 """
 
 
 class DescribeVIPRequestSchema(schema.RequestSchema):
-    """ DescribeVIP - 获取内网VIP详细信息
-    """
+    """DescribeVIP - 获取内网VIP详细信息"""
 
     fields = {
         "BusinessId": fields.Str(required=False, dump_to="BusinessId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetId": fields.Str(required=False, dump_to="SubnetId"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribeVIPResponseSchema(schema.ResponseSchema):
-    """ DescribeVIP - 获取内网VIP详细信息
-    """
+    """DescribeVIP - 获取内网VIP详细信息"""
 
     fields = {
         "DataSet": fields.List(
             fields.Str(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
         "VIPSet": fields.List(
@@ -535,57 +503,53 @@
 API: DisassociateEIPWithShareBandwidth
 
 将EIP移出共享带宽
 """
 
 
 class DisassociateEIPWithShareBandwidthRequestSchema(schema.RequestSchema):
-    """ DisassociateEIPWithShareBandwidth - 将EIP移出共享带宽
-    """
+    """DisassociateEIPWithShareBandwidth - 将EIP移出共享带宽"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "EIPIds": fields.List(fields.Str()),
         "PayMode": fields.Str(required=False, dump_to="PayMode"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ShareBandwidthId": fields.Str(
             required=True, dump_to="ShareBandwidthId"
         ),
     }
 
 
 class DisassociateEIPWithShareBandwidthResponseSchema(schema.ResponseSchema):
-    """ DisassociateEIPWithShareBandwidth - 将EIP移出共享带宽
-    """
+    """DisassociateEIPWithShareBandwidth - 将EIP移出共享带宽"""
 
     fields = {}
 
 
 """
 API: GetEIPPayMode
 
 获取弹性IP计费模式
 """
 
 
 class GetEIPPayModeRequestSchema(schema.RequestSchema):
-    """ GetEIPPayMode - 获取弹性IP计费模式
-    """
+    """GetEIPPayMode - 获取弹性IP计费模式"""
 
     fields = {
         "EIPId": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class GetEIPPayModeResponseSchema(schema.ResponseSchema):
-    """ GetEIPPayMode - 获取弹性IP计费模式
-    """
+    """GetEIPPayMode - 获取弹性IP计费模式"""
 
     fields = {
         "EIPPayMode": fields.List(
             models.EIPPayModeSetSchema(), required=False, load_from="EIPPayMode"
         )
     }
 
@@ -594,31 +558,29 @@
 API: GetEIPPrice
 
 获取弹性IP价格
 """
 
 
 class GetEIPPriceRequestSchema(schema.RequestSchema):
-    """ GetEIPPrice - 获取弹性IP价格
-    """
+    """GetEIPPrice - 获取弹性IP价格"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "OperatorName": fields.Str(required=True, dump_to="OperatorName"),
         "PayMode": fields.Str(required=False, dump_to="PayMode"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=False, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class GetEIPPriceResponseSchema(schema.ResponseSchema):
-    """ GetEIPPrice - 获取弹性IP价格
-    """
+    """GetEIPPrice - 获取弹性IP价格"""
 
     fields = {
         "PriceSet": fields.List(
             models.EIPPriceDetailSetSchema(),
             required=False,
             load_from="PriceSet",
         )
@@ -629,346 +591,320 @@
 API: GetEIPUpgradePrice
 
 获取弹性IP带宽改动价格
 """
 
 
 class GetEIPUpgradePriceRequestSchema(schema.RequestSchema):
-    """ GetEIPUpgradePrice - 获取弹性IP带宽改动价格
-    """
+    """GetEIPUpgradePrice - 获取弹性IP带宽改动价格"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class GetEIPUpgradePriceResponseSchema(schema.ResponseSchema):
-    """ GetEIPUpgradePrice - 获取弹性IP带宽改动价格
-    """
+    """GetEIPUpgradePrice - 获取弹性IP带宽改动价格"""
 
     fields = {"Price": fields.Float(required=False, load_from="Price")}
 
 
 """
 API: GrantFirewall
 
 将防火墙应用到资源上
 """
 
 
 class GrantFirewallRequestSchema(schema.RequestSchema):
-    """ GrantFirewall - 将防火墙应用到资源上
-    """
+    """GrantFirewall - 将防火墙应用到资源上"""
 
     fields = {
         "FWId": fields.Str(required=True, dump_to="FWId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceId": fields.Str(required=True, dump_to="ResourceId"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
     }
 
 
 class GrantFirewallResponseSchema(schema.ResponseSchema):
-    """ GrantFirewall - 将防火墙应用到资源上
-    """
+    """GrantFirewall - 将防火墙应用到资源上"""
 
     fields = {}
 
 
 """
 API: ModifyEIPBandwidth
 
 调整弹性IP的外网带宽
 """
 
 
 class ModifyEIPBandwidthRequestSchema(schema.RequestSchema):
-    """ ModifyEIPBandwidth - 调整弹性IP的外网带宽
-    """
+    """ModifyEIPBandwidth - 调整弹性IP的外网带宽"""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class ModifyEIPBandwidthResponseSchema(schema.ResponseSchema):
-    """ ModifyEIPBandwidth - 调整弹性IP的外网带宽
-    """
+    """ModifyEIPBandwidth - 调整弹性IP的外网带宽"""
 
     fields = {}
 
 
 """
 API: ModifyEIPWeight
 
 修改弹性IP的外网出口权重
 """
 
 
 class ModifyEIPWeightRequestSchema(schema.RequestSchema):
-    """ ModifyEIPWeight - 修改弹性IP的外网出口权重
-    """
+    """ModifyEIPWeight - 修改弹性IP的外网出口权重"""
 
     fields = {
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Weight": fields.Int(required=True, dump_to="Weight"),
     }
 
 
 class ModifyEIPWeightResponseSchema(schema.ResponseSchema):
-    """ ModifyEIPWeight - 修改弹性IP的外网出口权重
-    """
+    """ModifyEIPWeight - 修改弹性IP的外网出口权重"""
 
     fields = {}
 
 
 """
 API: ReleaseEIP
 
 释放弹性IP资源, 所释放弹性IP必须为非绑定状态.
 """
 
 
 class ReleaseEIPRequestSchema(schema.RequestSchema):
-    """ ReleaseEIP - 释放弹性IP资源, 所释放弹性IP必须为非绑定状态.
-    """
+    """ReleaseEIP - 释放弹性IP资源, 所释放弹性IP必须为非绑定状态."""
 
     fields = {
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class ReleaseEIPResponseSchema(schema.ResponseSchema):
-    """ ReleaseEIP - 释放弹性IP资源, 所释放弹性IP必须为非绑定状态.
-    """
+    """ReleaseEIP - 释放弹性IP资源, 所释放弹性IP必须为非绑定状态."""
 
     fields = {}
 
 
 """
 API: ReleaseShareBandwidth
 
 关闭共享带宽
 """
 
 
 class ReleaseShareBandwidthRequestSchema(schema.RequestSchema):
-    """ ReleaseShareBandwidth - 关闭共享带宽
-    """
+    """ReleaseShareBandwidth - 关闭共享带宽"""
 
     fields = {
         "EIPBandwidth": fields.Int(required=True, dump_to="EIPBandwidth"),
         "PayMode": fields.Str(required=False, dump_to="PayMode"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ShareBandwidthId": fields.Str(
             required=True, dump_to="ShareBandwidthId"
         ),
     }
 
 
 class ReleaseShareBandwidthResponseSchema(schema.ResponseSchema):
-    """ ReleaseShareBandwidth - 关闭共享带宽
-    """
+    """ReleaseShareBandwidth - 关闭共享带宽"""
 
     fields = {}
 
 
 """
 API: ReleaseVIP
 
 释放VIP资源
 """
 
 
 class ReleaseVIPRequestSchema(schema.RequestSchema):
-    """ ReleaseVIP - 释放VIP资源
-    """
+    """ReleaseVIP - 释放VIP资源"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VIPId": fields.Str(required=True, dump_to="VIPId"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ReleaseVIPResponseSchema(schema.ResponseSchema):
-    """ ReleaseVIP - 释放VIP资源
-    """
+    """ReleaseVIP - 释放VIP资源"""
 
     fields = {}
 
 
 """
 API: ResizeShareBandwidth
 
 调整共享带宽的带宽值
 """
 
 
 class ResizeShareBandwidthRequestSchema(schema.RequestSchema):
-    """ ResizeShareBandwidth - 调整共享带宽的带宽值
-    """
+    """ResizeShareBandwidth - 调整共享带宽的带宽值"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ShareBandwidth": fields.Int(required=True, dump_to="ShareBandwidth"),
         "ShareBandwidthId": fields.Str(
             required=True, dump_to="ShareBandwidthId"
         ),
     }
 
 
 class ResizeShareBandwidthResponseSchema(schema.ResponseSchema):
-    """ ResizeShareBandwidth - 调整共享带宽的带宽值
-    """
+    """ResizeShareBandwidth - 调整共享带宽的带宽值"""
 
     fields = {}
 
 
 """
 API: SetEIPPayMode
 
 设置弹性IP计费模式, 切换时会涉及付费/退费.
 """
 
 
 class SetEIPPayModeRequestSchema(schema.RequestSchema):
-    """ SetEIPPayMode - 设置弹性IP计费模式, 切换时会涉及付费/退费.
-    """
+    """SetEIPPayMode - 设置弹性IP计费模式, 切换时会涉及付费/退费."""
 
     fields = {
         "Bandwidth": fields.Int(required=True, dump_to="Bandwidth"),
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "PayMode": fields.Str(required=True, dump_to="PayMode"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
     }
 
 
 class SetEIPPayModeResponseSchema(schema.ResponseSchema):
-    """ SetEIPPayMode - 设置弹性IP计费模式, 切换时会涉及付费/退费.
-    """
+    """SetEIPPayMode - 设置弹性IP计费模式, 切换时会涉及付费/退费."""
 
     fields = {}
 
 
 """
 API: UnBindEIP
 
 将弹性IP从资源上解绑
 """
 
 
 class UnBindEIPRequestSchema(schema.RequestSchema):
-    """ UnBindEIP - 将弹性IP从资源上解绑
-    """
+    """UnBindEIP - 将弹性IP从资源上解绑"""
 
     fields = {
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceId": fields.Str(required=True, dump_to="ResourceId"),
         "ResourceType": fields.Str(required=True, dump_to="ResourceType"),
     }
 
 
 class UnBindEIPResponseSchema(schema.ResponseSchema):
-    """ UnBindEIP - 将弹性IP从资源上解绑
-    """
+    """UnBindEIP - 将弹性IP从资源上解绑"""
 
     fields = {}
 
 
 """
 API: UpdateEIPAttribute
 
 更新弹性IP名称，业务组，备注等属性字段
 """
 
 
 class UpdateEIPAttributeRequestSchema(schema.RequestSchema):
-    """ UpdateEIPAttribute - 更新弹性IP名称，业务组，备注等属性字段
-    """
+    """UpdateEIPAttribute - 更新弹性IP名称，业务组，备注等属性字段"""
 
     fields = {
         "EIPId": fields.Str(required=True, dump_to="EIPId"),
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class UpdateEIPAttributeResponseSchema(schema.ResponseSchema):
-    """ UpdateEIPAttribute - 更新弹性IP名称，业务组，备注等属性字段
-    """
+    """UpdateEIPAttribute - 更新弹性IP名称，业务组，备注等属性字段"""
 
     fields = {}
 
 
 """
 API: UpdateFirewall
 
 更新防火墙规则
 """
 
 
 class UpdateFirewallRequestSchema(schema.RequestSchema):
-    """ UpdateFirewall - 更新防火墙规则
-    """
+    """UpdateFirewall - 更新防火墙规则"""
 
     fields = {
         "FWId": fields.Str(required=True, dump_to="FWId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Rule": fields.List(fields.Str()),
     }
 
 
 class UpdateFirewallResponseSchema(schema.ResponseSchema):
-    """ UpdateFirewall - 更新防火墙规则
-    """
+    """UpdateFirewall - 更新防火墙规则"""
 
     fields = {"FWId": fields.Str(required=False, load_from="FWId")}
 
 
 """
 API: UpdateFirewallAttribute
 
 更新防火墙规则
 """
 
 
 class UpdateFirewallAttributeRequestSchema(schema.RequestSchema):
-    """ UpdateFirewallAttribute - 更新防火墙规则
-    """
+    """UpdateFirewallAttribute - 更新防火墙规则"""
 
     fields = {
         "FWId": fields.Str(required=True, dump_to="FWId"),
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class UpdateFirewallAttributeResponseSchema(schema.ResponseSchema):
-    """ UpdateFirewallAttribute - 更新防火墙规则
-    """
+    """UpdateFirewallAttribute - 更新防火墙规则"""
 
     fields = {}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/unet/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/umem/schemas/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,216 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
-class UnetEIPAddrSetSchema(schema.ResponseSchema):
-    """ UnetEIPAddrSet - DescribeEIP
-    """
+class UMemBackupSetSchema(schema.ResponseSchema):
+    """UMemBackupSet - DescribeUMemBackup"""
 
     fields = {
-        "IP": fields.Str(required=False, load_from="IP"),
-        "OperatorName": fields.Str(required=False, load_from="OperatorName"),
+        "BackupId": fields.Str(required=True, load_from="BackupId"),
+        "BackupName": fields.Str(required=True, load_from="BackupName"),
+        "BackupType": fields.Str(required=True, load_from="BackupType"),
+        "BlockCount": fields.Int(required=True, load_from="BlockCount"),
+        "CreateTime": fields.Int(required=True, load_from="CreateTime"),
+        "State": fields.Str(required=True, load_from="State"),
     }
 
 
-class UnetAllocateEIPSetSchema(schema.ResponseSchema):
-    """ UnetAllocateEIPSet - AllocateEIP
-    """
+class UMemBlockInfoSchema(schema.ResponseSchema):
+    """UMemBlockInfo - 分布式redis 分片信息"""
 
     fields = {
-        "EIPAddr": fields.List(UnetEIPAddrSetSchema()),
-        "EIPId": fields.Str(required=False, load_from="EIPId"),
+        "BlockId": fields.Str(required=True, load_from="BlockId"),
+        "BlockPort": fields.Int(required=True, load_from="BlockPort"),
+        "BlockSize": fields.Int(required=True, load_from="BlockSize"),
+        "BlockSlotBegin": fields.Int(required=True, load_from="BlockSlotBegin"),
+        "BlockSlotEnd": fields.Int(required=True, load_from="BlockSlotEnd"),
+        "BlockState": fields.Str(required=True, load_from="BlockState"),
+        "BlockUsedSize": fields.Int(required=True, load_from="BlockUsedSize"),
+        "BlockVip": fields.Str(required=True, load_from="BlockVip"),
     }
 
 
-class VIPSetSchema(schema.ResponseSchema):
-    """ VIPSet - VIPSet
-    """
+class UMemPriceSetSchema(schema.ResponseSchema):
+    """UMemPriceSet - DescribeUMemPrice"""
 
     fields = {
-        "VIP": fields.Str(required=False, load_from="VIP"),
-        "VIPId": fields.Str(required=False, load_from="VIPId"),
-        "VPCId": fields.Str(required=False, load_from="VPCId"),
+        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "ListPrice": fields.Int(required=False, load_from="ListPrice"),
+        "OriginalPrice": fields.Int(required=False, load_from="OriginalPrice"),
+        "Price": fields.Int(required=False, load_from="Price"),
     }
 
 
-class EIPAddrSetSchema(schema.ResponseSchema):
-    """ EIPAddrSet - DescribeShareBandwidth
-    """
+class UMemSpaceAddressSetSchema(schema.ResponseSchema):
+    """UMemSpaceAddressSet - DescribeUMemSpace"""
 
     fields = {
         "IP": fields.Str(required=False, load_from="IP"),
-        "OperatorName": fields.Str(required=False, load_from="OperatorName"),
+        "Port": fields.Int(required=False, load_from="Port"),
     }
 
 
-class UnetBandwidthPackageSetSchema(schema.ResponseSchema):
-    """ UnetBandwidthPackageSet - DescribeBandwidthPackage
-    """
+class UMemSpaceSetSchema(schema.ResponseSchema):
+    """UMemSpaceSet - DescribeUMemSpace"""
 
     fields = {
-        "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
-        "BandwidthPackageId": fields.Str(
-            required=False, load_from="BandwidthPackageId"
-        ),
+        "Address": fields.List(UMemSpaceAddressSetSchema()),
+        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "DisableTime": fields.Int(required=False, load_from="DisableTime"),
-        "EIPAddr": fields.List(EIPAddrSetSchema()),
-        "EIPId": fields.Str(required=False, load_from="EIPId"),
-        "EnableTime": fields.Int(required=False, load_from="EnableTime"),
-    }
-
-
-class UnetBandwidthUsageEIPSetSchema(schema.ResponseSchema):
-    """ UnetBandwidthUsageEIPSet - DescribeBandwidthUsage
-    """
-
-    fields = {
-        "CurBandwidth": fields.Float(required=False, load_from="CurBandwidth"),
-        "EIPId": fields.Str(required=False, load_from="EIPId"),
-    }
-
-
-class ShareBandwidthSetSchema(schema.ResponseSchema):
-    """ ShareBandwidthSet - DescribeEIP
-    """
-
-    fields = {
-        "ShareBandwidth": fields.Int(
-            required=False, load_from="ShareBandwidth"
-        ),
-        "ShareBandwidthId": fields.Str(
-            required=False, load_from="ShareBandwidthId"
-        ),
-        "ShareBandwidthName": fields.Str(
-            required=False, load_from="ShareBandwidthName"
-        ),
+        "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
+        "Name": fields.Str(required=False, load_from="Name"),
+        "Protocol": fields.Str(required=False, load_from="Protocol"),
+        "RewriteTime": fields.Int(required=True, load_from="RewriteTime"),
+        "Size": fields.Int(required=False, load_from="Size"),
+        "SpaceId": fields.Str(required=False, load_from="SpaceId"),
+        "State": fields.Str(required=False, load_from="State"),
+        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
+        "Tag": fields.Str(required=True, load_from="Tag"),
+        "Type": fields.Str(required=False, load_from="Type"),
+        "UsedSize": fields.Int(required=False, load_from="UsedSize"),
+        "VPCId": fields.Str(required=False, load_from="VPCId"),
+        "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
-class UnetEIPResourceSetSchema(schema.ResponseSchema):
-    """ UnetEIPResourceSet - DescribeEIP
-    """
+class PriceDataSetSchema(schema.ResponseSchema):
+    """PriceDataSet - 升降级价格"""
 
     fields = {
-        "EIPId": fields.Str(required=False, load_from="EIPId"),
-        "ResourceId": fields.Str(required=False, load_from="ResourceId"),
-        "ResourceName": fields.Str(required=False, load_from="ResourceName"),
-        "ResourceType": fields.Str(required=False, load_from="ResourceType"),
-        "SubResourceId": fields.Str(required=False, load_from="SubResourceId"),
-        "SubResourceName": fields.Str(
-            required=False, load_from="SubResourceName"
-        ),
-        "SubResourceType": fields.Str(
-            required=False, load_from="SubResourceType"
-        ),
+        "CustomPrice": fields.Int(required=False, load_from="CustomPrice"),
+        "PurchaseValue": fields.Int(required=False, load_from="PurchaseValue"),
+        "TotalPrice": fields.Int(required=False, load_from="TotalPrice"),
     }
 
 
-class UnetEIPSetSchema(schema.ResponseSchema):
-    """ UnetEIPSet - DescribeEIP
-    """
+class UMemcacheGroupSetSchema(schema.ResponseSchema):
+    """UMemcacheGroupSet - DescribeUMemcacheGroup"""
 
     fields = {
-        "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
-        "BandwidthType": fields.Int(required=False, load_from="BandwidthType"),
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "ConfigId": fields.Str(required=False, load_from="ConfigId"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "EIPAddr": fields.List(UnetEIPAddrSetSchema()),
-        "EIPId": fields.Str(required=False, load_from="EIPId"),
-        "Expire": fields.Bool(required=False, load_from="Expire"),
         "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
+        "GroupId": fields.Str(required=False, load_from="GroupId"),
+        "ModifyTime": fields.Int(required=False, load_from="ModifyTime"),
         "Name": fields.Str(required=False, load_from="Name"),
-        "PayMode": fields.Str(required=False, load_from="PayMode"),
-        "Remark": fields.Str(required=False, load_from="Remark"),
-        "Resource": UnetEIPResourceSetSchema(),
-        "ShareBandwidthSet": ShareBandwidthSetSchema(),
-        "Status": fields.Str(required=False, load_from="Status"),
+        "Port": fields.Int(required=False, load_from="Port"),
+        "Size": fields.Int(required=False, load_from="Size"),
+        "State": fields.Str(required=False, load_from="State"),
+        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
         "Tag": fields.Str(required=False, load_from="Tag"),
-        "Weight": fields.Int(required=False, load_from="Weight"),
+        "UsedSize": fields.Int(required=False, load_from="UsedSize"),
+        "VPCId": fields.Str(required=False, load_from="VPCId"),
+        "Version": fields.Str(required=False, load_from="Version"),
+        "VirtualIP": fields.Str(required=False, load_from="VirtualIP"),
     }
 
 
-class FirewallRuleSetSchema(schema.ResponseSchema):
-    """ FirewallRuleSet - DescribeFirewall
-    """
+class UMemcachePriceSetSchema(schema.ResponseSchema):
+    """UMemcachePriceSet - DescribeUMemcachePrice"""
 
     fields = {
-        "DstPort": fields.Str(required=False, load_from="DstPort"),
-        "Priority": fields.Str(required=False, load_from="Priority"),
-        "ProtocolType": fields.Str(required=False, load_from="ProtocolType"),
-        "Remark": fields.Str(required=False, load_from="Remark"),
-        "RuleAction": fields.Str(required=False, load_from="RuleAction"),
-        "SrcIP": fields.Str(required=False, load_from="SrcIP"),
+        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "ListPrice": fields.Int(required=False, load_from="ListPrice"),
+        "OriginalPrice": fields.Int(required=False, load_from="OriginalPrice"),
+        "Price": fields.Int(required=False, load_from="Price"),
     }
 
 
-class FirewallDataSetSchema(schema.ResponseSchema):
-    """ FirewallDataSet - DescribeFirewall
-    """
+class URedisBackupSetSchema(schema.ResponseSchema):
+    """URedisBackupSet - DescribeURedisBackup"""
 
     fields = {
-        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "FWId": fields.Str(required=True, load_from="FWId"),
-        "GroupId": fields.Str(required=True, load_from="GroupId"),
-        "Name": fields.Str(required=False, load_from="Name"),
-        "Remark": fields.Str(required=False, load_from="Remark"),
-        "ResourceCount": fields.Int(required=False, load_from="ResourceCount"),
-        "Rule": fields.List(FirewallRuleSetSchema()),
-        "Tag": fields.Str(required=False, load_from="Tag"),
-        "Type": fields.Str(required=False, load_from="Type"),
+        "BackupId": fields.Str(required=False, load_from="BackupId"),
+        "BackupName": fields.Str(required=False, load_from="BackupName"),
+        "BackupSize": fields.Int(required=False, load_from="BackupSize"),
+        "BackupTime": fields.Int(required=False, load_from="BackupTime"),
+        "BackupType": fields.Str(required=False, load_from="BackupType"),
+        "GroupId": fields.Str(required=False, load_from="GroupId"),
+        "GroupName": fields.Str(required=False, load_from="GroupName"),
+        "State": fields.Str(required=False, load_from="State"),
+        "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
-class ResourceSetSchema(schema.ResponseSchema):
-    """ ResourceSet - 资源信息
-    """
+class URedisConfigSetSchema(schema.ResponseSchema):
+    """URedisConfigSet - 主备Redis配置文件信息"""
 
     fields = {
+        "ConfigId": fields.Str(required=False, load_from="ConfigId"),
+        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
+        "Description": fields.Str(required=False, load_from="Description"),
+        "IsModify": fields.Str(required=False, load_from="IsModify"),
+        "ModifyTime": fields.Int(required=False, load_from="ModifyTime"),
         "Name": fields.Str(required=False, load_from="Name"),
-        "PrivateIP": fields.Str(required=False, load_from="PrivateIP"),
-        "Remark": fields.Str(required=False, load_from="Remark"),
-        "ResourceID": fields.Str(required=False, load_from="ResourceID"),
-        "ResourceType": fields.Str(required=False, load_from="ResourceType"),
-        "Status": fields.Int(required=False, load_from="Status"),
-        "Tag": fields.Str(required=False, load_from="Tag"),
-        "Zone": fields.Int(required=False, load_from="Zone"),
-    }
-
-
-class EIPSetDataSchema(schema.ResponseSchema):
-    """ EIPSetData - describeShareBandwidth
-    """
-
-    fields = {
-        "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
-        "EIPAddr": fields.List(EIPAddrSetSchema()),
-        "EIPId": fields.Str(required=False, load_from="EIPId"),
+        "RegionFlag": fields.Bool(required=False, load_from="RegionFlag"),
+        "State": fields.Str(required=False, load_from="State"),
+        "Version": fields.Str(required=False, load_from="Version"),
+        "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
-class UnetShareBandwidthSetSchema(schema.ResponseSchema):
-    """ UnetShareBandwidthSet - DescribeShareBandwidth
-    """
+class URedisGroupSetSchema(schema.ResponseSchema):
+    """URedisGroupSet - DescribeURedisGroup"""
 
     fields = {
-        "BandwidthGuarantee": fields.Int(
-            required=False, load_from="BandwidthGuarantee"
-        ),
+        "AutoBackup": fields.Str(required=False, load_from="AutoBackup"),
+        "BackupTime": fields.Int(required=False, load_from="BackupTime"),
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "ConfigId": fields.Str(required=False, load_from="ConfigId"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "EIPSet": fields.List(EIPSetDataSchema()),
         "ExpireTime": fields.Int(required=False, load_from="ExpireTime"),
-        "Name": fields.Str(required=False, load_from="Name"),
-        "PostPayStartTime": fields.Int(
-            required=False, load_from="PostPayStartTime"
-        ),
-        "ShareBandwidth": fields.Int(
-            required=False, load_from="ShareBandwidth"
-        ),
-        "ShareBandwidthId": fields.Str(
-            required=False, load_from="ShareBandwidthId"
+        "GroupId": fields.Str(required=False, load_from="GroupId"),
+        "GroupName": fields.Str(required=False, load_from="GroupName"),
+        "HighAvailability": fields.Str(
+            required=False, load_from="HighAvailability"
         ),
+        "MemorySize": fields.Int(required=False, load_from="MemorySize"),
+        "ModifyTime": fields.Int(required=False, load_from="ModifyTime"),
+        "Name": fields.Str(required=False, load_from="Name"),
+        "Port": fields.Int(required=False, load_from="Port"),
+        "Protocol": fields.Str(required=False, load_from="Protocol"),
+        "RewriteTime": fields.Int(required=True, load_from="RewriteTime"),
+        "Role": fields.Str(required=True, load_from="Role"),
+        "Size": fields.Int(required=False, load_from="Size"),
+        "SlaveZone": fields.Str(required=False, load_from="SlaveZone"),
+        "State": fields.Str(required=False, load_from="State"),
+        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
+        "Tag": fields.Str(required=False, load_from="Tag"),
+        "Type": fields.Str(required=False, load_from="Type"),
+        "UsedSize": fields.Int(required=False, load_from="UsedSize"),
+        "VPCId": fields.Str(required=True, load_from="VPCId"),
+        "Version": fields.Str(required=False, load_from="Version"),
+        "VirtualIP": fields.Str(required=False, load_from="VirtualIP"),
+        "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
-class VIPDetailSetSchema(schema.ResponseSchema):
-    """ VIPDetailSet - VIPDetailSet
-    """
+class URedisPriceSetSchema(schema.ResponseSchema):
+    """URedisPriceSet - 主备Redis价格"""
 
     fields = {
-        "CreateTime": fields.Int(required=False, load_from="CreateTime"),
-        "Name": fields.Str(required=False, load_from="Name"),
-        "RealIp": fields.Str(required=False, load_from="RealIp"),
-        "SubnetId": fields.Str(required=False, load_from="SubnetId"),
-        "VIP": fields.Str(required=False, load_from="VIP"),
-        "VIPId": fields.Str(required=False, load_from="VIPId"),
-        "VPCId": fields.Str(required=False, load_from="VPCId"),
-        "Zone": fields.Str(required=False, load_from="Zone"),
+        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
+        "ListPrice": fields.Int(required=False, load_from="ListPrice"),
+        "OriginalPrice": fields.Int(required=True, load_from="OriginalPrice"),
+        "Price": fields.Int(required=False, load_from="Price"),
     }
 
 
-class EIPPayModeSetSchema(schema.ResponseSchema):
-    """ EIPPayModeSet - GetEIPPayModeEIP
-    """
+class URedisSlowlogSetSchema(schema.ResponseSchema):
+    """URedisSlowlogSet - DescribeURedisSlowlog"""
 
     fields = {
-        "EIPId": fields.Str(required=False, load_from="EIPId"),
-        "EIPPayMode": fields.Str(required=False, load_from="EIPPayMode"),
+        "Command": fields.Str(required=False, load_from="Command"),
+        "SpendTime": fields.Int(required=False, load_from="SpendTime"),
+        "StartTime": fields.Int(required=False, load_from="StartTime"),
     }
 
 
-class EIPPriceDetailSetSchema(schema.ResponseSchema):
-    """ EIPPriceDetailSet - GetEIPPrice
-    """
+class URedisVersionSetSchema(schema.ResponseSchema):
+    """URedisVersionSet - DescribeURedisVersion"""
 
     fields = {
-        "ChargeType": fields.Str(required=False, load_from="ChargeType"),
-        "Price": fields.Float(required=False, load_from="Price"),
-        "PurchaseValue": fields.Int(required=False, load_from="PurchaseValue"),
+        "Version": fields.Str(required=False, load_from="Version"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uphost/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uphost/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,98 +12,98 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(UPHostClient, self).__init__(
             config, transport, middleware, logger
         )
 
     def create_phost(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreatePHost - 指定数据中心，根据资源使用量创建指定数量的UPHost物理云主机实例。
+        """CreatePHost - 指定数据中心，根据资源使用量创建指定数量的UPHost物理云主机实例。
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ImageId** (str) - (Required) 镜像ID。 请通过 [DescribePHostImage]获取
         - **Password** (str) - (Required) 密码（密码需使用base64进行编码）
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - 计费模式，枚举值为：year, 按年付费； month,按月付费；dynamic，按需付费，（需开启权限） trial, 试用（需开启权限）。默认为按月付费
         - **Cluster** (str) - 网络环境，可选千兆：1G ，万兆：10G， 默认1G
         - **Count** (int) - 购买数量，默认为1，（暂不支持）
         - **CouponId** (str) - 代金券
         - **Name** (str) - 物理机名称，默认为phost
         - **Quantity** (str) - 购买时长，默认为1，范围[1-10]
         - **Raid** (str) - Raid配置，默认Raid10  支持:Raid0、Raid1、Raid5、Raid10，NoRaid
         - **Remark** (str) - 物理机备注，默认为空
-        - **SecurityGroupId** (str) - 防火墙Id，默认：Web推荐防火墙。如何查询SecurityGroupId请参见  `DescribeSecurityGroup <https://docs.ucloud.cn/api/unet-api/describe_security_group.html>`_ 
+        - **SecurityGroupId** (str) - 防火墙Id，默认：Web推荐防火墙。如何查询SecurityGroupId请参见  `DescribeSecurityGroup <https://docs.ucloud.cn/api/unet-api/describe_security_group.html>`_
         - **SubnetId** (str) - 子网ID，不填为默认，VPC2.0下需要填写此字段。
         - **Tag** (str) - 业务组，默认为default
         - **Type** (str) - 物理机类型，默认为：db-2(基础型-SAS-V3)
         - **VPCId** (str) - VPC ID，不填为默认，VPC2.0下需要填写此字段。
-        
+
         **Response**
 
         - **PHostId** (list) - PHost的资源ID数组
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreatePHostRequestSchema().dumps(d)
 
         resp = self.invoke("CreatePHost", d, **kwargs)
         return apis.CreatePHostResponseSchema().loads(resp)
 
     def describe_phost(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribePHost - 获取物理机详细信息
+        """DescribePHost - 获取物理机详细信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) - 返回数据长度，默认为20
         - **Offset** (int) - 数据偏移量，默认为0
         - **PHostId** (list) - PHost资源ID，若为空，则返回当前Region所有PHost。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PHostSet** (list) - 见 **PHostSet** 模型定义
         - **TotalCount** (int) - 满足条件的PHost总数
-        
+
         **Response Model**
-        
-        **PHostCPUSet** 
-        
+
+        **PHostCPUSet**
+
         - **CoreCount** (int) - CPU核数
         - **Count** (int) - CPU个数
         - **Frequence** (float) - CPU主频
         - **Model** (str) - CPU型号
 
-        **PHostDiskSet** 
-        
+        **PHostDiskSet**
+
         - **Count** (int) - 磁盘数量
         - **IOCap** (int) - 磁盘IO性能，单位MB/s（待废弃）
         - **Name** (str) - 磁盘名称，sys/data
         - **Space** (int) - 单盘大小，单位GB
         - **Type** (str) - 磁盘属性
 
-        **PHostIPSet** 
-        
+        **PHostIPSet**
+
         - **Bandwidth** (int) - IP对应带宽，单位Mb，内网IP不显示带宽信息
         - **IPAddr** (str) - IP地址，
         - **IPId** (str) - IP资源ID(内网IP无资源ID)（待废弃）
         - **MACAddr** (str) - MAC地址
         - **OperatorName** (str) - 国际: Internation， BGP: BGP， 内网: Private
         - **SubnetId** (str) - 子网ID
         - **VPCId** (str) - VPC ID
 
-        **PHostSet** 
-        
+        **PHostSet**
+
         - **AutoRenew** (str) - 自动续费
         - **CPUSet** (dict) - 见 **PHostCPUSet** 模型定义
         - **ChargeType** (str) - 计费模式，枚举值为： Year，按年付费； Month，按月付费； Dynamic，按需付费（需开启权限）； Trial，试用（需开启权限）默认为月付
         - **Cluster** (str) - 网络环境。枚举值：千兆：1G ，万兆：10G
         - **Components** (str) - 组件信息（暂不支持）
         - **CreateTime** (int) - 创建时间
         - **DiskSet** (list) - 见 **PHostDiskSet** 模型定义
@@ -119,49 +119,49 @@
         - **PHostType** (str) - 物理机类型，参见DescribePHostMachineType返回值
         - **PMStatus** (str) - 物理云主机状态。枚举值：\\ > 初始化:Initializing; \\ > 启动中：Starting； \\ > 运行中：Running；\\ > 关机中：Stopping； \\ > 安装失败：InstallFailed； \\ > 重启中：Rebooting；\\ > 关机：Stopped；
         - **PowerState** (str) - 电源状态，on 或 off
         - **RaidSupported** (str) - 是否支持Raid。枚举值：Yes：支持；No：不支持。
         - **Remark** (str) - 物理机备注
         - **SN** (str) - 物理机序列号
         - **Tag** (str) - 业务组
-        - **Zone** (str) - 可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - 可用区，参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DescribePHostRequestSchema().dumps(d)
 
         resp = self.invoke("DescribePHost", d, **kwargs)
         return apis.DescribePHostResponseSchema().loads(resp)
 
     def describe_phost_image(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribePHostImage - 获取物理云主机镜像列表
+        """DescribePHostImage - 获取物理云主机镜像列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ImageId** (list) - 镜像ID
         - **ImageType** (str) - 镜像类别，枚举为：Base,标准镜像；默认为标准镜像。
         - **Limit** (int) - 返回数据长度，默认为20
         - **Offset** (int) - 数据偏移量，默认为0
-        
+
         **Response**
 
         - **ImageSet** (list) - 见 **PHostImageSet** 模型定义
         - **TotalCount** (int) - 满足条件的镜像总数
-        
+
         **Response Model**
-        
-        **PHostImageSet** 
-        
+
+        **PHostImageSet**
+
         - **ImageId** (str) - 镜像ID
         - **ImageName** (str) - 镜像名称
         - **OsName** (str) - 操作系统名称
         - **OsType** (str) - 操作系统类型
 
         """
         # build request
@@ -171,31 +171,31 @@
 
         resp = self.invoke("DescribePHostImage", d, **kwargs)
         return apis.DescribePHostImageResponseSchema().loads(resp)
 
     def describe_phost_tags(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribePHostTags - 获取物理机tag列表（业务组）
+        """DescribePHostTags - 获取物理机tag列表（业务组）
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **TagSet** (list) - 见 **PHostTagSet** 模型定义
         - **TotalCount** (int) - Tag的个数
-        
+
         **Response Model**
-        
-        **PHostTagSet** 
-        
+
+        **PHostTagSet**
+
         - **Tag** (str) - 业务组名称
         - **TotalCount** (int) - 该业务组中包含的主机个数
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
@@ -203,35 +203,35 @@
 
         resp = self.invoke("DescribePHostTags", d, **kwargs)
         return apis.DescribePHostTagsResponseSchema().loads(resp)
 
     def get_phost_price(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetPHostPrice - 获取物理机价格列表
+        """GetPHostPrice - 获取物理机价格列表
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ChargeType** (str) - (Required) 计费模式，枚举值为： Year/Month/Trial/Dynamic
         - **Count** (int) - (Required) 购买数量，范围[1-5]
         - **Quantity** (int) - (Required) 购买时长，1-10个月或1-10年
         - **Cluster** (str) - 网络环境，可选千兆：1G ，万兆：10G
         - **Type** (str) - 默认为：DB(数据库型)
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PriceSet** (list) - 见 **PHostPriceSet** 模型定义
-        
+
         **Response Model**
-        
-        **PHostPriceSet** 
-        
+
+        **PHostPriceSet**
+
         - **ChargeType** (str) - Year/Month/Trial/Dynamic
         - **Price** (float) - 价格, 单位:元, 保留小数点后两位有效数字
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
@@ -239,159 +239,159 @@
 
         resp = self.invoke("GetPHostPrice", d, **kwargs)
         return apis.GetPHostPriceResponseSchema().loads(resp)
 
     def modify_phost_info(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyPHostInfo - 更改物理机信息
+        """ModifyPHostInfo - 更改物理机信息
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PHostId** (str) - (Required) 物理机资源ID
         - **Name** (str) - 物理机名称，默认不更改
         - **Remark** (str) - 物理机备注，默认不更改
         - **Tag** (str) - 业务组，默认不更改
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PHostId** (str) - PHost 的资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ModifyPHostInfoRequestSchema().dumps(d)
 
         resp = self.invoke("ModifyPHostInfo", d, **kwargs)
         return apis.ModifyPHostInfoResponseSchema().loads(resp)
 
     def poweroff_phost(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ PoweroffPHost - 断电物理云主机
+        """PoweroffPHost - 断电物理云主机
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PHostId** (str) - (Required) PHost资源ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PHostId** (str) - PHost 的资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.PoweroffPHostRequestSchema().dumps(d)
 
         resp = self.invoke("PoweroffPHost", d, **kwargs)
         return apis.PoweroffPHostResponseSchema().loads(resp)
 
     def reboot_phost(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ RebootPHost - 重启物理机
+        """RebootPHost - 重启物理机
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PHostId** (str) - (Required) PHost资源ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PHostId** (str) - PHost 的资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.RebootPHostRequestSchema().dumps(d)
 
         resp = self.invoke("RebootPHost", d, **kwargs)
         return apis.RebootPHostResponseSchema().loads(resp)
 
     def reinstall_phost(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ReinstallPHost - 重装物理机操作系统
+        """ReinstallPHost - 重装物理机操作系统
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PHostId** (str) - (Required) PHost资源ID
         - **Password** (str) - (Required) 密码
-        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **Zone** (str) - (Required) 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **ImageId** (str) - 镜像Id，参考镜像列表，默认使用原镜像
         - **Name** (str) - 物理机名称，默认不更改
         - **Raid** (str) - 不保留数据盘重装，可选Raid
         - **Remark** (str) - 物理机备注，默认为不更改。
         - **ReserveDisk** (str) - 是否保留数据盘，保留：Yes，不报留：No， 默认：Yes
         - **Tag** (str) - 业务组，默认不更改。
-        
+
         **Response**
 
         - **PHostId** (str) - PHost 的资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.ReinstallPHostRequestSchema().dumps(d)
 
         resp = self.invoke("ReinstallPHost", d, **kwargs)
         return apis.ReinstallPHostResponseSchema().loads(resp)
 
     def start_phost(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ StartPHost - 启动物理机
+        """StartPHost - 启动物理机
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PHostId** (str) - (Required) PHost资源ID
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PHostId** (str) - PHost 的资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.StartPHostRequestSchema().dumps(d)
 
         resp = self.invoke("StartPHost", d, **kwargs)
         return apis.StartPHostResponseSchema().loads(resp)
 
     def terminate_phost(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ TerminatePHost - 删除物理云主机
+        """TerminatePHost - 删除物理云主机
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PHostId** (str) - (Required) PHost资源ID
         - **ReleaseEIP** (bool) - 是否释放绑定的EIP。true: 解绑EIP后，并释放；其他值或不填：解绑EIP。
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **PHostId** (str) - PHost 的资源ID
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.TerminatePHostRequestSchema().dumps(d)
 
         resp = self.invoke("TerminatePHost", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uphost/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uphost/schemas/apis.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 API: CreatePHost
 
 指定数据中心，根据资源使用量创建指定数量的UPHost物理云主机实例。
 """
 
 
 class CreatePHostRequestSchema(schema.RequestSchema):
-    """ CreatePHost - 指定数据中心，根据资源使用量创建指定数量的UPHost物理云主机实例。
-    """
+    """CreatePHost - 指定数据中心，根据资源使用量创建指定数量的UPHost物理云主机实例。"""
 
     fields = {
         "ChargeType": fields.Str(required=False, dump_to="ChargeType"),
         "Cluster": fields.Str(required=False, dump_to="Cluster"),
         "Count": fields.Int(required=False, dump_to="Count"),
         "CouponId": fields.Str(required=False, dump_to="CouponId"),
         "ImageId": fields.Str(required=True, dump_to="ImageId"),
@@ -40,16 +39,15 @@
         "Type": fields.Str(required=False, dump_to="Type"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class CreatePHostResponseSchema(schema.ResponseSchema):
-    """ CreatePHost - 指定数据中心，根据资源使用量创建指定数量的UPHost物理云主机实例。
-    """
+    """CreatePHost - 指定数据中心，根据资源使用量创建指定数量的UPHost物理云主机实例。"""
 
     fields = {
         "PHostId": fields.List(
             fields.Str(), required=False, load_from="PHostId"
         )
     }
 
@@ -58,30 +56,28 @@
 API: DescribePHost
 
 获取物理机详细信息
 """
 
 
 class DescribePHostRequestSchema(schema.RequestSchema):
-    """ DescribePHost - 获取物理机详细信息
-    """
+    """DescribePHost - 获取物理机详细信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "PHostId": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribePHostResponseSchema(schema.ResponseSchema):
-    """ DescribePHost - 获取物理机详细信息
-    """
+    """DescribePHost - 获取物理机详细信息"""
 
     fields = {
         "PHostSet": fields.List(
             models.PHostSetSchema(), required=False, load_from="PHostSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -91,31 +87,29 @@
 API: DescribePHostImage
 
 获取物理云主机镜像列表
 """
 
 
 class DescribePHostImageRequestSchema(schema.RequestSchema):
-    """ DescribePHostImage - 获取物理云主机镜像列表
-    """
+    """DescribePHostImage - 获取物理云主机镜像列表"""
 
     fields = {
         "ImageId": fields.List(fields.Str()),
         "ImageType": fields.Str(required=False, dump_to="ImageType"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class DescribePHostImageResponseSchema(schema.ResponseSchema):
-    """ DescribePHostImage - 获取物理云主机镜像列表
-    """
+    """DescribePHostImage - 获取物理云主机镜像列表"""
 
     fields = {
         "ImageSet": fields.List(
             models.PHostImageSetSchema(), required=False, load_from="ImageSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -125,27 +119,25 @@
 API: DescribePHostTags
 
 获取物理机tag列表（业务组）
 """
 
 
 class DescribePHostTagsRequestSchema(schema.RequestSchema):
-    """ DescribePHostTags - 获取物理机tag列表（业务组）
-    """
+    """DescribePHostTags - 获取物理机tag列表（业务组）"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DescribePHostTagsResponseSchema(schema.ResponseSchema):
-    """ DescribePHostTags - 获取物理机tag列表（业务组）
-    """
+    """DescribePHostTags - 获取物理机tag列表（业务组）"""
 
     fields = {
         "TagSet": fields.List(
             models.PHostTagSetSchema(), required=False, load_from="TagSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -155,32 +147,30 @@
 API: GetPHostPrice
 
 获取物理机价格列表
 """
 
 
 class GetPHostPriceRequestSchema(schema.RequestSchema):
-    """ GetPHostPrice - 获取物理机价格列表
-    """
+    """GetPHostPrice - 获取物理机价格列表"""
 
     fields = {
         "ChargeType": fields.Str(required=True, dump_to="ChargeType"),
         "Cluster": fields.Str(required=False, dump_to="Cluster"),
         "Count": fields.Int(required=True, dump_to="Count"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Quantity": fields.Int(required=True, dump_to="Quantity"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Type": fields.Str(required=False, dump_to="Type"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class GetPHostPriceResponseSchema(schema.ResponseSchema):
-    """ GetPHostPrice - 获取物理机价格列表
-    """
+    """GetPHostPrice - 获取物理机价格列表"""
 
     fields = {
         "PriceSet": fields.List(
             models.PHostPriceSetSchema(), required=False, load_from="PriceSet"
         )
     }
 
@@ -189,97 +179,90 @@
 API: ModifyPHostInfo
 
 更改物理机信息
 """
 
 
 class ModifyPHostInfoRequestSchema(schema.RequestSchema):
-    """ ModifyPHostInfo - 更改物理机信息
-    """
+    """ModifyPHostInfo - 更改物理机信息"""
 
     fields = {
         "Name": fields.Str(required=False, dump_to="Name"),
         "PHostId": fields.Str(required=True, dump_to="PHostId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class ModifyPHostInfoResponseSchema(schema.ResponseSchema):
-    """ ModifyPHostInfo - 更改物理机信息
-    """
+    """ModifyPHostInfo - 更改物理机信息"""
 
     fields = {"PHostId": fields.Str(required=False, load_from="PHostId")}
 
 
 """
 API: PoweroffPHost
 
 断电物理云主机
 """
 
 
 class PoweroffPHostRequestSchema(schema.RequestSchema):
-    """ PoweroffPHost - 断电物理云主机
-    """
+    """PoweroffPHost - 断电物理云主机"""
 
     fields = {
         "PHostId": fields.Str(required=True, dump_to="PHostId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class PoweroffPHostResponseSchema(schema.ResponseSchema):
-    """ PoweroffPHost - 断电物理云主机
-    """
+    """PoweroffPHost - 断电物理云主机"""
 
     fields = {"PHostId": fields.Str(required=False, load_from="PHostId")}
 
 
 """
 API: RebootPHost
 
 重启物理机
 """
 
 
 class RebootPHostRequestSchema(schema.RequestSchema):
-    """ RebootPHost - 重启物理机
-    """
+    """RebootPHost - 重启物理机"""
 
     fields = {
         "PHostId": fields.Str(required=True, dump_to="PHostId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class RebootPHostResponseSchema(schema.ResponseSchema):
-    """ RebootPHost - 重启物理机
-    """
+    """RebootPHost - 重启物理机"""
 
     fields = {"PHostId": fields.Str(required=False, load_from="PHostId")}
 
 
 """
 API: ReinstallPHost
 
 重装物理机操作系统
 """
 
 
 class ReinstallPHostRequestSchema(schema.RequestSchema):
-    """ ReinstallPHost - 重装物理机操作系统
-    """
+    """ReinstallPHost - 重装物理机操作系统"""
 
     fields = {
         "ImageId": fields.Str(required=False, dump_to="ImageId"),
         "Name": fields.Str(required=False, dump_to="Name"),
         "PHostId": fields.Str(required=True, dump_to="PHostId"),
         "Password": fields.Str(required=True, dump_to="Password"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
@@ -289,64 +272,59 @@
         "ReserveDisk": fields.Str(required=False, dump_to="ReserveDisk"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "Zone": fields.Str(required=True, dump_to="Zone"),
     }
 
 
 class ReinstallPHostResponseSchema(schema.ResponseSchema):
-    """ ReinstallPHost - 重装物理机操作系统
-    """
+    """ReinstallPHost - 重装物理机操作系统"""
 
     fields = {"PHostId": fields.Str(required=False, load_from="PHostId")}
 
 
 """
 API: StartPHost
 
 启动物理机
 """
 
 
 class StartPHostRequestSchema(schema.RequestSchema):
-    """ StartPHost - 启动物理机
-    """
+    """StartPHost - 启动物理机"""
 
     fields = {
         "PHostId": fields.Str(required=True, dump_to="PHostId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class StartPHostResponseSchema(schema.ResponseSchema):
-    """ StartPHost - 启动物理机
-    """
+    """StartPHost - 启动物理机"""
 
     fields = {"PHostId": fields.Str(required=False, load_from="PHostId")}
 
 
 """
 API: TerminatePHost
 
 删除物理云主机
 """
 
 
 class TerminatePHostRequestSchema(schema.RequestSchema):
-    """ TerminatePHost - 删除物理云主机
-    """
+    """TerminatePHost - 删除物理云主机"""
 
     fields = {
         "PHostId": fields.Str(required=True, dump_to="PHostId"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ReleaseEIP": fields.Bool(required=False, dump_to="ReleaseEIP"),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class TerminatePHostResponseSchema(schema.ResponseSchema):
-    """ TerminatePHost - 删除物理云主机
-    """
+    """TerminatePHost - 删除物理云主机"""
 
     fields = {"PHostId": fields.Str(required=False, load_from="PHostId")}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/uphost/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/uphost/schemas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class PHostIPSetSchema(schema.ResponseSchema):
-    """ PHostIPSet - DescribePHost
-    """
+    """PHostIPSet - DescribePHost"""
 
     fields = {
         "Bandwidth": fields.Int(required=False, load_from="Bandwidth"),
         "IPAddr": fields.Str(required=False, load_from="IPAddr"),
         "IPId": fields.Str(required=False, load_from="IPId"),
         "MACAddr": fields.Str(required=False, load_from="MACAddr"),
         "OperatorName": fields.Str(required=False, load_from="OperatorName"),
         "SubnetId": fields.Str(required=False, load_from="SubnetId"),
         "VPCId": fields.Str(required=False, load_from="VPCId"),
     }
 
 
 class PHostDiskSetSchema(schema.ResponseSchema):
-    """ PHostDiskSet - GetPHostTypeInfo
-    """
+    """PHostDiskSet - GetPHostTypeInfo"""
 
     fields = {
         "Count": fields.Int(required=False, load_from="Count"),
         "IOCap": fields.Int(required=False, load_from="IOCap"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Space": fields.Int(required=False, load_from="Space"),
         "Type": fields.Str(required=False, load_from="Type"),
     }
 
 
 class PHostCPUSetSchema(schema.ResponseSchema):
-    """ PHostCPUSet - DescribePHost
-    """
+    """PHostCPUSet - DescribePHost"""
 
     fields = {
         "CoreCount": fields.Int(required=False, load_from="CoreCount"),
         "Count": fields.Int(required=False, load_from="Count"),
         "Frequence": fields.Float(required=False, load_from="Frequence"),
         "Model": fields.Str(required=False, load_from="Model"),
     }
 
 
 class PHostSetSchema(schema.ResponseSchema):
-    """ PHostSet - DescribePHost
-    """
+    """PHostSet - DescribePHost"""
 
     fields = {
         "AutoRenew": fields.Str(required=False, load_from="AutoRenew"),
         "CPUSet": PHostCPUSetSchema(),
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
         "Cluster": fields.Str(required=False, load_from="Cluster"),
         "Components": fields.Str(required=False, load_from="Components"),
@@ -72,36 +68,33 @@
         "SN": fields.Str(required=False, load_from="SN"),
         "Tag": fields.Str(required=False, load_from="Tag"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class PHostImageSetSchema(schema.ResponseSchema):
-    """ PHostImageSet - DescribePHostImage
-    """
+    """PHostImageSet - DescribePHostImage"""
 
     fields = {
         "ImageId": fields.Str(required=False, load_from="ImageId"),
         "ImageName": fields.Str(required=False, load_from="ImageName"),
         "OsName": fields.Str(required=False, load_from="OsName"),
         "OsType": fields.Str(required=False, load_from="OsType"),
     }
 
 
 class PHostTagSetSchema(schema.ResponseSchema):
-    """ PHostTagSet - DescribePHostTags
-    """
+    """PHostTagSet - DescribePHostTags"""
 
     fields = {
         "Tag": fields.Str(required=False, load_from="Tag"),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
 
 
 class PHostPriceSetSchema(schema.ResponseSchema):
-    """ PHostPriceSet - GetPHostPrice
-    """
+    """PHostPriceSet - GetPHostPrice"""
 
     fields = {
         "ChargeType": fields.Str(required=False, load_from="ChargeType"),
         "Price": fields.Float(required=False, load_from="Price"),
     }
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/usms/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/usms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,33 +12,33 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(USMSClient, self).__init__(config, transport, middleware, logger)
 
     def create_usms_signature(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUSMSSignature - 调用接口CreateUSMSSignature申请短信签名
+        """CreateUSMSSignature - 调用接口CreateUSMSSignature申请短信签名
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **CertificateType** (int) - (Required) 签名的资质证明文件类型，需与签名类型保持一致，说明如下：0-三证合一/企业营业执照/组织机构代码证书/社会信用代码证书；1-应用商店后台开发者管理截图；2-备案服务商的备案成功截图(含域名，网站名称，备案号)；3-公众号或小程序的管理界面截图；4-商标注册证书；5-组织机构代码证书、社会信用代码证书；
         - **Description** (str) - (Required) 短信签名申请原因
         - **File** (str) - (Required) 短信签名的资质证明文件，需先进行base64编码格式转换，此处填写转换后的字符串。文件大小不超过4 MB
         - **SigContent** (str) - (Required) 短信签名名称；长度为2-12个字符, 可包含中文、数字和符号；无需填写【】或[]，系统会自动添加
         - **SigPurpose** (int) - (Required) 签名用途，0-自用，1-他用；
         - **SigType** (int) - (Required) 签名类型，说明如下：0-公司或企业的全称或简称；1-App应用的全称或简称；2-工信部备案网站的全称或简称；3-公众号或小程序的全称或简称；4-商标名的全称或简称；5-政府/机关事业单位/其他单位的全称或简称；
         - **ProxyFile** (str) - 短信签名授权委托文件，需先进行base64编码格式转换，此处填写转换后的字符串。文件大小不超过4 MB；当您是代理并使用第三方的签名时（也即SigPurpose为1-他用），该项为必填项；
-        
+
         **Response**
 
         - **Message** (str) - 返回状态码描述，如果操作成功，默认返回为空
         - **SigContent** (str) - 短信签名名称
         - **SigId** (str) - 短信签名ID（短信签名申请时的工单ID）
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.CreateUSMSSignatureRequestSchema().dumps(d)
 
         # build options
@@ -46,32 +46,32 @@
 
         resp = self.invoke("CreateUSMSSignature", d, **kwargs)
         return apis.CreateUSMSSignatureResponseSchema().loads(resp)
 
     def create_usms_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateUSMSTemplate - 调用接口CreateUSMSTemplate申请短信模板
+        """CreateUSMSTemplate - 调用接口CreateUSMSTemplate申请短信模板
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Purpose** (int) - (Required) 短信模板用途类型：1-验证码类短信模板；2-系统通知类短信模板；3-会员推广类短信模板；
         - **Template** (str) - (Required) 短信模板内容，说明如下：字数不超过500，每个中文、符号、英文、数组等都计为一个字；模板中的变量填写格式：{N}，其中N为大于1的整数，有多个参数时，建议N从1开始顺次，例如：{1}、{2}等；短信模板禁止仅包括变量的情况；
         - **TemplateName** (str) - (Required) 短信模板名称，不超过32个字符，每个中文、符号、英文、数字等都计为1个字。
         - **Remark** (str) - 短信模板申请原因说明，字数不超过128，每个中文、符号、英文、数字等都计为1个字。
         - **UnsubscribeInfo** (str) - 当Purpose为3时，也即会员推广类短信模板，该项必填。枚举值：TD退订、回T退订、回N退订、回TD退订、退订回T、退订回D、退订回TD、退订回复T、退订回复D、退订回复N、退订回复TD、拒收回T
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Message** (str) - 返回状态码描述，如果操作成功，默认返回为空
         - **TemplateId** (str) - 短信模板ID（短信模板申请时的工单ID）
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.CreateUSMSTemplateRequestSchema().dumps(d)
 
         # build options
@@ -79,88 +79,88 @@
 
         resp = self.invoke("CreateUSMSTemplate", d, **kwargs)
         return apis.CreateUSMSTemplateResponseSchema().loads(resp)
 
     def delete_usms_signature(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUSMSSignature - 调用接口DeleteUSMSSignature删除短信签名
+        """DeleteUSMSSignature - 调用接口DeleteUSMSSignature删除短信签名
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **SigIds** (list) - (Required) 签名ID（也即短信签名申请时的工单ID），支持以数组的方式，举例，以SigIds.0、SigIds.1...SigIds.N方式传入
-        
+
         **Response**
 
         - **Message** (str) - 返回状态码描述，如果操作成功，默认返回为空
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.DeleteUSMSSignatureRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUSMSSignature", d, **kwargs)
         return apis.DeleteUSMSSignatureResponseSchema().loads(resp)
 
     def delete_usms_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteUSMSTemplate - 调用接口DeleteUSMSTemplate删除短信模板
+        """DeleteUSMSTemplate - 调用接口DeleteUSMSTemplate删除短信模板
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **TemplateIds** (list) - (Required) 模板ID（也即短信模板申请时的工单ID），支持以数组的方式，举例，以TemplateIds.0、TemplateIds.1...TemplateIds.N方式传入
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Message** (str) - 返回状态码描述，如果操作成功，默认返回为空
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.DeleteUSMSTemplateRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteUSMSTemplate", d, **kwargs)
         return apis.DeleteUSMSTemplateResponseSchema().loads(resp)
 
     def get_usms_send_receipt(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ GetUSMSSendReceipt - 获取短信发送回执信息。下游服务提供商回执信息返回会有一定延时，建议发送完短信以后，5-10分钟后再调用该接口拉取回执信息。若超过12小时未返回，则请联系技术支持确认原因
+        """GetUSMSSendReceipt - 获取短信发送回执信息。下游服务提供商回执信息返回会有一定延时，建议发送完短信以后，5-10分钟后再调用该接口拉取回执信息。若超过12小时未返回，则请联系技术支持确认原因
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SessionNoSet** (list) - (Required) 发送短信时返回的SessionNo集合，SessionNoSet.0,SessionNoSet.1....格式
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Data** (list) - 见 **ReceiptPerSession** 模型定义
         - **Message** (str) - 错误描述
-        
+
         **Response Model**
-        
-        **ReceiptPerPhone** 
-        
+
+        **ReceiptPerPhone**
+
         - **CostCount** (int) - 消耗短信条数
         - **Phone** (str) - 手机号码
         - **ReceiptDesc** (str) - 回执结果描述
         - **ReceiptResult** (str) - 回执结果
         - **ReceiptTime** (int) - 回执返回时间
 
-        **ReceiptPerSession** 
-        
+        **ReceiptPerSession**
+
         - **ReceiptSet** (list) - 见 **ReceiptPerPhone** 模型定义
         - **SessionNo** (str) - 发送短信时返回的SessionNo
 
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
@@ -168,31 +168,31 @@
 
         resp = self.invoke("GetUSMSSendReceipt", d, **kwargs)
         return apis.GetUSMSSendReceiptResponseSchema().loads(resp)
 
     def query_usms_signature(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ QueryUSMSSignature - 调用接口QueryUSMSSignature查询短信签名申请状态
+        """QueryUSMSSignature - 调用接口QueryUSMSSignature查询短信签名申请状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **SigContent** (str) - 签名内容；签名ID和签名至少需填写1项；
         - **SigId** (str) - 已申请的短信签名ID（短信签名申请时的工单ID）；签名ID和签名至少需填写1项；
-        
+
         **Response**
 
         - **Data** (dict) - 见 **OutSignature** 模型定义
         - **Message** (str) - 发生错误时，表示具体错误描述
-        
+
         **Response Model**
-        
-        **OutSignature** 
-        
+
+        **OutSignature**
+
         - **ErrDesc** (str) - 签名审核失败原因
         - **SigContent** (str) - 签名内容
         - **SigId** (str) - 签名ID
         - **Status** (int) - 签名状态。0-待审核 1-审核中 2-审核通过 3-审核未通过 4-被禁用
 
         """
         # build request
@@ -202,30 +202,30 @@
 
         resp = self.invoke("QueryUSMSSignature", d, **kwargs)
         return apis.QueryUSMSSignatureResponseSchema().loads(resp)
 
     def query_usms_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ QueryUSMSTemplate - 调用接口QueryUSMSTemplate查询短信模板申请状态
+        """QueryUSMSTemplate - 调用接口QueryUSMSTemplate查询短信模板申请状态
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **TemplateId** (str) - (Required) 模板ID
-        
+
         **Response**
 
         - **Data** (dict) - 见 **OutTemplate** 模型定义
         - **Message** (str) - 当RetCode不为0时，Message中显示具体错误描述
-        
+
         **Response Model**
-        
-        **OutTemplate** 
-        
+
+        **OutTemplate**
+
         - **CreateTime** (int) - 创建时间
         - **ErrDesc** (str) - 审核失败原因
         - **Purpose** (int) - 模板类型，选项：1-验证码类 2-通知类 3-会员推广类
         - **Remark** (str) - 模板说明
         - **Status** (int) - 短信模板状态；状态说明：0-待审核，1-审核中，2-审核通过，3-审核未通过，4-被禁用
         - **Template** (str) - 短信模板内容
         - **TemplateId** (str) - 短信模板ID
@@ -240,33 +240,33 @@
 
         resp = self.invoke("QueryUSMSTemplate", d, **kwargs)
         return apis.QueryUSMSTemplateResponseSchema().loads(resp)
 
     def send_usms_message(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ SendUSMSMessage - 发送短信息。短信字数超过70个后，按照每66个进行切割(因为要加上1/3), 2/3)等字样，占用4个字长)。短信最大长度不能超过600个字。每个汉字、数字、字母、字符都按一个字计
+        """SendUSMSMessage - 发送短信息。短信字数超过70个后，按照每66个进行切割(因为要加上1/3), 2/3)等字样，占用4个字长)。短信最大长度不能超过600个字。每个汉字、数字、字母、字符都按一个字计
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **PhoneNumbers** (list) - (Required) 电话号码数组，电话号码格式为(60)1xxxxxxxx，()中为国际长途区号(如中国为86或0086，两种格式都支持)，后面为电话号码.若不传入国际区号，如1851623xxxx，则默认为国内手机号
         - **TemplateId** (str) - (Required) 模板ID。若指定的模板ID审核未通过(status不等于2)则不允许发送
         - **TemplateParams** (list) - (Required) 模板参数数组，以TempalteParams.0，TempalteParams.1.。。格式。若模板ID指定的模板无可变参数，则不传入该参数。模板参数个数与模板不匹配，则不允许发送
         - **SigContent** (str) - 使用的签名，如果不输入则使用默认签名，若没有申请默认签名不允许发送；若输入的签名没有申请，则无法发送
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Action** (str) - 操作名称
         - **Message** (str) - 发生错误时表示错误描述
         - **RetCode** (int) - 返回码
         - **SessionNo** (str) - 本次提交发送的短信的唯一ID，可根据该值查询本次发送的短信列表
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.SendUSMSMessageRequestSchema().dumps(d)
 
         # build options
@@ -274,60 +274,60 @@
 
         resp = self.invoke("SendUSMSMessage", d, **kwargs)
         return apis.SendUSMSMessageResponseSchema().loads(resp)
 
     def update_usms_signature(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateUSMSSignature - 调用接口UpdateUSMSSignature修改未通过审核的短信签名，并重新提交审核
+        """UpdateUSMSSignature - 调用接口UpdateUSMSSignature修改未通过审核的短信签名，并重新提交审核
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID，不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **File** (str) - (Required) 短信签名的资质证明文件，需先进行base64编码格式转换，此处填写转换后的字符串。文件大小不超过4 MB
         - **SigContent** (str) - (Required) 新的短信签名名称；长度为2-12个字符, 可包含中文、数字和符号；无需填写【】或[]，系统会自动添加
         - **SigId** (str) - (Required) 签名ID（也即短信签名申请时的工单ID），支持以数组的方式，举例，以SigIds.0、SigIds.1...SigIds.N方式传入
         - **SigPurpose** (int) - (Required) 签名用途，0-自用，1-他用；
         - **SigType** (int) - (Required) 签名类型，说明如下：0-公司或企业的全称或简称；1-App应用的全称或简称；2-工信部备案网站的全称或简称；3-公众号或小程序的全称或简称；4-商标名的全称或简称；5-政府/机关事业单位/其他单位的全称或简称；
         - **CertificateType** (int) - 签名的资质证明文件类型，需与签名类型保持一致，说明如下：0-三证合一/企业营业执照/组织机构代码证书/社会信用代码证书；1-应用商店后台开发者管理截图；2-备案服务商的备案成功截图(含域名，网站名称，备案号)；3-公众号或小程序的管理界面截图；4-商标注册证书；5-组织机构代码证书、社会信用代码证书；
         - **ProxyFile** (str) - 短信签名授权委托文件，需先进行base64编码格式转换，此处填写转换后的字符串。文件大小不超过4 MB；当您是代理并使用第三方的签名时（也即SigPurpose为1-他用），该项为必填项；
-        
+
         **Response**
 
         - **Message** (str) - 返回状态码描述，如果操作成功，默认返回为空
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id}
         req and d.update(req)
         d = apis.UpdateUSMSSignatureRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateUSMSSignature", d, **kwargs)
         return apis.UpdateUSMSSignatureResponseSchema().loads(resp)
 
     def update_usms_template(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateUSMSTemplate - 调用接口UpdateUSMSTemplate修改未通过审核的短信模板，并重新提交审核
+        """UpdateUSMSTemplate - 调用接口UpdateUSMSTemplate修改未通过审核的短信模板，并重新提交审核
 
         **Request**
 
-        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_ 
-        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
+        - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
+        - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Template** (str) - (Required) 新的模板内容。模板名称和模板内容必须提供一个，否则会报错。小于等于600个字
         - **TemplateId** (str) - (Required) 短信模板ID
         - **Remark** (str) - 短信模板申请原因说明，字数不超过128，每个中文、符号、英文、数字等都计为1个字。
         - **TemplateName** (str) - 新的模板名称。小于等于32个字，每个中文、英文、数组、符合都计为一个字
         - **UnsubscribeInfo** (str) - 当Purpose为3时，也即会员推广类短信模板，该项必填。枚举值：TD退订、回T退订、回N退订、回TD退订、退订回T、退订回D、退订回TD、退订回复T、退订回复D、退订回复N、退订回复TD、拒收回T
-        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_ 
-        
+        - **Zone** (str) - 可用区。参见  `可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
+
         **Response**
 
         - **Message** (str) - 发生错误时表示错误描述
-        
+
         """
         # build request
         d = {"ProjectId": self.config.project_id, "Region": self.config.region}
         req and d.update(req)
         d = apis.UpdateUSMSTemplateRequestSchema().dumps(d)
 
         resp = self.invoke("UpdateUSMSTemplate", d, **kwargs)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/usms/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/usms/schemas/apis.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,30 @@
 API: CreateUSMSSignature
 
 调用接口CreateUSMSSignature申请短信签名
 """
 
 
 class CreateUSMSSignatureRequestSchema(schema.RequestSchema):
-    """ CreateUSMSSignature - 调用接口CreateUSMSSignature申请短信签名
-    """
+    """CreateUSMSSignature - 调用接口CreateUSMSSignature申请短信签名"""
 
     fields = {
         "CertificateType": fields.Int(required=True, dump_to="CertificateType"),
         "Description": fields.Str(required=True, dump_to="Description"),
         "File": fields.Str(required=True, dump_to="File"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "ProxyFile": fields.Str(required=False, dump_to="ProxyFile"),
         "SigContent": fields.Str(required=True, dump_to="SigContent"),
         "SigPurpose": fields.Int(required=True, dump_to="SigPurpose"),
         "SigType": fields.Int(required=True, dump_to="SigType"),
     }
 
 
 class CreateUSMSSignatureResponseSchema(schema.ResponseSchema):
-    """ CreateUSMSSignature - 调用接口CreateUSMSSignature申请短信签名
-    """
+    """CreateUSMSSignature - 调用接口CreateUSMSSignature申请短信签名"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "SigContent": fields.Str(required=False, load_from="SigContent"),
         "SigId": fields.Str(required=False, load_from="SigId"),
     }
 
@@ -46,16 +44,15 @@
 API: CreateUSMSTemplate
 
 调用接口CreateUSMSTemplate申请短信模板
 """
 
 
 class CreateUSMSTemplateRequestSchema(schema.RequestSchema):
-    """ CreateUSMSTemplate - 调用接口CreateUSMSTemplate申请短信模板
-    """
+    """CreateUSMSTemplate - 调用接口CreateUSMSTemplate申请短信模板"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Purpose": fields.Int(required=True, dump_to="Purpose"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Template": fields.Str(required=True, dump_to="Template"),
@@ -64,16 +61,15 @@
             required=False, dump_to="UnsubscribeInfo"
         ),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class CreateUSMSTemplateResponseSchema(schema.ResponseSchema):
-    """ CreateUSMSTemplate - 调用接口CreateUSMSTemplate申请短信模板
-    """
+    """CreateUSMSTemplate - 调用接口CreateUSMSTemplate申请短信模板"""
 
     fields = {
         "Message": fields.Str(required=True, load_from="Message"),
         "TemplateId": fields.Str(required=True, load_from="TemplateId"),
     }
 
 
@@ -81,78 +77,72 @@
 API: DeleteUSMSSignature
 
 调用接口DeleteUSMSSignature删除短信签名
 """
 
 
 class DeleteUSMSSignatureRequestSchema(schema.RequestSchema):
-    """ DeleteUSMSSignature - 调用接口DeleteUSMSSignature删除短信签名
-    """
+    """DeleteUSMSSignature - 调用接口DeleteUSMSSignature删除短信签名"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "SigIds": fields.List(fields.Str()),
     }
 
 
 class DeleteUSMSSignatureResponseSchema(schema.ResponseSchema):
-    """ DeleteUSMSSignature - 调用接口DeleteUSMSSignature删除短信签名
-    """
+    """DeleteUSMSSignature - 调用接口DeleteUSMSSignature删除短信签名"""
 
     fields = {"Message": fields.Str(required=True, load_from="Message")}
 
 
 """
 API: DeleteUSMSTemplate
 
 调用接口DeleteUSMSTemplate删除短信模板
 """
 
 
 class DeleteUSMSTemplateRequestSchema(schema.RequestSchema):
-    """ DeleteUSMSTemplate - 调用接口DeleteUSMSTemplate删除短信模板
-    """
+    """DeleteUSMSTemplate - 调用接口DeleteUSMSTemplate删除短信模板"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "TemplateIds": fields.List(fields.Str()),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class DeleteUSMSTemplateResponseSchema(schema.ResponseSchema):
-    """ DeleteUSMSTemplate - 调用接口DeleteUSMSTemplate删除短信模板
-    """
+    """DeleteUSMSTemplate - 调用接口DeleteUSMSTemplate删除短信模板"""
 
     fields = {"Message": fields.Str(required=True, load_from="Message")}
 
 
 """
 API: GetUSMSSendReceipt
 
 获取短信发送回执信息。下游服务提供商回执信息返回会有一定延时，建议发送完短信以后，5-10分钟后再调用该接口拉取回执信息。若超过12小时未返回，则请联系技术支持确认原因
 """
 
 
 class GetUSMSSendReceiptRequestSchema(schema.RequestSchema):
-    """ GetUSMSSendReceipt - 获取短信发送回执信息。下游服务提供商回执信息返回会有一定延时，建议发送完短信以后，5-10分钟后再调用该接口拉取回执信息。若超过12小时未返回，则请联系技术支持确认原因
-    """
+    """GetUSMSSendReceipt - 获取短信发送回执信息。下游服务提供商回执信息返回会有一定延时，建议发送完短信以后，5-10分钟后再调用该接口拉取回执信息。若超过12小时未返回，则请联系技术支持确认原因"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "SessionNoSet": fields.List(fields.Str()),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class GetUSMSSendReceiptResponseSchema(schema.ResponseSchema):
-    """ GetUSMSSendReceipt - 获取短信发送回执信息。下游服务提供商回执信息返回会有一定延时，建议发送完短信以后，5-10分钟后再调用该接口拉取回执信息。若超过12小时未返回，则请联系技术支持确认原因
-    """
+    """GetUSMSSendReceipt - 获取短信发送回执信息。下游服务提供商回执信息返回会有一定延时，建议发送完短信以后，5-10分钟后再调用该接口拉取回执信息。若超过12小时未返回，则请联系技术支持确认原因"""
 
     fields = {
         "Data": fields.List(
             models.ReceiptPerSessionSchema(), required=True, load_from="Data"
         ),
         "Message": fields.Str(required=True, load_from="Message"),
     }
@@ -162,27 +152,25 @@
 API: QueryUSMSSignature
 
 调用接口QueryUSMSSignature查询短信签名申请状态
 """
 
 
 class QueryUSMSSignatureRequestSchema(schema.RequestSchema):
-    """ QueryUSMSSignature - 调用接口QueryUSMSSignature查询短信签名申请状态
-    """
+    """QueryUSMSSignature - 调用接口QueryUSMSSignature查询短信签名申请状态"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "SigContent": fields.Str(required=False, dump_to="SigContent"),
         "SigId": fields.Str(required=False, dump_to="SigId"),
     }
 
 
 class QueryUSMSSignatureResponseSchema(schema.ResponseSchema):
-    """ QueryUSMSSignature - 调用接口QueryUSMSSignature查询短信签名申请状态
-    """
+    """QueryUSMSSignature - 调用接口QueryUSMSSignature查询短信签名申请状态"""
 
     fields = {
         "Data": models.OutSignatureSchema(),
         "Message": fields.Str(required=True, load_from="Message"),
     }
 
 
@@ -190,26 +178,24 @@
 API: QueryUSMSTemplate
 
 调用接口QueryUSMSTemplate查询短信模板申请状态
 """
 
 
 class QueryUSMSTemplateRequestSchema(schema.RequestSchema):
-    """ QueryUSMSTemplate - 调用接口QueryUSMSTemplate查询短信模板申请状态
-    """
+    """QueryUSMSTemplate - 调用接口QueryUSMSTemplate查询短信模板申请状态"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "TemplateId": fields.Str(required=True, dump_to="TemplateId"),
     }
 
 
 class QueryUSMSTemplateResponseSchema(schema.ResponseSchema):
-    """ QueryUSMSTemplate - 调用接口QueryUSMSTemplate查询短信模板申请状态
-    """
+    """QueryUSMSTemplate - 调用接口QueryUSMSTemplate查询短信模板申请状态"""
 
     fields = {
         "Data": models.OutTemplateSchema(),
         "Message": fields.Str(required=False, load_from="Message"),
     }
 
 
@@ -217,31 +203,29 @@
 API: SendUSMSMessage
 
 发送短信息。短信字数超过70个后，按照每66个进行切割(因为要加上1/3), 2/3)等字样，占用4个字长)。短信最大长度不能超过600个字。每个汉字、数字、字母、字符都按一个字计
 """
 
 
 class SendUSMSMessageRequestSchema(schema.RequestSchema):
-    """ SendUSMSMessage - 发送短信息。短信字数超过70个后，按照每66个进行切割(因为要加上1/3), 2/3)等字样，占用4个字长)。短信最大长度不能超过600个字。每个汉字、数字、字母、字符都按一个字计
-    """
+    """SendUSMSMessage - 发送短信息。短信字数超过70个后，按照每66个进行切割(因为要加上1/3), 2/3)等字样，占用4个字长)。短信最大长度不能超过600个字。每个汉字、数字、字母、字符都按一个字计"""
 
     fields = {
         "PhoneNumbers": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "SigContent": fields.Str(required=False, dump_to="SigContent"),
         "TemplateId": fields.Str(required=True, dump_to="TemplateId"),
         "TemplateParams": fields.List(fields.Str()),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class SendUSMSMessageResponseSchema(schema.ResponseSchema):
-    """ SendUSMSMessage - 发送短信息。短信字数超过70个后，按照每66个进行切割(因为要加上1/3), 2/3)等字样，占用4个字长)。短信最大长度不能超过600个字。每个汉字、数字、字母、字符都按一个字计
-    """
+    """SendUSMSMessage - 发送短信息。短信字数超过70个后，按照每66个进行切割(因为要加上1/3), 2/3)等字样，占用4个字长)。短信最大长度不能超过600个字。每个汉字、数字、字母、字符都按一个字计"""
 
     fields = {
         "Action": fields.Str(required=True, load_from="Action"),
         "Message": fields.Str(required=True, load_from="Message"),
         "RetCode": fields.Int(required=True, load_from="RetCode"),
         "SessionNo": fields.Str(required=False, load_from="SessionNo"),
     }
@@ -251,16 +235,15 @@
 API: UpdateUSMSSignature
 
 调用接口UpdateUSMSSignature修改未通过审核的短信签名，并重新提交审核
 """
 
 
 class UpdateUSMSSignatureRequestSchema(schema.RequestSchema):
-    """ UpdateUSMSSignature - 调用接口UpdateUSMSSignature修改未通过审核的短信签名，并重新提交审核
-    """
+    """UpdateUSMSSignature - 调用接口UpdateUSMSSignature修改未通过审核的短信签名，并重新提交审核"""
 
     fields = {
         "CertificateType": fields.Int(
             required=False, dump_to="CertificateType"
         ),
         "File": fields.Str(required=True, dump_to="File"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
@@ -269,30 +252,28 @@
         "SigId": fields.Str(required=True, dump_to="SigId"),
         "SigPurpose": fields.Int(required=True, dump_to="SigPurpose"),
         "SigType": fields.Int(required=True, dump_to="SigType"),
     }
 
 
 class UpdateUSMSSignatureResponseSchema(schema.ResponseSchema):
-    """ UpdateUSMSSignature - 调用接口UpdateUSMSSignature修改未通过审核的短信签名，并重新提交审核
-    """
+    """UpdateUSMSSignature - 调用接口UpdateUSMSSignature修改未通过审核的短信签名，并重新提交审核"""
 
     fields = {"Message": fields.Str(required=True, load_from="Message")}
 
 
 """
 API: UpdateUSMSTemplate
 
 调用接口UpdateUSMSTemplate修改未通过审核的短信模板，并重新提交审核
 """
 
 
 class UpdateUSMSTemplateRequestSchema(schema.RequestSchema):
-    """ UpdateUSMSTemplate - 调用接口UpdateUSMSTemplate修改未通过审核的短信模板，并重新提交审核
-    """
+    """UpdateUSMSTemplate - 调用接口UpdateUSMSTemplate修改未通过审核的短信模板，并重新提交审核"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Template": fields.Str(required=True, dump_to="Template"),
         "TemplateId": fields.Str(required=True, dump_to="TemplateId"),
@@ -301,11 +282,10 @@
             required=False, dump_to="UnsubscribeInfo"
         ),
         "Zone": fields.Str(required=False, dump_to="Zone"),
     }
 
 
 class UpdateUSMSTemplateResponseSchema(schema.ResponseSchema):
-    """ UpdateUSMSTemplate - 调用接口UpdateUSMSTemplate修改未通过审核的短信模板，并重新提交审核
-    """
+    """UpdateUSMSTemplate - 调用接口UpdateUSMSTemplate修改未通过审核的短信模板，并重新提交审核"""
 
     fields = {"Message": fields.Str(required=True, load_from="Message")}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/usms/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/usms/schemas/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class ReceiptPerPhoneSchema(schema.ResponseSchema):
-    """ ReceiptPerPhone - 每个目的手机号的发送回执信息
-    """
+    """ReceiptPerPhone - 每个目的手机号的发送回执信息"""
 
     fields = {
         "CostCount": fields.Int(required=True, load_from="CostCount"),
         "Phone": fields.Str(required=True, load_from="Phone"),
         "ReceiptDesc": fields.Str(required=True, load_from="ReceiptDesc"),
         "ReceiptResult": fields.Str(required=True, load_from="ReceiptResult"),
         "ReceiptTime": fields.Int(required=True, load_from="ReceiptTime"),
     }
 
 
 class ReceiptPerSessionSchema(schema.ResponseSchema):
-    """ ReceiptPerSession - 每个提交的回执结果集合
-    """
+    """ReceiptPerSession - 每个提交的回执结果集合"""
 
     fields = {
         "ReceiptSet": fields.List(ReceiptPerPhoneSchema()),
         "SessionNo": fields.Str(required=True, load_from="SessionNo"),
     }
 
 
 class OutSignatureSchema(schema.ResponseSchema):
-    """ OutSignature - 短信签名
-    """
+    """OutSignature - 短信签名"""
 
     fields = {
         "ErrDesc": fields.Str(required=True, load_from="ErrDesc"),
         "SigContent": fields.Str(required=True, load_from="SigContent"),
         "SigId": fields.Str(required=True, load_from="SigId"),
         "Status": fields.Int(required=True, load_from="Status"),
     }
 
 
 class OutTemplateSchema(schema.ResponseSchema):
-    """ OutTemplate - 短信模板
-    """
+    """OutTemplate - 短信模板"""
 
     fields = {
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "ErrDesc": fields.Str(required=True, load_from="ErrDesc"),
         "Purpose": fields.Int(required=True, load_from="Purpose"),
         "Remark": fields.Str(required=True, load_from="Remark"),
         "Status": fields.Int(required=True, load_from="Status"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/vpc/client.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/vpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self, config: dict, transport=None, middleware=None, logger=None
     ):
         super(VPCClient, self).__init__(config, transport, middleware, logger)
 
     def add_vpc_network(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ AddVPCNetwork - 添加VPC网段
+        """AddVPCNetwork - 添加VPC网段
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Network** (list) - (Required) 增加网段
         - **VPCId** (str) - (Required) 源VPC短ID
@@ -39,15 +39,15 @@
 
         resp = self.invoke("AddVPCNetwork", d, **kwargs)
         return apis.AddVPCNetworkResponseSchema().loads(resp)
 
     def associate_route_table(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ AssociateRouteTable - 绑定子网的路由表
+        """AssociateRouteTable - 绑定子网的路由表
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **RouteTableId** (str) - (Required) 路由表ID，仅限自定义路由表
         - **SubnetId** (str) - (Required) 子网ID
@@ -63,15 +63,15 @@
 
         resp = self.invoke("AssociateRouteTable", d, **kwargs)
         return apis.AssociateRouteTableResponseSchema().loads(resp)
 
     def clone_route_table(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CloneRouteTable - 根据一张现有路由表复制一张新的路由表
+        """CloneRouteTable - 根据一张现有路由表复制一张新的路由表
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **RouteTableId** (str) - (Required) 被克隆的路由表ID
 
@@ -89,15 +89,15 @@
 
         resp = self.invoke("CloneRouteTable", d, **kwargs)
         return apis.CloneRouteTableResponseSchema().loads(resp)
 
     def create_route_table(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateRouteTable - 创建路由表
+        """CreateRouteTable - 创建路由表
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **VPCId** (str) - (Required) VPC ID
         - **Name** (str) - 路由表名称 Default RouteTable
@@ -119,15 +119,15 @@
 
         resp = self.invoke("CreateRouteTable", d, **kwargs)
         return apis.CreateRouteTableResponseSchema().loads(resp)
 
     def create_subnet(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateSubnet - 创建子网
+        """CreateSubnet - 创建子网
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Subnet** (str) - (Required) 子网网络地址，例如192.168.0.0
         - **VPCId** (str) - (Required) VPC资源ID
@@ -149,15 +149,15 @@
         # build options
         kwargs["max_retries"] = 0  # ignore retry when api is not idempotent
 
         resp = self.invoke("CreateSubnet", d, **kwargs)
         return apis.CreateSubnetResponseSchema().loads(resp)
 
     def create_vpc(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ CreateVPC - 创建VPC
+        """CreateVPC - 创建VPC
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Name** (str) - (Required) VPC名称
         - **Network** (list) - (Required) VPC网段
@@ -180,15 +180,15 @@
 
         resp = self.invoke("CreateVPC", d, **kwargs)
         return apis.CreateVPCResponseSchema().loads(resp)
 
     def create_vpc_intercom(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ CreateVPCIntercom - 新建VPC互通关系
+        """CreateVPCIntercom - 新建VPC互通关系
 
         **Request**
 
         - **ProjectId** (str) - (Config) 源VPC所在项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 源VPC所在地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DstVPCId** (str) - (Required) 目的VPC短ID
         - **VPCId** (str) - (Required) 源VPC短ID
@@ -209,15 +209,15 @@
 
         resp = self.invoke("CreateVPCIntercom", d, **kwargs)
         return apis.CreateVPCIntercomResponseSchema().loads(resp)
 
     def delete_route_table(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteRouteTable - 删除自定义路由表
+        """DeleteRouteTable - 删除自定义路由表
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **RouteTableId** (str) - (Required) 路由ID
 
@@ -232,15 +232,15 @@
 
         resp = self.invoke("DeleteRouteTable", d, **kwargs)
         return apis.DeleteRouteTableResponseSchema().loads(resp)
 
     def delete_subnet(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteSubnet - 删除子网
+        """DeleteSubnet - 删除子网
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SubnetId** (str) - (Required) 子网ID
 
@@ -253,15 +253,15 @@
         req and d.update(req)
         d = apis.DeleteSubnetRequestSchema().dumps(d)
 
         resp = self.invoke("DeleteSubnet", d, **kwargs)
         return apis.DeleteSubnetResponseSchema().loads(resp)
 
     def delete_vpc(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DeleteVPC - 删除VPC
+        """DeleteVPC - 删除VPC
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **VPCId** (str) - (Required) VPC资源Id
 
@@ -276,15 +276,15 @@
 
         resp = self.invoke("DeleteVPC", d, **kwargs)
         return apis.DeleteVPCResponseSchema().loads(resp)
 
     def delete_vpc_intercom(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DeleteVPCIntercom - 删除VPC互通关系
+        """DeleteVPCIntercom - 删除VPC互通关系
 
         **Request**
 
         - **ProjectId** (str) - (Config) 源VPC所在项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 源VPC所在地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **DstVPCId** (str) - (Required) 目的VPC短ID
         - **VPCId** (str) - (Required) 源VPC短ID
@@ -302,15 +302,15 @@
 
         resp = self.invoke("DeleteVPCIntercom", d, **kwargs)
         return apis.DeleteVPCIntercomResponseSchema().loads(resp)
 
     def describe_route_table(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeRouteTable - 获取路由表详细信息(包括路由策略)
+        """DescribeRouteTable - 获取路由表详细信息(包括路由策略)
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BusinessId** (str) - 业务组ID
         - **Limit** (int) - Limit
@@ -354,15 +354,15 @@
 
         resp = self.invoke("DescribeRouteTable", d, **kwargs)
         return apis.DescribeRouteTableResponseSchema().loads(resp)
 
     def describe_subnet(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeSubnet - 获取子网信息
+        """DescribeSubnet - 获取子网信息
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **BusinessId** (str) - 业务组
         - **Limit** (int) - 列表长度，默认为20
@@ -411,15 +411,15 @@
 
         resp = self.invoke("DescribeSubnet", d, **kwargs)
         return apis.DescribeSubnetResponseSchema().loads(resp)
 
     def describe_subnet_resource(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeSubnetResource - 展示子网资源
+        """DescribeSubnetResource - 展示子网资源
         **Request**
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SubnetId** (str) - (Required) 子网id
         - **Limit** (int) - 单页返回数据长度，默认为20
         - **Offset** (int) - 列表起始位置偏移量，默认为0
         - **ResourceType** (str) - 资源类型，默认为全部资源类型。枚举值为：UHOST，云主机；PHOST，物理云主机；ULB，负载均衡；UHADOOP_HOST，hadoop节点；UFORTRESS_HOST，堡垒机；UNATGW，NAT网关；UKAFKA，Kafka消息队列；UMEM，内存存储；DOCKER，容器集群；UDB，数据库；UDW，数据仓库；VIP，内网VIP.
@@ -446,15 +446,15 @@
         req and d.update(req)
         d = apis.DescribeSubnetResourceRequestSchema().dumps(d)
 
         resp = self.invoke("DescribeSubnetResource", d, **kwargs)
         return apis.DescribeSubnetResourceResponseSchema().loads(resp)
 
     def describe_vpc(self, req: typing.Optional[dict] = None, **kwargs) -> dict:
-        """ DescribeVPC - 获取VPC信息
+        """DescribeVPC - 获取VPC信息
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Limit** (int) -
         - **Offset** (int) -
@@ -493,15 +493,15 @@
 
         resp = self.invoke("DescribeVPC", d, **kwargs)
         return apis.DescribeVPCResponseSchema().loads(resp)
 
     def describe_vpc_intercom(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ DescribeVPCIntercom - 获取VPC互通信息
+        """DescribeVPCIntercom - 获取VPC互通信息
 
         **Request**
 
         - **ProjectId** (str) - (Config) 源VPC所在项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 源VPC所在地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **VPCId** (str) - (Required) VPC短ID
         - **DstProjectId** (str) - 目的项目ID，默认为全部项目
@@ -530,15 +530,15 @@
 
         resp = self.invoke("DescribeVPCIntercom", d, **kwargs)
         return apis.DescribeVPCIntercomResponseSchema().loads(resp)
 
     def modify_route_rule(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ ModifyRouteRule - 路由策略增、删、改
+        """ModifyRouteRule - 路由策略增、删、改
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **RouteRule** (list) - (Required) 格式: RouteRuleId | 目的网段 | 下一跳类型 | 下一跳 |优先级| 备注 | 增、删、改标志  (下一跳类型为instance或者vip，下一跳为云主机id或者vip的id，优先级使用0，动作标志为add/delete/update)   。"添加"示例: test_id | 10.8.0.0/16 | instance | uhost-xd8ja | 0 | Default Route Rule| add (添加的RouteRuleId填任意非空字符串)     。"删除"示例: routerule-xk3jxa | 10.8.0.0/16 | instance | uhost-xd8ja | 0 | Default Route Rule| delete (RouteRuleId来自DescribeRouteTable中)     。“修改”示例: routerule-xk3jxa | 10.8.0.0/16 | instance | uhost-cjksa2 | 0 | Default Route Rule| update (RouteRuleId来自DescribeRouteTable中)
         - **RouteTableId** (str) - (Required) 通过DescribeRouteTable拿到
@@ -554,15 +554,15 @@
 
         resp = self.invoke("ModifyRouteRule", d, **kwargs)
         return apis.ModifyRouteRuleResponseSchema().loads(resp)
 
     def update_route_table_attribute(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateRouteTableAttribute - 更新路由表基本信息
+        """UpdateRouteTableAttribute - 更新路由表基本信息
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **RouteTableId** (str) - (Required) 路由表ID
         - **Name** (str) - 名称
@@ -580,15 +580,15 @@
 
         resp = self.invoke("UpdateRouteTableAttribute", d, **kwargs)
         return apis.UpdateRouteTableAttributeResponseSchema().loads(resp)
 
     def update_subnet_attribute(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateSubnetAttribute - 更新子网信息
+        """UpdateSubnetAttribute - 更新子网信息
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **SubnetId** (str) - (Required) 子网ID
         - **Name** (str) - 子网名称(如果Name不填写，Tag必须填写)
@@ -605,15 +605,15 @@
 
         resp = self.invoke("UpdateSubnetAttribute", d, **kwargs)
         return apis.UpdateSubnetAttributeResponseSchema().loads(resp)
 
     def update_vpc_network(
         self, req: typing.Optional[dict] = None, **kwargs
     ) -> dict:
-        """ UpdateVPCNetwork - 更新VPC网段
+        """UpdateVPCNetwork - 更新VPC网段
 
         **Request**
 
         - **ProjectId** (str) - (Config) 项目ID。不填写为默认项目，子帐号必须填写。 请参考 `GetProjectList接口 <https://docs.ucloud.cn/api/summary/get_project_list.html>`_
         - **Region** (str) - (Config) 地域。 参见  `地域和可用区列表 <https://docs.ucloud.cn/api/summary/regionlist.html>`_
         - **Network** (list) - (Required) 需要保留的VPC网段。当前仅支持删除VPC网段，添加网段请参考 `AddVPCNetwork <https://docs.ucloud.cn/api/vpc2.0-api/add_vpc_network>`_
         - **VPCId** (str) - (Required) VPC的ID
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/vpc/schemas/apis.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/vpc/schemas/apis.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,328 +12,304 @@
 API: AddVPCNetwork
 
 添加VPC网段
 """
 
 
 class AddVPCNetworkRequestSchema(schema.RequestSchema):
-    """ AddVPCNetwork - 添加VPC网段
-    """
+    """AddVPCNetwork - 添加VPC网段"""
 
     fields = {
         "Network": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class AddVPCNetworkResponseSchema(schema.ResponseSchema):
-    """ AddVPCNetwork - 添加VPC网段
-    """
+    """AddVPCNetwork - 添加VPC网段"""
 
     fields = {}
 
 
 """
 API: AssociateRouteTable
 
 绑定子网的路由表
 """
 
 
 class AssociateRouteTableRequestSchema(schema.RequestSchema):
-    """ AssociateRouteTable - 绑定子网的路由表
-    """
+    """AssociateRouteTable - 绑定子网的路由表"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RouteTableId": fields.Str(required=True, dump_to="RouteTableId"),
         "SubnetId": fields.Str(required=True, dump_to="SubnetId"),
     }
 
 
 class AssociateRouteTableResponseSchema(schema.ResponseSchema):
-    """ AssociateRouteTable - 绑定子网的路由表
-    """
+    """AssociateRouteTable - 绑定子网的路由表"""
 
     fields = {}
 
 
 """
 API: CloneRouteTable
 
 根据一张现有路由表复制一张新的路由表
 """
 
 
 class CloneRouteTableRequestSchema(schema.RequestSchema):
-    """ CloneRouteTable - 根据一张现有路由表复制一张新的路由表
-    """
+    """CloneRouteTable - 根据一张现有路由表复制一张新的路由表"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=False, dump_to="Region"),
         "RouteTableId": fields.Str(required=True, dump_to="RouteTableId"),
     }
 
 
 class CloneRouteTableResponseSchema(schema.ResponseSchema):
-    """ CloneRouteTable - 根据一张现有路由表复制一张新的路由表
-    """
+    """CloneRouteTable - 根据一张现有路由表复制一张新的路由表"""
 
     fields = {}
 
 
 """
 API: CreateRouteTable
 
 创建路由表
 """
 
 
 class CreateRouteTableRequestSchema(schema.RequestSchema):
-    """ CreateRouteTable - 创建路由表
-    """
+    """CreateRouteTable - 创建路由表"""
 
     fields = {
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class CreateRouteTableResponseSchema(schema.ResponseSchema):
-    """ CreateRouteTable - 创建路由表
-    """
+    """CreateRouteTable - 创建路由表"""
 
     fields = {
         "RouteTableId": fields.Str(required=False, load_from="RouteTableId")
     }
 
 
 """
 API: CreateSubnet
 
 创建子网
 """
 
 
 class CreateSubnetRequestSchema(schema.RequestSchema):
-    """ CreateSubnet - 创建子网
-    """
+    """CreateSubnet - 创建子网"""
 
     fields = {
         "Netmask": fields.Int(required=False, dump_to="Netmask"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Subnet": fields.Str(required=True, dump_to="Subnet"),
         "SubnetName": fields.Str(required=False, dump_to="SubnetName"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class CreateSubnetResponseSchema(schema.ResponseSchema):
-    """ CreateSubnet - 创建子网
-    """
+    """CreateSubnet - 创建子网"""
 
     fields = {"SubnetId": fields.Str(required=False, load_from="SubnetId")}
 
 
 """
 API: CreateVPC
 
 创建VPC
 """
 
 
 class CreateVPCRequestSchema(schema.RequestSchema):
-    """ CreateVPC - 创建VPC
-    """
+    """CreateVPC - 创建VPC"""
 
     fields = {
         "Name": fields.Str(required=True, dump_to="Name"),
         "Network": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "Type": fields.Int(required=False, dump_to="Type"),
     }
 
 
 class CreateVPCResponseSchema(schema.ResponseSchema):
-    """ CreateVPC - 创建VPC
-    """
+    """CreateVPC - 创建VPC"""
 
     fields = {"VPCId": fields.Str(required=False, load_from="VPCId")}
 
 
 """
 API: CreateVPCIntercom
 
 新建VPC互通关系
 """
 
 
 class CreateVPCIntercomRequestSchema(schema.RequestSchema):
-    """ CreateVPCIntercom - 新建VPC互通关系
-    """
+    """CreateVPCIntercom - 新建VPC互通关系"""
 
     fields = {
         "DstProjectId": fields.Str(required=False, dump_to="DstProjectId"),
         "DstRegion": fields.Str(required=False, dump_to="DstRegion"),
         "DstVPCId": fields.Str(required=True, dump_to="DstVPCId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class CreateVPCIntercomResponseSchema(schema.ResponseSchema):
-    """ CreateVPCIntercom - 新建VPC互通关系
-    """
+    """CreateVPCIntercom - 新建VPC互通关系"""
 
     fields = {}
 
 
 """
 API: DeleteRouteTable
 
 删除自定义路由表
 """
 
 
 class DeleteRouteTableRequestSchema(schema.RequestSchema):
-    """ DeleteRouteTable - 删除自定义路由表
-    """
+    """DeleteRouteTable - 删除自定义路由表"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RouteTableId": fields.Str(required=True, dump_to="RouteTableId"),
     }
 
 
 class DeleteRouteTableResponseSchema(schema.ResponseSchema):
-    """ DeleteRouteTable - 删除自定义路由表
-    """
+    """DeleteRouteTable - 删除自定义路由表"""
 
     fields = {}
 
 
 """
 API: DeleteSubnet
 
 删除子网
 """
 
 
 class DeleteSubnetRequestSchema(schema.RequestSchema):
-    """ DeleteSubnet - 删除子网
-    """
+    """DeleteSubnet - 删除子网"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetId": fields.Str(required=True, dump_to="SubnetId"),
     }
 
 
 class DeleteSubnetResponseSchema(schema.ResponseSchema):
-    """ DeleteSubnet - 删除子网
-    """
+    """DeleteSubnet - 删除子网"""
 
     fields = {}
 
 
 """
 API: DeleteVPC
 
 删除VPC
 """
 
 
 class DeleteVPCRequestSchema(schema.RequestSchema):
-    """ DeleteVPC - 删除VPC
-    """
+    """DeleteVPC - 删除VPC"""
 
     fields = {
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class DeleteVPCResponseSchema(schema.ResponseSchema):
-    """ DeleteVPC - 删除VPC
-    """
+    """DeleteVPC - 删除VPC"""
 
     fields = {}
 
 
 """
 API: DeleteVPCIntercom
 
 删除VPC互通关系
 """
 
 
 class DeleteVPCIntercomRequestSchema(schema.RequestSchema):
-    """ DeleteVPCIntercom - 删除VPC互通关系
-    """
+    """DeleteVPCIntercom - 删除VPC互通关系"""
 
     fields = {
         "DstProjectId": fields.Str(required=False, dump_to="DstProjectId"),
         "DstRegion": fields.Str(required=False, dump_to="DstRegion"),
         "DstVPCId": fields.Str(required=True, dump_to="DstVPCId"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class DeleteVPCIntercomResponseSchema(schema.ResponseSchema):
-    """ DeleteVPCIntercom - 删除VPC互通关系
-    """
+    """DeleteVPCIntercom - 删除VPC互通关系"""
 
     fields = {}
 
 
 """
 API: DescribeRouteTable
 
 获取路由表详细信息(包括路由策略)
 """
 
 
 class DescribeRouteTableRequestSchema(schema.RequestSchema):
-    """ DescribeRouteTable - 获取路由表详细信息(包括路由策略)
-    """
+    """DescribeRouteTable - 获取路由表详细信息(包括路由策略)"""
 
     fields = {
         "BusinessId": fields.Str(required=False, dump_to="BusinessId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "OffSet": fields.Int(required=False, dump_to="OffSet"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RouteTableId": fields.Str(required=False, dump_to="RouteTableId"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
     }
 
 
 class DescribeRouteTableResponseSchema(schema.ResponseSchema):
-    """ DescribeRouteTable - 获取路由表详细信息(包括路由策略)
-    """
+    """DescribeRouteTable - 获取路由表详细信息(包括路由策略)"""
 
     fields = {
         "RouteTables": fields.List(
             models.RouteTableInfoSchema(),
             required=False,
             load_from="RouteTables",
         ),
@@ -345,16 +321,15 @@
 API: DescribeSubnet
 
 获取子网信息
 """
 
 
 class DescribeSubnetRequestSchema(schema.RequestSchema):
-    """ DescribeSubnet - 获取子网信息
-    """
+    """DescribeSubnet - 获取子网信息"""
 
     fields = {
         "BusinessId": fields.Str(required=False, dump_to="BusinessId"),
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
@@ -366,16 +341,15 @@
         "SubnetIds": fields.List(fields.Str()),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VPCId": fields.Str(required=False, dump_to="VPCId"),
     }
 
 
 class DescribeSubnetResponseSchema(schema.ResponseSchema):
-    """ DescribeSubnet - 获取子网信息
-    """
+    """DescribeSubnet - 获取子网信息"""
 
     fields = {
         "DataSet": fields.List(
             models.SubnetInfoSchema(), required=True, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=True, load_from="TotalCount"),
     }
@@ -385,30 +359,28 @@
 API: DescribeSubnetResource
 
 展示子网资源
 """
 
 
 class DescribeSubnetResourceRequestSchema(schema.RequestSchema):
-    """ DescribeSubnetResource - 展示子网资源
-    """
+    """DescribeSubnetResource - 展示子网资源"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "ResourceType": fields.Str(required=False, dump_to="ResourceType"),
         "SubnetId": fields.Str(required=True, dump_to="SubnetId"),
     }
 
 
 class DescribeSubnetResourceResponseSchema(schema.ResponseSchema):
-    """ DescribeSubnetResource - 展示子网资源
-    """
+    """DescribeSubnetResource - 展示子网资源"""
 
     fields = {
         "DataSet": fields.List(
             models.SubnetResourceSchema(), required=False, load_from="DataSet"
         ),
         "TotalCount": fields.Int(required=False, load_from="TotalCount"),
     }
@@ -418,30 +390,28 @@
 API: DescribeVPC
 
 获取VPC信息
 """
 
 
 class DescribeVPCRequestSchema(schema.RequestSchema):
-    """ DescribeVPC - 获取VPC信息
-    """
+    """DescribeVPC - 获取VPC信息"""
 
     fields = {
         "Limit": fields.Int(required=False, dump_to="Limit"),
         "Offset": fields.Int(required=False, dump_to="Offset"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
         "VPCIds": fields.List(fields.Str()),
     }
 
 
 class DescribeVPCResponseSchema(schema.ResponseSchema):
-    """ DescribeVPC - 获取VPC信息
-    """
+    """DescribeVPC - 获取VPC信息"""
 
     fields = {
         "DataSet": fields.List(
             models.VPCInfoSchema(), required=False, load_from="DataSet"
         )
     }
 
@@ -450,29 +420,27 @@
 API: DescribeVPCIntercom
 
 获取VPC互通信息
 """
 
 
 class DescribeVPCIntercomRequestSchema(schema.RequestSchema):
-    """ DescribeVPCIntercom - 获取VPC互通信息
-    """
+    """DescribeVPCIntercom - 获取VPC互通信息"""
 
     fields = {
         "DstProjectId": fields.Str(required=False, dump_to="DstProjectId"),
         "DstRegion": fields.Str(required=False, dump_to="DstRegion"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class DescribeVPCIntercomResponseSchema(schema.ResponseSchema):
-    """ DescribeVPCIntercom - 获取VPC互通信息
-    """
+    """DescribeVPCIntercom - 获取VPC互通信息"""
 
     fields = {
         "DataSet": fields.List(
             models.VPCIntercomInfoSchema(), required=False, load_from="DataSet"
         )
     }
 
@@ -481,104 +449,96 @@
 API: ModifyRouteRule
 
 路由策略增、删、改
 """
 
 
 class ModifyRouteRuleRequestSchema(schema.RequestSchema):
-    """ ModifyRouteRule - 路由策略增、删、改
-    """
+    """ModifyRouteRule - 路由策略增、删、改"""
 
     fields = {
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "RouteRule": fields.List(fields.Str()),
         "RouteTableId": fields.Str(required=True, dump_to="RouteTableId"),
     }
 
 
 class ModifyRouteRuleResponseSchema(schema.ResponseSchema):
-    """ ModifyRouteRule - 路由策略增、删、改
-    """
+    """ModifyRouteRule - 路由策略增、删、改"""
 
     fields = {}
 
 
 """
 API: UpdateRouteTableAttribute
 
 更新路由表基本信息
 """
 
 
 class UpdateRouteTableAttributeRequestSchema(schema.RequestSchema):
-    """ UpdateRouteTableAttribute - 更新路由表基本信息
-    """
+    """UpdateRouteTableAttribute - 更新路由表基本信息"""
 
     fields = {
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "Remark": fields.Str(required=False, dump_to="Remark"),
         "RouteTableId": fields.Str(required=True, dump_to="RouteTableId"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class UpdateRouteTableAttributeResponseSchema(schema.ResponseSchema):
-    """ UpdateRouteTableAttribute - 更新路由表基本信息
-    """
+    """UpdateRouteTableAttribute - 更新路由表基本信息"""
 
     fields = {}
 
 
 """
 API: UpdateSubnetAttribute
 
 更新子网信息
 """
 
 
 class UpdateSubnetAttributeRequestSchema(schema.RequestSchema):
-    """ UpdateSubnetAttribute - 更新子网信息
-    """
+    """UpdateSubnetAttribute - 更新子网信息"""
 
     fields = {
         "Name": fields.Str(required=False, dump_to="Name"),
         "ProjectId": fields.Str(required=False, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "SubnetId": fields.Str(required=True, dump_to="SubnetId"),
         "Tag": fields.Str(required=False, dump_to="Tag"),
     }
 
 
 class UpdateSubnetAttributeResponseSchema(schema.ResponseSchema):
-    """ UpdateSubnetAttribute - 更新子网信息
-    """
+    """UpdateSubnetAttribute - 更新子网信息"""
 
     fields = {}
 
 
 """
 API: UpdateVPCNetwork
 
 更新VPC网段
 """
 
 
 class UpdateVPCNetworkRequestSchema(schema.RequestSchema):
-    """ UpdateVPCNetwork - 更新VPC网段
-    """
+    """UpdateVPCNetwork - 更新VPC网段"""
 
     fields = {
         "Network": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=True, dump_to="ProjectId"),
         "Region": fields.Str(required=True, dump_to="Region"),
         "VPCId": fields.Str(required=True, dump_to="VPCId"),
     }
 
 
 class UpdateVPCNetworkResponseSchema(schema.ResponseSchema):
-    """ UpdateVPCNetwork - 更新VPC网段
-    """
+    """UpdateVPCNetwork - 更新VPC网段"""
 
     fields = {"Message": fields.Str(required=True, load_from="Message")}
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/services/vpc/schemas/models.py` & `ucloud-sdk-python3-0.9.4/ucloud/services/vpc/schemas/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """ Code is generated by ucloud-model, DO NOT EDIT IT. """
 
 from ucloud.core.typesystem import schema, fields
 
 
 class RouteRuleInfoSchema(schema.ResponseSchema):
-    """ RouteRuleInfo - 路由规则信息
-    """
+    """RouteRuleInfo - 路由规则信息"""
 
     fields = {
         "DstAddr": fields.Str(required=False, load_from="DstAddr"),
         "NexthopId": fields.Str(required=False, load_from="NexthopId"),
         "NexthopType": fields.Str(required=False, load_from="NexthopType"),
         "Remark": fields.Str(required=False, load_from="Remark"),
         "RouteRuleId": fields.Str(required=False, load_from="RouteRuleId"),
         "RuleType": fields.Int(required=False, load_from="RuleType"),
     }
 
 
 class RouteTableInfoSchema(schema.ResponseSchema):
-    """ RouteTableInfo - 路由表信息
-    """
+    """RouteTableInfo - 路由表信息"""
 
     fields = {
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Remark": fields.Str(required=False, load_from="Remark"),
         "RouteRules": fields.List(RouteRuleInfoSchema()),
         "RouteTableId": fields.Str(required=False, load_from="RouteTableId"),
         "RouteTableType": fields.Int(
@@ -33,16 +31,15 @@
         "Tag": fields.Str(required=False, load_from="Tag"),
         "VPCId": fields.Str(required=False, load_from="VPCId"),
         "VPCName": fields.Str(required=False, load_from="VPCName"),
     }
 
 
 class SubnetInfoSchema(schema.ResponseSchema):
-    """ SubnetInfo - 子网信息
-    """
+    """SubnetInfo - 子网信息"""
 
     fields = {
         "AvailableIPs": fields.Int(required=False, load_from="AvailableIPs"),
         "CreateTime": fields.Int(required=False, load_from="CreateTime"),
         "Gateway": fields.Str(required=False, load_from="Gateway"),
         "HasNATGW": fields.Bool(required=False, load_from="HasNATGW"),
         "IPv6Network": fields.Str(required=False, load_from="IPv6Network"),
@@ -57,16 +54,15 @@
         "VPCId": fields.Str(required=False, load_from="VPCId"),
         "VPCName": fields.Str(required=False, load_from="VPCName"),
         "Zone": fields.Str(required=False, load_from="Zone"),
     }
 
 
 class SubnetResourceSchema(schema.ResponseSchema):
-    """ SubnetResource - 子网下资源
-    """
+    """SubnetResource - 子网下资源"""
 
     fields = {
         "IP": fields.Str(required=False, load_from="IP"),
         "IPv6Address": fields.Str(required=False, load_from="IPv6Address"),
         "Name": fields.Str(required=False, load_from="Name"),
         "ResourceId": fields.Str(required=False, load_from="ResourceId"),
         "ResourceType": fields.Str(required=False, load_from="ResourceType"),
@@ -77,26 +73,24 @@
         "SubResourceType": fields.Str(
             required=False, load_from="SubResourceType"
         ),
     }
 
 
 class VPCNetworkInfoSchema(schema.ResponseSchema):
-    """ VPCNetworkInfo - vpc地址空间信息
-    """
+    """VPCNetworkInfo - vpc地址空间信息"""
 
     fields = {
         "Network": fields.Str(required=False, load_from="Network"),
         "SubnetCount": fields.Int(required=False, load_from="SubnetCount"),
     }
 
 
 class VPCInfoSchema(schema.ResponseSchema):
-    """ VPCInfo - VPC信息
-    """
+    """VPCInfo - VPC信息"""
 
     fields = {
         "CreateTime": fields.Int(required=True, load_from="CreateTime"),
         "IPv6Network": fields.Str(required=False, load_from="IPv6Network"),
         "Name": fields.Str(required=True, load_from="Name"),
         "Network": fields.List(fields.Str()),
         "NetworkInfo": fields.List(VPCNetworkInfoSchema()),
@@ -105,16 +99,15 @@
         "Tag": fields.Str(required=True, load_from="Tag"),
         "UpdateTime": fields.Int(required=True, load_from="UpdateTime"),
         "VPCId": fields.Str(required=False, load_from="VPCId"),
     }
 
 
 class VPCIntercomInfoSchema(schema.ResponseSchema):
-    """ VPCIntercomInfo -
-    """
+    """VPCIntercomInfo -"""
 
     fields = {
         "DstRegion": fields.Str(required=False, load_from="DstRegion"),
         "Name": fields.Str(required=False, load_from="Name"),
         "Network": fields.List(fields.Str()),
         "ProjectId": fields.Str(required=False, load_from="ProjectId"),
         "Tag": fields.Str(required=False, load_from="Tag"),
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/driver/_scenario.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/driver/_scenario.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/driver/_specification.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/driver/_specification.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/driver/_step.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/driver/_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         startup_delay: int = 0,
         retry_for: typing.Tuple = (CompareError, ValueNotFoundError),
         fast_fail: bool = False,
         validators: typing.Callable[[dict], typing.List[typing.Tuple]] = None,
         title: str = "",
         **kwargs
     ):
-        """ Step is the test step in a test scenario
+        """Step is the test step in a test scenario
         :param invoker: invoker is a callable function
         :param max_retries: the maximum retry number by the `retry_for` exception,
                             it will resolve the flaky testing case
         :param retry_interval: the interval between twice retrying
         :param retry_for: the exceptions to retrying
         :param startup_delay: the delay seconds before any action execution
         :param fast_fail: if fast fail is true, the test will fail when got
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/env.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 
 def is_ut() -> bool:
     """ check test env is unit testing or not """
     return not is_acc()
 
 
 def pre_check_env():
-    """ pre check environment for testing
+    """pre check environment for testing
 
     NOTE: system environment variables credential is required for test environment
     """
     assert os.getenv("UCLOUD_PUBLIC_KEY"), "invalid public key"
     assert os.getenv("UCLOUD_PRIVATE_KEY"), "invalid private key"
     assert os.getenv("UCLOUD_PROJECT_ID"), "invalid region"
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/funcs.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import datetime
 import time
 
 
 def concat(*args):
-    """  cancat strings
+    """cancat strings
 
     >>> concat(42, 'foo', 'bar')
     '42foobar'
     """
     return "".join([str(s) for s in args])
 
 
 def concat_without_dot(args):
-    """  replace blank
+    """replace blank
 
     >>> concat_without_dot('42foo bar')
     '42foobar'
     """
     return "".join([str(s) for s in args.split()])
 
 
 def search_value(array, origin_key, origin_value, dest_key):
-    """ given origin key and value,search dest_value form array by dest_key
+    """given origin key and value,search dest_value form array by dest_key
 
     >>> d = [{"UHostId": "foo", "Name": "testing"}]
     >>> search_value(d, "Name", "testing", "UHostId")
     'foo'
     """
     arr = [i.get(dest_key, "") for i in array if i[origin_key] == origin_value]
     if arr:
         return arr[0]
     return ""
 
 
 def timedelta(timestamp, value, typ="days"):
-    """ given timestamp(10bit) and calculate relative delta time
+    """given timestamp(10bit) and calculate relative delta time
 
     >>> timedelta(0, 1, "days")
     86400.0
 
     :param timestamp: timestamp (round to second)
     :param value: float, can as positive or negative
     :param typ: days/hours
@@ -50,15 +50,15 @@
         dt += datetime.timedelta(days=value)
     elif typ == "hours":
         dt += datetime.timedelta(hours=value)
     return time.mktime(dt.timetuple())
 
 
 def get_timestamp(length=13):
-    """ get current timestamp string
+    """get current timestamp string
 
     >>> len(str(int(get_timestamp(10))))
     10
 
     :param length: length of timestamp, can only between 0 and 16
     :return:
     """
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/mock.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/mock.py`

 * *Files identical despite different names*

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/op.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/op.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,110 +1,94 @@
 import re
 
 from ucloud.testing.exc import CompareError
 
 
 def eq(value, expected):
-    """ value is equal to expected
-    """
+    """value is equal to expected"""
     assert value == expected
 
 
 def ne(value, expected):
-    """ value is equal to expected
-    """
+    """value is equal to expected"""
     assert value != expected
 
 
 def gt(value, expected):
-    """ value is greater than expected
-    """
+    """value is greater than expected"""
     assert float(value) > float(expected)
 
 
 def ge(value, expected):
-    """ value is greater than or equal to expected
-    """
+    """value is greater than or equal to expected"""
     assert float(value) >= float(expected)
 
 
 def abs_eq(value, expected):
-    """ value is approx equal to expected
-    """
+    """value is approx equal to expected"""
     assert round(float(value), 2) == round(float(expected), 2)
 
 
 def lt(value, expected):
-    """ value is less than excepted
-    """
+    """value is less than excepted"""
     assert float(value) < float(expected)
 
 
 def le(value, expected):
-    """ value is less than or equal to excepted
-    """
+    """value is less than or equal to excepted"""
     assert float(value) <= float(expected)
 
 
 def str_eq(value, expected):
-    """ value is equal to excepted as string
-    """
+    """value is equal to excepted as string"""
     assert str(value) == str(expected)
 
 
 def float_eq(value, expected):
-    """ value is equal to excepted as float
-    """
+    """value is equal to excepted as float"""
     assert round(float(value), 2) == round(float(expected), 2)
 
 
 def len_eq(value, expected):
-    """ length of value is equal to excepted
-    """
+    """length of value is equal to excepted"""
     assert isinstance(expected, int)
     assert len(value) == expected
 
 
 def len_gt(value, expected):
-    """ length of value is greater than excepted
-    """
+    """length of value is greater than excepted"""
     assert isinstance(expected, int)
     assert len(value) > expected
 
 
 def len_ge(value, expected):
-    """ length of value is greater than or equal to excepted
-    """
+    """length of value is greater than or equal to excepted"""
     assert isinstance(expected, int)
     assert len(value) >= expected
 
 
 def len_lt(value, expected):
-    """ length of value is less than excepted
-    """
+    """length of value is less than excepted"""
     assert isinstance(expected, int)
     assert len(value) < expected
 
 
 def len_le(value, expected):
-    """ length of value is less than or equal to excepted
-    """
+    """length of value is less than or equal to excepted"""
     assert isinstance(expected, int)
     assert len(value) <= expected
 
 
 def contains(value, expected):
-    """ value is contains expected
-    """
+    """value is contains expected"""
     assert expected in value
 
 
 def contained_by(value, expected):
-    """ value is contained by expected
-    """
+    """value is contained by expected"""
     assert value in expected
 
 
 def type_eq(value, expected):
     assert isinstance(value, expected)
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud/testing/utest.py` & `ucloud-sdk-python3-0.9.4/ucloud/testing/utest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         retry_interval: int = 0,
         startup_delay: int = 0,
         retry_for: typing.Tuple = (CompareError, ValueNotFoundError),
         fast_fail: bool = False,
         validators: typing.Callable[[dict], typing.List[typing.Tuple]] = None,
         **kwargs
     ):
-        """ Step is the test step in a test scenario
+        """Step is the test step in a test scenario
         :param invoker: invoker is a callable function
         :param max_retries: the maximum retry number by the `retry_for` exception,
                             it will resolve the flaky testing case
         :param retry_interval: the interval between twice retrying
         :param retry_for: the exceptions to retrying
         :param startup_delay: the delay seconds before any action execution
         :param fast_fail: if fast fail is true, the test will fail when got
@@ -157,15 +157,15 @@
         self.summary()
 
     def initial(self, variables: typing.Optional[dict] = None):
         self.variables = variables
 
 
 def value_at_path(d: dict, path: str):
-    """ access value by object path
+    """access value by object path
 
     :param d: dict or list of dict
     :param path: object path like `Data.1.UHostId`
     :return: any value access by path
     """
     if d is None:
         return
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/PKG-INFO` & `ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucloud-sdk-python3
-Version: 0.9.3
+Version: 0.9.4
 Summary: UCloud Service Development Kit - Python
 Home-page: https://github.com/ucloud/ucloud-sdk-python3
 Author: ucloud
 Author-email: esl_ipdd@ucloud.cn
 License: Apache License 2.0
 Description: <p align="center">
             <img src="https://ucloud-sdk.dl.ufileos.com/logos%2Flogo-mini.png" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ucloud-sdk-python3 Version: 0.9.3 Summary: UCloud
+Metadata-Version: 2.1 Name: ucloud-sdk-python3 Version: 0.9.4 Summary: UCloud
 Service Development Kit - Python Home-page: https://github.com/ucloud/ucloud-
 sdk-python3 Author: ucloud Author-email: esl_ipdd@ucloud.cn License: Apache
 License 2.0 Description:
            [https://ucloud-sdk.dl.ufileos.com/logos%2Flogo-mini.png]
                        ****** UCloud SDK Python 3 ******
    [Latest_Stable_Version] [Travis_CI_Status] [Codecov_Status] [Doc_Status]
 UCloud SDK is a Python client library for accessing the UCloud API. This client
```

### Comparing `ucloud-sdk-python3-0.9.3/ucloud_sdk_python3.egg-info/SOURCES.txt` & `ucloud-sdk-python3-0.9.4/ucloud_sdk_python3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

