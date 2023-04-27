# Comparing `tmp/SCAutolib-1.0.17.tar.gz` & `tmp/SCAutolib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SCAutolib-1.0.17.tar", last modified: Thu Apr 13 08:04:40 2023, max compression
+gzip compressed data, was "SCAutolib-1.1.0.tar", last modified: Thu Apr 27 15:26:04 2023, max compression
```

## Comparing `SCAutolib-1.0.17.tar` & `SCAutolib-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.852830 SCAutolib-1.0.17/SCAutolib/
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/SCAutolib/models/
--rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/CA.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/authselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/card.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/SCAutolib/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/ca.cnf
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/softhsm2.conf
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/sssd.conf
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/user.cnf
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/virt_cacard.service
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/templates/virtcacard.cil
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/SCAutolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/SCAutolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 08:04:40.000000 SCAutolib-1.0.17/SCAutolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:04:40.856830 SCAutolib-1.0.17/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_openssl_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_sssd_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-13 08:04:31.000000 SCAutolib-1.0.17/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:26:04.046595 SCAutolib-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-27 15:26:04.046595 SCAutolib-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:26:04.038595 SCAutolib-1.1.0/SCAutolib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18554 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:26:04.042595 SCAutolib-1.1.0/SCAutolib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/CA.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/authselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12192 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:26:04.042595 SCAutolib-1.1.0/SCAutolib/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/templates/ca.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/templates/gnome_disable_welcome
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/templates/softhsm2.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/templates/sssd.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/templates/user.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/templates/virt_cacard.service
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/templates/virtcacard.cil
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/SCAutolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:26:04.042595 SCAutolib-1.1.0/SCAutolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-27 15:26:04.000000 SCAutolib-1.1.0/SCAutolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-27 15:26:04.000000 SCAutolib-1.1.0/SCAutolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:26:04.000000 SCAutolib-1.1.0/SCAutolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 15:26:04.000000 SCAutolib-1.1.0/SCAutolib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 15:26:04.000000 SCAutolib-1.1.0/SCAutolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 15:26:04.000000 SCAutolib-1.1.0/SCAutolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:26:04.046595 SCAutolib-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:26:04.046595 SCAutolib-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_openssl_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_sssd_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-27 15:25:41.000000 SCAutolib-1.1.0/tox.ini
```

### Comparing `SCAutolib-1.0.17/LICENSE` & `SCAutolib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/PKG-INFO` & `SCAutolib-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: SCAutolib
-Version: 1.0.17
+Version: 1.1.0
 Summary: Python library for automation tests of smart cards using virtualization.
 Home-page: https://github.com/redhat-qe-security/SCAutolib
 Author: Pavel Yadlouski
 Author-email: pyadlous@redhat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: graphical
 License-File: LICENSE
 
 # Smart Card Automation library (SCAutolib)
 Test automation library for Smart Cards.
 
 > ⚠️ This library is in development phase. There is nothing 100% stable.
```

### Comparing `SCAutolib-1.0.17/README.md` & `SCAutolib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/__init__.py` & `SCAutolib-1.1.0/SCAutolib/__init__.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/cli_commands.py` & `SCAutolib-1.1.0/SCAutolib/cli_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,23 +58,33 @@
 
 @click.command()
 @click.option("--gdm", "-g",
               required=False,
               default=False,
               is_flag=True,
               help="Install GDM package")
+@click.option("--graphical",
+              required=False,
+              default=False,
+              is_flag=True,
+              help="Install dependencies for GUI testing module")
 @click.option("--install-missing", "-i",
               required=False,
               default=False,
               is_flag=True,
               help="Install missing packages")
 @click.pass_context
-def prepare(ctx, gdm, install_missing):
+def prepare(ctx, gdm, install_missing, graphical):
     """Configure entire system for smart cards based on the config file."""
-    ctx.obj["CONTROLLER"].prepare(ctx.obj["FORCE"], gdm, install_missing)
+    ctx.obj["CONTROLLER"].prepare(
+        ctx.obj["FORCE"],
+        gdm,
+        install_missing,
+        graphical
+    )
     exit(ReturnCode.SUCCESS.value)
 
 
 @click.command()
 @click.argument("name",
                 required=True,
                 default=None)
```

### Comparing `SCAutolib-1.0.17/SCAutolib/controller.py` & `SCAutolib-1.1.0/SCAutolib/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from pathlib import Path
 from schema import Schema, Use
 from shutil import rmtree
 from typing import Union
 
 from SCAutolib import exceptions, schema_cas, schema_user
 from SCAutolib import (logger, run, LIB_DIR, LIB_BACKUP, LIB_DUMP,
-                       LIB_DUMP_USERS, LIB_DUMP_CAS, LIB_DUMP_CARDS)
+                       LIB_DUMP_USERS, LIB_DUMP_CAS, LIB_DUMP_CARDS,
+                       TEMPLATES_DIR)
 from SCAutolib.models import CA, file, user, card, authselect as auth
 from SCAutolib.models.file import File
 from SCAutolib.utils import (OSVersion, _check_selinux, _gen_private_key,
                              _get_os_version, _install_packages,
                              _check_packages, dump_to_json, local_ca_factory)
 
 
@@ -18,14 +19,16 @@
     authselect: auth.Authselect = auth.Authselect()
     sssd_conf: file.SSSDConf = file.SSSDConf()
     lib_conf: dict = None
     _lib_conf_path: Path = None
     local_ca: CA.LocalCA = None
     ipa_ca: CA.IPAServerCA = None
     users: [user.User] = None
+    dconf_file = File(filepath='/etc/dconf/db/local.d/gnome_disable_welcome',
+                      template=Path(TEMPLATES_DIR, 'gnome_disable_welcome'))
 
     @property
     def conf_path(self):
         return self._lib_conf_path
 
     def __init__(self, config: Union[Path, str], params: {} = None):
         """
@@ -58,35 +61,36 @@
                     "Data are not loaded correctly.")
         self.lib_conf = self._validate_configuration(tmp_conf, params)
         self.users = []
         for d in (LIB_DIR, LIB_BACKUP, LIB_DUMP, LIB_DUMP_USERS, LIB_DUMP_CAS,
                   LIB_DUMP_CARDS):
             d.mkdir(exist_ok=True)
 
-    def prepare(self, force: bool, gdm: bool, install_missing: bool):
+    def prepare(self, force: bool, gdm: bool, install_missing: bool,
+                graphical: bool):
         """
         Method for setting up whole system based on configuration file and
         CLI commands
         """
-        self.setup_system(install_missing, gdm)
+        self.setup_system(install_missing, gdm, graphical)
 
         # In this method not having section for local CA and/or for IPA CA is OK
         try:
             self.setup_local_ca(force=force)
         except exceptions.SCAutolibWrongConfig as e:
             logger.info(e)
         try:
             self.setup_ipa_client(force=force)
         except exceptions.SCAutolibWrongConfig as e:
             logger.info(e)
         for usr in self.lib_conf["users"]:
             u = self.setup_user(usr, force=force)
             self.enroll_card(u)
 
-    def setup_system(self, install_missing: bool, gdm: bool):
+    def setup_system(self, install_missing: bool, gdm: bool, graphical: bool):
         """
         Do general system setup meaning package installation based on
         specifications in the configuration file, SSSD configuration,
         configurations for virtual smart cards, etc.
 
         :param install_missing: If True, all missing packages would be
             installed
@@ -99,14 +103,18 @@
                   LIB_DUMP_CARDS):
             d.mkdir(exist_ok=True)
 
         packages = ["opensc", "httpd", "sssd", "sssd-tools", "gnutls-utils"]
         if gdm:
             packages.append("gdm")
 
+        if graphical:
+            # ffmpeg-free is in EPEL repo
+            packages += ["tesseract", "ffmpeg-free"]
+
         # Prepare for virtual cards
         if "virtual" in [u["card_type"] for u in self.lib_conf["users"]]:
             packages += ["pcsc-lite-ccid", "pcsc-lite", "virt_cacard",
                          "vpcd", "softhsm"]
             run("dnf -y copr enable jjelen/vsmartcard")
 
         # Add IPA packages if needed
@@ -119,14 +127,24 @@
             _install_packages(missing)
         elif missing:
             msg = "Can't continue. Some packages are missing: " \
                   f"{', '.join(missing)}"
             logger.critical(msg)
             raise exceptions.SCAutolibException(msg)
 
+        if graphical:
+            run(['dnf', 'groupinstall', 'Server with GUI', '-y'])
+            # disable subsription message
+            run(['systemctl', '--global', 'mask',
+                 'org.gnome.SettingsDaemon.Subscription.target'])
+            # disable welcome message
+            self.dconf_file.create()
+            self.dconf_file.save()
+            run('dconf update')
+
         run(['dnf', 'groupinstall', "Smart Card Support", '-y'])
         logger.debug("Smart Card Support group in installed.")
 
         self.sssd_conf.create()
         self.sssd_conf.save()
         self._general_steps_for_virtual_sc()
```

### Comparing `SCAutolib-1.0.17/SCAutolib/exceptions.py` & `SCAutolib-1.1.0/SCAutolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/models/CA.py` & `SCAutolib-1.1.0/SCAutolib/models/CA.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/models/authselect.py` & `SCAutolib-1.1.0/SCAutolib/models/authselect.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/models/card.py` & `SCAutolib-1.1.0/SCAutolib/models/card.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/models/file.py` & `SCAutolib-1.1.0/SCAutolib/models/file.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/models/user.py` & `SCAutolib-1.1.0/SCAutolib/models/user.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/templates/ca.cnf` & `SCAutolib-1.1.0/SCAutolib/templates/ca.cnf`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib/utils.py` & `SCAutolib-1.1.0/SCAutolib/utils.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/SCAutolib.egg-info/PKG-INFO` & `SCAutolib-1.1.0/SCAutolib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: SCAutolib
-Version: 1.0.17
+Version: 1.1.0
 Summary: Python library for automation tests of smart cards using virtualization.
 Home-page: https://github.com/redhat-qe-security/SCAutolib
 Author: Pavel Yadlouski
 Author-email: pyadlous@redhat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: graphical
 License-File: LICENSE
 
 # Smart Card Automation library (SCAutolib)
 Test automation library for Smart Cards.
 
 > ⚠️ This library is in development phase. There is nothing 100% stable.
```

### Comparing `SCAutolib-1.0.17/SCAutolib.egg-info/SOURCES.txt` & `SCAutolib-1.1.0/SCAutolib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 SCAutolib.egg-info/requires.txt
 SCAutolib.egg-info/top_level.txt
 SCAutolib/models/CA.py
 SCAutolib/models/__init__.py
 SCAutolib/models/authselect.py
 SCAutolib/models/card.py
 SCAutolib/models/file.py
+SCAutolib/models/gui.py
+SCAutolib/models/log.py
 SCAutolib/models/user.py
 SCAutolib/templates/ca.cnf
+SCAutolib/templates/gnome_disable_welcome
 SCAutolib/templates/softhsm2.conf
 SCAutolib/templates/sssd.conf
 SCAutolib/templates/user.cnf
 SCAutolib/templates/virt_cacard.service
 SCAutolib/templates/virtcacard.cil
 test/test_ca.py
 test/test_card.py
```

### Comparing `SCAutolib-1.0.17/setup.py` & `SCAutolib-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,17 +10,26 @@
 
 with requirements.open() as f:
     reqs = f.readlines()
 
 with readme.open() as f:
     long_description = f.read()
 
+graphical_reqs = [
+    'python-uinput',
+    'opencv-python',
+    'pandas',
+    'numpy',
+    'pytesseract',
+    'keyboard',
+]
+
 setup(
     name="SCAutolib",
-    version="1.0.17",
+    version="1.1.0",
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/redhat-qe-security/SCAutolib",
     author="Pavel Yadlouski",
     author_email="pyadlous@redhat.com",
     classifiers=[
@@ -32,12 +41,16 @@
         'Operating System :: Unix',
         'Topic :: Software Development :: Testing',
         'Topic :: Software Development :: Testing :: Acceptance',
     ],
     packages=find_packages(),
     python_requires='>=3',
     install_requires=reqs,
+    extras_require={
+        'graphical': graphical_reqs
+    },
     include_package_data=True,
     tests_require=["pytest", "pytest-env"],
     entry_points={
-        "console_scripts": ["scauto=SCAutolib.cli_commands:cli"]}
+        "console_scripts": ["scauto=SCAutolib.cli_commands:cli"]
+    }
 )
```

### Comparing `SCAutolib-1.0.17/test/test_ca.py` & `SCAutolib-1.1.0/test/test_ca.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/test/test_card.py` & `SCAutolib-1.1.0/test/test_card.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/test/test_cli.py` & `SCAutolib-1.1.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/test/test_controller.py` & `SCAutolib-1.1.0/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/test/test_file.py` & `SCAutolib-1.1.0/test/test_file.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/test/test_openssl_conf.py` & `SCAutolib-1.1.0/test/test_openssl_conf.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/test/test_sssd_conf.py` & `SCAutolib-1.1.0/test/test_sssd_conf.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/test/test_user.py` & `SCAutolib-1.1.0/test/test_user.py`

 * *Files identical despite different names*

### Comparing `SCAutolib-1.0.17/tox.ini` & `SCAutolib-1.1.0/tox.ini`

 * *Files identical despite different names*

