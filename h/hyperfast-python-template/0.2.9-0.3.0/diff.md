# Comparing `tmp/hyperfast_python_template-0.2.9.tar.gz` & `tmp/hyperfast_python_template-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.2.9.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.3.0.tar", max compression
```

## Comparing `hyperfast_python_template-0.2.9.tar` & `hyperfast_python_template-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-04-21 00:05:51.214146 hyperfast_python_template-0.2.9/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-21 00:05:44.734172 hyperfast_python_template-0.2.9/README.md
--rw-r--r--   0        0        0     2942 2023-04-21 00:06:12.214193 hyperfast_python_template-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-27 07:14:25.134899 hyperfast_python_template-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-27 07:14:18.682906 hyperfast_python_template-0.3.0/README.md
+-rw-r--r--   0        0        0     3112 2023-04-27 07:14:40.554888 hyperfast_python_template-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.3.0/PKG-INFO
```

### Comparing `hyperfast_python_template-0.2.9/LICENSE` & `hyperfast_python_template-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.9/README.md` & `hyperfast_python_template-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.9/pyproject.toml` & `hyperfast_python_template-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,90 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.2.9"
+version = "0.3.0"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
 
 [tool.poetry.scripts]
 hyperfastpy = 'hyperfastpy.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 
+[tool.poetry.group.dev]
+optional = true
+
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
-setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
+[tool.poe]
+include = ".tasks.toml"
+
 [tool.black]
-exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+exclude = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.isort]
 profile = "black"
-skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+skip = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.flake8]
 ignore = ['F401', 'E501', 'W503']
-exclude = ["node_modules", "_build", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "_build",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
-exclude = ["node_modules", "build", "_build", "dist", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "build",
+    "_build",
+    "dist",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+]
 # 3rd party import
 ignore_missing_imports = true
 # dynamic typing
 disallow_any_unimported = true
 disallow_any_expr = false
 disallow_any_decorated = false
 disallow_any_explicit = true
@@ -69,33 +110,31 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
 [tool.setuptools_scm]
-write_to = "src/hyperfastpy/_version.py"
 write_to_template = '__version__ = "{version}"'
 tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_source = "tag"
-commit_version_number = true # required for version_source = "tag"
+commit_version_number = true                                    # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
-hvcs = "github" # hosting version control system, gitlab is also supported
+hvcs = "github"                                                 # hosting version control system, gitlab is also supported
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools>=45", "setuptools_scm[toml]>=6.2"]
-build-backend = 'setuptools.build_meta'
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hyperfast_python_template-0.2.9/PKG-INFO` & `hyperfast_python_template-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.2.9
+Version: 0.3.0
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

