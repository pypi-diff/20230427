# Comparing `tmp/JsonPreprocessor-0.1.5.tar.gz` & `tmp/JsonPreprocessor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonPreprocessor-0.1.5.tar", last modified: Thu Apr 27 09:21:03 2023, max compression
+gzip compressed data, was "dist\JsonPreprocessor-0.2.0.tar", last modified: Tue Jun 28 13:28:17 2022, max compression
```

## Comparing `JsonPreprocessor-0.1.5.tar` & `JsonPreprocessor-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:03.074110 JsonPreprocessor-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:03.070109 JsonPreprocessor-0.1.5/JsonPreprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)    27824 2023-04-27 09:18:56.000000 JsonPreprocessor-0.1.5/JsonPreprocessor/CJsonPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)   304189 2023-04-27 09:18:56.000000 JsonPreprocessor-0.1.5/JsonPreprocessor/JsonPreprocessor.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-27 09:18:56.000000 JsonPreprocessor-0.1.5/JsonPreprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 09:18:56.000000 JsonPreprocessor-0.1.5/JsonPreprocessor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:03.070109 JsonPreprocessor-0.1.5/JsonPreprocessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-27 09:21:02.000000 JsonPreprocessor-0.1.5/JsonPreprocessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 09:21:03.000000 JsonPreprocessor-0.1.5/JsonPreprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:21:02.000000 JsonPreprocessor-0.1.5/JsonPreprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 09:21:02.000000 JsonPreprocessor-0.1.5/JsonPreprocessor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:21:02.000000 JsonPreprocessor-0.1.5/JsonPreprocessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-27 09:18:56.000000 JsonPreprocessor-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-27 09:21:03.074110 JsonPreprocessor-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-27 09:18:56.000000 JsonPreprocessor-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:21:03.074110 JsonPreprocessor-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-27 09:18:56.000000 JsonPreprocessor-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-28 13:28:17.544932 JsonPreprocessor-0.2.0/
+drwxrwxrwx   0        0        0        0 2022-06-28 13:28:17.527354 JsonPreprocessor-0.2.0/JsonPreprocessor/
+-rw-rw-rw-   0        0        0    16246 2022-05-31 17:55:29.000000 JsonPreprocessor-0.2.0/JsonPreprocessor/CJsonPreprocessor.py
+-rw-rw-rw-   0        0        0      659 2022-05-31 17:55:29.000000 JsonPreprocessor-0.2.0/JsonPreprocessor/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-28 13:28:17.541026 JsonPreprocessor-0.2.0/JsonPreprocessor.egg-info/
+-rw-rw-rw-   0        0        0     3511 2022-06-28 13:28:16.000000 JsonPreprocessor-0.2.0/JsonPreprocessor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2022-06-28 13:28:17.000000 JsonPreprocessor-0.2.0/JsonPreprocessor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-28 13:28:16.000000 JsonPreprocessor-0.2.0/JsonPreprocessor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2022-06-28 13:28:16.000000 JsonPreprocessor-0.2.0/JsonPreprocessor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-06-28 13:28:16.000000 JsonPreprocessor-0.2.0/JsonPreprocessor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11356 2022-05-31 17:55:29.000000 JsonPreprocessor-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3511 2022-06-28 13:28:17.543955 JsonPreprocessor-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2988 2022-05-31 17:55:29.000000 JsonPreprocessor-0.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2022-06-28 13:28:17.544932 JsonPreprocessor-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0    10126 2022-05-31 17:55:29.000000 JsonPreprocessor-0.2.0/setup.py
```

### Comparing `JsonPreprocessor-0.1.5/JsonPreprocessor/__init__.py` & `JsonPreprocessor-0.2.0/JsonPreprocessor/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,10 +7,8 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from .CJsonPreprocessor import CJsonPreprocessor
-from .CJsonPreprocessor import CSyntaxType
-
+from .CJsonPreprocessor import CJsonPreprocessor
```

### Comparing `JsonPreprocessor-0.1.5/LICENSE` & `JsonPreprocessor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.1.5/README.rst` & `JsonPreprocessor-0.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .. Copyright 2020-2022 Robert Bosch GmbH
 
-.. Licensed under the Apache License, Version 2.0 (the "License");
+   Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
-.. http://www.apache.org/licenses/LICENSE-2.0
+   http://www.apache.org/licenses/LICENSE-2.0
 
-.. Unless required by applicable law or agreed to in writing, software
+   Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 Json Preprocessor's Package Description
 =======================================
@@ -27,44 +27,31 @@
 
 These json files will be handled by the JsonPreprocessor which returns as result
 a dictionary object of the deserialized data.
 
 How to install
 --------------
 
-**JsonPreprocessor** can be installed in two different ways.
+Firstly, clone **python-jsonpreprocessor** repository to your machine.
 
-1. Installation via PyPi (recommended for users)
+Then go to python-jsonpreprocessor, using the 2 common commands below to build or install this package:
 
-   .. code::
+.. code-block::
 
-      pip install JsonPreprocessor
+    setup.py build      will build the package underneath 'build/'
+    setup.py install    will install the package
 
-   `JsonPreprocessor in PyPi <https://pypi.org/project/JsonPreprocessor/>`_
+After the build processes is completed, the package is located in 'build/', and the generated 
+package documentation is located in 'doc/_build/'.
 
-2. Installation via GitHub (recommended for developers)
-
-   Clone the **JsonPreprocessor** repository to your machine.
-
-   .. code::
-
-      git clone https://github.com/test-fullautomation/python-jsonpreprocessor.git
-
-   `JsonPreprocessor in GitHub <https://github.com/test-fullautomation/python-jsonpreprocessor>`_
-
-   Use the following command to install **JsonPreprocessor**:
-
-   .. code::
-
-      setup.py install
 
 Package Documentation
 ---------------------
 
-A detailed documentation of the Json Preprocessor's package can be found here: `JsonPreprocessor.pdf <https://github.com/test-fullautomation/python-jsonpreprocessor/blob/develop/JsonPreprocessor/JsonPreprocessor.pdf>`_
+A detailed documentation of the Json Preprocessor's package can be found here: `Json-Preprocessor.pdf <https://github.com/test-fullautomation/python-jsonpreprocessor/blob/develop/doc/_build/latex/Json-Preprocessor.pdf>`_
 
 Feedback
 --------
 
 To give us a feedback, you can send an email to `Thomas Pollerspöck <mailto:Thomas.Pollerspoeck@de.bosch.com>`_ 
 
 In case you want to report a bug or request any interesting feature, please don't
```

### Comparing `JsonPreprocessor-0.1.5/setup.py` & `JsonPreprocessor-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 #
 # **************************************************************************************************************
 #
 # setup.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# Extends the standard setuptools installation by adding the documentation in PDF format
+# Extends the standard setuptools installation by adding the documentation in HTML format
 # (requires installation mode) and tidying up some folders.
 #
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 #
-# This script deletes folders (as defined in config.CRepositoryConfig, depending on the position of this script):
+# This script deletes folders (as defined in config.CConfig, depending on the position of this script):
 # - previous builds within this repository
 # - previous installations within
 #   * <Python installation>\Lib\site-packages (Windows)
 #   * <Python installation>/../lib/python3.9/site-packages (Linux)
 #
 # before the build and the installation start again!
 #
@@ -40,43 +40,54 @@
 # --------------------------------------------------------------------------------------------------------------
 #
 # * Hints:
 #
 # The usual
 #    packages = setuptools.find_packages(),
 # is replaced by
-#    packages = [str(oRepositoryConfig.Get('PACKAGENAME')), ],
-# to avoid that also config.CRepositoryConfig() and additions.CExtendedSetup() are part of the distribution.
-# CRepositoryConfig and CExtendedSetup() are only repository internal helper.
+#    packages = [str(oRepositoryConfig.Get('sPackageName')), ],
+# to avoid that also config.CConfig() and config.CExtendedSetup() are part of the distribution.
+# CConfig and CExtendedSetup() are only repository internal helper.
 #
 # * Known issues:
 #
 #   - setuptools do not properly update an existing package installation under <Python installation>\Lib\site-packages\<package name>!
 #     > Files modified manually within installation folder, are still modified after repeated execution of setuptools.
 #     > Files added manually within installation folder, are still present there after repeated execution of setuptools.
 #     > Only files deleted manually within installation folder, are are restored there after repeated execution of setuptools.
 #   - No such issues with <Python installation>\Lib\site-packages\<package name>-<versions>.egg-info.
 #   - Solution: explicit deletion of all previous output (all documentation-, build- and installation-folder, except the egg-info folder)
 #     (see 'delete_previous_build()' and 'delete_previous_installation()')
 #
 # --------------------------------------------------------------------------------------------------------------
 #
-# 30.06.2022
+# 21.02.2022 / XC-CT/ECA3-Queckenstedt
+#
+# "sdist bdist_wheel" maintenance: some steps moved from inside 'ExtendedInstallCommand' to outside
+#
+# 09.02.2022 / XC-CT/ECA3-Queckenstedt
+# Suppressed generation of documents and installations in case of command line
+# parameter is not 'install' and not 'build' (this enables printing the help only). (10.02.2022: and not 'sdist')
+#
+# 11.10.2021 / XC-CI1/ECA3-Queckenstedt
+# Fixed computation order of readme files together with long_description
+# 
+# 30.09.2021 / XC-CI1/ECA3-Queckenstedt
+# Added wrapper for error messages
+# 
+# Initial version 08/2021
 #
 # --------------------------------------------------------------------------------------------------------------
 
 import os, sys, platform, shlex, subprocess
 import setuptools
 from setuptools.command.install import install
 
-# prefer the repository local version of all additional libraries (instead of the installed version under site-packages)
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "./additions")))
-
-from config.CRepositoryConfig import CRepositoryConfig # providing repository and environment specific information
-from additions.CExtendedSetup import CExtendedSetup # providing functions to support the extended setup process
+from config.CConfig import CConfig # providing repository and environment specific information
+from config.CExtendedSetup import CExtendedSetup # providing functions to support the extended setup process
 
 import colorama as col
 
 col.init(autoreset=True)
 
 COLBR = col.Style.BRIGHT + col.Fore.RED
 COLBY = col.Style.BRIGHT + col.Fore.YELLOW
@@ -98,28 +109,50 @@
 class ExtendedInstallCommand(install):
     """Extended setup for installation mode."""
 
     def run(self):
 
         listCmdArgs = sys.argv
         if ( ('install' in listCmdArgs) or ('build' in listCmdArgs) or ('sdist' in listCmdArgs) or ('bdist_wheel' in listCmdArgs) ):
-            install.run(self)
+            print()
+            print(COLBY + "Extended setup step 4/5: install.run(self)") # creates the build folder .\build
+            print()
+            install.run(self) # TODO: What does install.run(self) return? How to realize error handling?
+            print()
+            if 'bdist_wheel' in listCmdArgs:
+                print(COLBY + "Extended setup step 5/5: Add html documentation to local wheel folder inside build")
+                print()
+                nReturn = oExtendedSetup.add_htmldoc_to_wheel()
+                if nReturn != SUCCESS:
+                    return nReturn
+                print()
+            else:
+                print(COLBY + "Extended setup step 5/5: Add html documentation to package installation folder") # (./doc/_build/html to <Python installation>\Lib\site-packages\<package name>_doc)
+                print()
+                nReturn = oExtendedSetup.add_htmldoc_to_installation()
+                if nReturn != SUCCESS:
+                    return nReturn
+                print()
+            print(COLBG + "Extended installation done")
+            print()
+
         return SUCCESS
 
 # eof class ExtendedInstallCommand(install):
 
 # --------------------------------------------------------------------------------------------------------------
 
 # -- Even in case of other command line parameters than 'install' or 'build' are used we need the following objects.
 #    (Without repository configuration commands like '--author-email' would not be possible)
 
 # -- setting up the repository configuration
 oRepositoryConfig = None
+sReferencePath = os.path.dirname(os.path.abspath(sys.argv[0]))
 try:
-    oRepositoryConfig = CRepositoryConfig(os.path.abspath(sys.argv[0]))
+    oRepositoryConfig = CConfig(sReferencePath)
 except Exception as ex:
     print()
     printexception(str(ex))
     print()
     sys.exit(ERROR)
 
 # -- setting up the extended setup
@@ -139,83 +172,63 @@
 listCmdArgs = sys.argv
 if ( ('install' in listCmdArgs) or ('build' in listCmdArgs) or ('sdist' in listCmdArgs) or ('bdist_wheel' in listCmdArgs) ):
     print()
     print(COLBY + "Entering extended installation")
     print()
 
     print(COLBY + "Extended setup step 1/5: Calling the documentation builder")
+    # (previously called inside ExtendedInstallCommand - but this is too late, because the content of the initially
+    # generated or updated README file is already needed for the long_description below.)
     print()
-
-    nReturn = oExtendedSetup.genpackagedoc()
-    if nReturn != SUCCESS:
-        sys.exit(nReturn)
-
-    print(COLBY + "Extended setup step 2/5: Converting the repository README")
-    print()
-
-    nReturn = oExtendedSetup.convert_repo_readme()
+    nReturn = oExtendedSetup.gen_doc()
     if nReturn != SUCCESS:
         sys.exit(nReturn)
 
-    print(COLBY + "Extended setup step 3/5: Deleting previous setup outputs (build, dist, <package name>.egg-info within repository)")
+    print(COLBY + "Extended setup step 2/5: Deleting previous setup outputs (build, dist, <package name>.egg-info within repository)")
     print()
     nReturn = oExtendedSetup.delete_previous_build()
     if nReturn != SUCCESS:
         sys.exit(nReturn)
 
-    if ( ('bdist_wheel' in listCmdArgs) or ('build' in listCmdArgs) ):
+    if not 'bdist_wheel' in listCmdArgs:
         print()
-        print(COLBY + "Skipping extended setup step 4/5: Deleting previous package installation folder within site-packages")
-        print()
-    else:
-        print()
-        print(COLBY + "Extended setup step 4/5: Deleting previous package installation folder within site-packages") # (<package name> and <package name>_doc under <Python installation>\Lib\site-packages
+        print(COLBY + "Extended setup step 3/5: Deleting previous package installation folder within site-packages") # (<package name> and <package name>_doc under <Python installation>\Lib\site-packages
         print()
         nReturn = oExtendedSetup.delete_previous_installation()
         if nReturn != SUCCESS:
             sys.exit(nReturn)
 
-    README_MD = str(oRepositoryConfig.Get('README_MD'))
-    with open(README_MD, "r", encoding="utf-8") as fh:
+    with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
-    fh.close()
-
-# --------------------------------------------------------------------------------------------------------------
+    print()
 
-# -- the 'setup' itself
 
-print(COLBY + "Extended setup step 5/5: install.run(self)")
-print()
+# --------------------------------------------------------------------------------------------------------------
 
+# This also handles the printing of help to console and therefore must be called in every case.
+# And therefore all variables and objects must exist (even in case of the values are not used).
 setuptools.setup(
-    name         = str(oRepositoryConfig.Get('PACKAGENAME')),
-    version      = str(oRepositoryConfig.Get('PACKAGEVERSION')),
-    author       = str(oRepositoryConfig.Get('AUTHOR')),
-    author_email = str(oRepositoryConfig.Get('AUTHOREMAIL')),
-    description  = str(oRepositoryConfig.Get('DESCRIPTION')),
+    name         = str(oRepositoryConfig.Get('sPackageName')),
+    version      = str(oRepositoryConfig.Get('sVersion')),
+    author       = str(oRepositoryConfig.Get('sAuthor')),
+    author_email = str(oRepositoryConfig.Get('sAuthorEMail')),
+    description  = str(oRepositoryConfig.Get('sDescription')),
     long_description = long_description,
-    long_description_content_type = str(oRepositoryConfig.Get('LONGDESCRIPTIONCONTENTTYPE')),
-    url = str(oRepositoryConfig.Get('URL')),
-    packages = [str(oRepositoryConfig.Get('PACKAGENAME')),],
+    long_description_content_type = str(oRepositoryConfig.Get('sLongDescriptionContentType')),
+    url = str(oRepositoryConfig.Get('sURL')),
+    packages = [str(oRepositoryConfig.Get('sPackageName')), ],
     classifiers = [
-        str(oRepositoryConfig.Get('PROGRAMMINGLANGUAGE')),
-        str(oRepositoryConfig.Get('LICENCE')),
-        str(oRepositoryConfig.Get('OPERATINGSYSTEM')),
-        str(oRepositoryConfig.Get('DEVELOPMENTSTATUS')),
-        str(oRepositoryConfig.Get('INTENDEDAUDIENCE')),
-        str(oRepositoryConfig.Get('TOPIC')),
+        str(oRepositoryConfig.Get('sProgrammingLanguage')),
+        str(oRepositoryConfig.Get('sLicence')),
+        str(oRepositoryConfig.Get('sOperatingSystem')),
+        str(oRepositoryConfig.Get('sDevelopmentStatus')),
+        str(oRepositoryConfig.Get('sIntendedAudience')),
+        str(oRepositoryConfig.Get('sTopic')),
     ],
-    python_requires = str(oRepositoryConfig.Get('PYTHONREQUIRES')),
+    python_requires = str(oRepositoryConfig.Get('sPythonRequires')),
     cmdclass={
         'install': ExtendedInstallCommand,
     },
-    install_requires = oRepositoryConfig.Get('INSTALLREQUIRES'),
-    package_data={f"{oRepositoryConfig.Get('PACKAGENAME')}" : oRepositoryConfig.Get('PACKAGEDATA')},
+    install_requires = oRepositoryConfig.Get('arInstallRequires'),
 )
 # --------------------------------------------------------------------------------------------------------------
 
-print()
-print(COLBG + "Extended installation done")
-print()
-
-# --------------------------------------------------------------------------------------------------------------
-
```

