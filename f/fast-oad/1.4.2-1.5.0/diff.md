# Comparing `tmp/FAST-OAD-1.4.2.tar.gz` & `tmp/fast_oad-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAST-OAD-1.4.2.tar", max compression
+gzip compressed data, was "fast_oad-1.5.0.tar", max compression
```

## Comparing `FAST-OAD-1.4.2.tar` & `fast_oad-1.5.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     3301 2023-01-20 07:20:17.174387 FAST-OAD-1.4.2/README.md
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.514581 FAST-OAD-1.4.2/_fastoad/__init__.py
--rw-r--r--   0        0        0     2726 2023-01-20 07:20:17.614382 FAST-OAD-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     4111 2023-01-20 07:20:18.159023 FAST-OAD-1.4.2/setup.py
--rw-r--r--   0        0        0     4522 2023-01-20 07:20:18.159310 FAST-OAD-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3488 2023-04-27 14:57:39.585432 fast_oad-1.5.0/README.md
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.147289 fast_oad-1.5.0/_fastoad/__init__.py
+-rw-r--r--   0        0        0     2400 2023-04-27 14:57:40.889530 fast_oad-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 fast_oad-1.5.0/PKG-INFO
```

### Comparing `FAST-OAD-1.4.2/README.md` & `fast_oad-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+<p align="center">
+  <img src="docs/img/FAST_OAD_logo2.jpg" alt="FAST-OAD logo" width="600">
+</p>
+
+Future Aircraft Sizing Tool - Overall Aircraft Design
+===============================================================
+
 ![Tests](https://github.com/fast-aircraft-design/FAST-OAD/workflows/Tests/badge.svg)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9691f1d1430c45cf9c94bc342b4c6122)](https://www.codacy.com/gh/fast-aircraft-design/FAST-OAD?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fast-aircraft-design/FAST-OAD&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/fast-aircraft-design/FAST-OAD/branch/master/graph/badge.svg)](https://codecov.io/gh/fast-aircraft-design/FAST-OAD)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![Documentation Status](https://readthedocs.org/projects/fast-oad/badge/?version=stable)](https://fast-oad.readthedocs.io/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fast-aircraft-design/FAST-OAD.git/latest-release?urlpath=lab%2Ftree%2Fsrc%2Ffastoad%2Fnotebooks)
+[![DOI](https://zenodo.org/badge/186570813.svg)](https://zenodo.org/badge/latestdoi/186570813)
+
+
 
 
-FAST-OAD: Future Aircraft Sizing Tool - Overall Aircraft Design
-===============================================================
 
 FAST-OAD is a framework for performing rapid Overall Aircraft Design.
 
 It proposes multi-disciplinary analysis and optimisation by relying on
 the [OpenMDAO framework](https://openmdao.org/).
 
 FAST-OAD allows easy switching between models for a same discipline, and
```

### Comparing `FAST-OAD-1.4.2/_fastoad/__init__.py` & `fast_oad-1.5.0/_fastoad/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-1.4.2/pyproject.toml` & `fast_oad-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FAST-OAD"
-version = "v1.4.2" # This version number is overwritten by GitHub packaging workflow but setting 1.3 here will allow installation of CS25 models in development mode
+version = "1.5.0" # This version number is overwritten by GitHub packaging workflow but setting 1.3 here will allow installation of CS25 models in development mode
 description = "FAST-OAD is a framework for performing rapid Overall Aircraft Design"
 readme = "README.md"
 authors = [
     "Christophe DAVID <christophe.david@onera.fr>",
     "Scott DELBECQ <Scott.DELBECQ@isae-supaero.fr>"
 ]
 packages = [{ include = "_fastoad"}]
@@ -30,27 +30,26 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
 [tool.poetry.dependencies]
-# IMPORTANT: when modifying this list, docs/requirements.txt must be updated for
-# ReadTheDocs to be able to compile the documentation.
-# A pre-commit hook has been added to do this task. As a result, any modification
-# of poetry.lock file will modify docs/requirements.txt and make
-# the commit fail because "files were modified by this hook". In that case,
-# doing again the commit including changes in docs/requirements.txt will succeed.
 python = "^3.7"
-fast-oad-core = "^v1.4.2"
+fast-oad-core = "^1.5.0"
 fast-oad-cs25 = ">=0.1.4"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 100
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov fastoad --cov-report term-missing --cov-report html --verbose"
```

### Comparing `FAST-OAD-1.4.2/setup.py` & `fast_oad-1.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,113 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fast-oad
+Version: 1.5.0
+Summary: FAST-OAD is a framework for performing rapid Overall Aircraft Design
+Home-page: https://github.com/fast-aircraft-design/FAST-OAD
+License: GPL-3.0-only
+Keywords: aircraft,design,multi-disciplinary
+Author: Christophe DAVID
+Author-email: christophe.david@onera.fr
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Dist: fast-oad-core (>=1.5.0,<2.0.0)
+Requires-Dist: fast-oad-cs25 (>=0.1.4)
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <img src="docs/img/FAST_OAD_logo2.jpg" alt="FAST-OAD logo" width="600">
+</p>
+
+Future Aircraft Sizing Tool - Overall Aircraft Design
+===============================================================
+
+![Tests](https://github.com/fast-aircraft-design/FAST-OAD/workflows/Tests/badge.svg)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/9691f1d1430c45cf9c94bc342b4c6122)](https://www.codacy.com/gh/fast-aircraft-design/FAST-OAD?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fast-aircraft-design/FAST-OAD&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/fast-aircraft-design/FAST-OAD/branch/master/graph/badge.svg)](https://codecov.io/gh/fast-aircraft-design/FAST-OAD)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+[![Documentation Status](https://readthedocs.org/projects/fast-oad/badge/?version=stable)](https://fast-oad.readthedocs.io/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fast-aircraft-design/FAST-OAD.git/latest-release?urlpath=lab%2Ftree%2Fsrc%2Ffastoad%2Fnotebooks)
+[![DOI](https://zenodo.org/badge/186570813.svg)](https://zenodo.org/badge/latestdoi/186570813)
 
-packages = \
-['_fastoad']
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['fast-oad-core>=v1.4.2,<2.0.0', 'fast-oad-cs25>=0.1.4']
-
-setup_kwargs = {
-    'name': 'fast-oad',
-    'version': '1.4.2',
-    'description': 'FAST-OAD is a framework for performing rapid Overall Aircraft Design',
-    'long_description': '![Tests](https://github.com/fast-aircraft-design/FAST-OAD/workflows/Tests/badge.svg)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/9691f1d1430c45cf9c94bc342b4c6122)](https://www.codacy.com/gh/fast-aircraft-design/FAST-OAD?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fast-aircraft-design/FAST-OAD&amp;utm_campaign=Badge_Grade)\n[![codecov](https://codecov.io/gh/fast-aircraft-design/FAST-OAD/branch/master/graph/badge.svg)](https://codecov.io/gh/fast-aircraft-design/FAST-OAD)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![Documentation Status](https://readthedocs.org/projects/fast-oad/badge/?version=stable)](https://fast-oad.readthedocs.io/)\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fast-aircraft-design/FAST-OAD.git/latest-release?urlpath=lab%2Ftree%2Fsrc%2Ffastoad%2Fnotebooks)\n\n\nFAST-OAD: Future Aircraft Sizing Tool - Overall Aircraft Design\n===============================================================\n\nFAST-OAD is a framework for performing rapid Overall Aircraft Design.\n\nIt proposes multi-disciplinary analysis and optimisation by relying on\nthe [OpenMDAO framework](https://openmdao.org/).\n\nFAST-OAD allows easy switching between models for a same discipline, and\nalso adding/removing/developing models to match the need of your study.\n\nMore details can be found in the [official documentation](https://fast-oad.readthedocs.io/).\n\n> **Important notice:**\n>\n> Since version 1.3.0, FAST-OAD models for commercial transport aircraft have moved in \n> package  \n> [FAST-OAD-CS25](https://pypi.org/project/fast-oad-cs25/). This package is installed along with \n> FAST-OAD, to keep backward compatibility.\n> \n> Keep in mind that any update of these models will now come through new releases of FAST-OAD-CS25.\n> \n> To get FAST-OAD without these models, you may install\n> [FAST-OAD-core](https://pypi.org/project/fast-oad-core/).\n> \n> :warning: Upgrading from an earlier version than 1.3 may break the `fastoad` command line (no \n> impact on PythonAPI). See [this issue](https://github.com/fast-aircraft-design/FAST-OAD/issues/425)\n> for details and fix.\n\nWant to try quickly?\n--------------------\nYou can run FAST-OAD tutorials **without installation** using our\n[Binder-hosted Jupyter notebooks](https://mybinder.org/v2/gh/fast-aircraft-design/FAST-OAD.git/latest-release?filepath=src%2Ffastoad%2Fnotebooks).\n\n\nInstall\n-------\n\n**Prerequisite**:FAST-OAD needs at least **Python 3.7.0**.\n\nIt is recommended (but not required) to install FAST-OAD in a virtual\nenvironment ([conda](https://docs.conda.io/en/latest/),\n[venv](https://docs.python.org/3.7/library/venv.html), ...)\n\nOnce Python is installed, FAST-OAD can be installed using pip.\n\n> **Note**: If your network uses a proxy, you may have to do [some\n> settings](https://pip.pypa.io/en/stable/user_guide/#using-a-proxy-server)\n> for pip to work correctly\n\nYou can install the latest version with this command:\n\n``` {.bash}\n$ pip install --upgrade fast-oad\n```\n\nor, if you want the minimum installation without the CS25-related models:\n\n``` {.bash}\n$ pip install --upgrade fast-oad-core\n```\n',
-    'author': 'Christophe DAVID',
-    'author_email': 'christophe.david@onera.fr',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/fast-aircraft-design/FAST-OAD',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
 
 
-setup(**setup_kwargs)
+FAST-OAD is a framework for performing rapid Overall Aircraft Design.
+
+It proposes multi-disciplinary analysis and optimisation by relying on
+the [OpenMDAO framework](https://openmdao.org/).
+
+FAST-OAD allows easy switching between models for a same discipline, and
+also adding/removing/developing models to match the need of your study.
+
+More details can be found in the [official documentation](https://fast-oad.readthedocs.io/).
+
+> **Important notice:**
+>
+> Since version 1.3.0, FAST-OAD models for commercial transport aircraft have moved in 
+> package  
+> [FAST-OAD-CS25](https://pypi.org/project/fast-oad-cs25/). This package is installed along with 
+> FAST-OAD, to keep backward compatibility.
+> 
+> Keep in mind that any update of these models will now come through new releases of FAST-OAD-CS25.
+> 
+> To get FAST-OAD without these models, you may install
+> [FAST-OAD-core](https://pypi.org/project/fast-oad-core/).
+> 
+> :warning: Upgrading from an earlier version than 1.3 may break the `fastoad` command line (no 
+> impact on PythonAPI). See [this issue](https://github.com/fast-aircraft-design/FAST-OAD/issues/425)
+> for details and fix.
+
+Want to try quickly?
+--------------------
+You can run FAST-OAD tutorials **without installation** using our
+[Binder-hosted Jupyter notebooks](https://mybinder.org/v2/gh/fast-aircraft-design/FAST-OAD.git/latest-release?filepath=src%2Ffastoad%2Fnotebooks).
+
+
+Install
+-------
+
+**Prerequisite**:FAST-OAD needs at least **Python 3.7.0**.
+
+It is recommended (but not required) to install FAST-OAD in a virtual
+environment ([conda](https://docs.conda.io/en/latest/),
+[venv](https://docs.python.org/3.7/library/venv.html), ...)
+
+Once Python is installed, FAST-OAD can be installed using pip.
+
+> **Note**: If your network uses a proxy, you may have to do [some
+> settings](https://pip.pypa.io/en/stable/user_guide/#using-a-proxy-server)
+> for pip to work correctly
+
+You can install the latest version with this command:
+
+``` {.bash}
+$ pip install --upgrade fast-oad
+```
+
+or, if you want the minimum installation without the CS25-related models:
+
+``` {.bash}
+$ pip install --upgrade fast-oad-core
+```
+
```

