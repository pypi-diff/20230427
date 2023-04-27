# Comparing `tmp/setuptools-rust-1.5.2.tar.gz` & `tmp/setuptools-rust-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-rust-1.5.2.tar", last modified: Mon Sep 19 19:44:07 2022, max compression
+gzip compressed data, was "setuptools-rust-1.6.0.tar", last modified: Thu Apr 27 20:50:21 2023, max compression
```

## Comparing `setuptools-rust-1.5.2.tar` & `setuptools-rust-1.6.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.104003 setuptools-rust-1.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.104003 setuptools-rust-1.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)    15573 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    12304 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.104003 setuptools-rust-1.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/building_wheels.md
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.104003 setuptools-rust-1.5.2/emscripten/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/emscripten/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/emscripten/_sysconfigdata__emscripten_wasm32-emscripten.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      537 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/emscripten/emcc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/emscripten/pyo3_config.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/emscripten/runner.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.100003 setuptools-rust-1.5.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.104003 setuptools-rust-1.5.2/examples/hello-world/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/hello-world/hello_world/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/hello-world/src/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/hello-world-script/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/hello-world-script/hello_world/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/hello-world-script/src/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/hello-world-script/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/html-py-ever/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.100003 setuptools-rust-1.5.2/examples/html-py-ever/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/html-py-ever/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/.github/workflows/upload.yml
--rw-r--r--   0 runner    (1001) docker     (121)    17533 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10859 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      632 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/build-wheels.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/html-py-ever/html_py_ever/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/html_py_ever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      182 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.108003 setuptools-rust-1.5.2/examples/html-py-ever/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.112004 setuptools-rust-1.5.2/examples/html-py-ever/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/empty.html
--rw-r--r--   0 runner    (1001) docker     (121)   325989 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/monty-python.html
--rw-r--r--   0 runner    (1001) docker     (121)  1762191 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/python.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     1819 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (121)   693144 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/rust.html
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/small.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      733 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/test_parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      621 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/html-py-ever/tests/test_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.112004 setuptools-rust-1.5.2/examples/namespace_package/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.112004 setuptools-rust-1.5.2/examples/namespace_package/.cargo/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (121)     6559 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/Cross.toml
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.100003 setuptools-rust-1.5.2/examples/namespace_package/namespace_package/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.112004 setuptools-rust-1.5.2/examples/namespace_package/namespace_package/python/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/namespace_package/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.112004 setuptools-rust-1.5.2/examples/namespace_package/src/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.112004 setuptools-rust-1.5.2/examples/namespace_package/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/namespace_package/tests/test_namespace_package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.112004 setuptools-rust-1.5.2/examples/rust_with_cffi/
--rw-r--r--   0 runner    (1001) docker     (121)     6551 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/cffi_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/examples/rust_with_cffi/rust_with_cffi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/rust_with_cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/examples/rust_with_cffi/src/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/examples/rust_with_cffi/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/examples/rust_with_cffi/tests/test_rust_with_cffi.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3988 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       92 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/setuptools_rust/
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    26628 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     4571 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/command.py
--rw-r--r--   0 runner    (1001) docker     (121)    14253 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/extension.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/rustc_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12604 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/setuptools_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/setuptools_rust/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/setuptools_rust.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-09-19 19:44:07.000000 setuptools-rust-1.5.2/setuptools_rust.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-09-19 19:44:07.000000 setuptools-rust-1.5.2/setuptools_rust.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 19:44:07.000000 setuptools-rust-1.5.2/setuptools_rust.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-19 19:44:07.000000 setuptools-rust-1.5.2/setuptools_rust.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-19 19:44:07.000000 setuptools-rust-1.5.2/setuptools_rust.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-19 19:44:07.000000 setuptools-rust-1.5.2/setuptools_rust.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 19:44:07.000000 setuptools-rust-1.5.2/setuptools_rust.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 19:44:07.116004 setuptools-rust-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-09-19 19:43:59.000000 setuptools-rust-1.5.2/tests/test_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.898828 setuptools-rust-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.866828 setuptools-rust-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.866828 setuptools-rust-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-27 20:50:21.898828 setuptools-rust-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.866828 setuptools-rust-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/building_wheels.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.870828 setuptools-rust-1.6.0/emscripten/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/emscripten/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/emscripten/_sysconfigdata__emscripten_wasm32-emscripten.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/emscripten/emcc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/emscripten/pyo3_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/emscripten/runner.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.858828 setuptools-rust-1.6.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.870828 setuptools-rust-1.6.0/examples/hello-world/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.874828 setuptools-rust-1.6.0/examples/hello-world/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.874828 setuptools-rust-1.6.0/examples/hello-world/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.874828 setuptools-rust-1.6.0/examples/hello-world-script/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.874828 setuptools-rust-1.6.0/examples/hello-world-script/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.874828 setuptools-rust-1.6.0/examples/hello-world-script/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/hello-world-script/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.878828 setuptools-rust-1.6.0/examples/html-py-ever/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.858828 setuptools-rust-1.6.0/examples/html-py-ever/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.878828 setuptools-rust-1.6.0/examples/html-py-ever/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/build-wheels.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.878828 setuptools-rust-1.6.0/examples/html-py-ever/html_py_ever/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/html_py_ever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.878828 setuptools-rust-1.6.0/examples/html-py-ever/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.882828 setuptools-rust-1.6.0/examples/html-py-ever/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/empty.html
+-rw-r--r--   0 runner    (1001) docker     (123)   325989 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/monty-python.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1762191 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/python.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-04-27 20:50:09.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)   693144 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/rust.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/small.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/test_parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      621 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/html-py-ever/tests/test_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.886828 setuptools-rust-1.6.0/examples/namespace_package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.886828 setuptools-rust-1.6.0/examples/namespace_package/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/Cross.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.858828 setuptools-rust-1.6.0/examples/namespace_package/namespace_package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.886828 setuptools-rust-1.6.0/examples/namespace_package/namespace_package/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/namespace_package/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.886828 setuptools-rust-1.6.0/examples/namespace_package/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.886828 setuptools-rust-1.6.0/examples/namespace_package/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/namespace_package/tests/test_namespace_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.890828 setuptools-rust-1.6.0/examples/rust_with_cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/cffi_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.890828 setuptools-rust-1.6.0/examples/rust_with_cffi/rust_with_cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/rust_with_cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.890828 setuptools-rust-1.6.0/examples/rust_with_cffi/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.890828 setuptools-rust-1.6.0/examples/rust_with_cffi/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/examples/rust_with_cffi/tests/test_rust_with_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-27 20:50:21.898828 setuptools-rust-1.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.894828 setuptools-rust-1.6.0/setuptools_rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/rustc_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/setuptools_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/setuptools_rust/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.894828 setuptools-rust-1.6.0/setuptools_rust.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-27 20:50:21.000000 setuptools-rust-1.6.0/setuptools_rust.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-27 20:50:21.000000 setuptools-rust-1.6.0/setuptools_rust.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:50:21.000000 setuptools-rust-1.6.0/setuptools_rust.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 20:50:21.000000 setuptools-rust-1.6.0/setuptools_rust.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 20:50:21.000000 setuptools-rust-1.6.0/setuptools_rust.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 20:50:21.000000 setuptools-rust-1.6.0/setuptools_rust.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:50:21.000000 setuptools-rust-1.6.0/setuptools_rust.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:21.898828 setuptools-rust-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-27 20:50:10.000000 setuptools-rust-1.6.0/tests/test_extension.py
```

### Comparing `setuptools-rust-1.5.2/.github/workflows/ci.yml` & `setuptools-rust-1.6.0/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,95 +12,91 @@
 jobs:
   fmt:
     runs-on: "ubuntu-latest"
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - run: pip install black
 
       - run: black --check .
 
   mypy:
     runs-on: "ubuntu-latest"
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - run: pip install nox
 
       - run: nox -s mypy
 
   pytest:
     runs-on: "ubuntu-latest"
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - name: Install Rust toolchain
-        uses: actions-rs/toolchain@v1
-        with:
-          toolchain: stable
-          profile: minimal
-          default: true
+        uses: dtolnay/rust-toolchain@stable
 
       - run: pip install nox
 
       - run: nox -s test
 
   build:
     name:  ${{ matrix.python-version }} ${{ matrix.platform.os }}-${{ matrix.platform.python-architecture }}
     runs-on: ${{ matrix.platform.os }}
     strategy:
       # If one platform fails, allow the rest to keep testing if `CI-no-fail-fast` label is present
       fail-fast: ${{ !contains(github.event.pull_request.labels.*.name, 'CI-no-fail-fast') }}
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", pypy-3.7, pypy-3.8]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev", pypy-3.7, pypy-3.8, pypy-3.9]
         platform: [
           { os: "macos-latest",   python-architecture: "x64", rust-target: "x86_64-apple-darwin" },
           { os: "ubuntu-latest", python-architecture: "x64", rust-target: "x86_64-unknown-linux-gnu" },
           { os: "windows-latest", python-architecture: "x64", rust-target: "x86_64-pc-windows-msvc" },
           { os: "windows-latest", python-architecture: "x86", rust-target: "i686-pc-windows-msvc" },
         ]
         exclude:
           # No 32-bit pypy 3.7 on Windows
           - python-version: pypy-3.7
             platform: { os: "windows-latest", python-architecture: "x86" }
           # No 32-bit pypy 3.8 on Windows
           - python-version: pypy-3.8
             platform: { os: "windows-latest", python-architecture: "x86" }
+          # No 32-bit pypy 3.9 on Windows
+          - python-version: pypy-3.9
+            platform: { os: "windows-latest", python-architecture: "x86" }
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: ${{ matrix.platform.python-architecture }}
 
       - name: Install Rust toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@stable
         with:
-          toolchain: stable
-          target: ${{ matrix.platform.rust-target }}
-          profile: minimal
-          default: true
+          targets: ${{ matrix.platform.rust-target }}
 
       - name: Install Rust aarch64-apple-darwin target
         if: matrix.platform.os == 'macos-latest'
         run: rustup target add aarch64-apple-darwin
 
       - name: Install test dependencies
         run: pip install --upgrade nox
@@ -144,60 +140,66 @@
       # If one platform fails, allow the rest to keep testing if `CI-no-fail-fast` label is present
       fail-fast: ${{ !contains(github.event.pull_request.labels.*.name, 'CI-no-fail-fast') }}
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
     steps:
       - uses: actions/checkout@master
       - name: Setup python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.9
 
-      - uses: actions-rs/toolchain@v1
-        with:
-          profile: minimal
-          toolchain: stable
-          override: true
+      - uses: dtolnay/rust-toolchain@stable
 
       - name: Install Rust aarch64-apple-darwin target
         if: matrix.os == 'macos-latest'
         run: rustup target add aarch64-apple-darwin
 
       - name: Build package
         run: pip install -e .
 
       - name: Build an abi3 wheel
         shell: bash
         run: |
+          set -e
           cd examples/rust_with_cffi/
           python --version
           pip install -U wheel
           python setup.py bdist_wheel --py-limited-api=cp39
           ls -la dist/
         env:
           # https://github.com/actions/setup-python/issues/26
           MACOSX_DEPLOYMENT_TARGET: 10.9
 
       # Now we switch to a differnet Python version and ensure we can install
       # the wheel we just built.
       - name: Setup python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: Install abi3 wheel and run tests
         shell: bash
         run: |
+          set -e
           cd examples/
           pip install -U wheel
           python --version
           pip install rust_with_cffi/dist/rust_with_cffi*.whl
           python -c "from rust_with_cffi import rust; assert rust.rust_func() == 14"
           python -c "from rust_with_cffi.cffi import lib; assert lib.cffi_func() == 15"
 
+      - name: Run abi3audit
+        shell: bash
+        run: |
+          set -e
+          pip install abi3audit
+          cd examples/
+          abi3audit rust_with_cffi/dist/rust_with_cffi*.whl
+
   test-crossenv:
     runs-on: ubuntu-latest
     strategy:
       # If one platform fails, allow the rest to keep testing if `CI-no-fail-fast` label is present
       fail-fast: ${{ !contains(github.event.pull_request.labels.*.name, 'CI-no-fail-fast') }}
       matrix:
         platform: [
@@ -247,22 +249,18 @@
             python3 -c "from rust_with_cffi.cffi import lib; assert lib.cffi_func() == 15"
 
   test-cross:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Setup python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
-      - uses: actions-rs/toolchain@v1
-        with:
-          profile: minimal
-          toolchain: stable
-          override: true
+      - uses: dtolnay/rust-toolchain@stable
       - name: Install cross
         uses: taiki-e/install-action@v1
         with:
           tool: cross
       - name: Build package
         run: pip install -e .
       - name: Build wheel using cross
@@ -294,23 +292,20 @@
             python3 -c "from namespace_package import python; assert python.python_func() == 15"
 
   test-zigbuild:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Setup python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
-      - uses: actions-rs/toolchain@v1
+      - uses: dtolnay/rust-toolchain@stable
         with:
-          profile: minimal
-          toolchain: stable
-          target: aarch64-unknown-linux-gnu
-          override: true
+          targets: aarch64-unknown-linux-gnu
       - name: Install cargo-zigbuild
         run: |
           python3 -m pip install cargo-zigbuild
       - name: Build package
         run: pip install -e .
       - name: Build wheel using cargo-zigbuild
         shell: bash
@@ -341,20 +336,17 @@
             python3 -c "from namespace_package import rust; assert rust.rust_func() == 14"
             python3 -c "from namespace_package import python; assert python.python_func() == 15"
 
   test-cibuildwheel:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v3
-      - uses: actions-rs/toolchain@v1
+      - uses: dtolnay/rust-toolchain@stable
         with:
-          profile: minimal
-          toolchain: stable
-          target: aarch64-apple-darwin
-          override: true
+          targets: aarch64-apple-darwin
       - uses: pypa/cibuildwheel@v2.3.1
         env:
           CIBW_BUILD: cp39-*
           CIBW_BEFORE_BUILD: pip install -e .
           CIBW_ARCHS_MACOS: "x86_64 universal2 arm64"
           CIBW_BUILD_VERBOSITY: 1
         with:
@@ -380,19 +372,17 @@
           install: >-
             git
             mingw-w64-${{ matrix.arch }}-python
             mingw-w64-${{ matrix.arch }}-python-pip
             mingw-w64-${{ matrix.arch }}-openssl
             mingw-w64-${{ matrix.arch }}-toolchain
 
-      - uses: actions-rs/toolchain@v1
+      - uses: dtolnay/rust-toolchain@master
         with:
-          profile: minimal
           toolchain: stable-${{ matrix.rust_target }}
-          default: true
 
       - name: Install test dependencies
         shell: msys2 {0}
         run: python -m pip install --upgrade nox pip wheel
 
       - name: Create libpython symlink
         shell: msys2 {0}
@@ -415,39 +405,36 @@
           PYODIDE_VERSION=0.21.0
 
           cd emscripten
           npm i pyodide@0.21.0 prettier
           cd node_modules/pyodide/
           node ../prettier/bin-prettier.js -w pyodide.asm.js
           EMSCRIPTEN_VERSION=$(node -p "require('./repodata.json').info.platform.split('_').slice(1).join('.')")
-          PYTHON_VERSION=3.10.2
+          PYTHON_VERSION=3.10
 
           echo "PYODIDE_VERSION=$PYODIDE_VERSION" >> $GITHUB_ENV
           echo "EMSCRIPTEN_VERSION=$EMSCRIPTEN_VERSION" >> $GITHUB_ENV
           echo "PYTHON_VERSION=$PYTHON_VERSION" >> $GITHUB_ENV
           echo "ORIG_PATH=$PATH" >> $GITHUB_ENV
-      - uses: actions-rs/toolchain@v1
+      - uses: dtolnay/rust-toolchain@nightly
         with:
-          profile: minimal
-          toolchain: nightly
           components: rust-src
-          target: wasm32-unknown-emscripten
-          override: true
+          targets: wasm32-unknown-emscripten
       - uses: mymindstorm/setup-emsdk@v11
         with:
           version: ${{env.EMSCRIPTEN_VERSION}}
           actions-cache-folder: emsdk-cache
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         id: setup-python
         with:
           python-version: ${{env.PYTHON_VERSION}}
       - run: pip install nox
       - uses: actions/cache@v3
         with:
           path: |
             tests/pyodide
           key: ${{ hashFiles('tests/*.js') }} - ${{ hashFiles('noxfile.py') }} - ${{ steps.setup-python.outputs.python-path }}
-      - uses: Swatinem/rust-cache@v1
+      - uses: Swatinem/rust-cache@v2
       - name: Test
         run: |
           export PATH=$ORIG_PATH:$PATH
           nox -s test-examples-emscripten
```

### Comparing `setuptools-rust-1.5.2/.github/workflows/python-publish.yml` & `setuptools-rust-1.6.0/.github/workflows/python-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         # Fetch all history so that setuptools_scm works correctly
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       # Install build and packaging dependencies.
       # setuptools-scm is necessary for ensuring all files from VCS (such as
       # examples) are in the sdist.
       run: |
```

### Comparing `setuptools-rust-1.5.2/CHANGELOG.md` & `setuptools-rust-1.6.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## 1.6.0 (2023-04-27)
+### Changed
+- Prefer passing `--crate-type` option to cargo if "toolchain >= 1.64". [#322](https://github.com/PyO3/setuptools-rust/pull/322)
+
+### Fixed
+- Fix a bug where rebuilding the library would cause any running processes using it to segfault. [#295](https://github.com/PyO3/setuptools-rust/pull/295)
+- Fix `setup.cfg` format for compatibility with "poetry==1.4.0". [#319](https://github.com/PyO3/setuptools-rust/pull/319)
+
 ## 1.5.2 (2022-09-19)
 ### Fixed
 - Fix regression in `dylib` build artifacts not being found since 1.5.0. [#290](https://github.com/PyO3/setuptools-rust/pull/290)
 - Fix regression in sdist missing examples and other supplementary files since 1.5.0. [#291](https://github.com/PyO3/setuptools-rust/pull/291)
 
 ## 1.5.1 (2022-08-14)
 ### Fixed
```

### Comparing `setuptools-rust-1.5.2/LICENSE` & `setuptools-rust-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/PKG-INFO` & `setuptools-rust-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: setuptools-rust
-Version: 1.5.2
+Version: 1.6.0
 Summary: Setuptools Rust extension plugin
 Home-page: https://github.com/PyO3/setuptools-rust
 Author: Nikolay Kim
 Author-email: fafhrd91@gmail.com
 License: MIT
 Keywords: distutils,setuptools,rust
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `setuptools-rust-1.5.2/README.md` & `setuptools-rust-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/docs/Makefile` & `setuptools-rust-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/docs/building_wheels.md` & `setuptools-rust-1.6.0/docs/building_wheels.md`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/docs/conf.py` & `setuptools-rust-1.6.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 
 from sphinx.transforms import SphinxTransform
 
 DOCS_URL = "https://setuptools-rust.readthedocs.io/en/latest/"
 
 
 class RelativeDocLinks(SphinxTransform):
-
     default_priority = 750
 
     def apply(self):
         from docutils.nodes import Text, reference
 
         baseref = lambda o: (
             isinstance(o, reference) and o.get("refuri", "").startswith(DOCS_URL)
```

### Comparing `setuptools-rust-1.5.2/docs/make.bat` & `setuptools-rust-1.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/emscripten/_sysconfigdata__emscripten_wasm32-emscripten.py` & `setuptools-rust-1.6.0/emscripten/_sysconfigdata__emscripten_wasm32-emscripten.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/emscripten/emcc_wrapper.py` & `setuptools-rust-1.6.0/emscripten/emcc_wrapper.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/emscripten/runner.js` & `setuptools-rust-1.6.0/emscripten/runner.js`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/hello-world/noxfile.py` & `setuptools-rust-1.6.0/examples/hello-world/noxfile.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/hello-world-script/noxfile.py` & `setuptools-rust-1.6.0/examples/hello-world-script/noxfile.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/.github/workflows/upload.yml` & `setuptools-rust-1.6.0/examples/html-py-ever/.github/workflows/upload.yml`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/Cargo.lock` & `setuptools-rust-1.6.0/examples/html-py-ever/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -230,17 +230,17 @@
 name = "matches"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e378b66a060d48947b590737b30a1be76706c8dd7b8ba0f2fe3989c68a853f"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "new_debug_unreachable"
 version = "1.0.4"
@@ -372,66 +372,66 @@
 checksum = "c7342d5883fbccae1cc37a2353b09c87c9b0f3afd73f5fb9bba687a1f733b029"
 dependencies = [
  "unicode-xid",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12f72538a0230791398a0986a6518ebd88abc3fded89007b506ed072acc831e1"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc4cf18c20f4f09995f3554e6bcf9b09bd5e4d6b67c562fdfaafa644526ba479"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41877f28d8ebd600b6aa21a17b40c3b0fc4dfe73a27b6e81ab3d895e401b0e9"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e81c8d4bcc2f216dc1b665412df35e46d12ee8d3d046b381aad05f1fcf30547"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85752a767ee19399a78272cc2ab625cd7d373b2e112b4b13db28de71fa892784"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/README.md` & `setuptools-rust-1.6.0/examples/html-py-ever/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/build-wheels.sh` & `setuptools-rust-1.6.0/examples/html-py-ever/build-wheels.sh`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/noxfile.py` & `setuptools-rust-1.6.0/examples/html-py-ever/noxfile.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/setup.cfg` & `setuptools-rust-1.6.0/examples/html-py-ever/setup.cfg`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/src/lib.rs` & `setuptools-rust-1.6.0/examples/html-py-ever/src/lib.rs`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/src/main.rs` & `setuptools-rust-1.6.0/examples/html-py-ever/src/main.rs`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/tests/monty-python.html` & `setuptools-rust-1.6.0/examples/html-py-ever/tests/monty-python.html`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/tests/python.html` & `setuptools-rust-1.6.0/examples/html-py-ever/tests/python.html`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/tests/run_all.py` & `setuptools-rust-1.6.0/examples/html-py-ever/tests/run_all.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/tests/rust.html` & `setuptools-rust-1.6.0/examples/html-py-ever/tests/rust.html`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/tests/test_parsing.py` & `setuptools-rust-1.6.0/examples/html-py-ever/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/html-py-ever/tests/test_selector.py` & `setuptools-rust-1.6.0/examples/html-py-ever/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/namespace_package/Cargo.lock` & `setuptools-rust-1.6.0/examples/rust_with_cffi/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -51,29 +51,22 @@
 checksum = "88943dd7ef4a2e5a4bfa2753aaab3013e34ce2533d1996fb18ef591e315e2b3b"
 dependencies = [
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "namespace_package_rust"
-version = "0.1.0"
-dependencies = [
- "pyo3",
-]
-
-[[package]]
 name = "once_cell"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87f3e037eac156d1775da914196f0f37741a274155e34a0b7e427c35d2a2ecb9"
 
 [[package]]
 name = "parking_lot"
@@ -107,66 +100,66 @@
 checksum = "c7342d5883fbccae1cc37a2353b09c87c9b0f3afd73f5fb9bba687a1f733b029"
 dependencies = [
  "unicode-xid",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12f72538a0230791398a0986a6518ebd88abc3fded89007b506ed072acc831e1"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc4cf18c20f4f09995f3554e6bcf9b09bd5e4d6b67c562fdfaafa644526ba479"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41877f28d8ebd600b6aa21a17b40c3b0fc4dfe73a27b6e81ab3d895e401b0e9"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e81c8d4bcc2f216dc1b665412df35e46d12ee8d3d046b381aad05f1fcf30547"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85752a767ee19399a78272cc2ab625cd7d373b2e112b4b13db28de71fa892784"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -184,14 +177,21 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8380fe0152551244f0747b1bf41737e0f8a74f97a14ccefd1148187271634f3c"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "rust_with_cffi"
+version = "0.1.0"
+dependencies = [
+ "pyo3",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
```

### Comparing `setuptools-rust-1.5.2/examples/namespace_package/noxfile.py` & `setuptools-rust-1.6.0/examples/namespace_package/noxfile.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/rust_with_cffi/Cargo.lock` & `setuptools-rust-1.6.0/examples/namespace_package/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -51,22 +51,29 @@
 checksum = "88943dd7ef4a2e5a4bfa2753aaab3013e34ce2533d1996fb18ef591e315e2b3b"
 dependencies = [
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "namespace_package_rust"
+version = "0.1.0"
+dependencies = [
+ "pyo3",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87f3e037eac156d1775da914196f0f37741a274155e34a0b7e427c35d2a2ecb9"
 
 [[package]]
 name = "parking_lot"
@@ -100,66 +107,66 @@
 checksum = "c7342d5883fbccae1cc37a2353b09c87c9b0f3afd73f5fb9bba687a1f733b029"
 dependencies = [
  "unicode-xid",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12f72538a0230791398a0986a6518ebd88abc3fded89007b506ed072acc831e1"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc4cf18c20f4f09995f3554e6bcf9b09bd5e4d6b67c562fdfaafa644526ba479"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41877f28d8ebd600b6aa21a17b40c3b0fc4dfe73a27b6e81ab3d895e401b0e9"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e81c8d4bcc2f216dc1b665412df35e46d12ee8d3d046b381aad05f1fcf30547"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85752a767ee19399a78272cc2ab625cd7d373b2e112b4b13db28de71fa892784"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -177,21 +184,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8380fe0152551244f0747b1bf41737e0f8a74f97a14ccefd1148187271634f3c"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "rust_with_cffi"
-version = "0.1.0"
-dependencies = [
- "pyo3",
-]
-
-[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
```

### Comparing `setuptools-rust-1.5.2/examples/rust_with_cffi/noxfile.py` & `setuptools-rust-1.6.0/examples/rust_with_cffi/noxfile.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/examples/rust_with_cffi/setup.py` & `setuptools-rust-1.6.0/examples/rust_with_cffi/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/noxfile.py` & `setuptools-rust-1.6.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/setup.cfg` & `setuptools-rust-1.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 [metadata]
 name = setuptools-rust
-version = 1.5.2
+version = 1.6.0
 author = Nikolay Kim
 author_email = fafhrd91@gmail.com
 license = MIT
 description = Setuptools Rust extension plugin
 keywords = distutils, setuptools, rust
 url = https://github.com/PyO3/setuptools-rust
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Topic :: Software Development :: Version Control
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Development Status :: 5 - Production/Stable
 	Operating System :: POSIX
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 
 [options]
 packages = setuptools_rust
 zip_safe = True
-install_requires = setuptools>=62.4; semantic_version>=2.8.2,<3; typing_extensions>=3.7.4.3
+install_requires = 
+	setuptools>=62.4
+	semantic_version>=2.8.2,<3
+	typing_extensions>=3.7.4.3
 setup_requires = setuptools>=62.4
 python_requires = >=3.7
 
 [options.entry_points]
 distutils.commands = 
 	clean_rust=setuptools_rust:clean_rust
 	build_rust=setuptools_rust:build_rust
```

### Comparing `setuptools-rust-1.5.2/setuptools_rust/_utils.py` & `setuptools-rust-1.6.0/setuptools_rust/_utils.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/setuptools_rust/build.py` & `setuptools-rust-1.6.0/setuptools_rust/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,38 @@
     DistutilsPlatformError,
 )
 from distutils.sysconfig import get_config_var
 from pathlib import Path
 from typing import Dict, Iterable, List, NamedTuple, Optional, Set, Tuple, cast
 
 import pkg_resources
+from semantic_version import Version
 from setuptools.command.build import build as CommandBuild  # type: ignore[import]
 from setuptools.command.build_ext import build_ext as CommandBuildExt
 from setuptools.command.build_ext import get_abi3_suffix
 from typing_extensions import Literal
 
 from ._utils import format_called_process_error
 from .command import RustCommand
 from .extension import Binding, RustBin, RustExtension, Strip
-from .rustc_info import get_rust_host, get_rust_target_list, get_rustc_cfgs
+from .rustc_info import (
+    get_rust_host,
+    get_rust_target_list,
+    get_rust_version,
+    get_rustc_cfgs,
+)
+
+
+def _check_cargo_supports_crate_type_option() -> bool:
+    version = get_rust_version()
+
+    if version is None:
+        return False
+
+    return version.major > 1 or (version.major == 1 and version.minor >= 64)  # type: ignore
 
 
 class build_rust(RustCommand):
     """Command for building Rust crates via cargo."""
 
     description = "build Rust extensions (compile/link to build directory)"
 
@@ -89,16 +104,18 @@
         )
 
         if self.build_number is not None and not self.build_number[:1].isdigit():
             raise ValueError("Build tag (build-number) must start with a digit.")
 
     def get_data_dir(self) -> str:
         components = (
-            pkg_resources.safe_name(self.distribution.get_name()).replace("-", "_"),  # type: ignore[attr-defined]
-            pkg_resources.safe_version(self.distribution.get_version()).replace("-", "_"),  # type: ignore[attr-defined]
+            pkg_resources.safe_name(self.distribution.get_name()).replace("-", "_"),
+            pkg_resources.safe_version(self.distribution.get_version()).replace(
+                "-", "_"
+            ),
         )
         if self.build_number:
             components += (self.build_number,)
         return "-".join(components) + ".data"
 
     def run_for_extension(self, ext: RustExtension) -> None:
         assert self.plat_name is not None
@@ -126,27 +143,27 @@
         else:
             dylib_paths = self.build_extension(ext, self.target)
         self.install_extension(ext, dylib_paths)
 
     def build_extension(
         self, ext: RustExtension, forced_target_triple: Optional[str] = None
     ) -> List["_BuiltModule"]:
-
         target_triple = self._detect_rust_target(forced_target_triple)
         rustc_cfgs = get_rustc_cfgs(target_triple)
 
         env = _prepare_build_environment()
 
         if not os.path.exists(ext.path):
             raise DistutilsFileError(
                 f"can't find Rust extension project file: {ext.path}"
             )
 
         quiet = self.qbuild or ext.quiet
         debug = self._is_debug_build(ext)
+        use_cargo_crate_type = _check_cargo_supports_crate_type_option()
 
         cargo_args = self._cargo_args(
             ext=ext, target_triple=target_triple, release=not debug, quiet=quiet
         )
 
         rustflags = []
 
@@ -157,19 +174,26 @@
                 "--manifest-path",
                 ext.path,
                 "--message-format=json-render-diagnostics",
                 *cargo_args,
             ]
 
         else:
-            rustc_args = [
-                "--crate-type",
-                "cdylib",
-                *ext.rustc_flags,
-            ]
+            # If toolchain >= 1.64.0, use '--crate-type' option of cargo.
+            # See https://github.com/PyO3/setuptools-rust/issues/320
+            if use_cargo_crate_type:
+                rustc_args = [
+                    *ext.rustc_flags,
+                ]
+            else:
+                rustc_args = [
+                    "--crate-type",
+                    "cdylib",
+                    *ext.rustc_flags,
+                ]
 
             # OSX requires special linker arguments
             if rustc_cfgs.get("target_os") == "macos":
                 ext_basename = os.path.basename(self.get_dylib_ext_path(ext, ext.name))
                 rustc_args.extend(
                     [
                         "-C",
@@ -186,14 +210,17 @@
 
             elif (rustc_cfgs.get("target_arch"), rustc_cfgs.get("target_os")) == (
                 "wasm32",
                 "emscripten",
             ):
                 rustc_args.extend(["-C", f"link-args=-sSIDE_MODULE=2 -sWASM_BIGINT"])
 
+            if use_cargo_crate_type and "--crate-type" not in cargo_args:
+                cargo_args.extend(["--crate-type", "cdylib"])
+
             command = [
                 self.cargo,
                 "rustc",
                 "--lib",
                 "--message-format=json-render-diagnostics",
                 "--manifest-path",
                 ext.path,
@@ -341,15 +368,26 @@
                 else:
                     ext.install_script(module_name.split(".")[-1], ext_path)
             else:
                 ext_path = self.get_dylib_ext_path(ext, module_name)
                 os.makedirs(os.path.dirname(ext_path), exist_ok=True)
 
             log.info("Copying rust artifact from %s to %s", dylib_path, ext_path)
-            shutil.copyfile(dylib_path, ext_path)
+
+            # We want to atomically replace any existing library file. We can't
+            # just copy the new library directly on top of the old one as that
+            # causes the existing library to be modified (rather the replaced).
+            # This means that any process that currently uses the shared library
+            # will see it modified and likely segfault.
+            #
+            # We first copy the file to the same directory, as `os.rename`
+            # doesn't work across file system boundaries.
+            temp_ext_path = ext_path + "~"
+            shutil.copyfile(dylib_path, temp_ext_path)
+            os.replace(temp_ext_path, ext_path)
 
             if sys.platform != "win32" and not debug_build:
                 args = []
                 if ext.strip == Strip.All:
                     args.append("-x")
                 elif ext.strip == Strip.Debug:
                     args.append("-S")
```

### Comparing `setuptools-rust-1.5.2/setuptools_rust/clean.py` & `setuptools-rust-1.6.0/setuptools_rust/clean.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/setuptools_rust/command.py` & `setuptools-rust-1.6.0/setuptools_rust/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 
         if not isinstance(extensions, list):
             ty = type(extensions)
             raise ValueError(
                 "expected list of RustExtension objects for rust_extensions "
                 f"argument to setup(), got `{ty}`"
             )
-        for (i, extension) in enumerate(extensions):
-
+        for i, extension in enumerate(extensions):
             if not isinstance(extension, RustExtension):
                 ty = type(extension)
                 raise ValueError(
                     "expected RustExtension object for rust_extensions "
                     f"argument to setup(), got `{ty}` at position {i}"
                 )
         # Extensions have been verified to be at the correct type
```

### Comparing `setuptools-rust-1.5.2/setuptools_rust/extension.py` & `setuptools-rust-1.6.0/setuptools_rust/extension.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/setuptools_rust/rustc_info.py` & `setuptools-rust-1.6.0/setuptools_rust/rustc_info.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/setuptools_rust/setuptools_ext.py` & `setuptools-rust-1.6.0/setuptools_rust/setuptools_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,18 +271,16 @@
 def rust_extensions(
     dist: Distribution, attr: Literal["rust_extensions"], value: List[RustExtension]
 ) -> None:
     assert attr == "rust_extensions"
     has_rust_extensions = len(value) > 0
 
     # Monkey patch has_ext_modules to include Rust extensions.
-    #
-    # has_ext_modules is missing from Distribution typing.
-    orig_has_ext_modules = dist.has_ext_modules  # type: ignore[attr-defined]
-    dist.has_ext_modules = lambda: (orig_has_ext_modules() or has_rust_extensions)  # type: ignore[attr-defined]
+    orig_has_ext_modules = dist.has_ext_modules
+    dist.has_ext_modules = lambda: (orig_has_ext_modules() or has_rust_extensions)  # type: ignore[method-assign]
 
     if has_rust_extensions:
         add_rust_extension(dist)
 
 
 _CARGO_VENDOR_CONFIG = b"""
 [source.crates-io]
```

### Comparing `setuptools-rust-1.5.2/setuptools_rust.egg-info/PKG-INFO` & `setuptools-rust-1.6.0/setuptools_rust.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: setuptools-rust
-Version: 1.5.2
+Version: 1.6.0
 Summary: Setuptools Rust extension plugin
 Home-page: https://github.com/PyO3/setuptools-rust
 Author: Nikolay Kim
 Author-email: fafhrd91@gmail.com
 License: MIT
 Keywords: distutils,setuptools,rust
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `setuptools-rust-1.5.2/setuptools_rust.egg-info/SOURCES.txt` & `setuptools-rust-1.6.0/setuptools_rust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/tests/test_build.py` & `setuptools-rust-1.6.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `setuptools-rust-1.5.2/tests/test_extension.py` & `setuptools-rust-1.6.0/tests/test_extension.py`

 * *Files identical despite different names*

