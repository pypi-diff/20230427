# Comparing `tmp/promql_parser-0.1.1.tar.gz` & `tmp/promql_parser-0.1.2.tar.gz`

## Comparing `promql_parser-0.1.1.tar` & `promql_parser-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 promql_parser-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     1561 2023-02-14 03:31:24.000000 promql_parser-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-02-14 03:31:24.000000 promql_parser-0.1.1/.gitignore
--rw-r--r--   0     1001      123     1086 2023-02-14 03:31:24.000000 promql_parser-0.1.1/LICENSE
--rw-r--r--   0     1001      123      632 2023-02-14 03:31:24.000000 promql_parser-0.1.1/README.md
--rw-r--r--   0     1001      123      321 2023-02-14 03:31:24.000000 promql_parser-0.1.1/pyproject.toml
--rwxr-xr-x   0     1001      123      768 2023-02-14 03:31:52.000000 promql_parser-0.1.1/run-maturin-action.sh
--rw-r--r--   0     1001      123    17324 2023-02-14 03:31:24.000000 promql_parser-0.1.1/src/expr.rs
--rw-r--r--   0     1001      123     1765 2023-02-14 03:31:24.000000 promql_parser-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123      321 2023-02-14 03:31:24.000000 promql_parser-0.1.1/test_promql_parser.py
--rw-r--r--   0     1001      123    25865 2023-02-14 03:31:24.000000 promql_parser-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 promql_parser-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 promql_parser-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     1561 2023-04-27 11:35:35.000000 promql_parser-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-27 11:35:35.000000 promql_parser-0.1.2/.gitignore
+-rw-r--r--   0     1001      123     1086 2023-04-27 11:35:35.000000 promql_parser-0.1.2/LICENSE
+-rw-r--r--   0     1001      123      632 2023-04-27 11:35:35.000000 promql_parser-0.1.2/README.md
+-rw-r--r--   0     1001      123      321 2023-04-27 11:35:35.000000 promql_parser-0.1.2/pyproject.toml
+-rwxr-xr-x   0     1001      123      833 2023-04-27 11:36:06.000000 promql_parser-0.1.2/run-maturin-action.sh
+-rw-r--r--   0     1001      123    17378 2023-04-27 11:35:35.000000 promql_parser-0.1.2/src/expr.rs
+-rw-r--r--   0     1001      123     1755 2023-04-27 11:35:35.000000 promql_parser-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123      321 2023-04-27 11:35:35.000000 promql_parser-0.1.2/test_promql_parser.py
+-rw-r--r--   0     1001      123    19588 2023-04-27 11:35:35.000000 promql_parser-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 promql_parser-0.1.2/PKG-INFO
```

### Comparing `promql_parser-0.1.1/Cargo.toml` & `promql_parser-0.1.2/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-promql-parser"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 description = "PromQL Parser for Python"
 license = "MIT"
 repository = "https://github.com/messense/py-promql-parser"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `promql_parser-0.1.1/.github/workflows/CI.yml` & `promql_parser-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.1/.gitignore` & `promql_parser-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.1/LICENSE` & `promql_parser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.1/README.md` & `promql_parser-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.1/run-maturin-action.sh` & `promql_parser-0.1.2/run-maturin-action.sh`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 set -e
 echo "::group::Install Rust"
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain stable
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set stable
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
-export PATH="$PATH:/opt/python/cp36-cp36m/bin:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin"
+export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/download/v0.14.13/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v0.14.17/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
+python3 -m pip install cffi || true
 echo "::endgroup::"
 maturin build --release --sdist -o dist --find-interpreter
```

### Comparing `promql_parser-0.1.1/src/expr.rs` & `promql_parser-0.1.2/src/expr.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 use std::collections::HashSet;
 
 use chrono::Duration;
 use promql_parser::label::Labels;
 use promql_parser::parser::{
-    self, AggModifier, AggregateExpr, AtModifier, BinaryExpr, Call, Expr, MatrixSelector,
+    self, AggregateExpr, AtModifier, BinaryExpr, Call, Expr, LabelModifier, MatrixSelector,
     NumberLiteral, Offset, ParenExpr, StringLiteral, SubqueryExpr, TokenType, UnaryExpr, ValueType,
-    VectorMatchCardinality, VectorMatchModifier, VectorSelector,
+    VectorMatchCardinality, VectorSelector,
 };
-use pyo3::exceptions::{PyOverflowError, PyValueError};
+use pyo3::exceptions::{PyNotImplementedError, PyOverflowError, PyValueError};
 use pyo3::prelude::*;
 
 #[pyclass(subclass, name = "Expr", module = "promql_parser")]
 #[derive(Debug, Clone)]
 pub struct PyExpr {
     pub expr: Expr,
 }
@@ -25,14 +25,15 @@
             Expr::Paren(expr) => PyParenExpr::create(py, expr),
             Expr::Subquery(subquery) => PySubqueryExpr::create(py, subquery),
             Expr::NumberLiteral(lit) => PyNumberLiteral::create(py, lit),
             Expr::StringLiteral(lit) => PyStringLiteral::create(py, lit),
             Expr::VectorSelector(selector) => PyVectorSelector::create(py, selector),
             Expr::MatrixSelector(selector) => PyMatrixSelector::create(py, selector),
             Expr::Call(call) => PyCall::create(py, call),
+            Expr::Extension(_ext) => Err(PyNotImplementedError::new_err("extension unimplemented")),
         }
     }
 }
 
 #[pymethods]
 impl PyExpr {
     #[staticmethod]
@@ -74,19 +75,19 @@
             op: op.into(),
             expr: PyExpr::create(py, *expr)?,
             param: match param {
                 Some(param) => Some(PyExpr::create(py, *param)?),
                 None => None,
             },
             modifier: match modifier {
-                Some(AggModifier::By(labels)) => Some(PyAggModifier {
+                Some(LabelModifier::Include(labels)) => Some(PyAggModifier {
                     r#type: PyAggModifierType::By,
                     labels,
                 }),
-                Some(AggModifier::Without(labels)) => Some(PyAggModifier {
+                Some(LabelModifier::Exclude(labels)) => Some(PyAggModifier {
                     r#type: PyAggModifierType::Without,
                     labels,
                 }),
                 None => None,
             },
         });
         Ok(Py::new(py, initializer)?.into_py(py))
@@ -163,20 +164,20 @@
             rhs,
             modifier,
         } = expr;
         let py_modifier = match modifier {
             Some(modifier) => Some(PyBinModifier {
                 card: modifier.card.into(),
                 matching: match modifier.matching {
-                    Some(VectorMatchModifier::On(labels)) => Some(PyVectorMatchModifier {
-                        r#type: PyVectorMatchModifierType::On,
+                    Some(LabelModifier::Include(labels)) => Some(PyLabelModifier {
+                        r#type: PyLabelModifierType::Include,
                         labels,
                     }),
-                    Some(VectorMatchModifier::Ignoring(labels)) => Some(PyVectorMatchModifier {
-                        r#type: PyVectorMatchModifierType::Ignoring,
+                    Some(LabelModifier::Exclude(labels)) => Some(PyLabelModifier {
+                        r#type: PyLabelModifierType::Exclude,
                         labels,
                     }),
                     None => None,
                 },
                 return_bool: modifier.return_bool,
             }),
             None => None,
@@ -193,33 +194,33 @@
 
 #[pyclass(name = "BinModifier", module = "promql_parser")]
 #[derive(Debug, Clone)]
 pub struct PyBinModifier {
     #[pyo3(get)]
     card: PyVectorMatchCardinality,
     #[pyo3(get)]
-    matching: Option<PyVectorMatchModifier>,
+    matching: Option<PyLabelModifier>,
     #[pyo3(get)]
     return_bool: bool,
 }
 
-#[pyclass(name = "VectorMatchModifier", module = "promql_parser")]
+#[pyclass(name = "LabelModifier", module = "promql_parser")]
 #[derive(Debug, Clone)]
-pub struct PyVectorMatchModifier {
+pub struct PyLabelModifier {
     #[pyo3(get)]
-    r#type: PyVectorMatchModifierType,
+    r#type: PyLabelModifierType,
     #[pyo3(get)]
     labels: Labels,
 }
 
-#[pyclass(name = "VectorMatchModifierType", module = "promql_parser")]
+#[pyclass(name = "LabelModifierType", module = "promql_parser")]
 #[derive(Debug, Clone, Copy)]
-pub enum PyVectorMatchModifierType {
-    On,
-    Ignoring,
+pub enum PyLabelModifierType {
+    Include,
+    Exclude,
 }
 
 #[pyclass(name = "VectorMatchCardinality", module = "promql_parser")]
 #[derive(Debug, Clone, Copy)]
 pub enum PyVectorMatchCardinality {
     OneToOne,
     ManyToOne,
```

### Comparing `promql_parser-0.1.1/src/lib.rs` & `promql_parser-0.1.2/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use ::promql_parser::parser;
+use ::promql_parser::parser::ast;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 
 mod expr;
 
 use self::expr::PyExpr;
 
@@ -10,15 +10,15 @@
 #[pyfunction]
 fn parse(py: Python, input: &str) -> PyResult<PyObject> {
     PyExpr::parse(py, input)
 }
 
 #[pyfunction]
 fn check_ast(py: Python, ast: PyExpr) -> PyResult<PyObject> {
-    let expr = parser::check_ast(ast.expr).map_err(PyValueError::new_err)?;
+    let expr = ast::check_ast(ast.expr).map_err(PyValueError::new_err)?;
     let py_expr = PyExpr::create(py, expr)?;
     Ok(py_expr)
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn promql_parser(_py: Python, m: &PyModule) -> PyResult<()> {
@@ -26,16 +26,16 @@
     m.add_class::<expr::PyAggregateExpr>()?;
     m.add_class::<expr::PyTokenType>()?;
     m.add_class::<expr::PyAggModifier>()?;
     m.add_class::<expr::PyAggModifierType>()?;
     m.add_class::<expr::PyUnaryExpr>()?;
     m.add_class::<expr::PyBinaryExpr>()?;
     m.add_class::<expr::PyBinModifier>()?;
-    m.add_class::<expr::PyVectorMatchModifier>()?;
-    m.add_class::<expr::PyVectorMatchModifierType>()?;
+    m.add_class::<expr::PyLabelModifier>()?;
+    m.add_class::<expr::PyLabelModifierType>()?;
     m.add_class::<expr::PyVectorMatchCardinality>()?;
     m.add_class::<expr::PyParenExpr>()?;
     m.add_class::<expr::PySubqueryExpr>()?;
     m.add_class::<expr::PyAtModifier>()?;
     m.add_class::<expr::PyAtModifierType>()?;
     m.add_class::<expr::PyNumberLiteral>()?;
     m.add_class::<expr::PyStringLiteral>()?;
```

### Comparing `promql_parser-0.1.1/Cargo.lock` & `promql_parser-0.1.2/Cargo.lock`

 * *Files 18% similar despite different names*

```diff
@@ -8,27 +8,18 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "android_system_properties"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
@@ -44,32 +35,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "bumpalo"
-version = "3.12.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
-
-[[package]]
 name = "cactus"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf034765b7d19a011c6d619e880582bf95e8186b580e6fab56589872dd87dcf5"
 
 [[package]]
-name = "cc"
-version = "1.0.79"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
-
-[[package]]
 name = "cfg-if"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4785bdd1c96b2a846b2bd7cc02e86b6b3dbf14e7e53446c4f54c92a361040822"
 
 [[package]]
 name = "cfg-if"
@@ -89,105 +68,40 @@
  "regex",
  "serde",
  "vob",
 ]
 
 [[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
- "iana-time-zone",
- "js-sys",
  "num-integer",
  "num-traits",
- "time 0.1.45",
- "wasm-bindgen",
- "winapi",
-]
-
-[[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
-name = "core-foundation-sys"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
-
-[[package]]
-name = "cxx"
-version = "1.0.90"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90d59d9acd2a682b4e40605a242f6670eaa58c5957471cbf85e8aa6a0b97a5e8"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.90"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebfa40bda659dd5c864e65f4c9a2b0aff19bea56b017b9b77c73d3766a453a38"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.90"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "457ce6757c5c70dc6ecdbda6925b958aae7f959bda7d8fb9bde889e34a09dc03"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.90"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebf883b7aacd7b2aeb2a7b338648ee19f57c140d4ee8e52c68979c6b2f7f2263"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
 ]
 
 [[package]]
 name = "enum-iterator"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ea166b3f7dc1032f7866d13f8d8e02c8d87507b61750176b86554964dc6a7bf"
+checksum = "706d9e7cf1c7664859d79cd524e4e53ea2b67ea03c98cc2870c5e539695d597e"
 dependencies = [
  "enum-iterator-derive",
 ]
 
 [[package]]
 name = "enum-iterator-derive"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "828de45d0ca18782232dfb8f3ea9cc428e8ced380eb26a520baaacfc70de39ce"
+checksum = "355f93763ef7b0ae1c43c4d8eccc9d5848d84ad1a1d8ce61c421d1ac85a19d05"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "filetime"
 version = "0.2.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
@@ -218,119 +132,68 @@
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e45727250e75cc04ff2846a66397da8ef2b3db8e40e0cef4df67950a07621eb9"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
-name = "iana-time-zone"
-version = "0.1.53"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
-dependencies = [
- "android_system_properties",
- "core-foundation-sys",
- "iana-time-zone-haiku",
- "js-sys",
- "wasm-bindgen",
- "winapi",
-]
-
-[[package]]
-name = "iana-time-zone-haiku"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
-dependencies = [
- "cxx",
- "cxx-build",
-]
-
-[[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
-
-[[package]]
-name = "js-sys"
-version = "0.3.61"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
-dependencies = [
- "wasm-bindgen",
-]
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.140"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
-name = "log"
-version = "0.4.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if 1.0.0",
-]
-
-[[package]]
 name = "lrlex"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22b832738fbfa58ad036580929e973b3b6bd31c6d6c7f18f6b5ea7b626675c85"
 dependencies = [
  "getopts",
  "lazy_static",
@@ -411,17 +274,17 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "packedvec"
 version = "1.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bde3c690ec20e4a2b4fb46f0289a451181eb50011a1e2acc8d85e2fde9062a45"
 dependencies = [
@@ -450,32 +313,32 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "pest"
-version = "2.5.5"
+version = "2.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "028accff104c4e513bad663bbcd2ad7cfd5304144404c31ed0a77ac103d00660"
+checksum = "8cbd939b234e95d72bc393d51788aec68aeeb5d51e748ca08ff3aad58cb722f7"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -484,48 +347,48 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.53"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "ba466839c78239c09faf015484e5cc04860f88242cff4d03eb038f04b4699b73"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "promql-parser"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24766dbb98852e704a98fc2c003d2b3ffa48317ab09b4ae184925f0e60385764"
+checksum = "b86b6a58ddafa87824aecefd60ab8bf33638f4dc687c560a3c06a31122948274"
 dependencies = [
  "cfgrammar",
  "lazy_static",
  "lrlex",
  "lrpar",
  "regex",
 ]
 
 [[package]]
 name = "py-promql-parser"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "chrono",
  "promql-parser",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if 1.0.0",
  "chrono",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
@@ -533,60 +396,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -594,57 +457,51 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "rustc_version"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0dfe2087c51c460008730de8b57e6a320782fbfb312e1f4d520e6c6fae155ee"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5583e89e108996506031660fe09baa5011b9dd0341b89029313006d1fb508d70"
+checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddccb15bcce173023b3fedd9436f882a0739b8dfb45e4f6b6002bee5929f61b2"
-
-[[package]]
 name = "semver"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f301af10236f6df4160f7c3f04eec6dbc70ace82d23326abad5edee88801c6b6"
 dependencies = [
  "semver-parser",
 ]
@@ -656,30 +513,30 @@
 checksum = "00b0bef5b7f9e0df16536d3961cfb6e84331c065b4066afb39768d0e319411f7"
 dependencies = [
  "pest",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.158"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.158"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.9",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
@@ -700,74 +557,65 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.6"
+name = "syn"
+version = "2.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "0da4a3c17e109f700685ec577c0f85efd9b19bcf15c913985f14dc1ac01775aa"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
+name = "target-lexicon"
+version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
-dependencies = [
- "winapi-util",
-]
+checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
-]
-
-[[package]]
-name = "time"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
-dependencies = [
- "libc",
- "wasi",
- "winapi",
+ "syn 2.0.9",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.17"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a561bf4617eebd33bca6434b988f39ed798e527f51a1e797d0ee4f61c0a38376"
+checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
@@ -775,17 +623,17 @@
 name = "time-core"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
 
 [[package]]
 name = "time-macros"
-version = "0.2.6"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d967f99f534ca7e495c575c62638eebc2898a8c84c119b89e250477bc4ba16b2"
+checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "try_from"
 version = "0.3.2"
@@ -799,17 +647,17 @@
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
@@ -827,15 +675,15 @@
 dependencies = [
  "anyhow",
  "cfg-if 1.0.0",
  "enum-iterator",
  "getset",
  "rustversion",
  "thiserror",
- "time 0.3.17",
+ "time",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
@@ -848,162 +696,71 @@
 dependencies = [
  "num-traits",
  "rustc_version",
  "serde",
 ]
 
 [[package]]
-name = "wasi"
-version = "0.10.0+wasi-snapshot-preview1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
-
-[[package]]
-name = "wasm-bindgen"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
-dependencies = [
- "cfg-if 1.0.0",
- "wasm-bindgen-macro",
-]
-
-[[package]]
-name = "wasm-bindgen-backend"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
-dependencies = [
- "bumpalo",
- "log",
- "once_cell",
- "proc-macro2",
- "quote",
- "syn",
- "wasm-bindgen-shared",
-]
-
-[[package]]
-name = "wasm-bindgen-macro"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
-dependencies = [
- "quote",
- "wasm-bindgen-macro-support",
-]
-
-[[package]]
-name = "wasm-bindgen-macro-support"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
- "wasm-bindgen-backend",
- "wasm-bindgen-shared",
-]
-
-[[package]]
-name = "wasm-bindgen-shared"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
-
-[[package]]
-name = "winapi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
-
-[[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
-name = "winapi-util"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
-dependencies = [
- "winapi",
-]
-
-[[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
```

### Comparing `promql_parser-0.1.1/PKG-INFO` & `promql_parser-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promql-parser
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: PromQL Parser for Python
 License: MIT
 Requires-Python: >=3.7
```

