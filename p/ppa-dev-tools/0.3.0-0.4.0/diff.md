# Comparing `tmp/ppa-dev-tools-0.3.0.tar.gz` & `tmp/ppa-dev-tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppa-dev-tools-0.3.0.tar", last modified: Fri Oct 28 07:29:17 2022, max compression
+gzip compressed data, was "ppa-dev-tools-0.4.0.tar", last modified: Thu Apr 27 02:39:45 2023, max compression
```

## Comparing `ppa-dev-tools-0.3.0.tar` & `ppa-dev-tools-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,58 @@
-drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2022-10-28 07:29:17.724177 ppa-dev-tools-0.3.0/
--rw-rw-r--   0 bryce     (1000) bryce     (1000)      174 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/AUTHORS.md
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     1292 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/INSTALL.md
--rw-rw-r--   0 bryce     (1000) bryce     (1000)    17987 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/LICENSE.GPLv2+
--rw-rw-r--   0 bryce     (1000) bryce     (1000)       36 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/MANIFEST.in
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     2557 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/NEWS.md
--rw-rw-r--   0 bryce     (1000) bryce     (1000)    23882 2022-10-28 07:29:17.724177 ppa-dev-tools-0.3.0/PKG-INFO
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     2237 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/README
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     2237 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/README.md
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     2747 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/RELEASING.md
--rw-rw-r--   0 bryce     (1000) bryce     (1000)      135 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/TESTING.md
-drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2022-10-28 07:29:17.724177 ppa-dev-tools-0.3.0/ppa/
--rw-rw-r--   0 bryce     (1000) bryce     (1000)        0 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/__init__.py
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)      156 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/_version.py
--rw-rw-r--   0 bryce     (1000) bryce     (1000)      689 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/constants.py
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     1152 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/debug.py
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     1023 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/io.py
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)     7993 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/job.py
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     4648 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/lp.py
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)    15334 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/ppa.py
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)     4421 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/ppa_group.py
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     3090 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/processes.py
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)     9276 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/result.py
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)     2953 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/subtest.py
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     4354 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/text.py
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)     3587 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/ppa/trigger.py
-drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2022-10-28 07:29:17.724177 ppa-dev-tools-0.3.0/ppa_dev_tools.egg-info/
--rw-rw-r--   0 bryce     (1000) bryce     (1000)    23882 2022-10-28 07:29:17.000000 ppa-dev-tools-0.3.0/ppa_dev_tools.egg-info/PKG-INFO
--rw-rw-r--   0 bryce     (1000) bryce     (1000)      485 2022-10-28 07:29:17.000000 ppa-dev-tools-0.3.0/ppa_dev_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 bryce     (1000) bryce     (1000)        1 2022-10-28 07:29:17.000000 ppa-dev-tools-0.3.0/ppa_dev_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 bryce     (1000) bryce     (1000)        4 2022-10-28 07:29:17.000000 ppa-dev-tools-0.3.0/ppa_dev_tools.egg-info/top_level.txt
--rw-rw-r--   0 bryce     (1000) bryce     (1000)     1160 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/pyproject.toml
-drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2022-10-28 07:29:17.724177 ppa-dev-tools-0.3.0/scripts/
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)    26879 2022-10-28 07:29:03.000000 ppa-dev-tools-0.3.0/scripts/ppa
--rw-rw-r--   0 bryce     (1000) bryce     (1000)      201 2022-10-28 07:29:17.724177 ppa-dev-tools-0.3.0/setup.cfg
--rwxrwxr-x   0 bryce     (1000) bryce     (1000)     2324 2022-10-28 07:29:02.000000 ppa-dev-tools-0.3.0/setup.py
+drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2023-04-27 02:39:45.046559 ppa-dev-tools-0.4.0/
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)      174 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/AUTHORS.md
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     1337 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/INSTALL.md
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)    17987 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/LICENSE.GPLv2+
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)       36 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/MANIFEST.in
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     4085 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/NEWS.md
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)    24897 2023-04-27 02:39:45.046559 ppa-dev-tools-0.4.0/PKG-INFO
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     3277 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/README
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     3277 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/README.md
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     2662 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/RELEASING.md
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)      135 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/TESTING.md
+drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2023-04-27 02:39:45.042559 ppa-dev-tools-0.4.0/ppa/
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)        0 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/__init__.py
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)      156 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/_version.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     8055 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/binary_package.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     1455 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/constants.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     1152 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/debug.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     7776 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/dict.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     1023 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/io.py
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)     7993 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/job.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     5080 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/lp.py
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)    21343 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/ppa.py
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)     4349 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/ppa_group.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     3090 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/processes.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     3545 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/repository.py
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)     9494 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/result.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)    10623 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/source_package.py
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)     3039 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/subtest.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)    11851 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/suite.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     4472 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/text.py
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)     4162 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/ppa/trigger.py
+drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2023-04-27 02:39:45.042559 ppa-dev-tools-0.4.0/ppa_dev_tools.egg-info/
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)    24897 2023-04-27 02:39:45.000000 ppa-dev-tools-0.4.0/ppa_dev_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)      920 2023-04-27 02:39:45.000000 ppa-dev-tools-0.4.0/ppa_dev_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)        1 2023-04-27 02:39:45.000000 ppa-dev-tools-0.4.0/ppa_dev_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)        4 2023-04-27 02:39:45.000000 ppa-dev-tools-0.4.0/ppa_dev_tools.egg-info/top_level.txt
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     1160 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/pyproject.toml
+drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2023-04-27 02:39:45.042559 ppa-dev-tools-0.4.0/scripts/
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)    35106 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/scripts/ppa
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)      201 2023-04-27 02:39:45.046559 ppa-dev-tools-0.4.0/setup.cfg
+-rwxrwxr-x   0 bryce     (1000) bryce     (1000)     2324 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/setup.py
+drwxrwxr-x   0 bryce     (1000) bryce     (1000)        0 2023-04-27 02:39:45.046559 ppa-dev-tools-0.4.0/tests/
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     4725 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_binary_package.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     3922 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_dict.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)      893 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_io.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     3725 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_job.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     4843 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_lp.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     2449 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_ppa.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     2479 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_ppa_group.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     1455 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_repository.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     2045 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_result.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)    21989 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_scripts_ppa.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     2944 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_source_package.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     2443 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_subtest.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)    22931 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_suite.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     1316 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_text.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)     3203 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_trigger.py
+-rw-rw-r--   0 bryce     (1000) bryce     (1000)      958 2023-04-27 02:39:34.000000 ppa-dev-tools-0.4.0/tests/test_version.py
```

### Comparing `ppa-dev-tools-0.3.0/INSTALL.md` & `ppa-dev-tools-0.4.0/INSTALL.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 The prerequisites for ppa-dev-tools can be satisified either through
 PIP, or on Ubuntu 20.04-ish via the packaging system.
 
 These modules are required:
 
   * appdirs
+  * apt_pkg
   * debian.deb822
+  * distro_info
   * launchpadlib
   * lazr.restfulclient
   * setuptools
   * software-properties
   * yaml or ruamel.yaml
 
 
 ### DEB ###
 
 A PPA with .deb packages are available for Ubuntu.
 
-  $ sudo add-apt-repository -yus ppa:bryce/ppa-dev-tools
+  $ sudo add-apt-repository --yes --enable-source ppa:bryce/ppa-dev-tools
   $ sudo apt-get install ppa-dev-tools
 
 
 ### PIP ###
 
 Alternatively, the package and its dependencies can be satisfied via PIP
 for a user installation:
```

### Comparing `ppa-dev-tools-0.3.0/LICENSE.GPLv2+` & `ppa-dev-tools-0.4.0/LICENSE.GPLv2+`

 * *Files identical despite different names*

### Comparing `ppa-dev-tools-0.3.0/NEWS.md` & `ppa-dev-tools-0.4.0/NEWS.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+# 0.4.0 #
+
+Reverse dependencies, build dependencies, and installation dependencies
+can be identified for a given source package using cached APT
+information.  This list of packages will be used to generate lists of
+autopkgtest triggers, which when run should help identify issues that
+could get flagged in Britney2 runs.  While similar to functionality
+provided by Bileto+Britney2, it is a lighterweight facsimile which
+doesn't handle special cases so should not be considered an equivalent,
+just as a preliminary screen to catch basic issues.
+
+For now, users will need to create and maintain this cache by hand
+(automatic caching is planned for 0.5).  See the README for a suggested
+rsync command to do this.
+
+In addition, The `ppa set` command now supports a number of new command
+line options.  `--ppa-dependencies` allows you to specify that your PPA
+can use the contents of one or more other PPAs to satisfy build
+dependencies.  The `--architectures` option now has some related options
+`--all-architectures` and `--default-architectures` for "Give me
+everything" and "Just the usual", respectively.  The `--enable` and
+`--disable` arguments control whether packages can be uploaded to the
+PPA to build.
+
+All of the options supported by `ppa set` can also be specified to `ppa
+create` to allow specifying them at creation time.
+
+Beyond these two features, notable bugfixes address problems with Ubuntu
+release specification, improvements to the `ppa tests` output, and
+various idiosyncrasies with command line arguments.
+
+
 # 0.3.0 Release #
 
 Autopkgtest trigger action URLs are printed for packages in the PPA when
 running the `ppa tests` command.  Both plain and 'all-proposed' style
 triggers are displayed.  These can be loaded in a web browser by someone
 with core-dev permissions to start the test runs.  `ppa tests` can then
 be re-run to check on the tests status and results.
```

### Comparing `ppa-dev-tools-0.3.0/PKG-INFO` & `ppa-dev-tools-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppa-dev-tools
-Version: 0.3.0
+Version: 0.4.0
 Summary: command line client for managing PPAs in Launchpad
 Home-page: https://launchpad.net/ppa-dev-tools
 Author: Bryce W. Harrington
 Author-email: Bryce Harrington <bryce@canonical.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
@@ -355,15 +355,14 @@
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.GPLv2+
-License-File: AUTHORS.md
 
 Ppa Dev Tools
 =============
 
 ppa is a command line client for managing PPAs in Launchpad.
 
 This primarily focuses on functionality needed by owners of PPAs, to
@@ -446,7 +445,34 @@
   - Tilix 3.26 (VTE 0.50)
   - Terminator 2.0
 
 This is not a comprehensive list, and likely will lengthen swiftly.
 Meanwhile, if you have a non-supporting browser, the --show-urls option
 can be passed to `ppa tests` to make it display the raw URLs that can be
 manually cut and pasted into your web browser.
+
+
+Autopkgtesting Reverse-dependencies
+-----------------------------------
+
+In addition to creating trigger URLs for running your package's
+autopkgtest, it is also possible to do the same for everything dependent
+on your package.  These other packages are termed 'reverse
+dependencies', aka 'rdepends'.  To generate these URLs, just include the
+'--show-rdepends' option in your command line.  For example:
+
+```
+$ ppa tests --show-rdepends ppa:my-name/my-ppa
+```
+
+The `ppa` command calculates the dependency trees using information from
+the Apt archive, which needs to be cached locally.  Only the index
+information is needed, not a complete mirror.  You can generate (and
+refresh) a dists-only mirror thusly:
+
+  $ mkdir {LOCAL_REPOSITORY_PATH}
+  $ rsync -va \\
+      --exclude={{'*/installer*','*/i18n/*','*/uefi/*','*/Contents*','*/by-hash/*','*tar.gz'}} \\
+      rsync://archive.ubuntu.com/ubuntu/dists {LOCAL_REPOSITORY_PATH}
+
+It's recommended to run the rsync command as a cronjob to keep your
+repository up to date as often as desired.
```

### Comparing `ppa-dev-tools-0.3.0/README` & `ppa-dev-tools-0.4.0/README`

 * *Files 22% similar despite different names*

```diff
@@ -83,7 +83,34 @@
   - Tilix 3.26 (VTE 0.50)
   - Terminator 2.0
 
 This is not a comprehensive list, and likely will lengthen swiftly.
 Meanwhile, if you have a non-supporting browser, the --show-urls option
 can be passed to `ppa tests` to make it display the raw URLs that can be
 manually cut and pasted into your web browser.
+
+
+Autopkgtesting Reverse-dependencies
+-----------------------------------
+
+In addition to creating trigger URLs for running your package's
+autopkgtest, it is also possible to do the same for everything dependent
+on your package.  These other packages are termed 'reverse
+dependencies', aka 'rdepends'.  To generate these URLs, just include the
+'--show-rdepends' option in your command line.  For example:
+
+```
+$ ppa tests --show-rdepends ppa:my-name/my-ppa
+```
+
+The `ppa` command calculates the dependency trees using information from
+the Apt archive, which needs to be cached locally.  Only the index
+information is needed, not a complete mirror.  You can generate (and
+refresh) a dists-only mirror thusly:
+
+  $ mkdir {LOCAL_REPOSITORY_PATH}
+  $ rsync -va \\
+      --exclude={{'*/installer*','*/i18n/*','*/uefi/*','*/Contents*','*/by-hash/*','*tar.gz'}} \\
+      rsync://archive.ubuntu.com/ubuntu/dists {LOCAL_REPOSITORY_PATH}
+
+It's recommended to run the rsync command as a cronjob to keep your
+repository up to date as often as desired.
```

### Comparing `ppa-dev-tools-0.3.0/README.md` & `ppa-dev-tools-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -83,7 +83,34 @@
   - Tilix 3.26 (VTE 0.50)
   - Terminator 2.0
 
 This is not a comprehensive list, and likely will lengthen swiftly.
 Meanwhile, if you have a non-supporting browser, the --show-urls option
 can be passed to `ppa tests` to make it display the raw URLs that can be
 manually cut and pasted into your web browser.
+
+
+Autopkgtesting Reverse-dependencies
+-----------------------------------
+
+In addition to creating trigger URLs for running your package's
+autopkgtest, it is also possible to do the same for everything dependent
+on your package.  These other packages are termed 'reverse
+dependencies', aka 'rdepends'.  To generate these URLs, just include the
+'--show-rdepends' option in your command line.  For example:
+
+```
+$ ppa tests --show-rdepends ppa:my-name/my-ppa
+```
+
+The `ppa` command calculates the dependency trees using information from
+the Apt archive, which needs to be cached locally.  Only the index
+information is needed, not a complete mirror.  You can generate (and
+refresh) a dists-only mirror thusly:
+
+  $ mkdir {LOCAL_REPOSITORY_PATH}
+  $ rsync -va \\
+      --exclude={{'*/installer*','*/i18n/*','*/uefi/*','*/Contents*','*/by-hash/*','*tar.gz'}} \\
+      rsync://archive.ubuntu.com/ubuntu/dists {LOCAL_REPOSITORY_PATH}
+
+It's recommended to run the rsync command as a cronjob to keep your
+repository up to date as often as desired.
```

### Comparing `ppa-dev-tools-0.3.0/RELEASING.md` & `ppa-dev-tools-0.4.0/RELEASING.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,86 +3,88 @@
 
 Before you start
 ----------------
 
 * Update local Git repository to the current `main` tip.  For a
   maintenance release (e.g. version 1.2.3), update to the current
   `stable-1.2` tip, instead.
+
 * Commit everything that needs included in the release
+
 * Doublecheck all new dependencies are specified in packaging
-  $ grep -h import */* | sed 's/    //' | grep -vE '(import|from) (ppa|\.)' | sort -u 
+  $ grep -h import */* | sed 's/    //' | grep -vE '(import|from) (ppa|\.)' | sort -u
+
 * Doublecheck the INSTALL.md file is still up to date
+
 * Verify the build system works without errors
   $ make build
+
 * Verify the testsuite, lint, flake, etc. passes
   $ make check
   $ make coverage
+
 * Verify the snapcraft config is ready
   $ snapcraft --debug
   $ rm *.snap
+
 * Cleanup
-  * make clean
-  * git status --ignored
+  $ make clean
+  $ git status --ignored
+
 * Write an entry in NEWS.md file with release notes
 
-Prepare and commit files
-------------------------
 
+Generate the source release
+---------------------------
+
+* Set the version
   $ export VERSION="X.Y.Z"
   $ make set-release-version
+
+* Add the release collateral
   $ git commit NEWS.md ppa/_version.py pyproject.toml snap/snapcraft.yaml -m "Releasing ${VERSION}"
   $ git tag -a -m "PPA Dev Tools ${VERSION}" "v${VERSION}"
-  $ git push origin main "v${VERSION}"
-
 
-Create the release directory
-----------------------------
+* Push the release
+  $ git push origin main "v${VERSION}"
 
+* Create the release directory
   $ cp -ir ../$(basename $(pwd)) ../Releases/ppa-dev-tools-${VERSION}/
   $ cd ../Releases/ppa-dev-tools-${VERSION}
 
-
-Generate the release tarball
-----------------------------
-
+* Generate the release tarball
   $ make build
   $ python3 -m twine upload --verbose --repository pypi dist/*-${VERSION}*
 
 
 Generate the debian package
 ---------------------------
 
-    Set to latest distro release, and add changelog entry for "New release"
-    $ dch -v "${VERSION}"
+* Set to latest distro release, and add changelog entry for "New release"
+  $ dch -v "${VERSION}"
+  $ debuild -S -sa
+  $ dput ppa:bryce/ppa-dev-tools ../ppa-dev-tools_${VERSION}_source.changes
+
+* Repeat for each LTS release, with version set to ${VERSION}~YY.MM.N
+  and changelog entry "Backport for ${codename}"
+  $ dput ppa:bryce/ppa-dev-tools ../ppa-dev-tools_${VERSION}~YY.MM.N_source.changes
 
-    $ debuild -S -sa
-    $ dput ppa:bryce/ppa-dev-tools ../ppa-dev-tools_${VERSION}_source.changes
-
-    Repeat for each LTS release, with version set to ${VERSION}~YY.MM.N
-    and changelog entry "Backport for ${codename}"
-
-    $ dput ppa:bryce/ppa-dev-tools ../ppa-dev-tools_${VERSION}~YY.MM.N_source.changes
 
 Generate the snap
 -----------------
 
 * Build the snap locally
-
-  $ export SNAPCRAFT_BUILD_ENVIRONMENT_CPU=8
-  $ export SNAPCRAFT_BUILD_ENVIRONMENT_MEMORY=16G
-  $ snapcraft
+  $ make snap
 
 * Verify the snap
-
   $ sudo snap install ppa-dev-tools_<version>_amd64.snap --devmode
   ppa-dev-tools <version> installed
   $ /snap/ppa-dev-tools/current/bin/ppa --version
 
 * Push snap to the snap repository
-
   $ snapcraft login
   $ snapcraft upload --release edge *.snap
 
 * Push the tag up to the repository
 
 
 Announce release
@@ -92,10 +94,10 @@
 * Send email to appropriate list(s)
 * Update roadmap
 
 
 Return to Development
 ---------------------
 
-Add a final commit bumping the package version to a new development one
+* Add a final commit bumping the package version to a new development one
 
-Finally, a manual `git push` (including tags) is required.
+* Finally, a manual `git push` (including tags) is required.
```

### Comparing `ppa-dev-tools-0.3.0/ppa/debug.py` & `ppa-dev-tools-0.4.0/ppa/debug.py`

 * *Files identical despite different names*

### Comparing `ppa-dev-tools-0.3.0/ppa/io.py` & `ppa-dev-tools-0.4.0/ppa/io.py`

 * *Files identical despite different names*

### Comparing `ppa-dev-tools-0.3.0/ppa/job.py` & `ppa-dev-tools-0.4.0/ppa/job.py`

 * *Files identical despite different names*

### Comparing `ppa-dev-tools-0.3.0/ppa/lp.py` & `ppa-dev-tools-0.4.0/ppa/lp.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,24 +35,32 @@
     ROOT_URL = 'https://launchpad.net/'
     API_ROOT_URL = 'https://api.launchpad.net/devel/'
     BUGS_ROOT_URL = 'https://bugs.launchpad.net/'
     CODE_ROOT_URL = 'https://code.launchpad.net/'
 
     _real_instance = None
 
-    def __init__(self, application_name, service=Launchpad):
+    def __init__(self, application_name, service=Launchpad, staging=False):
         """Create a Launchpad service object."""
         self._app_name = application_name
         self._service = service
+        if staging:
+            self._service_root = 'qastaging'
+            self.ROOT_URL = 'https://qastaging.launchpad.net/'
+            self.API_ROOT_URL = 'https://api.qastaging.launchpad.net/devel/'
+            self.BUGS_ROOT_URL = 'https://bugs.qastaging.launchpad.net/'
+            self.CODE_ROOT_URL = 'https://code.qastaging.launchpad.net/'
+        else:
+            self._service_root = 'production'
 
     def _get_instance(self):
         """Authenticate to Launchpad."""
         return self._service.login_with(
             application_name=self._app_name,
-            service_root='production',
+            service_root=self._service_root,
             allow_access_levels=['WRITE_PRIVATE'],
             version='devel',  # Need devel for copyPackage.
         )
 
     @property
     def _instance(self):
         """Cache LP object."""
```

### Comparing `ppa-dev-tools-0.3.0/ppa/ppa.py` & `ppa-dev-tools-0.4.0/ppa/ppa.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 #
 # Released under GNU GPLv2 or later, read the file 'LICENSE.GPLv2+' for
 # more information.
 
 """A wrapper around a Launchpad Personal Package Archive object."""
 
 import re
+import sys
 
 from functools import lru_cache
-from lazr.restfulclient.errors import BadRequest, NotFound
+from lazr.restfulclient.errors import BadRequest, NotFound, Unauthorized
+
+from .constants import URL_AUTOPKGTEST
+from .io import open_url
+from .job import (get_waiting, get_running)
 
 
 class PpaDoesNotExist(BaseException):
     """Exception indicating a requested PPA could not be found."""
 
     def __init__(self, ppa_name, team_name, message=None):
         """Initializes the exception object.
@@ -67,24 +72,24 @@
         self.team_name = team_name
         if ppa_description is None:
             self.ppa_description = ''
         else:
             self.ppa_description = ppa_description
         self._service = service
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Machine-parsable unique representation of object.
 
         :rtype: str
         :returns: Official string representation of the object.
         """
         return (f'{self.__class__.__name__}('
                 f'ppa_name={self.ppa_name!r}, team_name={self.team_name!r})')
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Returns a displayable string identifying the PPA.
 
         :rtype: str
         :returns: Displayable representation of the PPA.
         """
         return f"{self.team_name}/{self.name}"
 
@@ -93,14 +98,16 @@
     def archive(self):
         """Retrieves the LP Archive object from the Launchpad service.
 
         :rtype: archive
         :returns: The Launchpad archive object.
         :raises PpaDoesNotExist: Raised if a PPA does not exist in Launchpad.
         """
+        if not self._service:
+            raise AttributeError("Ppa object not connected to the Launchpad service")
         try:
             owner = self._service.people[self.team_name]
             return owner.getPPAByName(name=self.ppa_name)
         except NotFound:
             raise PpaDoesNotExist(self.ppa_name, self.team_name)
 
     @lru_cache
@@ -134,15 +141,15 @@
     @property
     def url(self):
         """The HTTP url for the PPA in Launchpad.
 
         :rtype: str
         :returns: The url of the PPA.
         """
-        return "https://launchpad.net/~{}/+archive/ubuntu/{}".format(self.team_name, self.ppa_name)
+        return self.archive.web_link
 
     @property
     def description(self):
         """The description body for the PPA.
 
         :rtype: str
         :returns: The description body for the PPA.
@@ -165,45 +172,111 @@
         retval = a.lp_save()
         print("setting desc to '{}'".format(description))
         print("desc is now '{}'".format(self.archive.description))
         return retval and self.archive.description == description
 
     @property
     @lru_cache
-    def architectures(self):
+    def publish(self):
+        return self.archive.publish
+
+    def set_publish(self, publish: bool):
+        if publish is None:
+            return
+        self.archive.publish = publish
+        self.archive.lp_save()
+
+    @property
+    @lru_cache
+    def architectures(self) -> list[str]:
         """Returns the architectures configured to build packages in the PPA.
 
         :rtype: list[str]
         :returns: List of architecture names, or None on error.
         """
         try:
             return [proc.name for proc in self.archive.processors]
         except PpaDoesNotExist as e:
-            print(e)
+            sys.stderr.write(e)
             return None
 
-    def set_architectures(self, architectures):
+    def set_architectures(self, architectures: list[str]) -> bool:
         """Configures the architectures used to build packages in the PPA.
 
         Note that some architectures may only be available upon request
         from Launchpad administrators.  ppa.constants.ARCHES_PPA is a
         list of standard architectures that don't require permissions.
 
+        :param list[str] architectures: List of processor architecture names
         :rtype: bool
-        :returns: True if architectures could be set, False on error.
+        :returns: True if architectures could be set, False on error or
+            if no architectures were specified.
         """
-        uri_base = "https://api.launchpad.net/devel/+processors/{}"
-        procs = [uri_base.format(arch) for arch in architectures]
+        if not architectures:
+            return False
+        base = self._service.API_ROOT_URL.rstrip('/')
+        procs = []
+        for arch in architectures:
+            procs.append(f'{base}/+processors/{arch}')
         try:
             self.archive.setProcessors(processors=procs)
             return True
         except PpaDoesNotExist as e:
-            print(e)
+            sys.stderr.write(e)
             return False
 
+    @property
+    @lru_cache
+    def dependencies(self) -> list[str]:
+        """Returns the additional PPAs configured for building packages in this PPA.
+
+        :rtype: list[str]
+        :returns: List of PPA addresses
+        """
+        ppa_addresses = []
+        for dep in self.archive.dependencies:
+            ppa_dep = dep.dependency
+            ppa_addresses.append(ppa_dep.reference)
+        return ppa_addresses
+
+    def set_dependencies(self, ppa_addresses: list[str]):
+        """Configures the additional PPAs used to build packages in this PPA.
+
+        This removes any existing PPA dependencies and adds the ones
+        in the corresponding list.  If any of these new PPAs cannot be
+        found, this routine bails out without changing the current set.
+
+        :param list[str] ppa_addresses: Additional PPAs to add
+        """
+        base = self._service.API_ROOT_URL.rstrip('/')
+        new_ppa_deps = []
+        for ppa_address in ppa_addresses:
+            team_name, ppa_name = ppa_address_split(ppa_address)
+            new_ppa_dep = f'{base}/~{team_name}/+archive/ubuntu/{ppa_name}'
+            new_ppa_deps.append(new_ppa_dep)
+
+        # TODO: Remove all existing dependencies
+#        for ppa_dep in self.archive.dependencies:
+#            the_ppa.removeArchiveDependency(ppa_dep)
+
+        # TODO: Not sure what to pass here, maybe a string ala 'main'?
+        component = None
+
+        # TODO: Allow setting alternate pockets
+        # TODO: Maybe for convenience it should be same as what's set for main archive?
+        pocket = 'Release'
+
+        for ppa_dep in new_ppa_deps:
+            self.archive.addArchiveDependency(
+                component=component,
+                dependency=ppa_dep,
+                pocket=pocket)
+        # TODO: Error checking
+        #       This can throw ArchiveDependencyError if the ppa_address does not fit the_ppa
+
     def get_binaries(self, distro=None, series=None, arch=None):
         """Retrieves the binary packages available in the PPA.
 
         :param distribution distro: The Launchpad distribution object.
         :param str series: The distro's codename for the series.
         :param str arch: The hardware architecture.
         :rtype: list[binary_package_publishing_history]
@@ -354,14 +427,42 @@
             print("* Missing some builds")
             retval = True
 
         if not retval:
             print("Successfully published all builds for all architectures")
         return retval
 
+    def get_autopkgtest_waiting(self, releases):
+        """Returns iterator of queued autopkgtests for this PPA.
+
+        See get_waiting() for details
+
+        :param list[str] releases: The Ubuntu series codename(s), or None.
+        :rtype: Iterator[Job]
+        :returns: Currently waiting jobs, if any, or an empty list on error
+        """
+        response = open_url(f"{URL_AUTOPKGTEST}/queues.json", "waiting autopkgtests")
+        if response:
+            return get_waiting(response, releases=releases, ppa=str(self))
+        return []
+
+    def get_autopkgtest_running(self, releases):
+        """Returns iterator of queued autopkgtests for this PPA.
+
+        See get_running() for details
+
+        :param list[str] releases: The Ubuntu series codename(s), or None.
+        :rtype: Iterator[Job]
+        :returns: Currently running jobs, if any, or an empty list on error
+        """
+        response = open_url(f"{URL_AUTOPKGTEST}/static/running.json", "running autopkgtests")
+        if response:
+            return get_running(response, releases=releases, ppa=str(self))
+        return []
+
 
 def ppa_address_split(ppa_address, default_team=None):
     """Parse an address for a PPA into its team and name components.
 
     :param str ppa_address: A ppa name or address.
     :param str default_team: (Optional) name of team to use if missing.
     :rtype: tuple(str, str)
@@ -428,7 +529,74 @@
     :rtype: Ppa
     :returns: Specified PPA as a Ppa object.
     """
     return Ppa(
         ppa_name=config.get('ppa_name', None),
         team_name=config.get('team_name', None),
         service=lp)
+
+
+if __name__ == "__main__":
+    import pprint
+    import random
+    import string
+    from .lp import Lp
+    from .ppa_group import PpaGroup
+
+    pp = pprint.PrettyPrinter(indent=4)
+
+    print('##########################')
+    print('## Ppa class smoke test ##')
+    print('##########################')
+    print()
+
+    rndstr = str(''.join(random.choices(string.ascii_lowercase, k=6)))
+    dep_name = f'dependency-ppa-{rndstr}'
+    smoketest_ppa_name = f'test-ppa-{rndstr}'
+
+    lp = Lp('smoketest', staging=True)
+    ppa_group = PpaGroup(service=lp, name=lp.me.name)
+
+    dep_ppa = ppa_group.create(dep_name, ppa_description=dep_name)
+    the_ppa = ppa_group.create(smoketest_ppa_name, ppa_description=smoketest_ppa_name)
+    ppa_dependencies = [f'ppa:{lp.me.name}/{dep_name}']
+
+    try:
+        the_ppa.set_publish(True)
+
+        if not the_ppa.exists():
+            print("Error: PPA does not exist")
+            sys.exit(1)
+        the_ppa.set_description("This is a testing PPA and can be deleted")
+        the_ppa.set_publish(False)
+        the_ppa.set_architectures(["amd64", "arm64"])
+        the_ppa.set_dependencies(ppa_dependencies)
+
+        print()
+        print(f"name:          {the_ppa.name}")
+        print(f"address:       {the_ppa.address}")
+        print(f"str(ppa):      {the_ppa}")
+        print(f"reference:     {the_ppa.archive.reference}")
+        print(f"self_link:     {the_ppa.archive.self_link}")
+        print(f"web_link:      {the_ppa.archive.web_link}")
+        print(f"description:   {the_ppa.description}")
+        print(f"has_packages:  {the_ppa.has_packages()}")
+        print(f"architectures: {'/'.join(the_ppa.architectures)}")
+        print(f"dependencies:  {','.join(the_ppa.dependencies)}")
+        print(f"url:           {the_ppa.url}")
+        print()
+
+    except BadRequest as e:
+        print(f"Error: (BadRequest) {str(e.content.decode('utf-8'))}")
+    except Unauthorized as e:
+        print(f"Error: (Unauthorized) {e}")
+
+    answer = 'x'
+    while answer not in ['y', 'n']:
+        answer = input('Ready to cleanup (i.e. delete) temporary test PPAs? (y/n) ')
+        answer = answer[0].lower()
+
+    if answer == 'y':
+        print("  Cleaning up temporary test PPAs...")
+        the_ppa.destroy()
+        dep_ppa.destroy()
+        print("  ...Done")
```

### Comparing `ppa-dev-tools-0.3.0/ppa/ppa_group.py` & `ppa-dev-tools-0.4.0/ppa/ppa_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,24 +96,24 @@
         :param str ppa_name: Name for the PPA to create.
         :param str ppa_description: Text description of the PPA.
         :rtype: Ppa
         :returns: A Ppa object that describes the created PPA.
 
         :raises PpaAlreadyExists: Raised if a PPA by this name already exists in Launchpad.
         """
-        ppa_displayname = ''
-        if ppa_description is None:
-            ppa_description = ppa_name
-            ppa_displayname = ppa_name
+        ppa_settings = {
+            'description': ppa_description,
+            'displayname': ppa_name,
+        }
 
         try:
             self.team.createPPA(
                 name=ppa_name,
-                description=ppa_description,
-                displayname=ppa_displayname)
+                **ppa_settings
+            )
             self.team.lp_save()
         except BadRequest as e:
             if "You already have a PPA" in o2str(e.content):
                 raise PpaAlreadyExists(ppa_name, e.content)
             else:
                 raise e
```

### Comparing `ppa-dev-tools-0.3.0/ppa/processes.py` & `ppa-dev-tools-0.4.0/ppa/processes.py`

 * *Files identical despite different names*

### Comparing `ppa-dev-tools-0.3.0/ppa/result.py` & `ppa-dev-tools-0.4.0/ppa/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -235,39 +235,46 @@
 
 if __name__ == "__main__":
     import os
 
     from ppa.io import open_url
     from ppa.constants import ARCHES_AUTOPKGTEST, URL_AUTOPKGTEST
 
-    print("### Result class smoke test ###")
+    print('#############################')
+    print('## Result class smoke test ##')
+    print('#############################')
+    print()
 
+    print("Basic result")
+    print("------------")
     timestamp = time.strptime('20030201_040506', "%Y%m%d_%H%M%S")
     result_1 = Result('url-here', timestamp, 'kinetic', 'amd64', 'my-package')
+    print("* Result object:")
     print(repr(result_1))
     print(result_1)
     print()
 
     data_dir = os.path.realpath(os.path.join(os.path.dirname(__file__), "../tests/data"))
     url = f"file://{data_dir}/results-six-s390x.log.gz"
     result_2 = Result(url, timestamp, 'kinetic', 'amd64', 'my-package')
-    print("Log Head:")
+    print("* Log Head:")
     print("\n".join(result_2.log.splitlines()[0:4]))
     print()
 
     # TODO: Implement something that dumps the passing tests for given package from -proposed
     # TODO: Filter to items with only Pass, Not a regression, or No test results
 
     print("Loading live excuses data")
+    print("-------------------------")
     base_results_fmt = f"{URL_AUTOPKGTEST}/results/autopkgtest-%s-%s-%s/"
     base_results_url = base_results_fmt % ('kinetic', 'bryce', 'nginx-merge-v1.22.0-1')
     url = f"{base_results_url}?format=plain"
     response = open_url(url)
 
     for result in get_results(response, base_results_url, arches=ARCHES_AUTOPKGTEST):
         print(f"* {result}")
-        print(f"  - Triggers: " + ', '.join([str(r) for r in result.get_triggers()]))
+        print("  - Triggers: " + ', '.join([str(r) for r in result.get_triggers()]))
 
         for subtest in result.get_subtests():
             print(f"  - {subtest}")
 
         print()
```

### Comparing `ppa-dev-tools-0.3.0/ppa/subtest.py` & `ppa-dev-tools-0.4.0/ppa/subtest.py`

 * *Files 18% similar despite different names*

```diff
@@ -86,15 +86,17 @@
         :rtype: str
         :returns: Single unicode character matching the status.
         """
         return Subtest.VALUES[self.status]
 
 
 if __name__ == "__main__":
-    print("### Subtest class smoke test ###")
+    print('##############################')
+    print('## Subtest class smoke test ##')
+    print('##############################')
     print()
 
     print("Valid cases")
     print("-----------")
     print(Subtest('subtest-a   UNKNOWN'))
     print(Subtest('subtest-b   PASS'))
     print(Subtest('subtest-c   FAIL'))
```

### Comparing `ppa-dev-tools-0.3.0/ppa/text.py` & `ppa-dev-tools-0.4.0/ppa/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,8 +129,13 @@
     """
     OSC8 = "\u001b]8"
     ST = "\u001b\\"
     return f"{OSC8};;{url}{ST}{text}{OSC8};;{ST}"
 
 
 if __name__ == "__main__":
+    print('#####################')
+    print('## Text smoke test ##')
+    print('#####################')
+    print()
+
     print(ansi_hyperlink("https://launchpad.net/ppa-dev-tools", "ppa-dev-tools"))
```

### Comparing `ppa-dev-tools-0.3.0/ppa/trigger.py` & `ppa-dev-tools-0.4.0/ppa/trigger.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,45 +23,53 @@
     given series (generally to a specific version) when running
     autopkgtests for a Job.
 
     A Job can have multiple Triggers, each against a different source
     package and/or architectures, but all such Triggers must be against
     the same series as the Job itself.
     """
-    def __init__(self, package, version, arch, series, ppa=None):
+    def __init__(self, package, version, arch, series, ppa=None, test_package=None):
         """Initializes a new Trigger for a given package and version.
 
         :param str package: The source package name.
         :param str version: The version of the source package to install.
         :param str arch: The architecture for the trigger.
         :param str series: The distro release series codename.
         :param Ppa ppa: (Optional) PPA wrapper object to run tests against.
+        :param str test_package: The package to run autopkgtests from.
         """
         self.package = package
         self.version = version
         self.arch = arch
         self.series = series
         self.ppa = ppa
+        if test_package:
+            self.test_package = test_package
+        else:
+            self.test_package = package
 
     def __repr__(self) -> str:
         """Machine-parsable unique representation of object.
 
         :rtype: str
         :returns: Official string representation of the object.
         """
         return (f'{self.__class__.__name__}('
                 f'package={self.package!r}, version={self.version!r}, '
-                f'arch={self.arch!r}, series={self.series!r}, ppa={self.ppa!r})')
+                f'arch={self.arch!r}, series={self.series!r}, ppa={self.ppa!r}, '
+                f'test_package={self.test_package!r})')
 
     def __str__(self) -> str:
         """Human-readable summary of the object.
 
         :rtype: str
         :returns: Printable summary of the object.
         """
+        if self.test_package != self.package:
+            return f"({self.test_package}) {self.package}/{self.version}"
         return f"{self.package}/{self.version}"
 
     @property
     @lru_cache
     def history_url(self) -> str:
         """Renders the trigger as a URL to the job history.
 
@@ -81,15 +89,15 @@
         """Renders the trigger as a URL to start running the test.
 
         :rtype: str
         :returns: Trigger action URL
         """
         params = [
             ("release", self.series),
-            ("package", self.package),
+            ("package", self.test_package),
             ("arch", self.arch),
         ]
 
         # Trigger for the source package itself
         params.append(("trigger", f"{self.package}/{self.version}"))
 
         # TODO: Additional triggers...
@@ -98,20 +106,26 @@
         if self.ppa:
             params.append(("ppa", self.ppa))
 
         return f"{URL_AUTOPKGTEST}/request.cgi?" + urlencode(params)
 
 
 if __name__ == "__main__":
-    print("### Trigger class smoke test ###")
+    print('##############################')
+    print('## Trigger class smoke test ##')
+    print('##############################')
+    print()
 
+    print("Basic trigger")
+    print("-------------")
     trigger = Trigger('my-package', '1.2.3', 'amd64', 'kinetic')
     print(trigger)
     print(trigger.history_url)
     print(trigger.action_url)
     print()
 
+    print("* PPA trigger:")
     trigger = Trigger('my-ppa-package', '1.2.3', 'amd64', 'kinetic', 'my-ppa')
     print(trigger)
     print(trigger.history_url)
     print(trigger.action_url)
     print()
```

### Comparing `ppa-dev-tools-0.3.0/ppa_dev_tools.egg-info/PKG-INFO` & `ppa-dev-tools-0.4.0/ppa_dev_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppa-dev-tools
-Version: 0.3.0
+Version: 0.4.0
 Summary: command line client for managing PPAs in Launchpad
 Home-page: https://launchpad.net/ppa-dev-tools
 Author: Bryce W. Harrington
 Author-email: Bryce Harrington <bryce@canonical.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
@@ -355,15 +355,14 @@
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.GPLv2+
-License-File: AUTHORS.md
 
 Ppa Dev Tools
 =============
 
 ppa is a command line client for managing PPAs in Launchpad.
 
 This primarily focuses on functionality needed by owners of PPAs, to
@@ -446,7 +445,34 @@
   - Tilix 3.26 (VTE 0.50)
   - Terminator 2.0
 
 This is not a comprehensive list, and likely will lengthen swiftly.
 Meanwhile, if you have a non-supporting browser, the --show-urls option
 can be passed to `ppa tests` to make it display the raw URLs that can be
 manually cut and pasted into your web browser.
+
+
+Autopkgtesting Reverse-dependencies
+-----------------------------------
+
+In addition to creating trigger URLs for running your package's
+autopkgtest, it is also possible to do the same for everything dependent
+on your package.  These other packages are termed 'reverse
+dependencies', aka 'rdepends'.  To generate these URLs, just include the
+'--show-rdepends' option in your command line.  For example:
+
+```
+$ ppa tests --show-rdepends ppa:my-name/my-ppa
+```
+
+The `ppa` command calculates the dependency trees using information from
+the Apt archive, which needs to be cached locally.  Only the index
+information is needed, not a complete mirror.  You can generate (and
+refresh) a dists-only mirror thusly:
+
+  $ mkdir {LOCAL_REPOSITORY_PATH}
+  $ rsync -va \\
+      --exclude={{'*/installer*','*/i18n/*','*/uefi/*','*/Contents*','*/by-hash/*','*tar.gz'}} \\
+      rsync://archive.ubuntu.com/ubuntu/dists {LOCAL_REPOSITORY_PATH}
+
+It's recommended to run the rsync command as a cronjob to keep your
+repository up to date as often as desired.
```

### Comparing `ppa-dev-tools-0.3.0/pyproject.toml` & `ppa-dev-tools-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 package = "ppa-dev-tools"
 directory = "changes"
 issue_format = ""
 title_format = "ppa-dev-tools {version} ({project_date})"
 
 [project]
 name = "ppa-dev-tools"
-version = "0.3.0"
+version = "0.4.0"
 requires-python = '>=3'
 description = "command line client for managing PPAs in Launchpad"
 readme = "README.md"
 authors = [{ name= "Bryce Harrington", email = "bryce@canonical.com" }]
 license = { file = "LICENSE.GPLv2+" }
 keywords = [ 'ppa', 'archive', 'ubuntu', 'debian' ]
 classifiers = [
```

### Comparing `ppa-dev-tools-0.3.0/scripts/ppa` & `ppa-dev-tools-0.4.0/scripts/ppa`

 * *Files 19% similar despite different names*

```diff
@@ -47,87 +47,79 @@
 '''
 
 import os
 import sys
 import time
 import argparse
 from inspect import currentframe
-from distro_info import UbuntuDistroInfo, DistroDataOutdated
 from textwrap import indent
+from typing import Any
+from distro_info import UbuntuDistroInfo
 
 try:
     from ruamel import yaml
 except ImportError:
     import yaml
 
 if '__file__' in globals():
     sys.path.insert(0, os.path.realpath(
         os.path.join(os.path.dirname(os.path.realpath(__file__)), "..")))
 
 from ppa._version import __version__
 from ppa.constants import (
-    ARCHES_PPA,
+    ARCHES_PPA_ALL,
+    ARCHES_PPA_DEFAULT,
     ARCHES_AUTOPKGTEST,
     URL_AUTOPKGTEST,
+    LOCAL_REPOSITORY_PATH,
+    LOCAL_REPOSITORY_MIRRORING_DIRECTIONS,
 )
+from ppa.dict import unpack_to_dict
 from ppa.io import open_url
-from ppa.job import (
-    Job,
-    get_waiting,
-    show_waiting,
-    get_running,
-    show_running
-)
+from ppa.job import show_waiting, show_running
 from ppa.lp import Lp
 from ppa.ppa import (
     get_ppa,
     ppa_address_split,
     Ppa,
     PpaDoesNotExist
 )
 from ppa.ppa_group import PpaGroup, PpaAlreadyExists
-from ppa.result import (
-    Result,
-    get_results
-)
+from ppa.repository import Repository
+from ppa.result import get_results
 from ppa.text import o2str, ansi_hyperlink
 from ppa.trigger import Trigger
 
 import ppa.debug
 from ppa.debug import dbg, warn, error
 
 
 def UNIMPLEMENTED():
     """Marks functionality that's not yet been coded"""
     warn("[UNIMPLEMENTED]: %s()" % (currentframe().f_back.f_code.co_name))
 
 
 def load_yaml_as_dict(filename):
-    """Returns content of yaml-formatted filename as a dictionary.
+    """Returns content of yaml-formatted file as a dictionary.
 
     :rtype: dict
     :returns: Content of file as a dict object.
     """
     d = dict()
     with open(filename, 'r') as f:
         for y in yaml.safe_load_all(f.read()):
             d.update(y)
         return d
 
 
-def create_arg_parser():
-    """Sets up the command line parser object.
+def add_global_options(parser: argparse.ArgumentParser) -> None:
+    """Adds arguments to the given parser for generic options.
 
-    :rtype: argparse.ArgumentParser
-    :returns: parser object, ready to run <parser>.parse_args().
+    :param argparse.ArgumentParser parser: A parser or subparser.
     """
-    parser = argparse.ArgumentParser(
-        description=__doc__,
-        formatter_class=argparse.RawTextHelpFormatter,
-        epilog=__example__)
     parser.add_argument('-C', '--config',
                         dest='config_filename', action='store',
                         default="~/.config/ppa-dev-tools/config.yml",
                         help="Location of config file")
     parser.add_argument('-D', '--debug',
                         dest='debug', action='store_true',
                         help="Turn on general debugging")
@@ -141,95 +133,275 @@
     parser.add_argument('-v', '--verbose',
                         dest='verbose', action='store_true',
                         help="Print more information during processing")
     parser.add_argument('-q', '--quiet',
                         dest='quiet', action='store_true',
                         help="Minimize output during processing")
 
+
+def add_basic_config_options(parser: argparse.ArgumentParser) -> None:
+    """Adds to a parser the command line options to configure the PPA.
+
+    The config options are supported by the 'create' and 'set' command,
+    to allow configuring the PPA at creation time, or after, respectively.
+
+    These options represent what can be set as a user from the Launchpad
+    web interface.
+
+    :param argparse.ArgumentParser parser: A parser or subparser.
+    """
+    # Architectures
+    parser.add_argument(
+        '-a', '--arches', '--arch', '--architectures',
+        dest="architectures",
+        action='store',
+        default=None,
+        help="Comma-separated list of hardware architectures to use"
+    )
+    parser.add_argument(
+        '--all-arches', '--all-architectures',
+        dest="architectures",
+        action='store_const',
+        const=','.join(ARCHES_PPA_ALL),
+        help="Enable all available architectures for the PPA"
+    )
+    parser.add_argument(
+        '--default-arches', '--default-architectures',
+        dest="architectures",
+        action='store_const',
+        const=','.join(ARCHES_PPA_DEFAULT),
+        help="Enable all available architectures for the PPA"
+    )
+
+    # Displayname
+    parser.add_argument(
+        '--displayname',
+        dest="displayname",
+        action='store',
+        default=None,
+        help="A short title for the PPA's web page."
+    )
+
+    # Description
+    parser.add_argument(
+        '--description',
+        dest="description",
+        action='store',
+        default=None,
+        help="A short description of the archive.  URLs will be rendered as links.  (See also 'ppa desc'.)"
+    )
+
+    # Enable/Disable uploading
+    parser.add_argument(
+        '--enable',
+        dest="set_enabled",
+        action='store_true',
+        help="Accept and build packages uploaded to the PPA."
+    )
+    parser.add_argument(
+        '--disable',
+        dest="set_disabled",
+        action='store_true',
+        help="Do not accept or build packages uploaded to the PPA."
+    )
+
+    # Dependencies
+    parser.add_argument(
+        '--ppa-dependencies', '--ppa-depends',
+        dest="ppa_dependencies", action='store',
+        help="The set of other PPAs this PPA should use for satisfying build dependencies."
+    )
+
+    parser.add_argument(
+        '--publish',
+        dest="publish", action='store_true',
+        help=("Allow built packages in the PPA to be made available for download.")
+    )
+
+    parser.add_argument(
+        '--no-publish',
+        dest="publish", action='store_false',
+        help=("Do not make packages in the PPA available for download.  " +
+              "They will still be built.")
+    )
+
+
+def create_arg_parser() -> argparse.ArgumentParser:
+    """Sets up the command line parser object.
+
+    :rtype: argparse.ArgumentParser
+    :returns: parser object, ready to run <parser>.parse_args().
+    """
+    progname = "ppa"
+    parser = argparse.ArgumentParser(
+        prog=progname,
+        description=__doc__,
+        formatter_class=argparse.RawTextHelpFormatter,
+        epilog=__example__)
+    add_global_options(parser)
+
     subparser = parser.add_subparsers(dest='command')
 
     # Create Command
-    create_parser = subparser.add_parser('create', help='create help')
+    create_parser = subparser.add_parser(
+        'create',
+        argument_default=argparse.SUPPRESS,
+        help='create help',
+        prog=progname,
+    )
+    add_global_options(create_parser)
     create_parser.add_argument('ppa_name', metavar='ppa-name',
                                action='store',
                                help="Name of the PPA to be created")
-    create_parser.add_argument('-a', '--arches', '--arch', '--architectures',
-                               dest="architectures", action='store',
-                               help="Comma-separated list of hardware architectures to use")
+    add_basic_config_options(create_parser)
 
     # Desc Command
-    desc_parser = subparser.add_parser('desc', help='desc help')
+    desc_parser = subparser.add_parser(
+        'desc',
+        argument_default=argparse.SUPPRESS,
+        help='desc help',
+        prog=progname,
+    )
+    add_global_options(desc_parser)
     desc_parser.add_argument('ppa_name', metavar='ppa-name',
                              action='store',
                              help="Name of the PPA to describe")
     desc_parser.add_argument('description',
                              nargs=argparse.REMAINDER)
 
     # Destroy Command
-    destroy_parser = subparser.add_parser('destroy', help='destroy help')
+    destroy_parser = subparser.add_parser(
+        'destroy',
+        argument_default=argparse.SUPPRESS,
+        help='destroy help',
+        prog=progname,
+    )
+    add_global_options(destroy_parser)
     destroy_parser.add_argument('ppa_name', metavar='ppa-name',
                                 action='store',
                                 help="Name of the PPA to destroy")
 
     # List Command
-    list_parser = subparser.add_parser('list', help='list help')
+    list_parser = subparser.add_parser(
+        'list',
+        argument_default=argparse.SUPPRESS,
+        help='list help',
+        prog=progname,
+    )
+    add_global_options(list_parser)
     list_parser.add_argument('ppa_name', metavar='ppa-name',
                              action='store',
                              nargs='?', default='me',
                              help="Name of the PPA to list")
 
+    # Set Command
+    set_parser = subparser.add_parser(
+        'set',
+        argument_default=argparse.SUPPRESS,
+        help='set help',
+        prog=progname,
+    )
+    add_global_options(set_parser)
+    set_parser.add_argument('ppa_name', metavar='ppa-name',
+                            action='store',
+                            help="Name of the PPA to be set config values on")
+    add_basic_config_options(set_parser)
+
     # Show Command
-    show_parser = subparser.add_parser('show', help='show help')
+    show_parser = subparser.add_parser(
+        'show',
+        argument_default=argparse.SUPPRESS,
+        help='show help',
+        prog=progname,
+        )
+    add_global_options(show_parser)
     show_parser.add_argument('ppa_name', metavar='ppa-name',
                              action='store',
                              help="Name of the PPA to show")
     show_parser.add_argument('-a', '--arches', '--arch', '--architectures',
                              dest="architectures", action='store',
+                             default=None,
                              help="Comma-separated list of hardware architectures to show")
     show_parser.add_argument('-r', '--releases', '--release',
                              dest="releases", action='store',
+                             default=None,
                              help="Comma-separated list of Ubuntu release codenames to show")
     show_parser.add_argument('-p', '--packages', '--package',
                              dest="packages", action='store',
                              help="Comma-separated list of source package names to show")
 
     # Status Command
-    status_parser = subparser.add_parser('status', help='status help')
+    status_parser = subparser.add_parser(
+        'status',
+        argument_default=argparse.SUPPRESS,
+        help='status help',
+        prog=progname,
+    )
+    add_global_options(status_parser)
     status_parser.add_argument('ppa_name', metavar='ppa-name',
                                action='store',
+                               default=None,
                                help="Name of the PPA to report status of")
 
     # Tests Command
-    tests_parser = subparser.add_parser('tests', help='tests help')
+    tests_parser = subparser.add_parser(
+        'tests',
+        argument_default=argparse.SUPPRESS,
+        help='tests help',
+        prog=progname,
+    )
+    add_global_options(tests_parser)
     tests_parser.add_argument('ppa_name', metavar='ppa-name',
                               action='store',
+                              default=None,
                               help="Name of the PPA to view tests")
     tests_parser.add_argument('-a', '--arches', '--arch', '--architectures',
                               dest="architectures", action='store',
-                              help="Comma-separated list of hardware architectures to include in triggers")
+                              default=None,
+                              help="Comma-separated list of hardware architectures to include")
     tests_parser.add_argument('-r', '--releases', '--release',
                               dest="releases", action='store',
-                              help="Comma-separated list of Ubuntu release codenames to show triggers for")
+                              default=None,
+                              help="Comma-separated list of Ubuntu release codenames to show")
     tests_parser.add_argument('-p', '--packages', '--package',
                               dest="packages", action='store',
-                              help="Comma-separated list of source package names to show triggers for")
-    tests_parser.add_argument('-L', '--show-urls',
+                              default=None,
+                              help="Comma-separated list of source package names to show")
+    tests_parser.add_argument('-L', '--show-url', '--show-urls',
                               dest='show_urls', action='store_true',
+                              default=False,
                               help="Display unformatted trigger action URLs")
+    tests_parser.add_argument('--show-rdepends',
+                              dest='show_rdepends', action='store_true',
+                              default=False,
+                              help="Display test triggers for reverse dependencies")
 
     # Wait Command
-    wait_parser = subparser.add_parser('wait', help='wait help')
+    wait_parser = subparser.add_parser(
+        'wait',
+        argument_default=argparse.SUPPRESS,
+        help='wait help',
+        prog=progname,
+    )
+    add_global_options(wait_parser)
     wait_parser.add_argument('ppa_name', metavar='ppa-name',
                              action='store',
                              help="Name of the PPA to wait on")
 
     return parser
 
 
-def create_config(lp, args):
+DEFAULT_CONFIG = {
+    'debug': False,
+    'ppa_name': None,
+    'team_name': None,
+    'wait_seconds': 10.0
+    }
+
+def create_config(lp: Lp, args: argparse.Namespace) -> dict[str, Any]:
     """Creates config object by loading from file and adding args.
 
     This routine merges the command line parameter values with data
     loaded from the program's YAML formatted configuration file at
     ~/.config/ppa-dev-tools/config.yml (or as specified by the --config
     parameter).
 
@@ -237,135 +409,122 @@
     the command line args for variable settings and overrides.
 
     :param launchpadlib.service lp: The Launchpad service object.
     :param Namespace args: The parsed args from ArgumentParser.
     :rtype: dict
     :returns: dict of configuration parameters and values, or None on error
     """
-    DEFAULT_CONFIG = {
-        'debug': False,
-        'ppa_name': None,
-        'team_name': None,
-        'wait_seconds': 10.0
-        }
     config_path = os.path.expanduser(args.config_filename)
     try:
         config = load_yaml_as_dict(config_path)
     except FileNotFoundError:
         # Assume defaults
         dbg("Using default config since no config file found at {}".format(config_path))
-        config = DEFAULT_CONFIG
+        config = dict(DEFAULT_CONFIG)
 
     # Map all non-empty elements from argparse Namespace into config dict
     config.update({k: v for k, v in vars(args).items() if v})
 
     # Use defaults for any remaining parameters not yet configured
     for k, v in DEFAULT_CONFIG.items():
         config.setdefault(k, v)
 
     lp_username = None
     if lp.me:
         lp_username = lp.me.name
+    if not hasattr(args, 'ppa_name'):
+        warn("No ppa name given")
+        return None
+
     config['team_name'], config['ppa_name'] = ppa_address_split(args.ppa_name, lp_username)
     if not config['team_name'] or not config['ppa_name']:
-        warn("Invalid ppa name '{}'".format(args.ppa_name))
-        return None
+        raise ValueError("Invalid ppa name '{}'".format(args.ppa_name))
 
     if args.dry_run:
         config['dry_run'] = True
 
-    # TODO: Each subcommand should have its own args->config parser
-    # TODO: Also, loading the values from the config file will need namespaced,
+    # TODO: Loading the values from the config file will need namespaced,
     #       so e.g. create.architectures = a,b,c
-    if args.command == 'create':
-        if args.architectures is not None:
-            if args.architectures:
-                config['architectures'] = args.architectures.split(',')
-            else:
-                warn(f"Invalid architectures '{args.architectures}'")
-                return None
-    elif args.command == 'tests':
-        if args.architectures is not None:
-            if args.architectures:
-                config['architectures'] = args.architectures.split(',')
-            else:
-                warn(f"Invalid architectures '{args.architectures}'")
-                return None
-
-        if args.releases is not None:
-            if args.releases:
-                config['releases'] = args.releases.split(',')
-            else:
-                warn(f"Invalid releases '{args.releases}'")
-                return None
 
     return config
 
 
 ################
 ### Commands ###
 ################
 
-def command_create(lp, config):
+def command_create(lp: Lp, config: dict[str, str]) -> int:
     """Creates a new PPA in Launchpad.
 
     :param Lp lp: The Launchpad wrapper object.
-    :param dict config: Configuration param:value map.
+    :param dict[str, str] config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     # Take description from stdin if it's not a tty
-    description = None
-    if not sys.stdin.isatty():
+    description = config.get('description')
+    if not description and not sys.stdin.isatty():
         description = sys.stdin.read()
 
     ppa_name = config.get('ppa_name')
     if not ppa_name:
         warn("Could not determine PPA name")
         return os.EX_USAGE
 
     team_name = config.get('team_name')
     if not team_name:
         warn("Could not determine team name")
         return os.EX_USAGE
 
-    architectures = config.get('architectures', ARCHES_PPA)
+    publish = config.get('publish', None)
+
+    architectures = config.get('architectures', ARCHES_PPA_ALL)
+    if type(architectures) is str:
+        architectures = unpack_to_dict(architectures).keys()
 
     try:
         if not config.get('dry_run', False):
             ppa_group = PpaGroup(service=lp, name=team_name)
-            ppa = ppa_group.create(ppa_name, ppa_description=description)
-            ppa.set_architectures(architectures)
-            arch_str = ', '.join(ppa.architectures)
+            the_ppa = ppa_group.create(ppa_name, ppa_description=description)
+            the_ppa.set_publish(publish)
+            if architectures:
+                the_ppa.set_architectures(architectures)
+            arch_str = ', '.join(the_ppa.architectures)
+
+            if 'ppa_dependencies' in config:
+                # Split value on comma
+                ppa_addresses = unpack_to_dict(config.get('ppa_dependencies'))
+                the_ppa.set_dependencies(ppa_addresses)
+
         else:
-            ppa = Ppa(ppa_name, team_name, description)
+            the_ppa = Ppa(ppa_name, team_name, description)
             arch_str = ', '.join(architectures)
         if not config.get('quiet', False):
-            print("PPA '{}' created for the following architectures:\n".format(ppa.ppa_name))
+            print("PPA '{}' created for the following architectures:\n".format(the_ppa.ppa_name))
             print("  {}\n".format(arch_str))
             print("The PPA can be viewed at:\n")
-            print("  {}\n".format(ppa.url))
+            print("  {}\n".format(the_ppa.url))
             print("You can upload packages to this PPA using:\n")
-            print("  dput {} <source.changes>\n".format(ppa.address))
+            print("  dput {} <source.changes>\n".format(the_ppa.address))
             print("Wait for the uploads to build and publish using:\n")
-            print("  ppa wait {}\n".format(ppa.address))
+            print("  ppa wait {}\n".format(the_ppa.address))
             print("To add the repository and to your system:\n")
-            print("  sudo add-apt-repository -yus {}".format(ppa.address))
+            print("  sudo add-apt-repository -yus {}".format(the_ppa.address))
             print("  sudo apt-get install <package(s)>")
         return os.EX_OK
     except PpaAlreadyExists as e:
         warn(o2str(e.message))
         return 3
     except KeyboardInterrupt:
         return 2
     print("Unhandled error")
     return 1
 
 
-def command_desc(lp, config):
+def command_desc(lp: Lp, config: dict[str, str]) -> int:
     """Sets the description for a PPA.
 
     :param dict config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     if not sys.stdin.isatty():
@@ -374,51 +533,51 @@
         description = ' '.join(config.get('description', None))
 
     if not description or len(description) < 3:
         warn('No description provided')
         return os.EX_USAGE
 
     try:
-        ppa = get_ppa(lp, config)
+        the_ppa = get_ppa(lp, config)
         if config.get('dry_run', False):
             print("dry_run: Set description to '{}'".format(description))
             return os.EX_OK
 
-        return ppa.set_description(description)
+        return the_ppa.set_description(description)
     except KeyboardInterrupt:
         return 2
     print("Unhandled error")
     return 1
 
 
-def command_destroy(lp, config):
+def command_destroy(lp: Lp, config: dict[str, str]) -> int:
     """Destroys the PPA.
 
     :param Lp lp: The Launchpad wrapper object.
-    :param dict config: Configuration param:value map.
+    :param dict[str, str] config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     try:
-        ppa = get_ppa(lp, config)
+        the_ppa = get_ppa(lp, config)
         if not config.get('dry_run'):
             # Attempt deletion of the PPA
-            ppa.destroy()
+            the_ppa.destroy()
         return os.EX_OK
     except KeyboardInterrupt:
         return 2
     print("Unhandled error")
     return 1
 
 
-def command_list(lp, config, filter_func=None):
+def command_list(lp: Lp, config: dict[str, str], filter_func=None) -> int:
     """Lists the PPAs for the user or team.
 
     :param Lp lp: The Launchpad wrapper object.
-    :param dict config: Configuration param:value map.
+    :param dict[str, str] config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     # TODO: Apply filters such as:
     #  - Ones with packages for the given arch or codename
     #  - filter_not_empty: Ones with packages
     #  - filter_empty: Ones without packages
@@ -435,69 +594,112 @@
             team_name = lp.me.name
         else:
             warn("Could not determine team name")
             return os.EX_USAGE
 
     try:
         ppa_group = PpaGroup(service=lp, name=team_name)
-        for ppa in ppa_group.ppas:
-            print(ppa.address)
+        for p in ppa_group.ppas:
+            print(p.address)
         return os.EX_OK
     except KeyboardInterrupt:
         return 2
     print("Unhandled error")
     return 1
 
 
-def command_exists(lp, config):
+def command_exists(lp: Lp, config: dict[str, str]) -> int:
     """Checks if the named PPA exists in Launchpad.
 
     :param Lp lp: The Launchpad wrapper object.
-    :param dict config: Configuration param:value map.
+    :param dict[str, str] config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     try:
-        ppa = get_ppa(lp, config)
-        if ppa.archive is not None:
+        the_ppa = get_ppa(lp, config)
+        if the_ppa.archive is not None:
             return os.EX_OK
     except KeyboardInterrupt:
         return 2
     return 1
 
 
-def command_show(lp, config):
+def command_set(lp: Lp, config: dict[str, str]) -> int:
+    """Sets one or more properties of PPA in Launchpad.
+
+    :param Lp lp: The Launchpad wrapper object.
+    :param dict[str, str] config: Configuration param:value map.
+    :rtype: int
+    :returns: Status code OK (0) on success, non-zero on error.
+    """
+    try:
+        the_ppa = get_ppa(lp, config)
+
+        if 'architectures' in config:
+            architectures = config['architectures']
+            if type(architectures) is str:
+                architectures = unpack_to_dict(architectures).keys()
+            the_ppa.set_architectures(architectures)
+
+        if 'description' in config:
+            the_ppa.archive.description = config['description']
+
+        if 'displayname' in config:
+            the_ppa.archive.displayname = config['displayname']
+
+        if 'ppa_dependencies' in config:
+            # Split value on comma
+            ppa_addresses = unpack_to_dict(config.get('ppa_dependencies'))
+            the_ppa.set_dependencies(ppa_addresses)
+
+        if 'publish' in config:
+            the_ppa.archive.publish = config.get('publish')
+
+        return the_ppa.archive.lp_save()
+    except PpaDoesNotExist as e:
+        print(e)
+    except ValueError as e:
+        print(f"Error: {e}")
+        return os.EX_USAGE
+    except KeyboardInterrupt:
+        return 2
+    print("Unhandled error")
+    return 1
+
+
+def command_show(lp: Lp, config: dict[str, str]) -> int:
     """Displays details about the given PPA.
 
     :param Lp lp: The Launchpad wrapper object.
     :param dict config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     distro = None
     series = None
     arch = None
     try:
-        ppa = get_ppa(lp, config)
-        print(f"ppa:        {ppa.name}")
-        print(f"address:    {ppa.address}")
-        print(f"url:        {ppa.url}")
+        the_ppa = get_ppa(lp, config)
+        print(f"ppa:        {the_ppa.name}")
+        print(f"address:    {the_ppa.address}")
+        print(f"url:        {the_ppa.url}")
         print(f"description:")
-        print(indent(ppa.description, 4))
+        print(indent(the_ppa.description, 4))
 
         print("sources:")
-        for source in ppa.get_source_publications(distro, series, arch):
+        for source in the_ppa.get_source_publications(distro, series, arch):
             print("   %s (%s) %s" % (
                 source.source_package_name,
                 source.source_package_version,
                 source.status))
         # Only show binary details if specifically requested
         print("binaries:")
         total_downloads = 0
-        for binary in ppa.get_binaries(distro, series, arch) or []:
+        for binary in the_ppa.get_binaries(distro, series, arch) or []:
             # Skip uninteresting binaries
             if not config.get('show-debug', False) and binary.is_debug:
                 continue
             if not config.get('show-superseded', False) and binary.status == 'Superseded':
                 continue
             if not config.get('show-deleted', False) and binary.status == 'Deleted':
                 continue
@@ -519,19 +721,19 @@
         return 1
     except KeyboardInterrupt:
         return 2
     print("Unhandled error")
     return 1
 
 
-def command_status(lp, config):
+def command_status(lp: Lp, config: dict[str, str]) -> int:
     """Displays current status of the given ppa.
 
     :param Lp lp: The Launchpad wrapper object.
-    :param dict config: Configuration param:value map.
+    :param dict[str, str] config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
 
     # TODO: Allow option to limit to particular binary package
     #       Prints a two-line output showing the status of the binaries
     #       for a particular package and version.
@@ -543,189 +745,233 @@
 
     # TODO: Allow option to limit to particular series name
 
     UNIMPLEMENTED()
     return 1
 
 
-def command_wait(lp, config):
+def command_wait(lp: Lp, config: dict[str, str]) -> int:
     """Polls the PPA build status and block until all builds are finished and published.
 
     :param Lp lp: The Launchpad wrapper object.
-    :param dict config: Configuration param:value map.
+    :param dict[str, str] config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     try:
-        ppa = get_ppa(lp, config)
+        the_ppa = get_ppa(lp, config)
         waiting = True
         while waiting:
-            if not ppa.has_packages():
+            if not the_ppa.has_packages():
                 print("Nothing present in PPA.  Waiting for new package uploads...")
                 # TODO: Only wait a configurable amount of time (15 min?)
                 waiting = True  # config['wait_for_packages']
             else:
-                waiting = ppa.has_pending_publications()
+                waiting = the_ppa.has_pending_publications()
             time.sleep(config['wait_seconds'])
             print()
         return os.EX_OK
     except PpaDoesNotExist as e:
         print(e)
     except ValueError as e:
         print(f"Error: {e}")
         return os.EX_USAGE
     except KeyboardInterrupt:
         return 2
     print("Unhandled error")
     return 1
 
 
-def command_tests(lp, config):
+def command_tests(lp: Lp, config: dict[str, str]) -> int:
     """Displays testing status for the PPA.
 
     :param Lp lp: The Launchpad wrapper object.
-    :param dict config: Configuration param:value map.
+    :param dict[str, str] config: Configuration param:value map.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
     if not lp:
         return 1
 
+    apt_repository = None
+    if config.get("show_rdepends"):
+        local_dists_path = os.path.join(LOCAL_REPOSITORY_PATH, "dists")
+        try:
+            apt_repository = Repository(cache_dir=local_dists_path)
+        except FileNotFoundError as e:
+            error(f'Missing checkout\n{LOCAL_REPOSITORY_MIRRORING_DIRECTIONS}')
+            return 1
+
     releases = config.get('releases', None)
     if releases is None:
         udi = UbuntuDistroInfo()
-        try:
-            # Show tests only from the current development release
-            releases = [ udi.devel() ]
-        except DistroDataOutdated as e:
-            # If no development release defined, use the current active release
-            warn(f"Devel release is undefined; assuming stable release instead.")
-            dbg(f"({e})", wrap=72, prefix='  - ', indent='    ')
-            releases = [ udi.stable() ]
+        releases = udi.supported()
 
     packages = config.get('packages', None)
 
-    ppa = get_ppa(lp, config)
-    if not ppa.exists():
-        error(f"PPA {ppa.name} does not exist for user {ppa.team_name}")
+    the_ppa = get_ppa(lp, config)
+    if not the_ppa.exists():
+        error(f"PPA {the_ppa.name} does not exist for user {the_ppa.team_name}")
         return 1
 
     architectures = config.get('architectures', ARCHES_AUTOPKGTEST)
+    if type(architectures) is str:
+        architectures = unpack_to_dict(architectures).keys()
 
     try:
         # Triggers
         print("* Triggers:")
-        for source_pub in ppa.get_source_publications():
-            series = source_pub.distro_series.name
-            if series not in releases:
+        for source_pub in the_ppa.get_source_publications():
+            series_codename = source_pub.distro_series.name
+            if series_codename not in releases:
                 continue
             pkg = source_pub.source_package_name
             if packages and (pkg not in packages):
                 continue
             ver = source_pub.source_package_version
             url = f"https://launchpad.net/ubuntu/+source/{pkg}/{ver}"
             source_hyperlink = ansi_hyperlink(url, f"{pkg}/{ver}")
             print(f"  - Source {source_hyperlink}: {source_pub.status}")
-            triggers = [Trigger(pkg, ver, arch, series, ppa) for arch in architectures]
+            triggers = [Trigger(pkg, ver, arch, series_codename, the_ppa) for arch in architectures]
+
+            rdepends = None
+            if config.get("show_rdepends"):
+                # Construct suite object from repository.
+                # NOTE: If a package has been freshly added to 'proposed' it
+                #       will be missed since we consider only packages present
+                #       in the release pocket.
+                suite = apt_repository.get_suite(series_codename, 'release')
+                if not suite:
+                    raise RuntimeError(f'Could not find suite for "{series_codename}" in the local Apt cache')
+
+                # Lookup rdepends for the package
+                source_package = suite.sources.get(pkg)
+                if not source_package:
+                    raise RuntimeError(f'Could not find source package "{pkg}" in the local Apt cache for "{suite}"')
+
+                rdepends_source_package_names = suite.dependent_packages(source_package)
+                for rdep_name in rdepends_source_package_names:
+                    rdep = suite.sources.get(rdep_name)
+                    if not rdep:
+                        raise RuntimeError(f'Undefined reverse dependency "{rdep_name}"')
+
+                    triggers.extend([
+                        Trigger(pkg, ver, arch, series_codename, the_ppa, rdep.name)
+                        for arch
+                        in architectures
+                    ])
 
             if config.get("show_urls"):
                 for trigger in triggers:
-                    print(f"    + {trigger.arch}: {trigger.action_url}♻️ ")
+                    title = ''
+                    if config.get('show_rdepends'):
+                        title = trigger.test_package
+                    print(f"    + {title}@{trigger.arch}: {trigger.action_url}♻️ ")
                 for trigger in triggers:
-                    print(f"    + {trigger.arch}: {trigger.action_url}💍")
+                    title = ''
+                    if config.get('show_rdepends'):
+                        title = trigger.test_package
+                        print(f"    + {trigger.package}@{trigger.arch}: {trigger.action_url}💍")
 
             else:
                 for trigger in triggers:
                     pad = ' ' * (1 + abs(len('ppc64el') - len(trigger.arch)))
-                    basic_trig = ansi_hyperlink(trigger.action_url, f"Trigger basic @{trigger.arch}♻️ ")
-                    all_proposed_trig = ansi_hyperlink(trigger.action_url + "&all-proposed=1",
-                                                       f"Trigger all-proposed @{trigger.arch}💍")
+                    title = ''
+                    if config.get('show_rdepends'):
+                        title = trigger.test_package
+
+                    basic_trig = ansi_hyperlink(
+                        trigger.action_url, f"Trigger basic {title}@{trigger.arch}♻️ "
+                    )
+                    all_proposed_trig = ansi_hyperlink(
+                        trigger.action_url + "&all-proposed=1",
+                        f"Trigger all-proposed {title}@{trigger.arch}💍"
+                    )
                     print(f"    + " + pad.join([basic_trig, all_proposed_trig]))
 
         # Results
-        print()
         print("* Results:")
         for release in releases:
             base_results_fmt = f"{URL_AUTOPKGTEST}/results/autopkgtest-%s-%s-%s/"
-            base_results_url = base_results_fmt % (release, ppa.team_name, ppa.name)
+            base_results_url = base_results_fmt % (release, the_ppa.team_name, the_ppa.name)
             url = f"{base_results_url}?format=plain"
             response = open_url(url)
             if response:
                 trigger_sets = {}
                 for result in get_results(response, base_results_url, arches=architectures):
                     trigger = ', '.join([str(r) for r in result.get_triggers()])
                     trigger_sets.setdefault(trigger, '')
                     if config.get("show_urls"):
                         trigger_sets[trigger] += f"    + {result.status_icon} {result}\n"
+                        trigger_sets[trigger] += f"      • Log: {result.url}\n"
                         if result.status != 'PASS':
                             trigger_sets[trigger] += f"      • Status: {result.status}\n"
-                            trigger_sets[trigger] += f"      • Log: {result.url}\n"
                             for subtest in result.get_subtests():
                                 trigger_sets[trigger] += f"      • {subtest}\n"
                     else:
                         log_link = ansi_hyperlink(result.url, f"Log️ 🗒️ ")
                         trigger_sets[trigger] += f"    + {result.status_icon} {result}  {log_link}\n"
                         if result.status != 'PASS':
                             for subtest in result.get_subtests():
                                 trigger_sets[trigger] += f"      • {subtest}\n"
 
                 for trigger, result in trigger_sets.items():
-                    print(f"  - {trigger}\n{result}")
+                    print(f"  - {trigger}\n{result.rstrip()}")
 
         # Running Queue
-        response = open_url(f"{URL_AUTOPKGTEST}/static/running.json", "running autopkgtests")
-        if response:
-            show_running(sorted(get_running(response, releases=releases, ppa=str(ppa)),
-                                key=lambda k: str(k.submit_time)))
+        show_running(sorted(the_ppa.get_autopkgtest_running(releases),
+                            key=lambda k: str(k.submit_time)))
 
         # Waiting Queue
-        response = open_url(f"{URL_AUTOPKGTEST}/queues.json", "waiting autopkgtests")
-        if response:
-            show_waiting(get_waiting(response, releases=releases, ppa=str(ppa)))
+        show_waiting(the_ppa.get_autopkgtest_waiting(releases))
 
         return os.EX_OK
     except KeyboardInterrupt:
         return 2
     print("Unhandled error")
     return 1
 
 
 COMMANDS = {
     'create':     (command_create, None),
     'desc':       (command_desc, None),
     'destroy':    (command_destroy, None),
     'list':       (command_list, None),
+    'set':        (command_set, None),
     'show':       (command_show, None),
     'status':     (command_status, None),
     'tests':      (command_tests, None),
     'wait':       (command_wait, None),
     }
 
 
-def main(args):
+def main(args: argparse.Namespace) -> int:
     """Main entrypoint for the command.
 
     :param argparse.Namespace args: Command line arguments.
     :rtype: int
     :returns: Status code OK (0) on success, non-zero on error.
     """
+    if not args.command:
+        error("No command given.")
+        return os.EX_USAGE
+
     lp = Lp('ppa-dev-tools')
 
     config = create_config(lp, args)
     if not config:
         return os.EX_CONFIG
 
     ppa.debug.DEBUGGING = config.get('debug', False)
+
     dbg("Configuration:")
     dbg(config)
 
     command = args.command
 
-    ppa.debug.DEBUGGING = config.get('debug', False)
-
     try:
         func, param = COMMANDS[command]
         if param:
             return func(lp, config, param)
         return func(lp, config)
     except KeyError:
         parser.error(f"No such command {args.command}")
```

### Comparing `ppa-dev-tools-0.3.0/setup.py` & `ppa-dev-tools-0.4.0/setup.py`

 * *Files identical despite different names*

