# Comparing `tmp/cancelchain-1.3.0.tar.gz` & `tmp/cancelchain-1.3.1.tar.gz`

## Comparing `cancelchain-1.3.0.tar` & `cancelchain-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/__init__.py
--rw-r--r--   0        0        0    17826 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/api.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/api_client.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/application.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/block.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/browser.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/cache.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/chain.py
--rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/command.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/config.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/console.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/database.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/exceptions.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/miller.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/milling.py
--rw-r--r--   0        0        0    20782 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/models.py
--rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/node.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/payload.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/schema.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/signals.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/tasks.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/transaction.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/util.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/wallet.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/base.html
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/block.html
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/chains.html
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/index.html
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/transaction.html
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.3.0/.gitignore
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.3.0/LICENSE
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 cancelchain-1.3.0/README.rst
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 cancelchain-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/__init__.py
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/api.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/api_client.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/application.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/block.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/browser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/cache.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/chain.py
+-rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/command.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/config.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/console.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/database.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/exceptions.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/miller.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/milling.py
+-rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/models.py
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/node.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/payload.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/schema.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/signals.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/tasks.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/transaction.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/util.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/wallet.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/base.html
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/block.html
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/chains.html
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/index.html
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/transaction.html
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.3.1/.gitignore
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.3.1/LICENSE
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 cancelchain-1.3.1/README.rst
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 cancelchain-1.3.1/PKG-INFO
```

### Comparing `cancelchain-1.3.0/src/cancelchain/__init__.py` & `cancelchain-1.3.1/src/cancelchain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import click
 from flask import Flask
 from flask.cli import FlaskGroup
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 
 def create_app(app=None, register_browser=True, test_config=None):
     from .application import init_app
     from .cache import cache
     from .config import EnvAppSettings
     from .database import db
```

### Comparing `cancelchain-1.3.0/src/cancelchain/api.py` & `cancelchain-1.3.1/src/cancelchain/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,16 @@
                         authorized = True
             except jwt.exceptions.ExpiredSignatureError:
                 abort(401)
             except Exception as e:
                 current_app.logger.exception(e)
                 abort(401)
             if authorized:
+                kwargs['_address'] = address
+                kwargs['_role'] = role
                 return func(*args, **kwargs)
             abort(401)
         return wrapper
     return _authorize
 
 
 authorize_reader = authorize(required_role=Role.READER)
```

### Comparing `cancelchain-1.3.0/src/cancelchain/api_client.py` & `cancelchain-1.3.1/src/cancelchain/api_client.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/application.py` & `cancelchain-1.3.1/src/cancelchain/application.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/block.py` & `cancelchain-1.3.1/src/cancelchain/block.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/browser.py` & `cancelchain-1.3.1/src/cancelchain/browser.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/chain.py` & `cancelchain-1.3.1/src/cancelchain/chain.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/command.py` & `cancelchain-1.3.1/src/cancelchain/command.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/config.py` & `cancelchain-1.3.1/src/cancelchain/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         return os.environ.get(f'{cls._prefix}{name}')
 
     @classmethod
     def from_env(cls):
         c = cls()
         for f in fields(c):
             if (v := cls.getenv(f.name)) is not None:
+                v = v.strip()
                 try:
                     setattr(c, f.name, json.loads(v))
                 except Exception:
                     setattr(c, f.name, v)
         return c
```

### Comparing `cancelchain-1.3.0/src/cancelchain/exceptions.py` & `cancelchain-1.3.1/src/cancelchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/miller.py` & `cancelchain-1.3.1/src/cancelchain/miller.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/milling.py` & `cancelchain-1.3.1/src/cancelchain/milling.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/models.py` & `cancelchain-1.3.1/src/cancelchain/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from passlib.hash import argon2, pbkdf2_sha256
 
 from cancelchain.database import db
 from cancelchain.wallet import Wallet
 
 
-def rollback_sesssion():
+def rollback_session():
     db.session.rollback()
 
 
 block_transactions = db.Table(
     'block_transaction',
     db.Column(
         'block_id', db.Integer, db.ForeignKey('block.id'),
```

### Comparing `cancelchain-1.3.0/src/cancelchain/node.py` & `cancelchain-1.3.1/src/cancelchain/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     InvalidTransactionIdError,
     MissingBlockError,
 )
 from cancelchain.models import (
     ChainDAO,
     ChainFill,
     ChainFillBlock,
-    rollback_sesssion,
+    rollback_session,
 )
 from cancelchain.signals import new_block as new_block_signal
 from cancelchain.transaction import PendingTxnSet, Transaction
 from cancelchain.util import host_address, now
 
 
 class Node():
@@ -61,15 +61,15 @@
         if txid != txn.txid:
             raise InvalidTransactionIdError()
         txn.validate()
         if txn not in self.pending_txns:
             try:
                 self.pending_txns.add(txn)
             except SQLAlchemyError:
-                rollback_sesssion()
+                rollback_session()
                 if txn.txid not in self.pending_txns:
                     raise
             added = True
         if process:
             self.send_transaction(txn, visited_hosts=visited_hosts)
         return txn if added else None
 
@@ -131,15 +131,15 @@
             chain = Chain.from_db(block_hash=block.prev_hash)
             if chain:
                 chain.add_block(block)
             else:
                 chain = self.create_chain(block=block)
             chain.to_db()
         except SQLAlchemyError:
-            rollback_sesssion()
+            rollback_session()
             if not Block.from_db(block.block_hash):
                 raise
             block = None
         return block
 
     def create_chain(self, block=None):
         block_hash = block.prev_hash if block else None
```

### Comparing `cancelchain-1.3.0/src/cancelchain/payload.py` & `cancelchain-1.3.1/src/cancelchain/payload.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/schema.py` & `cancelchain-1.3.1/src/cancelchain/schema.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/tasks.py` & `cancelchain-1.3.1/src/cancelchain/tasks.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/transaction.py` & `cancelchain-1.3.1/src/cancelchain/transaction.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/util.py` & `cancelchain-1.3.1/src/cancelchain/util.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/wallet.py` & `cancelchain-1.3.1/src/cancelchain/wallet.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/templates/base.html` & `cancelchain-1.3.1/src/cancelchain/templates/base.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/templates/block.html` & `cancelchain-1.3.1/src/cancelchain/templates/block.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/templates/chains.html` & `cancelchain-1.3.1/src/cancelchain/templates/chains.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/templates/index.html` & `cancelchain-1.3.1/src/cancelchain/templates/index.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/src/cancelchain/templates/transaction.html` & `cancelchain-1.3.1/src/cancelchain/templates/transaction.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/.gitignore` & `cancelchain-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/LICENSE` & `cancelchain-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/README.rst` & `cancelchain-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/pyproject.toml` & `cancelchain-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.0/PKG-INFO` & `cancelchain-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cancelchain
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Blockchain of Accountability, Support, and Forgiveness
 Project-URL: Homepage, https://cancelchain.org
 Project-URL: Documentation, https://docs.cancelchain.org
 Project-URL: Source, https://github.com/cancelchain/cancelchain
 Project-URL: Tracker, https://github.com/cancelchain/cancelchain/issues
 Author-email: Thomas Bohmbach Jr <tom@cancelchain.org>
 License-Expression: MIT
```

