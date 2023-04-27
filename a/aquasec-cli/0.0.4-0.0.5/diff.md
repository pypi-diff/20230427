# Comparing `tmp/aquasec-cli-0.0.4.tar.gz` & `tmp/aquasec-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aquasec-cli-0.0.4.tar", last modified: Tue Apr 25 19:24:47 2023, max compression
+gzip compressed data, was "aquasec-cli-0.0.5.tar", last modified: Thu Apr 27 15:26:49 2023, max compression
```

## Comparing `aquasec-cli-0.0.4.tar` & `aquasec-cli-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.673781 aquasec-cli-0.0.4/
--rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/LICENSE
--rw-rw-r--   0 adamt      (501) staff       (20)       97 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/MANIFEST.in
--rw-r--r--   0 adamt      (501) staff       (20)    44107 2023-04-25 19:24:47.674174 aquasec-cli-0.0.4/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     2211 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/README.md
--rw-rw-r--   0 adamt      (501) staff       (20)     2667 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/README.rst
--rw-rw-r--   0 adamt      (501) staff       (20)      520 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/SECURITY.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.667005 aquasec-cli-0.0.4/aquasec_cli/
--rw-rw-r--   0 adamt      (501) staff       (20)       60 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/_version.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.673238 aquasec-cli-0.0.4/aquasec_cli/commands/
--rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/commands/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1530 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/commands/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1916 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/commands/report.py
--rw-rw-r--   0 adamt      (501) staff       (20)      290 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/main.py
--rw-rw-r--   0 adamt      (501) staff       (20)      570 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/utils.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.671271 aquasec-cli-0.0.4/aquasec_cli.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)    44107 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      526 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       53 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/entry_points.txt
--rw-r--r--   0 adamt      (501) staff       (20)      107 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/top_level.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 19:24:41.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/zip-safe
--rw-rw-r--   0 adamt      (501) staff       (20)      931 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/pyproject.toml
--rw-rw-r--   0 adamt      (501) staff       (20)       61 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/requirements.txt
--rw-rw-r--   0 adamt      (501) staff       (20)      725 2023-04-25 19:24:47.675164 aquasec-cli-0.0.4/setup.cfg
--rw-rw-r--   0 adamt      (501) staff       (20)      111 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/setup.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.215618 aquasec-cli-0.0.5/
+-rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/LICENSE
+-rw-rw-r--   0 adamt      (501) staff       (20)       97 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/MANIFEST.in
+-rw-r--r--   0 adamt      (501) staff       (20)    43887 2023-04-27 15:26:49.216049 aquasec-cli-0.0.5/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)     2458 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/README.md
+-rw-rw-r--   0 adamt      (501) staff       (20)     2667 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/README.rst
+-rw-rw-r--   0 adamt      (501) staff       (20)      509 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/SECURITY.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.208872 aquasec-cli-0.0.5/aquasec_cli/
+-rw-rw-r--   0 adamt      (501) staff       (20)       60 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/_version.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.214779 aquasec-cli-0.0.5/aquasec_cli/commands/
+-rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/commands/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1530 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/commands/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1916 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/commands/report.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      290 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/main.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      570 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.212665 aquasec-cli-0.0.5/aquasec_cli.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    43887 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      526 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       53 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/entry_points.txt
+-rw-r--r--   0 adamt      (501) staff       (20)      107 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/top_level.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/zip-safe
+-rw-rw-r--   0 adamt      (501) staff       (20)      953 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/pyproject.toml
+-rw-rw-r--   0 adamt      (501) staff       (20)       61 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/requirements.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)      740 2023-04-27 15:26:49.217424 aquasec-cli-0.0.5/setup.cfg
+-rw-rw-r--   0 adamt      (501) staff       (20)      111 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/setup.py
```

### Comparing `aquasec-cli-0.0.4/LICENSE` & `aquasec-cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.4/PKG-INFO` & `aquasec-cli-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Aqua Security cli
 Author: atav928
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,117 +682,119 @@
 Project-URL: repository, https://github.com/atav928/aquasec-cli
 Keywords: aquasec,aqua security,workload protection
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-aquasec-cli
-===========
+# aquasec-cli
 
 Aqua Security CLI
 
-Installation
-------------
+## Installation
 
-.. code:: bash
+```bash
+>>> python -m pip install aquasec-cli
+```
 
-   >>> python -m pip install aquasec-cli
+## Usage
 
-Usage
------
+__Help Menu of all Groups:__
 
-**Help Menu of all Groups:**
+```bash
+>>> aquasec-cli --help
+Usage: aquasec-cli [OPTIONS] COMMAND [ARGS]...
 
-.. code:: bash
+  AquaSec CLI tool to manage AquaSec Tenant
 
-   aquasec-cli  --help    
-   Usage: aquasec-cli [OPTIONS] COMMAND [ARGS]...
+Options:
+  --help  Show this message and exit.
 
-     AquaSec CLI tool to manage AquaSec Tenant
+Commands:
+  delete   Deletes created API Auth
+  init     Initializes API Auth
+  reports  Generate CIS Bench Reports
+```
 
-   Options:
-     --help  Show this message and exit.
+__NOTE:__ Each subcommand has a help menu to assist with the calls being made. This project relies on the yaml or localized configurations being help as they are not passed in the commands as of this release.
 
-   Commands:
-     delapi   Deletes created API Auth
-     initapi  Initializes API Auth
-     reports  Generate CIS Bench Reports
+__Create API Auth Token:__
 
-**NOTE:** Each subcommand has a help menu to assist with the calls being
-made. This project relies on the yaml or localized configurations being
-help as they are not passed in the commands as of this release.
+```bash
+>>> aquasec-cli init --csp_roles="Auditor" --csp_roles="Admin" --endpoints="Any"
+Initializing API
+INFO    : Created WorkloadAuth Token for URL https://1234abcff1.cloud.aquasec.com
+```
 
-**Create API Auth Token:**
+__Run Report:__
 
-.. code:: bash
+```bash
+aquasec-cli  reports --report_type kube_bench --report_location /var/tmp
+Report completed Saving
+Report written out to /var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
+```
 
-   >>> aquasec-cli init --csp_roles="Auditor" --csp_roles="Admin" --endpoints="Any"
-   Initializing API
-   INFO    : Created WorkloadAuth Token for URL https://1234abcff1.cloud.aquasec.com
+__Delete API Auth:__
 
-**Run Report:**
+```bash
+>>> aquasec-cli delete                                              
+Are you sure you want to delete the auth api token? [y/N]: y
+Deleted Auth
+```
 
-.. code:: bash
+## Release Info
 
-   aquasec-cli  reports --report_type kube_bench --report_location /Users/username/var/tmp
-   Report completed Saving
-   Report written out to /Users/adamt/var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
+### v0.0.5
 
-**Delete API Auth:**
+* Updated Readme and changed type from RST to MD
+* Reverted snyk workflow file
 
-.. code:: bash
+### v0.0.4
 
-   >>> aquasec-cli delete                                              
-   Are you sure you want to delete the auth api token? [y/N]: y
-   Deleted Auth
+* fixed issue with broken aquasec-api v0.0.3
 
-Release Info
-------------
+### v0.0.3
 
-v0.0.2
-~~~~~~
+* Fixed installation and dependencies
+* locked down dependencies
+* added toml and setup.cfg to support furture installations
 
--  Bug fix with requirements
+### v0.0.2
 
-Version
--------
+* Bug fix with requirements
 
-+-------------------------+-----------------+-------------------------+
-| Version                 | Build           | Changes                 |
-+=========================+=================+=========================+
-| **0.0.2**               | **a1**          | issues with dataclasses |
-|                         |                 | getting installed under |
-|                         |                 | normal condition        |
-+-------------------------+-----------------+-------------------------+
-| **0.0.2**               | **final**       | tested in pytest and    |
-|                         |                 | seems to now accept the |
-|                         |                 | dataclass               |
-+-------------------------+-----------------+-------------------------+
-| **0.0.3**               | **a1**          | issues with dataclasses |
-|                         |                 | and now yaml getting    |
-|                         |                 | installed under normal  |
-|                         |                 | condition               |
-+-------------------------+-----------------+-------------------------+
+## Version
 
-Warnings
-~~~~~~~~
+| Version | Build | Changes |
+| ------- | ----- | ------- |
+| __0.0.2__ | __a1__ | issues with dataclasses getting installed under normal condition |
+| __0.0.2__ | __final__ | tested in pytest and seems to now accept the dataclass |
+| __0.0.3__ | __a1__ | issues with dataclasses and now yaml getting installed under normal condition |
+| __0.0.3__ | __a3__ | migrating to toml and setup.cfg |
+| __0.0.3__ | __a4__ | cleaned up utils and updated snyk to confirm pass locally; added to git ignore |
+| __0.0.3__ | __a5__ | setup.cfg issues wiht pip |
+| __0.0.3__ | __final__ | found issue with toml and other dependencies |
+| __0.0.4__ | __final__ | fixed issue with aquaapi dependency |
+| __0.0.5__ | __a1__ | fixed readme to point to md file; adjusting snyk |
+| __0.0.5__ | __final__ | tested and released |
+
+### Warnings
 
 Use at your own risk!!!
 
 # Security Policy
 
 ## Supported Versions
 
 Use this section to tell people about which versions of your project are
 currently being supported with security updates.
 
 | Version | Supported          |
 | ------- | ------------------ |
-| 0.0.x   | :white_check_mark: |
+| 0.0.x   | &check; |
 
 ## Reporting a Vulnerability
 
 Use this section to tell people how to report a vulnerability.
 
 Tell them where to go, how often they can expect to get an update on a
 reported vulnerability, what to expect if the vulnerability is accepted or
```

### Comparing `aquasec-cli-0.0.4/README.md` & `aquasec-cli-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 ```
 
 ## Usage
 
 __Help Menu of all Groups:__
 
 ```bash
-aquasec-cli  --help    
+>>> aquasec-cli --help
 Usage: aquasec-cli [OPTIONS] COMMAND [ARGS]...
 
   AquaSec CLI tool to manage AquaSec Tenant
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  delapi   Deletes created API Auth
-  initapi  Initializes API Auth
+  delete   Deletes created API Auth
+  init     Initializes API Auth
   reports  Generate CIS Bench Reports
 ```
 
 __NOTE:__ Each subcommand has a help menu to assist with the calls being made. This project relies on the yaml or localized configurations being help as they are not passed in the commands as of this release.
 
 __Create API Auth Token:__
 
@@ -36,29 +36,34 @@
 Initializing API
 INFO    : Created WorkloadAuth Token for URL https://1234abcff1.cloud.aquasec.com
 ```
 
 __Run Report:__
 
 ```bash
-aquasec-cli  reports --report_type kube_bench --report_location /Users/username/var/tmp
+aquasec-cli  reports --report_type kube_bench --report_location /var/tmp
 Report completed Saving
-Report written out to /Users/username/var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
+Report written out to /var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
 ```
 
 __Delete API Auth:__
 
 ```bash
 >>> aquasec-cli delete                                              
 Are you sure you want to delete the auth api token? [y/N]: y
 Deleted Auth
 ```
 
 ## Release Info
 
+### v0.0.5
+
+* Updated Readme and changed type from RST to MD
+* Reverted snyk workflow file
+
 ### v0.0.4
 
 * fixed issue with broken aquasec-api v0.0.3
 
 ### v0.0.3
 
 * Fixed installation and dependencies
@@ -76,11 +81,14 @@
 | __0.0.2__ | __a1__ | issues with dataclasses getting installed under normal condition |
 | __0.0.2__ | __final__ | tested in pytest and seems to now accept the dataclass |
 | __0.0.3__ | __a1__ | issues with dataclasses and now yaml getting installed under normal condition |
 | __0.0.3__ | __a3__ | migrating to toml and setup.cfg |
 | __0.0.3__ | __a4__ | cleaned up utils and updated snyk to confirm pass locally; added to git ignore |
 | __0.0.3__ | __a5__ | setup.cfg issues wiht pip |
 | __0.0.3__ | __final__ | found issue with toml and other dependencies |
+| __0.0.4__ | __final__ | fixed issue with aquaapi dependency |
+| __0.0.5__ | __a1__ | fixed readme to point to md file; adjusting snyk |
+| __0.0.5__ | __final__ | tested and released |
 
 ### Warnings
 
 Use at your own risk!!!
```

### Comparing `aquasec-cli-0.0.4/README.rst` & `aquasec-cli-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.4/aquasec_cli/commands/api.py` & `aquasec-cli-0.0.5/aquasec_cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.4/aquasec_cli/commands/report.py` & `aquasec-cli-0.0.5/aquasec_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.4/aquasec_cli/utils.py` & `aquasec-cli-0.0.5/aquasec_cli/utils.py`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.4/aquasec_cli.egg-info/PKG-INFO` & `aquasec-cli-0.0.5/aquasec_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Aqua Security cli
 Author: atav928
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,117 +682,119 @@
 Project-URL: repository, https://github.com/atav928/aquasec-cli
 Keywords: aquasec,aqua security,workload protection
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-aquasec-cli
-===========
+# aquasec-cli
 
 Aqua Security CLI
 
-Installation
-------------
+## Installation
 
-.. code:: bash
+```bash
+>>> python -m pip install aquasec-cli
+```
 
-   >>> python -m pip install aquasec-cli
+## Usage
 
-Usage
------
+__Help Menu of all Groups:__
 
-**Help Menu of all Groups:**
+```bash
+>>> aquasec-cli --help
+Usage: aquasec-cli [OPTIONS] COMMAND [ARGS]...
 
-.. code:: bash
+  AquaSec CLI tool to manage AquaSec Tenant
 
-   aquasec-cli  --help    
-   Usage: aquasec-cli [OPTIONS] COMMAND [ARGS]...
+Options:
+  --help  Show this message and exit.
 
-     AquaSec CLI tool to manage AquaSec Tenant
+Commands:
+  delete   Deletes created API Auth
+  init     Initializes API Auth
+  reports  Generate CIS Bench Reports
+```
 
-   Options:
-     --help  Show this message and exit.
+__NOTE:__ Each subcommand has a help menu to assist with the calls being made. This project relies on the yaml or localized configurations being help as they are not passed in the commands as of this release.
 
-   Commands:
-     delapi   Deletes created API Auth
-     initapi  Initializes API Auth
-     reports  Generate CIS Bench Reports
+__Create API Auth Token:__
 
-**NOTE:** Each subcommand has a help menu to assist with the calls being
-made. This project relies on the yaml or localized configurations being
-help as they are not passed in the commands as of this release.
+```bash
+>>> aquasec-cli init --csp_roles="Auditor" --csp_roles="Admin" --endpoints="Any"
+Initializing API
+INFO    : Created WorkloadAuth Token for URL https://1234abcff1.cloud.aquasec.com
+```
 
-**Create API Auth Token:**
+__Run Report:__
 
-.. code:: bash
+```bash
+aquasec-cli  reports --report_type kube_bench --report_location /var/tmp
+Report completed Saving
+Report written out to /var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
+```
 
-   >>> aquasec-cli init --csp_roles="Auditor" --csp_roles="Admin" --endpoints="Any"
-   Initializing API
-   INFO    : Created WorkloadAuth Token for URL https://1234abcff1.cloud.aquasec.com
+__Delete API Auth:__
 
-**Run Report:**
+```bash
+>>> aquasec-cli delete                                              
+Are you sure you want to delete the auth api token? [y/N]: y
+Deleted Auth
+```
 
-.. code:: bash
+## Release Info
 
-   aquasec-cli  reports --report_type kube_bench --report_location /Users/username/var/tmp
-   Report completed Saving
-   Report written out to /Users/adamt/var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
+### v0.0.5
 
-**Delete API Auth:**
+* Updated Readme and changed type from RST to MD
+* Reverted snyk workflow file
 
-.. code:: bash
+### v0.0.4
 
-   >>> aquasec-cli delete                                              
-   Are you sure you want to delete the auth api token? [y/N]: y
-   Deleted Auth
+* fixed issue with broken aquasec-api v0.0.3
 
-Release Info
-------------
+### v0.0.3
 
-v0.0.2
-~~~~~~
+* Fixed installation and dependencies
+* locked down dependencies
+* added toml and setup.cfg to support furture installations
 
--  Bug fix with requirements
+### v0.0.2
 
-Version
--------
+* Bug fix with requirements
 
-+-------------------------+-----------------+-------------------------+
-| Version                 | Build           | Changes                 |
-+=========================+=================+=========================+
-| **0.0.2**               | **a1**          | issues with dataclasses |
-|                         |                 | getting installed under |
-|                         |                 | normal condition        |
-+-------------------------+-----------------+-------------------------+
-| **0.0.2**               | **final**       | tested in pytest and    |
-|                         |                 | seems to now accept the |
-|                         |                 | dataclass               |
-+-------------------------+-----------------+-------------------------+
-| **0.0.3**               | **a1**          | issues with dataclasses |
-|                         |                 | and now yaml getting    |
-|                         |                 | installed under normal  |
-|                         |                 | condition               |
-+-------------------------+-----------------+-------------------------+
+## Version
 
-Warnings
-~~~~~~~~
+| Version | Build | Changes |
+| ------- | ----- | ------- |
+| __0.0.2__ | __a1__ | issues with dataclasses getting installed under normal condition |
+| __0.0.2__ | __final__ | tested in pytest and seems to now accept the dataclass |
+| __0.0.3__ | __a1__ | issues with dataclasses and now yaml getting installed under normal condition |
+| __0.0.3__ | __a3__ | migrating to toml and setup.cfg |
+| __0.0.3__ | __a4__ | cleaned up utils and updated snyk to confirm pass locally; added to git ignore |
+| __0.0.3__ | __a5__ | setup.cfg issues wiht pip |
+| __0.0.3__ | __final__ | found issue with toml and other dependencies |
+| __0.0.4__ | __final__ | fixed issue with aquaapi dependency |
+| __0.0.5__ | __a1__ | fixed readme to point to md file; adjusting snyk |
+| __0.0.5__ | __final__ | tested and released |
+
+### Warnings
 
 Use at your own risk!!!
 
 # Security Policy
 
 ## Supported Versions
 
 Use this section to tell people about which versions of your project are
 currently being supported with security updates.
 
 | Version | Supported          |
 | ------- | ------------------ |
-| 0.0.x   | :white_check_mark: |
+| 0.0.x   | &check; |
 
 ## Reporting a Vulnerability
 
 Use this section to tell people how to report a vulnerability.
 
 Tell them where to go, how often they can expect to get an update on a
 reported vulnerability, what to expect if the vulnerability is accepted or
```

### Comparing `aquasec-cli-0.0.4/aquasec_cli.egg-info/SOURCES.txt` & `aquasec-cli-0.0.5/aquasec_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.4/pyproject.toml` & `aquasec-cli-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "aquasec-cli"
 authors = [
     {name = "atav928", email = "dev@tavnets.com"},
 ]
 description = "Aqua Security cli"
 requires-python = ">=3.8"
 keywords = ['aquasec', 'aqua security', 'workload protection']
-license = {file = "LICENSE"}
+license = {file = "LICENSE", content-type = "text"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "aquasec-api==0.0.2",
     "click>=8.1.3",
     "dataclasses>=0.6",
@@ -27,12 +27,12 @@
 [project.scripts]
 aquasec-cli = "aquasec_cli.main:cli"
 
 [project.urls]
 repository = "https://github.com/atav928/aquasec-cli"
 
 [tool.setuptools.dynamic]
-readme = {file = ["README.rst", "SECURITY.md"], content-type = "text/markdown"}
+readme = {file = ["README.md", "SECURITY.md"], content-type = "text/markdown"}
 version = {attr = "aquasec_cli.__version__"}
 
 [tools.setuptools.packages]
 find = {}
```

### Comparing `aquasec-cli-0.0.4/setup.cfg` & `aquasec-cli-0.0.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [metadata]
 name = aquasec-cli
 version = attr: aquasec_cli.__version__
 author = atav928
 description = Aqua Security cli
 author_email = dev@tavnets.com
 keywords = aquasec, aqua security, workload protection
-long_description = file: README.md, SECURITY.md, LICENSE
+long_description = file: README.md, SECURITY.md
 long_description_content_type = text/markdown
 license = GNU
+license_files = LICENSE
 
 [options]
 python_requires = >3.8, <4
 include_package_data = True
 packages = find:
 install_requires = 
 	aquasec-api == 0.0.2
```

