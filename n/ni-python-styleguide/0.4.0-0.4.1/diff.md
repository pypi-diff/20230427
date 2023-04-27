# Comparing `tmp/ni_python_styleguide-0.4.0.tar.gz` & `tmp/ni_python_styleguide-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_python_styleguide-0.4.0.tar", max compression
+gzip compressed data, was "ni_python_styleguide-0.4.1.tar", max compression
```

## Comparing `ni_python_styleguide-0.4.0.tar` & `ni_python_styleguide-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1089 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/LICENSE
--rw-r--r--   0        0        0     2046 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/README.md
--rw-r--r--   0        0        0      214 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/__init__.py
--rw-r--r--   0        0        0      164 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/__main__.py
--rw-r--r--   0        0        0     5292 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_acknowledge_existing_errors/__init__.py
--rw-r--r--   0        0        0     5948 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_cli.py
--rw-r--r--   0        0        0      192 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_config_constants.py
--rw-r--r--   0        0        0     5240 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_fix.py
--rw-r--r--   0        0        0     1001 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_format.py
--rw-r--r--   0        0        0     1652 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_lint.py
--rw-r--r--   0        0        0      184 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/__init__.py
--rw-r--r--   0        0        0      806 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/code_analysis.py
--rw-r--r--   0        0        0     3084 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/lint.py
--rw-r--r--   0        0        0     2109 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/string_helpers.py
--rw-r--r--   0        0        0      518 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/temp_file.py
--rw-r--r--   0        0        0     3535 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/config.ini
--rw-r--r--   0        0        0      337 2023-01-20 14:41:50.846255 ni_python_styleguide-0.4.0/ni_python_styleguide/config.toml
--rw-r--r--   0        0        0     2000 2023-01-20 14:42:40.106124 ni_python_styleguide-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.0/setup.py
--rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2046 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/README.md
+-rw-r--r--   0        0        0      214 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/__main__.py
+-rw-r--r--   0        0        0     6940 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_acknowledge_existing_errors/__init__.py
+-rw-r--r--   0        0        0     5948 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_cli.py
+-rw-r--r--   0        0        0      192 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_config_constants.py
+-rw-r--r--   0        0        0     5240 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_fix.py
+-rw-r--r--   0        0        0     1001 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_format.py
+-rw-r--r--   0        0        0     1652 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_lint.py
+-rw-r--r--   0        0        0      184 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/__init__.py
+-rw-r--r--   0        0        0      806 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/code_analysis.py
+-rw-r--r--   0        0        0     3131 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/lint.py
+-rw-r--r--   0        0        0     2109 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/string_helpers.py
+-rw-r--r--   0        0        0      518 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/temp_file.py
+-rw-r--r--   0        0        0     3667 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/config.ini
+-rw-r--r--   0        0        0      337 2023-04-27 20:00:42.163305 ni_python_styleguide-0.4.1/ni_python_styleguide/config.toml
+-rw-r--r--   0        0        0     1856 2023-04-27 20:01:26.687750 ni_python_styleguide-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.1/setup.py
+-rw-r--r--   0        0        0     3158 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.1/PKG-INFO
```

### Comparing `ni_python_styleguide-0.4.0/LICENSE` & `ni_python_styleguide-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/README.md` & `ni_python_styleguide-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_acknowledge_existing_errors/__init__.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_acknowledge_existing_errors/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 import logging
 import pathlib
 import re
 from collections import defaultdict
 
-from ni_python_styleguide import _format
-from ni_python_styleguide import _utils
+from ni_python_styleguide import _format, _utils
 
 _module_logger = logging.getLogger(__name__)
 
 EXCLUDED_ERRORS = {
     "BLK100",
 }
 
 
 def _add_noqa_to_line(lineno, code_lines, error_code, explanation):
     line = code_lines[lineno]
     old_line_ending = "\n" if line.endswith("\n") else ""
     line = line.rstrip("\n")
 
-    if f"noqa {error_code}" not in line:
+    if f"noqa: {error_code}" not in line:
         prefix = "  " if line.strip() else ""
-        line += f"{prefix}# noqa {error_code}: {explanation} (auto-generated noqa)"
+        code, _, existing = line.partition("# noqa:")
+
+        existing_codes, _, existing_explanations = existing.partition(" - ")
+        if existing_codes:
+            error_code = existing_codes + ", " + error_code
+            explanation = f"{existing_explanations}, {explanation} (auto-generated noqa)"
+        else:
+            explanation = explanation + " (auto-generated noqa)"
+
+        line = f"{code.rstrip()}{prefix}# noqa: {error_code.lstrip()} - {explanation}"
 
     code_lines[lineno] = line + old_line_ending
 
 
 def _filter_suppresion_from_line(line: str):
     if "(auto-generated noqa)" in line:
-        return re.sub(r"# noqa .+\(auto-generated noqa\)", "", line).rstrip()
+        return re.sub(r"# noqa:? .+\(auto-generated noqa\)$", "", line).rstrip()
     else:
         return line
 
 
 def acknowledge_lint_errors(
     exclude, app_import_names, extend_ignore, file_or_dir, *_, aggressive=False
 ):
@@ -52,14 +60,16 @@
     for error in lint_errors_to_process:
         lint_errors_by_file[pathlib.Path(error.file)].append(error)
 
     failed_files = []
     for bad_file, errors_in_file in lint_errors_by_file.items():
         _suppress_errors_in_file(bad_file, errors_in_file, encoding=_utils.DEFAULT_ENCODING)
 
+        _handle_emergent_violations(exclude, app_import_names, extend_ignore, file_or_dir, bad_file)
+
         if aggressive:
             # some cases are expected to take up to 4 passes, making this 2x rounded
             per_file_format_iteration_limit = 10
             for _ in range(per_file_format_iteration_limit):
                 # format the files - this may move the suppression off the correct lines
                 #  Note: due to Github pycodestyle#868, we have to format, change, format
                 #   (check if that time made changes)
@@ -77,26 +87,55 @@
                     excluded_errors=EXCLUDED_ERRORS,
                 )
 
                 _suppress_errors_in_file(
                     bad_file, current_lint_errors, encoding=_utils.DEFAULT_ENCODING
                 )
 
+                remaining_errors = _handle_emergent_violations(
+                    exclude=exclude,
+                    app_import_names=app_import_names,
+                    extend_ignore=extend_ignore,
+                    file_or_dir=file_or_dir,
+                    bad_file=bad_file,
+                )
+
                 changed = _format.format_check(bad_file)
-                if not changed:  # are we done?
+                if not changed and not remaining_errors:  # are we done?
                     break
             else:
                 failed_files.append(
                     f"Could not handle suppressions/formatting of file {bad_file} after maximum number of tries ({per_file_format_iteration_limit})"
                 )
                 _module_logger.warning("Max tries reached on %s", bad_file)
     if failed_files:
         raise RuntimeError("Could not handle some files:\n" + "\n\n".join(failed_files) + "\n\n\n")
 
 
+def _handle_emergent_violations(exclude, app_import_names, extend_ignore, file_or_dir, bad_file):
+    """Some errors can be created by adding the acknowledge comments handle those now.
+
+    Example emergent violations:
+      W505 -> due to adding comment to docstring
+    """
+    current_lint_errors = set(
+        _utils.lint.get_errors_to_process(
+            exclude=exclude,
+            app_import_names=app_import_names,
+            extend_ignore=extend_ignore,
+            file_or_dir=file_or_dir,
+            excluded_errors=EXCLUDED_ERRORS,
+        )
+    )
+    errors_to_process_now = set(filter(lambda o: o.code in {"W505"}, current_lint_errors))
+    _suppress_errors_in_file(bad_file, errors_to_process_now, encoding=_utils.DEFAULT_ENCODING)
+    remaining_errors = current_lint_errors - errors_to_process_now
+    return remaining_errors
+
+
 def remove_auto_suppressions_from_file(file: pathlib.Path):
     """Removes auto-suppressions from file."""
     lines = file.read_text(encoding=_utils.DEFAULT_ENCODING).splitlines()
     stripped_lines = [_filter_suppresion_from_line(line) for line in lines]
     file.write_text("\n".join(stripped_lines) + "\n", encoding=_utils.DEFAULT_ENCODING)
```

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_cli.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_cli.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_fix.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_fix.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_format.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_format.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_lint.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_lint.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/code_analysis.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/code_analysis.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/lint.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/lint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import re
-from collections import namedtuple
+import typing
 
 from ni_python_styleguide import _lint
 
 
 def get_errors_to_process(exclude, app_import_names, extend_ignore, file_or_dir, excluded_errors):
     """Get lint errors to process."""
     lint_errors = sorted(
@@ -19,15 +19,22 @@
     )
     parsed_errors = map(parse, lint_errors)
     parsed_errors = list(filter(None, parsed_errors))
     lint_errors_to_process = [error for error in parsed_errors if error.code not in excluded_errors]
     return lint_errors_to_process
 
 
-LintError = namedtuple("LintError", ["file", "line", "column", "code", "explanation"])
+class LintError(typing.NamedTuple):
+    """Class defining a lint error."""
+
+    file: str
+    line: int
+    column: int
+    code: str
+    explanation: str
 
 
 def parse(line):
     r"""
     Parses line into :class:`LintError`.
 
     >>> parse(r'source\arfile.py:55:16: BLK100 Black would make changes.')
```

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/string_helpers.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/string_helpers.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/_utils/temp_file.py` & `ni_python_styleguide-0.4.1/ni_python_styleguide/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.0/ni_python_styleguide/config.ini` & `ni_python_styleguide-0.4.1/ni_python_styleguide/config.ini`

 * *Files 13% similar despite different names*

```diff
@@ -97,14 +97,17 @@
     D407
     D408
     D409
     D413
     # flake8-import-order
     I101  #  The names in your from import are in the wrong order. (Enforced by E401)
 
+# We want to ignore missing docstrings in test methods as they are self documenting
+per-file-ignores= tests/**/test_*.py:D100,D103
+
 # Flake8 includes mccabe by default.
 # We have yet to evaluate it, so ignore the errors for now
 extend-ignore=C90
 
 # flake8-docstrings
 docstring-convention=all
```

### Comparing `ni_python_styleguide-0.4.0/pyproject.toml` & `ni_python_styleguide-0.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "ni-python-styleguide"
 # The -alpha.0 here denotes a source based version
 # This is removed when released through the Publish-Package.yml GitHub action
 # Official PyPI releases follow Major.Minor.Patch
-version = "0.4.0"
+version = "0.4.1"
 description = "NI's internal and external Python linter rules and plugins"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md" # apply the repo readme to the package as well
 repository = "https://github.com/ni/python-styleguide"
 license = "MIT"
 include = ["ni_python_styleguide/config.toml"]
 
+
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # Tools we aggregate
 flake8 = "^5.0"
-black = ">=22.3, !=22.10.0"  # https://github.com/psf/black/issues/3312
+black = ">=23.1"
 
 # Additional support libraries
 # These dependencies were selected because they are already used by black.
 click = ">=7.1.2"
 toml = ">=0.10.1"
 isort = ">=5.10"
 
-
 # flake8 plugins should be listed here (in alphabetical order)
 flake8-black = ">=0.2.1"
 flake8-docstrings = ">=1.5.0"
 flake8-import-order = ">=0.18.1"
 pep8-naming = ">=0.11.1"
 
 # Rejected flake8 plugins should be listed here (in alphabetical order)
@@ -36,34 +36,35 @@
 # flake8-commas: Already handled by flake8-black
 # flake8-isort: Already covered by flake8-import-order
 # hacking: Most rules are either covered by other plugins or would be turned off.
 
 # Tooling that we're locking so our tool can run
 importlib-metadata = {version= "<5.0", python="<3.8"}
 
+
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0.1"
 pytest_click = ">=1.0.2"
 pytest-snapshot = ">=0.6.3"
 
+
 [tool.poetry.scripts]
 ni-python-styleguide = 'ni_python_styleguide._cli:main'
 
+
 [tool.black]
 line-length = 100
-extend-exclude = '''
-(
-/.*__snapshots/.*output\.py # exclude the simple snapshot outputs
-)
-'''
+
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 norecursedirs = "*__snapshots"
 
+
 [tool.ni-python-styleguide]
 extend_exclude = "*__snapshots/*/*input.py"
 
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `ni_python_styleguide-0.4.0/setup.py` & `ni_python_styleguide-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  'ni_python_styleguide._acknowledge_existing_errors',
  'ni_python_styleguide._utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['black>=22.3,!=22.10.0',
+['black>=23.1',
  'click>=7.1.2',
  'flake8-black>=0.2.1',
  'flake8-docstrings>=1.5.0',
  'flake8-import-order>=0.18.1',
  'flake8>=5.0,<6.0',
  'isort>=5.10',
  'pep8-naming>=0.11.1',
@@ -24,15 +24,15 @@
 {':python_version < "3.8"': ['importlib-metadata<5.0']}
 
 entry_points = \
 {'console_scripts': ['ni-python-styleguide = ni_python_styleguide._cli:main']}
 
 setup_kwargs = {
     'name': 'ni-python-styleguide',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': "NI's internal and external Python linter rules and plugins",
     'long_description': '# NI Python Style Guide\n\n![logo](https://raw.githubusercontent.com/ni/python-styleguide/main/docs/logo.svg)\n\n---\n\n[![PyPI version](https://badge.fury.io/py/ni-python-styleguide.svg)](https://badge.fury.io/py/ni-python-styleguide) ![Publish Package](https://github.com/ni/python-styleguide/workflows/Publish%20Package/badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\nWelcome to NI\'s internal and external Python conventions and enforcement tooling.\n\n## Written Conventions\n\nOur written conventions can be found at https://ni.github.io/python-styleguide/.\n\nTheir source is in [docs/Coding-Conventions.md](https://github.com/ni/python-styleguide/tree/main/docs/Coding-Conventions.md).\n\nNOTE: Using the GitHub Pages link is preferable to a GitHub `/blob` link.\n\n## Enforcement tooling\n\nAs a tool, `ni-python-styleguide` is installed like any other script:\n\n```bash\npip install ni-python-styleguide\n```\n\n### Linting\n\nTo lint, just run the `lint` subcommand (from within the project root, or lower):\n\n```bash\nni-python-styleguide lint\n# or\nni-python-styleguide lint ./dir/\n# or\nni-python-styleguide lint module.py\n```\n\nThe rules enforced are all rules documented in the written convention, which are marked as enforced.\n\n### Configuration\n\n`ni-python-styleguide` aims to keep the configuration to a bare minimum (none wherever possible).\nHowever there are some situations you might need to configure the tool.\n\n#### When using `setup.py`\n\nIf you\'re using `setup.py`, you\'ll need to set your app\'s import names for import sorting.\n\n```toml\n# pyproject.toml\n[tool.ni-python-styleguide]\napplication-import-names = "<app_name>"\n```\n\n### Formatting\n\n`ni-python-styleguide` in the future will have a `format` command which we intend to fix as many lint issues as possible.\n\nUntil then you\'ll want to set the following to get `black` formatting as the styleguide expects.\n\n```toml\n# pyproject.toml\n[tool.black]\nline-length = 100\n```\n\n### Editor Integration\n\n(This section to come!)\n',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/python-styleguide',
```

### Comparing `ni_python_styleguide-0.4.0/PKG-INFO` & `ni_python_styleguide-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ni-python-styleguide
-Version: 0.4.0
+Version: 0.4.1
 Summary: NI's internal and external Python linter rules and plugins
 Home-page: https://github.com/ni/python-styleguide
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=22.3,!=22.10.0)
+Requires-Dist: black (>=23.1)
 Requires-Dist: click (>=7.1.2)
 Requires-Dist: flake8 (>=5.0,<6.0)
 Requires-Dist: flake8-black (>=0.2.1)
 Requires-Dist: flake8-docstrings (>=1.5.0)
 Requires-Dist: flake8-import-order (>=0.18.1)
 Requires-Dist: importlib-metadata (<5.0); python_version < "3.8"
 Requires-Dist: isort (>=5.10)
```

