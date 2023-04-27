# Comparing `tmp/rormula-0.1.3.tar.gz` & `tmp/rormula-0.1.4.tar.gz`

## Comparing `rormula-0.1.3.tar` & `rormula-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 rormula-0.1.3/local_dependencies/rormula-rs/Cargo.toml
--rw-r--r--   0     1001      123        6 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/.gitignore
--rw-r--r--   0     1001      123     4474 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/array.rs
--rw-r--r--   0     1001      123    11681 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs
--rw-r--r--   0     1001      123    10877 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs
--rw-r--r--   0     1001      123      211 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/expression/mod.rs
--rw-r--r--   0     1001      123     3092 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/expression/ops_common.rs
--rw-r--r--   0     1001      123     1577 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/expression/value.rs
--rw-r--r--   0     1001      123       66 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/lib.rs
--rw-r--r--   0     1001      123     1232 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/src/result.rs
--rw-r--r--   0     1001      123     2090 2023-04-27 09:46:12.000000 rormula-0.1.3/local_dependencies/rormula-rs/tests/test_rormula.rs
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 rormula-0.1.3/Cargo.toml
--rw-r--r--   0     1001      123        6 2023-04-27 09:46:12.000000 rormula-0.1.3/.gitignore
--rw-r--r--   0     1001      123      696 2023-04-27 09:46:12.000000 rormula-0.1.3/README-pypi.md
--rw-r--r--   0     1001      123     3523 2023-04-27 09:46:12.000000 rormula-0.1.3/benches/benchmark.rs
--rw-r--r--   0     1001      123      765 2023-04-27 09:46:12.000000 rormula-0.1.3/pyproject.toml
--rw-r--r--   0     1001      123       45 2023-04-27 09:46:12.000000 rormula-0.1.3/requirements-dev.txt
--rw-r--r--   0     1001      123     2749 2023-04-27 09:46:12.000000 rormula-0.1.3/rormula/__init__.py
--rw-r--r--   0     1001      123      764 2023-04-27 09:46:12.000000 rormula-0.1.3/rormula/_rormula.pyi
--rw-r--r--   0     1001      123     8276 2023-04-27 09:46:12.000000 rormula-0.1.3/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-04-27 09:46:12.000000 rormula-0.1.3/test/__init__.py
--rw-r--r--   0     1001      123     1575 2023-04-27 09:46:12.000000 rormula-0.1.3/test/test_arithmetic.py
--rw-r--r--   0     1001      123     1178 2023-04-27 09:46:12.000000 rormula-0.1.3/test/test_meta.py
--rw-r--r--   0     1001      123     5561 2023-04-27 09:46:12.000000 rormula-0.1.3/test/test_wilkinson.py
--rw-r--r--   0     1001      123    25081 2023-04-27 09:46:12.000000 rormula-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 rormula-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 rormula-0.1.4/local_dependencies/rormula-rs/Cargo.toml
+-rw-r--r--   0     1001      123        6 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/.gitignore
+-rw-r--r--   0     1001      123     4474 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/array.rs
+-rw-r--r--   0     1001      123    12246 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs
+-rw-r--r--   0     1001      123    10877 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs
+-rw-r--r--   0     1001      123      211 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/expression/mod.rs
+-rw-r--r--   0     1001      123     3096 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/expression/ops_common.rs
+-rw-r--r--   0     1001      123     1577 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/expression/value.rs
+-rw-r--r--   0     1001      123       66 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/lib.rs
+-rw-r--r--   0     1001      123     1232 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/src/result.rs
+-rw-r--r--   0     1001      123     3120 2023-04-27 18:42:08.000000 rormula-0.1.4/local_dependencies/rormula-rs/tests/test_rormula.rs
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 rormula-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123        6 2023-04-27 18:42:08.000000 rormula-0.1.4/.gitignore
+-rw-r--r--   0     1001      123      548 2023-04-27 18:42:08.000000 rormula-0.1.4/README-pypi.md
+-rw-r--r--   0     1001      123     3523 2023-04-27 18:42:08.000000 rormula-0.1.4/benches/benchmark.rs
+-rw-r--r--   0     1001      123      765 2023-04-27 18:42:08.000000 rormula-0.1.4/pyproject.toml
+-rw-r--r--   0     1001      123       45 2023-04-27 18:42:08.000000 rormula-0.1.4/requirements-dev.txt
+-rw-r--r--   0     1001      123     2749 2023-04-27 18:42:08.000000 rormula-0.1.4/rormula/__init__.py
+-rw-r--r--   0     1001      123      764 2023-04-27 18:42:08.000000 rormula-0.1.4/rormula/_rormula.pyi
+-rw-r--r--   0     1001      123     8276 2023-04-27 18:42:08.000000 rormula-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-04-27 18:42:08.000000 rormula-0.1.4/test/__init__.py
+-rw-r--r--   0     1001      123     1881 2023-04-27 18:42:08.000000 rormula-0.1.4/test/test_arithmetic.py
+-rw-r--r--   0     1001      123     1178 2023-04-27 18:42:08.000000 rormula-0.1.4/test/test_meta.py
+-rw-r--r--   0     1001      123     5561 2023-04-27 18:42:08.000000 rormula-0.1.4/test/test_wilkinson.py
+-rw-r--r--   0     1001      123    25081 2023-04-27 18:42:08.000000 rormula-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 rormula-0.1.4/PKG-INFO
```

### Comparing `rormula-0.1.3/local_dependencies/rormula-rs/src/array.rs` & `rormula-0.1.4/local_dependencies/rormula-rs/src/array.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs` & `rormula-0.1.4/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 fn apply_op(mut a: Value, mut b: Value, op: &impl Fn(f64, f64) -> f64) -> Value {
     // We take mutable references because otherwise in second (scalar) arm they would already have
     // been moved and not available anymore
     let res = match (&mut a, &mut b) {
         (Value::Array(a), Value::Array(b)) => {
             ops_common::op_componentwise_array(mem::take(a), mem::take(b), op).map(Value::Array)
         }
+        (_, Value::Error(e)) => Ok(Value::Error(mem::take(e))),
+        (Value::Error(e), _) => Ok(Value::Error(mem::take(e))),
         _ => Ok(ops_common::op_scalar(a, b, op)),
     };
     match res {
         Ok(res) => res,
         Err(e) => Value::Error(e.to_string()),
     }
 }
@@ -122,15 +124,15 @@
                 Value::RowInds(compare_slices(&c1, &c2, $comp_exact))
             }
             (Value::RowInds(ri1), Value::RowInds(ri2)) => {
                 Value::RowInds(compare_slices(&ri1, &ri2, $comp_exact))
             }
             (Value::Error(e), _) => Value::Error(e),
             (_, Value::Error(e)) => Value::Error(e),
-            _ => Value::RowInds(vec![]),
+            _ => Value::Error("cannot compare values".to_string()),
         }
     };
 }
 
 pub fn op_compare_ge(a: Value, b: Value) -> Value {
     op_compare!(a, b, |v1, v2| v1 >= v2, floats_ge)
 }
@@ -146,22 +148,31 @@
 pub fn op_compare_equals(a: Value, b: Value) -> Value {
     op_compare!(a, b, |v1, v2| v1 == v2, floats_almost_equals)
 }
 
 pub fn op_restrict(a: Value, b: Value) -> Value {
     match (a, b) {
         (Value::Array(a), Value::RowInds(ris)) => {
-            let data = ris.iter().map(|i| a.data[*i]).collect::<Vec<f64>>();
-            let n_rows = data.len();
-            Value::Array(Array2d {
-                data,
-                n_rows,
-                n_cols: 1,
-                ..a
-            })
+            let max = ris.iter().max();
+            if let Some(max) = max {
+                if *max >= a.n_rows {
+                    Value::Error(format!("row index out of bounds: {} >= {}", max, a.n_rows))
+                } else {
+                    let data = ris.iter().map(|ri| a.data[*ri]).collect::<Vec<f64>>();
+                    let n_rows = data.len();
+                    Value::Array(Array2d {
+                        data,
+                        n_rows,
+                        n_cols: 1,
+                        ..a
+                    })
+                }
+            } else {
+                Value::Array(Array2d::ones(0, a.n_cols))
+            }
         }
         (Value::Cats(mut c), Value::RowInds(ris)) => {
             Value::Cats(ris.iter().map(|i| mem::take(&mut c[*i])).collect())
         }
         (Value::RowInds(a), Value::RowInds(ris)) => {
             Value::RowInds(ris.iter().map(|i| a[*i]).collect())
         }
```

### Comparing `rormula-0.1.3/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs` & `rormula-0.1.4/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/local_dependencies/rormula-rs/src/expression/ops_common.rs` & `rormula-0.1.4/local_dependencies/rormula-rs/src/expression/ops_common.rs`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,14 @@
             *elt = op(sc, *elt);
         }
         Value::Array(mem::take(arr))
     };
     match (a, b) {
         (Value::Array(mut arr), Value::Scalar(sc)) => arr_vs_sc(&mut arr, sc),
         (Value::Scalar(sc), Value::Array(mut arr)) => sc_vs_arr(sc, &mut arr),
-        _ => Value::Error("power can only be applied to matrix and skalar".to_string()),
+        _ => Value::Error("scalar op can only be applied to matrix and scalar".to_string()),
     }
 }
 
 pub fn op_power(a: Value, b: Value) -> Value {
     op_scalar(a, b, &|x, y| x.powf(y))
 }
```

### Comparing `rormula-0.1.3/local_dependencies/rormula-rs/src/expression/value.rs` & `rormula-0.1.4/local_dependencies/rormula-rs/src/expression/value.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/local_dependencies/rormula-rs/src/result.rs` & `rormula-0.1.4/local_dependencies/rormula-rs/src/result.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/local_dependencies/rormula-rs/tests/test_rormula.rs` & `rormula-0.1.4/local_dependencies/rormula-rs/tests/test_rormula.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use rormula_rs::{
     array::Array2d,
     expression::{ExprArithmetic, Value},
     expression::{ExprNames, ExprWilkinson, NameValue},
 };
 
 #[test]
-fn test_rormula() {
+fn test_wilkinson() {
     let n1 = NameValue::Array(vec!["n".to_string()]);
     let v1 = Value::Array(Array2d::from_iter([0.1, 0.2, 0.3].iter(), 3, 1).unwrap());
     let n2 = NameValue::Array(vec!["o".to_string()]);
     let v2 = Value::Array(Array2d::from_iter([0.4, 0.5, 0.6].iter(), 3, 1).unwrap());
     let s = "n+o+n";
     let expr = ExprWilkinson::parse(s).unwrap();
     match expr.eval_vec(vec![v1, v2]).unwrap() {
@@ -56,7 +56,40 @@
         .collect::<Vec<_>>();
     let res = expr.eval_vec(vars).unwrap();
     let s_ref = "x * -2.0";
     let expr_ref = ExprArithmetic::parse(s_ref).unwrap();
     let rev_val = expr_ref.eval(&[Value::Array(Array2d::ones(5, 1))]).unwrap();
     assert_eq!(res, rev_val);
 }
+#[test]
+fn test_restrict() {
+    let cols = ["first_var", "second.var"];
+    // - has higher precedence than ==
+
+    let s = "(first_var|{second.var}==1.0) - (first_var|{second.var}==1.0)";
+
+    let mut vars = (0..cols.len())
+        .map(|_| Value::Array(Array2d::ones(5, 1)))
+        .collect::<Vec<_>>();
+    vars[0] = Value::Array(Array2d::zeros(5, 1));
+    let exp = ExprArithmetic::parse(s).unwrap();
+    println!("{:?}", exp.var_indices_ordered());
+    let res = exp.eval_vec(vars).unwrap();
+    println!("{:?}", res);
+    if let Value::Array(a) = res {
+        assert_eq!(a.data, vec![0.0; 5]);
+    } else {
+        assert!(false);
+    }
+    let s = "first_var|{second.var}==1.0 - first_var|{second.var}==1.0";
+
+    let vars = (0..cols.len())
+        .map(|_| Value::Array(Array2d::ones(5, 1)))
+        .collect::<Vec<_>>();
+    let exp = ExprArithmetic::parse(s).unwrap();
+    let res = exp.eval_vec(vars).unwrap();
+    if let Value::Error(_) = res {
+        assert!(true);
+    } else {
+        assert!(false);
+    }
+}
```

### Comparing `rormula-0.1.3/benches/benchmark.rs` & `rormula-0.1.4/benches/benchmark.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/pyproject.toml` & `rormula-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "rormula"
 requires-python = ">=3.7"
-version = "0.1.3"
+version = "0.1.4"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = ["pandas"]
 license = {text = "BSD-3-Clause"}
 description = "Formula parser and evaluator for Wilkinson notation"
```

### Comparing `rormula-0.1.3/rormula/__init__.py` & `rormula-0.1.4/rormula/__init__.py`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/rormula/_rormula.pyi` & `rormula-0.1.4/rormula/_rormula.pyi`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/src/lib.rs` & `rormula-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/test/test_arithmetic.py` & `rormula-0.1.4/test/test_arithmetic.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,21 +40,27 @@
     data[7, :] = 2.5
     df = pd.DataFrame(data=data, columns=["alpha", "beta", "gamma"])
     s = "beta|alpha==2.5"
     rormula = Arithmetic(s, "reduced")
     res = rormula.eval_asdf(df)
     assert res.shape == (2, 1)
     assert np.allclose(res, 2.5)
-    print(res)
     s = "beta|alpha>=2.5"
     rormula = Arithmetic(s, s)
     res = rormula.eval_asdf(df)
     assert res.shape == (2, 1)
     assert np.allclose(res, 2.5)
     s = "beta|alpha<2.5"
     rormula = Arithmetic(s, s)
     res = rormula.eval_asdf(df)
     assert res.shape == (98, 1)
+    
+    s = "((first_var|{second.var}==5.0) - (first_var|{second.var}==2.5)) / 4.0"
+    data[7, :] = 5.0
+    df = pd.DataFrame(data=data[:10, :2], columns=["first_var", "second.var"])
+    rormula = Arithmetic(s, "reduced")
+    res = rormula.eval_asdf(df)
+    assert np.allclose(res.to_numpy().item(), (5.0 - 2.5) / 4.0)
 
 
 if __name__ == "__main__":
     test_arithmetic()
```

### Comparing `rormula-0.1.3/test/test_meta.py` & `rormula-0.1.4/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/test/test_wilkinson.py` & `rormula-0.1.4/test/test_wilkinson.py`

 * *Files identical despite different names*

### Comparing `rormula-0.1.3/Cargo.lock` & `rormula-0.1.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -195,17 +195,17 @@
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "exmex"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22ad4c3ff389c7cd2478a1ae0b45275cfea2d69028e949b01d54edc60f8e5c79"
+checksum = "04cf492b44826a2d801408d6c0ee8f847dcaff09271023c81695b1328cc626c8"
 dependencies = [
  "lazy_static",
  "num",
  "regex",
  "smallvec",
 ]
 
@@ -657,15 +657,15 @@
 name = "regex-syntax"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rormula"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "criterion",
  "numpy",
  "pyo3",
  "rormula-rs",
  "which",
 ]
```

### Comparing `rormula-0.1.3/PKG-INFO` & `rormula-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: rormula
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: pandas
 Summary: Formula parser and evaluator for Wilkinson notation
 Keywords: design of experiments,Wilkinson,parser,eval,doe
 Author-email: Behrang Shafei <behrang.shafei@basf.com>
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://github.com/basf/rormula
 Project-URL: repository, https://github.com/basf/rormula
+Project-URL: homepage, https://github.com/basf/rormula
 
 # Rormula
 
-[![CI](https://github.com/basf/rormula/actions/workflows/ci.yml/badge.svg)](https://github.com/basf/rormula/actions)
-[![PyPI](https://img.shields.io/pypi/v/rormula.svg?color=%2334D058)](https://pypi.org/project/rormula)
-
 Rormula is a Python package that parses the Wilkinson notation to create model matrices useful in design of experiments. 
 Additionally, it can be used for column arithmetics similar to
-`df.eval` where `df` is a Pandas dataframe. Rormula is significantly faster for small matrices than `df.eval` or [Formulaic](https://github.com/matthewwardrop/formulaic)
+`df.eval` where `df` is a Pandas dataframe. Rormula is significantly faster for small matrices than `df.eval` or [Formulaic](https://github.com/matthewwardrop/formulaic), does not allow arbitrary code execution but only pre-defined operators,
 and still a not well tested prototype.
 
 More information can be found under https://github.com/basf/rormula.
```

