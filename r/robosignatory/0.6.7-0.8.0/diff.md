# Comparing `tmp/robosignatory-0.6.7.tar.gz` & `tmp/robosignatory-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robosignatory-0.6.7.tar", last modified: Wed Jun 10 15:36:26 2020, max compression
+gzip compressed data, was "robosignatory-0.8.0.tar", last modified: Thu Apr 27 11:58:15 2023, max compression
```

## Comparing `robosignatory-0.6.7.tar` & `robosignatory-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxr-x   0 abompard  (1000) abompard  (1000)        0 2020-06-10 15:36:26.362180 robosignatory-0.6.7/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    18002 2019-07-22 15:20:56.000000 robosignatory-0.6.7/LICENSE
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      107 2019-09-12 10:42:38.000000 robosignatory-0.6.7/MANIFEST.in
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      288 2020-06-10 15:36:26.362180 robosignatory-0.6.7/PKG-INFO
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     4320 2019-09-05 15:07:46.000000 robosignatory-0.6.7/README.rst
-drwxrwxr-x   0 abompard  (1000) abompard  (1000)        0 2020-06-10 15:36:26.360180 robosignatory-0.6.7/robosignatory/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2019-07-22 15:20:56.000000 robosignatory-0.6.7/robosignatory/__init__.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1511 2019-10-11 21:01:24.000000 robosignatory-0.6.7/robosignatory/atomic.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2437 2019-09-18 14:31:08.000000 robosignatory-0.6.7/robosignatory/cli.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2063 2019-09-09 15:45:16.000000 robosignatory-0.6.7/robosignatory/consumer.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     6872 2020-06-10 15:34:07.000000 robosignatory-0.6.7/robosignatory/coreos.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    11892 2019-10-02 13:47:07.000000 robosignatory-0.6.7/robosignatory/tag.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     4952 2019-09-16 12:25:10.000000 robosignatory-0.6.7/robosignatory/utils.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2415 2020-06-10 15:34:07.000000 robosignatory-0.6.7/robosignatory/work.py
-drwxrwxr-x   0 abompard  (1000) abompard  (1000)        0 2020-06-10 15:36:26.360180 robosignatory-0.6.7/robosignatory.egg-info/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      288 2020-06-10 15:36:26.000000 robosignatory-0.6.7/robosignatory.egg-info/PKG-INFO
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      609 2020-06-10 15:36:26.000000 robosignatory-0.6.7/robosignatory.egg-info/SOURCES.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2020-06-10 15:36:26.000000 robosignatory-0.6.7/robosignatory.egg-info/dependency_links.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      192 2020-06-10 15:36:26.000000 robosignatory-0.6.7/robosignatory.egg-info/entry_points.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       40 2020-06-10 15:36:26.000000 robosignatory-0.6.7/robosignatory.egg-info/requires.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       14 2020-06-10 15:36:26.000000 robosignatory-0.6.7/robosignatory.egg-info/top_level.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     3865 2020-06-10 15:34:07.000000 robosignatory-0.6.7/robosignatory.toml
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      315 2020-06-10 15:36:26.362180 robosignatory-0.6.7/setup.cfg
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1669 2020-06-10 15:35:00.000000 robosignatory-0.6.7/setup.py
-drwxrwxr-x   0 abompard  (1000) abompard  (1000)        0 2020-06-10 15:36:26.361180 robosignatory-0.6.7/tests/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2019-07-22 15:20:56.000000 robosignatory-0.6.7/tests/__init__.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2171 2019-10-11 21:02:12.000000 robosignatory-0.6.7/tests/test_atomic.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2885 2019-09-09 15:45:16.000000 robosignatory-0.6.7/tests/test_consumers.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     7718 2020-06-10 15:34:07.000000 robosignatory-0.6.7/tests/test_coreos.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    15098 2020-06-10 15:34:07.000000 robosignatory-0.6.7/tests/test_tag.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      839 2019-09-05 15:07:46.000000 robosignatory-0.6.7/tests/test_utils.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      309 2019-10-10 14:27:50.000000 robosignatory-0.6.7/tox.ini
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-04-27 11:58:15.888037 robosignatory-0.8.0/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    18002 2019-07-22 15:20:56.000000 robosignatory-0.8.0/LICENSE
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      107 2019-09-12 10:42:38.000000 robosignatory-0.8.0/MANIFEST.in
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      271 2023-04-27 11:58:15.888037 robosignatory-0.8.0/PKG-INFO
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     4320 2019-09-05 15:07:46.000000 robosignatory-0.8.0/README.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      207 2023-04-25 09:40:57.000000 robosignatory-0.8.0/pyproject.toml
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-04-27 11:58:15.885037 robosignatory-0.8.0/robosignatory/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2019-07-22 15:20:56.000000 robosignatory-0.8.0/robosignatory/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1445 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/atomic.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2371 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/cli.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2236 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/consumer.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     6763 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/coreos.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    12068 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/tag.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     6064 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/utils.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2381 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/work.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3448 2023-04-25 09:40:57.000000 robosignatory-0.8.0/robosignatory/xml.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-04-27 11:58:15.886036 robosignatory-0.8.0/robosignatory.egg-info/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      271 2023-04-27 11:58:15.000000 robosignatory-0.8.0/robosignatory.egg-info/PKG-INFO
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      663 2023-04-27 11:58:15.000000 robosignatory-0.8.0/robosignatory.egg-info/SOURCES.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2023-04-27 11:58:15.000000 robosignatory-0.8.0/robosignatory.egg-info/dependency_links.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      167 2023-04-27 11:58:15.000000 robosignatory-0.8.0/robosignatory.egg-info/entry_points.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       47 2023-04-27 11:58:15.000000 robosignatory-0.8.0/robosignatory.egg-info/requires.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       14 2023-04-27 11:58:15.000000 robosignatory-0.8.0/robosignatory.egg-info/top_level.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     4090 2023-04-24 13:14:48.000000 robosignatory-0.8.0/robosignatory.toml
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      315 2023-04-27 11:58:15.889037 robosignatory-0.8.0/setup.cfg
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1676 2023-04-27 11:53:15.000000 robosignatory-0.8.0/setup.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-04-27 11:58:15.888037 robosignatory-0.8.0/tests/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2019-07-22 15:20:56.000000 robosignatory-0.8.0/tests/__init__.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2184 2023-04-25 09:17:58.000000 robosignatory-0.8.0/tests/test_atomic.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2949 2023-04-25 09:16:51.000000 robosignatory-0.8.0/tests/test_consumers.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     7792 2023-04-25 09:18:57.000000 robosignatory-0.8.0/tests/test_coreos.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    17802 2023-04-25 09:40:57.000000 robosignatory-0.8.0/tests/test_tag.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1734 2023-04-24 13:14:47.000000 robosignatory-0.8.0/tests/test_utils.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2704 2023-04-25 09:20:53.000000 robosignatory-0.8.0/tests/test_xml.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      404 2023-04-25 09:40:57.000000 robosignatory-0.8.0/tox.ini
```

### Comparing `robosignatory-0.6.7/LICENSE` & `robosignatory-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robosignatory-0.6.7/README.rst` & `robosignatory-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `robosignatory-0.6.7/robosignatory/atomic.py` & `robosignatory-0.8.0/robosignatory/atomic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from __future__ import unicode_literals, absolute_import
-
 import robosignatory.utils as utils
 import robosignatory.work
 
 import logging
 log = logging.getLogger("robosignatory.atomicconsumer")
 
 
-class AtomicSigner(object):
+class AtomicSigner:
 
     def __init__(self, config):
         self.config = config
         self.signer = utils.get_signing_helper(**self.config["signing"])
 
         self.refs = {}
         for ref, val in self.config['ostree_refs'].items():
             if 'ref_to' in val:
-                raise ValueError('ref_to in %s found. This is depricated' %
+                raise ValueError('ref_to in %s found. This is deprecated' %
                                  ref)
             self.refs[ref] = val
 
         log.info('AtomicSigner ready for service')
 
     def consume(self, msg):
         # Example message:
@@ -32,16 +30,16 @@
         #   u'compose_id': u'Fedora-25-20161002.n.0'}
 
         ref = msg.body['ref']
         commitid = msg.body['commitid']
         if commitid is None:
             return
 
-        log.info('pungi composed %(ref)s (%(commitid)s, variant %(variant)s, '
-                 'arch %(arch)s)' % msg.body)
+        log.info('pungi composed {ref} ({commitid}, variant {variant}, '
+                 'arch {arch})'.format(**msg.body))
 
         if ref not in self.refs:
             log.info('Unknown reference %s. Skipping' % ref)
             return
 
         val = self.refs[ref]
```

### Comparing `robosignatory-0.6.7/robosignatory/cli.py` & `robosignatory-0.8.0/robosignatory/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals, absolute_import
-
 import os
 
 import click
 from fedora_messaging.config import conf
 
 import robosignatory.work
 from robosignatory.tag import TagSigner
@@ -18,15 +16,15 @@
     "-c", "--config",
     default="/etc/fedora-messaging/robosignatory.toml",
     type=click.Path(exists=True, dir_okay=False),
     help="Path to the configuration file"
 )
 def cli(config):
     if not os.path.isfile(config):
-        raise click.exceptions.BadParameter("{} is not a file".format(config))
+        raise click.exceptions.BadParameter(f"{config} is not a file")
     conf.load_config(config_path=config)
     conf.setup_logging()
 
 
 @cli.command("sign-tag")
 @click.option("--tag", is_flag=True)
 @click.argument("koji_instance")
```

### Comparing `robosignatory-0.6.7/robosignatory/consumer.py` & `robosignatory-0.8.0/robosignatory/consumer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from __future__ import unicode_literals, absolute_import
-
 import logging
 
 import fedora_messaging
 
 from .tag import TagSigner
 from .atomic import AtomicSigner
 from .coreos import CoreOSSigner
+from .xml import XMLSigner
 
 
 log = logging.getLogger('robosignatory')
 
 
-class Consumer(object):
+class Consumer:
     """All messages are received by this class's __call__() method."""
 
     def __init__(self):
         log.info('Initializing Robosignatory consumer')
         self.config = fedora_messaging.config.conf["consumer_config"]
         self.tag_handler = TagSigner(self.config)
         self.atomic_handler = AtomicSigner(self.config)
         self.coreos_handler = CoreOSSigner(self.config)
+        self.xml_handler = XMLSigner(self.config)
 
     def __call__(self, msg):
         """
         Callback method called by fedora-messaging consume.
 
         Redirect messages to the correct handler using the
         message topic.
@@ -45,11 +45,14 @@
             elif msg.topic.endswith('.pungi.compose.ostree'):
                 log.debug('Passing message to the Atomic handler')
                 self.atomic_handler.consume(msg)
             elif (msg.topic.endswith('.coreos.build.request.artifacts-sign')
                   or msg.topic.endswith('.coreos.build.request.ostree-sign')):
                 log.debug('Passing message to the CoreOS handler')
                 self.coreos_handler.consume(msg)
+            elif msg.topic.endswith('.robosignatory.xml-sign'):
+                log.debug('Passing message to the Text handler')
+                self.xml_handler.consume(msg)
         except Exception as e:
-            error_msg = '{e}: Unable to handle message: {msg}'.format(e=e, msg=msg)
+            error_msg = f'{e}: Unable to handle message: {msg}'
             log.exception(error_msg)
-            raise fedora_messaging.exceptions.Nack(error_msg)
+            raise fedora_messaging.exceptions.Nack(error_msg) from e
```

### Comparing `robosignatory-0.6.7/robosignatory/coreos.py` & `robosignatory-0.8.0/robosignatory/coreos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from __future__ import unicode_literals, absolute_import
-
 import os
 import stat
 import logging
 import shutil
 import tempfile
+from urllib.parse import urlparse
 
 import boto3
 import robosignatory.utils as utils
 from botocore.exceptions import ClientError
-from six.moves.urllib.parse import urlparse
 from fedora_messaging.api import Message, publish
 
 
 log = logging.getLogger(__name__)
 
 
-class CoreOSSigner(object):
+class CoreOSSigner:
 
     def __init__(self, config):
         self.config = config
 
         aws_config = self.config['coreos']['aws']
         s3 = boto3.resource(
             's3',
@@ -52,20 +50,20 @@
         return 'fedora-' + str(major)
 
     def consume(self, msg):
         # Message structure:
         # https://github.com/coreos/fedora-coreos-tracker/issues/198#issuecomment-513944390
         log.info(
             'CoreOS wants to sign '
-            '%(build_id)s for %(basearch)s' % msg.body
+            '{build_id} for {basearch}'.format(**msg.body)
         )
         key = self.get_key(msg)
 
         response = Message(
-            topic="{}.finished".format(msg.topic),
+            topic=f"{msg.topic}.finished",
             # respond with the same body, but clone so we keep the original one
             body=dict(msg.body)
         )
 
         try:
             if msg.topic.endswith('.coreos.build.request.artifacts-sign'):
                 wrapper = ArtifactSignerWrapper(self.signer, key, self.bucket)
@@ -85,15 +83,15 @@
             publish(response)
 
 
 class SigningFailed(Exception):
     pass
 
 
-class SignerWrapper(object):
+class SignerWrapper:
     """
     This class handles the common operations that come with signing a file in S3.
     """
 
     def __init__(self, signer, key, bucket):
         self.signer = signer
         self.key = key
@@ -103,52 +101,52 @@
         raise NotImplementedError
 
     def _get_cmdline(self, filepath):
         raise NotImplementedError
 
     def sign(self, url, checksum):
         if ':' not in checksum:
-            raise SigningFailed("Missing algo prefix in {}".format(checksum))
+            raise SigningFailed(f"Missing algo prefix in {checksum}")
         algo, checksum = checksum.split(':', 1)
         if algo != "sha256":
             # for now, we only handle sha256
-            raise SigningFailed("Unknown checksum algo {}".format(algo))
-        tmpdir = tempfile.mkdtemp(prefix="/tmp/robosignatory-")
+            raise SigningFailed(f"Unknown checksum algo {algo}")
+        tmpdir = tempfile.mkdtemp(prefix="/tmp/robosignatory-")  # noqa: S108
         try:
             self._sign_object(url, checksum, tmpdir)
         finally:
             shutil.rmtree(tmpdir)
 
     def _sign_object(self, url, checksum, tmpdir):
         filepath = urlparse(url).path.lstrip("/")
         local_filepath = os.path.join(tmpdir, os.path.basename(filepath))
 
         log.info("Downloading %s", filepath)
         try:
             self.bucket.download_file(filepath, local_filepath)
         except ClientError as e:
-            raise SigningFailed("Could not download {}: {}".format(filepath, e))
+            raise SigningFailed(f"Could not download {filepath}: {e}") from e
 
         log.info("Checking hash for %s", filepath)
         if utils.get_hash(local_filepath) != checksum:
-            raise SigningFailed("Incorrect SHA256 for {}, not signing".format(filepath))
+            raise SigningFailed(f"Incorrect SHA256 for {filepath}, not signing")
 
         log.info("Signing %s", filepath)
         sig_filepath = self._get_sig_filepath(local_filepath)
         cmdline = self._get_cmdline(local_filepath, checksum)
         log.info('Signing command line: %s', cmdline)
         ret, stdout, stderr = utils.run_command(cmdline)
         if ret != 0:
             raise SigningFailed(
                 'Error signing! Signing output: {}, stdout: {}, stderr: {}'.format(
                     ret, stdout, stderr)
             )
         if not os.path.exists(sig_filepath):
             raise SigningFailed(
-                "Signer did not produce any signature file for {}".format(filepath)
+                f"Signer did not produce any signature file for {filepath}"
             )
         log.debug('Fixing signature file permissions')
         # Sigul writes it as 0600, which makes a lot of sense as a general file
         # mode for it, but this is just a signature file that we want published
         os.chmod(sig_filepath,
                  (stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IROTH))
```

### Comparing `robosignatory-0.6.7/robosignatory/tag.py` & `robosignatory-0.8.0/robosignatory/tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,61 @@
-from __future__ import unicode_literals, absolute_import
-
 import logging
 import re
 
 import koji
 
-import six
-
 import robosignatory.utils as utils
 
 
 log = logging.getLogger("robosignatory.tagconsumer")
 
 KNOWN_TAG_TYPES = ['plain', 'modular']
 
 
-class TagSigner(object):
+class TagSigner:
 
     def __init__(self, config):
         self.config = config
 
         signing_config = self.config['signing']
         self.signer = utils.get_signing_helper(**signing_config)
 
         self.koji_clients = {}
         for instance, instance_info in self.config['koji_instances'].items():
             url = instance_info['url']
-            if six.PY2:
-                url = url.encode("utf-8")
             client = koji.ClientSession(url, instance_info['options'])
 
             if instance_info['options']['authmethod'] == 'ssl':
                 client.ssl_login(instance_info['options']['cert'],
                                  None,
                                  instance_info['options']['serverca'])
             elif instance_info['options']['authmethod'] == 'kerberos':
                 kwargs = {}
                 for opt in ('principal', 'keytab', 'ccache'):
                     if opt in instance_info['options']:
                         value = instance_info['options'][opt]
-                        if six.PY2:
-                            value = value.encode("utf-8")
                         kwargs[opt] = value
-                client.krb_login(**kwargs)
+                client.gssapi_login(**kwargs)
             else:
                 raise Exception('Only SSL and kerberos authmethods supported')
 
             instance_obj = {'client': client,
                             'sidetags': {},
                             'tags': {}}
             if 'mbs_user' in instance_info:
                 instance_obj['mbs_user'] = instance_info['mbs_user']
             for tag in instance_info['tags']:
                 if tag['from'] in instance_obj['tags']:
                     raise Exception('From detected twice: %s' % tag['from'])
-                instance_obj['tags'][tag['from']] = {'to': tag['to'],
-                                                     'key': tag['key'],
-                                                     'keyid': tag['keyid']}
+                instance_obj['tags'][tag['from']] = {
+                    'to': tag['to'],
+                    'key': tag['key'],
+                    'keyid': tag['keyid'],
+                    'file_signing_key': tag.get('file_signing_key'),
+                }
 
                 tag_type = tag.get('type')
                 if tag_type is None:
                     tag_type = 'plain'
                 elif tag_type not in KNOWN_TAG_TYPES:
                     raise Exception('Invalid tag type detected: %s' % tag_type)
                 instance_obj['tags'][tag['from']]['type'] = tag_type
@@ -93,15 +88,15 @@
 
                 # The 'trusted_taggers' option is a list which defines the user
                 # ids from which we want to accept builds tagged into the
                 # '<sidetag>-pending-signing' tag.
                 trusted_taggers = sidetags['trusted_taggers']
                 if (
                     not isinstance(trusted_taggers, list)
-                    or not all(isinstance(x, six.text_type) for x in trusted_taggers)
+                    or not all(isinstance(x, str) for x in trusted_taggers)
                 ):
                     raise TypeError("`trusted_taggers` must be a list of strings, not %r."
                                     % trusted_taggers)
 
                 instance_obj['sidetags'][pattern_filled_in] = {
                     'pattern': sidetags['pattern'],
                     'from_tag_re': from_tag_re,
@@ -122,15 +117,15 @@
         #   u'instance': u'primary',
         #   u'tag': u'epel7-infra',
         #   u'user': u'puiterwijk',
         #   u'version': u'0.9.1',
         #   u'owner': u'sayanchowdhury',
         #   u'release': u'1.el7'}}
 
-        build_nvr = '%(name)s-%(version)s-%(release)s' % msg.body
+        build_nvr = '{name}-{version}-{release}'.format(**msg.body)
         build_id = msg.body['build_id']
         tag = msg.body['tag']
         koji_instance = msg.body['instance']
 
         log.info('Build %s (%s) tagged into %s on %s',
                  build_nvr, build_id, tag, koji_instance)
 
@@ -140,32 +135,32 @@
 
         self.dowork(build_nvr, build_id, tag, koji_instance,
                     skip_tagging=False)
 
     def match_sidetag(self, build_nvr, build_id, tag, koji_instance):
         instance = self.koji_clients[koji_instance]
 
-        for pattern_filled_in, sidetag_matched in instance['sidetags'].items():
+        for sidetag_matched in instance['sidetags'].values():
             from_tag_re = sidetag_matched['from_tag_re']
 
             m = from_tag_re.match(tag)
             if not m:
                 continue
 
             sidetag = m.group('sidetag')
 
             # Verify that the build was tagged into the tag by one of the
             # trusted taggers.
-            for hist_event in sorted(instance['client'].tagHistory(build_id),
+            for hist_event in sorted(instance['client'].queryHistory(build=build_id)['tag_listing'],
                                      key=lambda ev: ev['create_ts'],
                                      reverse=True):
                 # We want to verify the latest matching tagging event only.
                 if (
                     hist_event['active']
-                    and hist_event['tag_name'] == tag
+                    and hist_event['tag.name'] == tag
                 ):
                     if hist_event['creator_name'] in sidetag_matched['trusted_taggers']:
                         # This is how it should be, break out of the loop.
                         break
 
                     log.error("Side tag build not tagged into %s by trusted user (%s)"
                               " but by '%s'!",
@@ -206,16 +201,23 @@
             tag_matched, tag_info, tag_to = self.match_sidetag(build_nvr, build_id, tag,
                                                                koji_instance)
 
         if not tag_matched:
             log.info('Tag not autosigned, skipping')
             return
 
-        log.info('Going to sign %s with %s (%s) and move to %s',
-                 build_nvr, tag_info['key'], tag_info['keyid'], tag_to)
+        if tag_info['file_signing_key']:
+            log.info(
+                'Going to sign %s with %s (%s) and file signing key %s and move to %s',
+                build_nvr, tag_info['key'], tag_info['keyid'], tag_info['file_signing_key'], tag_to)
+        else:
+            log.info(
+                'Going to sign %s with %s (%s) and move to %s',
+                build_nvr, tag_info['key'], tag_info['keyid'], tag_to
+            )
 
         if tag_info['type'] == 'plain':
             self.signwrite_single_build(build_nvr, build_id, tag_info, instance, koji_instance)
         elif tag_info['type'] == 'modular':
             self.signwrite_module(build_nvr, build_id, tag_info, instance, koji_instance)
         else:
             raise NotImplementedError('Tag type %s not implemented' % tag_info['type'])
@@ -235,40 +237,46 @@
         if not buildinfo:
             raise Exception('No build object found?')
         content_koji_tag = buildinfo['extra']['typeinfo']['module']['content_koji_tag']
         log.info('Content tag: %s', content_koji_tag)
         log.info('Signing all module content')
         for build in instance['client'].listTagged(content_koji_tag):
             if build['owner_name'] != instance['mbs_user']:
-                log.error('Build %(build_id)s has owner %(owner_name)s, which is NOT mbs_user!'
-                          % build)
+                log.error(
+                    'Build {build_id} has owner {owner_name}, which is NOT mbs_user!'.format(
+                        **build
+                    )
+                )
                 raise Exception('Modular content tag contains invalid owned build')
             self.signwrite_single_build(build['nvr'], build['build_id'], tag_info, instance,
                                         koji_instance)
 
     def signwrite_single_build(self, build_nvr, build_id, tag_info, instance, koji_instance):
         log.info('Signing and writing build %s', build_nvr)
         rpms = utils.get_rpms(instance['client'],
                               build_nvr=build_nvr,
                               build_id=build_id,
                               sigkey=tag_info['keyid'])
         log.info('RPMs to sign and move: %s',
-                 ['%s (%s, signed: %s)' % (key, rpm['id'], rpm['signed'])
+                 ['{} ({}, signed: {})'.format(key, rpm['id'], rpm['signed'])
                   for key, rpm in rpms.items()])
         if len(rpms) < 1:
             log.info('Build contains no rpms, skipping signing and writing')
 
         if all([rpm['signed'] for rpm in rpms.values()]) or len(rpms) < 1:
             log.debug('All RPMs are already signed')
         else:
             to_sign = [key for key, rpm in rpms.items() if not rpm['signed']]
             log.debug('RPMs needing signing: %s' % to_sign)
-            cmdline = self.signer.build_sign_cmdline(tag_info['key'],
-                                                     to_sign,
-                                                     koji_instance)
+            cmdline = self.signer.build_sign_cmdline(
+                tag_info['key'],
+                to_sign,
+                koji_instance,
+                tag_info.get('file_signing_key'),
+            )
             log.debug('Signing command line: %s' % cmdline)
 
             ret, stdout, stderr = utils.run_command(cmdline)
             if ret != 0:
                 log.error('Error signing! Signing output: %s, stdout: '
                           '%s, stderr: %s', ret, stdout, stderr)
                 raise Exception('Signing failed')
```

### Comparing `robosignatory-0.6.7/robosignatory/utils.py` & `robosignatory-0.8.0/robosignatory/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     rpminfo = {}
     for rpm in rpms:
         info = {'id': rpm['id']}
         if sigkey:
             sigs = koji_client.queryRPMSigs(rpm_id=rpm['id'],
                                             sigkey=sigkey)
             info['signed'] = len(sigs) != 0
-        rpminfo['%s.%s' % (rpm['nvr'], rpm['arch'])] = info
+        rpminfo['{}.{}'.format(rpm['nvr'], rpm['arch'])] = info
     return rpminfo
 
 
 def get_builds_in_tag(koji_client, tag):
     """ Return the list of builds in Koji tag. """
 
     try:
@@ -38,17 +38,20 @@
         # If the tag doesn't exist.. then there are no rpms in that tag.
         return []
 
     return builds
 
 
 def run_command(command):
-    child = subprocess.Popen(command, stdin=subprocess.PIPE,
-                             stdout=subprocess.PIPE,
-                             stderr=subprocess.PIPE)
+    child = subprocess.Popen(
+        command,  # noqa: S603
+        stdin=subprocess.PIPE,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+    )
     stdout, stderr = child.communicate()
     ret = child.wait()
     return ret, stdout, stderr
 
 
 def get_hash(filepath):
     hasher = sha256()
@@ -63,21 +66,19 @@
 
 def get_signing_helper(backend, *args, **kwargs):
     """ Instantiate and return the appropriate signing backend. """
     points = pkg_resources.iter_entry_points('robosignatory.signing.helpers')
     classes = dict([(point.name, point.load()) for point in points])
     log.debug("Found the following installed signing helpers %r" % classes)
     cls = classes[backend]
-    log.debug("Instantiating helper %r from backend key %r" % (cls, backend))
+    log.debug(f"Instantiating helper {cls!r} from backend key {backend!r}")
     return cls(*args, **kwargs)
 
 
-class BaseSigningHelper(object):
-    __metaclass__ = abc.ABCMeta
-
+class BaseSigningHelper(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def build_cmdline(self, *args):
         pass
 
     @abc.abstractmethod
     def build_sign_cmdline(self, *args):
         pass
@@ -86,19 +87,23 @@
     def build_atomic_cmdline(self, *args):
         pass
 
     @abc.abstractmethod
     def build_coreos_cmdline(self, *args):
         pass
 
+    @abc.abstractmethod
+    def build_xml_cmdline(self, *args):
+        pass
+
 
 class EchoHelper(BaseSigningHelper):
     """ A dummy "hello world" helper, used for debugging. """
     def __init__(self, *args, **kwargs):
-        log.info("Constructing EchoHelper(%r, %r)" % (args, kwargs))
+        log.info(f"Constructing EchoHelper({args!r}, {kwargs!r})")
 
     def build_cmdline(self, *args, **kwargs):
         result = ['echo', ' '.join(['build_cmdline:', str(args), str(kwargs)])]
         log.info(result)
         return result
 
     def build_sign_cmdline(self, *args, **kwargs):
@@ -112,50 +117,73 @@
         return result
 
     def build_coreos_cmdline(self, *args, **kwargs):
         result = ['echo', ' '.join(['build_coreos_cmdline:', str(args), str(kwargs)])]
         log.info(result)
         return result
 
+    def build_xml_cmdline(self, *args, **kwargs):
+        result = ['echo', ' '.join(['build_xml_cmdline:', str(args), str(kwargs)])]
+        log.info(result)
+        return result
+
 
 class SigulHelper(BaseSigningHelper):
-    def __init__(self, user, passphrase_file, config_file=None):
+    def __init__(self, user, passphrase_file, config_file=None,
+                 file_signing_key_passphrase_file=None):
         self.user = user
         self.passphrase_file = passphrase_file
         self.config_file = config_file
+        self.file_signing_key_passphrase_file = file_signing_key_passphrase_file
 
     def build_cmdline(self, *args):
         cmdline = ['sigul', '--batch', '--user-name', self.user,
                    '--passphrase-file', self.passphrase_file]
         if self.config_file:
             cmdline.extend(["--config-file", self.config_file])
         cmdline.extend(args)
         return cmdline
 
-    def build_sign_cmdline(self, key, rpms, koji_instance=None):
+    def build_sign_cmdline(self, key, rpms, koji_instance=None,
+                           file_signing_key=None):
         if len(rpms) == 1:
             sigul_cmd = "sign-rpm"
         else:
             sigul_cmd = "sign-rpms"
 
         command = self.build_cmdline(sigul_cmd, '--store-in-koji',
                                      '--koji-only')
         if koji_instance:
             command.extend(['-k', koji_instance])
 
+        if file_signing_key:
+            log.debug('Adding file signing key: %s', file_signing_key)
+            if not self.file_signing_key_passphrase_file:
+                raise Exception("No passphrase file for file signing key configured")
+            command.extend([
+                '--file-signing-key', file_signing_key,
+                '--file-signing-key-passphrase-file',
+                self.file_signing_key_passphrase_file,
+            ])
+
         # TODO: See if this always needs to be set or optional
         # if self.v3:
         command.append('--v3-signature')
 
         command.append(key)
 
         return command + rpms
 
     def build_atomic_cmdline(self, key, checksum, input_file, output_file):
-        command = self.build_cmdline('sign-ostree', key, checksum, input_file,
-                                     '--output', output_file)
+        command = self.build_cmdline('sign-ostree', '--output', output_file,
+                                     '--', key, checksum, input_file)
         return command
 
     def build_coreos_cmdline(self, key, input_file, output_file):
-        command = self.build_cmdline('sign-data', key, input_file,
-                                     '--output', output_file)
+        command = self.build_cmdline('sign-data', '--output', output_file, '--',
+                                     key, input_file)
+        return command
+
+    def build_xml_cmdline(self, key, input_file, output_file):
+        command = self.build_cmdline('sign-data', '--output', output_file, '--',
+                                     key, input_file)
         return command
```

### Comparing `robosignatory-0.6.7/robosignatory/work.py` & `robosignatory-0.8.0/robosignatory/work.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if not os.path.exists(commitpath):
         log.info('Commit file at %s not found. Skipping' % commitpath)
         return
     if os.path.exists(commitmetapath):
         log.info('Commitmeta file at %s found. Skipping' % commitmetapath)
         return
 
-    log.info('All checks passed, signing %s with %s' % (commitid, key))
+    log.info(f'All checks passed, signing {commitid} with {key}')
     cmdline = signer.build_atomic_cmdline(key,
                                           commitid,
                                           commitpath,
                                           commitmetapath)
     log.info('Signing command line: %s' % cmdline)
 
     ret, stdout, stderr = utils.run_command(cmdline)
@@ -39,29 +39,28 @@
     os.chmod(commitmetapath, (stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP
                               | stat.S_IROTH))
 
     log.info('Commit was succesfully signed, writing ref %s' % ref)
 
     refpath = os.path.join(directory, 'refs', 'heads', ref)
     if os.path.exists(refpath):
-        with open(refpath, 'r') as f:
-            log.info('Previous commit for %s: %s'
-                     % (ref, f.read().replace('\n', '')))
+        with open(refpath) as f:
+            log.info('Previous commit for {}: {}'.format(ref, f.read().replace('\n', '')))
 
     dirname_refpath = os.path.dirname(refpath)
     if doref and not os.path.exists(dirname_refpath):
         log.info("Creating the directories for the refpath")
         # Set the umask to be more permissive so directories get group write
         # permissions. See https://pagure.io/releng/issue/8811#comment-629051
         oldumask = os.umask(0o0002)
         try:
             os.makedirs(dirname_refpath)
         finally:
             os.umask(oldumask)
 
     if doref:
-        log.info('Writing %s to %s' % (commitid, refpath))
+        log.info(f'Writing {commitid} to {refpath}')
 
         with open(refpath, 'w') as f:
             f.write(commitid + '\n')
 
     log.info('Done')
```

### Comparing `robosignatory-0.6.7/robosignatory.egg-info/SOURCES.txt` & `robosignatory-0.8.0/robosignatory.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 robosignatory.toml
 setup.cfg
 setup.py
 tox.ini
 robosignatory/__init__.py
 robosignatory/atomic.py
 robosignatory/cli.py
 robosignatory/consumer.py
 robosignatory/coreos.py
 robosignatory/tag.py
 robosignatory/utils.py
 robosignatory/work.py
+robosignatory/xml.py
 robosignatory.egg-info/PKG-INFO
 robosignatory.egg-info/SOURCES.txt
 robosignatory.egg-info/dependency_links.txt
 robosignatory.egg-info/entry_points.txt
 robosignatory.egg-info/requires.txt
 robosignatory.egg-info/top_level.txt
 tests/__init__.py
 tests/test_atomic.py
 tests/test_consumers.py
 tests/test_coreos.py
 tests/test_tag.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_xml.py
```

### Comparing `robosignatory-0.6.7/robosignatory.toml` & `robosignatory-0.8.0/robosignatory.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 [[bindings]]
 queue = "robosignatory"
 exchange = "amq.topic"
 routing_keys = [
     "org.fedoraproject.*.pungi.compose.ostree",
     "org.fedoraproject.*.coreos.build.request.artifacts-sign",
     "org.fedoraproject.*.coreos.build.request.ostree-sign",
+    "org.fedoraproject.*.robosignatory.xml-sign",
     "org.fedoraproject.*.buildsys.tag",
 ]
 
 [[bindings]]
 queue = "robosignatory"
 exchange = "zmq.topic"
 routing_keys = [
@@ -81,14 +82,15 @@
     [consumer_config.signing]
     # This should be the name of an entrypoint plugin that provides
     # SigningHelper functionality.
     backend = "sigul"
     # These are arguments to the __init__ method of that helper.
     user = "robosignatory"
     passphrase_file = "robosignatory.pass"
+    file_signing_passphrase_file = "robosignatory-file-signing.pass"
     config_file = "/etc/sigul/client.conf"
 
     [consumer_config.koji_instances]
     # The keys here need to be the same in the sigul bridge
         [consumer_config.koji_instances.primary]
         url = 'http://koji.fedoraproject.org/kojihub'
         mbs_user = 'mbs/mbs.example.com'
@@ -99,26 +101,28 @@
             cert = 'robosignatory.cert'
             serverca = 'servcer-ca.cert'
 
             [[consumer_config.koji_instances.primary.tags]]
             from = 'rawhide-signcandidate'
             to = 'rawhide'
             key = 'fedora26'
+            file_signing_key = 'fedora-file-signing'
             keyid = 'xxxxxxxx'
 
                 [consumer_config.koji_instances.primary.tags.sidetags]
                 pattern = '<to>-build-side-<seq_id>'
                 from = '<sidetag>-pending-signing'
                 to = '<sidetag>-testing'
                 trusted_taggers = ['bodhi']
 
             [[consumer_config.koji_instances.primary.tags]]
             from = 'rawhide-modular-signcandidate'
             to = 'rawhide-modular'
             key = 'fedora26'
+            file_signing_key = 'fedora-file-signing'
             keyid = 'xxxxxxxx'
             type = 'modular'
 
     [consumer_config.ostree_refs]
         [consumer_config.ostree_refs."fedora-atomic/25/x86_64/docker-host"]
         directory = '/mnt/koji/compose/atomic/25/'
         key = 'fedora-25'
```

### Comparing `robosignatory-0.6.7/setup.py` & `robosignatory-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,26 +26,26 @@
             msg = 'pytest failed!'
             self.announce(msg, distutils.log.ERROR)
             raise distutils.errors.DistutilsError(msg)
 
 
 setup(
     name='robosignatory',
-    version='0.6.7',
+    version='0.8.0',
     description='fedora-messaging consumer that automatically signs artifacts',
     author='Patrick Uiterwijk',
     author_email='puiterwijk@redhat.com',
     url='https://pagure.io/robosignatory/',
     license='gplv2+',
     install_requires=[
         "fedora_messaging",
         "psutil",
         "boto3",
-        "six",
         "click",
+        "setuptools",
         # Don't depend on koji here: https://bugzilla.redhat.com/show_bug.cgi?id=1537197
         #"koji",
     ],
     tests_require=[
         "pytest",
         "mock",
     ],
```

### Comparing `robosignatory-0.6.7/tests/test_atomic.py` & `robosignatory-0.8.0/tests/test_atomic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import unittest
 import copy
+import unittest
+from unittest import mock
 
-import mock
 from fedora_messaging.api import Message
 
 from robosignatory.atomic import AtomicSigner
 
 
 TEST_CONFIG = {
     "signing": {
@@ -67,8 +67,7 @@
 
     @mock.patch('robosignatory.work.process_atomic')
     def test_no_commitid(self, process_atomic):
         msg = Message(topic=IOT_MESSAGE.topic, body=copy.deepcopy(IOT_MESSAGE.body))
         msg.body["commitid"] = None
         self.consumer.consume(msg)
         process_atomic.assert_not_called()
-
```

### Comparing `robosignatory-0.6.7/tests/test_consumers.py` & `robosignatory-0.8.0/tests/test_consumers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
+from unittest import mock
 
 from fedora_messaging.api import Message
 from fedora_messaging.exceptions import Nack
-import mock
 
 from robosignatory.consumer import Consumer
 
 
 TEST_CONFIG = {
     "signing": {
         "backend": "echo",
@@ -18,18 +18,21 @@
         "key": "testing",
         "aws": {
             "access_key": "testing",
             "access_secret": "testing",
             "region": "us-east-1",
         }
     },
+    "xml": {
+        "key": "testing",
+    }
 }
 
 
-@mock.patch(
+@mock.patch.dict(
     "robosignatory.consumer.fedora_messaging.config.conf",
     {"consumer_config": TEST_CONFIG}
 )
 class TestConsumers(unittest.TestCase):
 
     @mock.patch('robosignatory.consumer.TagSigner')
     def test_message_tag(self, Handler):
```

### Comparing `robosignatory-0.6.7/tests/test_coreos.py` & `robosignatory-0.8.0/tests/test_coreos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import unittest
 import copy
 from collections import namedtuple
+from unittest import mock
 
-import mock
 from botocore.exceptions import ClientError
 from fedora_messaging.api import Message
 from fedora_messaging.testing import mock_sends
 
 from robosignatory.coreos import CoreOSSigner
 
 
@@ -48,22 +48,25 @@
         "commit_object": "s3://host/some/path/test1",
         "checksum": "sha256:e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
     }
 )
 
 S3Object = namedtuple("S3Object", "size")
 
+
 def fake_download(source, local):
     open(local, "w").close()
 
+
 def fake_download_and_artifact_sign(source, local):
     fake_download(source, local)
     # Also create the sig file for testing
     open(local + ".sig", "w").close()
 
+
 def fake_download_and_ostree_sign(source, local):
     fake_download(source, local)
     # Also create the sig file for testing
     open(os.path.dirname(local) + "/ostree-commitmeta-object", "w").close()
 
 
 class TestCoreOS(unittest.TestCase):
@@ -108,24 +111,29 @@
         with mock_sends(expected_response):
             self.consumer.consume(OSTREE_MESSAGE)
 
         self.consumer.bucket.download_file.assert_called()
         assert self.consumer.bucket.download_file.call_args_list[0][0][0] == "some/path/test1"
         run_command.assert_called()
         self.consumer.bucket.upload_file.assert_called()
-        assert self.consumer.bucket.upload_file.call_args_list[0][0][1] == "some/path/ostree-commitmeta-object"
+        assert (
+            self.consumer.bucket.upload_file.call_args_list[0][0][1]
+            == "some/path/ostree-commitmeta-object"
+        )
 
     @mock.patch('robosignatory.coreos.utils.run_command')
     def test_wrong_checksum(self, run_command):
         new_body = copy.deepcopy(ARTIFACTS_MESSAGE.body)
         new_body["artifacts"][0]["checksum"] = "sha256:wrong-checksum"
         msg = Message(topic=ARTIFACTS_MESSAGE.topic, body=new_body)
         self.consumer.bucket.download_file.side_effect = fake_download
-        expected_response = self._get_response_message(msg, failed=True,
-            failure_msg='Incorrect SHA256 for some/path/test1, not signing')
+        expected_response = self._get_response_message(
+            msg, failed=True,
+            failure_msg='Incorrect SHA256 for some/path/test1, not signing'
+        )
 
         with mock_sends(expected_response):
             self.consumer.consume(msg)
 
         self.consumer.bucket.download_file.assert_called()
         run_command.assert_not_called()
         self.consumer.bucket.upload_file.assert_not_called()
@@ -178,15 +186,15 @@
         consumer = CoreOSSigner(TEST_CONFIG)
         msg = Message(topic=ARTIFACTS_MESSAGE.topic, body=ARTIFACTS_MESSAGE.body)
         self.assertEqual(consumer.get_key(msg), "testing")
 
     def test_key_parse_autodetect(self):
         # Verify that when no key is provided via the config the key
         # is autodetected.
-        # 
+        #
         # Grab the config and remove the hardcoded key to enable auto detection
         config = copy.deepcopy(TEST_CONFIG)
         del config["coreos"]["key"]
         consumer = CoreOSSigner(config)
         # Grab the message body and set the build_id to a version number
         new_body = copy.deepcopy(ARTIFACTS_MESSAGE.body)
         new_body["build_id"] = "32.20200601.2.1"
```

### Comparing `robosignatory-0.6.7/tests/test_tag.py` & `robosignatory-0.8.0/tests/test_tag.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from __future__ import unicode_literals
-
 import copy
 import logging
-import mock
+from unittest import mock
 
-import six
 from fedora_messaging.api import Message
 from pkg_resources import parse_version
 from pytest import raises, mark, __version__ as pytest_version
 
 from robosignatory.tag import TagSigner
 
 try:
     import _pytest.logging
 except ImportError:
     pass
 else:
-    if not hasattr(_pytest.logging.LogCaptureFixture, 'messages'):  # noqa
+    if not hasattr(_pytest.logging.LogCaptureFixture, 'messages'):
         # monkey-patch missing messages property
         class MyLogCaptureFixture(_pytest.logging.LogCaptureFixture):
             @property
             def messages(self):
                 return [r.getMessage() for r in self.records]
 
 
@@ -64,15 +61,38 @@
                 },
                 {
                     'from': 'f30-modular-signing-pending',
                     'to': 'f30-modular-updates-testing-pending',
                     'key': 'fedora-30',
                     'keyid': 'OU812I81B4U',
                     'type': 'modular',
-                }
+                },
+                {
+                    'from': 'f31-pending-fsk',
+                    'to': 'f31',
+                    'key': 'fedora-31',
+                    'keyid': 'deadbeef',
+                    'file_signing_key': 'file-sign-key',
+                },
+                {
+                    'from': 'f30-signing-pending-fsk',
+                    'to': 'f30-updates-testing-pending',
+                    'key': 'fedora-30',
+                    'keyid': 'OU812I81B4U',
+                    'file_signing_key': 'file-sign-key',
+                    'type': 'plain',
+                },
+                {
+                    'from': 'f30-modular-signing-pending-fsk',
+                    'to': 'f30-modular-updates-testing-pending',
+                    'key': 'fedora-30',
+                    'keyid': 'OU812I81B4U',
+                    'file_signing_key': 'file-sign-key',
+                    'type': 'modular',
+                },
             ],
         },
     },
     'ostree_refs': {},
     'coreos': {
         'bucket': 'testing',
         'key': 'testing',
@@ -138,28 +158,28 @@
     def get_signing_helper(self, **signing_config):
         return mock.MagicMock(signing_config=signing_config)
 
     def run_command(self, cmdline):
         return 0, "", ""
 
 
-class DummyContext(object):
+class DummyContext:
 
     def __enter__(self):
         pass
 
     def __exit__(self, *args):
         pass
 
 
-@mock.patch(
+@mock.patch.dict(
     'robosignatory.consumer.fedora_messaging.config.conf',
     {'consumer_config': TEST_CONFIG}
 )
-class TestTagSigner(object):
+class TestTagSigner:
     """Test the Koji tag signer class"""
 
     test_msg = {
         'topic': 'org.fedoraproject.prod.buildsys.tag',
         'body': {
             'name': 'foo', 'version': '1', 'release': '1.fc31',
             'build_id': 1, 'tag': 'f31-pending',
@@ -189,15 +209,15 @@
 
     def test_init(self):
         """Test that the tag signer can be created"""
         # The signer gets created in .setUp().
 
         assert self.instance_obj['mbs_user'] == 'mbs_user'
 
-        self.koji_client.krb_login.assert_called_once_with(
+        self.koji_client.gssapi_login.assert_called_once_with(
             principal='test@EXAMPLE.COM')
         self.koji_client.ssl_login.assert_not_called()
 
     def test_init_with_ssl(self):
         """Test that a signer using SSL authentication can be created"""
         # We overwrite the signer here to inject non-standard configuration.
         test_config = copy.deepcopy(TEST_CONFIG)
@@ -205,15 +225,15 @@
             'authmethod': 'ssl', 'cert': 'cert', 'serverca': 'serverca',
         }
         with mock.patch('robosignatory.tag.koji.ClientSession'):
             self.tag_signer = TagSigner(test_config)
 
         self.koji_client.ssl_login.assert_called_once_with(
             'cert', None, 'serverca')
-        self.koji_client.krb_login.assert_not_called()
+        self.koji_client.gssapi_login.assert_not_called()
 
     def test_init_with_unknown_authmethod(self):
         """Test that unknown authmethods are caught"""
         # We overwrite the signer here to inject non-standard configuration.
         test_config = copy.deepcopy(TEST_CONFIG)
         test_config['koji_instances']['test']['options'] = {
             'authmethod': 'unknown'
@@ -222,15 +242,15 @@
             'robosignatory.tag.koji.ClientSession'
         ) as koji_client, raises(
             Exception, match='Only SSL and kerberos authmethods supported'
         ):
             self.tag_signer = TagSigner(test_config)
 
         koji_client.ssl_login.assert_not_called()
-        koji_client.krb_login.assert_not_called()
+        koji_client.gssapi_login.assert_not_called()
 
     def test_init_with_duplicate_from_tag(self):
         """Test behavior with duplicate from tag"""
         # We overwrite the signer here to inject non-standard configuration.
         test_config = copy.deepcopy(TEST_CONFIG)
         tags = test_config['koji_instances']['test']['tags']
         tags.insert(1, tags[0])
@@ -257,37 +277,39 @@
 
     # Test well-formed messages.
 
     def _prep_sidetag_test(self, sidetag_pending, error):
         tags_key = self.test_msg['body']['tag']  # normal tag where we find robosig configuration
         tag_conf = self.instance_obj['tags'][tags_key]
 
-        for sidetag_conf in self.instance_obj['sidetags'].values():
+        for sidetag_conf in list(self.instance_obj['sidetags'].values()):
             if sidetag_conf['tags_key'] == tags_key:
                 tag_conf['sidetags'] = sidetag_conf
                 break
         else:
             raise RuntimeError("Can't find sidetag configuration for {}".format(
-                tag_conf['from']))
+                sidetag_conf))
 
         if error == 'untrusted-tagger':
             tagger = 'hamburglar'
         else:
             tagger = 'bodhi'
 
         if error == 'missing-from-history':
-            tag_history = []
+            tag_history = {'tag_listing': []}
         else:
-            tag_history = [
-                {'active': True,
-                 'create_ts': 1554076800,
-                 'creator_name': tagger,
-                 'tag_name': sidetag_pending},
-            ]
-        self.koji_client.tagHistory.return_value = tag_history
+            tag_history = {
+                'tag_listing': [
+                    {'active': True,
+                     'create_ts': 1554076800,
+                     'creator_name': tagger,
+                     'tag.name': sidetag_pending},
+                ]
+            }
+        self.koji_client.queryHistory.return_value = tag_history
 
         return tag_conf, tagger
 
     def _get_expected_messages_and_exceptions(self, sidetag_pending, error,
                                               build_owner, tag_conf, tagger):
         body = self.test_msg['body']
         instance = body['instance']
@@ -298,15 +320,15 @@
         expected_log_msgs = [
             "Build {} ({}) tagged into {} on {}".format(
                 build_nvr, build_id, from_tag, instance),
         ]
 
         if error == 'non-mbs-owner':
             expected_log_msgs.append(
-                "Build {} has owner {}, which is NOT mbs_user!".format(build_id, build_owner))
+                f"Build {build_id} has owner {build_owner}, which is NOT mbs_user!")
             expected_exc_ctx = raises(Exception,
                                       match="Modular content tag contains invalid owned build")
         elif error == 'untrusted-tagger':
             expected_log_msgs.append(
                 "Side tag build not tagged into {} by trusted user ({}) but by '{}'!".format(
                     sidetag_pending, ", ".join(tag_conf['sidetags']['trusted_taggers']), tagger
                 )
@@ -384,14 +406,70 @@
         if not error:
             self.koji_client.tagBuild.assert_called_once_with(to_tag, build_id,
                                                               False, from_tag)
         else:
             self.koji_client.tagBuild.assert_not_called()
 
     @requires_caplog
+    @mock.patch('robosignatory.tag.utils', new_callable=MockUtils())
+    @mark.parametrize(
+        'type_',
+        (('plain'),
+         ('modular'),))
+    def test_file_signing_key(self, utils, caplog, type_):
+        """Test with file signing key"""
+        caplog.set_level(logging.DEBUG)
+
+        body = self.test_msg['body']
+        build_nvr = '{name}-{version}-{release}'.format(**body)
+        body['tag'] = body['tag'] + '-fsk'
+        from_tag = body['tag']
+        build_id = body['build_id']
+        tag_conf = self.instance_obj['tags'][from_tag]
+        to_tag = tag_conf['to']
+        build_owner = None
+
+        if type_ == 'modular':
+            body['tag'] = from_tag = 'f30-modular-signing-pending-fsk'
+            to_tag = 'f30-modular-updates-testing-pending'
+            build_owner = TEST_CONFIG['koji_instances']['test']['mbs_user']
+
+            self.koji_client.listTagged.return_value = [
+                {'owner_name': build_owner, 'nvr': build_nvr, 'build_id': build_id}
+            ]
+            expected_log_msgs = [
+                'Packages correctly signed, moving to f30-modular-updates-testing-pending',
+                'Signing command line: [\'echo\', "build_sign_cmdline: (\'fedora-30\', '
+                '[\'foo-1-1.fc31.x64_64\', \'foo-libs-1-1.fc31.x64_64\'], \'test\', '
+                '\'file-sign-key\') {}"]',
+                'Going to sign foo-1-1.fc31 with fedora-30 (OU812I81B4U) and file signing '
+                'key file-sign-key and move to f30-modular-updates-testing-pending',
+            ]
+        else:
+            expected_log_msgs = [
+                'Signing command line: [\'echo\', "build_sign_cmdline: (\'fedora-31\', '
+                '[\'foo-1-1.fc31.x64_64\', \'foo-libs-1-1.fc31.x64_64\'], \'test\', '
+                '\'file-sign-key\') {}"]',
+                'Going to sign foo-1-1.fc31 with fedora-31 (deadbeef) and file signing key '
+                'file-sign-key and move to f31',
+            ]
+
+        msg = Message(**self.test_msg)
+        self.tag_signer.consume(msg)
+
+        # Equivalent to caplog.messages but compatible with pytest < 3.7
+        logged_messages = [record.getMessage() for record in caplog.records]
+
+        for msg in expected_log_msgs:
+            assert msg in logged_messages
+
+        self.koji_client.tagBuild.assert_called_once_with(to_tag, build_id,
+                                                          False, from_tag)
+
+    @requires_caplog
     def test_plain_build_message_with_unconfigured_tag(self, caplog):
         """Test the behavior with an unconfigured tag"""
         caplog.set_level(logging.DEBUG)
 
         self.test_msg['body']['tag'] = 'unconfigured'
         msg = Message(**self.test_msg)
         self.tag_signer.consume(msg)
@@ -409,22 +487,7 @@
     def test_unknown_koji_instance(self, log):
         """Test an unknown Koji instance in the message"""
         self.test_msg['body']['instance'] = 'unknown'
         msg = Message(**self.test_msg)
         self.tag_signer.consume(msg)
 
         log.info.assert_called_with('Koji instance not known, skipping')
-
-    @mark.skipif(not six.PY2, reason="only relevant on Python 2")
-    def test_py2_koji_client_args(self):
-        assert self._koji_ClientSession.call_count == 1
-        assert not isinstance(self._koji_ClientSession.call_args_list[0][0][0], unicode)
-        for kwarg, value in self._koji_ClientSession.call_args_list[0][1].items():
-            assert not isinstance(value, unicode)
-
-    @mark.skipif(not six.PY2, reason="only relevant on Python 2")
-    def test_py2_krb_login_args(self):
-        assert self.instance_obj["client"].krb_login.call_count == 1
-        assert not isinstance(
-            self.instance_obj["client"].krb_login.call_args_list[0][1]["principal"],
-            unicode
-        )
```

### Comparing `robosignatory-0.6.7/tests/test_utils.py` & `robosignatory-0.8.0/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,37 @@
     def test_get_sigul_helper(self):
         helper = robosignatory.utils.get_signing_helper(
             backend='sigul',
             user='ralph',
             passphrase_file='/tmp/wide-open.txt',
         )
         assert type(helper) == robosignatory.utils.SigulHelper
+        assert helper.file_signing_key_passphrase_file is None
+
+    def test_get_sigul_helper_with_fsk(self):
+        helper = robosignatory.utils.get_signing_helper(
+            backend='sigul',
+            user='ralph',
+            passphrase_file='/tmp/wide-open.txt',
+            file_signing_key_passphrase_file='/tmp/wide-closed.txt',
+        )
+        assert type(helper) == robosignatory.utils.SigulHelper
+        assert helper.file_signing_key_passphrase_file == '/tmp/wide-closed.txt'
 
     def test_simple_echo_helper(self):
         helper = robosignatory.utils.get_signing_helper(
             backend='echo',
             user='ralph',
             passphrase_file='/tmp/wide-open.txt',
         )
         cmdline = helper.build_cmdline('wat')
         assert cmdline == ["echo", "build_cmdline: ('wat',) {}"]
+
+    def test_simple_echo_helper_with_fsk(self):
+        helper = robosignatory.utils.get_signing_helper(
+            backend='echo',
+            user='ralph',
+            passphrase_file='/tmp/wide-open.txt',
+            file_signing_key_passphrase_file='/tmp/wide-closed.txt',
+        )
+        cmdline = helper.build_cmdline('wat')
+        assert cmdline == ["echo", "build_cmdline: ('wat',) {}"]
```

