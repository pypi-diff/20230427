# Comparing `tmp/infisical-1.0.1.tar.gz` & `tmp/infisical-1.1.0.tar.gz`

## Comparing `infisical-1.0.1.tar` & `infisical-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,42 @@
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 infisical-1.0.1/.editorconfig
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 infisical-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/__version__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/constants.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/logger.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/models.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/api/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/api/get_secrets.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/api/get_service_token_data.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/api/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/client/__init__.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/client/infisicalclient.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/services/__init__.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/services/key_service.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/services/secret_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/utils/__init__.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/utils/crypto.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 infisical-1.0.1/infisical/utils/http.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 infisical-1.0.1/scripts/format.sh
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 infisical-1.0.1/scripts/lint.sh
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 infisical-1.0.1/scripts/test.sh
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_infisical.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/data/__init__.py
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/data/secrets_reponse.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/data/service_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_api/__init__.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_api/test_api_request.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_api/test_get_secrets.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_api/test_get_service_token_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_client/__init__.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_client/test_infisical_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_services/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_services/test_key_service.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_services/test_secret_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_utils/test_crypto_decrypt_asymmetric.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_utils/test_crypto_decrypt_symmetric.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_utils/test_crypto_encrypt_asymmetric.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 infisical-1.0.1/tests/test_utils/test_crypto_encrypt_symmetric.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 infisical-1.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 infisical-1.0.1/LICENSE
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 infisical-1.0.1/README.md
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 infisical-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 infisical-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 infisical-1.1.0/.editorconfig
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 infisical-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 infisical-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/__version__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/constants.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/logger.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/__init__.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/create_secret.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/delete_secret.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/get_secret.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/get_secrets.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/get_service_token_data.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/models.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/api/update_secret.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/client/__init__.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/client/infisicalclient.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/helpers/__init__.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/helpers/client.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/helpers/secrets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/api.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/models.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/models/secret_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/services/__init__.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/services/secret_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/utils/__init__.py
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/utils/crypto.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 infisical-1.1.0/infisical/utils/http.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 infisical-1.1.0/scripts/format.sh
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 infisical-1.1.0/scripts/lint.sh
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 infisical-1.1.0/scripts/test.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/test_infisical.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/test_client/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 infisical-1.1.0/tests/test_client/test_infisical_client.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 infisical-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 infisical-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 infisical-1.1.0/README.md
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 infisical-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 infisical-1.1.0/PKG-INFO
```

### Comparing `infisical-1.0.1/infisical/api/__init__.py` & `infisical-1.1.0/infisical/api/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from infisical.__version__ import __version__
-from infisical.utils.http import BaseUrlSession, get_http_client
-
-USER_AGENT = f"InfisicalPythonSDK/{__version__}"
-
-
-def create_api_request_with_auth(base_url: str, service_token: str) -> BaseUrlSession:
-    """Returns a :class:`requests.Session` with a ``base_url`` and the authorization
-    bearer set to the ``service_token``.
-
-    :param base_url: The base url to use
-    :param service_token: The service token to use as a authorization bearer token
-    :return: A :class:`requests.Session` instance preconfigured
-    """
-    api_request = get_http_client(base_url=base_url.rstrip("/"))
-
-    api_request.headers.update({"User-Agent": USER_AGENT})
-    api_request.headers.update({"Content-Type": "application/json"})
-    api_request.headers.update({"Authorization": f"Bearer {service_token}"})
-
-    return api_request
+from infisical.__version__ import __version__
+from infisical.utils.http import BaseUrlSession, get_http_client
+
+USER_AGENT = f"InfisicalPythonSDK/{__version__}"
+
+
+def create_api_request_with_auth(base_url: str, service_token: str) -> BaseUrlSession:
+    """Returns a :class:`requests.Session` with a ``base_url`` and the authorization
+    bearer set to the ``service_token``.
+
+    :param base_url: The base url to use
+    :param service_token: The service token to use as a authorization bearer token
+    :return: A :class:`requests.Session` instance preconfigured
+    """
+    api_request = get_http_client(base_url=base_url.rstrip("/"))
+
+    api_request.headers.update({"User-Agent": USER_AGENT})
+    api_request.headers.update({"Content-Type": "application/json"})
+    api_request.headers.update({"Authorization": f"Bearer {service_token}"})
+
+    return api_request
```

### Comparing `infisical-1.0.1/infisical/api/get_secrets.py` & `infisical-1.1.0/infisical/api/get_secrets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from infisical.api.models import GetEncryptedSecretsV2Response
-from requests import Session
-
-
-def get_secrets(
-    api_request: Session, workspace_id: str, environment: str
-) -> GetEncryptedSecretsV2Response:
-    """Send request again Infisical API to fetch secrets.
-    See more information on https://infisical.com/docs/api-reference/endpoints/secrets/read
-
-    :param api_request: The :class:`requests.Session` instance used to perform the request
-    :param workspace_id: The ID of the workspace
-    :param environment: The environment
-    :return: Returns the API response as-is
-    """
-    response = api_request.get(
-        "/api/v2/secrets",
-        params={
-            "environment": environment,
-            "workspaceId": workspace_id,
-            "tagSlugs": "",
-        },
-    )
-
-    return GetEncryptedSecretsV2Response.parse_obj(response.json())
+from infisical.models.api import GetSecretsDTO, SecretsResponse
+from requests import Session
+
+
+def get_secrets_req(api_request: Session, options: GetSecretsDTO) -> SecretsResponse:
+    """Send request again Infisical API to fetch secrets.
+    See more information on https://infisical.com/docs/api-reference/endpoints/secrets/read
+
+    :param api_request: The :class:`requests.Session` instance used to perform the request
+    :param workspace_id: The ID of the workspace
+    :param environment: The environment
+    :return: Returns the API response as-is
+    """
+    response = api_request.get(
+        "/api/v3/secrets",
+        params={
+            "environment": options.environment,
+            "workspaceId": options.workspace_id,
+        },
+    )
+
+    return SecretsResponse.parse_obj(response.json())
```

### Comparing `infisical-1.0.1/infisical/api/get_service_token_data.py` & `infisical-1.1.0/infisical/api/get_service_token_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from infisical.api.models import GetServiceTokenDetailsResponse
-from requests import Session
-
-
-def get_service_token_data(
-    api_request: Session,
-) -> GetServiceTokenDetailsResponse:
-    """Send request again Infisical API to fetch service token data.
-    See more information on https://infisical.com/docs/api-reference/endpoints/service-tokens/get
-
-    :param api_request: The :class:`requests.Session` instance used to perform the request
-    :return: Returns the API response as-is
-    """
-    response = api_request.get("/api/v2/service-token")
-
-    return GetServiceTokenDetailsResponse.parse_obj(response.json())
+from infisical.api.models import GetServiceTokenDetailsResponse
+from requests import Session
+
+
+def get_service_token_data_req(
+    api_request: Session,
+) -> GetServiceTokenDetailsResponse:
+    """Send request again Infisical API to fetch service token data.
+    See more information on https://infisical.com/docs/api-reference/endpoints/service-tokens/get
+
+    :param api_request: The :class:`requests.Session` instance used to perform the request
+    :return: Returns the API response as-is
+    """
+    response = api_request.get("/api/v2/service-token")
+
+    return GetServiceTokenDetailsResponse.parse_obj(response.json())
```

### Comparing `infisical-1.0.1/infisical/utils/crypto.py` & `infisical-1.1.0/infisical/utils/crypto.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from Cryptodome.Cipher import AES
 from Cryptodome.Random import get_random_bytes
 from nacl import public, utils
 
 Base64String = str
 Buffer = Union[bytes, bytearray, memoryview]
+import binascii
 
 
 def encrypt_asymmetric(
     plaintext: Union[Buffer, str],
     public_key: Union[Buffer, Base64String, public.PublicKey],
     private_key: Union[Buffer, Base64String, public.PrivateKey],
 ) -> Tuple[Base64String, Base64String]:
@@ -107,71 +108,60 @@
     box = public.Box(m_private_key, m_public_key)
     plaintext = box.decrypt(m_ciphertext, m_nonce)
 
     return plaintext.decode("utf-8")
 
 
 def encrypt_symmetric(
-    plaintext: Union[Buffer, str], key: Union[Buffer, Base64String]
+    plaintext: str, key: str
 ) -> Tuple[Base64String, Base64String, Base64String]:
     """Encrypts the ``plaintext`` with aes-256-gcm using the given ``key``.
     The key should be either the raw value in bytes or a base64 string.
 
-    :param plaintext: The text to encrypt
-    :param key: The AES key used for encryption
+    :param plaintext: text to encrypt
+    :param key: UTF-8, 128-bit AES key used for encryption
     :raises ValueError: If either ``plaintext`` or ``key`` is empty
     :return: Ciphered text
     """
     if len(key) == 0:
         raise ValueError("The given key is empty!")
 
     BLOCK_SIZE_BYTES = 16
 
-    m_key = b64decode(key) if isinstance(key, Base64String) else key
-    m_plaintext = (
-        str.encode(plaintext, "utf-8") if isinstance(plaintext, str) else plaintext
-    )
-
     iv = get_random_bytes(BLOCK_SIZE_BYTES)
-    cipher = AES.new(m_key, AES.MODE_GCM, nonce=iv)
+    cipher = AES.new(bytes(key, "utf-8"), AES.MODE_GCM, nonce=iv)
 
-    cipher_text, tag = cipher.encrypt_and_digest(m_plaintext)
+    ciphertext, tag = cipher.encrypt_and_digest(str.encode(plaintext, "utf-8"))
 
     return (
-        b64encode(cipher_text).decode("utf-8"),
+        b64encode(ciphertext).decode("utf-8"),
         b64encode(iv).decode("utf-8"),
         b64encode(tag).decode("utf-8"),
     )
 
 
-def decrypt_symmetric(
-    key: Union[Buffer, Base64String],
-    ciphertext: Union[Buffer, Base64String],
-    tag: Union[Buffer, Base64String],
-    iv: Union[Buffer, Base64String],
-) -> str:
+def decrypt_symmetric(key: str, ciphertext: str, tag: str, iv: str) -> str:
     """Decrypts the ``ciphertext`` with aes-256-gcm using ``iv``, ``tag``
-    and ``key``. Each of those params should be either the raw value in bytes
-    or a base64 string.
+    and ``key``.
 
-    :param key: The AES key
-    :param ciphertext: The ciphered text to decrypt
-    :param tag: The tag/mac used for verification
-    :param iv: The nonce
+    :param key: UTF-8, 128-bit hex AES key
+    :param ciphertext: base64 ciphered text to decrypt
+    :param tag: base64 tag/mac used for verification
+    :param iv: base64 nonce
     :raises ValueError: If ``ciphertext``, ``iv``, ``tag`` or ``key`` are empty or tag/mac does not match
     :return: Deciphered text
     """
     if len(tag) == 0 or len(iv) == 0 or len(key) == 0:
         raise ValueError("One of the given parameter is empty!")
 
-    m_key = b64decode(key) if isinstance(key, Base64String) else key
-    m_iv = b64decode(iv) if isinstance(iv, Base64String) else iv
-    m_ciphertext = (
-        b64decode(ciphertext) if isinstance(ciphertext, Base64String) else ciphertext
-    )
-    m_tag = b64decode(tag) if isinstance(tag, Base64String) else tag
-
-    cipher = AES.new(m_key, AES.MODE_GCM, nonce=m_iv)
-
-    plaintext = cipher.decrypt_and_verify(m_ciphertext, m_tag)
-
-    return plaintext.decode("utf-8")
+    try:
+        key = bytes(key, "utf-8")
+        iv = b64decode(iv)
+        tag = b64decode(tag)
+        ciphertext = b64decode(ciphertext)
+
+        cipher = AES.new(key, AES.MODE_GCM, nonce=iv)
+        plaintext = cipher.decrypt_and_verify(ciphertext, tag)
+
+        return plaintext.decode("utf-8")
+    except ValueError:
+        raise ValueError("Incorrect decryption or MAC check failed")
```

### Comparing `infisical-1.0.1/infisical/utils/http.py` & `infisical-1.1.0/infisical/utils/http.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from typing import Any, Optional, Union
-from urllib.parse import urljoin
-
-import requests
-from requests.adapters import HTTPAdapter
-from urllib3.util import Retry
-
-DEFAULT_TIMEOUT = 40  # seconds
-
-
-class BaseUrlSession(requests.Session):
-    base_url = ""
-
-    def __init__(self, base_url: Optional[str] = None) -> None:
-        if base_url:
-            self.base_url = base_url
-        super().__init__()
-
-    def request(
-        self,
-        method: Union[str, bytes],
-        url: Any,
-        *args: Any,
-        **kwargs: Any,
-    ) -> requests.Response:
-        url = self.create_url(url)
-        return super().request(method, url, *args, **kwargs)
-
-    def prepare_request(self, request: requests.Request) -> requests.PreparedRequest:
-        request.url = self.create_url(request.url)
-        return super().prepare_request(request)
-
-    def create_url(self, url: str) -> str:
-        return urljoin(self.base_url, url)
-
-
-class TimeoutHTTPAdapter(HTTPAdapter):
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        self.timeout = DEFAULT_TIMEOUT
-        if "timeout" in kwargs:
-            self.timeout = kwargs["timeout"]
-            del kwargs["timeout"]
-        super().__init__(*args, **kwargs)
-
-    def send(
-        self, request: requests.PreparedRequest, *args: Any, **kwargs: Any
-    ) -> requests.Response:
-        timeout = kwargs.get("timeout")
-        if timeout is None:
-            kwargs["timeout"] = self.timeout
-        return super().send(request, *args, **kwargs)
-
-
-def get_http_client(
-    base_url: Optional[str],
-    retries: int = 3,
-    backoff_factor: int = 1,
-    timeout: int = DEFAULT_TIMEOUT,
-) -> BaseUrlSession:
-    """Returns a pre-configured :class:`requests.Session` with a optional ``base_url``
-    and some sane options for timeout and retry handling.
-
-    :param base_url: (optional) A base url used for each request made with this client
-    :param retries: The number of retries to do if request fail, defaults to 3
-    :param backoff_factor: A backoff factor to apply between attempts after the second try, defaults to 1
-    :param timeout: The timeout in seconds, defaults to 40
-    :return: A ready-to-use instance of :class:`requests.Session`
-    """
-    retry_strategy = Retry(
-        total=retries,
-        backoff_factor=backoff_factor,
-        status_forcelist=[429, 500, 502, 503, 504],
-    )
-    adapter = TimeoutHTTPAdapter(max_retries=retry_strategy, timeout=timeout)
-
-    http = BaseUrlSession(base_url=base_url)
-    http.mount("https://", adapter)
-    http.mount("http://", adapter)
-
-    return http
+from typing import Any, Optional, Union
+from urllib.parse import urljoin
+
+import requests
+from requests.adapters import HTTPAdapter
+from urllib3.util import Retry
+
+DEFAULT_TIMEOUT = 40  # seconds
+
+
+class BaseUrlSession(requests.Session):
+    base_url = ""
+
+    def __init__(self, base_url: Optional[str] = None) -> None:
+        if base_url:
+            self.base_url = base_url
+        super().__init__()
+
+    def request(
+        self,
+        method: Union[str, bytes],
+        url: Any,
+        *args: Any,
+        **kwargs: Any,
+    ) -> requests.Response:
+        url = self.create_url(url)
+        return super().request(method, url, *args, **kwargs)
+
+    def prepare_request(self, request: requests.Request) -> requests.PreparedRequest:
+        request.url = self.create_url(request.url)
+        return super().prepare_request(request)
+
+    def create_url(self, url: str) -> str:
+        return urljoin(self.base_url, url)
+
+
+class TimeoutHTTPAdapter(HTTPAdapter):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        self.timeout = DEFAULT_TIMEOUT
+        if "timeout" in kwargs:
+            self.timeout = kwargs["timeout"]
+            del kwargs["timeout"]
+        super().__init__(*args, **kwargs)
+
+    def send(
+        self, request: requests.PreparedRequest, *args: Any, **kwargs: Any
+    ) -> requests.Response:
+        timeout = kwargs.get("timeout")
+        if timeout is None:
+            kwargs["timeout"] = self.timeout
+        return super().send(request, *args, **kwargs)
+
+
+def get_http_client(
+    base_url: Optional[str],
+    retries: int = 3,
+    backoff_factor: int = 1,
+    timeout: int = DEFAULT_TIMEOUT,
+) -> BaseUrlSession:
+    """Returns a pre-configured :class:`requests.Session` with a optional ``base_url``
+    and some sane options for timeout and retry handling.
+
+    :param base_url: (optional) A base url used for each request made with this client
+    :param retries: The number of retries to do if request fail, defaults to 3
+    :param backoff_factor: A backoff factor to apply between attempts after the second try, defaults to 1
+    :param timeout: The timeout in seconds, defaults to 40
+    :return: A ready-to-use instance of :class:`requests.Session`
+    """
+    retry_strategy = Retry(
+        total=retries,
+        backoff_factor=backoff_factor,
+        status_forcelist=[429, 500, 502, 503, 504],
+    )
+    adapter = TimeoutHTTPAdapter(max_retries=retry_strategy, timeout=timeout)
+
+    http = BaseUrlSession(base_url=base_url)
+    http.mount("https://", adapter)
+    http.mount("http://", adapter)
+
+    return http
```

### Comparing `infisical-1.0.1/.gitignore` & `infisical-1.1.0/.gitignore`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-
-# Created by https://www.toptal.com/developers/gitignore/api/windows,linux,python,visualstudiocode
-# Edit at https://www.toptal.com/developers/gitignore?templates=windows,linux,python,visualstudiocode
-
-### Linux ###
-*~
-
-# temporary files which can be created if a process still has a handle open of a deleted file
-.fuse_hidden*
-
-# KDE directory preferences
-.directory
-
-# Linux trash folder which might appear on any partition or disk
-.Trash-*
-
-# .nfs files are created when an open file is removed but is still being accessed
-.nfs*
-
-### Python ###
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Ruff
-.ruff_cache/
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-### Windows ###
-# Windows thumbnail cache files
-Thumbs.db
-Thumbs.db:encryptable
-ehthumbs.db
-ehthumbs_vista.db
-
-# Dump file
-*.stackdump
-
-# Folder config file
-[Dd]esktop.ini
-
-# Recycle Bin used on file shares
-$RECYCLE.BIN/
-
-# Windows Installer files
-*.cab
-*.msi
-*.msix
-*.msm
-*.msp
-
-# Windows shortcuts
-*.lnk
-
-### VisualStudioCode ###
-.vscode/*
-!.vscode/settings.json
-!.vscode/tasks.json
-!.vscode/launch.json
-!.vscode/extensions.json
-*.code-workspace
-
-# Local History for Visual Studio Code
-.history/
-
-### VisualStudioCode Patch ###
-# Ignore all local history of files
-.history
-.ionide
-
-# End of https://www.toptal.com/developers/gitignore/api/windows,linux,python,visualstudiocode
-
-.infisical.json
+
+# Created by https://www.toptal.com/developers/gitignore/api/windows,linux,python,visualstudiocode
+# Edit at https://www.toptal.com/developers/gitignore?templates=windows,linux,python,visualstudiocode
+
+### Linux ###
+*~
+
+# temporary files which can be created if a process still has a handle open of a deleted file
+.fuse_hidden*
+
+# KDE directory preferences
+.directory
+
+# Linux trash folder which might appear on any partition or disk
+.Trash-*
+
+# .nfs files are created when an open file is removed but is still being accessed
+.nfs*
+
+### Python ###
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Ruff
+.ruff_cache/
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+### Windows ###
+# Windows thumbnail cache files
+Thumbs.db
+Thumbs.db:encryptable
+ehthumbs.db
+ehthumbs_vista.db
+
+# Dump file
+*.stackdump
+
+# Folder config file
+[Dd]esktop.ini
+
+# Recycle Bin used on file shares
+$RECYCLE.BIN/
+
+# Windows Installer files
+*.cab
+*.msi
+*.msix
+*.msm
+*.msp
+
+# Windows shortcuts
+*.lnk
+
+### VisualStudioCode ###
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
+*.code-workspace
+
+# Local History for Visual Studio Code
+.history/
+
+### VisualStudioCode Patch ###
+# Ignore all local history of files
+.history
+.ionide
+
+# End of https://www.toptal.com/developers/gitignore/api/windows,linux,python,visualstudiocode
+
+.infisical.json
```

### Comparing `infisical-1.0.1/LICENSE` & `infisical-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Yohann MARTIN
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Yohann MARTIN
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

