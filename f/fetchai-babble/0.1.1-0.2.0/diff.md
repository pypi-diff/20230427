# Comparing `tmp/fetchai_babble-0.1.1.tar.gz` & `tmp/fetchai_babble-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchai_babble-0.1.1.tar", max compression
+gzip compressed data, was "fetchai_babble-0.2.0.tar", max compression
```

## Comparing `fetchai_babble-0.1.1.tar` & `fetchai_babble-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-03-14 15:29:41.621719 fetchai_babble-0.1.1/LICENSE
--rw-r--r--   0        0        0      730 2023-01-30 14:03:36.544062 fetchai_babble-0.1.1/README.md
--rw-r--r--   0        0        0      616 2023-04-01 12:53:17.476534 fetchai_babble-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-02-28 15:03:09.430563 fetchai_babble-0.1.1/src/babble/__init__.py
--rw-r--r--   0        0        0     1594 2023-01-30 14:03:36.548062 fetchai_babble-0.1.1/src/babble/auth.py
--rw-r--r--   0        0        0     5874 2023-03-14 13:54:25.624660 fetchai_babble-0.1.1/src/babble/client.py
--rw-r--r--   0        0        0      162 2023-03-30 10:25:37.450431 fetchai_babble-0.1.1/src/babble/config.py
--rw-r--r--   0        0        0       31 2023-01-30 14:03:36.548062 fetchai_babble-0.1.1/src/babble/crypto/__init__.py
--rw-r--r--   0        0        0       90 2023-01-30 14:03:36.548062 fetchai_babble-0.1.1/src/babble/crypto/exceptions.py
--rw-r--r--   0        0        0      272 2023-01-30 14:03:36.548062 fetchai_babble-0.1.1/src/babble/crypto/hashfuncs.py
--rw-r--r--   0        0        0     2911 2023-01-30 14:03:36.548062 fetchai_babble-0.1.1/src/babble/crypto/identity.py
--rw-r--r--   0        0        0      457 2023-01-30 14:03:36.548062 fetchai_babble-0.1.1/src/babble/encoding.py
--rw-r--r--   0        0        0     3969 2023-03-30 10:25:37.450431 fetchai_babble-0.1.1/src/babble/mailbox.py
--rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 fetchai_babble-0.1.1/setup.py
--rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 fetchai_babble-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 15:29:41.621719 fetchai_babble-0.2.0/LICENSE
+-rw-r--r--   0        0        0      730 2023-01-30 14:03:36.544062 fetchai_babble-0.2.0/README.md
+-rw-r--r--   0        0        0      616 2023-04-27 07:56:55.315343 fetchai_babble-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-02-28 15:03:09.430563 fetchai_babble-0.2.0/src/babble/__init__.py
+-rw-r--r--   0        0        0     1594 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/auth.py
+-rw-r--r--   0        0        0     5925 2023-04-27 07:56:38.515274 fetchai_babble-0.2.0/src/babble/client.py
+-rw-r--r--   0        0        0      247 2023-04-27 07:56:38.515274 fetchai_babble-0.2.0/src/babble/config.py
+-rw-r--r--   0        0        0       31 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/__init__.py
+-rw-r--r--   0        0        0       90 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/exceptions.py
+-rw-r--r--   0        0        0      272 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/hashfuncs.py
+-rw-r--r--   0        0        0     2911 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/identity.py
+-rw-r--r--   0        0        0      457 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/encoding.py
+-rw-r--r--   0        0        0     3969 2023-03-30 10:25:37.450431 fetchai_babble-0.2.0/src/babble/mailbox.py
+-rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 fetchai_babble-0.2.0/setup.py
+-rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 fetchai_babble-0.2.0/PKG-INFO
```

### Comparing `fetchai_babble-0.1.1/LICENSE` & `fetchai_babble-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.1.1/README.md` & `fetchai_babble-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.1.1/pyproject.toml` & `fetchai_babble-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fetchai-babble"
-version = "0.1.1"
+version = "0.2.0"
 description = "A simple python library for interacting with the Fetch.ai messaging service (called Memorandum)"
 authors = ["Fetch.AI Limited"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "babble", from = "src" }]
```

### Comparing `fetchai_babble-0.1.1/src/babble/auth.py` & `fetchai_babble-0.2.0/src/babble/auth.py`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.1.1/src/babble/client.py` & `fetchai_babble-0.2.0/src/babble/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     hrp, _ = bech32.bech32_decode(address)
     if hrp is None or hrp not in ("fetch", "agent"):
         raise ValueError(f"Bad delegate address {address}")
 
 
 @dataclass
 class Message:
+    id: str
     sender: str
     target: str
     text: str
     sent_at: datetime
     expires_at: datetime
 
 
@@ -137,14 +138,15 @@
             envelope = from_json(from_base64(raw_message.contents))
             payload = from_json(from_base64(envelope["data"]))
             encrypted_message = from_base64(payload["encryptedTargetData"])
             message = from_json(self._identity.decrypt_message(encrypted_message))
 
             output.append(
                 Message(
+                    id=raw_message.id,
                     sender=raw_message.sender,
                     target=raw_message.target,
                     text=message["content"]["text"],
                     sent_at=raw_message.sent_at,
                     expires_at=raw_message.expires_at,
                 )
             )
```

### Comparing `fetchai_babble-0.1.1/src/babble/crypto/identity.py` & `fetchai_babble-0.2.0/src/babble/crypto/identity.py`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.1.1/src/babble/mailbox.py` & `fetchai_babble-0.2.0/src/babble/mailbox.py`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.1.1/setup.py` & `fetchai_babble-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'eciespy>=0.3.13,<0.4.0',
  'pycryptodome>=3.16.0,<4.0.0',
  'pyjwt>=2.6.0,<3.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'fetchai-babble',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'A simple python library for interacting with the Fetch.ai messaging service (called Memorandum)',
     'long_description': '# Babble\n\nA simple python library for interacting with the Fetch.ai messaging service (called Memorandum)\n\n## Quick Example\n\n```python\nfrom babble import Client, Identity\n\n# create a set of agents with random identities\nclient1 = Client(\'agent1.....\', Identity.generate())\nclient2 = Client(\'agent1.....\', Identity.generate())\n\n# send a message from one client to another\nclient1.send(client2.delegate_address, "why hello there")\n\n# receive the messages from the other client\nfor msg in client2.receive():\n    print(msg.text)\n```\n\n## Developing\n\n**Install dependencies**\n\n    poetry install\n\n**Run examples**\n\n    poetry run ./examples/simple-e2e.py\n\n**Run tests**\n\n    poetry run pytest\n\n**Run formatter**\n\n    poetry run black .\n',
     'author': 'Fetch.AI Limited',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fetchai_babble-0.1.1/PKG-INFO` & `fetchai_babble-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchai-babble
-Version: 0.1.1
+Version: 0.2.0
 Summary: A simple python library for interacting with the Fetch.ai messaging service (called Memorandum)
 License: Apache 2.0
 Author: Fetch.AI Limited
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

