# Comparing `tmp/suricata-language-server-0.5.1.tar.gz` & `tmp/suricata-language-server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suricata-language-server-0.5.1.tar", last modified: Sat Jan 15 00:46:55 2022, max compression
+gzip compressed data, was "suricata-language-server-0.9.0.tar", last modified: Thu Apr 27 12:09:24 2023, max compression
```

## Comparing `suricata-language-server-0.5.1.tar` & `suricata-language-server-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-15 00:46:55.400117 suricata-language-server-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8203 2022-01-15 00:46:55.400117 suricata-language-server-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7494 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-01-15 00:46:55.404117 suricata-language-server-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-15 00:46:55.400117 suricata-language-server-0.5.1/suricata_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8203 2022-01-15 00:46:55.000000 suricata-language-server-0.5.1/suricata_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-01-15 00:46:55.000000 suricata-language-server-0.5.1/suricata_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-15 00:46:55.000000 suricata-language-server-0.5.1/suricata_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-01-15 00:46:55.000000 suricata-language-server-0.5.1/suricata_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-15 00:46:55.000000 suricata-language-server-0.5.1/suricata_language_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-15 00:46:55.000000 suricata-language-server-0.5.1/suricata_language_server.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-15 00:46:55.400117 suricata-language-server-0.5.1/suricatals/
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/suricatals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8224 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/suricatals/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    15060 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/suricatals/langserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/suricatals/parse_signatures.py
--rw-r--r--   0 runner    (1001) docker     (121)    26083 2022-01-15 00:46:36.000000 suricata-language-server-0.5.1/suricatals/tests_rules.py
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-04-27 12:09:24.802888 suricata-language-server-0.9.0/
+-rw-r--r--   0 eric      (1000) eric      (1000)    35147 2021-12-31 12:35:43.000000 suricata-language-server-0.9.0/LICENSE
+-rw-r--r--   0 eric      (1000) eric      (1000)     8789 2023-04-27 12:09:24.802888 suricata-language-server-0.9.0/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)     8100 2023-03-19 21:57:26.000000 suricata-language-server-0.9.0/README.rst
+-rw-r--r--   0 eric      (1000) eric      (1000)      109 2022-01-02 10:25:28.000000 suricata-language-server-0.9.0/pyproject.toml
+-rw-r--r--   0 eric      (1000) eric      (1000)      875 2023-04-27 12:09:24.802888 suricata-language-server-0.9.0/setup.cfg
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-04-27 12:09:24.798888 suricata-language-server-0.9.0/suricata_language_server.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)     8789 2023-04-27 12:09:24.000000 suricata-language-server-0.9.0/suricata_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)      507 2023-04-27 12:09:24.000000 suricata-language-server-0.9.0/suricata_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2023-04-27 12:09:24.000000 suricata-language-server-0.9.0/suricata_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       70 2023-04-27 12:09:24.000000 suricata-language-server-0.9.0/suricata_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       11 2023-04-27 12:09:24.000000 suricata-language-server-0.9.0/suricata_language_server.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2022-01-02 10:45:30.000000 suricata-language-server-0.9.0/suricata_language_server.egg-info/zip-safe
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-04-27 12:09:24.802888 suricata-language-server-0.9.0/suricatals/
+-rw-r--r--   0 eric      (1000) eric      (1000)     3280 2023-03-19 21:57:26.000000 suricata-language-server-0.9.0/suricatals/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     8996 2023-03-19 21:57:26.000000 suricata-language-server-0.9.0/suricatals/jsonrpc.py
+-rw-r--r--   0 eric      (1000) eric      (1000)    17934 2023-03-19 21:57:26.000000 suricata-language-server-0.9.0/suricatals/langserver.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     2362 2023-03-19 21:57:26.000000 suricata-language-server-0.9.0/suricatals/lsp_helpers.py
+-rw-r--r--   0 eric      (1000) eric      (1000)    14869 2023-03-19 22:13:16.000000 suricata-language-server-0.9.0/suricatals/parse_signatures.py
+-rw-r--r--   0 eric      (1000) eric      (1000)    33410 2023-03-19 22:18:08.000000 suricata-language-server-0.9.0/suricatals/tests_rules.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     2491 2023-03-19 21:57:26.000000 suricata-language-server-0.9.0/suricatals/unit_tests.py
```

### Comparing `suricata-language-server-0.5.1/LICENSE` & `suricata-language-server-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suricata-language-server-0.5.1/PKG-INFO` & `suricata-language-server-0.9.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: suricata-language-server
-Version: 0.5.1
-Summary: Suricata Signatures Language Server for the Language Server Protocol
-Home-page: https://github.com/StamusNetworks/suricata-language-server
-Author: Eric Leblond
-Author-email: el@stamus-networks.com
-License: GNU General Public License v3
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: No Input/Output (Daemon)
-Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Security
-License-File: LICENSE
-
 ========================
 Suricata Language Server
 ========================
 
 Suricata Language Server is an implementation of the Language Server Protocol for Suricata signatures.
 It adds syntax check and hints as well as auto-completion to your preferred editor once it is configured.
 
@@ -51,14 +33,22 @@
 
 You can use pip to install the Suricata language server ::
 
  pip install suricata-language-server
 
 Run this command with sudo if you want to install it globally.
 
+On system where `PEP 704 <https://peps.python.org/pep-0704/>`_  is implemented,
+the installation via PIP is done by default in a virtualenv which is not convenient
+for our use case where the editor is running the server. A workaround is to force
+the installation outside a virtualenv
+by doing ::
+
+ pip install --break-system-packages suricata-language-server
+
 If you are a Microsoft Windows user and need to install Suricata, you can use the MSI available on `Suricata download page <https://suricata.io/download/>`_.
 For Python, the installer from Python website available on their `Download page <https://www.python.org/downloads/windows/>`_ is working well.
 
 Manual Installation
 -------------------
 
 After cloning the repository, you need to install first the server by running in the root directory of the project ::
@@ -70,17 +60,19 @@
 to install it system wide if needed.
 
 Server options
 --------------
 
 See `suricata-language-server -h` for complete and up-to-date help.
 
-* --suricata-binary: path to the suricata binary used for signatures testing
-* --max-lines: don't run suricata tests if file is bigger then this limit (auto-completion only)
-
+* --suricata-binary: path to the suricata binary used for signatures testing (optional)
+* --suricata-config: path to the suricata config used for signatures testing (optional)
+* --max-lines: don't run suricata tests if file is bigger than this limit (auto-completion only)
+* --max-tracked-files: don't start suricata analysis if workspace file count is superior to this limit
+* --batch-file: batch mode to parse only the file in argument and return result on stdout
 
 Editors Configuration
 =====================
 
 Neovim
 ------
 
@@ -133,15 +125,15 @@
 The Suricata IntelliSense extension is hosted on its `own project on GitHub <https://github.com/StamusNetworks/suricata-ls-vscode>`_.
 
 Sublime Text 3
 --------------
 
 You can use the `LSP <https://lsp.sublimetext.io/>`_ Package to provide support for LSP to Sublime Text 3.
 
-To activate Suricata Language Server on .rules file, you need to create a new syntax for Suricata file by using the content of `Suricata Sublime syntax from justjamesnow <https://github.com/justjamesnow/SublimeSuricata/blob/master/suricata.sublime-syntax>`_
+To activate Suricata Language Server on .rules file, you need to create a new syntax for Suricata file by using the content of `Suricata Sublime syntax from OzurieXV <https://github.com/ozuriexv/SublimeSuricata>`_
 
 To do so you can click on ``Tools > Developer > New Syntax`` then paste the content of the file and modify the text `text.suricata` to `source.suricata`. This will provide syntax highlighting as well as a `source.suricata` Sublime selector that can be used to trigger the Suricata Language Server activation.
 
 To do that, you can setup the Suricata Language Server by following the documentation for the LSP package on `client configuration <https://lsp.sublimetext.io/guides/client_configuration/>`_. You will need to open ``Preferences > Package Settings > LSP > Settings`` and edit the configuration to add the Suricata Language Server.
 
 The following configuration is known to work ::
 
@@ -157,15 +149,15 @@
 
 Kate
 ----
 
 You can use Suricata Language Server in Kate by activating the `LSP Client Plugin <https://docs.kde.org/stable5/en/kate/kate/kate-application-plugin-lspclient.html>`_.
 
 .. image:: https://raw.githubusercontent.com/StamusNetworks/suricata-language-server/main/images/kate-sample.png
- 
+
 Once activated, you can go to ``Settings > Configure Kate > LSP Client`` then open the ``User Server Settings`` tab and add the configuration
 for the Language Server Protocol ::
 
   {
     "servers": {
         "suricata": {
             "command": ["/path/to/suricata-language-server", "--suricata-binary=/path/to/suricata"],
@@ -179,9 +171,7 @@
 Getting help
 ============
 
 You can get help by:
 
 * Opening an `issue on GitHub <https://github.com/StamusNetworks/suricata-language-server/issues>`_
 * Asking on `#suricata-language-server <https://discordapp.com/channels/911231224448712714/927591953967751199>`_ on Discord.
-
-
```

### Comparing `suricata-language-server-0.5.1/README.rst` & `suricata-language-server-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: suricata-language-server
+Version: 0.9.0
+Summary: Suricata Signatures Language Server for the Language Server Protocol
+Home-page: https://github.com/StamusNetworks/suricata-language-server
+Author: Eric Leblond
+Author-email: el@stamus-networks.com
+License: GNU General Public License v3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: No Input/Output (Daemon)
+Classifier: Intended Audience :: Information Technology
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security
+License-File: LICENSE
+
 ========================
 Suricata Language Server
 ========================
 
 Suricata Language Server is an implementation of the Language Server Protocol for Suricata signatures.
 It adds syntax check and hints as well as auto-completion to your preferred editor once it is configured.
 
@@ -33,14 +50,22 @@
 
 You can use pip to install the Suricata language server ::
 
  pip install suricata-language-server
 
 Run this command with sudo if you want to install it globally.
 
+On system where `PEP 704 <https://peps.python.org/pep-0704/>`_  is implemented,
+the installation via PIP is done by default in a virtualenv which is not convenient
+for our use case where the editor is running the server. A workaround is to force
+the installation outside a virtualenv
+by doing ::
+
+ pip install --break-system-packages suricata-language-server
+
 If you are a Microsoft Windows user and need to install Suricata, you can use the MSI available on `Suricata download page <https://suricata.io/download/>`_.
 For Python, the installer from Python website available on their `Download page <https://www.python.org/downloads/windows/>`_ is working well.
 
 Manual Installation
 -------------------
 
 After cloning the repository, you need to install first the server by running in the root directory of the project ::
@@ -52,17 +77,19 @@
 to install it system wide if needed.
 
 Server options
 --------------
 
 See `suricata-language-server -h` for complete and up-to-date help.
 
-* --suricata-binary: path to the suricata binary used for signatures testing
-* --max-lines: don't run suricata tests if file is bigger then this limit (auto-completion only)
-
+* --suricata-binary: path to the suricata binary used for signatures testing (optional)
+* --suricata-config: path to the suricata config used for signatures testing (optional)
+* --max-lines: don't run suricata tests if file is bigger than this limit (auto-completion only)
+* --max-tracked-files: don't start suricata analysis if workspace file count is superior to this limit
+* --batch-file: batch mode to parse only the file in argument and return result on stdout
 
 Editors Configuration
 =====================
 
 Neovim
 ------
 
@@ -115,15 +142,15 @@
 The Suricata IntelliSense extension is hosted on its `own project on GitHub <https://github.com/StamusNetworks/suricata-ls-vscode>`_.
 
 Sublime Text 3
 --------------
 
 You can use the `LSP <https://lsp.sublimetext.io/>`_ Package to provide support for LSP to Sublime Text 3.
 
-To activate Suricata Language Server on .rules file, you need to create a new syntax for Suricata file by using the content of `Suricata Sublime syntax from justjamesnow <https://github.com/justjamesnow/SublimeSuricata/blob/master/suricata.sublime-syntax>`_
+To activate Suricata Language Server on .rules file, you need to create a new syntax for Suricata file by using the content of `Suricata Sublime syntax from OzurieXV <https://github.com/ozuriexv/SublimeSuricata>`_
 
 To do so you can click on ``Tools > Developer > New Syntax`` then paste the content of the file and modify the text `text.suricata` to `source.suricata`. This will provide syntax highlighting as well as a `source.suricata` Sublime selector that can be used to trigger the Suricata Language Server activation.
 
 To do that, you can setup the Suricata Language Server by following the documentation for the LSP package on `client configuration <https://lsp.sublimetext.io/guides/client_configuration/>`_. You will need to open ``Preferences > Package Settings > LSP > Settings`` and edit the configuration to add the Suricata Language Server.
 
 The following configuration is known to work ::
 
@@ -139,15 +166,15 @@
 
 Kate
 ----
 
 You can use Suricata Language Server in Kate by activating the `LSP Client Plugin <https://docs.kde.org/stable5/en/kate/kate/kate-application-plugin-lspclient.html>`_.
 
 .. image:: https://raw.githubusercontent.com/StamusNetworks/suricata-language-server/main/images/kate-sample.png
- 
+
 Once activated, you can go to ``Settings > Configure Kate > LSP Client`` then open the ``User Server Settings`` tab and add the configuration
 for the Language Server Protocol ::
 
   {
     "servers": {
         "suricata": {
             "command": ["/path/to/suricata-language-server", "--suricata-binary=/path/to/suricata"],
```

### Comparing `suricata-language-server-0.5.1/setup.cfg` & `suricata-language-server-0.9.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = suricata-language-server
-version = 0.5.1
+version = 0.9.0
 description = Suricata Signatures Language Server for the Language Server Protocol
 long_description = file: README.rst
 license = GNU General Public License v3
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python :: 3
 	Development Status :: 4 - Beta
```

### Comparing `suricata-language-server-0.5.1/suricata_language_server.egg-info/PKG-INFO` & `suricata-language-server-0.9.0/suricata_language_server.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: suricata-language-server
-Version: 0.5.1
+Version: 0.9.0
 Summary: Suricata Signatures Language Server for the Language Server Protocol
 Home-page: https://github.com/StamusNetworks/suricata-language-server
 Author: Eric Leblond
 Author-email: el@stamus-networks.com
 License: GNU General Public License v3
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
@@ -51,14 +50,22 @@
 
 You can use pip to install the Suricata language server ::
 
  pip install suricata-language-server
 
 Run this command with sudo if you want to install it globally.
 
+On system where `PEP 704 <https://peps.python.org/pep-0704/>`_  is implemented,
+the installation via PIP is done by default in a virtualenv which is not convenient
+for our use case where the editor is running the server. A workaround is to force
+the installation outside a virtualenv
+by doing ::
+
+ pip install --break-system-packages suricata-language-server
+
 If you are a Microsoft Windows user and need to install Suricata, you can use the MSI available on `Suricata download page <https://suricata.io/download/>`_.
 For Python, the installer from Python website available on their `Download page <https://www.python.org/downloads/windows/>`_ is working well.
 
 Manual Installation
 -------------------
 
 After cloning the repository, you need to install first the server by running in the root directory of the project ::
@@ -70,17 +77,19 @@
 to install it system wide if needed.
 
 Server options
 --------------
 
 See `suricata-language-server -h` for complete and up-to-date help.
 
-* --suricata-binary: path to the suricata binary used for signatures testing
-* --max-lines: don't run suricata tests if file is bigger then this limit (auto-completion only)
-
+* --suricata-binary: path to the suricata binary used for signatures testing (optional)
+* --suricata-config: path to the suricata config used for signatures testing (optional)
+* --max-lines: don't run suricata tests if file is bigger than this limit (auto-completion only)
+* --max-tracked-files: don't start suricata analysis if workspace file count is superior to this limit
+* --batch-file: batch mode to parse only the file in argument and return result on stdout
 
 Editors Configuration
 =====================
 
 Neovim
 ------
 
@@ -133,15 +142,15 @@
 The Suricata IntelliSense extension is hosted on its `own project on GitHub <https://github.com/StamusNetworks/suricata-ls-vscode>`_.
 
 Sublime Text 3
 --------------
 
 You can use the `LSP <https://lsp.sublimetext.io/>`_ Package to provide support for LSP to Sublime Text 3.
 
-To activate Suricata Language Server on .rules file, you need to create a new syntax for Suricata file by using the content of `Suricata Sublime syntax from justjamesnow <https://github.com/justjamesnow/SublimeSuricata/blob/master/suricata.sublime-syntax>`_
+To activate Suricata Language Server on .rules file, you need to create a new syntax for Suricata file by using the content of `Suricata Sublime syntax from OzurieXV <https://github.com/ozuriexv/SublimeSuricata>`_
 
 To do so you can click on ``Tools > Developer > New Syntax`` then paste the content of the file and modify the text `text.suricata` to `source.suricata`. This will provide syntax highlighting as well as a `source.suricata` Sublime selector that can be used to trigger the Suricata Language Server activation.
 
 To do that, you can setup the Suricata Language Server by following the documentation for the LSP package on `client configuration <https://lsp.sublimetext.io/guides/client_configuration/>`_. You will need to open ``Preferences > Package Settings > LSP > Settings`` and edit the configuration to add the Suricata Language Server.
 
 The following configuration is known to work ::
 
@@ -157,15 +166,15 @@
 
 Kate
 ----
 
 You can use Suricata Language Server in Kate by activating the `LSP Client Plugin <https://docs.kde.org/stable5/en/kate/kate/kate-application-plugin-lspclient.html>`_.
 
 .. image:: https://raw.githubusercontent.com/StamusNetworks/suricata-language-server/main/images/kate-sample.png
- 
+
 Once activated, you can go to ``Settings > Configure Kate > LSP Client`` then open the ``User Server Settings`` tab and add the configuration
 for the Language Server Protocol ::
 
   {
     "servers": {
         "suricata": {
             "command": ["/path/to/suricata-language-server", "--suricata-binary=/path/to/suricata"],
@@ -179,9 +188,7 @@
 Getting help
 ============
 
 You can get help by:
 
 * Opening an `issue on GitHub <https://github.com/StamusNetworks/suricata-language-server/issues>`_
 * Asking on `#suricata-language-server <https://discordapp.com/channels/911231224448712714/927591953967751199>`_ on Discord.
-
-
```

### Comparing `suricata-language-server-0.5.1/suricatals/jsonrpc.py` & `suricata-language-server-0.9.0/suricatals/jsonrpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,48 @@
+"""
+Copyright(C) 2018-2021 Chris Hansen <hansec@uw.edu>
+Copyright(C) 2021-2023 Stamus Networks
+Written by Chris Hansen <hansec@uw.edu>
+Written by Eric Leblond <eld@stamus-networks.com>
+
+This file is part of Suricata Language Server.
+
+Suricata Language Server is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Suricata Language Server is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Suricata Language Server.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
 import json
 import logging
-try:
-    import Queue
-except ImportError:
-    import queue as Queue
+import queue
 import threading
 from collections import deque
 import os
-try:
-    from urllib.parse import unquote
-except ImportError:
-    from urlparse import unquote
+from urllib.parse import unquote
 
 log = logging.getLogger(__name__)
 
 
 def path_from_uri(uri):
     # Convert file uri to path (strip html like head part)
     if not uri.startswith("file://"):
         return uri
     if os.name == "nt":
         if uri.startswith("file:///"):
             _, path = uri.split("file:///", 1)
-        else: # we should have an UNC path
+        else:  # we should have an UNC path
             _, path = uri.split("file:", 1)
             return path
     else:
         _, path = uri.split("file://", 1)
     return os.path.normpath(unquote(path))
 
 
@@ -174,15 +190,15 @@
 
         The responses is a generator where the nth response corresponds
         with the nth request. Users must read the generator until the end,
         otherwise you will leak a thread."""
 
         # We communicate the request ids using a thread safe queue.
         # It also allows us to bound the number of concurrent requests.
-        q = Queue.Queue(100)
+        q = queue.Queue(100)
 
         def send():
             for method, params in requests:
                 rid = self._next_id
                 self._next_id += 1
                 q.put(rid)
                 body = {
@@ -271,15 +287,15 @@
         while line != "\r\n":
             line = content.readline()
         body = content.read(length)
         # log.debug("RECV %s", body)
         return json.loads(body)
     #
     result_list = []
-    while(True):
+    while (True):
         try:
             result = receive_next()
         except EOFError:
             break
         else:
             result_list.append(result)
     return result_list
```

### Comparing `suricata-language-server-0.5.1/suricatals/langserver.py` & `suricata-language-server-0.9.0/suricatals/langserver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,64 @@
+"""
+Copyright(C) 2018-2021 Chris Hansen <hansec@uw.edu>
+Copyright(C) 2021-2022 Stamus Networks
+
+This file is part of Suricata Language Server.
+
+Suricata Language Server is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Suricata Language Server is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Suricata Language Server.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
 import logging
 import os
 import traceback
 import re
 
 from suricatals.jsonrpc import path_from_uri
 from suricatals.parse_signatures import SuricataFile
 from suricatals.tests_rules import TestRules
 
 log = logging.getLogger(__name__)
 
 SURICATA_RULES_EXT_REGEX = re.compile(r'^\.rules?$', re.I)
 
-def init_file(filepath, rules_tester):
-    file_obj = SuricataFile(filepath, rules_tester=rules_tester)
+
+def init_file(filepath, rules_tester, line_limit):
+    file_obj = SuricataFile(filepath, rules_tester)
+    if file_obj.nLines < line_limit:
+        file_obj.check_file()
     return file_obj, None
 
 
 class LangServer:
+    ACTIONS_ITEMS = [
+        {'label': 'alert', 'kind': 14, 'detail': 'Alert action', 'documentation': 'Trigger alert'},
+        {'label': 'config', 'kind': 14, 'detail': 'Alert action',
+         'documentation': 'Configuration signature. Used mostly for conditional logging.'},
+        {'label': 'drop', 'kind': 14, 'detail': 'Alert action', 'documentation': 'Trigger alert and drop flow'},
+        {'label': 'pass', 'kind': 14, 'detail': 'Alert action', 'documentation': 'Stop inspecting the data'},
+        {'label': 'reject', 'kind': 14, 'detail': 'Alert action', 'documentation': 'Trigger alert and reset session'},
+        {'label': 'rejectsrc', 'kind': 14, 'detail': 'Alert action',
+            'documentation': 'Trigger alert and reset session for source IP'},
+        {'label': 'rejectdst', 'kind': 14, 'detail': 'Alert action',
+            'documentation': 'Trigger alert and reset session for destination IP'},
+        {'label': 'rejectboth', 'kind': 14, 'detail': 'Alert action',
+            'documentation': 'Trigger alert and reset session for both IPs'},
+    ]
+
     def __init__(self, conn, debug_log=False, settings=None):
         self.conn = conn
         self.running = True
         self.root_path = None
         self.fs = None
         self.workspace = {}
         self.source_dirs = []
@@ -32,17 +70,20 @@
         # Get launch settings
         if settings is None:
             settings = {}
         self.nthreads = settings.get("nthreads", 4)
         self.notify_init = settings.get("notify_init", False)
         self.sync_type = settings.get("sync_type", 1)
         self.suricata_binary = settings.get("suricata_binary", 'suricata')
+        self.suricata_config = settings.get("suricata_config", None)
         self.max_lines = settings.get("max_lines", 1000)
-        self.rules_tester = TestRules(suricata_binary=self.suricata_binary)
+        self.max_tracked_files = settings.get("max_tracked_files", 100)
+        self.rules_tester = TestRules(suricata_binary=self.suricata_binary, suricata_config=self.suricata_config)
         self.keywords_list = self.rules_tester.build_keywords_list()
+        self.app_layer_list = self.rules_tester.build_app_layer_list()
 
     def post_message(self, message, msg_type=1):
         self.conn.send_notification("window/showMessage", {
             "type": msg_type,
             "message": message
         })
 
@@ -60,16 +101,15 @@
                 break
             else:
                 for message in self.post_messages:
                     self.post_message(message[1], message[0])
                 self.post_messages = []
 
     def handle(self, request):
-        # pylint: disable=unused-argument
-        def noop(request):
+        def noop(_):
             return None
         # Request handler
         log.debug("REQUEST %s %s", request.get("id"), request.get("method"))
         handler = {
             "initialize": self.serve_initialize,
             "textDocument/documentSymbol": noop,
             "textDocument/completion": self.serve_autocomplete,
@@ -97,15 +137,15 @@
         # We handle notifications differently since we can't respond
         if "id" not in request:
             try:
                 handler(request)
             # pylint: disable=W0703
             except Exception:
                 log.warning(
-                        "error handling notification %s", request, exc_info=True)
+                    "error handling notification %s", request, exc_info=True)
             return
         #
         try:
             resp = handler(request)
         except JSONRPC2Error as e:
             self.conn.write_error(
                 request["id"], code=e.code, message=e.message, data=e.data)
@@ -130,15 +170,15 @@
             params.get("rootUri") or params.get("rootPath") or "")
         self.source_dirs.append(self.root_path)
         # Recursively add sub-directories
         if len(self.source_dirs) == 1:
             self.source_dirs = []
             for dirName, subdirList, fileList in os.walk(self.root_path):
                 if self.excl_paths.count(dirName) > 0:
-                    while(len(subdirList) > 0):
+                    while (len(subdirList) > 0):
                         del subdirList[0]
                     continue
                 contains_source = False
                 for filename in fileList:
                     _, ext = os.path.splitext(os.path.basename(filename))
                     if SURICATA_RULES_EXT_REGEX.match(ext):
                         contains_source = True
@@ -149,48 +189,59 @@
         self.workspace_init()
         #
         server_capabilities = {
             "completionProvider": {
                 "resolveProvider": False,
                 "triggerCharacters": ["%"]
             },
-            #"definitionProvider": True,
-            #"documentSymbolProvider": True,
-            #"referencesProvider": True,
-            #"hoverProvider": True,
-            #"implementationProvider": True,
-            #"renameProvider": True,
-            #"workspaceSymbolProvider": True,
+            # "definitionProvider": True,
+            # "documentSymbolProvider": True,
+            # "referencesProvider": True,
+            # "hoverProvider": True,
+            # "implementationProvider": True,
+            # "renameProvider": True,
+            # "workspaceSymbolProvider": True,
             "textDocumentSync": self.sync_type
         }
         if self.notify_init:
             self.post_messages.append([3, "suricatals initialization complete"])
         return {"capabilities": server_capabilities}
         #     "workspaceSymbolProvider": True,
         #     "streaming": False,
         # }
 
+    def _initial_params_autocomplete(self, request, file_obj):
+        params = request["params"]
+        edit_index = params['position']['line']
+        sig_content = file_obj.contents_split[edit_index]
+        sig_index = params['position']['character']
+        word_split = re.split(' +', sig_content[0:sig_index])
+        if len(word_split) == 1:
+            return self.ACTIONS_ITEMS
+        if len(word_split) == 2:
+            return self.app_layer_list
+        if edit_index == 0:
+            return None
+        elif not re.search(r'\\ *$', file_obj.contents_split[edit_index - 1]):
+            return None
+
     def serve_autocomplete(self, request):
         params = request["params"]
         uri = params["textDocument"]["uri"]
         path = path_from_uri(uri)
         file_obj = self.workspace.get(path)
         if file_obj is None:
             return None
         edit_index = params['position']['line']
         sig_content = file_obj.contents_split[edit_index]
-        sig_index = params['position']['character'] 
+        sig_index = params['position']['character']
         log.debug(sig_content)
         # not yet in content matching so just return nothing
-        if not '(' in sig_content[0:sig_index]:
-            if edit_index == 0:
-                return None
-            elif not re.search(r'\\ *$', file_obj.contents_split[edit_index - 1]):
-                return None
-                
+        if '(' not in sig_content[0:sig_index]:
+            return self._initial_params_autocomplete(request, file_obj)
         cursor = sig_index - 1
         while cursor > 0:
             log.debug("At index: %d of %d (%s)", cursor, len(sig_content), sig_content[cursor:sig_index])
             if not sig_content[cursor].isalnum() and not sig_content[cursor] in ['.', '_']:
                 break
             cursor -= 1
         log.debug("Final is: %d : %d", cursor, sig_index)
@@ -227,21 +278,19 @@
                 })
 
     def get_diagnostics(self, uri):
         filepath = path_from_uri(uri)
         file_obj = self.workspace.get(filepath)
         if file_obj is not None and file_obj.nLines < self.max_lines:
             try:
-                diags = file_obj.check_file()
+                diags = [diag.to_message() for diag in file_obj.check_file(workspace=self.workspace)]
             # pylint: disable=W0703
             except Exception as e:
                 if os.path.isfile(file_obj.path):
                     return None, e
-                else:
-                    return None, None
             else:
                 return diags, None
         return None, None
 
     def serve_onChange(self, request):
         # Update workspace from file sent by editor
         params = request["params"]
@@ -269,15 +318,14 @@
                     log.error('Change request failed for file "%s": Could not apply change', path, exc_info=True)
                     return
         # Parse newly updated file
         if reparse_req:
             _, err_str = self.update_workspace_file(path)
             if err_str is not None:
                 self.post_message('Change request failed for file "{0}": {1}'.format(path, err_str))
-                return
 
     def serve_onOpen(self, request):
         self.serve_onSave(request, did_open=True)
 
     def serve_onClose(self, request):
         self.serve_onSave(request, did_close=True)
 
@@ -298,15 +346,15 @@
 
     def update_workspace_file(self, filepath, read_file=False, allow_empty=False):
         # Update workspace from file contents and path
         try:
             file_obj = self.workspace.get(filepath)
             if read_file:
                 if file_obj is None:
-                    file_obj = SuricataFile(filepath, rules_tester=self.rules_tester)
+                    file_obj = SuricataFile(filepath, self.rules_tester)
                     # Create empty file if not yet saved to disk
                     if not os.path.isfile(filepath):
                         if allow_empty:
                             self.workspace[filepath] = file_obj
                             return False, None
                         else:
                             return False, 'File does not exist'  # Error during load
@@ -342,40 +390,48 @@
                     for excl_suffix in self.excl_suffixes:
                         if filepath.endswith(excl_suffix):
                             inc_file = False
                             break
                     if inc_file:
                         file_list.append(filepath)
         # Process files
+        # don't send to analysis if too many files
+        if len(file_list) > self.max_tracked_files:
+            return
         from multiprocessing import Pool
         pool = Pool(processes=self.nthreads)
         results = {}
         for filepath in file_list:
-            results[filepath] = pool.apply_async(init_file, args=(filepath, self.rules_tester))
+            results[filepath] = pool.apply_async(init_file, args=(filepath, self.rules_tester, self.max_lines))
         pool.close()
         pool.join()
         for path, result in results.items():
             result_obj = result.get()
             if result_obj[0] is None:
                 self.post_messages.append([1, 'Initialization failed for file "{0}": {1}'.format(path, result_obj[1])])
                 continue
             self.workspace[path] = result_obj[0]
 
-    # pylint: disable=unused-argument
-    def serve_exit(self, request):
+    def serve_exit(self, _):
         # Exit server
         self.workspace = {}
         self.running = False
 
     def serve_default(self, request):
         # Default handler (errors!)
         raise JSONRPC2Error(
             code=-32601,
             message="method {} not found".format(request["method"]))
 
+    def analyse_file(self, filepath):
+        file_obj = SuricataFile(filepath, self.rules_tester)
+        file_obj.load_from_disk()
+        return file_obj.check_file()
+
+
 
 class JSONRPC2Error(Exception):
     def __init__(self, code, message, data=None):
         super().__init__(message)
         self.code = code
         self.message = message
         self.data = data
```

### Comparing `suricata-language-server-0.5.1/suricatals/tests_rules.py` & `suricata-language-server-0.9.0/suricatals/tests_rules.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 """
-Copyright(C) 2018-2020 Stamus Networks
-Written by Eric Leblond <eleblond@stamus-networks.com>
+Copyright(C) 2018-2023 Stamus Networks
+Written by Eric Leblond <el@stamus-networks.com>
 
-This file is part of Scirius.
+This file is part of Suricata Language Server.
 
-Scirius is free software: you can redistribute it and/or modify
+Suricata Language Server is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Scirius is distributed in the hope that it will be useful,
+Suricata Language Server is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Scirius.  If not, see <http://www.gnu.org/licenses/>.
+along with Suricata Language Server.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from json.decoder import JSONDecodeError
 import subprocess
 import tempfile
 import shutil
 import os
 import json
 import io
 import re
 import logging
 
 log = logging.getLogger(__name__)
 
+
 class TestRules():
     VARIABLE_ERROR = 101
     OPENING_RULE_FILE = 41  # Error when opening a file referenced in the source
     OPENING_DATASET_FILE = 322  # Error when opening a dataset referenced in the source
     RULEFILE_ERRNO = [39, 42]
     USELESS_ERRNO = [40, 43, 44]
     CONFIG_FILE = """
 %YAML 1.1
 ---
+stats:
+  enabled: no
 logging:
   default-log-level: warning
   outputs:
   - console:
       enabled: yes
       type: json
 app-layer:
   protocols:
     tls:
       ja3-fingerprints: yes
+engine-analysis:
+  rules-fast-pattern: yes
+  rules: yes
 vars:
   address-groups:
     HOME_NET: "[192.168.0.0/16,10.0.0.0/8,172.16.0.0/12]"
     EXTERNAL_NET: "!$HOME_NET"
     HTTP_SERVERS: "$HOME_NET"
     SMTP_SERVERS: "$HOME_NET"
     SQL_SERVERS: "$HOME_NET"
@@ -155,232 +161,313 @@
 config classification: social-engineering,Possible Social Engineering Attempted,2
 config classification: coin-mining,Crypto Currency Mining Activity Detected,2
 config classification: command-and-control,Malware Command and Control Activity Detected,1
 """
     SURICATA_SYNTAX_CHECK = "Suricata Syntax Check"
     SURICATA_ENGINE_ANALYSIS = "Suricata Engine Analysis"
 
-    def __init__(self, suricata_binary='suricata') -> None:
+    def __init__(self, suricata_binary='suricata', suricata_config=None) -> None:
         self.suricata_binary = suricata_binary
+        self.suricata_config = suricata_config
         self.suricata_version = self.get_suricata_version()
 
     def get_suricata_version(self):
         suri_cmd = [self.suricata_binary, '-V']
         suriprocess = subprocess.Popen(suri_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (outdata, _) = suriprocess.communicate()
         for line in io.StringIO(outdata.decode('utf-8')):
             mm = re.match(r'This is Suricata version (\d+\.\d+\.\d+)', line)
             if mm is not None:
                 return mm.group(1)
+        return "6.0.0"
 
     def json_compat_version(self):
         (major, minor, fix) = self.suricata_version.split('.')
         if int(major) < 6:
             return True
         elif int(major) == 6 and int(minor) == 0 and int(fix) < 4:
             return False
         return True
 
-    def parse_suricata_error(self, error, single=False):
+    def parse_suricata_error_after_7(self, error):
+        ret = {
+            'errors': [],
+            'warnings': [],
+        }
+        error_stream = io.StringIO(error)
+        wait_line = False
+        prev_err = {}
+        for line in error_stream:
+            try:
+                s_err = json.loads(line)
+            except JSONDecodeError:
+                continue
+            if s_err['event_type'] != 'engine':
+                continue
+            s_err['engine']['source'] = self.SURICATA_SYNTAX_CHECK
+
+            if not s_err['engine']['module'].startswith('detect') and s_err['engine']['module'] not in ['rule-vars']:
+                continue
+            if s_err['engine']['module'] == 'detect-parse':
+                if s_err['log_level'] == 'Error':
+                    ret['errors'].append(s_err['engine'])
+                    wait_line = True
+                else:
+                    ret['warnings'].append(s_err['engine'])
+                    getsid = re.compile(r"sid *:(\d+)")
+                    match = getsid.search(line)
+                    if match:
+                        s_err['engine']['sid'] = int(match.groups()[0])
+            elif s_err['engine']['module'] == 'detect-dataset':
+                if not wait_line:
+                    if s_err['engine']['message'].startswith("bad type"):
+                        s_err['engine']['message'] = "dataset: " + s_err['engine']['message']
+                    ret['errors'].append(s_err['engine'])
+                    wait_line = True
+            elif s_err['engine']['module'] == 'rules-vars':
+                ret['errors'].append(s_err['engine'])
+            elif s_err['engine']['module'] == 'detect':
+                if 'error parsing signature' in s_err['engine']['message']:
+                    message = s_err['engine']['message']
+                    s_err['engine']['message'] = s_err['engine']['message'].split(' from file')[0]
+                    getsid = re.compile(r"sid *:(\d+)")
+                    match = getsid.search(line)
+                    if match:
+                        s_err['engine']['sid'] = int(match.groups()[0])
+                    getline = re.compile(r"at line (\d+)$")
+                    match = getline.search(message)
+                    if match:
+                        line_nb = int(match.groups()[0])
+                        if wait_line:
+                            if prev_err!= {}:
+                                prev_err['engine']['line'] = line_nb - 1
+                                ret['errors'].append(prev_err['engine'])
+                        else:
+                            if prev_err != {} and prev_err['log_level'] == 'Warning':
+                                prev_err['engine']['line'] = line_nb - 1
+                                ret['errors'].append(prev_err['engine'])
+                            else:
+                                s_err['engine']['line'] = line_nb - 1
+                                ret['errors'].append(s_err['engine'])
+                    wait_line = False
+                else:
+                    ret['errors'].append(s_err['engine'])
+            else:
+                if not wait_line:
+                    if s_err['log_level'] == 'Error':
+                        ret['errors'].append(s_err['engine'])
+                        wait_line = True
+            prev_err = s_err
+        return ret
+
+    # pylint: disable=W0613
+    def parse_suricata_error_before_7(self, error, single=False):
         ret = {
             'errors': [],
             'warnings': [],
         }
-        variable_list = []
         files_list = []
         ignore_next = False
         error_stream = io.StringIO(error)
+        error_type = 'errors'
+        prev_err = None
         for line in error_stream:
             try:
                 s_err = json.loads(line)
             except JSONDecodeError:
-                ret['errors'].append({'message': error, 'format': 'raw', 'source': self.SURICATA_SYNTAX_CHECK})
-                return ret
+                continue
             s_err['engine']['source'] = self.SURICATA_SYNTAX_CHECK
             errno = s_err['engine']['error_code']
-            if not single or errno not in self.RULEFILE_ERRNO:
-                if errno == self.VARIABLE_ERROR:
-                    variable = s_err['engine']['message'].split("\"")[1]
-                    if not "$" + variable in variable_list:
-                        variable_list.append("$" + variable)
-                        s_err['engine']['message'] = "Custom address variable \"$%s\" is used and need to be defined in probes configuration" % (variable)
-                        ret['warnings'].append(s_err['engine'])
+            if s_err.get('log_level', '') != 'Error':
+                if errno not in [176, 242]:
+                    prev_err = s_err['engine']
                     continue
-                if errno == self.OPENING_DATASET_FILE:
-                    m = re.match('fopen \'([^:]*)\' failed: No such file or directory', s_err['engine']['message'])
-                    if m is not None:
-                        datasource = m.group(1)
-                        s_err['engine']['message'] = 'Dataset source "%s" is a dependancy and needs to be added to rulesets' % datasource
-                        ret['warnings'].append(s_err['engine'])
-                        ignore_next = True
-                        continue
-                if errno == self.OPENING_RULE_FILE:
-                    m = re.match('opening hash file ([^:]*): No such file or directory', s_err['engine']['message'])
-                    if m is not None:
-                        filename = m.group(1)
-                        filename = filename.rsplit('/', 1)[1]
-                        files_list.append(filename)
-                        s_err['engine']['message'] = 'External file "%s" is a dependancy and needs to be added to rulesets' % filename
-                        ret['warnings'].append(s_err['engine'])
-                        continue
-                if errno not in self.USELESS_ERRNO:
-                    # clean error message
-                    if errno == 39:
-                        if 'failed to set up dataset' in s_err['engine']['message']:
-                            if ignore_next:
-                                continue
+            if errno == self.VARIABLE_ERROR:
+                variable = s_err['engine']['message'].split("\"")[1]
+                s_err['engine']['message'] = "Custom address variable \"$%s\" is used " \
+                    "and need to be defined in probes configuration" % (variable)
+                s_err['engine']['suricata_error'] = True
+                if self.suricata_config is None:
+                    error_type = 'warnings'
+                ret[error_type].append(s_err['engine'])
+                continue
+            elif errno == self.OPENING_DATASET_FILE:
+                m = re.match('fopen \'([^:]*)\' failed: No such file or directory', s_err['engine']['message'])
+                if m is not None:
+                    datasource = m.group(1)
+                    s_err['engine']['message'] = 'Dataset source "%s" is a dependency " \
+                        "and needs to be added to rulesets' % datasource
+                    s_err['engine']['suricata_error'] = True
+                    error_type = 'warnings'
+                    ret[error_type].append(s_err['engine'])
+                    ignore_next = True
+                    continue
+            elif errno == self.OPENING_RULE_FILE:
+                m = re.match('opening hash file ([^:]*): No such file or directory', s_err['engine']['message'])
+                if m is not None:
+                    filename = m.group(1)
+                    filename = filename.rsplit('/', 1)[1]
+                    files_list.append(filename)
+                    s_err['engine']['message'] = 'External file "%s" is a dependency ' \
+                        'and needs to be added to rulesets' % filename
+                    s_err['engine']['suricata_error'] = True
+                    error_type = 'warnings'
+                    ret[error_type].append(s_err['engine'])
+                    continue
+            elif errno == 176:
+                warning, sig_content = s_err['engine']['message'].split('"', 1)
+                ret['warnings'].append({'message': warning.rstrip(),
+                                           'source': self.SURICATA_SYNTAX_CHECK,
+                                           'content': sig_content.rstrip('"')})
+            # Message for invalid signature
+            elif errno == 276:
+                rule, warning = s_err['engine']['message'].split(': ', 1)
+                rule = int(rule.split(' ')[1])
+                ret['warnings'].append({'message': warning.rstrip(), 'source': self.SURICATA_SYNTAX_CHECK, 'sid': rule})
+            elif errno not in self.USELESS_ERRNO:
+                # clean error message
+                if errno == 39:
+                    if 'failed to set up dataset' in s_err['engine']['message']:
                         if ignore_next:
-                            ignore_next = False
                             continue
-                        # exclude error on variable
-                        found = False
-                        for variable in variable_list:
-                            if variable in s_err['engine']['message']:
-                                found = True
-                                break
-                        else:
-                            # exclude error on external file
-                            for filename in files_list:
-                                if re.search(': *%s *;' % filename, s_err['engine']['message']):
-                                    found = True
-                                    break
-                        if found:
+                    if ignore_next:
+                        ignore_next = False
+                        continue
+                    if 'error parsing signature' in s_err['engine']['message']:
+                        message = s_err['engine']['message']
+                        s_err['engine']['message'] = s_err['engine']['message'].split(' from file')[0]
+                        getsid = re.compile(r"sid *:(\d+)")
+                        match = getsid.search(line)
+                        if match:
+                            s_err['engine']['sid'] = int(match.groups()[0])
+                        getline = re.compile(r"at line (\d+)$")
+                        match = getline.search(message)
+                        if match:
+                            line_nb = int(match.groups()[0])
+                            if prev_err is not None:
+                                prev_err['line'] = line_nb - 1
+                                ret['errors'].append(prev_err)
+                                prev_err = None
+                            else:
+                                if len(ret[error_type]):
+                                    ret[error_type][-1]['line'] = line_nb - 1
+                                error_type = 'errors'
                             continue
-                        if 'error parsing signature' in s_err['engine']['message']:
-                            message = s_err['engine']['message']
-                            s_err['engine']['message'] = s_err['engine']['message'].split(' from file')[0]
-                            getsid = re.compile(r"sid *:(\d+)")
-                            match = getsid.search(line)
-                            if match:
-                                s_err['engine']['sid'] = int(match.groups()[0])
-                            getline = re.compile(r"at line (\d+)$")
-                            match = getline.search(message)
-                            if match:
-                                line_nb = int(match.groups()[0])
-                                if len(ret['errors']):
-                                    ret['errors'][-1]['line'] = line_nb - 1
-                                continue
-                    if errno == 42:
-                        s_err['engine']['message'] = s_err['engine']['message'].split(' from')[0]
-                    ret['errors'].append(s_err['engine'])
+                if errno == 42:
+                    s_err['engine']['message'] = s_err['engine']['message'].split(' from')[0]
+                ret['errors'].append(s_err['engine'])
         return ret
 
-    def generate_config(self, tmpdir, config_buffer=None, related_files=None, reference_config=None, classification_config=None):
+    def parse_suricata_error(self, error, single=False):
+        (major, _, _) = self.suricata_version.split('.')
+        if int(major) < 7:
+            return self.parse_suricata_error_before_7(error, single)
+        else:
+            return self.parse_suricata_error_after_7(error)
+
+    def generate_config(self, tmpdir, config_buffer=None, related_files=None,
+                        reference_config=None, classification_config=None):
         if not reference_config:
             reference_config = self.REFERENCE_CONFIG
         reference_file = os.path.join(tmpdir, "reference.config")
-        rf = open(reference_file, 'w', encoding='utf-8')
-        rf.write(reference_config)
-        rf.close()
+        with open(reference_file, 'w', encoding='utf-8') as rf:
+            rf.write(reference_config)
 
         if not classification_config:
             classification_config = self.CLASSIFICATION_CONFIG
         classification_file = os.path.join(tmpdir, "classification.config")
-        cf = open(classification_file, 'w', encoding='utf-8')
-        cf.write(classification_config)
-        cf.close()
+        with open(classification_file, 'w', encoding='utf-8') as cf:
+            cf.write(classification_config)
 
         if not config_buffer:
-            config_buffer = self.CONFIG_FILE
+            if self.suricata_config is None:
+                config_buffer = self.CONFIG_FILE
+            else:
+                with open(self.suricata_config, 'r', encoding='utf-8') as conf_file:
+                    config_buffer = conf_file.read()
         config_file = os.path.join(tmpdir, "suricata.yaml")
-        cf = open(config_file, 'w', encoding='utf-8')
-        # write the config file in temp dir
-        cf.write(config_buffer)
-        cf.write("mpm-algo: ac-bs\n")
-        cf.write("default-rule-path: " + tmpdir + "\n")
-        cf.write("reference-config-file: " + tmpdir + "/reference.config\n")
-        cf.write("classification-file: " + tmpdir + "/classification.config\n")
-        cf.write("""
+        with open(config_file, 'w', encoding='utf-8') as cf:
+            # write the config file in temp dir
+            cf.write(config_buffer)
+            cf.write("mpm-algo: ac-bs\n")
+            cf.write("default-rule-path: " + tmpdir + "\n")
+            cf.write("reference-config-file: " + tmpdir + "/reference.config\n")
+            cf.write("classification-file: " + tmpdir + "/classification.config\n")
+            cf.write("""
 engine-analysis:
   rules-fast-pattern: yes
-  rules: yes""")
+  rules: yes
+logging:
+  default-log-level: warning
+  outputs:
+  - console:
+      enabled: yes
+      type: json
+stats:
+  enabled: no
+                 """)
 
-        cf.close()
         related_files = related_files or {}
         for rfile in related_files:
             related_file = os.path.join(tmpdir, rfile)
-            rf = open(related_file, 'w', encoding='utf-8')
-            rf.write(related_files[rfile])
-            rf.close()
+            with open(related_file, 'w', encoding='utf-8') as rf:
+                rf.write(related_files[rfile])
 
         return config_file
 
-    def rule_buffer(self, rule_buffer, config_buffer=None, related_files=None, reference_config=None, classification_config=None):
+    def rule_buffer(self, rule_buffer, config_buffer=None, related_files=None,
+                    reference_config=None, classification_config=None):
         # create temp directory
         tmpdir = tempfile.mkdtemp()
         # write the rule file in temp dir
         rule_file = os.path.join(tmpdir, "file.rules")
-        rf = open(rule_file, 'w', encoding='utf-8')
-        rf.write(rule_buffer)
-        rf.close()
+        with open(rule_file, 'w', encoding='utf-8') as rf:
+            rf.write(rule_buffer)
 
-        config_file = self.generate_config(tmpdir, config_buffer=config_buffer, related_files=related_files, reference_config=reference_config, classification_config=classification_config)
+        config_file = self.generate_config(tmpdir, config_buffer=config_buffer,
+                                           related_files=related_files, reference_config=reference_config,
+                                           classification_config=classification_config)
 
         suri_cmd = [self.suricata_binary, '-T', '-l', tmpdir, '-S', rule_file, '-c', config_file]
         # start suricata in test mode
-        suriprocess = subprocess.Popen(suri_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        (outdata, errdata) = suriprocess.communicate()
-        result = {'status': True, 'errors': "", 'warnings': [], 'info': [] }
+        suriprocess = subprocess.Popen(suri_cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        (errdata, _) = suriprocess.communicate()
+        result = {'status': True, 'errors': "", 'warnings': [], 'info': []}
         # if not a success
         if suriprocess.returncode != 0:
             result['status'] = False
-            result['errors'] = errdata.decode('utf-8')
-        # analyse potential warnings
-        message_stream = io.StringIO(outdata.decode('utf-8'))
-        for message in message_stream:
-            try:
-                struct_msg = json.loads(message)
-            except JSONDecodeError:
-                continue
-            if not 'engine' in struct_msg:
-                continue
-            # Check for duplicate signatures
-            error_code = struct_msg['engine'].get('error_code', 0) 
-            if error_code == 176:
-                warning, sig_content = struct_msg['engine']['message'].split('"', 1)
-                result['warnings'].append({'message': warning.rstrip(), 'source': self.SURICATA_SYNTAX_CHECK, 'content': sig_content.rstrip('"')})
-            # Message for invalid signature
-            elif error_code == 276:
-                rule, warning = struct_msg['engine']['message'].split(': ', 1)
-                rule = int(rule.split(' ')[1])
-                result['warnings'].append({'message': warning.rstrip(), 'source': self.SURICATA_SYNTAX_CHECK, 'sid': rule})
-
+        result['errors'] = errdata.decode('utf-8')
         # runs rules analysis to have warnings
         suri_cmd = [self.suricata_binary, '--engine-analysis', '-l', tmpdir, '-S', rule_file, '-c', config_file]
         # start suricata in test mode
         suriprocess = subprocess.Popen(suri_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        (outdata, errdata) = suriprocess.communicate()
+        (_, errdata) = suriprocess.communicate()
         engine_analysis = self.parse_engine_analysis(tmpdir)
         for signature in engine_analysis:
             for warning in signature.get('warnings', []):
-                result['warnings'].append({'message': warning, 'source': self.SURICATA_ENGINE_ANALYSIS, 'content': signature['content']})
+                result['warnings'].append({'message': warning,
+                                           'source': self.SURICATA_ENGINE_ANALYSIS,
+                                           'content': signature['content']})
             for info in signature.get('info', []):
-                msg = {'message': info, 'source': self.SURICATA_ENGINE_ANALYSIS, 'content': signature['content'], 'start_char': 0, 'end_char': 1}
-                if "Fast Pattern \"" in info:
-                    if 'fast_pattern' in signature['content']:
-                        continue
-                    if signature['content'].count('content:') <= 1:
-                        continue
-                    pattern = info.split('"')[1]
-                    try:
-                        msg['start_char'] = signature['content'].index(pattern)
-                        msg['end_char'] = signature['content'].index(pattern) + len(pattern)
-                    except ValueError:
-                        msg['start_char'] = 0
-                        msg['end_char'] = 1
+                msg = {'message': info, 'source': self.SURICATA_ENGINE_ANALYSIS, 'content': signature['content']}
                 result['info'].append(msg)
+        mpm_analysis = self.mpm_parse_rules_json(tmpdir)
+        result['mpm'] = mpm_analysis
         shutil.rmtree(tmpdir)
         return result
 
     def check_rule_buffer(self, rule_buffer, config_buffer=None, related_files=None, single=False):
         related_files = related_files or {}
         prov_result = self.rule_buffer(rule_buffer, config_buffer=config_buffer, related_files=related_files)
         if len(prov_result.get('errors', [])):
             res = self.parse_suricata_error(prov_result['errors'], single=single)
-            prov_result['errors'] = res['errors']
+            if 'errors' in res:
+                prov_result['errors'] = res['errors']
+            if 'warnings' in res:
+                prov_result['warnings'].extend(res['warnings'])
         return prov_result
 
     def parse_engine_analysis(self, log_dir):
         json_path = os.path.join(log_dir, 'rules.json')
         if os.path.isfile(json_path) and self.json_compat_version():
             return self.parse_engine_analysis_v2(json_path)
         return self.parse_engine_analysis_v1(log_dir)
@@ -395,24 +482,24 @@
                     in_sid_data = True
                     signature = {'sid': line.split(' ')[2]}
                     continue
                 elif in_sid_data and len(line) == 1:
                     in_sid_data = False
                     analysis.append(signature)
                     signature = {}
-                elif in_sid_data and not 'content' in signature:
+                elif in_sid_data and 'content' not in signature:
                     signature['content'] = line.strip()
                     continue
                 elif in_sid_data and 'Warning: ' in line:
-                    warning = line.split('arning: ')[1]
-                    if not 'warnings' in signature:
+                    warning = line.split('Warning: ')[1]
+                    if 'warnings' not in signature:
                         signature['warnings'] = []
                     signature['warnings'].append(warning.strip())
                 elif in_sid_data and 'Fast Pattern' in line:
-                    if not 'info' in signature:
+                    if 'info' not in signature:
                         signature['info'] = []
                     signature['info'].append(line.strip())
         return analysis
 
     def parse_engine_analysis_v2(self, json_path):
         analysis = []
         with open(json_path, 'r', encoding='utf-8') as analysis_file:
@@ -423,79 +510,129 @@
                 except JSONDecodeError:
                     pass
                 signature_msg = {'content': signature_info['raw']}
                 if 'id' in signature_info:
                     signature_msg['sid'] = signature_info['id']
                 if 'flags' in signature_info:
                     if 'toserver' in signature_info['flags'] and 'toclient' in signature_info['flags']:
-                        if not 'warnings' in signature_msg:
+                        if 'warnings' not in signature_msg:
                             signature_msg['warnings'] = []
                         signature_msg['warnings'].append('Rule inspect server and client side, consider adding a flow keyword')
-                if 'mpm' in signature_info:
-                    if not 'info' in signature_msg:
-                        signature_msg['info'] = []
-                    signature_msg['info'].append('Fast Pattern "%s" on %s' % (signature_info['mpm']['pattern'], signature_info['mpm']['buffer']))
-                elif 'engines' in signature_info:
-                    # Suricata 6.0.x don't have the mpm sub object
-                    fp_buffer = None
-                    fp_pattern = None
-                    for engine in signature_info['engines']:
-                        if engine['is_mpm']:
-                            fp_buffer = engine['name']
-                            for match in engine.get('matches', []):
-                                if match.get('content', {}).get('is_mpm', False):
-                                    fp_pattern = match['content']['pattern']
-                    if fp_buffer and fp_pattern:
-                        if not 'info' in signature_msg:
-                            signature_msg['info'] = []
-                        signature_msg['info'].append('Fast Pattern "%s" on %s' % (fp_pattern, fp_buffer))
                 if 'warnings' in signature_info:
-                    if not 'warnings' in signature_msg:
+                    if 'warnings' not in signature_msg:
                         signature_msg['warnings'] = []
                     signature_msg['warnings'].extend(signature_info.get('warnings', []))
                 if 'notes' in signature_info:
-                    if not 'info' in signature_msg:
+                    if 'info' not in signature_msg:
                         signature_msg['info'] = []
                     signature_msg['info'].extend(signature_info.get('notes', []))
                 if 'engines' in signature_info:
                     app_proto = None
                     multiple_app_proto = False
                     got_raw_match = False
                     got_content = False
                     got_pcre = False
                     for engine in signature_info['engines']:
                         if 'app_proto' in engine:
                             if app_proto is None:
                                 app_proto = engine.get('app_proto')
                             else:
                                 if app_proto != engine.get('app_proto'):
-                                    if not app_proto in ['http', 'http2'] or not engine.get('app_proto') in ['http', 'http2']:
+                                    if app_proto not in ['http', 'http2'] or engine.get('app_proto') not in ['http', 'http2']:
                                         multiple_app_proto = True
                         else:
                             got_raw_match = True
                         for match in engine.get('matches', []):
                             if match['name'] == 'content':
                                 got_content = True
                             elif match['name'] == 'pcre':
                                 got_pcre = True
                     if got_pcre and not got_content:
-                        if not 'warnings' in signature_msg:
+                        if 'warnings' not in signature_msg:
                             signature_msg['warnings'] = []
                         signature_msg['warnings'].append('Rule with pcre without content match (possible performance issue)')
                     if app_proto is not None and got_raw_match:
-                        if not 'warnings' in signature_msg:
+                        if 'warnings' not in signature_msg:
                             signature_msg['warnings'] = []
-                        signature_msg['warnings'].append('Application layer "%s" combined with raw match, consider using a match on application buffer' %  (app_proto))
+                        signature_msg['warnings'].append('Application layer "%s" combined with raw match, '
+                                                         'consider using a match on application buffer' % (app_proto))
                     if multiple_app_proto:
-                        if not 'warnings' in signature_msg:
+                        if 'warnings' not in signature_msg:
                             signature_msg['warnings'] = []
                         signature_msg['warnings'].append('Multiple application layers in same signature')
                 analysis.append(signature_msg)
         return analysis
 
+    def mpm_parse_rules_json(self, log_dir):
+        mpm_data = []
+        mpm_analysis = {'buffer': {}, 'sids': {}}
+        try:
+            with open(os.path.join(log_dir, 'rules.json'), 'r', encoding='utf-8') as rules_json:
+                for line in rules_json:
+                    # some suricata version have an invalid JSON formatted message
+                    try:
+                        rule_analysis = json.loads(line)
+                    except json.JSONDecodeError:
+                        return None
+                    if 'mpm' in rule_analysis:
+                        rule_analysis['mpm']['id'] = rule_analysis['id']
+                        rule_analysis['mpm']['gid'] = rule_analysis['gid']
+                        mpm_data.append(rule_analysis['mpm'])
+                    else:
+                        if 'engines' in rule_analysis:
+                            fp_buffer = None
+                            fp_pattern = None
+                            for engine in rule_analysis.get('engines', []):
+                                if engine['is_mpm']:
+                                    fp_buffer = engine['name']
+                                    for match in engine.get('matches', []):
+                                        if match.get('name') == 'content':
+                                            if match.get('content', {}).get('is_mpm', False):
+                                                fp_pattern = match['content']['pattern']
+                                                break
+                                    if fp_pattern:
+                                        break
+                            if fp_buffer and fp_pattern:
+                                mpm_data.append({'id': rule_analysis['id'], 'gid': rule_analysis['gid'],
+                                                 'buffer': fp_buffer, 'pattern': fp_pattern})
+                            continue
+                        if 'lists' in rule_analysis:
+                            fp_buffer = None
+                            fp_pattern = None
+                            for key in rule_analysis['lists']:
+                                fp_buffer = key
+                                for match in rule_analysis['lists'][key].get('matches', []):
+                                    if match.get('name') == 'content':
+                                        if match.get('content', {}).get('is_mpm', False):
+                                            fp_pattern = match['content']['pattern']
+                                            break
+                                if fp_pattern:
+                                    break
+                            if fp_buffer and fp_pattern:
+                                mpm_data.append({'id': rule_analysis['id'], 'gid': rule_analysis['gid'],
+                                                 'buffer': fp_buffer, 'pattern': fp_pattern})
+                            continue
+        except FileNotFoundError:
+            return mpm_analysis
+        # target to have
+        # { 'http.host': { 'grosminet': { 'count': 34, sigs: [{'id': 2, 'gid':1}]} } }
+        for sig in mpm_data:
+            if sig['buffer'] in mpm_analysis['buffer']:
+                if sig['pattern'] in mpm_analysis['buffer'][sig['buffer']]:
+                    mpm_analysis['buffer'][sig['buffer']][sig['pattern']]['count'] += 1
+                    mpm_analysis['buffer'][sig['buffer']][sig['pattern']]['sigs'].append({'id': sig['id'], 'gid': sig['gid']})
+                else:
+                    mpm_analysis['buffer'][sig['buffer']][sig['pattern']] = {'count': 1,
+                                                                             'sigs': [{'id': sig['id'], 'gid': sig['gid']}]}
+            else:
+                mpm_analysis['buffer'][sig['buffer']] = {sig['pattern']: {'count': 1,
+                                                                          'sigs': [{'id': sig['id'], 'gid': sig['gid']}]}}
+            mpm_analysis['sids'][sig['id']] = {'buffer': sig['buffer'], 'pattern': sig['pattern']}
+        return mpm_analysis
+
     def build_keywords_list(self):
         tmpdir = tempfile.mkdtemp()
         config_file = self.generate_config(tmpdir)
         suri_cmd = [self.suricata_binary, '--list-keywords=csv', '-l', tmpdir, '-c', config_file]
         # start suricata in test mode
         suriprocess = subprocess.Popen(suri_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (outdata, _) = suriprocess.communicate()
@@ -523,8 +660,25 @@
                 if 'content modifier' in keyword_array[3]:
                     keyword_item['tags'] = [1]
                     keyword_item['detail'] = 'Content Modifier'
                 keywords_list.append(keyword_item)
             except IndexError:
                 pass
         return keywords_list
-    
+
+    def build_app_layer_list(self):
+        tmpdir = tempfile.mkdtemp()
+        config_file = self.generate_config(tmpdir)
+        suri_cmd = [self.suricata_binary, '--list-app-layer-proto', '-l', tmpdir, '-c', config_file]
+        # start suricata in test mode
+        suriprocess = subprocess.Popen(suri_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        (outdata, _) = suriprocess.communicate()
+        shutil.rmtree(tmpdir)
+        applayers = outdata.decode('utf-8').splitlines()
+        while not applayers[0].startswith("===="):
+            applayers.pop(0)
+        applayers.pop(0)
+        applayers_list = [{'label': 'tcp', 'detail': 'tcp', 'kind': 14}, {'label': 'udp', 'detail': 'udp', 'kind': 14}]
+        for app_layer in applayers:
+            app_layer_item = {'label': app_layer, 'detail': app_layer, 'kind': 14}
+            applayers_list.append(app_layer_item)
+        return applayers_list
```

