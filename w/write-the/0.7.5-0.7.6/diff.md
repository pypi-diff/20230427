# Comparing `tmp/write_the-0.7.5.tar.gz` & `tmp/write_the-0.7.6.tar.gz`

## Comparing `write_the-0.7.5.tar` & `write_the-0.7.6.tar`

### file list

```diff
@@ -1,61 +1,66 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.5/mkdocs.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.7.5/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.7.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.7.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/CNAME
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/reference/cli.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/reference/cst.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/reference/docs.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/reference/mkdocs.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/reference/tests.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.5/docs/reference/utils.md
--rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.7.5/images/docs-help.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.7.5/images/logo-black.svg
--rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.7.5/images/logo.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.5/images/mkdocs-help.png
--rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.5/images/multiply-docs-tests.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.5/images/tests-help.png
--rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.7.5/images/untitled.blend
--rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.7.5/images/untitled.blend1
--rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.7.5/images/write-the-docs.gif
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.5/images/write-the-icon.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.7.5/images/write-the.svg
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_cli_main.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_cst_utils.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/test_utils.py
--rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/data/expected.dat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/data/multiply.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.5/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/__main__.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cli/__init__.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cli/main.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cli/tasks.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/cst/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/docs/__init__.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/docs/chain.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/docs/write.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/mkdocs/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/mkdocs/write.py
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/tests/__init__.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/tests/chain.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 write_the-0.7.5/write_the/tests/write.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 write_the-0.7.5/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.5/LICENSE.txt
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 write_the-0.7.5/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 write_the-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 write_the-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.6/mkdocs.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.7.6/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.7.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.7.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/CNAME
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/cli.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/cst.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/docs.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/mkdocs.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/tests.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/utils.md
+-rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.7.6/images/docs-help.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.7.6/images/logo-black.svg
+-rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.7.6/images/logo.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.6/images/mkdocs-help.png
+-rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.6/images/multiply-docs-tests.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.6/images/tests-help.png
+-rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.7.6/images/untitled.blend
+-rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.7.6/images/untitled.blend1
+-rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.7.6/images/write-the-docs.gif
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.6/images/write-the-icon.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.7.6/images/write-the.svg
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cli_main.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_utils.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_utils.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/calculate.py
+-rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/expected.dat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/multiply.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/__main__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/llm.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cli/main.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cli/tasks.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/__init__.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/docs.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/prompts.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/mkdocs/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/mkdocs/mkdocs.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/mkdocs/templates.py
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/tests/prompts.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/tests/tests.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 write_the-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.6/LICENSE.txt
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 write_the-0.7.6/README.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 write_the-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 write_the-0.7.6/PKG-INFO
```

### Comparing `write_the-0.7.5/mkdocs.yml` & `write_the-0.7.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/.github/workflows/publish.yml` & `write_the-0.7.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/.github/workflows/tests.yml` & `write_the-0.7.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/docs/index.md` & `write_the-0.7.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/docs-help.png` & `write_the-0.7.6/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/logo-black.svg` & `write_the-0.7.6/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/logo.png` & `write_the-0.7.6/images/logo.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/mkdocs-help.png` & `write_the-0.7.6/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/multiply-docs-tests.png` & `write_the-0.7.6/images/multiply-docs-tests.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/tests-help.png` & `write_the-0.7.6/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/untitled.blend` & `write_the-0.7.6/images/untitled.blend`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/untitled.blend1` & `write_the-0.7.6/images/untitled.blend1`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/write-the-docs.gif` & `write_the-0.7.6/images/write-the-docs.gif`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/write-the-icon.svg` & `write_the-0.7.6/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/images/write-the.svg` & `write_the-0.7.6/images/write-the.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/tests/test_cli_main.py` & `write_the-0.7.6/tests/test_cli_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from write_the.__about__ import __version__
 from pathlib import Path
 from write_the.cli.main import app
-from write_the.docs.chain import run
+from write_the.llm import LLM
 from typer.testing import CliRunner
 import unittest.mock as mock
 
 
 @pytest.fixture(scope='function')
 def file_path(tmp_path) -> Path:
     temp_file = tmp_path / "test_add.py"
@@ -32,15 +32,15 @@
         (True, True, True, True),
         (True, True, True, False),
         (True, True, False, True),
         (True, False, True, True),
         (False, True, True, True),
     ],
 )
-@mock.patch('write_the.docs.write.run', return_value="\n\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n")
+@mock.patch('write_the.llm.LLM.run', return_value="\n\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n")
 def test_docs_mocked(mocked_run, file_path: Path, nodes, save, context, pretty, force):
     runner = CliRunner()
     args = ["docs", str(file_path)]
 
     if nodes:
         for node in nodes:
             args.append("--node")
@@ -86,15 +86,15 @@
         (True, True, True),
         (True, True, True),
         (True, True, False),
         (True, False, True),
         (False, True, True),
     ],
 )
-@mock.patch('write_the.tests.write.run', return_value="""@pytest.mark.parametrize(
+@mock.patch('write_the.llm.LLM.run', return_value="""@pytest.mark.parametrize(
     "a, b, expected", [(2, 3, 5), (0, 5, 5), (-2, -3, -5), (2.5, 3, 5.5), (2, -3, -1)]
 )
 def test_add(a, b, expected):
     assert add(a, b) == expected""")
 def test_tests_mocked(mocked_run, file_path: Path, save, pretty, force):
     runner = CliRunner()
     test_dir = file_path.parent / 'docs'
```

### Comparing `write_the-0.7.5/tests/test_cst_docstring_adder.py` & `write_the-0.7.6/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/tests/test_cst_docstring_remover.py` & `write_the-0.7.6/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/tests/test_cst_function_and_class_collector.py` & `write_the-0.7.6/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/tests/test_cst_node_extractor.py` & `write_the-0.7.6/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/tests/test_cst_node_remover.py` & `write_the-0.7.6/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/tests/test_cst_utils.py` & `write_the-0.7.6/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/tests/test_utils.py` & `write_the-0.7.6/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def directory():
     return Path("tests/data")
 
 
 def test_list_python_files(directory):
     python_files = list_python_files(directory)
     assert isinstance(python_files, list)
-    assert len(python_files) == 2
+    assert len(python_files) == 3
     assert Path("tests/data/multiply_docstring.py") in python_files
     assert Path("tests/data/multiply.py") in python_files
 
 
 @pytest.mark.parametrize(
     "directory, expected",
     [
```

### Comparing `write_the-0.7.5/tests/data/expected.dat` & `write_the-0.7.6/tests/data/expected.dat`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/write_the/utils.py` & `write_the-0.7.6/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/write_the/cli/main.py` & `write_the-0.7.6/write_the/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import typer
 import os
 from write_the.__about__ import __version__
-from write_the.tests import write_the_tests
-from write_the.mkdocs import write_the_mkdocs
+from write_the.commands import write_the_tests, write_the_mkdocs
 from write_the.utils import list_python_files
 from pathlib import Path
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from typing import List, Optional
 from black import InvalidInput
@@ -118,16 +117,16 @@
 ):
     """
     Generate a mkdocs website for a project including the API reference.
     """
     write_the_mkdocs(code_dir=code_dir, readme=readme, out_dir=out_dir)
 
 
-@app.command()
-def tests(
+@app.async_command()
+async def tests(
     file: Path = typer.Argument(..., help="Path to the code file/folder."),
     tests_dir: Path = typer.Option(
         'tests', "--out", "-o", help="Path to save the docs."
     ),
     save: bool = typer.Option(
         False, "--save/--print", "-s", help="Save the tests to the tests directory or print to stdout."
     ),
@@ -172,15 +171,15 @@
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             transient=True,
         ) as progress:
             failed = False
             progress.add_task(description=f"{file}", total=None)
             try:
-                result = write_the_tests(file, gpt_4=gpt_4)
+                result = await write_the_tests(file, gpt_4=gpt_4)
             except InvalidInput:
                 failed = True
                 result = ""
             progress.stop()
             if len(files) > 1 or save or failed:
                 icon = "❌" if failed else "✅"
                 colour = "red" if failed else "green"
```

### Comparing `write_the-0.7.5/write_the/cli/tasks.py` & `write_the-0.7.6/write_the/cli/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from write_the.docs.write import write_the_docs
+from write_the.commands import write_the_docs
 from write_the.utils import create_tree, format_source_code, load_source_code
 from rich.syntax import Syntax
 from rich.progress import Progress
 from typing import List
 from pathlib import Path
 
 
@@ -56,23 +56,23 @@
             batch=batch,
         )
     except Exception as e:
         print(e)
         failed = True
     progress.remove_task(task_id)
     progress.refresh()
-    if failed:
-        return None
     if print_status or save or failed:
         icon = "❌" if failed else "✅"
         colour = "red" if failed else "green"
         progress.print(
             f"[not underline]{icon} [/not underline]{file}",
             style=f"bold {colour} underline",
         )
+    if failed:
+        return None
     if save:
         with open(file, "w") as f:
             f.writelines(result)
         return None
     if pretty:
         syntax = Syntax(result, "python")
         progress.print(syntax)
```

### Comparing `write_the-0.7.5/write_the/cst/docstring_adder.py` & `write_the-0.7.6/write_the/cst/docstring_adder.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,7 +64,10 @@
             dedented_docstring = textwrap.dedent(escaped_docstring)
             indented_docstring = textwrap.indent(dedented_docstring, '    ')
             new_docstring = cst.parse_statement(f'"""{indented_docstring}    """')
             body = node.body.with_changes(body=[new_docstring] + list(node.body.body))
             return node.with_changes(body=body)
         
         return node
+
+def add_docstrings_to_tree(tree, docstring_dict, force=False):
+    return tree.visit(DocstringAdder(docstring_dict, force))
```

### Comparing `write_the-0.7.5/write_the/cst/docstring_remover.py` & `write_the-0.7.6/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/write_the/cst/function_and_class_collector.py` & `write_the-0.7.6/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/write_the/cst/node_extractor.py` & `write_the-0.7.6/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/write_the/cst/node_remover.py` & `write_the-0.7.6/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/write_the/cst/utils.py` & `write_the-0.7.6/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/write_the/docs/write.py` & `write_the-0.7.6/write_the/commands/docs/docs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,18 @@
 import libcst as cst
 from black import format_str, FileMode
 
 from write_the.cst import nodes_to_tree
-from write_the.cst.docstring_adder import DocstringAdder
+from write_the.cst.docstring_adder import add_docstrings_to_tree
 from write_the.cst.docstring_remover import remove_docstrings
 from write_the.cst.function_and_class_collector import get_node_names
 from write_the.cst.node_extractor import extract_nodes_from_tree
-from write_the.cst.node_remover import remove_nodes_from_tree
-from write_the.docs.chain import run
-
-
-def process_nodes(tree: cst.Module, nodes, context, extract_specific_nodes) -> str:
-    """
-    Processes a tree of nodes.
-    Args:
-      tree (cst.Module): The tree of nodes to process.
-      nodes (list): The list of nodes to process.
-      context (bool): Whether to include context nodes.
-      extract_specific_nodes (bool): Whether to extract specific nodes.
-    Returns:
-      str: The processed tree as a string.
-    Examples:
-      >>> process_nodes(tree, nodes, context, extract_specific_nodes)
-      "Processed tree as a string"
-    """
-    tree_without_docstrings = remove_docstrings(tree, nodes)
-    if not context:
-        if extract_specific_nodes:
-            extracted_nodes = extract_nodes_from_tree(tree_without_docstrings, nodes)
-            processed_tree = nodes_to_tree(extracted_nodes)
-        else:
-            all_nodes = get_node_names(tree, False)
-            nodes_to_remove = [n for n in all_nodes if n not in nodes]
-            processed_tree = remove_nodes_from_tree(
-                tree_without_docstrings, nodes_to_remove
-            )
-        code = processed_tree.code
-    else:
-        code = tree_without_docstrings.code
-
-    return code
+from write_the.commands.docs.utils import extract_block, process_nodes
+from write_the.llm import LLM
+from .prompts import write_docstings_for_nodes_prompt
 
 
 async def write_the_docs(
     tree: cst.Module,
     nodes=[],
     force=False,
     save=False,
@@ -81,24 +50,19 @@
     if nodes:
         extract_specific_nodes = True
         force = True
     else:
         nodes = get_node_names(tree, force)
     if not nodes:
         return tree.code
-
-    code = process_nodes(tree, nodes, context, extract_specific_nodes)
-    result = await run(code=code, nodes=nodes)
-    docstring_dict = {}
-    for line in result.split("\n\n"):
-        line = line.strip()
-        if not line:
-            continue
-        (node_name, docsting) = line.split(":", 1)
-        docstring_dict[node_name] = docsting + "\n"
-    modified_tree = tree.visit(DocstringAdder(docstring_dict, force))
+    tree_without_docstrings = remove_docstrings(tree, nodes)
+    code = process_nodes(tree_without_docstrings, nodes, context, extract_specific_nodes)
+    llm = LLM(write_docstings_for_nodes_prompt)
+    result = await llm.run(code=code, nodes=nodes)
+    docstring_dict = extract_block(result, nodes)
+    modified_tree = add_docstrings_to_tree(tree, docstring_dict, force=force)
     if not save and extract_specific_nodes:
         extracted_nodes = extract_nodes_from_tree(modified_tree, nodes)
         modified_tree = nodes_to_tree(extracted_nodes)
     if pretty:
         return format_str(modified_tree.code, mode=FileMode())
     return modified_tree.code
```

### Comparing `write_the-0.7.5/write_the/tests/write.py` & `write_the-0.7.6/write_the/commands/tests/tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from black import format_str, FileMode
-from .chain import run
+from .prompts import write_tests_for_file_prompt
+from write_the.llm import LLM
 
-
-def write_the_tests(
+async def write_the_tests(
     filename: Path,
     gpt_4: bool = False
 ) -> str:
     """
     Formats and runs the tests for a given file.
     Args:
       filename (Path): The path to the file to be tested.
@@ -17,10 +17,11 @@
     Examples:
       >>> write_the_tests(Path("test.py"), gpt_4=True)
       "Formatted and tested code"
     """
     with open(filename, "r") as file:
         source_code = file.read()
     source_code = format_str(source_code, mode=FileMode())
-    result = run(code=source_code, path=filename, gpt_4=gpt_4)
+    llm = LLM(write_tests_for_file_prompt, gpt_4=gpt_4)
+    result = await llm.run(code=source_code, path=filename)
     code = result.strip().lstrip("Test Code:\n```python").lstrip("```python").lstrip("```").rstrip("```")
     return format_str(code, mode=FileMode())
```

### Comparing `write_the-0.7.5/LICENSE.txt` & `write_the-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/README.md` & `write_the-0.7.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ## Real-world examples
 
 - [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
 - [`write-the mkdocs` to build the documentation site for `write-the` 🤖](https://write-the.wytamma.com/)
 - [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
-
+- [`write-the docs` and `write-the mkdocs` to build documenation for `CUPCAKEAGI` 🤖](https://github.com/AkshitIreddy/CUPCAKEAGI/pull/4)
 
 ## Installation
 ```console
 pip install write-the
 ```
 ## Features
```

### Comparing `write_the-0.7.5/pyproject.toml` & `write_the-0.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.5/PKG-INFO` & `write_the-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.7.5
+Version: 0.7.6
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -44,15 +44,15 @@
 ## Real-world examples
 
 - [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
 - [`write-the mkdocs` to build the documentation site for `write-the` 🤖](https://write-the.wytamma.com/)
 - [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
-
+- [`write-the docs` and `write-the mkdocs` to build documenation for `CUPCAKEAGI` 🤖](https://github.com/AkshitIreddy/CUPCAKEAGI/pull/4)
 
 ## Installation
 ```console
 pip install write-the
 ```
 ## Features
```

