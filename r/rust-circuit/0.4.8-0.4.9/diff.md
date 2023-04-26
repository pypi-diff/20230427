# Comparing `tmp/rust_circuit-0.4.8.tar.gz` & `tmp/rust_circuit-0.4.9.tar.gz`

## Comparing `rust_circuit-0.4.8.tar` & `rust_circuit-0.4.9.tar`

### file list

```diff
@@ -1,226 +1,230 @@
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/Cargo.toml
--rw-r--r--   0     1001     1002    50453 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/iterative_matcher.rs
--rw-r--r--   0     1001     1002     2449 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/lib.rs
--rw-r--r--   0     1001     1002     3340 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/library.rs
--rw-r--r--   0     1001     1002    16317 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/matcher.rs
--rw-r--r--   0     1001     1002    16302 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/matcher_debug.rs
--rw-r--r--   0     1001     1002    24467 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/operations.rs
--rw-r--r--   0     1001     1002    25230 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/sampler.rs
--rw-r--r--   0     1001     1002     2788 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/get_update_node/src/transform.rs
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/rr_util/Cargo.toml
--rw-r--r--   0     1001     1002      264 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/get_primes.py
--rw-r--r--   0     1001     1002    40000 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/primes.bin
--rw-r--r--   0     1001     1002      242 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/py_circuit_interop.py
--rw-r--r--   0     1001     1002    13806 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/rust_circuit_type_utils.py
--rw-r--r--   0     1001     1002    10681 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/caching.rs
--rw-r--r--   0     1001     1002     2690 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/char_tokenizer.rs
--rw-r--r--   0     1001     1002    13479 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/compact_data.rs
--rw-r--r--   0     1001     1002     4381 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/conv_shape.rs
--rw-r--r--   0     1001     1002     1748 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/eq_by_big_hash.rs
--rw-r--r--   0     1001     1002     7947 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/errors_util.rs
--rw-r--r--   0     1001     1002     1521 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/lazy.rs
--rw-r--r--   0     1001     1002     3263 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/lib.rs
--rw-r--r--   0     1001     1002     6284 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/lru_cache.rs
--rw-r--r--   0     1001     1002     4240 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/name.rs
--rw-r--r--   0     1001     1002    29795 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/opt_einsum.rs
--rw-r--r--   0     1001     1002     4647 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/print.rs
--rw-r--r--   0     1001     1002    21484 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/py_types.rs
--rw-r--r--   0     1001     1002     2513 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/python_callables.rs
--rw-r--r--   0     1001     1002     6591 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/python_wrapped.rs
--rw-r--r--   0     1001     1002    63612 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/rearrange_spec.rs
--rw-r--r--   0     1001     1002     4587 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/repr.rs
--rw-r--r--   0     1001     1002     2571 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/rrfs.rs
--rw-r--r--   0     1001     1002     1392 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/set_cover.rs
--rw-r--r--   0     1001     1002    16518 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/shape.rs
--rw-r--r--   0     1001     1002    12476 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/tensor_db.rs
--rw-r--r--   0     1001     1002    48108 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/tensor_util.rs
--rw-r--r--   0     1001     1002     1982 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/union_find.rs
--rw-r--r--   0     1001     1002    21225 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/src/util.rs
--rw-r--r--   0     1001     1002     7319 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/rr_util/tensor_hash.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/Cargo.toml
--rw-r--r--   0     1001     1002    79045 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/algebraic_rewrite.rs
--rw-r--r--   0     1001     1002    11085 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/batching.rs
--rw-r--r--   0     1001     1002     1351 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/bin/print_simp_fn_stub_part.rs
--rw-r--r--   0     1001     1002     3167 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/canonicalize.rs
--rw-r--r--   0     1001     1002     7001 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/circuit_evaluate.rs
--rw-r--r--   0     1001     1002     2462 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/circuit_manipulation.rs
--rw-r--r--   0     1001     1002    14390 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/circuit_optimizer.rs
--rw-r--r--   0     1001     1002     2516 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/compiler_heuristics.rs
--rw-r--r--   0     1001     1002     1096 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/compiler_strip.rs
--rw-r--r--   0     1001     1002    16712 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/concat_rewrite.rs
--rw-r--r--   0     1001     1002     4293 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/debugging.rs
--rw-r--r--   0     1001     1002    31150 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/deep_rewrite.rs
--rw-r--r--   0     1001     1002    14182 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/diag_rewrite.rs
--rw-r--r--   0     1001     1002     4341 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/generalfunction_rewrite.rs
--rw-r--r--   0     1001     1002    11026 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/lib.rs
--rw-r--r--   0     1001     1002     9399 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/module_rewrite.rs
--rw-r--r--   0     1001     1002     6850 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/nb_rewrites.rs
--rw-r--r--   0     1001     1002      528 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/sampling.rs
--rw-r--r--   0     1001     1002    12774 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/scatter_rewrite.rs
--rw-r--r--   0     1001     1002     7764 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/schedule_send.rs
--rw-r--r--   0     1001     1002    44864 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/scheduled_execution.rs
--rw-r--r--   0     1001     1002    47583 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/scheduling_alg.rs
--rw-r--r--   0     1001     1002     1665 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/server.rs
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/circuit_print/Cargo.toml
--rw-r--r--   0     1001     1002      454 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_print/lib.rs
--rw-r--r--   0     1001     1002    43636 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_print/parsing.rs
--rw-r--r--   0     1001     1002    40231 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_print/print.rs
--rw-r--r--   0     1001     1002    27481 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_print/print_html.rs
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/expand_node/Cargo.toml
--rw-r--r--   0     1001     1002    33231 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/expand_node/lib.rs
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/Cargo.toml
--rw-r--r--   0     1001     1002       71 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/build.rs
--rw-r--r--   0     1001     1002     3067 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/auto_name.rs
--rw-r--r--   0     1001     1002      351 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/bin/print_functions.rs
--rw-r--r--   0     1001     1002     1007 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/cached_circuit_properties.rs
--rw-r--r--   0     1001     1002    37126 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit.rs
--rw-r--r--   0     1001     1002     7377 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit_info.rs
--rw-r--r--   0     1001     1002     5610 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit_node_private.rs
--rw-r--r--   0     1001     1002    13919 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit_utils.rs
--rw-r--r--   0     1001     1002    47830 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/computational_node.rs
--rw-r--r--   0     1001     1002     9308 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/constant.rs
--rw-r--r--   0     1001     1002    13175 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/cumulant.rs
--rw-r--r--   0     1001     1002     8495 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/errors.rs
--rw-r--r--   0     1001     1002    55658 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/generalfunction.rs
--rw-r--r--   0     1001     1002    17413 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/lib.rs
--rw-r--r--   0     1001     1002    57626 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/module.rs
--rw-r--r--   0     1001     1002     6809 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/named_axes.rs
--rw-r--r--   0     1001     1002      832 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/nrc.rs
--rw-r--r--   0     1001     1002    11273 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/opaque_iterative_matcher.rs
--rw-r--r--   0     1001     1002     2615 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/self_funcs.rs
--rw-r--r--   0     1001     1002    12104 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_base/src/variable_nodes.rs
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/Cargo.toml
--rw-r--r--   0     1001     1002    13182 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/cumulant_rewrites.rs
--rw-r--r--   0     1001     1002     7429 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/diff.rs
--rw-r--r--   0     1001     1002     2631 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/distribute_and_factor.rs
--rw-r--r--   0     1001     1002    19269 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/generalfunction.rs
--rw-r--r--   0     1001     1002     2272 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/index_rewrites.rs
--rw-r--r--   0     1001     1002     2166 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/lib.rs
--rw-r--r--   0     1001     1002    66360 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/modules.rs
--rw-r--r--   0     1001     1002    43315 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/nb_operations/src/nest.rs
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/local_dependencies/circuit_utils/Cargo.toml
--rw-r--r--   0     1001     1002    15385 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_utils/lib.rs
--rw-r--r--   0     1001     1002     1331 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/local_dependencies/circuit_utils/set_of_circuits.rs
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/Cargo.toml
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/.root
--rw-r--r--   0     1001     1002      100 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/.rustfmt.toml
--rw-r--r--   0     1001     1002    35277 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/Cargo.lock
--rw-r--r--   0     1001     1002    10220 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/benches/benches.rs
--rw-r--r--   0     1001     1002       71 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/build.rs
--rw-r--r--   0     1001     1002     1971 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/dao.md
--rw-r--r--   0     1001     1002     1570 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/faq.md
--rw-r--r--   0     1001     1002      486 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/naming_rules.md
--rw-r--r--   0     1001     1002      271 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/pyproject.toml
--rw-r--r--   0     1001     1002      141 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/__init__.py
--rw-r--r--   0     1001     1002     1257 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/_rust.py
--rw-r--r--   0     1001     1002   149486 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/_rust.pyi
--rw-r--r--   0     1001     1002    54828 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/algebric_rewrite.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/__init__.py
--rw-r--r--   0     1001     1002     3902 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/dataset.py
--rw-r--r--   0     1001     1002    19023 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/experiment.py
--rw-r--r--   0     1001     1002    25212 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/hypothesis.py
--rw-r--r--   0     1001     1002     1249 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/testing_utils.py
--rw-r--r--   0     1001     1002     4453 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/cum_algo.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/__init__.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/causal_scrubbing/__init__.py
--rw-r--r--   0     1001     1002    23195 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/causal_scrubbing/causal_scrubbing_simple.py
--rw-r--r--   0     1001     1002    18088 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/causal_scrubbing/incr_number_simple.py
--rw-r--r--   0     1001     1002    10088 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/causal_scrubbing/pool.py
--rw-r--r--   0     1001     1002     1189 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/notebook_testing.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/__init__.py
--rw-r--r--   0     1001     1002    41991 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/causal_scrubbing_experiments.py
--rw-r--r--   0     1001     1002    11222 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/setup.py
--rw-r--r--   0     1001     1002     9949 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/test_paren_balancer_exercises.py
--rw-r--r--   0     1001     1002     4623 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/writeup_attribution_plots.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/__init__.py
--rw-r--r--   0     1001     1002    11318 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/basic_scope_manager.py
--rw-r--r--   0     1001     1002    12948 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/custom_general_function.py
--rw-r--r--   0     1001     1002     1726 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/fancy_error.py
--rw-r--r--   0     1001     1002    19812 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/handcrafted_model_cumulants.py
--rw-r--r--   0     1001     1002     8388 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/iterative_matchers.py
--rw-r--r--   0     1001     1002    30679 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/modules_and_symbols.py
--rw-r--r--   0     1001     1002    19267 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/nest.py
--rw-r--r--   0     1001     1002     5438 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/printing_parsing.py
--rw-r--r--   0     1001     1002    11787 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/push_down_index.py
--rw-r--r--   0     1001     1002     3977 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/push_down_module.py
--rw-r--r--   0     1001     1002     2899 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/save_models.py
--rw-r--r--   0     1001     1002     1185 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/simp.py
--rw-r--r--   0     1001     1002     9004 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/transformer_config.py
--rw-r--r--   0     1001     1002     7446 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/uitest.py
--rw-r--r--   0     1001     1002     2518 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/general_function_spec_base.py
--rw-r--r--   0     1001     1002     2572 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/generalfuncs/rotary_pos_emb.py
--rw-r--r--   0     1001     1002      111 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/index_util/__init__.py
--rw-r--r--   0     1001     1002    13948 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/index_util/internal/general_function.py
--rw-r--r--   0     1001     1002     4198 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/index_util/internal/infer_shapes.py
--rw-r--r--   0     1001     1002     7380 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/index_util/internal/ops.py
--rw-r--r--   0     1001     1002     5021 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/index_util/internal/parse.py
--rw-r--r--   0     1001     1002    12288 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/index_util/internal/resolve.py
--rw-r--r--   0     1001     1002     5700 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/index_util/internal/view.py
--rw-r--r--   0     1001     1002    14071 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/interop_rust.py
--rw-r--r--   0     1001     1002     6807 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/jax_to_module.py
--rw-r--r--   0     1001     1002    18429 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/model_rewrites.py
--rw-r--r--   0     1001     1002    34307 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/module_library.py
--rw-r--r--   0     1001     1002      970 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/module_utils.py
--rw-r--r--   0     1001     1002      725 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/optional.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/py.typed
--rw-r--r--   0     1001     1002     3367 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/py_utils.py
--rw-r--r--   0     1001     1002      233 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/rrfs.py
--rw-r--r--   0     1001     1002     7727 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/scope_manager.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/ui/__init__.py
--rw-r--r--   0     1001     1002    14365 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/ui/circuits_very_named_tensor.py
--rw-r--r--   0     1001     1002     5566 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/ui/cui.py
--rw-r--r--   0     1001     1002     3799 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/ui/encoding.py
--rw-r--r--   0     1001     1002     3250 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/ui/ui.py
--rw-r--r--   0     1001     1002    18757 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/rust_circuit/ui/very_named_tensor.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/__init__.py
--rw-r--r--   0     1001     1002        0 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/causal_scrubbing/__init__.py
--rw-r--r--   0     1001     1002    26807 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/causal_scrubbing/test_experiment.py
--rw-r--r--   0     1001     1002     7634 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/causal_scrubbing/test_hypothesis.py
--rw-r--r--   0     1001     1002      205 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/requirements.txt
--rw-r--r--   0     1001     1002    40100 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_algebric_rewrites.py
--rw-r--r--   0     1001     1002     2135 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_auto_names.py
--rw-r--r--   0     1001     1002      835 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_circuit_type.py
--rw-r--r--   0     1001     1002     1506 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_conv.py
--rw-r--r--   0     1001     1002     2322 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_convenience_methods.py
--rw-r--r--   0     1001     1002    11684 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_cum_algo.py
--rw-r--r--   0     1001     1002     2430 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_expand_at_axes.py
--rw-r--r--   0     1001     1002     2055 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_expand_symbolic.py
--rw-r--r--   0     1001     1002     3098 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_flags.py
--rw-r--r--   0     1001     1002     7926 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_gen_index.py
--rw-r--r--   0     1001     1002     3682 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_general_function.py
--rw-r--r--   0     1001     1002      383 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_immutable_check.py
--rw-r--r--   0     1001     1002    14674 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_index_util.py
--rw-r--r--   0     1001     1002     5108 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_jax_to_module.py
--rw-r--r--   0     1001     1002    12535 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_models.py
--rw-r--r--   0     1001     1002    60554 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_module.py
--rw-r--r--   0     1001     1002     1075 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_nb_rewrites.py
--rw-r--r--   0     1001     1002     4626 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_nest.py
--rw-r--r--   0     1001     1002     3130 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_notebooks_and_demos.py
--rw-r--r--   0     1001     1002     6761 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_push_down_index.py
--rw-r--r--   0     1001     1002      824 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_python_callables.py
--rw-r--r--   0     1001     1002     4498 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_batching.py
--rw-r--r--   0     1001     1002    55127 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_get_update.py
--rw-r--r--   0     1001     1002     3322 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_large_models.py
--rw-r--r--   0     1001     1002    99025 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_printing.py
--rw-r--r--   0     1001     1002     2441 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_python_manipulation.py
--rw-r--r--   0     1001     1002    71610 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_rewrite.py
--rw-r--r--   0     1001     1002     2561 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_schedule.py
--rw-r--r--   0     1001     1002     3289 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_rust_variables.py
--rw-r--r--   0     1001     1002    32752 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_sample_transform.py
--rw-r--r--   0     1001     1002      735 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_schedule_serialize.py
--rw-r--r--   0     1001     1002      496 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_serialization.py
--rw-r--r--   0     1001     1002      197 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_server.py
--rw-r--r--   0     1001     1002      282 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_set_of_circuit.py
--rw-r--r--   0     1001     1002      371 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_tensor_saving.py
--rw-r--r--   0     1001     1002     1469 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/test_type_alias_import.py
--rw-r--r--   0     1001     1002     1166 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/python/tests/util.py
--rw-r--r--   0     1001     1002     5360 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/readme.md
--rw-r--r--   0     1001     1002       43 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/rust-toolchain.toml
--rw-r--r--   0     1001     1002     2811 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/rust_circuit_example.py
--rw-r--r--   0     1001     1002     2882 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/rust_rewrite_example.py
--rw-r--r--   0     1001     1002      521 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/src/bin/print_exception_stubs.rs
--rw-r--r--   0     1001     1002     2357 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/src/bin/to_profile.rs
--rw-r--r--   0     1001     1002     3839 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/src/lib.rs
--rw-r--r--   0     1001     1002     1367 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/tests/compiler_bench_runs.rs
--rw-r--r--   0     1001     1002    12073 2023-03-16 22:47:25.000000 rust_circuit-0.4.8/tests/tests.rs
--rw-r--r--   0        0        0      219 1970-01-01 00:00:00.000000 rust_circuit-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/Cargo.toml
+-rw-r--r--   0     1001     1002       71 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/build.rs
+-rw-r--r--   0     1001     1002     3067 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/auto_name.rs
+-rw-r--r--   0     1001     1002      351 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/bin/print_functions.rs
+-rw-r--r--   0     1001     1002     1007 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/cached_circuit_properties.rs
+-rw-r--r--   0     1001     1002    37126 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit.rs
+-rw-r--r--   0     1001     1002     7377 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit_info.rs
+-rw-r--r--   0     1001     1002     5610 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit_node_private.rs
+-rw-r--r--   0     1001     1002    13919 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit_utils.rs
+-rw-r--r--   0     1001     1002    47830 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/computational_node.rs
+-rw-r--r--   0     1001     1002     9308 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/constant.rs
+-rw-r--r--   0     1001     1002    13175 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/cumulant.rs
+-rw-r--r--   0     1001     1002     8530 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/errors.rs
+-rw-r--r--   0     1001     1002    78362 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/generalfunction.rs
+-rw-r--r--   0     1001     1002    17831 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/lib.rs
+-rw-r--r--   0     1001     1002    57708 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/module.rs
+-rw-r--r--   0     1001     1002     6809 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/named_axes.rs
+-rw-r--r--   0     1001     1002      832 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/nrc.rs
+-rw-r--r--   0     1001     1002    11242 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/opaque_iterative_matcher.rs
+-rw-r--r--   0     1001     1002     2422 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/self_funcs.rs
+-rw-r--r--   0     1001     1002    12104 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_base/src/variable_nodes.rs
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/Cargo.toml
+-rw-r--r--   0     1001     1002    13182 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/cumulant_rewrites.rs
+-rw-r--r--   0     1001     1002    10490 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/diff.rs
+-rw-r--r--   0     1001     1002     2631 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/distribute_and_factor.rs
+-rw-r--r--   0     1001     1002    19893 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/generalfunction.rs
+-rw-r--r--   0     1001     1002     2272 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/index_rewrites.rs
+-rw-r--r--   0     1001     1002     2166 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/lib.rs
+-rw-r--r--   0     1001     1002    66360 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/modules.rs
+-rw-r--r--   0     1001     1002    43315 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/nb_operations/src/nest.rs
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/circuit_print/Cargo.toml
+-rw-r--r--   0     1001     1002      454 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_print/lib.rs
+-rw-r--r--   0     1001     1002    43636 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_print/parsing.rs
+-rw-r--r--   0     1001     1002    38372 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_print/print.rs
+-rw-r--r--   0     1001     1002    27209 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_print/print_html.rs
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/rr_util/Cargo.toml
+-rw-r--r--   0     1001     1002      264 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/get_primes.py
+-rw-r--r--   0     1001     1002    40000 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/primes.bin
+-rw-r--r--   0     1001     1002      242 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/py_circuit_interop.py
+-rw-r--r--   0     1001     1002    14393 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/rust_circuit_type_utils.py
+-rw-r--r--   0     1001     1002    10681 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/caching.rs
+-rw-r--r--   0     1001     1002     2690 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/char_tokenizer.rs
+-rw-r--r--   0     1001     1002    13479 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/compact_data.rs
+-rw-r--r--   0     1001     1002     4381 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/conv_shape.rs
+-rw-r--r--   0     1001     1002     1748 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/eq_by_big_hash.rs
+-rw-r--r--   0     1001     1002     7947 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/errors_util.rs
+-rw-r--r--   0     1001     1002     1521 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/lazy.rs
+-rw-r--r--   0     1001     1002     3340 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/lib.rs
+-rw-r--r--   0     1001     1002     6284 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/lru_cache.rs
+-rw-r--r--   0     1001     1002     4240 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/name.rs
+-rw-r--r--   0     1001     1002    29795 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/opt_einsum.rs
+-rw-r--r--   0     1001     1002     4318 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/print.rs
+-rw-r--r--   0     1001     1002    21778 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/py_types.rs
+-rw-r--r--   0     1001     1002     2513 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/python_callables.rs
+-rw-r--r--   0     1001     1002     6591 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/python_wrapped.rs
+-rw-r--r--   0     1001     1002    63612 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/rearrange_spec.rs
+-rw-r--r--   0     1001     1002     4587 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/repr.rs
+-rw-r--r--   0     1001     1002     2571 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/rrfs.rs
+-rw-r--r--   0     1001     1002     1392 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/set_cover.rs
+-rw-r--r--   0     1001     1002    16518 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/shape.rs
+-rw-r--r--   0     1001     1002     5500 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/signal.rs
+-rw-r--r--   0     1001     1002    12476 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/tensor_db.rs
+-rw-r--r--   0     1001     1002    48108 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/tensor_util.rs
+-rw-r--r--   0     1001     1002     1982 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/union_find.rs
+-rw-r--r--   0     1001     1002    21237 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/src/util.rs
+-rw-r--r--   0     1001     1002     7454 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/rr_util/tensor_hash.py
+-rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/Cargo.toml
+-rw-r--r--   0     1001     1002    50559 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/iterative_matcher.rs
+-rw-r--r--   0     1001     1002     2449 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/lib.rs
+-rw-r--r--   0     1001     1002     3340 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/library.rs
+-rw-r--r--   0     1001     1002    16317 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/matcher.rs
+-rw-r--r--   0     1001     1002    16065 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/matcher_debug.rs
+-rw-r--r--   0     1001     1002    27369 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/operations.rs
+-rw-r--r--   0     1001     1002    25539 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/sampler.rs
+-rw-r--r--   0     1001     1002     2542 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/get_update_node/src/transform.rs
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/circuit_utils/Cargo.toml
+-rw-r--r--   0     1001     1002    15385 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_utils/lib.rs
+-rw-r--r--   0     1001     1002     1331 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_utils/set_of_circuits.rs
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/expand_node/Cargo.toml
+-rw-r--r--   0     1001     1002    33006 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/expand_node/lib.rs
+-rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/Cargo.toml
+-rw-r--r--   0     1001     1002    79035 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/algebraic_rewrite.rs
+-rw-r--r--   0     1001     1002    11085 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/batching.rs
+-rw-r--r--   0     1001     1002     1351 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/bin/print_simp_fn_stub_part.rs
+-rw-r--r--   0     1001     1002     3167 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/canonicalize.rs
+-rw-r--r--   0     1001     1002     8161 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/circuit_evaluate.rs
+-rw-r--r--   0     1001     1002     2462 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/circuit_manipulation.rs
+-rw-r--r--   0     1001     1002    14391 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/circuit_optimizer.rs
+-rw-r--r--   0     1001     1002     2516 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/compiler_heuristics.rs
+-rw-r--r--   0     1001     1002     1096 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/compiler_strip.rs
+-rw-r--r--   0     1001     1002    16699 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/concat_rewrite.rs
+-rw-r--r--   0     1001     1002     4293 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/debugging.rs
+-rw-r--r--   0     1001     1002    31150 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/deep_rewrite.rs
+-rw-r--r--   0     1001     1002    14182 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/diag_rewrite.rs
+-rw-r--r--   0     1001     1002     4394 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/generalfunction_rewrite.rs
+-rw-r--r--   0     1001     1002    11026 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/lib.rs
+-rw-r--r--   0     1001     1002     9399 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/module_rewrite.rs
+-rw-r--r--   0     1001     1002     6850 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/nb_rewrites.rs
+-rw-r--r--   0     1001     1002      528 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/sampling.rs
+-rw-r--r--   0     1001     1002    12774 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/scatter_rewrite.rs
+-rw-r--r--   0     1001     1002     7369 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/schedule_send.rs
+-rw-r--r--   0     1001     1002    50604 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/scheduled_execution.rs
+-rw-r--r--   0     1001     1002    47388 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/scheduling_alg.rs
+-rw-r--r--   0     1001     1002     1665 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/server.rs
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/Cargo.toml
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/.root
+-rw-r--r--   0     1001     1002      100 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/.rustfmt.toml
+-rw-r--r--   0     1001     1002    35595 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/Cargo.lock
+-rw-r--r--   0     1001     1002    10198 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/benches/benches.rs
+-rw-r--r--   0     1001     1002       71 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/build.rs
+-rw-r--r--   0     1001     1002     1971 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/dao.md
+-rw-r--r--   0     1001     1002     1570 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/faq.md
+-rw-r--r--   0     1001     1002      486 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/naming_rules.md
+-rw-r--r--   0     1001     1002      271 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/pyproject.toml
+-rw-r--r--   0     1001     1002      219 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/__init__.py
+-rw-r--r--   0     1001     1002     1257 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/_rust.py
+-rw-r--r--   0     1001     1002   152683 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/_rust.pyi
+-rw-r--r--   0     1001     1002    54828 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/algebric_rewrite.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/__init__.py
+-rw-r--r--   0     1001     1002     3902 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/dataset.py
+-rw-r--r--   0     1001     1002    19023 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/experiment.py
+-rw-r--r--   0     1001     1002    25212 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/hypothesis.py
+-rw-r--r--   0     1001     1002     1249 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/testing_utils.py
+-rw-r--r--   0     1001     1002     4453 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/cum_algo.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/__init__.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/causal_scrubbing/__init__.py
+-rw-r--r--   0     1001     1002    23195 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/causal_scrubbing/causal_scrubbing_simple.py
+-rw-r--r--   0     1001     1002    18088 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/causal_scrubbing/incr_number_simple.py
+-rw-r--r--   0     1001     1002    10088 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/causal_scrubbing/pool.py
+-rw-r--r--   0     1001     1002     1189 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/notebook_testing.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/__init__.py
+-rw-r--r--   0     1001     1002    41991 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/causal_scrubbing_experiments.py
+-rw-r--r--   0     1001     1002    11222 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/setup.py
+-rw-r--r--   0     1001     1002     9949 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/test_paren_balancer_exercises.py
+-rw-r--r--   0     1001     1002     4623 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/writeup_attribution_plots.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/__init__.py
+-rw-r--r--   0     1001     1002    11318 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/basic_scope_manager.py
+-rw-r--r--   0     1001     1002    14059 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/custom_general_function.py
+-rw-r--r--   0     1001     1002     1726 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/fancy_error.py
+-rw-r--r--   0     1001     1002    19812 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/handcrafted_model_cumulants.py
+-rw-r--r--   0     1001     1002     8388 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/iterative_matchers.py
+-rw-r--r--   0     1001     1002    30679 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/modules_and_symbols.py
+-rw-r--r--   0     1001     1002    19267 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/nest.py
+-rw-r--r--   0     1001     1002     5438 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/printing_parsing.py
+-rw-r--r--   0     1001     1002    11787 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/push_down_index.py
+-rw-r--r--   0     1001     1002     3977 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/push_down_module.py
+-rw-r--r--   0     1001     1002     2899 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/save_models.py
+-rw-r--r--   0     1001     1002     1185 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/simp.py
+-rw-r--r--   0     1001     1002     9086 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/transformer_config.py
+-rw-r--r--   0     1001     1002     7446 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/uitest.py
+-rw-r--r--   0     1001     1002     4929 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/general_function_spec_base.py
+-rw-r--r--   0     1001     1002     5666 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/generalfuncs/mlp_topk.py
+-rw-r--r--   0     1001     1002     2572 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/generalfuncs/rotary_pos_emb.py
+-rw-r--r--   0     1001     1002     1053 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/generalfuncs/test_a_samp_multinomial.py
+-rw-r--r--   0     1001     1002     1892 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/generalfuncs/train_mask.py
+-rw-r--r--   0     1001     1002      111 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/index_util/__init__.py
+-rw-r--r--   0     1001     1002    13948 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/index_util/internal/general_function.py
+-rw-r--r--   0     1001     1002     4198 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/index_util/internal/infer_shapes.py
+-rw-r--r--   0     1001     1002     7380 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/index_util/internal/ops.py
+-rw-r--r--   0     1001     1002     5021 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/index_util/internal/parse.py
+-rw-r--r--   0     1001     1002    12288 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/index_util/internal/resolve.py
+-rw-r--r--   0     1001     1002     5700 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/index_util/internal/view.py
+-rw-r--r--   0     1001     1002    14071 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/interop_rust.py
+-rw-r--r--   0     1001     1002     6807 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/jax_to_module.py
+-rw-r--r--   0     1001     1002    18240 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/model_rewrites.py
+-rw-r--r--   0     1001     1002    78002 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/module_library.py
+-rw-r--r--   0     1001     1002      970 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/module_utils.py
+-rw-r--r--   0     1001     1002      725 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/optional.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/py.typed
+-rw-r--r--   0     1001     1002     3367 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/py_utils.py
+-rw-r--r--   0     1001     1002      233 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/rrfs.py
+-rw-r--r--   0     1001     1002     7727 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/scope_manager.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/ui/__init__.py
+-rw-r--r--   0     1001     1002    14365 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/ui/circuits_very_named_tensor.py
+-rw-r--r--   0     1001     1002     5566 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/ui/cui.py
+-rw-r--r--   0     1001     1002     3799 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/ui/encoding.py
+-rw-r--r--   0     1001     1002     3250 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/ui/ui.py
+-rw-r--r--   0     1001     1002    18757 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/rust_circuit/ui/very_named_tensor.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/__init__.py
+-rw-r--r--   0     1001     1002        0 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/causal_scrubbing/__init__.py
+-rw-r--r--   0     1001     1002    26807 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/causal_scrubbing/test_experiment.py
+-rw-r--r--   0     1001     1002     7634 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/causal_scrubbing/test_hypothesis.py
+-rw-r--r--   0     1001     1002      205 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/requirements.txt
+-rw-r--r--   0     1001     1002    40100 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_algebric_rewrites.py
+-rw-r--r--   0     1001     1002     2135 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_auto_names.py
+-rw-r--r--   0     1001     1002      835 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_circuit_type.py
+-rw-r--r--   0     1001     1002     1506 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_conv.py
+-rw-r--r--   0     1001     1002     2322 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_convenience_methods.py
+-rw-r--r--   0     1001     1002    11684 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_cum_algo.py
+-rw-r--r--   0     1001     1002     2430 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_expand_at_axes.py
+-rw-r--r--   0     1001     1002     2055 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_expand_symbolic.py
+-rw-r--r--   0     1001     1002     3098 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_flags.py
+-rw-r--r--   0     1001     1002     7926 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_gen_index.py
+-rw-r--r--   0     1001     1002     4246 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_general_function.py
+-rw-r--r--   0     1001     1002      383 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_immutable_check.py
+-rw-r--r--   0     1001     1002    14674 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_index_util.py
+-rw-r--r--   0     1001     1002     5108 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_jax_to_module.py
+-rw-r--r--   0     1001     1002    12535 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_models.py
+-rw-r--r--   0     1001     1002    60554 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_module.py
+-rw-r--r--   0     1001     1002     1075 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_nb_rewrites.py
+-rw-r--r--   0     1001     1002     4626 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_nest.py
+-rw-r--r--   0     1001     1002     3130 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_notebooks_and_demos.py
+-rw-r--r--   0     1001     1002     6761 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_push_down_index.py
+-rw-r--r--   0     1001     1002      824 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_python_callables.py
+-rw-r--r--   0     1001     1002     4498 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_batching.py
+-rw-r--r--   0     1001     1002    55589 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_get_update.py
+-rw-r--r--   0     1001     1002     3322 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_large_models.py
+-rw-r--r--   0     1001     1002    99006 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_printing.py
+-rw-r--r--   0     1001     1002     2441 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_python_manipulation.py
+-rw-r--r--   0     1001     1002    71610 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_rewrite.py
+-rw-r--r--   0     1001     1002     2561 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_schedule.py
+-rw-r--r--   0     1001     1002     3289 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_rust_variables.py
+-rw-r--r--   0     1001     1002    32752 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_sample_transform.py
+-rw-r--r--   0     1001     1002      735 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_schedule_serialize.py
+-rw-r--r--   0     1001     1002      496 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_serialization.py
+-rw-r--r--   0     1001     1002      197 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_server.py
+-rw-r--r--   0     1001     1002      282 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_set_of_circuit.py
+-rw-r--r--   0     1001     1002      371 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_tensor_saving.py
+-rw-r--r--   0     1001     1002     1469 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/test_type_alias_import.py
+-rw-r--r--   0     1001     1002     1166 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/python/tests/util.py
+-rw-r--r--   0     1001     1002     5360 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/readme.md
+-rw-r--r--   0     1001     1002       43 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/rust-toolchain.toml
+-rw-r--r--   0     1001     1002     2811 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/rust_circuit_example.py
+-rw-r--r--   0     1001     1002     2882 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/rust_rewrite_example.py
+-rw-r--r--   0     1001     1002      521 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/src/bin/print_exception_stubs.rs
+-rw-r--r--   0     1001     1002     2357 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/src/bin/to_profile.rs
+-rw-r--r--   0     1001     1002     3789 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/src/lib.rs
+-rw-r--r--   0     1001     1002     1376 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/tests/compiler_bench_runs.rs
+-rw-r--r--   0     1001     1002    12073 2023-04-18 20:10:13.000000 rust_circuit-0.4.9/tests/tests.rs
+-rw-r--r--   0        0        0      219 1970-01-01 00:00:00.000000 rust_circuit-0.4.9/PKG-INFO
```

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/get_update_node/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 pyo3= { features=["num-bigint", "multiple-pymethods", "anyhow", "macros"], git = "https://github.com/redwoodresearch/pyo3" }
 cached= {version = "0.38.0", default-features = false}
 num-bigint= "0.4.3"
 anyhow= { version = "1.0.60", features = ["backtrace"] }
 thiserror= "1.0.32"
 paste= "1.0.8"
 itertools= "0.10.3"
-smallvec= { version = "1.10.0", features = ["union"] }
+smallvec= { version = "1.10.0", features = ["union", "specialization"] }
 macro_rules_attribute= "0.1.2"
 rustc-hash= "1.1.0"
 regex= "1.6.0"
 
 rr_util = {path = "../rr_util" }
 circuit_base = {path = "../circuit_base" }
 circuit_utils = {path = "../circuit_utils" }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/iterative_matcher.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/iterative_matcher.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     sync::Arc,
     vec,
 };
 
 use anyhow::{bail, Context, Result};
 use circuit_base::{
     opaque_iterative_matcher::{
-        Update as BaseUpdate, UpdatedIterativeMatcher as BaseUpdatedIterativeMatcher,
+        OpaqueIterativeMatcherVal, Update as BaseUpdate,
+        UpdatedIterativeMatcher as BaseUpdatedIterativeMatcher,
     },
     CircuitNode, CircuitNodeUnion, CircuitRc, CircuitType,
 };
 use circuit_utils::SetOfCircuitIdentities;
 use macro_rules_attribute::apply;
 use pyo3::{
     exceptions::{PyTypeError, PyValueError},
@@ -32,14 +33,15 @@
     },
 };
 use thiserror::Error;
 use uuid::uuid;
 
 use crate::{
     library::{apply_in_traversal, replace_outside_traversal_symbols},
+    operations::AssertFound,
     AnyFound, BoundAnyFound, BoundGetter, BoundUpdater, Getter, Matcher, MatcherData,
     MatcherFromPyBase, MatcherRc, TransformRc, Updater,
 };
 
 #[derive(Clone, FromPyObject)]
 pub enum IterativeMatcherFromPy {
     BaseMatch(MatcherFromPyBase),
@@ -664,14 +666,18 @@
                 }
                 Ok(())
             }
             IterativeMatcherData::All(_) => Ok(()), // TODO
             IterativeMatcherData::PyFunc(_) | IterativeMatcherData::Raw(_) => Ok(()),
         }
     }
+
+    pub fn as_opaque(&self) -> OpaqueIterativeMatcherVal {
+        Python::with_gil(|py| OpaqueIterativeMatcherVal::Py(self.clone().into_py(py)))
+    }
     // TODO: more rust niceness funcs like the py ones!
 }
 
 impl IterativeMatcherRc {
     // -> (found, all_finished, children matchers)
     pub fn match_iterate_continue(
         self,
@@ -1295,57 +1301,57 @@
     pub fn any_found(&self) -> BoundAnyFound {
         AnyFound::new().bind(self_.crc())
     }
 
     #[pyo3(signature=(
         circuit,
         transform,
-        cache_transform = Updater::default().cache_transform,
-        cache_update = Updater::default().cache_update,
         fancy_validate = Updater::default().default_fancy_validate,
-        assert_any_found = Updater::default().default_assert_any_found
+        assert_found = Updater::default().default_assert_found,
+        assert_different = Updater::default().default_assert_different,
     ))]
     pub fn update(
         &self,
         circuit: CircuitRc,
         transform: TransformRc,
-        cache_transform: bool,
-        cache_update: bool,
         fancy_validate: bool,
-        assert_any_found: bool,
+        assert_found: AssertFound,
+        assert_different: bool,
     ) -> Result<CircuitRc> {
-        Updater::new(transform, cache_transform, cache_update, false, false).update(
+        Updater {
+            transform,
+            ..Default::default()
+        }
+        .update(
             circuit,
             self_.crc(),
             Some(fancy_validate),
-            Some(assert_any_found),
+            Some(assert_found),
+            Some(assert_different),
         )
     }
 
     #[pyo3(signature=(
         transform,
-        cache_transform = Updater::default().cache_transform,
-        cache_update = Updater::default().cache_update,
         default_fancy_validate = Updater::default().default_fancy_validate,
-        default_assert_any_found = Updater::default().default_assert_any_found
+        default_assert_found = Updater::default().default_assert_found,
+        default_assert_different = Updater::default().default_assert_different,
     ))]
     pub fn updater(
         &self,
         transform: TransformRc,
-        cache_transform: bool,
-        cache_update: bool,
         default_fancy_validate: bool,
-        default_assert_any_found: bool,
+        default_assert_found: AssertFound,
+        default_assert_different: bool,
     ) -> BoundUpdater {
         Updater::new(
             transform,
-            cache_transform,
-            cache_update,
             default_fancy_validate,
-            default_assert_any_found,
+            default_assert_found,
+            default_assert_different,
         )
         .bind(self_.crc())
     }
 
     pub fn apply_in_traversal(
         &self,
         circuit: CircuitRc,
```

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/lib.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/library.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/library.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/matcher.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/matcher_debug.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/matcher_debug.rs`

 * *Files 3% similar despite different names*

```diff
@@ -359,34 +359,32 @@
     print_options: PrintOptions,
 ) -> Result<String> {
     let mut result = "".to_owned();
     let mut seen: HashSet<(CircuitRc, IterativeMatcherRc)> = Default::default();
     fn recurse(
         circuit: CircuitRc,
         matcher: IterativeMatcherRc,
-        last_child_stack: Vec<bool>,
+        prefix: &str,
         print_options: &PrintOptions,
         result: &mut String,
         seen: &mut HashSet<(CircuitRc, IterativeMatcherRc)>,
     ) -> Result<()> {
         let key = (circuit.clone(), matcher.clone());
         if !seen.insert(key) {
             writeln!(
                 result,
-                "{}'{}'...",
-                last_child_arrows(&last_child_stack, true, print_options.arrows),
+                "'{}'...\n",
                 circuit.info().name.unwrap_or("".into())
             )
             .unwrap();
             return Ok(());
         }
         let matched: IterateMatchResults = matcher.match_iterate(circuit.clone())?;
         let line_repr: String = format!(
-            "{}{}{}{}\n",
-            last_child_arrows(&last_child_stack, true, print_options.arrows),
+            "{}{}{}\n",
             print_options.repr_line_info(circuit.clone())?,
             if matched.found {
                 color(" # Found", clicolor!(Green))
             } else {
                 "".to_owned()
             },
             color(
@@ -395,41 +393,35 @@
             ),
         );
         result.push_str(&line_repr);
 
         let child_matchers = per_child(matched.updated, matcher, circuit.num_children());
         for (i, (child, child_matcher)) in zip(circuit.children(), child_matchers).enumerate() {
             if let Some(child_matcher) = child_matcher {
-                let new_last_child_stack = last_child_stack
-                    .iter()
-                    .cloned()
-                    .chain(once(i == circuit.num_children() - 1))
-                    .collect();
+                let next_prefix = last_child_arrows(
+                    result,
+                    prefix,
+                    i == circuit.num_children() - 1,
+                    print_options.arrows,
+                );
                 recurse(
                     child,
                     child_matcher,
-                    new_last_child_stack,
+                    &next_prefix,
                     print_options,
                     result,
                     seen,
                 )?;
             } else {
                 // reuslt.push_str("")
             }
         }
         Ok(())
     }
-    recurse(
-        circuit,
-        matcher,
-        vec![],
-        &print_options,
-        &mut result,
-        &mut seen,
-    )?;
+    recurse(circuit, matcher, "", &print_options, &mut result, &mut seen)?;
     Ok(result)
 }
 
 #[pyfunction]
 pub fn print_matcher_debug(
     circuit: CircuitRc,
     matcher: IterativeMatcherRc,
```

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/operations.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/operations.rs`

 * *Files 9% similar despite different names*

```diff
@@ -22,112 +22,159 @@
 use rustc_hash::FxHashSet as HashSet;
 
 use crate::{
     iterative_matcher::{all_finished, function_per_child, per_child, per_child_with_term},
     IterateMatchResults, IterativeMatcherRc, Transform, TransformData, TransformRc,
 };
 
+#[derive(FromPyObject, Clone, Debug)]
+pub enum AssertFound {
+    Any(bool),
+    Num(usize),
+}
+
+impl IntoPy<PyObject> for AssertFound {
+    fn into_py(self, py: Python<'_>) -> PyObject {
+        match self {
+            AssertFound::Any(a) => a.into_py(py),
+            AssertFound::Num(n) => n.into_py(py),
+        }
+    }
+}
+
+impl AssertFound {
+    fn validate(
+        &self,
+        x: &UpdateOutput,
+        circuit: &CircuitRc,
+        matchers: &[IterativeMatcherRc],
+    ) -> Result<()> {
+        let m = x.found_set.as_ref().map_or(0, |x| x.len());
+        match *self {
+            AssertFound::Any(b) => {
+                if b && m == 0 {
+                    bail!(format!(
+                        "No matches found\nmatcher(s): {matchers:?}, circuit: {circuit:?}"
+                    ));
+                }
+            }
+            AssertFound::Num(n) => {
+                if m != n {
+                    bail!(format!("Wrong number of matches found, found {m} assert_found={n}\nmatcher(s): {matchers:?}, circuit: {circuit:?}"));
+                }
+            }
+        };
+        Ok(())
+    }
+}
+
+impl Default for AssertFound {
+    fn default() -> Self {
+        Self::Any(false)
+    }
+}
+
 #[derive(Debug, Clone)]
 pub(super) struct UpdateOutput {
     pub(super) updated: CircuitRc,
-    pub(super) any_found: bool,
+    pub(super) found_set: Option<HashSet<HashBytes>>,
 }
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct Updater {
     #[pyo3(get)]
     pub(super) transform: TransformRc,
-    #[pyo3(get)]
-    pub(super) cache_transform: bool,
-    #[pyo3(get)]
-    pub(super) cache_update: bool,
     #[pyo3(get, set)]
     pub(super) default_fancy_validate: bool,
     #[pyo3(get, set)]
-    pub(super) default_assert_any_found: bool,
+    pub(super) default_assert_found: AssertFound,
+    #[pyo3(get, set)]
+    pub(super) default_assert_different: bool,
     pub(super) transform_cache: FastUnboundedCache<HashBytes, CircuitRc>,
     pub(super) updated_cache: FastUnboundedCache<(HashBytes, IterativeMatcherRc), UpdateOutput>,
     pub(super) validation_getter: Getter,
 }
 
 impl Default for Updater {
     fn default() -> Self {
         Self {
             transform: Transform::ident().into(),
-            cache_transform: true,
-            cache_update: true,
             default_fancy_validate: false,
-            default_assert_any_found: false,
+            default_assert_found: AssertFound::Any(false),
+            default_assert_different: false,
             transform_cache: FastUnboundedCache::default(),
             updated_cache: FastUnboundedCache::default(),
             validation_getter: Default::default(),
         }
     }
 }
 
 #[pymethods]
 impl Updater {
     #[new]
     #[pyo3(signature=(
         transform,
-        cache_transform = Updater::default().cache_transform,
-        cache_update = Updater::default().cache_update,
         default_fancy_validate = Updater::default().default_fancy_validate,
-        default_assert_any_found = Updater::default().default_assert_any_found
+        default_assert_found = Updater::default().default_assert_found,
+        default_assert_different = Updater::default().default_assert_different,
     ))]
     pub fn new(
         transform: TransformRc,
-        cache_transform: bool,
-        cache_update: bool,
         default_fancy_validate: bool,
-        default_assert_any_found: bool,
+        default_assert_found: AssertFound,
+        default_assert_different: bool,
     ) -> Self {
         Self {
             transform,
-            cache_transform,
-            cache_update,
             default_fancy_validate,
-            default_assert_any_found,
+            default_assert_found,
+            default_assert_different,
             ..Default::default()
         }
     }
 
     fn __call__(
         &mut self,
         _py: Python<'_>,
         circuit: CircuitRc,
         matcher: IterativeMatcherRc,
         fancy_validate: Option<bool>,
-        assert_any_found: Option<bool>,
+        assert_found: Option<AssertFound>,
+        assert_different: Option<bool>,
     ) -> Result<CircuitRc> {
-        self.update(circuit, matcher, fancy_validate, assert_any_found)
+        self.update(
+            circuit,
+            matcher,
+            fancy_validate,
+            assert_found,
+            assert_different,
+        )
     }
 
     pub fn update(
         &mut self,
         circuit: CircuitRc,
         matcher: IterativeMatcherRc,
         fancy_validate: Option<bool>,
-        assert_any_found: Option<bool>,
+        assert_found: Option<AssertFound>,
+        assert_different: Option<bool>,
     ) -> Result<CircuitRc> {
         if fancy_validate.unwrap_or(self.default_fancy_validate) {
             self.validation_getter
                 .validate(circuit.clone(), matcher.clone())?;
         }
         let out = self.update_impl(circuit.crc(), matcher.crc())?;
-        if assert_any_found.unwrap_or(self.default_assert_any_found) && !out.any_found {
-            bail!(
-                concat!(
-                    "No matches found during update\n",
-                    "matcher: {matcher:?}, circuit: {circuit:?}"
-                ),
-                matcher = matcher,
-                circuit = circuit
-            );
+        assert_found
+            .unwrap_or(self.default_assert_found.clone())
+            .validate(&out, &circuit, &[matcher])?;
+        if assert_different.unwrap_or(self.default_assert_different) && out.updated == circuit {
+            bail!(format!(
+                "update result same as input but assert_different=True, input={circuit:?}"
+            ))
         }
         Ok(out.updated)
     }
 
     pub fn bind(&self, matcher: IterativeMatcherRc) -> BoundUpdater {
         BoundUpdater {
             updater: self.clone(),
@@ -145,32 +192,38 @@
     fn update_impl(
         &mut self,
         circuit: CircuitRc,
         matcher: IterativeMatcherRc,
     ) -> Result<UpdateOutput> {
         let IterateMatchResults { updated, found } = matcher.match_iterate(circuit.clone())?;
 
-        let mut any_found = false;
+        let mut found_set: Option<HashSet<HashBytes>> = None;
         let mut new_circuit =
             function_per_child(updated, matcher, circuit.clone(), |circuit, new_matcher| {
                 let child_out = self_.update_impl(circuit, new_matcher)?;
-                any_found |= child_out.any_found;
+                if let Some(ref mut f) = found_set && let Some(fs) = child_out.found_set {
+                    f.extend(fs);
+                } else {
+                    found_set = child_out.found_set;
+                }
                 Ok(child_out.updated)
             })?;
 
         if found {
-            any_found = true;
+            found_set
+                .get_or_insert_with(|| HashSet::default())
+                .insert(circuit.info().hash);
             if !matches!(self_.transform.data(), TransformData::Ident) {
                 new_circuit = self_.run_transform(new_circuit)?;
             }
         }
 
         Ok(UpdateOutput {
             updated: new_circuit,
-            any_found,
+            found_set,
         })
     }
 
     #[apply(cached_method)]
     #[self_id(self_)]
     #[key(circuit.info().hash)]
     #[use_try]
@@ -197,30 +250,33 @@
     }
 
     fn __call__(
         &mut self,
         _py: Python<'_>,
         circuit: CircuitRc,
         fancy_validate: Option<bool>,
-        assert_any_found: Option<bool>,
+        assert_found: Option<AssertFound>,
+        assert_different: Option<bool>,
     ) -> Result<CircuitRc> {
-        self.update(circuit, fancy_validate, assert_any_found)
+        self.update(circuit, fancy_validate, assert_found, assert_different)
     }
 
     pub fn update(
         &mut self,
         circuit: CircuitRc,
         fancy_validate: Option<bool>,
-        assert_any_found: Option<bool>,
+        assert_found: Option<AssertFound>,
+        assert_different: Option<bool>,
     ) -> Result<CircuitRc> {
         self.updater.update(
             circuit,
             self.matcher.clone(),
             fancy_validate,
-            assert_any_found,
+            assert_found,
+            assert_different,
         )
     }
 }
 
 #[pyclass]
 #[derive(Debug, Clone, Default)]
 pub struct Getter {
@@ -626,15 +682,15 @@
 
     pub fn are_any_found(&mut self, circuit: CircuitRc) -> Result<bool> {
         self.any_found.are_any_found(circuit, self.matcher.clone())
     }
 }
 
 #[pyclass]
-#[derive(Debug, Clone, Default)]
+#[derive(Debug, Clone)]
 pub struct Expander {
     /// Note: we don't currently cache these transforms individually. We could
     /// do this.
     #[pyo3(get)]
     pub(super) replacements: Vec<TransformRc>,
     /// Technically, having all of these matchers stored here isn't important
     /// for key functionality (like unused for caching).
@@ -644,83 +700,104 @@
     #[pyo3(get)]
     pub(super) matchers: Vec<IterativeMatcherRc>,
     #[pyo3(set, get)]
     pub ban_multiple_matches_on_node: bool,
     #[pyo3(set, get)]
     pub default_fancy_validate: bool,
     #[pyo3(set, get)]
-    pub default_assert_any_found: bool,
+    pub default_assert_found: AssertFound,
+    #[pyo3(set, get)]
+    pub default_assert_different: bool,
     #[pyo3(get)]
     pub(super) suffix: Option<String>,
     pub(super) batch_cache:
         FastUnboundedCache<(HashBytes, Vec<IterativeMatcherRc>, HashBytes), UpdateOutput>,
     pub(super) validation_getter: Getter,
 }
 
+impl Default for Expander {
+    fn default() -> Self {
+        Self {
+            replacements: Vec::new(),
+            matchers: Vec::new(),
+            ban_multiple_matches_on_node: false,
+            default_fancy_validate: false,
+            default_assert_found: AssertFound::Any(false),
+            default_assert_different: false,
+            suffix: None,
+            batch_cache: FastUnboundedCache::default(),
+            validation_getter: Default::default(),
+        }
+    }
+}
+
 #[pymethods]
 impl Expander {
     #[new]
     #[pyo3(signature=(
         *expanders,
         ban_multiple_matches_on_node = Expander::default().ban_multiple_matches_on_node,
         default_fancy_validate = Expander::default().default_fancy_validate,
-        default_assert_any_found = Expander::default().default_assert_any_found,
+        default_assert_found = Expander::default().default_assert_found,
+        default_assert_different = Expander::default().default_assert_different,
         suffix = None
     ))]
     pub fn new(
         expanders: Vec<(IterativeMatcherRc, TransformRc)>,
         ban_multiple_matches_on_node: bool,
         default_fancy_validate: bool,
-        default_assert_any_found: bool,
+        default_assert_found: AssertFound,
+        default_assert_different: bool,
         suffix: Option<String>,
     ) -> Self {
         let (matchers, replacements) = expanders.into_iter().map(|(a, b)| (a, b)).unzip();
         Self {
             replacements,
             matchers,
             ban_multiple_matches_on_node,
             default_fancy_validate,
-            default_assert_any_found,
+            default_assert_found,
+            default_assert_different,
             suffix,
             ..Default::default()
         }
     }
 
     fn __call__(
         &mut self,
         _py: Python<'_>,
         circuit: CircuitRc,
         fancy_validate: Option<bool>,
-        assert_any_found: Option<bool>,
+        assert_found: Option<AssertFound>,
+        assert_different: Option<bool>,
     ) -> Result<CircuitRc> {
-        self.batch(circuit, fancy_validate, assert_any_found)
+        self.batch(circuit, fancy_validate, assert_found, assert_different)
     }
 
     pub fn batch(
         &mut self,
         circuit: CircuitRc,
         fancy_validate: Option<bool>,
-        assert_any_found: Option<bool>,
+        assert_found: Option<AssertFound>,
+        assert_different: Option<bool>,
     ) -> Result<CircuitRc> {
         if fancy_validate.unwrap_or(self.default_fancy_validate) {
             for m in &self.matchers {
                 self.validation_getter
                     .validate(circuit.clone(), m.clone())?;
             }
         }
         let out = self.batch_impl(circuit.crc(), self.matchers.clone(), &Default::default())?;
-        if assert_any_found.unwrap_or(self.default_assert_any_found) && !out.any_found {
-            bail!(
-                concat!(
-                    "No matches found during expand\n",
-                    "matchers: {matchers:?}, circuit: {circuit:?}"
-                ),
-                matchers = self.matchers,
-                circuit = circuit,
-            );
+        assert_found
+            .unwrap_or(self.default_assert_found.clone())
+            .validate(&out, &circuit, &self.matchers)?;
+        if assert_different.unwrap_or(self.default_assert_different) && out.updated == circuit {
+            bail!(format!(
+                "Expander result same as input but assert_different=True, input={circuit:?}"
+            ))
         }
         Ok(out.updated)
     }
 }
 
 impl Expander {
     #[apply(cached_method)]
@@ -746,72 +823,80 @@
                 let n_matches = filtered.count();
                 if n_matches != 1 {
                     bail!("multiple matches! got {} != 1", n_matches);
                 }
             }
 
             return Ok(UpdateOutput {
-                updated: self_.replacements[idx].run(circuit)?,
-                any_found: true,
+                updated: self_.replacements[idx].run(circuit.clone())?,
+                found_set: Some([circuit.info().hash].into_iter().collect()),
             });
         }
         if let Some(replaced) = extra_replacements.get(&circuit) {
             return Ok(UpdateOutput {
                 updated: replaced.clone(),
-                any_found: false,
+                found_set: None,
             });
         }
 
         if results.iter().all(|x| all_finished(&x.updated)) && extra_replacements.is_empty() {
             return Ok(UpdateOutput {
                 updated: circuit,
-                any_found: false,
+                found_set: None,
             });
         }
 
         let num_children = circuit.num_children();
 
         let new_matchers: Vec<_> = results
             .into_iter()
             .zip(matchers)
             .map(|(res, matcher)| per_child_with_term(res.updated, matcher, num_children))
             .collect();
         let new_matchers_per = transpose(new_matchers, num_children);
         assert_eq!(new_matchers_per.len(), circuit.num_children());
 
-        let mut any_found = false;
+        let mut found_set: Option<HashSet<HashBytes>> = None;
         let new_children = circuit
             .children()
             .zip(extra_replacements.per_child(&circuit))
             .zip(new_matchers_per.clone())
             .map(|((c, rep), new_matchers)| {
                 let child_out = self_.batch_impl(c, new_matchers, &rep)?;
-                any_found |= child_out.any_found;
+                if let Some(ref mut f) = found_set && let Some(fs) = child_out.found_set {
+                    f.extend(fs);
+                } else {
+                    found_set = child_out.found_set;
+                }
                 Ok(child_out.updated)
             })
             .collect::<Result<_>>()?;
 
         let expanded = expand_node(circuit.clone(), &new_children, &mut |c, rep, child_idx| {
             let out = self_.batch_impl(
                 c,
                 new_matchers_per[child_idx].clone(),
                 &extra_replacements.extend_into(rep),
             )?;
-            any_found |= out.any_found;
+            if let Some(ref mut f) = found_set && let Some(fs) = out.found_set {
+                    f.extend(fs);
+                } else {
+                    found_set = out.found_set;
+                }
             Ok(out.updated)
         })?;
         let expanded = if expanded != circuit {
             expanded.add_suffix(self_.suffix.as_deref())
         } else {
             expanded
         };
 
         Ok(UpdateOutput {
             updated: expanded,
-            any_found,
+            found_set,
         })
     }
 
     pub fn suffix(&self) -> Option<&str> {
         self.suffix.as_deref()
     }
 }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/sampler.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/sampler.rs`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     util::HashBytes,
 };
 use rustc_hash::FxHashSet as HashSet;
 use smallvec::SmallVec as Sv;
 use thiserror::Error;
 
 use crate::{
-    iterative_matcher::function_per_child, restrict, Expander, IterateMatchResults,
-    IterativeMatcherRc, Matcher, Transform, TransformRc,
+    iterative_matcher::function_per_child, operations::AssertFound, restrict, Expander,
+    IterateMatchResults, IterativeMatcherRc, Matcher, Transform, TransformRc,
 };
 
 fn_struct!(pub Seeder:Fn(circuit:CircuitRc)->i64);
 
 #[pyfunction]
 pub fn default_hash_seeder(base_seed: Option<i64>) -> Seeder {
     let base_seed = base_seed.unwrap_or_else(|| random_torch_i64());
@@ -80,25 +80,27 @@
     {
         Transform::new_func_err(move |circ| self.sample_var(circ.as_discrete_var_unwrap())).rc()
     }
     fn get_sample_expander(
         self,
         var_matcher: IterativeMatcherRc,
         default_fancy_validate: bool,
-        default_assert_any_found: bool,
+        default_assert_found: AssertFound,
+        default_assert_different: bool,
         suffix: Option<String>,
     ) -> Expander
     where
         Self: Sized + Sync + Send + 'static,
     {
         Expander::new(
             vec![(var_matcher, self.get_transform())],
             true,
             default_fancy_validate,
-            default_assert_any_found,
+            default_assert_found,
+            default_assert_different,
             suffix,
         )
     }
 }
 
 #[pyclass(subclass, name = "SampleSpec")]
 #[derive(Clone, Debug)]
@@ -137,26 +139,28 @@
             fn get_sample_shape_py(&self) -> PySymShape {
                 PySymShape(self.get_sample_shape())
             }
             #[pyo3(name = "get_transform")]
             fn get_transform_py(&self) -> TransformRc {
                 self.clone().get_transform()
             }
-            #[pyo3(name = "get_sample_expander", signature=(var_matcher = default_var_matcher(), default_fancy_validate = false, default_assert_any_found = false, suffix = "sample".to_owned()))]
+            #[pyo3(name = "get_sample_expander", signature=(var_matcher = default_var_matcher(), default_fancy_validate = false, default_assert_found = Default::default(), default_assert_different = false, suffix = "sample".to_owned()))]
             fn get_sample_expander_py(
                 &self,
                 var_matcher: IterativeMatcherRc,
                 default_fancy_validate: bool,
-                default_assert_any_found: bool,
+                default_assert_found: AssertFound,
+                default_assert_different: bool,
                 suffix: Option<String>,
             ) -> Expander {
                 self.clone().get_sample_expander(
                     var_matcher,
                     default_fancy_validate,
-                    default_assert_any_found,
+                    default_assert_found,
+                    default_assert_different,
                     suffix,
                 )
             }
         }
 
         impl $type {
             fn into_init(self) -> PyClassInitializer<Self> {
@@ -523,17 +527,21 @@
     fn new(
         sample_spec: SampleSpec,
         var_matcher: IterativeMatcherRc,
         cumulant_matcher: IterativeMatcherRc,
         suffix: Option<String>,
         run_on_sampled: TransformRc,
     ) -> Self {
-        let expander = sample_spec
-            .clone()
-            .get_sample_expander(var_matcher, false, false, suffix);
+        let expander = sample_spec.clone().get_sample_expander(
+            var_matcher,
+            false,
+            Default::default(),
+            false,
+            suffix,
+        );
         Self {
             expander,
             cumulant_matcher,
             sample_spec,
             estimated_cache: FastUnboundedCache::default(),
             run_on_sampled,
         }
@@ -543,15 +551,15 @@
 
     /// recusively estimate all cumulants
     #[pyo3(name = "estimate")]
     fn estimate_py(&mut self, circuit: CircuitRc) -> Result<CircuitRc> {
         self.estimate(circuit)
     }
     pub fn sample(&mut self, circuit: CircuitRc) -> Result<CircuitRc> {
-        let out = self.expander.batch(circuit.clone(), None, None)?;
+        let out = self.expander.batch(circuit.clone(), None, None, None)?;
         let is_orig_shape = out.shape() == circuit.shape();
         let is_sampled_shape = out.shape()
             == &self
                 .sample_spec
                 .get_sample_shape()
                 .iter()
                 .chain(circuit.shape())
```

### Comparing `rust_circuit-0.4.8/local_dependencies/get_update_node/src/transform.rs` & `rust_circuit-0.4.9/local_dependencies/get_update_node/src/transform.rs`

 * *Files 16% similar despite different names*

```diff
@@ -85,20 +85,14 @@
     }
 
     #[staticmethod]
     pub fn ident() -> Self {
         TransformData::Ident.into()
     }
 
-    #[pyo3(signature=(
-        cache_transform = Updater::default().cache_transform,
-        cache_update = Updater::default().cache_update
-    ))]
-    fn updater(&self, cache_transform: bool, cache_update: bool) -> Updater {
+    fn updater(&self) -> Updater {
         Updater {
             transform: self.clone().into(),
-            cache_transform,
-            cache_update,
             ..Default::default()
         }
     }
 }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/rr_util/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 pyo3= { features=["num-bigint", "multiple-pymethods", "anyhow", "macros"], git = "https://github.com/redwoodresearch/pyo3" }
 macro_rules_attribute= "0.1.2"
 thiserror= "1.0.32"
 regex= "1.6.0"
 cached= {version = "0.38.0", default-features = false}
 paste= "1.0.8"
 blake3= "1.3.1"
-smallvec= { version = "1.10.0", features = ["union"] }
+smallvec= { version = "1.10.0", features = ["union", "specialization"] }
 itertools= "0.10.3"
 rustc-hash= "1.1.0"
 once_cell= "1.14.0"
 num-bigint= "0.4.3"
 base16 = "0.2.1"
 threadpool = "1.8.1"
 indexmap= "1.9.2"
 inventory= "0.3.4"
+libc = "0.2.141"
 
 [dependencies.
 uuid]
 version = "1.1.2"
 features = [
     "v4",                # Lets you generate random UUIDs
     "fast-rng",          # Use a faster (but still sufficiently random) RNG
```

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/primes.bin` & `rust_circuit-0.4.9/local_dependencies/rr_util/primes.bin`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/rust_circuit_type_utils.py` & `rust_circuit-0.4.9/local_dependencies/rr_util/rust_circuit_type_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,27 +97,30 @@
     "abs": torch.abs,
     "exp": torch.exp,
     "log": torch.log,
     "logit": torch.logit,
 }
 
 pow = torch.pow
+minimum = torch.minimum
+maximum = torch.maximum
 
 
 def check_canon_idx(i: int, count: int):
     assert count >= 0, count
     if i >= 0:
         assert i < count, (i, count)
     else:
         assert i >= -count, (i, count)
     return i % count
 
 
 def check_ints(x: torch.Tensor):
-    assert (x.long().to(dtype=x.dtype) == x).all()
+    if x.is_floating_point():
+        assert (x.long().to(dtype=x.dtype) == x).all()
 
 
 def gen_index_function(
     x: torch.Tensor, index: torch.Tensor, index_dim: int, batch_x: bool, batch_index: bool, check_index_ints: bool
 ):
     # copy of  WildIndex from computational_node.py
     if check_index_ints:
@@ -207,14 +210,27 @@
         probs.reshape(math.prod(probs.shape[:-1]), probs.shape[-1]),
         num_samples=math.prod(shape),
         replacement=replacement,
         generator=generator,
     ).reshape((*probs.shape[:-1], *shape))
 
 
+def already_sampled_multinomial(
+    weights: torch.Tensor, exponentially_distributed_vals: torch.Tensor, shape: Sequence[int]
+):
+    final_vals = weights / exponentially_distributed_vals
+    return torch.topk(final_vals, k=math.prod(shape), sorted=False, dim=-1).indices.reshape(
+        (*final_vals.shape[:-1], *shape)
+    )
+
+
+def top_k(values: torch.Tensor, shape: Sequence[int]):
+    return torch.topk(values, k=math.prod(shape), sorted=False, dim=-1).indices.reshape((*values.shape[:-1], *shape))
+
+
 # we use different axis layout than pytorch,
 # batch_dims... height_width_ect... channels
 # we also allow asymmetric padding to support InceptionV1
 # which we have to do manually bc torch.conv doesn't support
 def conv(dim, input, filter, stride, padding):
     import einops
```

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/caching.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/caching.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/char_tokenizer.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/char_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/compact_data.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/compact_data.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/conv_shape.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/conv_shape.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/eq_by_big_hash.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/eq_by_big_hash.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/errors_util.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/errors_util.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/lazy.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/lazy.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/lib.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #![feature(let_chains)]
 #![feature(fs_try_exists)]
 #![feature(string_leak)]
 #![feature(if_let_guard)]
 #![feature(iter_intersperse)]
+#![feature(c_unwind)]
 /// reexport
 pub use pyo3;
 pub use uuid;
 
 #[macro_use]
 pub mod caching;
 pub mod eq_by_big_hash;
@@ -24,14 +25,15 @@
 pub mod py_types;
 pub mod python_callables;
 pub mod python_wrapped;
 pub mod rearrange_spec;
 pub mod rrfs;
 pub mod set_cover;
 pub mod shape;
+pub mod signal;
 pub mod tensor_db;
 pub mod tensor_util;
 pub mod union_find;
 pub mod util;
 
 pub type IndexSet<T> =
     indexmap::set::IndexSet<T, core::hash::BuildHasherDefault<rustc_hash::FxHasher>>;
@@ -42,14 +44,16 @@
         smallvec::smallvec!($($tt)*)
     };
 }
 
 use pyo3::{exceptions::PyValueError, types::PyModule, wrap_pyfunction, PyResult};
 
 pub fn register(_py: pyo3::Python<'_>, m: &PyModule) -> PyResult<()> {
+    signal::install_signal_handler();
+
     // we assume throughout the codebase that usize is 8 bytes, and otherwise error here
     if !core::mem::size_of::<usize>() == 8 {
         return PyResult::Err(PyValueError::new_err("Only supports x64"));
     }
     if !cfg!(target_endian = "little") {
         return PyResult::Err(PyValueError::new_err("tried to build non little endian, crate::compact_data::TinyVecU8 relies on little endian"));
     }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/lru_cache.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/lru_cache.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/name.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/name.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/opt_einsum.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/opt_einsum.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/print.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/print.rs`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             string
         );
     }
     string.to_owned()
 }
 
 // TODO: improve color scheme
-const COLOR_CODES: [usize; 14] = [31, 32, 33, 34, 35, 36, 90, 91, 92, 93, 94, 95, 96, 97];
+pub const COLOR_CODES: [usize; 14] = [31, 32, 33, 34, 35, 36, 90, 91, 92, 93, 94, 95, 96, 97];
 static NAME_TO_COLOR: Lazy<HashMap<String, usize>> = Lazy::new(|| {
     HashMap::from_iter(
         [
             ("Red", 0),
             ("Green", 1),
             ("Yellow", 2),
             ("Blue", 3),
@@ -118,42 +118,31 @@
             }
         } else {
             write!(f, "None")
         }
     }
 }
 
-pub fn last_child_arrows(last_child: &Vec<bool>, is_output: bool, arrows: bool) -> String {
+pub fn last_child_arrows(
+    result: &mut String,
+    prefix: &str,
+    is_last_child: bool,
+    arrows: bool,
+) -> String {
+    let mut out = prefix.to_owned();
+    result.push_str(prefix);
     if !arrows {
-        return "  ".repeat(last_child.len());
-    }
-    let depth = last_child.len();
-    let mut result = "".to_owned();
-    for i in 0..depth.saturating_sub(1) {
-        result.push_str(if last_child[i] { " " } else { BAR });
-        result.push(' ');
-    }
-    if depth > 0 {
-        if is_output {
-            result.push_str(if *last_child.last().unwrap() {
-                UP_ELBOW
-            } else {
-                TEE
-            });
-            result.push_str(ARROW);
-        } else {
-            write!(
-                result,
-                "{} ",
-                if !last_child[depth - 1] { BAR } else { " " }
-            )
-            .unwrap();
-        }
-    }
-    result
+        result.push_str("  ");
+        out.push_str("  ");
+        return out;
+    }
+    result.push_str(if is_last_child { UP_ELBOW } else { TEE });
+    result.push_str(ARROW);
+    write!(out, "{} ", if !is_last_child { BAR } else { " " }).unwrap();
+    out
 }
 
 #[macro_export]
 macro_rules! clicolor {
     ($name:ident) => {
         CliColor::from_string(stringify!($name).to_owned()).unwrap()
     };
```

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/py_types.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/py_types.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,22 @@
     pub dtype_convert: HashMap<TorchDtype, PyObject>,
     un_flat_concat: PyObject,
     tensor_scale: PyObject,
     pub generalfunctions: std::collections::HashMap<String, PyObject>,
     pub gen_index_function: PyObject,
     pub explicit_gen_index_function: PyObject,
     pub pow: PyObject,
+    pub minimum: PyObject,
+    pub maximum: PyObject,
     einsum: PyObject,
     make_diagonal: PyObject,
     pub print: PyObject,
     pub random_indices: PyObject,
+    pub already_sampled_multinomial: PyObject,
+    pub top_k: PyObject,
     pub conv: PyObject,
     pub tensor_to_bytes: PyObject,
     pub tensor_from_bytes: PyObject,
     pub assert_tensors_close: PyObject,
     pub builtins: Py<PyModule>,
     pub gc: Py<PyModule>,
     pub optimizing_symbolic_size_warning: PyObject,
@@ -86,18 +90,22 @@
             .getattr("generalfunctions")
             .unwrap()
             .extract()
             .unwrap(),
         gen_index_function: get("gen_index_function"),
         explicit_gen_index_function: get("explicit_gen_index_function"),
         pow: get("pow"),
+        minimum: get("minimum"),
+        maximum: get("maximum"),
         einsum: get("einsum"),
         make_diagonal: get("make_diagonal"),
         print: get_builtin("print"),
         random_indices: get("random_indices"),
+        already_sampled_multinomial: get("already_sampled_multinomial"),
+        top_k: get("top_k"),
         conv: get("conv"),
         tensor_to_bytes: get("tensor_to_bytes"),
         tensor_from_bytes: get("tensor_from_bytes"),
         assert_tensors_close: get("assert_tensors_close"),
         builtins: builtins.into(),
         gc: PyModule::import(py, "gc").unwrap().into(),
         optimizing_symbolic_size_warning: get("OptimizingSymbolicSizeWarning"),
```

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/python_callables.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/python_callables.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/python_wrapped.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/python_wrapped.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/rearrange_spec.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/rearrange_spec.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/repr.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/repr.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/rrfs.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/rrfs.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/set_cover.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/set_cover.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/shape.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/shape.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/tensor_db.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/tensor_db.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/tensor_util.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/tensor_util.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/union_find.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/union_find.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/src/util.rs` & `rust_circuit-0.4.9/local_dependencies/rr_util/src/util.rs`

 * *Files 0% similar despite different names*

```diff
@@ -623,15 +623,15 @@
                 Dyn([< $name DynStruct >]),
                 Py($crate::py_types::PyCallable),
                 $($(
                     $enum_name($type_name),
                 )*)*
             }
             impl $name{
-                fn new_dyn(f:Box<dyn Fn($($ity),*)->anyhow::Result<$retty> + Send + Sync>)->Self{
+                pub fn new_dyn(f:Box<dyn Fn($($ity),*)->anyhow::Result<$retty> + Send + Sync>)->Self{
                     Self::Dyn([< $name DynStruct >] (std::sync::Arc::new(f)))
                 }
             }
 
             $crate::fn_struct!(@mk_call $name $fn_ty($($iname:$ity),*)->$retty; ($($($enum_name,)*)*));
 
             #[pyclass]
@@ -670,15 +670,15 @@
                     write!(f,"dyn_fn_struct")
                 }
             }
         }
     };
     (@mk_call $name:ident Fn($($iname:ident:$ity:ty),*) -> $retty:ty; ($($enum_name:ident,)*)) => {
         impl $name {
-            fn call(&self,$($iname:$ity),*)->anyhow::Result<$retty>{
+            pub fn call(&self,$($iname:$ity),*)->anyhow::Result<$retty>{
                 // nested macro to deal with expansion resolution
                 #[allow(unused_macros)]
                 macro_rules! stuff {
                     ($x:expr) => (
                         $x.call($($iname,)*)
                     )
                 }
@@ -691,15 +691,15 @@
                     )*
                 }
             }
         }
     };
     (@mk_call $name:ident FnMut($($iname:ident:$ity:ty),*) -> $retty:ty; ($($enum_name:ident,)*)) => {
         impl $name {
-            fn call(&mut self,$($iname:$ity),*)->anyhow::Result<$retty>{
+            pub fn call(&mut self,$($iname:$ity),*)->anyhow::Result<$retty>{
                 // nested macro to deal with expansion resolution
                 #[allow(unused_macros)]
                 macro_rules! stuff {
                     ($x:expr) => (
                         $x.call($($iname,)*)
                     )
                 }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/rr_util/tensor_hash.py` & `rust_circuit-0.4.9/local_dependencies/rr_util/tensor_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     return (_gpuhash, _gpuhash_finalize, ctx)
 
 
 dtypes_to_bytes = {
     torch.float32: b"float32",
     torch.float64: b"float64",
     torch.float16: b"float16",
+    torch.bfloat16: b"bfoat16",
     torch.bool: b"bool---",
     torch.int8: b"int8---",
     torch.int16: b"int16--",
     torch.int32: b"int32--",
     torch.int64: b"int64--",
     torch.uint8: b"uint8--",
 }
@@ -140,22 +141,26 @@
         return cached[1]
     # print(f"didn't hit hash cache {id(tensor)=}")
     hash_out = hash_tensor_impl(tensor)
     tensor_hash_cache[id(tensor)] = (weakref.ref(tensor), hash_out)
     return hash_out
 
 
-def hash_tensor_impl(tensor):
+def hash_tensor_impl(tensor: torch.Tensor):
     m = blake3(max_threads=blake3.AUTO)
     m.update(b"c3c5ce3e-7d06-4939-8340-2a7e6b2984b4")
     m.update(int_tuple_to_bytes(tensor.shape, b""))
     m.update(b"fb782993-5fe7-43ac-acc2-d57fb429c2fc")
     m.update(dtypes_to_bytes[tensor.dtype])
     m.update(str(tensor.device).encode("utf-8"))
     m.update(b"9430f5c7-3c58-4339-b863-5449a4d74ee6")
+
+    if tensor.dtype == torch.bfloat16:
+        tensor = tensor.to(dtype=torch.float32)
+
     if str(tensor.device) == "cpu":
         m.update(tensor.detach().numpy().tobytes())  # this copies, could be optimized more
     else:
         if True:
             m.update(tensor.detach().cpu().numpy().tobytes())
         else:
             try:
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pyo3= { features=["num-bigint", "multiple-pymethods", "anyhow", "macros"], git = "https://github.com/redwoodresearch/pyo3" }
 cached= {version = "0.38.0", default-features = false}
 num-bigint= "0.4.3"
 anyhow= { version = "1.0.60", features = ["backtrace"] }
 thiserror= "1.0.32"
 paste= "1.0.8"
 itertools= "0.10.3"
-smallvec= { version = "1.10.0", features = ["union"] }
+smallvec= { version = "1.10.0", features = ["union", "specialization"] }
 macro_rules_attribute= "0.1.2"
 rustc-hash= "1.1.0"
 base16 = "0.2.1"
 regex= "1.6.0"
 miniserde = "0.1"
 tiny_http="0.12.0"
 ureq = {version = "2.6.2", default-features = false }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/algebraic_rewrite.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/algebraic_rewrite.rs`

 * *Files 0% similar despite different names*

```diff
@@ -666,19 +666,21 @@
         .iter()
         .filter(|x| (**x + node.num_non_batchable_output_dims as usize) < node.rank())
         .cloned()
         .collect();
     if removable_batchable_inp.is_empty() {
         return None;
     }
-    let new_generalfunction = GeneralFunction::new(
-        vec![remove_axes(&node.children_sl()[0], &removable_batchable_inp).unwrap()],
-        node.spec.clone(),
-        node.info().name,
-    );
+    let new_generalfunction = node
+        .replace_children(vec![remove_axes(
+            &node.children_sl()[0],
+            &removable_batchable_inp,
+        )
+        .unwrap()])
+        .unwrap();
     Some(Rearrange::nrc_elim_identity(
         new_generalfunction.rc(),
         RearrangeSpec::unremove_axes(&removable_batchable_inp, &node.info().shape),
         None,
     ))
 }
 
@@ -1500,15 +1502,15 @@
                             );
                             on_sub(i, child, index_passed, None)
                         } else {
                             Ok(child)
                         }
                     })
                     .collect::<Result<_>>()?;
-                let new_gf = GeneralFunction::nrc(new_operands, inner.spec.clone(), out_name);
+                let new_gf = inner.evolve(new_operands, out_name).unwrap().rc();
 
                 handle_non_batchable_remaining(rank_to_pass, new_gf).map_err(
                     |(_, top_axis_indices)| {
                         PushDownIndexError::GeneralFunctionSomeAxesNotPossible {
                             index_node: node.clone(),
                             is_batchable: inner.is_batchable(),
                             num_non_batch_out: inner.num_non_batchable_output_dims,
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/batching.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/batching.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/bin/print_simp_fn_stub_part.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/bin/print_simp_fn_stub_part.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/canonicalize.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/canonicalize.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/circuit_evaluate.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/circuit_evaluate.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 use std::iter::zip;
 
 use anyhow::{bail, Result};
-use circuit_base::{generalfunction::SpecTrait, Circuit, CircuitNode, CircuitRc, Module};
+use circuit_base::{
+    generalfunction::{GeneralFunctionSpecFull, SpecTrait},
+    Circuit, CircuitNode, CircuitRc, Module,
+};
 use macro_rules_attribute::apply;
 use pyo3::{exceptions::PyValueError, pyfunction, IntoPy, PyObject, Python};
 use rr_util::{
     py_types::{
         einops_repeat, einsum_py, make_diagonal_py, scalar_to_tensor, scalar_to_tensor_py,
         ExtraPySelfOps, Tensor, PY_UTILS,
     },
@@ -76,23 +79,33 @@
                 .conform_to_input_shape_spec()
                 .to_einops_string_and_letter_sizes();
             einops_repeat(&tensors[0], string, letter_sizes)
         }
         Circuit::Index(i) => {
             let tensors = upcast_tensor_device_dtypes(tensors);
             assert_eq!(tensors.len(), 1);
-            Python::with_gil(|py| {
-                PY_UTILS
-                    .index_apply_dimwise
-                    .call(py, (tensors[0].clone(), i.index.clone()), None)
-                    .map_err(|err| err.into())
-                    .map(|x| x.extract(py).unwrap())
-            })
+            PY_UTILS
+                .index_apply_dimwise
+                .call(py, (tensors[0].clone(), i.index.clone()), None)
+                .map_err(|err| err.into())
+                .map(|x| x.extract(py).unwrap())
         }
-        Circuit::GeneralFunction(g) => g.spec.function(tensors),
+        Circuit::GeneralFunction(g) => match &g.spec {
+            GeneralFunctionSpecFull::MultiOutput(x, n) => {
+                if *n != 0 {
+                    bail!("Internal error: attempt to eval_tensors a multi-output GeneralFunction where output != 0")
+                }
+                let r = x.function(tensors)?;
+                if r.len() != 1 {
+                    bail!("eval_tensors a multi-output GeneralFunction returned multiple outputs but it's expected to only return one (do spec.function(tensors) and spec.get_shape_info(shapes) have the same length?)")
+                }
+                Ok(r[0].clone())
+            }
+            GeneralFunctionSpecFull::SingleOutput(x) => x.function(tensors),
+        },
         Circuit::Concat(c) => {
             let tensors = upcast_tensor_device_dtypes(tensors);
             PY_UTILS
                 .torch
                 .getattr(py, "cat")
                 .unwrap()
                 .call(py, (tensors.to_vec(), c.axis), None)
@@ -153,14 +166,26 @@
                 )?,
             };
             Ok(out)
         }
     })
 }
 
+pub fn eval_tensors_multi_output(x: &CircuitRc, tensors: &[Tensor]) -> Result<Vec<Tensor>> {
+    match &***x {
+        Circuit::GeneralFunction(g) => match &g.spec {
+            GeneralFunctionSpecFull::MultiOutput(x, _) => x.function(tensors),
+            GeneralFunctionSpecFull::SingleOutput(_) => {
+                bail!("Internal error: attempt to eval_tensors_multi_output a single-output GeneralFunction")
+            }
+        },
+        _ => bail!("Internal error: attempt to eval_tensors_multi_output {x}"),
+    }
+}
+
 const INTERNAL_EVAL_ERROR_MESSAGE: &str = "this is likely an internal error (earlier errors should have triggered or an invalid circuit was constructed)";
 
 #[apply(python_error_exception)]
 #[base_error_name(TensorEval)]
 #[base_exception(PyValueError)]
 #[derive(Error, Debug, Clone)]
 pub enum TensorEvalError {
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/circuit_manipulation.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/circuit_manipulation.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/circuit_optimizer.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/circuit_optimizer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     #[pyo3(get, set)]
     /// plausibly this should instead by SimpFnSubset which defaults to compiler subset
     pub simp_fn_subset: SimpFnSubset,
 }
 
 impl Default for OptimizationSettings {
     fn default() -> Self {
-        const NUM_CPUS: Lazy<usize> = Lazy::new(|| {
+        static NUM_CPUS: Lazy<usize> = Lazy::new(|| {
             std::thread::available_parallelism()
                 .map_or(1, |x| x.get() - 2)
                 .max(1)
                 .min(8)
         });
         Self {
             verbose: 0,
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/compiler_heuristics.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/compiler_heuristics.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/compiler_strip.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/compiler_strip.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/concat_rewrite.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/concat_rewrite.rs`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
                                 ),
                                 None,
                             ))
                         }
                     })
                     .collect();
                     cur += span_here;
-                    Some(GeneralFunction::nrc(new_operands, generalfunction.spec.clone(), None))
+                    Some(generalfunction.evolve(new_operands, None).unwrap().crc())
                 })
                 .collect::<Option<Vec<_>>>()?;
             return Some(Concat::new(new_operands, concat.axis, None));
         }
     }
     None
 }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/debugging.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/debugging.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/deep_rewrite.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/deep_rewrite.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/diag_rewrite.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/diag_rewrite.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/generalfunction_rewrite.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/generalfunction_rewrite.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use circuit_base::{
     evaluate,
-    generalfunction::{SpecTrait, OFFICIAL_GENERALFUNCTION_INVERSES},
+    generalfunction::{GeneralFunctionSpecFull, OFFICIAL_GENERALFUNCTION_INVERSES},
     Circuit, CircuitNode, CircuitRc, GeneralFunction, GeneralFunctionSpec, Index, Scalar,
 };
 use pyo3::prelude::*;
 use rr_util::{
     sv,
     tensor_util::{TensorAxisIndex, TensorIndex},
 };
@@ -95,15 +95,15 @@
         });
     }
     None
 }
 
 #[pyfunction]
 pub fn generalfunction_gen_index_const_to_index(node: &GeneralFunction) -> Option<CircuitRc> {
-    if let GeneralFunctionSpec::Index(i) = &node.spec
+    if let GeneralFunctionSpecFull::SingleOutput(GeneralFunctionSpec::Index(i)) = &node.spec
         && let Circuit::Array(a) = &**node.children_sl()[1]
         && !i.batch_index
         && i.batch_x {
         let x = &node.children_sl()[0];
         let idx = if i.index_dim < 0 {
             (i.index_dim % (a.ndim() as i64)) as usize
         } else {
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/lib.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/module_rewrite.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/module_rewrite.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/nb_rewrites.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/nb_rewrites.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/sampling.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/sampling.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/scatter_rewrite.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/scatter_rewrite.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/schedule_send.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/schedule_send.rs`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 };
 use miniserde::{json, Deserialize, Serialize};
 use pyo3::{prelude::*, types::PyByteArray};
 use rr_util::{
     lru_cache::TensorCacheRrfs,
     py_types::{Tensor, PY_UTILS},
     pycall,
-    shape::{shape_into_known, Shape},
+    shape::shape_into_known,
     sv,
     tensor_util::{TorchDevice, TorchDeviceDtype, TorchDtype},
     unwrap,
 };
-use rustc_hash::FxHashMap as HashMap;
 
 use crate::scheduled_execution::{get_children_keys, Instruction, Schedule, ScheduleConstant};
 
 #[pyclass]
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct InstructionToSend {
     variant: String,
-    key: usize,
+    key: Vec<Option<usize>>,
     info: String,
     children: Vec<usize>,
 }
 
 #[pyclass]
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct ScheduleToSend {
@@ -88,61 +87,56 @@
 
 impl ScheduleToSend {
     pub fn load(self, cache: &mut Option<TensorCacheRrfs>) -> Result<Schedule> {
         let mut result = Schedule {
             instructions: vec![],
             constants: Default::default(),
             scalars: Default::default(),
-            output_circuits: Some(
-                self.output_circuits
-                    .iter()
-                    .map(|x| (x.0, Scalar::nrc(0.0, sv![], None)))
-                    .collect(),
-            ),
+            output_circuits: self
+                .output_circuits
+                .iter()
+                .map(|x| (x.0, Scalar::nrc(0.0, sv![], None)))
+                .collect(),
             old_constant_hashes: self
                 .old_constant_hashes
                 .iter()
                 .map(|(b, i)| (b.to_vec().try_into().unwrap(), *i))
                 .collect(),
         };
 
-        let mut shapes: HashMap<usize, Shape> = <HashMap<usize, Shape> as Default>::default();
         result.constants = self
             .constants
             .iter()
             .map(|(k, v)| {
                 let parsed = parse_circuit(v, cache)?;
-                shapes.insert(*k, parsed.info().shape.clone());
                 let irreducible: Option<IrreducibleNode> = (**parsed).clone().into();
                 Ok((*k, ScheduleConstant::Circ(irreducible.unwrap())))
             })
             .collect::<Result<_>>()?;
         result.scalars = self
             .scalars
             .iter()
             .map(|(k, v)| {
                 Ok((*k, {
                     let resulty = parse_circuit(v, cache)?.as_scalar().unwrap().clone();
-                    shapes.insert(*k, resulty.info().shape.clone());
                     resulty
                 }))
             })
             .collect::<Result<_>>()?;
         result.instructions = self
             .instructions
             .iter()
             .map(|ins| {
                 let v: &str = &ins.variant;
                 match v {
-                    "Drop" => Ok(Instruction::Drop(ins.key)),
-                    "Compute" => Ok(Instruction::Compute(ins.key, {
-                        let result = parse_circuit(&ins.info, cache)?;
-                        shapes.insert(ins.key, result.info().shape.clone());
-                        result
-                    })),
+                    "Drop" => Ok(Instruction::Drop(ins.key[0].unwrap())),
+                    "Compute" => Ok(Instruction::Compute(
+                        ins.key.clone().into(),
+                        parse_circuit(&ins.info, cache)?,
+                    )),
                     _ => {
                         panic!()
                     }
                 }
             })
             .collect::<Result<Vec<Instruction>>>()?;
         Ok(result)
@@ -172,21 +166,21 @@
         let out = Self {
             instructions: x
                 .instructions
                 .iter()
                 .map(|i| {
                     let out = match i {
                         Instruction::Compute(key, circ) => InstructionToSend {
-                            key: *key,
+                            key: (*key).to_vec(),
                             variant: "Compute".to_owned(),
                             info: repr_shape_always(circ.clone())?,
                             children: get_children_keys(circ.clone()),
                         },
                         Instruction::Drop(key) => InstructionToSend {
-                            key: *key,
+                            key: vec![Some(*key)],
                             variant: "Drop".to_owned(),
                             info: "".to_owned(),
                             children: vec![],
                         },
                     };
                     Ok(out)
                 })
@@ -195,16 +189,14 @@
                 x.constants
                     .iter()
                     .map(|(h, x)| (h, unwrap!(x, ScheduleConstant::Circ))), /* we checked no raw tensors above */
             )?,
             scalars: map_to_str(&x.scalars)?,
             output_circuits: x
                 .output_circuits
-                .as_ref()
-                .unwrap()
                 .iter()
                 .map(|c| (c.0, shape_into_known(c.1.info().shape.clone())))
                 .collect(),
             old_constant_hashes: x
                 .old_constant_hashes
                 .iter()
                 .map(|(b, i)| (b.to_vec(), *i))
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/scheduled_execution.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/scheduled_execution.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 use std::{
     collections::hash_map::Entry,
     fmt::{self, Display},
-    iter::zip,
 };
 
-use anyhow::{anyhow, bail, Context, Result};
+use anyhow::{bail, Context, Result};
 use circuit_base::{
-    cached_circuit_properties::max_non_leaf_size,
     circuit_utils::toposort_circuit,
-    generalfunction::GeneralFunctionOutputSpec,
+    generalfunction::{GeneralFunctionOutputSpec, GeneralFunctionSpecFull, PyWrapMultiOutput},
     module::{
         any_children_with_symbolic_sizes, any_modules, conform_all_modules, substitute_all_modules,
     },
     prelude::*,
     visit_circuit_non_free, Array, GeneralFunction, GeneralFunctionSpec, IrreducibleNode, Leaf,
     ModuleSpec, Scalar, Symbol,
 };
 use circuit_utils::{biggest_non_leaf, hash_to_node_non_free, is_definitely_view_on_child};
-use itertools::Itertools;
+use itertools::{izip, Itertools};
 use macro_rules_attribute::apply;
 use miniserde::json;
 use num_bigint::BigUint;
 use pyo3::{exceptions::PyValueError, prelude::*, types::PyBytes};
 use rr_util::{
     lru_cache::TensorCacheRrfs,
     print::oom_fmt,
@@ -32,28 +30,29 @@
     shape::Shape,
     sv,
     tensor_util::{TorchDevice, TorchDeviceDtype},
     timed, unwrap,
     util::{arc_ref_clone, hash_to_hex, with_context_failable, HashBytes},
 };
 use rustc_hash::{FxHashMap as HashMap, FxHashSet as HashSet};
+use smallvec::SmallVec;
 use thiserror::Error;
 
 use crate::{
-    circuit_evaluate::eval_tensors,
+    circuit_evaluate::{eval_tensors, eval_tensors_multi_output},
     circuit_optimizer::{OptimizationContext, OptimizationSettings},
     module_rewrite::deep_module_remove_unused_inputs,
     schedule_send::ScheduleToSend,
     scheduling_alg::{Dag, DagSimpSettings},
 };
 
 #[derive(Clone, Debug)]
 pub enum Instruction {
     Drop(usize),
-    Compute(usize, CircuitRc),
+    Compute(SmallVec<[Option<usize>; 1]>, CircuitRc), /* if if 0.len() != 1 then CircuitRc must be a multi-output GeneralFunction */
 }
 
 impl IntoPy<PyObject> for Instruction {
     fn into_py(self, py: Python<'_>) -> PyObject {
         match self {
             Instruction::Drop(hb) => hb.into_py(py),
             Instruction::Compute(key, circ) => (key, circ).into_py(py),
@@ -133,63 +132,58 @@
     #[pyo3(get)]
     pub constants: HashMap<usize, ScheduleConstant>,
     // keep scalar constants seperate so adjust numerical scale can work without losing precision
     // before when these were in tensors, they had to be right dtype and therefore overflowed when
     // adjustment needed
     #[pyo3(get)]
     pub scalars: HashMap<usize, Scalar>,
-    pub output_circuits: Option<Vec<(usize, CircuitRc)>>,
+    pub output_circuits: Vec<(usize, CircuitRc)>,
     pub old_constant_hashes: HashMap<HashBytes, usize>,
 }
 
 #[pymethods]
 impl Schedule {
-    pub fn validate(&self, validate_output: bool) -> Result<()> {
+    pub fn validate(&self) -> Result<()> {
         // NOTE: values can't be computed or dropped multiple times atm.
-        let mut prior_compute_numbers = HashSet::default();
+        let mut prior_compute_numbers: HashSet<usize> = HashSet::default();
         let mut prior_drop_numbers = HashSet::default();
 
         for num in self.scalars.keys() {
             if self.constants.contains_key(num) {
                 bail!("num={num} used for both constants and scalars!");
             }
         }
         for instruction in &self.instructions {
             match instruction {
                 Instruction::Drop(drop) => {
                     if !prior_compute_numbers.contains(drop) {
                         bail!("drop={drop} not previously computed");
                     }
-                    if !prior_drop_numbers.insert(drop) {
+                    if !prior_drop_numbers.insert(*drop) {
                         bail!("drop={drop} was already dropped!");
                     }
                 }
-                Instruction::Compute(key, circuit) => {
-                    if !prior_compute_numbers.insert(key) {
-                        bail!("key={key} was already computed!");
+                Instruction::Compute(keys, circuit) => {
+                    if keys
+                        .iter()
+                        .any(|x| x.is_some() && !prior_compute_numbers.insert(x.unwrap()))
+                    {
+                        bail!("some key was already computed!");
                     }
                     if circuit.is_leaf() {
                         bail!("leaf circuit is being computed circuit={circuit:?}");
                     }
                 }
             }
         }
 
-        if validate_output {
-            let output_ids: HashSet<usize> = self
-                .output_circuits
-                .as_ref()
-                .ok_or(anyhow!("no output!"))?
-                .iter()
-                .map(|x| x.0)
-                .collect();
-            for computed in prior_compute_numbers {
-                if !prior_drop_numbers.contains(computed) && !output_ids.contains(computed) {
-                    bail!("computed={computed} is never dropped (or returned)");
-                }
+        let output_ids: HashSet<usize> = self.output_circuits.iter().map(|x| x.0).collect();
+        for computed in prior_compute_numbers {
+            if !prior_drop_numbers.contains(&computed) && !output_ids.contains(&computed) {
+                bail!("computed={computed} is never dropped (or returned)");
             }
         }
 
         Ok(())
     }
 
     #[pyo3(signature=(map, allow_missing = false))]
@@ -249,16 +243,14 @@
             let v = if settings.adjust_numerical_scale {
                 evaluate_schedule_adjust_numerical_scale(self, settings)
             } else {
                 evaluate_schedule(self)
             }?;
             Ok(self
                 .output_circuits
-                .as_ref()
-                .unwrap()
                 .iter()
                 .map(|(id, _)| v[id].clone())
                 .collect())
         };
         Ok(timed!(eval()?, 10, timed))
     }
 
@@ -304,22 +296,38 @@
         let mut current: HashMap<usize, CircuitRc> = HashMap::default();
         for instruction in self.instructions.clone() {
             match instruction {
                 Instruction::Drop(drop) => {
                     let dropped = current.remove(&drop).unwrap();
                     mem -= dropped.info().naive_mem_use(None);
                 }
-                Instruction::Compute(key, circuit) => {
-                    current.insert(key, circuit.clone());
-                    mem += circuit.info().naive_mem_use(None);
-                    if mem > max_mem {
-                        max_mem = mem.clone();
-                        biggest = current.clone();
+                Instruction::Compute(keys, circuit) => {
+                    if let Circuit::GeneralFunction(gf) = circuit.as_ref() && let Some(ref shapes) = gf.multi_output_shapes {
+                        for (ix, k) in keys
+                            .iter()
+                            .enumerate()
+                            .filter_map(|(ix, x)| Some((ix, x.clone()?)))
+                        {
+                            current.insert(k, circuit.clone());
+                            mem += shapes[ix]
+                                .iter()
+                                .map(|x| BigUint::from(x.unwrap_or(1)))
+                                .product::<BigUint>()
+                                * circuit.info().device_dtype.unwrap_or_defaults().size();
+                        }
+                    } else {
+                        current.insert(keys[0].unwrap(), circuit.clone());
+                        assert!(keys.len() == 1);
+                        mem += circuit.info().naive_mem_use(None);
                     }
                 }
+            };
+            if mem > max_mem {
+                max_mem = mem.clone();
+                biggest = current.clone();
             }
         }
         ScheduleStats {
             max_mem,
             constant_mem: self
                 .constants
                 .values()
@@ -334,15 +342,15 @@
 
     pub fn next_key(&self) -> usize {
         *self
             .constants
             .keys()
             .chain(self.scalars.keys())
             .chain(self.instructions.iter().filter_map(|ins| match ins {
-                Instruction::Compute(k, _c) => Some(k),
+                Instruction::Compute(k, _c) => k.iter().filter_map(|x| x.as_ref()).max(),
                 _ => None,
             }))
             .max()
             .unwrap_or(&0)
             + 1
     }
 
@@ -386,26 +394,23 @@
         write!(
             f,
             "Schedule: instructions\n{}\nTensors: {} Arrays: {} Symbols: {} Scalars: {}",
             self.instructions
                 .iter()
                 .filter_map(|i| {
                     if let Instruction::Compute(k, c) = i {
-                        return Some(
-                            k.to_string()
-                                + " "
-                                + &c.variant_string()
-                                + " "
-                                + &format!("{:?}", c.info().device_dtype.dtype)
-                                + " "
-                                + &c.children()
-                                    .map(|x| get_child_key(x).to_string())
-                                    .collect::<Vec<String>>()
-                                    .join(" "),
-                        );
+                        return Some(format!(
+                            "{k:?} {} {:?} {}",
+                            c.variant_string(),
+                            c.info().device_dtype.dtype,
+                            c.children()
+                                .map(|x| get_child_key(x).to_string())
+                                .collect::<Vec<String>>()
+                                .join(" ")
+                        ));
                     }
                     None
                 })
                 .collect::<Vec<String>>()
                 .join("\n"),
             self.constants
                 .iter()
@@ -438,15 +443,15 @@
     max_mem: BigUint,
     #[pyo3(get)]
     constant_mem: BigUint, // this has already been allocated so it can't be over 2^64
     #[pyo3(get)]
     max_circuit_set: HashSet<CircuitRc>,
 }
 
-static SCHEDULING_ERROR_NOTE: &'static str = "(see circuit_to_schedule docstring for tips)";
+static SCHEDULING_ERROR_NOTE: &str = "(see circuit_to_schedule docstring for tips)";
 
 #[apply(python_error_exception)]
 #[base_error_name(SchedulingOOM)]
 #[base_exception(PyValueError)]
 #[derive(Error, Clone, Debug)]
 pub enum SchedulingOOMError {
     #[error("Schedule doesn't fit into max_memory={max_mem}, {stats} ({e_name}) {SCHEDULING_ERROR_NOTE}", max_mem=oom_fmt(*max_memory))]
@@ -559,34 +564,53 @@
     );
     for s in &schedule.instructions {
         let run = |_py: Python| match s {
             Instruction::Compute(key, circ) => {
                 let child_keys: Vec<usize> = circ.children().map(get_child_key).collect();
                 child_keys.iter().for_each(|child_key| {
                     if !live.contains_key(child_key) {
-                        panic!("FAIL");
+                        panic!("Internal error: bad schedule");
                     }
                 });
                 let tensors: Vec<Tensor> = child_keys
                     .iter()
                     .map(|child_key| live[child_key].clone())
                     .collect();
-                let result_err = eval_tensors(circ, &tensors);
-                if result_err.is_err() {
-                    println!("errored evaluate");
-                    circ.print().unwrap()
+                if key.len() == 1 {
+                    let result_err = eval_tensors(circ, &tensors);
+                    if result_err.is_err() {
+                        println!("errored evaluate");
+                        circ.print().unwrap()
+                    }
+                    let result = result_err.unwrap();
+                    assert!(
+                        result.shape() == circ.shape(),
+                        "circ={:?}, result_shape={:?}",
+                        circ,
+                        result.shape()
+                    );
+                    live.insert(key[0].unwrap(), result);
+                } else {
+                    let rs = eval_tensors_multi_output(circ, &tensors).unwrap();
+                    assert_eq!(rs.len(), key.len());
+                    for (k, r, os) in izip!(
+                        key,
+                        rs,
+                        &**circ
+                            .as_general_function_unwrap()
+                            .multi_output_shapes
+                            .as_ref()
+                            .unwrap()
+                    ) {
+                        assert_eq!(r.shape(), os);
+                        if let Some(k2) = k {
+                            live.insert(*k2, r);
+                        }
+                    }
                 }
-                let result = result_err.unwrap();
-                assert!(
-                    result.shape() == circ.shape(),
-                    "circ={:?}, result_shape={:?}",
-                    circ,
-                    result.shape()
-                );
-                live.insert(*key, result);
             }
             Instruction::Drop(key) => {
                 live.remove(key);
             }
         };
         unsafe { with_gil_pool(run) }
     }
@@ -670,209 +694,294 @@
                     }
                 });
                 let tensors_and_scales: Vec<(Tensor, f64)> = circ
                     .children()
                     .map(|x| live[&get_child_key(x)].clone())
                     .collect();
                 let tensors: Vec<Tensor> = tensors_and_scales.iter().map(|x| x.0.clone()).collect();
-                let result = match &***circ {
-                    Circuit::Einsum(_) => {
-                        let new_scale = tensors_and_scales.iter().map(|x| x.1).product();
-                        clamp(&(eval_tensors(circ, &tensors).unwrap(), new_scale))
-                    }
-                    Circuit::Add(_) | Circuit::Concat(_) => {
-                        let new_ts = uniformize(&tensors_and_scales);
-                        (
-                            eval_tensors(
-                                circ,
-                                &new_ts.iter().map(|x| x.0.clone()).collect::<Vec<_>>(),
+                if key.len() == 1 {
+                    let result = match &***circ {
+                        Circuit::Einsum(_) => {
+                            let new_scale = tensors_and_scales.iter().map(|x| x.1).product();
+                            clamp(&(eval_tensors(circ, &tensors).unwrap(), new_scale))
+                        }
+                        Circuit::Add(_) | Circuit::Concat(_) => {
+                            let new_ts = uniformize(&tensors_and_scales);
+                            (
+                                eval_tensors(
+                                    circ,
+                                    &new_ts.iter().map(|x| x.0.clone()).collect::<Vec<_>>(),
+                                )
+                                .unwrap(),
+                                new_ts[0].1,
                             )
-                            .unwrap(),
-                            new_ts[0].1,
-                        )
-                    }
-                    Circuit::GeneralFunction(_) => {
-                        let new_ts: Vec<(Tensor, f64)> = tensors_and_scales
-                            .iter()
-                            .map(|x| set_scale(x, 1.0))
-                            .collect();
-                        clamp(&(
+                        }
+                        Circuit::GeneralFunction(_) => {
+                            let new_ts: Vec<(Tensor, f64)> = tensors_and_scales
+                                .iter()
+                                .map(|x| set_scale(x, 1.0))
+                                .collect();
+                            clamp(&(
+                                eval_tensors(
+                                    circ,
+                                    &new_ts.iter().map(|x| x.0.clone()).collect::<Vec<_>>(),
+                                )
+                                .unwrap(),
+                                1.0,
+                            ))
+                        }
+                        Circuit::Index(_) | Circuit::Rearrange(_) | Circuit::Scatter(_) => (
                             eval_tensors(
                                 circ,
-                                &new_ts.iter().map(|x| x.0.clone()).collect::<Vec<_>>(),
+                                &tensors_and_scales
+                                    .iter()
+                                    .map(|x| x.0.clone())
+                                    .collect::<Vec<_>>(),
                             )
                             .unwrap(),
-                            1.0,
-                        ))
-                    }
-                    Circuit::Index(_) | Circuit::Rearrange(_) | Circuit::Scatter(_) => (
-                        eval_tensors(
-                            circ,
-                            &tensors_and_scales
-                                .iter()
-                                .map(|x| x.0.clone())
-                                .collect::<Vec<_>>(),
-                        )
-                        .unwrap(),
-                        tensors_and_scales[0].1,
-                    ),
-                    Circuit::Scalar(_) | Circuit::Array(_) | Circuit::Symbol(_) => {
-                        panic!("constant found as schedule instruction, not supposed to happen")
-                    }
-                    Circuit::Tag(_) => tensors_and_scales[0].clone(),
-                    _ => {
-                        unimplemented!()
+                            tensors_and_scales[0].1,
+                        ),
+                        Circuit::Scalar(_) | Circuit::Array(_) | Circuit::Symbol(_) => {
+                            panic!("constant found as schedule instruction, not supposed to happen")
+                        }
+                        Circuit::Tag(_) => tensors_and_scales[0].clone(),
+                        _ => {
+                            unimplemented!()
+                        }
+                    };
+                    assert!(result.0.shape()[..] == circ.info().shape[..]);
+                    live.insert(key[0].unwrap(), result);
+                } else {
+                    let gf = circ.as_general_function_unwrap();
+                    let rs = eval_tensors_multi_output(
+                        circ,
+                        &tensors_and_scales
+                            .iter()
+                            .map(|x| set_scale(x, 1.0).0)
+                            .collect::<Vec<_>>()[..],
+                    )
+                    .unwrap();
+                    assert_eq!(rs.len(), key.len());
+                    for (k, r, os) in izip!(key, rs, &**gf.multi_output_shapes.as_ref().unwrap()) {
+                        assert_eq!(r.shape(), os);
+                        if let Some(k2) = k {
+                            live.insert(*k2, clamp(&(r, 1.0)));
+                        }
                     }
-                };
-                assert!(result.0.shape()[..] == circ.info().shape[..]);
-                live.insert(*key, result);
+                }
             }
             Instruction::Drop(hash) => {
                 live.remove(hash);
             }
         };
         unsafe { with_gil_pool(run) }
     }
     let out = live
         .iter()
         .map(|(k, v)| (*k, set_scale(v, 1.0).0))
         .collect();
     Ok(out)
 }
 
-/// this supports dropping and recomputing. if you have an Evaluate(CircuitRc) of something you already evaluated
-/// it's assumed you dropped this and are recomputing it
+/// this does not support dropping & recomputing, due to treatment of multi-output generalfunctions
 pub fn order_to_schedule(
     order: &Vec<CircuitRc>,
     constants: &Vec<IrreducibleNode>,
     scalars: &Vec<Scalar>,
-    to_keep: &[HashBytes],
-) -> (Schedule, Vec<usize>) {
-    let to_keep_set: HashSet<HashBytes> = to_keep.iter().cloned().collect();
+    output_circuits: &Vec<CircuitRc>,
+) -> Schedule {
+    let to_keep_set: HashSet<HashBytes> = output_circuits.iter().map(|x| x.info().hash).collect();
     let mut circ_to_id: HashMap<HashBytes, usize> = Default::default();
     let constants: HashMap<usize, _> = constants
         .iter()
         .map(|x| {
             circ_to_id.insert(x.info().hash, circ_to_id.len());
             (circ_to_id.len() - 1, x.clone())
         })
         .collect();
-    let mut result: Schedule = Schedule {
-        instructions: vec![],
-        scalars: scalars
-            .iter()
-            .map(|x| {
-                circ_to_id.insert(x.info().hash, circ_to_id.len());
-                (circ_to_id.len() - 1, x.clone())
-            })
-            .collect(),
-        output_circuits: None,
-        old_constant_hashes: constants
-            .iter()
-            .map(|(id, node)| (node.info().hash, *id))
-            .collect(),
-        constants: constants
-            .into_iter()
-            .map(|(h, n)| (h, ScheduleConstant::Circ(n)))
-            .collect(),
-    };
+    let scalars: HashMap<usize, _> = scalars
+        .iter()
+        .map(|x| {
+            circ_to_id.insert(x.info().hash, circ_to_id.len());
+            (circ_to_id.len() - 1, x.clone())
+        })
+        .collect();
+    let mut instructions: Vec<_> = vec![];
+    let mut multi_output_gf_to_id: HashMap<
+        (&PyWrapMultiOutput, &Vec<CircuitRc>),
+        HashMap<usize, usize>,
+    > = HashMap::default();
+    for ex in order.iter() {
+        if let Circuit::GeneralFunction(g) = &***ex && let GeneralFunctionSpecFull::MultiOutput(spec, n) = &g.spec {
+            let next_id = circ_to_id.len();
+            if circ_to_id.contains_key(&ex.info().hash) {continue}
+            let our_id = *circ_to_id.entry(ex.info().hash).or_insert(next_id);
+              multi_output_gf_to_id
+                    .entry((&spec, &g.info().children))
+                    .or_insert_with(HashMap::default).insert(*n, our_id);
+        }
+    }
     let mut seen_dependencies: HashSet<usize> = HashSet::default();
     for ex in order.iter().rev() {
         for child in ex.non_free_children() {
             let next_id = circ_to_id.len();
             let dep = *circ_to_id.entry(child.info().hash).or_insert(next_id);
             if !Leaf::matches(&child)
                 && seen_dependencies.insert(dep)
                 && !to_keep_set.contains(&child.info().hash)
             {
-                result.instructions.push(Instruction::Drop(dep));
+                instructions.push(Instruction::Drop(dep));
             }
         }
         let next_id = circ_to_id.len();
         let our_id = *circ_to_id.entry(ex.info().hash).or_insert(next_id);
-        let node_here_symbol_children = (**ex.map_non_free_children_unwrap(|child| {
+        let node_here_symbol_children = ex.map_non_free_children_unwrap(|child| {
             child_from_key(circ_to_id[&child.info().hash], child).rc()
-        }))
-        .clone()
-        .rc();
-        result
-            .instructions
-            .push(Instruction::Compute(our_id, node_here_symbol_children));
-        // seen_dependencies.remove(&ex.info().hash);
+        });
+        if let Circuit::GeneralFunction(g) = &***ex && let GeneralFunctionSpecFull::MultiOutput(spec, _) = &g.spec {
+            let ids = &multi_output_gf_to_id[&(&**spec, &g.info().children)];
+            if *ids.values().min().unwrap() != our_id {
+                continue
+            }
+            let ids = (0..g.multi_output_shapes.as_ref().unwrap().len()).map(|i| ids.get(&i).cloned()).collect();
+            instructions
+                .push(Instruction::Compute(ids, node_here_symbol_children));
+        } else {
+            instructions
+                .push(Instruction::Compute(sv![Some(our_id)], node_here_symbol_children));
+        }
+    }
+    instructions.reverse();
+    Schedule {
+        instructions,
+        scalars,
+        output_circuits: output_circuits
+            .iter()
+            .map(|x| (circ_to_id[&x.info().hash], x.clone()))
+            .collect(),
+        old_constant_hashes: constants
+            .iter()
+            .map(|(id, node)| (node.info().hash, *id))
+            .collect(),
+        constants: constants
+            .into_iter()
+            .map(|(h, n)| (h, ScheduleConstant::Circ(n)))
+            .collect(),
     }
-    result.instructions.reverse();
-    (result, to_keep.iter().map(|x| circ_to_id[x]).collect())
 }
 
-pub fn circuit_to_dag(circuit: CircuitRc) -> Dag {
+pub fn circuit_to_dag(circuit: CircuitRc) -> (Vec<Option<CircuitRc>>, Dag) {
     let mut result: Dag = Default::default();
+    let mut result_nodes: Vec<Option<CircuitRc>> = vec![];
+    let mut hash_to_node: HashMap<HashBytes, usize> = HashMap::default();
     let mut to_merge_with_child: Vec<u32> = vec![];
     // append the circuit to the dag if it's not already there, and return its index
-    let number_node = |c: CircuitRc, result: &mut Dag, to_merge_with_child: &mut Vec<u32>| -> u32 {
-        if let Some(idx) = result.hash_to_node.get(&c.info().hash) {
+    let mut number_node = |c: CircuitRc, result: &mut Dag| -> u32 {
+        if let Some(idx) = hash_to_node.get(&c.info().hash) {
             return *idx as u32;
         }
         result.node_costs.push(c.info().naive_mem_use_usize(None));
-        result.node_hashes.push(c.info().hash);
-        result
-            .hash_to_node
-            .insert(c.info().hash, result.node_hashes.len() - 1);
+        result_nodes.push(Some(c.clone()));
+        hash_to_node.insert(c.info().hash, result_nodes.len() - 1);
         result.children.push(sv![]);
         result.parents.push(sv![]);
-        let output = (result.node_hashes.len() - 1) as u32;
+        let output = (result_nodes.len() - 1) as u32;
 
         if is_definitely_view_on_child(c) {
             to_merge_with_child.push(output)
         }
         output
     };
+    let mut multi_output_gfs: HashMap<
+        (PyWrapMultiOutput, Vec<CircuitRc>),
+        (HashMap<usize, u32>, Vec<Shape>),
+    > = HashMap::default();
+    fn add_children(
+        my_number: u32,
+        non_free_children: &[CircuitRc],
+        result: &mut Dag,
+        number_node: &mut impl FnMut(CircuitRc, &mut Dag) -> u32,
+    ) {
+        let children_to_consider: Vec<CircuitRc> = non_free_children
+            .iter()
+            .filter(|child| !Leaf::matches(child))
+            .cloned()
+            .collect();
+        result.children[my_number as usize] = children_to_consider
+            .iter()
+            .map(|child| number_node(child.clone(), result))
+            .unique()
+            .collect();
+        for child in children_to_consider {
+            let new_num = number_node(child.clone(), result);
+            if !result.parents[new_num as usize].iter().contains(&my_number) {
+                result.parents[new_num as usize].push(my_number);
+            }
+        }
+    }
     // non free so we avoid recuring into module spec.circuit
     visit_circuit_non_free(
-        circuit,
-        |c: CircuitRc| {
+        circuit.clone(),
+|c: CircuitRc| {
             // Arrays are never added to the dag to begin with because they're always 0 cost
-
             if !c.is_leaf() {
-                let my_number: u32 = number_node(c.clone(), &mut result, &mut to_merge_with_child);
-
-                let children_to_consider: Vec<CircuitRc> = c
-                    .non_free_children()
-                    .filter(|child| !Leaf::matches(child))
-                    .collect();
-                result.children[my_number as usize] = children_to_consider
-                    .iter()
-                    .map(|child| number_node(child.clone(), &mut result, &mut to_merge_with_child))
-                    .unique()
-                    .collect();
-                for child in children_to_consider {
-                    let new_num = number_node(child.clone(), &mut result, &mut to_merge_with_child);
-                    if !result.parents[new_num as usize]
-                        .iter()
-                        .contains(&(my_number as u32))
-                    {
-                        result.parents[new_num as usize].push(my_number as u32);
-                    }
-                }
-            }
-
-            Ok(())
-        },
+                let my_number: u32 = if
+                    let Circuit::GeneralFunction(g) = &**c &&
+                    let GeneralFunctionSpecFull::MultiOutput(spec, out) = &g.spec {
+                    *multi_output_gfs
+                        .entry((*spec.clone(), g.children_sl().to_vec()))
+                        .or_insert_with(|| (HashMap::default(), *g.multi_output_shapes.as_ref().unwrap().clone()))
+                        .0
+                        .entry(*out)
+                        .or_insert_with(|| number_node(c.clone(), &mut result))
+                } else {
+                    number_node(c.clone(), &mut result)
+                };
+                add_children(my_number, c.non_free_children_sl(), &mut result, &mut number_node)
+            }       Ok(()) },
         false,
     )
     .unwrap();
+    if !circuit.is_leaf() {
+        let root_id = number_node(circuit.clone(), &mut result);
+        // add node that uses all outputs of multi-output generalfunctions so that scheduler knows they must be all alive at once
+        for ((spec, children), (m, shapes)) in multi_output_gfs.iter() {
+            let gfs_new =
+                GeneralFunction::new_multi_output(children.clone(), spec.clone(), None).unwrap();
+            let ids = std::iter::zip(0..shapes.len(), gfs_new)
+                .map(|(i, f)| {
+                    m.get(&i).cloned().unwrap_or_else(|| {
+                        let c = f.crc();
+                        let n = number_node(c.clone(), &mut result);
+                        add_children(n, c.non_free_children_sl(), &mut result, &mut number_node);
+                        n
+                    })
+                })
+                .collect();
+            let my_id = result.children.len() as u32;
+            result.node_costs.push(0);
+            result.children.push(ids);
+            result.parents.push(sv![root_id]);
+            result.children[root_id as usize].push(my_id);
+        }
+        // in seperate loop for borrow checker :(
+        for _ in multi_output_gfs {
+            result_nodes.push(None);
+        }
+    }
     result.node_to_orig = (0..result.node_costs.len() as u32)
         .map(|x| (x, sv![x]))
         .collect();
     for tmp in to_merge_with_child {
         assert!(result.children[tmp as usize].len() < 2);
         if result.children[tmp as usize].len() == 1 {
             result.merge_larger(result.children[tmp as usize][0], tmp, false)
         }
     }
-    result
+    (result_nodes, result)
 }
 
 pub fn circuit_to_schedule(
     circuit: CircuitRc,
     context: &mut OptimizationContext,
 ) -> Result<Schedule> {
     // we could avoid this if we wanted, but a bit annoying
@@ -907,25 +1016,27 @@
     }
 
     if let Some((circ, mem)) = biggest_non_leaf(circuit.clone()) && mem > BigUint::from(context.settings.max_single_tensor_memory.min(context.settings.max_memory))
     {
         bail!(SchedulingOOMError::Single {
             max_single_tensor_memory: context.settings.max_single_tensor_memory,
             max_memory: context.settings.max_memory,
-            mem_usage: max_non_leaf_size(circuit.clone()),
+            mem_usage: mem,
             circuit: circ
         });
     }
-    let mut dag = circuit_to_dag(circuit.clone());
+    let (dag_circuits, mut dag) = circuit_to_dag(circuit.clone());
     let order_result = {
-        let mut dag_simp_settings: DagSimpSettings = Default::default();
-        dag_simp_settings.verbose = context.settings.verbose;
-        dag_simp_settings.parallelism = context.settings.optimization_parallelism;
-        dag_simp_settings.exhaustive_give_up_ns = context.settings.scheduling_timeout * 1_000_000;
-        dag_simp_settings.mem_limit = context.settings.max_memory;
+        let dag_simp_settings: DagSimpSettings = DagSimpSettings {
+            verbose: context.settings.verbose,
+            parallelism: context.settings.optimization_parallelism,
+            exhaustive_give_up_ns: context.settings.scheduling_timeout * 1_000_000,
+            mem_limit: context.settings.max_memory,
+            ..Default::default()
+        };
         if context.settings.scheduling_simplify {
             timed!(
                 dag.simplify(&dag_simp_settings)?,
                 10,
                 context.settings.verbose >= 2
             );
         }
@@ -938,45 +1049,44 @@
     let order = with_context_failable(order_result, || {
         Ok(format!("getting schedule failed for circuit:\n{circuit:?}",))
     })?;
 
     let to_node = hash_to_node_non_free(circuit.clone(), false);
     let mut circuit_order: Vec<CircuitRc> = order
         .iter()
-        .map(|x| to_node[&dag.node_hashes[*x as usize]].clone())
+        .filter_map(|x| dag_circuits[*x as usize].clone())
         .collect();
 
     let circuits = if let Circuit::GeneralFunction(g) = &**circuit
-                   && let GeneralFunctionSpec::Output(_) = g.spec {
+                   && let GeneralFunctionSpecFull::SingleOutput(GeneralFunctionSpec::Output(_)) = g.spec {
         circuit_order.pop();
         g.children_sl().to_vec()
     } else {
         vec![circuit.clone()]
     };
-    let (mut out, kept_keys) = order_to_schedule(
+    let out = order_to_schedule(
         &circuit_order,
         &to_node
             .iter()
             .filter_map(|x| Option::<IrreducibleNode>::from(arc_ref_clone(x.1)))
             .collect(),
         &to_node
             .iter()
             .filter_map(|x| x.1.as_scalar().cloned())
             .collect(),
-        &circuits.iter().map(|x| x.info().hash).collect::<Vec<_>>(),
+        &circuits,
     );
-    out.output_circuits = Some(zip(kept_keys, circuits.clone()).collect());
     let out = replace_module_schedules(&out, context)?;
-    out.validate(true)?;
+    out.validate()?;
     let stats = out.get_stats();
     // scheduling simplify & exhaustive currently overestimates mem usage by a lot (todo debug?), so we currently don't error during scheduling & just recheck & error here. also this is nice since it tells user schedule memory usage & takes modules into account!
     if stats.max_mem > context.settings.max_memory.into() {
         bail!(SchedulingOOMError::OverMemoryLimit {
             max_memory: context.settings.max_memory,
-            stats: stats
+            stats
         })
     }
     Ok(out)
 }
 
 pub fn circuit_to_schedule_naive_toposort(circuit: CircuitRc) -> Result<Schedule> {
     let circuit = substitute_all_modules(circuit);
@@ -992,48 +1102,38 @@
             constants.push(constant)
         } else {
             order.push(c)
         }
     }
 
     let circuits = if let Circuit::GeneralFunction(g) = &**circuit
-                   && let GeneralFunctionSpec::Output(_) = g.spec {
+                   && let GeneralFunctionSpecFull::SingleOutput(GeneralFunctionSpec::Output(_)) = g.spec {
         order.pop();
         g.children_sl().to_vec()
     } else {
         vec![circuit]
     };
-    let (mut result, kept_keys) = order_to_schedule(
-        &order,
-        &constants,
-        &scalars,
-        &circuits.iter().map(|x| x.info().hash).collect::<Vec<_>>(),
-    );
-    result.output_circuits = Some(zip(kept_keys, circuits).collect());
-    result.validate(true).expect("should be valid");
+    let result = order_to_schedule(&order, &constants, &scalars, &circuits);
+    result.validate()?;
     Ok(result)
 }
 
 pub fn schedule_out_many(circuits: Vec<CircuitRc>) -> CircuitRc {
-    GeneralFunction::try_new(
-        circuits,
-        GeneralFunctionSpec::Output(GeneralFunctionOutputSpec()),
-        None,
-    )
-    .unwrap()
-    .crc()
+    GeneralFunction::try_new(circuits, GeneralFunctionOutputSpec().into(), None)
+        .unwrap()
+        .crc()
 }
 
 #[pyfunction]
 pub fn scheduled_evaluate(circuit: CircuitRc, settings: OptimizationSettings) -> Result<Tensor> {
     let schedule = if settings.scheduling_naive {
         circuit_to_schedule_naive_toposort(circuit)
     } else {
         circuit_to_schedule(
-            circuit.clone(),
+            circuit,
             &mut OptimizationContext::new_settings(settings.clone()),
         )
     }?;
     schedule.evaluate(settings)
 }
 
 #[pyfunction]
@@ -1107,15 +1207,15 @@
                         .expect("unused args removed at start of circuit_to_schedule!");
 
                     let original_children: Vec<usize> =
                         mn.args().cloned().map(get_child_key).collect();
 
                     let inner_schedule = schedule_module_spec(&mn.spec, context)
                         .with_context(|| format!("while scheduling Module spec {mn:?}"))?;
-                    let mut inner_to_outer_key = HashMap::default();
+                    let mut inner_to_outer_key: HashMap<usize, usize> = HashMap::default();
                     for (inner_k, sc) in &inner_schedule.scalars {
                         let outer = scalar_to_id.get(sc).cloned().unwrap_or_else(|| {
                             let this_key = next_key;
                             scalar_to_id.insert(sc.clone(), this_key);
                             result.scalars.insert(this_key, sc.clone());
                             next_key += 1;
                             this_key
@@ -1158,57 +1258,63 @@
                         "empty_modules removed at start of circuit to schedule"
                     );
 
                     inner_to_outer_key
                         .try_insert(
                             inner_schedule
                                 .output_circuits
-                                .unwrap()
                                 .iter()
                                 .exactly_one()
                                 .unwrap()
                                 .0,
-                            *outermost_k,
+                            outermost_k[0].unwrap(),
                         )
                         .unwrap();
 
                     for inner_ins in &inner_schedule.instructions {
                         match inner_ins {
                             Instruction::Drop(drop) => {
                                 result
                                     .instructions
                                     .push(Instruction::Drop(inner_to_outer_key[drop]));
                             }
-                            Instruction::Compute(inner_k, c) => {
+                            Instruction::Compute(inner_ks, c) => {
                                 assert!(!c.is_module());
                                 let new_c = c
                                     .map_children_unwrap(|child| {
                                         let child_inner_k = get_child_key(child.clone());
                                         let child_outer_k =
                                             inner_to_outer_key.get(&child_inner_k).unwrap();
                                         child_from_key(*child_outer_k, child).rc()
                                     })
                                     .rc();
-                                let key =
-                                    inner_to_outer_key.get(inner_k).cloned().unwrap_or_else(|| {
-                                        let this_key = next_key;
-                                        inner_to_outer_key.insert(*inner_k, this_key);
-                                        next_key += 1;
-                                        this_key
-                                    });
-                                result.instructions.push(Instruction::Compute(key, new_c));
-                                inner_to_outer_key.insert(*inner_k, key);
+                                let keys = inner_ks
+                                    .iter()
+                                    .map(|k_opt| {
+                                        k_opt.map(|k| {
+                                            inner_to_outer_key.get(&k).cloned().unwrap_or_else(
+                                                || {
+                                                    let this_key = next_key;
+                                                    inner_to_outer_key.insert(k, this_key);
+                                                    next_key += 1;
+                                                    this_key
+                                                },
+                                            )
+                                        })
+                                    })
+                                    .collect();
+                                result.instructions.push(Instruction::Compute(keys, new_c));
                             }
                         }
                     }
                 }
                 // Note: if other node types have free we'd have to handle that here!
                 _ => {
                     result.instructions.push(ins.clone());
                 }
             },
         }
     }
-    result.validate(result.output_circuits.is_some())?;
+    result.validate()?;
 
     Ok(result)
 }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/scheduling_alg.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/scheduling_alg.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     },
     time::Instant,
 };
 
 use anyhow::{bail, Result};
 use itertools::Itertools;
 use rand::{rngs::SmallRng, Rng, SeedableRng};
-use rr_util::{print::oom_fmt, python_println, sv, timed, timed_value, util::HashBytes};
+use rr_util::{print::oom_fmt, python_println, sv, timed, timed_value};
 use rustc_hash::{FxHashMap as HashMap, FxHashSet as HashSet};
 use smallvec::SmallVec as Sv;
 
 use crate::scheduled_execution::SchedulingOOMError;
 
 #[derive(Clone, Debug)]
 pub struct DagSimpSettings {
@@ -45,16 +45,14 @@
 // rule: there can be only one edge between each pair of nodes
 #[derive(Default, Clone, Debug)]
 pub struct Dag {
     pub children: Vec<Sv<[u32; 6]>>,
     pub parents: Vec<Sv<[u32; 6]>>,
     pub node_costs: Vec<usize>,
     pub node_to_orig: HashMap<u32, Sv<[u32; 6]>>,
-    pub node_hashes: Vec<HashBytes>,
-    pub hash_to_node: HashMap<HashBytes, usize>,
     pub pre_root_nodes: Vec<u32>,
 }
 impl Dag {
     pub fn get_outputs(&self) -> Vec<usize> {
         let result = rr_util::util::filter_to_idx(self.parents.iter(), |y: &&Sv<_>| y.is_empty());
         result
     }
@@ -744,16 +742,14 @@
                 .map(|x| self.node_costs[*x as usize])
                 .collect(),
             node_to_orig: ordered
                 .iter()
                 .enumerate()
                 .map(|(i, x)| (i as u32, sv![*x]))
                 .collect(),
-            node_hashes: vec![],
-            hash_to_node: Default::default(),
             pre_root_nodes: vec![],
         }
     }
 
     pub fn get_costs_of_order(&self, order: &[u32]) -> Vec<(u32, usize)> {
         let mut children: Vec<i32> = self.children.iter().map(|x| x.len() as i32).collect();
         let mut parents: Vec<i32> = self.parents.iter().map(|x| x.len() as i32).collect();
@@ -952,18 +948,18 @@
             max_cost_so_far: 0,
             dag,
             settings,
             found_anything: false,
             rng: random_seed.map(|rs| SmallRng::seed_from_u64(rs)),
             numiters: 0,
         };
-        entry_point.map(|x| {
+        if let Some(x) = entry_point {
             // ensure x is alive at start, special cased
             result.num_parents[x as usize] += 1;
-        });
+        }
         result.reset();
         result
     }
     fn reset(&mut self) {
         self.parents_left = self.num_parents.clone();
         self.order.clear();
         self.order_nodes.clear();
@@ -995,15 +991,15 @@
             if self.parents_left[child as usize] == 0 {
                 self.options_stack.push(child)
             }
         }
     }
 
     fn choose(&mut self, i: u32) -> bool {
-        let choice = self.options_stack.last()[i as usize] as u32;
+        let choice = self.options_stack.last()[i as usize];
         let cost_before = self.alive_cost;
         let max_cost_so_far_before = self.max_cost_so_far;
 
         self.upd_alive_cost(choice);
 
         if self.alive_cost >= self.best.1 {
             self.alive_cost = cost_before;
@@ -1019,15 +1015,15 @@
         self.options_stack.push_copy_last();
         self.options_stack.last_swap_remove(i as usize);
 
         self.upd_rest(choice);
 
         loop {
             let mut did_anything = false;
-            for ix in (0..self.options_stack.last_len()).into_iter().rev() {
+            for ix in (0..self.options_stack.last_len()).rev() {
                 let x = self.options_stack.last()[ix];
                 let cost: usize = self.dag.children[x as usize]
                     .iter()
                     .map(|&ch| {
                         if self.parents_left[ch as usize] == self.num_parents[ch as usize] {
                             self.dag.node_costs[ch as usize]
                         } else {
@@ -1094,15 +1090,15 @@
             // lower means tried sooner
             self.dag.children[x as usize]
                 .iter()
                 .map(|&child| self.parents_left[child as usize])
                 .max()
                 .unwrap_or(0)
         });
-        return true;
+        true
     }
     #[inline]
     fn pop(&mut self) -> u32 {
         let popped = self.order.pop().unwrap();
         for (x, _) in self.order_nodes.last().iter().rev() {
             for child in &self.dag.children[*x as usize] {
                 self.parents_left[*child as usize] += 1;
@@ -1161,15 +1157,15 @@
             loop {
                 while !self.order.is_empty()
                     && (i >= self.options_stack.last_len() as u32
                         || self.max_cost_so_far >= best_cost)
                 {
                     i = self.pop() + 1;
                 }
-                if self.order.len() == 0 && i != 0 {
+                if self.order.is_empty() && i != 0 {
                     break;
                 }
                 if !self.choose(i) {
                     i += 1;
                 } else {
                     break;
                 }
@@ -1203,25 +1199,25 @@
                     > self.settings.exhaustive_settle_ns as u128)
                 || (start_instant.elapsed().as_nanos()
                     > self.settings.exhaustive_give_up_ns as u128)
                 || (halt_signal
                     .as_ref()
                     .map(|h| h.load(std::sync::atomic::Ordering::Relaxed))
                     .unwrap_or(false))))
-            || self.order.len() == 0
+            || self.order.is_empty()
     }
     fn get_out(self, halt_signal: Option<Arc<AtomicBool>>) -> Result<(Vec<(u32, usize)>, usize)> {
         halt_signal.map(|x| x.swap(true, std::sync::atomic::Ordering::Relaxed));
         if self.found_anything {
             let mut o = self.best.0;
-            self.entry_point.map(|x| {
+            if let Some(x) = self.entry_point {
                 let last = o.last().unwrap();
                 let last_cost = self.dag.node_costs[last.0 as usize];
                 o.push((x, last.1 - last_cost))
-            });
+            }
             o.reverse();
             assert_eq!(o.len(), self.parents_left.len());
             return Ok((o, self.best.1));
         }
         bail!(SchedulingOOMError::ExhaustiveTimeout {
             iters: self.numiters,
             size: self.dag.node_to_orig.len(),
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_rewrites/src/server.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_rewrites/src/server.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_print/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/circuit_print/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_print/parsing.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_print/parsing.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_print/print.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_print/print.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 use std::{
     fmt,
     fmt::{Debug, Write},
     hash::{Hash, Hasher},
-    iter,
     sync::Mutex,
 };
 
 use anyhow::{bail, Context, Error, Result};
 use circuit_base::{
     cached_circuit_properties::max_non_leaf_size,
     circuit_utils::{count_nodes, total_flops},
-    generalfunction::SpecTrait,
     opaque_iterative_matcher::{
         get_opaque_type_matcher, OpaqueIterativeMatcher, OpaqueIterativeMatcherVal,
     },
     prelude::*,
     CircuitType,
 };
 use itertools::Itertools;
 use num_bigint::BigUint;
 use pyo3::{once_cell::GILLazy, prelude::*};
 use rr_util::{
     clicolor, fn_struct,
     name::Name,
-    print::{color, last_child_arrows, oom_fmt, CliColor},
+    print::{color, last_child_arrows, oom_fmt, CliColor, COLOR_CODES},
     py_types::MaybeNotSet,
     python_println,
     tensor_db::write_tensor_to_dir_tree,
     util::{HashBytes, ALPHABET},
 };
 use rustc_hash::{FxHashMap as HashMap, FxHashSet as HashSet};
 
@@ -242,14 +240,223 @@
             }
 
             Some(result)
         } else {
             None
         }
     }
+
+    pub fn repr_build_go(
+        &self,
+        circ: &Circuit,
+        result: &mut String,
+        seen_hashes: &mut HashMap<HashBytes, (String, String)>,
+        runnning_serial_number: &mut usize,
+        runnning_leaf_number: &mut usize,
+        prefix: &str,
+        traversal: Option<OpaqueIterativeMatcherVal>,
+        disallow_name_ident: Option<&HashMap<Name, bool>>,
+        parent_info: Option<(&Circuit, usize)>,
+        mut node_comments: Vec<String>,
+    ) -> Result<()> {
+        let mut used_color = false;
+        if let Some(colorer) = &self.colorer {
+            if let Some(color) = colorer
+                .call(circ.clone().rc())
+                .context("colorer errored in print")?
+                .0
+            {
+                used_color = true;
+                result.push_str(&format!(
+                    "\u{001b}[{}m",
+                    COLOR_CODES[color % COLOR_CODES.len()]
+                ));
+            }
+        }
+
+        let term_on_repeat_or_reference = self.repr_full_line(
+            circ,
+            result,
+            seen_hashes,
+            runnning_serial_number,
+            disallow_name_ident,
+        )?;
+
+        if used_color {
+            result.push_str("\u{001b}[0m");
+        }
+
+        let info_from_parent = parent_info
+            .map(|(parent, child_idx)| {
+                self.get_child_info(
+                    parent,
+                    seen_hashes,
+                    runnning_serial_number,
+                    disallow_name_ident,
+                    child_idx,
+                )
+            })
+            .flatten();
+        if let Some(info) = info_from_parent {
+            result.push_str(&format!(" ! {}", info));
+        }
+
+        let num_children = circ.num_children();
+
+        let new_traversal_per_op = if !term_on_repeat_or_reference {
+            let new_traversal_per_op =
+                op_traversal_per(traversal, circ.crc()).context("traversal failed in printer")?;
+            if new_traversal_per_op.is_none() && circ.num_children() != 0 {
+                // all finished case
+                // traversal can't be used with bijection, so we can add ... without having to parse later
+                result.push_str(" ...");
+            }
+            new_traversal_per_op
+        } else {
+            None
+        };
+
+        let leaf_terming_here = circ.num_children() == 0 || new_traversal_per_op.is_none();
+
+        if self.number_leaves && leaf_terming_here {
+            node_comments.push(color(
+                &format!("{}", *runnning_leaf_number),
+                clicolor!(Magenta),
+            ));
+            *runnning_leaf_number += 1;
+        }
+
+        write_comment(result, node_comments, &self.commenters, circ.crc())?;
+        result.push('\n');
+
+        if term_on_repeat_or_reference || new_traversal_per_op.is_none() {
+            return Ok(());
+        }
+        let new_traversal_per = new_traversal_per_op.unwrap();
+
+        if self.seen_children_same_line && !self.has_child_info(circ) {
+            let child_prints_seen = circ
+                .children()
+                .filter_map(|c| seen_hashes.get(&c.info().hash).as_ref().map(|x| &x.0))
+                .join(HORIZ_BAR);
+            let unseen: Vec<_> = circ
+                .children()
+                .zip(new_traversal_per)
+                .filter(|(c, _t)| !seen_hashes.contains_key(&c.info().hash))
+                .enumerate()
+                .collect();
+            if !child_prints_seen.is_empty() {
+                let _ = last_child_arrows(result, prefix, unseen.len() == 0, self.arrows);
+                result.pop();
+                result.push_str(if self.arrows { HORIZ_BAR } else { UP_ELBOW });
+                write!(result, "{}\n", child_prints_seen).unwrap();
+            }
+            for (i, (child, new_traversal)) in &unseen {
+                let next_prefix = last_child_arrows(
+                    result,
+                    prefix,
+                    (*i == unseen.len() - 1) && child_prints_seen.is_empty(),
+                    self.arrows,
+                );
+                self.repr_build_go(
+                    child,
+                    result,
+                    seen_hashes,
+                    runnning_serial_number,
+                    runnning_leaf_number,
+                    &next_prefix,
+                    new_traversal.clone(),
+                    disallow_name_ident,
+                    None,
+                    vec![],
+                )?;
+            }
+            return Ok(());
+        }
+        if self.only_child_below && circ.num_children() == 1 {
+            write!(result, "{}▼\n{}", prefix, prefix).unwrap();
+            self.repr_build_go(
+                &circ.children().next().unwrap(),
+                result,
+                seen_hashes,
+                runnning_serial_number,
+                runnning_leaf_number,
+                prefix,
+                new_traversal_per[0].clone(),
+                disallow_name_ident,
+                Some((circ, 0)),
+                vec![],
+            )?;
+            return Ok(());
+        }
+        for (i, (child, new_traversal)) in circ.children().zip(new_traversal_per).enumerate() {
+            let next_prefix = last_child_arrows(result, prefix, i == num_children - 1, self.arrows);
+            let child_specific_commenters = if self.comment_arg_names {
+                get_child_comments(circ, i)
+            } else {
+                vec![]
+            };
+            self.repr_build_go(
+                &child,
+                result,
+                seen_hashes,
+                runnning_serial_number,
+                runnning_leaf_number,
+                &next_prefix,
+                new_traversal,
+                disallow_name_ident,
+                Some((circ, i)),
+                child_specific_commenters,
+            )?;
+        }
+        Ok(())
+    }
+
+    pub fn disallow_name_ident(&self, circuits: &[CircuitRc]) -> Option<HashMap<Name, bool>> {
+        if !self.force_use_serial_numbers {
+            let mut multiple_with_name: HashMap<Name, bool> = HashMap::default();
+            let mut seen = HashSet::default();
+
+            fn recurse(
+                circ: CircuitRc,
+                seen: &mut HashSet<HashBytes>,
+                multiple_with_name: &mut HashMap<Name, bool>,
+            ) {
+                if !seen.insert(circ.info().hash) {
+                    return;
+                }
+                if let Some(name) = circ.info().name {
+                    use std::collections::hash_map::Entry::*;
+                    match multiple_with_name.entry(name) {
+                        Occupied(mut entry) => {
+                            entry.insert(true);
+                        }
+                        Vacant(entry) => {
+                            entry.insert(false);
+                        }
+                    }
+                }
+
+                for child in circ.children() {
+                    recurse(child, seen, multiple_with_name)
+                }
+                if let Some(m) = circ.as_module() {
+                    for spec in &m.spec.arg_specs {
+                        recurse(spec.symbol.crc(), seen, multiple_with_name)
+                    }
+                }
+            }
+            for c in circuits {
+                recurse(c.clone(), &mut seen, &mut multiple_with_name)
+            }
+            Some(multiple_with_name)
+        } else {
+            None
+        }
+    }
 }
 
 const DEFAULT_END_DEPTH: usize = 2;
 
 #[derive(Debug, Clone)]
 pub struct TerseBool(pub bool);
 
@@ -624,23 +831,15 @@
                 if self.bijection {
                     scatter.index.repr_bijection(self.tensor_index_literal)?
                 } else {
                     format!("{}", scatter.index)
                 }
             }
             Circuit::Concat(concat) => concat.axis.to_string(),
-            Circuit::GeneralFunction(gf) => {
-                if self.bijection {
-                    gf.spec
-                        .serialize()
-                        .context("failed to get general function spec serialize in print, maybe you want circ.print(rust_circuit.PrintOptions(bijection=False)) ?")?
-                } else {
-                    gf.spec.name().to_owned()
-                }
-            }
+            Circuit::GeneralFunction(gf) => gf.spec.serialize(self.bijection)?,
             Circuit::Symbol(sy) => {
                 if sy.uuid.is_nil() {
                     "".to_owned()
                 } else {
                     format!("{}", &sy.uuid)
                 }
             }
@@ -674,261 +873,27 @@
             _ => "".to_owned(),
         })
     }
     #[pyo3(name = "repr", signature=(*circuits))]
     pub fn repr_circuits(&self, circuits: Vec<CircuitRc>) -> Result<String> {
         let mut seen_hashes = HashMap::default();
 
-        let disallow_name_ident = if !self.force_use_serial_numbers {
-            let mut multiple_with_name: HashMap<Name, bool> = HashMap::default();
-            let mut seen = HashSet::default();
-
-            fn recurse(
-                circ: CircuitRc,
-                seen: &mut HashSet<HashBytes>,
-                multiple_with_name: &mut HashMap<Name, bool>,
-            ) {
-                if !seen.insert(circ.info().hash) {
-                    return;
-                }
-                if let Some(name) = circ.info().name {
-                    use std::collections::hash_map::Entry::*;
-                    match multiple_with_name.entry(name) {
-                        Occupied(mut entry) => {
-                            entry.insert(true);
-                        }
-                        Vacant(entry) => {
-                            entry.insert(false);
-                        }
-                    }
-                }
-
-                for child in circ.children() {
-                    recurse(child, seen, multiple_with_name)
-                }
-                if let Some(m) = circ.as_module() {
-                    for spec in &m.spec.arg_specs {
-                        recurse(spec.symbol.crc(), seen, multiple_with_name)
-                    }
-                }
-            }
-            for c in &circuits {
-                recurse(c.clone(), &mut seen, &mut multiple_with_name)
-            }
-            Some(multiple_with_name)
-        } else {
-            None
-        };
-
-        // ideally this would separate method, but to avoid breaking blame we keep like this
-        fn recurse(
-            circ: &Circuit,
-            depth: usize,
-            is_only_child: bool,
-            result: &mut String,
-            seen_hashes: &mut HashMap<HashBytes, (String, String)>,
-            runnning_serial_number: &mut usize,
-            runnning_leaf_number: &mut usize,
-            selfy: &PrintOptions,
-            is_last_child: &Vec<bool>,
-            traversal: Option<OpaqueIterativeMatcherVal>,
-            disallow_name_ident: Option<&HashMap<Name, bool>>,
-            parent_info: Option<(&Circuit, usize)>,
-            mut node_comments: Vec<String>,
-        ) -> Result<()> {
-            result.push_str(&last_child_arrows(
-                is_last_child,
-                !(is_only_child && selfy.only_child_below),
-                selfy.arrows,
-            ));
-            let mut used_color = false;
-            if let Some(colorer) = &selfy.colorer {
-                let color = colorer
-                    .call(circ.clone().rc())
-                    .context("colorer errored in print")?;
-                if color.is_some() {
-                    used_color = true;
-                    result.push_str(&color.start_str());
-                }
-            }
-
-            let term_on_repeat_or_reference = selfy.repr_full_line(
-                circ,
-                result,
-                seen_hashes,
-                runnning_serial_number,
-                disallow_name_ident,
-            )?;
-
-            if used_color {
-                result.push_str("\u{001b}[0m");
-            }
-
-            let info_from_parent = parent_info.and_then(|(parent, child_idx)| {
-                selfy.get_child_info(
-                    parent,
-                    seen_hashes,
-                    runnning_serial_number,
-                    disallow_name_ident,
-                    child_idx,
-                )
-            });
-            if let Some(info) = info_from_parent {
-                result.push_str(&format!(" ! {}", info));
-            }
-
-            let num_children = circ.num_children();
-
-            let new_traversal_per_op = if !term_on_repeat_or_reference {
-                let new_traversal_per_op = op_traversal_per(traversal, circ.crc())
-                    .context("traversal failed in printer")?;
-                if new_traversal_per_op.is_none() && circ.num_children() != 0 {
-                    // all finished case
-                    // traversal can't be used with bijection, so we can add ... without having to parse later
-                    result.push_str(" ...");
-                }
-                new_traversal_per_op
-            } else {
-                None
-            };
-
-            let leaf_terming_here = circ.num_children() == 0 || new_traversal_per_op.is_none();
-
-            if selfy.number_leaves && leaf_terming_here {
-                node_comments.push(color(
-                    &format!("{}", *runnning_leaf_number),
-                    clicolor!(Magenta),
-                ));
-                *runnning_leaf_number += 1;
-            }
-
-            write_comment(result, node_comments, &selfy.commenters, circ.crc())?;
-            result.push('\n');
-
-            if term_on_repeat_or_reference || new_traversal_per_op.is_none() {
-                return Ok(());
-            }
-            let new_traversal_per = new_traversal_per_op.unwrap();
+        let disallow_name_ident = self.disallow_name_ident(&circuits);
 
-            if selfy.seen_children_same_line && !selfy.has_child_info(circ) {
-                let child_prints_seen = circ
-                    .children()
-                    .filter_map(|c| seen_hashes.get(&c.info().hash).as_ref().map(|x| &x.0))
-                    .join(HORIZ_BAR);
-                let unseen: Vec<_> = circ
-                    .children()
-                    .zip(new_traversal_per)
-                    .filter(|(c, _t)| !seen_hashes.contains_key(&c.info().hash))
-                    .enumerate()
-                    .collect();
-                if !child_prints_seen.is_empty() {
-                    let mut spacing = last_child_arrows(
-                        &is_last_child
-                            .iter()
-                            .copied()
-                            .chain(iter::once(unseen.is_empty()))
-                            .collect(),
-                        true,
-                        selfy.arrows,
-                    );
-                    spacing.pop();
-                    spacing.push_str(if selfy.arrows { HORIZ_BAR } else { UP_ELBOW });
-                    writeln!(result, "{}{}", spacing, child_prints_seen).unwrap();
-                }
-                for (i, (child, new_traversal)) in &unseen {
-                    let new_last_child = is_last_child
-                        .iter()
-                        .copied()
-                        .chain(iter::once(*i == unseen.len() - 1))
-                        .collect();
-                    recurse(
-                        child,
-                        depth + 1,
-                        circ.num_children() == 1,
-                        result,
-                        seen_hashes,
-                        runnning_serial_number,
-                        runnning_leaf_number,
-                        selfy,
-                        &new_last_child,
-                        new_traversal.clone(),
-                        disallow_name_ident,
-                        None,
-                        vec![],
-                    )?;
-                }
-                return Ok(());
-            }
-            if selfy.only_child_below && circ.num_children() == 1 {
-                writeln!(
-                    result,
-                    "{}▼",
-                    last_child_arrows(is_last_child, false, selfy.arrows)
-                )
-                .unwrap();
-                recurse(
-                    &circ.children().next().unwrap(),
-                    depth,
-                    circ.num_children() == 1,
-                    result,
-                    seen_hashes,
-                    runnning_serial_number,
-                    runnning_leaf_number,
-                    selfy,
-                    is_last_child,
-                    new_traversal_per[0].clone(),
-                    disallow_name_ident,
-                    Some((circ, 0)),
-                    vec![],
-                )?;
-                return Ok(());
-            }
-            for (i, (child, new_traversal)) in circ.children().zip(new_traversal_per).enumerate() {
-                let new_last_child = is_last_child
-                    .iter()
-                    .copied()
-                    .chain(iter::once(i == num_children - 1))
-                    .collect();
-                let child_specific_commenters = if selfy.comment_arg_names {
-                    get_child_comments(circ, i)
-                } else {
-                    vec![]
-                };
-                recurse(
-                    &child,
-                    depth + 1,
-                    circ.num_children() == 1,
-                    result,
-                    seen_hashes,
-                    runnning_serial_number,
-                    runnning_leaf_number,
-                    selfy,
-                    &new_last_child,
-                    new_traversal,
-                    disallow_name_ident,
-                    Some((circ, i)),
-                    child_specific_commenters,
-                )?;
-            }
-            Ok(())
-        }
         let mut result = String::new();
         let mut runnning_serial_number = 0;
         let mut runnning_leaf_number = 0;
         for circuit in circuits {
-            recurse(
-                &circuit,
-                0,
-                circuit.num_children() == 1,
+            self.repr_build_go(
+                &**circuit,
                 &mut result,
                 &mut seen_hashes,
                 &mut runnning_serial_number,
                 &mut runnning_leaf_number,
-                self,
-                &vec![],
+                "",
                 self.traversal.clone(),
                 disallow_name_ident.as_ref(),
                 None,
                 vec![],
             )?;
         }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_print/print_html.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_print/print_html.rs`

 * *Files 1% similar despite different names*

```diff
@@ -197,24 +197,21 @@
         }
         Ok(())
     }
     pub fn fill_to_expand_data(
         &self,
         circuits: Vec<CircuitRc>,
         to_expand_string: &mut String, // Nodes you can see the children of
-        seen: &HashSet<HashBytes>,     /* Data of all nodes which you might want to see */
     ) -> Result<()> {
         let mut expanded_nodes: HashSet<HashBytes> = Default::default(); // Nodes that are seen from the beginning
         fn recurse(
             circ: CircuitRc,
             to_expand_string: &mut String, // Nodes you can see the children of
             expanded_nodes: &mut HashSet<HashBytes>,
-            selfy: &PrintHtmlOptions,
             traversal: Option<OpaqueIterativeMatcherVal>,
-            seen: &HashSet<HashBytes>,
         ) -> Result<()> {
             let key = circ.info().hash;
             if !expanded_nodes.insert(key) {
                 return Ok(());
             }
             let new_traversal_per_op = op_traversal_per(traversal, circ.crc())?;
 
@@ -227,29 +224,25 @@
             write!(to_expand_string, "\"{}\",", &circ.hash_base16()).unwrap();
 
             for (child, new_traversal) in circ.children().zip(new_traversal_per) {
                 recurse(
                     child,
                     to_expand_string,
                     expanded_nodes,
-                    selfy,
                     new_traversal.clone(),
-                    seen,
                 )?;
             }
             Ok(())
         }
         for circuit in circuits {
             recurse(
                 circuit,
                 to_expand_string,
                 &mut expanded_nodes,
-                self,
                 self.traversal.clone(),
-                seen,
             )?;
         }
         Ok(())
     }
 
     fn get_print_options(&self) -> PrintOptions {
         PrintOptions {
@@ -404,15 +397,15 @@
         html.push_str("var datatoggle___js___ = {");
         let mut seen: HashSet<HashBytes> = HashSet::default();
         self.fill_overall_data(circuits.clone(), &mut html, &mut seen)?;
         html.push_str("};");
 
         // var toExpandtoggle___js___ = ['1', ...];
         html.push_str("var toExpandtoggle___js___ = [");
-        self.fill_to_expand_data(circuits.clone(), &mut html, &seen)?;
+        self.fill_to_expand_data(circuits.clone(), &mut html)?;
         html.push_str("];");
 
         // var rootstoggle___js___ = ['1', ...];
         html.push_str("var rootstoggle___js___ = [");
         html.push_str(
             &circuits
                 .iter()
```

### Comparing `rust_circuit-0.4.8/local_dependencies/expand_node/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/expand_node/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 rr_util = {path = "../rr_util" }
 
 pyo3= { features=["num-bigint", "multiple-pymethods", "anyhow", "macros"], git = "https://github.com/redwoodresearch/pyo3" }
 
 rustc-hash= "1.1.0"
 
 anyhow= { version = "1.0.60", features = ["backtrace"] }
-smallvec= { version = "1.10.0", features = ["union"] }
+smallvec= { version = "1.10.0", features = ["union", "specialization"] }
 
 macro_rules_attribute= "0.1.2"
 thiserror= "1.0.32"
 blake3= "1.3.1"
 
 itertools= "0.10.3"
 cached= {version = "0.38.0", default-features = false}
```

### Comparing `rust_circuit-0.4.8/local_dependencies/expand_node/lib.rs` & `rust_circuit-0.4.9/local_dependencies/expand_node/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,14 @@
                     .cloned()
                     .chain(node.info().shape.iter().cloned())
                     .collect(),
                 node.info().name,
             )
         }
         Circuit::Concat(node) => {
-            // TODO: error on concat axis having symbolic size? (or maybe concat axis is fine???
             let br = batch_rank;
 
             let inputs = get_expanded_inputs(&vec![true; inputs.len()]).unwrap();
 
             let new_axis = node.axis + br;
             if !zip(node.children(), &inputs).all(|(old, new)| {
                 old.info().shape[node.axis].eq_if_known(new.info().shape[new_axis])
@@ -346,25 +345,21 @@
             // We could optimize out these input expansions in various cases.
             // TODO: we could run into strange issues with general functions and expand.
             // Maybe resolve with an assert...
             // TODO: maybe alow for batching over individual inputs like:
             // (This is a bit annoying in various ways and probably shouldn't be supported).
             // - [b_0, b_1, b_2, (stuff)]
             // - [b_2, (other stuff)]
-            GeneralFunction::try_new(
-                get_expanded_inputs(&node.input_batchability).map_err(|input_i| {
-                    ExpandError::GeneralFunctionTriedToBatchNonBatchableInput {
-                        input_i,
-                        batched_inputs: inputs.clone(),
-                        general_function: node.clone(),
-                    }
-                })?,
-                node.spec.clone(),
-                node.info().name,
-            )?
+            node.replace_children(get_expanded_inputs(&node.input_batchability).map_err(
+                |input_i| ExpandError::GeneralFunctionTriedToBatchNonBatchableInput {
+                    input_i,
+                    batched_inputs: inputs.clone(),
+                    general_function: node.clone(),
+                },
+            )?)?
             .rc()
         }
         Circuit::Einsum(node) => {
             let br = batch_rank;
             let next_axis = node.next_axis();
             assert!(next_axis as usize + br <= u8::MAX as usize);
             let end_axis = next_axis + br as u8;
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/circuit_base/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pyo3= { features=["num-bigint", "multiple-pymethods", "anyhow", "macros"], git = "https://github.com/redwoodresearch/pyo3" }
 cached= {version = "0.38.0", default-features = false}
 num-bigint= "0.4.3"
 anyhow= { version = "1.0.60", features = ["backtrace"] }
 thiserror= "1.0.32"
 paste= "1.0.8"
 itertools= "0.10.3"
-smallvec= { version = "1.10.0", features = ["union"] }
+smallvec= { version = "1.10.0", features = ["union", "specialization"] }
 macro_rules_attribute= "0.1.2"
 rustc-hash= "1.1.0"
 base16 = "0.2.1"
 regex= "1.6.0"
 rand= {version = "0.8.5", features = ["small_rng"]}
 
 rr_util = {path = "../rr_util" }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/auto_name.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/auto_name.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/cached_circuit_properties.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/cached_circuit_properties.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit_info.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit_info.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit_node_private.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit_node_private.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/circuit_utils.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/circuit_utils.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/computational_node.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/computational_node.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/constant.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/constant.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/cumulant.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/cumulant.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/errors.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/errors.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     #[error("Wrong input shapes for GeneralFunction {input_shapes:?} {gf_spec:?} ({e_name})")]
     GeneralFunctionWrongInputShape {
         gf_spec: GeneralFunctionSpec,
         input_shapes: Vec<Shape>,
     },
 
-    #[error("Passed python object isn't instance of GeneralFunctionSpec abstract class, ob={ob} ({e_name})")]
+    #[error("Passed python object isn't instance of GeneralFunctionSpec/MultiOutputGeberalFunctionSpecBase abstract class, ob={ob} ({e_name})")]
     GeneralFunctionPyNotInstance { ob: PyObject },
 
     #[error("Concat requires at least one node ({e_name})")]
     ConcatZeroNodes {},
 
     #[error("Concat nodes have different shapes {shapes:?} ({e_name})")]
     ConcatShapeDifferent { shapes: Vec<Shape> },
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/generalfunction.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/generalfunction.rs`

 * *Files 21% similar despite different names*

```diff
@@ -7,28 +7,30 @@
     exceptions::PyValueError,
     once_cell::{GILLazy, GILLazyPy},
     prelude::{PyAny, *},
     types::PyTuple,
 };
 use regex::Regex;
 use rr_util::{
+    eq_by_big_hash::EqByBigHash,
+    impl_eq_by_big_hash,
     name::Name,
-    py_types::{scalar_to_tensor, PySymShape, Tensor, PY_UTILS, SELF_MODULE},
+    py_types::{PySymShape, Tensor, PY_UTILS, SELF_MODULE},
     pycall, python_error_exception,
     shape::{broadcast_shapes_impl, shape_eq_if_known, shape_join_eq, shape_to_py, Shape, Size},
     simple_from, sv,
     tensor_util::{
         check_canon_idxs, upcast_tensor_device_dtypes, upcast_tensor_devices, MiscInputError,
-        TorchDevice, TorchDeviceDtype, TorchDeviceDtypeOp, TorchDtype,
+        TorchDevice, TorchDeviceDtypeOp, TorchDtype,
     },
 };
 use rustc_hash::FxHashMap as HashMap;
 use smallvec::ToSmallVec;
 use thiserror::Error;
-use uuid::uuid;
+use uuid::{uuid, Uuid};
 
 use crate::{
     auto_name::OperatorPriority,
     circuit_node_auto_impl, circuit_node_extra_impl,
     circuit_node_private::{CircuitNodeComputeInfoImpl, CircuitNodeHashItems},
     new_rc_unwrap,
     prelude::*,
@@ -96,20 +98,19 @@
     BASIC_SPEC_ITEMS
         .iter()
         .cloned()
         .map(|(name, num_non_batchable_output_dims, removed_from_end)| {
             let name = name.into();
             (
                 name,
-                GeneralFunctionSimpleSpec {
+                GeneralFunctionSpec::Simple(GeneralFunctionSimpleSpec {
                     name,
                     num_non_batchable_output_dims,
                     removed_from_end,
-                }
-                .into(),
+                }),
             )
         })
         .collect()
 });
 
 pub const OFFICIAL_GENERALFUNCTION_INVERSES: [(&str, &str); 1] = [("reciprocal", "reciprocal")];
 
@@ -135,15 +136,15 @@
     } // returning None means use normal device_dtype inheritance. if Some, then error if dtypes are incorrect and dtype if correct
     fn should_const_fold(&self) -> bool {
         true
     }
 }
 
 #[pyclass]
-#[derive(Debug, Clone)]
+#[derive(Debug, Clone, Eq, Hash, PartialEq)]
 pub struct GeneralFunctionShapeInfo {
     #[pyo3(set)]
     pub shape: Shape,
     #[pyo3(get, set)]
     pub num_non_batchable_output_dims: u8,
     #[pyo3(get, set)]
     pub input_batchability: Vec<bool>,
@@ -176,35 +177,57 @@
         if shapes.len() != self.input_batchability.len() {
             bail!(GeneralFunctionShapeError::WrongNumShapes {
                 got: shapes.len(),
                 expected: self.input_batchability.len()
             })
         }
 
+        if self.num_non_batchable_output_dims as usize > self.shape.len() {
+            bail!("GeneralFunctionShapeInfo: too many num_non_batchable_output_dims! num_non_batchable_output_dims={:?} shape={:?}", self.num_non_batchable_output_dims, self.shape)
+        }
+
         if self.input_batchability.iter().any(|b| *b) {
             let batch_dims = self.shape.len() - self.num_non_batchable_output_dims as usize;
+
+            for (shape, &is_batch) in shapes.iter().zip(&self.input_batchability) {
+                if is_batch && shape.len() < batch_dims {
+                    bail!(
+                "some batchable shape too short for batch, shape.len()={} batch_dims={batch_dims}",
+                shape.len(),
+            );
+                }
+            }
+
             let mut batch_shape = self.shape[..batch_dims].to_smallvec();
             let batches: Vec<&[Size]> = shapes
                 .iter()
                 .zip(&self.input_batchability)
                 .filter(|(_, b)| **b)
                 .map(|(s, _)| &s[..batch_dims])
                 .collect();
             for x in &batches[..] {
                 batch_shape = shape_join_eq(&batch_shape, x, || {
                     anyhow!(GeneralFunctionShapeError::BatchDimsNotEqual {
-                        batches: batches.iter().cloned().map(|x| x.into()).collect(),
+                        batches: batches.iter().map(|x| (*x).into()).collect(),
                         output_batch: self.shape[..batch_dims].into()
                     })
                 })?
             }
         }
 
         Ok(())
     }
+
+    pub fn batch_dims(&self) -> usize {
+        self.shape.len() - self.num_non_batchable_output_dims as usize
+    }
+
+    pub fn batch_shape(&self) -> &[Size] {
+        &self.shape[..self.batch_dims()]
+    }
 }
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct GeneralFunctionSimpleSpec {
     #[pyo3(get)]
     pub name: Name,
@@ -262,16 +285,15 @@
                 .get_function()
                 .call(
                     py,
                     PyTuple::new(py, tensors.iter().map(|x| x.clone().into_py(py))),
                     None,
                 )
                 .context(format!("evaluate function {}", self.name))?
-                .extract(py)
-                .unwrap())
+                .extract(py)?)
         })
     }
 
     fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
         if shapes.len() != 1 {
             bail!(GeneralFunctionShapeError::WrongNumShapes {
                 got: shapes.len(),
@@ -381,16 +403,15 @@
                                 self.check_index_ints.into_py(py),
                             ])
                             .collect::<Vec<_>>(),
                     ),
                     None,
                 )
                 .context("evaluate gen index")?
-                .extract(py)
-                .unwrap())
+                .extract(py)?)
         })
     }
 
     fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
         let (x_shape, index_shape) = if let [x_shape, index_shape] = shapes {
             (x_shape, index_shape)
         } else {
@@ -581,16 +602,15 @@
                                 self.check_index_ints.into_py(py),
                             ])
                             .collect::<Vec<_>>(),
                     ),
                     None,
                 )
                 .context("evaluate explicit gen index")?
-                .extract(py)
-                .unwrap())
+                .extract(py)?)
         })
     }
 
     fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
         let (x_shape, index_shape) = if let [x_shape, index_shape] = shapes {
             (x_shape, index_shape)
         } else {
@@ -746,18 +766,30 @@
     }
     fn serialize(&self) -> Result<String> {
         Ok(self.name().to_owned())
     }
 }
 
 #[pyclass]
+#[derive(Debug, Clone, Copy)]
+pub enum PairwiseType {
+    Pow,
+    Minimum,
+    Maximum,
+}
+
+#[pyclass]
 #[derive(Debug, Clone)]
-pub struct GeneralFunctionPowSpec {}
+pub struct GeneralFunctionPairwiseSpec {
+    pairwise_type: PairwiseType,
+}
 
-simple_from!(|x: GeneralFunctionPowSpec| -> GeneralFunctionSpec { GeneralFunctionSpec::Pow(x) });
+simple_from!(|x: GeneralFunctionPairwiseSpec| -> GeneralFunctionSpec {
+    GeneralFunctionSpec::Pairwise(x)
+});
 
 /// NOTE: expanding/batching doesn't nicely handle this (in the way it nicely handles add)
 /// More generally, we have poor general func support for expand/batch
 #[pyfunction]
 #[pyo3(signature=(shapes, special_case_ones = true))]
 pub fn get_shape_info_broadcast(
     shapes: Vec<Shape>,
@@ -785,48 +817,59 @@
             .max()
             .unwrap_or(0) as u8,
         input_batchability: shapes.iter().map(|s| s.len() == shape.len()).collect(),
         shape,
     })
 }
 
-impl ToPyObject for GeneralFunctionPowSpec {
+impl ToPyObject for GeneralFunctionPairwiseSpec {
     fn to_object(&self, py: Python<'_>) -> PyObject {
         self.clone().into_py(py)
     }
 }
 
-impl SpecTrait for GeneralFunctionPowSpec {
+impl SpecTrait for GeneralFunctionPairwiseSpec {
     fn compute_hash(&self) -> HashBytes {
         let mut hasher = blake3::Hasher::new();
-        hasher.update(uuid!("315d2847-a56d-49c8-8fef-5bcf710a7bc8").as_bytes()); // uuid for Pow
+        hasher.update(uuid!("6b8f667c-7fa2-40e3-9822-c3b9797549bd").as_bytes()); // uuid for pairwise
+        hasher.update(&[self.pairwise_type as u8]);
         *hasher.finalize().as_bytes()
     }
 
     fn function(&self, tensors: &[Tensor]) -> Result<Tensor> {
         Python::with_gil(|py| {
-            let pow = PY_UTILS
-                .pow
-                .call1(py, (tensors[0].clone(), tensors[1].clone()));
-            Ok(pow.context("evaluate pow")?.extract(py).unwrap())
+            let func = match self.pairwise_type {
+                PairwiseType::Pow => &PY_UTILS.pow,
+                PairwiseType::Minimum => &PY_UTILS.minimum,
+                PairwiseType::Maximum => &PY_UTILS.maximum,
+            };
+            let out = func.call1(py, (tensors[0].clone(), tensors[1].clone()));
+            Ok(out
+                .context(format!("evaluate pairwise type={:?}", self.pairwise_type))?
+                .extract(py)
+                .unwrap())
         })
     }
 
     fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
         if shapes.len() != 2 {
             bail!(GeneralFunctionShapeError::WrongNumShapes {
                 got: shapes.len(),
                 expected: 2
             });
         }
         get_shape_info_broadcast(shapes.to_vec(), true)
     }
 
     fn name(&self) -> &'static str {
-        "pow"
+        match self.pairwise_type {
+            PairwiseType::Pow => "pow",
+            PairwiseType::Minimum => "minimum",
+            PairwiseType::Maximum => "maximum",
+        }
     }
 
     fn is_official(&self) -> bool {
         true
     }
 
     fn serialize(&self) -> Result<String> {
@@ -834,15 +877,47 @@
     }
 }
 
 #[pyfunction]
 pub fn pow(base: CircuitRc, exponent: CircuitRc, name: Option<Name>) -> Result<GeneralFunction> {
     GeneralFunction::try_new(
         vec![base, exponent],
-        GeneralFunctionSpec::Pow(GeneralFunctionPowSpec {}),
+        GeneralFunctionSpec::Pairwise(GeneralFunctionPairwiseSpec {
+            pairwise_type: PairwiseType::Pow,
+        }),
+        name,
+    )
+}
+
+#[pyfunction]
+pub fn minimum(
+    base: CircuitRc,
+    exponent: CircuitRc,
+    name: Option<Name>,
+) -> Result<GeneralFunction> {
+    GeneralFunction::try_new(
+        vec![base, exponent],
+        GeneralFunctionSpec::Pairwise(GeneralFunctionPairwiseSpec {
+            pairwise_type: PairwiseType::Minimum,
+        }),
+        name,
+    )
+}
+
+#[pyfunction]
+pub fn maximum(
+    base: CircuitRc,
+    exponent: CircuitRc,
+    name: Option<Name>,
+) -> Result<GeneralFunction> {
+    GeneralFunction::try_new(
+        vec![base, exponent],
+        GeneralFunctionSpec::Pairwise(GeneralFunctionPairwiseSpec {
+            pairwise_type: PairwiseType::Maximum,
+        }),
         name,
     )
 }
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct GeneralFunctionMultinomialSpec {
@@ -990,33 +1065,282 @@
     seed: CircuitRc,
     shape: Shape,
     replacement: bool,
     name: Option<Name>,
 ) -> Result<GeneralFunction> {
     GeneralFunction::try_new(
         vec![probs, seed],
-        GeneralFunctionSpec::Multinomial(GeneralFunctionMultinomialSpec { replacement, shape }),
+        GeneralFunctionMultinomialSpec { replacement, shape }.into(),
+        name,
+    )
+}
+
+#[pyclass]
+#[derive(Debug, Clone)]
+pub struct GeneralFunctionAlreadySampledMultinomialSpec {
+    shape: Shape,
+}
+
+#[pymethods]
+impl GeneralFunctionAlreadySampledMultinomialSpec {
+    #[getter]
+    #[pyo3(name = "shape")]
+    fn py_shape(&self) -> PySymShape {
+        PySymShape(self.shape.clone())
+    }
+}
+
+simple_from!(
+    |x: GeneralFunctionAlreadySampledMultinomialSpec| -> GeneralFunctionSpec {
+        GeneralFunctionSpec::AlreadySampledMultinomial(x)
+    }
+);
+
+impl ToPyObject for GeneralFunctionAlreadySampledMultinomialSpec {
+    fn to_object(&self, py: Python<'_>) -> PyObject {
+        self.clone().into_py(py)
+    }
+}
+
+fn compute_already_sampled_multinomial(
+    weights: Tensor,
+    exponentially_distributed_vals: Tensor,
+    shape: Shape,
+) -> Result<Tensor, PyErr> {
+    Python::with_gil(|py| {
+        PY_UTILS
+            .already_sampled_multinomial
+            .call(
+                py,
+                (weights, exponentially_distributed_vals, shape.clone()),
+                None,
+            )?
+            .extract::<Tensor>(py)
+    })
+}
+
+impl SpecTrait for GeneralFunctionAlreadySampledMultinomialSpec {
+    fn compute_hash(&self) -> HashBytes {
+        let mut hasher = blake3::Hasher::new();
+        hasher.update(uuid!("f1502696-ea6e-46ab-9f62-c1912684eabe").as_bytes());
+        for l in &self.shape {
+            hasher.update(&l.to_le_bytes());
+        }
+        *hasher.finalize().as_bytes()
+    }
+
+    fn function(&self, tensors: &[Tensor]) -> Result<Tensor> {
+        Ok(compute_already_sampled_multinomial(
+            tensors[0].clone(),
+            tensors[1].clone(),
+            self.shape.clone(),
+        )?)
+    }
+
+    fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
+        if shapes.len() != 2 {
+            bail!(GeneralFunctionShapeError::WrongNumShapes {
+                got: shapes.len(),
+                expected: 2
+            });
+        }
+        let info = get_shape_info_broadcast(shapes.to_vec(), true)
+            .context("probs and exponential vals didn't broadcast")?;
+
+        Ok(GeneralFunctionShapeInfo {
+            shape: info.shape[..info.shape.len() - 1]
+                .iter()
+                .chain(&self.shape)
+                .cloned()
+                .collect(),
+            num_non_batchable_output_dims: self.shape.len() as u8,
+            input_batchability: vec![true, true],
+        })
+    }
+
+    fn name(&self) -> &'static str {
+        "a_samp_multinomial"
+    }
+
+    fn is_official(&self) -> bool {
+        true
+    }
+
+    fn get_device_dtype_override(
+        &self,
+        device_dtypes: &[TorchDeviceDtypeOp],
+    ) -> Result<Option<TorchDeviceDtypeOp>> {
+        let (probs_dd, exponential_dd) = (device_dtypes[0], device_dtypes[1]);
+        if probs_dd
+            .dtype
+            .map(|dtype| !dtype.is_floating_point())
+            .unwrap_or(false)
+        {
+            bail!("probs dtype not floating point");
+        }
+        if exponential_dd
+            .dtype
+            .map(|dtype| !dtype.is_floating_point())
+            .unwrap_or(false)
+        {
+            bail!("exponential dtype not floating point");
+        }
+
+        if let Some(probs_dev) = probs_dd.device {
+            if let Some(exponential_dev) = exponential_dd.device {
+                if probs_dev != exponential_dev {
+                    bail!("probs and exponential dtypes different");
+                }
+            }
+        }
+
+        Ok(Some(TorchDeviceDtypeOp {
+            device: probs_dd.device.or(exponential_dd.device),
+            dtype: Some(TorchDtype::int64),
+        }))
+    }
+
+    fn serialize(&self) -> Result<String> {
+        Ok(format!("a_samp_multinomial_{:?}", self.shape))
+    }
+}
+
+#[pyfunction]
+#[pyo3(signature=(probs, exponentially_distributed_vals, shape,  name = None))]
+pub fn already_sampled_multinomial(
+    probs: CircuitRc,
+    exponentially_distributed_vals: CircuitRc,
+    shape: Shape,
+    name: Option<Name>,
+) -> Result<GeneralFunction> {
+    GeneralFunction::try_new(
+        vec![probs, exponentially_distributed_vals],
+        GeneralFunctionSpec::AlreadySampledMultinomial(
+            GeneralFunctionAlreadySampledMultinomialSpec { shape },
+        ),
+        name,
+    )
+}
+
+#[pyclass]
+#[derive(Debug, Clone)]
+pub struct GeneralFunctionTopKSpec {
+    shape: Shape,
+}
+
+#[pymethods]
+impl GeneralFunctionTopKSpec {
+    #[getter]
+    #[pyo3(name = "shape")]
+    fn py_shape(&self) -> PySymShape {
+        PySymShape(self.shape.clone())
+    }
+}
+
+simple_from!(|x: GeneralFunctionTopKSpec| -> GeneralFunctionSpec { GeneralFunctionSpec::TopK(x) });
+
+impl ToPyObject for GeneralFunctionTopKSpec {
+    fn to_object(&self, py: Python<'_>) -> PyObject {
+        self.clone().into_py(py)
+    }
+}
+
+fn compute_top_k(vals: Tensor, shape: Shape) -> Result<Tensor, PyErr> {
+    Python::with_gil(|py| {
+        PY_UTILS
+            .top_k
+            .call(py, (vals, shape.clone()), None)?
+            .extract::<Tensor>(py)
+    })
+}
+
+impl SpecTrait for GeneralFunctionTopKSpec {
+    fn compute_hash(&self) -> HashBytes {
+        let mut hasher = blake3::Hasher::new();
+        hasher.update(uuid!("b2b7c45b-658a-4df0-9a8a-20650978c94e").as_bytes());
+        for l in &self.shape {
+            hasher.update(&l.to_le_bytes());
+        }
+        *hasher.finalize().as_bytes()
+    }
+
+    fn function(&self, tensors: &[Tensor]) -> Result<Tensor> {
+        Ok(compute_top_k(tensors[0].clone(), self.shape.clone())?)
+    }
+
+    fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
+        if shapes.len() != 1 {
+            bail!(GeneralFunctionShapeError::WrongNumShapes {
+                got: shapes.len(),
+                expected: 1
+            });
+        }
+
+        Ok(GeneralFunctionShapeInfo {
+            shape: shapes[0][..shapes[0].len() - 1]
+                .iter()
+                .chain(&self.shape)
+                .cloned()
+                .collect(),
+            num_non_batchable_output_dims: self.shape.len() as u8,
+            input_batchability: vec![true],
+        })
+    }
+
+    fn name(&self) -> &'static str {
+        "top_k"
+    }
+
+    fn is_official(&self) -> bool {
+        true
+    }
+
+    fn get_device_dtype_override(
+        &self,
+        device_dtypes: &[TorchDeviceDtypeOp],
+    ) -> Result<Option<TorchDeviceDtypeOp>> {
+        Ok(Some(TorchDeviceDtypeOp {
+            device: device_dtypes[0].device,
+            dtype: Some(TorchDtype::int64),
+        }))
+    }
+
+    fn serialize(&self) -> Result<String> {
+        Ok(format!("top_k_{:?}", self.shape))
+    }
+}
+
+#[pyfunction]
+#[pyo3(signature=(values,  shape,  name = None))]
+pub fn top_k(values: CircuitRc, shape: Shape, name: Option<Name>) -> Result<GeneralFunction> {
+    GeneralFunction::try_new(
+        vec![values],
+        GeneralFunctionSpec::TopK(GeneralFunctionTopKSpec { shape }),
         name,
     )
 }
 
 #[pyclass]
 #[derive(Debug, Clone)]
 /// used internally to optimize & evaluate multiple circuits at once
 pub struct GeneralFunctionOutputSpec();
 
+simple_from!(|x: GeneralFunctionOutputSpec| -> GeneralFunctionSpec {
+    GeneralFunctionSpec::Output(x)
+});
+
 impl SpecTrait for GeneralFunctionOutputSpec {
     fn compute_hash(&self) -> HashBytes {
         let mut hasher = blake3::Hasher::new();
         hasher.update(uuid!("b79f926e-431d-47dc-a571-182c01eda8c9").as_bytes());
         *hasher.finalize().as_bytes()
     }
 
     fn function(&self, _tensors: &[Tensor]) -> Result<Tensor> {
-        scalar_to_tensor(0., sv![], TorchDeviceDtype::default())
+        bail!("Shouldn't happen: attempt to evaluate GeneralFunction Output")
     }
 
     fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
         Ok(GeneralFunctionShapeInfo {
             shape: sv![],
             num_non_batchable_output_dims: 0,
             input_batchability: shapes.iter().map(|_| false).collect(),
@@ -1121,54 +1445,68 @@
 }
 
 simple_from!(|x: PyWrap| -> GeneralFunctionSpec { GeneralFunctionSpec::Py(Box::new(x)) });
 
 pub static PY_WRAP_BASE: GILLazyPy<PyObject> =
     GILLazyPy::new_py(|py| SELF_MODULE.getattr(py, "GeneralFunctionSpecBase").unwrap());
 
-impl<'source> pyo3::FromPyObject<'source> for Box<PyWrap> {
-    fn extract(ob: &'source PyAny) -> PyResult<Self> {
-        let ob: PyObject = ob.into();
-        let mut hasher = blake3::Hasher::new();
-        if !Python::with_gil(|py| ob.as_ref(py).is_instance(PY_WRAP_BASE.as_ref(py)))
-            .context("is instance failed???")?
-        {
-            let err: anyhow::Error = ConstructError::GeneralFunctionPyNotInstance { ob }.into();
-            return Err(err.into());
-        }
-
-        let name: String =
-            Python::with_gil(|py| -> Result<_> { Ok(ob.getattr(py, "name")?.extract(py)?) })?;
-
-        if name.contains(" at ") {
-            return Err(anyhow!("Function names can't contain the substring ` at ` because it could interfere with parsing.").into());
-        }
-
-        let path: Option<String> =
-            Python::with_gil(|py| -> Result<_> { Ok(ob.getattr(py, "path")?.extract(py)?) })?;
+fn extract_py_generalfunction<'source>(
+    base: &PyObject,
+    base_uuid: Uuid,
+    ob: &'source PyAny,
+) -> PyResult<(Name, Option<String>, PyObject, HashBytes)> {
+    let ob: PyObject = ob.into();
+    let mut hasher = blake3::Hasher::new();
+    if !Python::with_gil(|py| ob.as_ref(py).is_instance(base.as_ref(py)))
+        .context("calling isinstance failed")?
+    {
+        let err: anyhow::Error = ConstructError::GeneralFunctionPyNotInstance { ob }.into();
+        return Err(err.into());
+    }
+
+    let name: String =
+        Python::with_gil(|py| -> Result<_> { Ok(ob.getattr(py, "name")?.extract(py)?) })?;
+
+    if name.contains(" at ") {
+        return Err(anyhow!("Function names can't contain the substring ` at ` because it could interfere with parsing.").into());
+    }
+
+    let path: Option<String> =
+        Python::with_gil(|py| -> Result<_> { Ok(ob.getattr(py, "path")?.extract(py)?) })?;
+
+    if let Some(p) = &path {
+        PyClassLocator::parse(p)?;
+    }
+
+    hasher.update(base_uuid.as_bytes());
+    hasher.update(name.as_bytes());
+    hasher.update(uuid!("dd4e76ed-2d6f-4a11-b5e6-5e32399dbe90").as_bytes());
+    hasher.update(path.as_ref().map_or(&[], |p| p.as_bytes()));
+    hasher.update(uuid!("a9737433-7947-46d7-a509-062e99daaebe").as_bytes());
+    let bytes: Vec<u8> = Python::with_gil(|py| -> Result<_> {
+        Ok(ob.call_method0(py, "compute_hash_bytes")?.extract(py)?)
+    })?;
+    hasher.update(&bytes);
 
-        if let Some(p) = &path {
-            PyClassLocator::parse(p)?;
-        }
+    Ok((name.into(), path, ob, *hasher.finalize().as_bytes()))
+}
 
-        hasher.update(uuid!("de3124ee-154c-4da8-bdb3-b7496ae6223c").as_bytes()); // uuid for PyWrap
-        hasher.update(name.as_bytes());
-        hasher.update(uuid!("dd4e76ed-2d6f-4a11-b5e6-5e32399dbe90").as_bytes());
-        hasher.update(path.as_ref().map_or(&[], |p| p.as_bytes()));
-        hasher.update(uuid!("a9737433-7947-46d7-a509-062e99daaebe").as_bytes());
-        let bytes: Vec<u8> = Python::with_gil(|py| -> Result<_> {
-            Ok(ob.call_method0(py, "compute_hash_bytes")?.extract(py)?)
-        })?;
-        hasher.update(&bytes);
+impl<'source> pyo3::FromPyObject<'source> for Box<PyWrap> {
+    fn extract(ob: &'source PyAny) -> PyResult<Self> {
+        let (name, path, ob, hash) = extract_py_generalfunction(
+            &*PY_WRAP_BASE,
+            uuid!("de3124ee-154c-4da8-bdb3-b7496ae6223c"),
+            ob,
+        )?;
 
         Ok(Box::new(PyWrap {
-            name: name.into(),
+            name,
             path,
             ob,
-            hash: *hasher.finalize().as_bytes(),
+            hash,
         }))
     }
 }
 
 impl ToPyObject for Box<PyWrap> {
     fn to_object(&self, _py: Python<'_>) -> PyObject {
         self.ob.clone()
@@ -1177,62 +1515,213 @@
 
 impl SpecTrait for Box<PyWrap> {
     fn compute_hash(&self) -> HashBytes {
         self.hash
     }
 
     fn function(&self, tensors: &[Tensor]) -> Result<Tensor> {
-        let result: Tensor = Python::with_gil(|py| {
-            Ok::<rr_util::py_types::Tensor, anyhow::Error>(
-                self.ob
-                    .call_method1(
-                        py,
-                        "function",
-                        PyTuple::new(py, tensors.iter().map(|x| x.clone().into_py(py))),
-                    )?
-                    .extract(py)?,
-            )
-        })?;
-        Ok(result)
+        Python::with_gil(|py| {
+            Ok(self
+                .ob
+                .call_method1(
+                    py,
+                    "function",
+                    PyTuple::new(py, tensors.iter().map(|x| x.clone().into_py(py))),
+                )?
+                .extract(py)?)
+        })
     }
 
     fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
         Python::with_gil(|py| {
             Ok(self
                 .ob
                 .call_method1(
                     py,
                     "get_shape_info",
                     PyTuple::new(py, shapes.iter().map(|x| shape_to_py(x))),
                 )?
                 .extract(py)?)
         })
     }
+
     fn get_device_dtype_override(
         &self,
         device_dtypes: &[TorchDeviceDtypeOp],
     ) -> Result<Option<TorchDeviceDtypeOp>> {
         Python::with_gil(|py| {
+            let x = self.ob.call_method1(
+                py,
+                "get_device_dtype_override",
+                PyTuple::new(
+                    py,
+                    device_dtypes
+                        .iter()
+                        .map(|x| x.into_py(py))
+                        .collect::<Vec<_>>(),
+                ),
+            )?;
+            Ok(x.extract::<Option<TorchDeviceDtypeOp>>(py)?)
+        })
+    }
+    fn name(&self) -> &'static str {
+        self.name.into()
+    }
+    fn serialize(&self) -> Result<String> {
+        match &self.path {
+            Some(p) => Ok(format!("{} at {}", &self.name, p)),
+            None => bail!(anyhow!(format!(
+                "Can't serialize function {}: no path given, override GeneralFunctionSpecBase.path to specify path",
+                &self.name
+            ))),
+        }
+    }
+}
+
+#[derive(Clone)]
+pub struct PyWrapMultiOutput {
+    ob: PyObject,
+    hash: HashBytes,
+    name: Name,
+    path: Option<String>,
+}
+
+impl_eq_by_big_hash!(PyWrapMultiOutput);
+
+impl EqByBigHash for PyWrapMultiOutput {
+    fn hash(&self) -> [u8; 32] {
+        self.hash
+    }
+}
+
+impl fmt::Debug for PyWrapMultiOutput {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+        f.debug_struct("PyWrapMultiOutput")
+            .field("ob", &self.ob)
+            .field("name", &self.name)
+            .field("path", &self.path)
+            .finish_non_exhaustive()
+    }
+}
+
+pub static PY_WRAP_MULTI_OUTPUT_BASE: GILLazyPy<PyObject> = GILLazyPy::new_py(|py| {
+    SELF_MODULE
+        .getattr(py, "MultiOutputGeneralFunctionSpecBase")
+        .unwrap()
+});
+
+impl<'source> pyo3::FromPyObject<'source> for PyWrapMultiOutput {
+    fn extract(ob: &'source PyAny) -> PyResult<Self> {
+        let (name, path, ob, hash) = extract_py_generalfunction(
+            &*PY_WRAP_MULTI_OUTPUT_BASE,
+            uuid!("cbb32067-ca14-4e6e-a938-212dc2f3eced"),
+            ob,
+        )?;
+
+        Ok(PyWrapMultiOutput {
+            name,
+            path,
+            ob,
+            hash,
+        })
+    }
+}
+
+impl ToPyObject for Box<PyWrapMultiOutput> {
+    fn to_object(&self, _py: Python<'_>) -> PyObject {
+        self.ob.clone()
+    }
+}
+
+impl PyWrapMultiOutput {
+    fn compute_hash(&self) -> HashBytes {
+        self.hash
+    }
+
+    pub fn function(&self, tensors: &[Tensor]) -> Result<Vec<Tensor>> {
+        Python::with_gil(|py| {
             Ok(self
                 .ob
                 .call_method1(
                     py,
-                    "get_device_dtype_override",
-                    PyTuple::new(
-                        py,
-                        device_dtypes
-                            .iter()
-                            .map(|x| x.into_py(py))
-                            .collect::<Vec<_>>(),
-                    ),
+                    "function",
+                    PyTuple::new(py, tensors.iter().map(|x| x.clone().into_py(py))),
                 )?
                 .extract(py)?)
         })
     }
-    fn name(&self) -> &'static str {
+
+    pub fn get_shape_info(&self, shapes: &[Shape]) -> Result<Vec<GeneralFunctionShapeInfo>> {
+        let si: Vec<GeneralFunctionShapeInfo> = Python::with_gil(|py| -> Result<_> {
+            Ok(self
+                .ob
+                .call_method1(
+                    py,
+                    "get_shape_info",
+                    PyTuple::new(py, shapes.iter().map(|x| shape_to_py(x))),
+                )?
+                .extract(py)?)
+        })?;
+
+        si.iter().try_for_each(|x| x.validate(&shapes).with_context(|| {
+            format!(
+                "invalid shape info in new with spec={:?} input_shapes={:?} (likely input shape error)",
+                self,
+                shapes,
+            )
+        }))?;
+
+        let input_batchability = si[0].input_batchability.clone();
+        for s in si.iter().skip(1) {
+            if s.input_batchability != input_batchability {
+                bail!("multi-output generalfunction: input_batchability must be the same across outputs")
+            }
+        }
+        if input_batchability.iter().any(|x| *x) {
+            let batch_shape = si[0].batch_shape();
+            for s in si.iter().skip(1) {
+                if s.batch_shape() != batch_shape {
+                    bail!(
+                        "multi-output generalfunction: shape[:-num_non_batchable_output_dims] must be the same across outputs"
+                    )
+                }
+            }
+        }
+
+        Ok(si)
+    }
+
+    fn get_device_dtype_override(
+        &self,
+        device_dtypes: &[TorchDeviceDtypeOp],
+    ) -> Result<Option<Vec<Option<TorchDeviceDtypeOp>>>> {
+        Python::with_gil(|py| {
+            let x = self.ob.call_method1(
+                py,
+                "get_device_dtype_override",
+                PyTuple::new(
+                    py,
+                    device_dtypes
+                        .iter()
+                        .map(|x| x.into_py(py))
+                        .collect::<Vec<_>>(),
+                ),
+            )?;
+            if x.is_none(py) {
+                Ok(None)
+            } else if let Ok(x) = x.extract::<Vec<Option<TorchDeviceDtypeOp>>>(py) {
+                Ok(Some(x))
+            } else if let Ok(x) = x.extract::<Option<TorchDeviceDtypeOp>>(py) {
+                Ok(Some(vec![x]))
+            } else {
+                bail!("python GeneralFunction {} get_device_dtype_override must return None, a TorchDeviceDtypeOp, or a list of TorchDeviceDtypeOp but returned {x}", self.name)
+            }
+        })
+    }
+    pub fn name(&self) -> &'static str {
         self.name.into()
     }
     fn serialize(&self) -> Result<String> {
         match &self.path {
             Some(p) => Ok(format!("{} at {}", &self.name, p)),
             None => bail!(anyhow!(format!(
                 "Can't serialize function {}: no path given, override GeneralFunctionSpecBase.path to specify path",
@@ -1244,36 +1733,106 @@
 
 #[derive(Debug, Clone, FromPyObject)]
 pub enum GeneralFunctionSpec {
     Simple(GeneralFunctionSimpleSpec),
     Index(GeneralFunctionIndexSpec),
     ExplicitIndex(GeneralFunctionExplicitIndexSpec),
     SetDD(GeneralFunctionSetDDSpec),
-    Pow(GeneralFunctionPowSpec),
+    Pairwise(GeneralFunctionPairwiseSpec),
     Multinomial(GeneralFunctionMultinomialSpec),
+    AlreadySampledMultinomial(GeneralFunctionAlreadySampledMultinomialSpec),
+    TopK(GeneralFunctionTopKSpec),
     Output(GeneralFunctionOutputSpec),
     Py(Box<PyWrap>), // boxed bc it was long pole for Circuit size
 }
 
+simple_from!(|x: GeneralFunctionSpec| -> GeneralFunctionSpecFull {
+    GeneralFunctionSpecFull::SingleOutput(x)
+});
+
+#[derive(Debug, Clone)]
+pub enum GeneralFunctionSpecFull {
+    SingleOutput(GeneralFunctionSpec),
+    MultiOutput(Box<PyWrapMultiOutput>, usize),
+}
+
+impl IntoPy<PyObject> for GeneralFunctionSpecFull {
+    fn into_py(self, py: Python) -> PyObject {
+        match self {
+            Self::SingleOutput(x) => x.into_py(py),
+            Self::MultiOutput(x, _) => x.ob,
+        }
+    }
+}
+
+impl GeneralFunctionSpecFull {
+    pub fn name(&self) -> &'static str {
+        match self {
+            Self::SingleOutput(x) => x.name(),
+            Self::MultiOutput(x, _) => x.name(),
+        }
+    }
+    pub fn is_official(&self) -> bool {
+        match self {
+            Self::SingleOutput(x) => x.is_official(),
+            Self::MultiOutput(..) => false,
+        }
+    }
+    pub fn should_const_fold(&self) -> bool {
+        match self {
+            Self::SingleOutput(x) => x.should_const_fold(),
+            Self::MultiOutput(..) => true,
+        }
+    }
+    pub fn serialize(&self, bijection: bool) -> Result<String> {
+        match self {
+            Self::SingleOutput(x) => Ok(if bijection {
+                x.serialize()?
+            } else {
+                x.name().to_owned()
+            }),
+            Self::MultiOutput(x, n) => Ok(format!(
+                "output:{} {}",
+                n,
+                if bijection {
+                    x.serialize()?
+                } else {
+                    x.name().to_owned()
+                }
+            )),
+        }
+    }
+}
+
 impl GeneralFunctionSpec {
     #[inline]
     fn as_trait_obj(&self) -> &dyn SpecTrait {
         match self {
             Self::Simple(x) => x,
             Self::Index(x) => x,
             Self::ExplicitIndex(x) => x,
             Self::SetDD(x) => x,
-            Self::Pow(x) => x,
+            Self::Pairwise(x) => x,
             Self::Multinomial(x) => x,
+            Self::AlreadySampledMultinomial(x) => x,
+            Self::TopK(x) => x,
             Self::Output(x) => x,
             Self::Py(x) => x,
         }
     }
 }
 
+impl EqByBigHash for GeneralFunctionSpec {
+    fn hash(&self) -> HashBytes {
+        self.as_trait_obj().compute_hash()
+    }
+}
+
+impl_eq_by_big_hash!(GeneralFunctionSpec);
+
 impl ToPyObject for GeneralFunctionSpec {
     fn to_object(&self, py: Python<'_>) -> PyObject {
         self.as_trait_obj().to_object(py)
     }
 }
 impl IntoPy<PyObject> for GeneralFunctionSpec {
     fn into_py(self, py: Python<'_>) -> PyObject {
@@ -1285,15 +1844,25 @@
     fn compute_hash(&self) -> HashBytes {
         self.as_trait_obj().compute_hash()
     }
     fn function(&self, tensors: &[Tensor]) -> Result<Tensor> {
         self.as_trait_obj().function(tensors)
     }
     fn get_shape_info(&self, shapes: &[Shape]) -> Result<GeneralFunctionShapeInfo> {
-        self.as_trait_obj().get_shape_info(shapes)
+        let si = self.as_trait_obj().get_shape_info(shapes)?;
+
+        si.validate(&shapes).with_context(|| {
+            format!(
+                "invalid shape info in new with spec={:?} input_shapes={:?} (likely input shape error)",
+                self,
+                shapes
+            )
+        })?;
+
+        Ok(si)
     }
     fn get_device_dtype_override(
         &self,
         device_dtypes: &[TorchDeviceDtypeOp],
     ) -> Result<Option<TorchDeviceDtypeOp>> {
         self.as_trait_obj().get_device_dtype_override(device_dtypes)
     }
@@ -1313,19 +1882,20 @@
     }
 }
 
 #[pyclass(extends=PyCircuitBase)]
 #[derive(Clone)]
 pub struct GeneralFunction {
     #[pyo3(get)]
-    pub spec: GeneralFunctionSpec,
+    pub spec: GeneralFunctionSpecFull,
     info: CachedCircuitInfo,
     #[pyo3(get)]
     pub num_non_batchable_output_dims: u8,
     pub input_batchability: Vec<bool>,
+    pub multi_output_shapes: Option<Box<Vec<Shape>>>,
 }
 
 impl GeneralFunction {
     #[apply(new_rc_unwrap)]
     pub fn try_new(
         nodes: Vec<CircuitRc>,
         spec: GeneralFunctionSpec,
@@ -1343,70 +1913,142 @@
                 nodes
                     .iter()
                     .map(|x| x.shape().clone())
                     .collect::<Vec<Shape>>()
             )
         })?;
 
-        si.validate(&shapes).with_context(|| {
+        let ddto = spec.get_device_dtype_override(
+            &nodes
+                .iter()
+                .map(|x| x.info().device_dtype)
+                .collect::<Vec<_>>(),
+        )?;
+
+        Self::new_(nodes, spec.into(), name, si, ddto, None)
+    }
+
+    pub fn new_multi_output(
+        nodes: Vec<CircuitRc>,
+        spec: PyWrapMultiOutput,
+        name: Option<Name>,
+    ) -> Result<Vec<Self>> {
+        let shapes = nodes
+            .iter()
+            .map(|x| x.shape().clone())
+            .collect::<Vec<Shape>>();
+
+        let si = spec.get_shape_info(&shapes[..]).with_context(|| {
             format!(
-                "invalid shape info in new with spec={:?} input_shapes={:?} (likely input shape error)",
+                "failed to compute shape info in new with spec={:?} input_shapes={:?}",
                 spec,
                 nodes
                     .iter()
                     .map(|x| x.shape().clone())
                     .collect::<Vec<Shape>>()
             )
         })?;
 
-        let GeneralFunctionShapeInfo {
-            shape,
-            num_non_batchable_output_dims,
-            input_batchability,
-        } = si;
-
-        let ddto = spec.get_device_dtype_override(
+        let ddtos = spec.get_device_dtype_override(
             &nodes
                 .iter()
                 .map(|x| x.info().device_dtype)
                 .collect::<Vec<_>>(),
         )?;
 
+        let multi_output_shapes = Some(Box::new(si.iter().map(|x| x.shape.clone()).collect()));
+
+        if ddtos.is_some() && ddtos.as_ref().unwrap().len() != si.len() {
+            bail!("multi-output generalfunction: device_dtype_override must be None or have the same length as the number of outputs")
+        }
+
+        (0..si.len())
+            .map(|n| {
+                Self::new_(
+                    nodes.clone(),
+                    GeneralFunctionSpecFull::MultiOutput(Box::new(spec.clone()), n),
+                    name,
+                    si[n].clone(),
+                    ddtos.as_ref().and_then(|x| x[n].clone()),
+                    multi_output_shapes.clone(),
+                )
+            })
+            .collect()
+    }
+
+    fn new_full(
+        nodes: Vec<CircuitRc>,
+        spec: GeneralFunctionSpecFull,
+        name: Option<Name>,
+    ) -> Result<Self> {
+        match spec {
+            GeneralFunctionSpecFull::SingleOutput(spec) => Self::try_new(nodes, spec, name),
+            GeneralFunctionSpecFull::MultiOutput(spec, n) => {
+                Ok(Self::new_multi_output(nodes, *spec, name)?[n].clone())
+            }
+        }
+    }
+
+    fn new_(
+        nodes: Vec<CircuitRc>,
+        spec: GeneralFunctionSpecFull,
+        name: Option<Name>,
+        shape_info: GeneralFunctionShapeInfo,
+        device_dtype_override: Option<TorchDeviceDtypeOp>,
+        multi_output_shapes: Option<Box<Vec<Shape>>>,
+    ) -> Result<Self> {
+        let GeneralFunctionShapeInfo {
+            shape,
+            num_non_batchable_output_dims,
+            input_batchability,
+        } = shape_info;
+
         let out = Self {
             spec,
-            info: match ddto {
+            info: match device_dtype_override {
                 Some(ddt) => CachedCircuitInfo::with_device_dtype(name, shape, nodes, ddt),
                 None => CachedCircuitInfo::incomplete(name, shape, nodes)?,
             },
             num_non_batchable_output_dims,
             input_batchability,
+            multi_output_shapes,
         };
         out.initial_init_info()
     }
 
+    pub fn evolve(&self, nodes: Vec<CircuitRc>, name: Option<Name>) -> Result<Self> {
+        Self::new_full(nodes, self.spec.clone(), name)
+    }
+
     pub fn is_batchable(&self) -> bool {
         self.input_batchability.iter().any(|x| *x)
     }
 }
 
 circuit_node_extra_impl!(GeneralFunction, self_hash_default);
 
 impl CircuitNodeComputeInfoImpl for GeneralFunction {}
 
 impl CircuitNodeHashItems for GeneralFunction {
     fn compute_hash_non_name_non_children(&self, hasher: &mut blake3::Hasher) {
-        hasher.update(&self.spec.compute_hash());
+        match &self.spec {
+            GeneralFunctionSpecFull::SingleOutput(x) => hasher.update(&x.compute_hash()),
+            GeneralFunctionSpecFull::MultiOutput(x, o) => {
+                hasher.update(&o.to_le_bytes());
+                hasher.update(&x.compute_hash())
+            }
+        };
     }
 }
 
 impl CircuitNode for GeneralFunction {
     circuit_node_auto_impl!("3c655670-b352-4a5f-891c-0d7160609341");
 
     fn _replace_children(&self, children: Vec<CircuitRc>) -> Result<Self> {
-        Self::try_new(children, self.spec.clone(), self.info().name)
+        Self::new_full(children, self.spec.clone(), self.info().name)
     }
 
     fn child_axis_map(&self) -> Vec<Vec<Option<usize>>> {
         let num_batchable_axes = self.rank() as u8 - self.num_non_batchable_output_dims;
         zip(self.children(), &self.input_batchability)
             .map(|(child, batchable)| {
                 if !batchable {
@@ -1458,22 +2100,54 @@
         name: Option<Name>,
     ) -> PyResult<PyClassInitializer<GeneralFunction>> {
         let out = GeneralFunction::try_new(nodes, spec, name)?;
 
         Ok(out.into_init())
     }
 
+    #[getter]
+    fn output(&self) -> Option<usize> {
+        match &self.spec {
+            GeneralFunctionSpecFull::SingleOutput(_) => None,
+            GeneralFunctionSpecFull::MultiOutput(_, o) => Some(*o),
+        }
+    }
+
+    #[staticmethod]
+    #[pyo3(signature=(*nodes, spec, name = None), name="new_multi_output")]
+    pub fn new_multi_output_py(
+        nodes: Vec<CircuitRc>,
+        spec: PyObject,
+        name: Option<Name>,
+    ) -> Result<Vec<Self>> {
+        Python::with_gil(|py| {
+            let spec: PyWrapMultiOutput = FromPyObject::extract(spec.as_ref(py))?;
+            Self::new_multi_output(nodes, spec, name)
+        })
+    }
+
     #[staticmethod]
     #[pyo3(signature=(*nodes, parse_string, name = None))]
     pub fn new_from_parse(
         nodes: Vec<CircuitRc>,
         parse_string: String,
         name: Option<Name>,
     ) -> Result<Self> {
-        if parse_string.contains(" at ") {
+        if let Some(inner) = parse_string.strip_prefix("output:") {
+            let (num, rest) = inner
+                .split_once(" ")
+                .context("failed to split output: into num & spec")?;
+            let num: usize = num.parse().context("failed to parse output num")?;
+
+            let mut split = rest.splitn(2, " at ");
+            let name = convert_op_str_to_format_err(split.next(), &parse_string)?;
+            let path = convert_op_str_to_format_err(split.next(), &parse_string)?;
+
+            Ok(Self::new_multi_output_by_path(nodes, path, Some(name.into()))?[num].clone())
+        } else if parse_string.contains(" at ") {
             let mut split = parse_string.splitn(2, " at ");
             let name = convert_op_str_to_format_err(split.next(), &parse_string)?;
             let path = convert_op_str_to_format_err(split.next(), &parse_string)?;
 
             Self::new_by_path(nodes, path, Some(name.into()))
         } else {
             Self::new_by_name(nodes, parse_string.into(), name)
@@ -1490,25 +2164,30 @@
     #[staticmethod]
     #[pyo3(signature=(*nodes, spec_name, name = None))]
     pub fn new_by_name_op(
         nodes: Vec<CircuitRc>,
         spec_name: Name,
         name: Option<Name>,
     ) -> Result<Option<Self>> {
-        // parse index case
+        // parse case
         static RE_MULTINOMIAL: Lazy<Regex> = Lazy::new(|| {
             Regex::new(r"^multinomial(_no_replace)?_\[\s*((?:\d+\s*,\s*)*(?:\d+\s*)?)\]$").unwrap()
         });
+        static RE_A_SAMP_MULTINOMIAL: Lazy<Regex> = Lazy::new(|| {
+            Regex::new(r"^a_samp_multinomial_\[\s*((?:\d+\s*,\s*)*(?:\d+\s*)?)\]$").unwrap()
+        });
+        static RE_TOP_K: Lazy<Regex> =
+            Lazy::new(|| Regex::new(r"^top_k_\[\s*((?:\d+\s*,\s*)*(?:\d+\s*)?)\]$").unwrap());
         static RE_GEN_INDEX: Lazy<Regex> = Lazy::new(|| {
             Regex::new(r"^gen_index_at_(-?\d+)(_batch_x)?(_no_batch_index)?(_c)?$").unwrap()
         });
         static RE_EXPLICIT_INDEX: Lazy<Regex> =
             Lazy::new(|| Regex::new(r"^explicit_index_at_(-?\d+)_x_non_b_(\d+)(_c)?$").unwrap());
         static RE_CAST: Lazy<Regex> = Lazy::new(|| {
-            Regex::new(r"^cast_from_\{device:([a-zA-Z0-9]+),dtype:([a-zA-Z0-9]+)\}_to_\{device:([a-zA-Z0-9]+),dtype:([a-zA-Z0-9]+)\}$").unwrap()
+            Regex::new(r"^cast_from_\{device:([a-zA-Z0-9:]+),dtype:([a-zA-Z0-9]+)\}_to_\{device:([a-zA-Z0-9:]+),dtype:([a-zA-Z0-9]+)\}$").unwrap()
         });
         let spec = if let Some(re_captures) = RE_GEN_INDEX.captures(&spec_name) {
             let index_dim = re_captures
                 .get(1)
                 .unwrap()
                 .as_str()
                 .parse()
@@ -1538,14 +2217,44 @@
             }
             let shape = axis_strs.into_iter().map(|x| x.parse().unwrap()).collect();
             GeneralFunctionMultinomialSpec {
                 replacement: re_captures.get(1).is_none(),
                 shape,
             }
             .into()
+        } else if let Some(re_captures) = RE_A_SAMP_MULTINOMIAL.captures(&spec_name) {
+            let mut axis_strs: Vec<_> = re_captures
+                .get(1)
+                .unwrap()
+                .as_str()
+                .split(',')
+                .map(|z| z.trim())
+                .collect();
+            if axis_strs.last() == Some(&"") {
+                // allow last axis to be empty due to trailing comma
+                // (Regex guarantees that only last axis has this I think, but better to be clear)
+                axis_strs.pop();
+            }
+            let shape = axis_strs.into_iter().map(|x| x.parse().unwrap()).collect();
+            GeneralFunctionAlreadySampledMultinomialSpec { shape }.into()
+        } else if let Some(re_captures) = RE_TOP_K.captures(&spec_name) {
+            let mut axis_strs: Vec<_> = re_captures
+                .get(1)
+                .unwrap()
+                .as_str()
+                .split(',')
+                .map(|z| z.trim())
+                .collect();
+            if axis_strs.last() == Some(&"") {
+                // allow last axis to be empty due to trailing comma
+                // (Regex guarantees that only last axis has this I think, but better to be clear)
+                axis_strs.pop();
+            }
+            let shape = axis_strs.into_iter().map(|x| x.parse().unwrap()).collect();
+            GeneralFunctionTopKSpec { shape }.into()
         } else if let Some(re_captures) = RE_EXPLICIT_INDEX.captures(&spec_name) {
             let index_dim = re_captures
                 .get(1)
                 .unwrap()
                 .as_str()
                 .parse()
                 .context("failed to parse index_dim for explicit_index_at")?;
@@ -1591,19 +2300,32 @@
                     } else {
                         Some(dtype_in.to_owned().try_into().unwrap())
                     },
                 },
             }
             .into()
         } else if spec_name.str() == "pow" {
-            GeneralFunctionPowSpec {}.into()
+            GeneralFunctionPairwiseSpec {
+                pairwise_type: PairwiseType::Pow,
+            }
+            .into()
+        } else if spec_name.str() == "minimum" {
+            GeneralFunctionPairwiseSpec {
+                pairwise_type: PairwiseType::Minimum,
+            }
+            .into()
+        } else if spec_name.str() == "maximum" {
+            GeneralFunctionPairwiseSpec {
+                pairwise_type: PairwiseType::Maximum,
+            }
+            .into()
         } else if spec_name.str() == "Output" {
-            GeneralFunctionSpec::Output(GeneralFunctionOutputSpec {})
+            GeneralFunctionOutputSpec {}.into()
         } else if let Some(spec) = SPECS.get(&spec_name) {
-            spec.clone()
+            spec.clone().into()
         } else {
             return Ok(None);
         };
 
         GeneralFunction::try_new(nodes, spec, name).map(Some)
     }
 
@@ -1614,15 +2336,32 @@
 
         let spec: GeneralFunctionSpec =
             Python::with_gil(|py| -> Result<GeneralFunctionSpec, pyo3::PyErr> {
                 let spec_cls = locator.get_class(py)?;
                 spec_cls.call0()?.extract()
             })?;
 
-        GeneralFunction::try_new(nodes, spec, name)
+        GeneralFunction::try_new(nodes, spec.into(), name)
+    }
+
+    #[staticmethod]
+    #[pyo3(signature=(*nodes, path, name = None))]
+    pub fn new_multi_output_by_path(
+        nodes: Vec<CircuitRc>,
+        path: String,
+        name: Option<Name>,
+    ) -> Result<Vec<Self>> {
+        let locator = PyClassLocator::parse(&path)?;
+
+        let spec = Python::with_gil(|py| -> Result<PyWrapMultiOutput, pyo3::PyErr> {
+            let spec_cls = locator.get_class(py)?;
+            spec_cls.call0()?.extract()
+        })?;
+
+        GeneralFunction::new_multi_output(nodes, spec.into(), name)
     }
 
     #[staticmethod]
     #[pyo3(signature=(
         x,
         index,
         index_dim,
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/lib.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     collections::{BTreeMap, BTreeSet},
     fmt::Debug,
     ops::{Deref, DerefMut},
 };
 
 use anyhow::Result;
 use num_bigint::BigUint;
-use pyo3::{prelude::*, pyclass::CompareOp};
+use pyo3::{once_cell::GILLazyPy, prelude::*, pyclass::CompareOp, types::PyBool};
 use rr_util::{
     eq_by_big_hash::EqByBigHash,
     name::Name,
     py_types::{
         reduction_to_ints, use_rust_comp, PyCallable, PyOpAtAxes, PySymShape, Tensor,
         PY_CIRCUIT_ITEMS,
     },
@@ -77,21 +77,28 @@
         m
     )?)?;
     m.add_function(wrap_pyfunction!(
         crate::generalfunction::get_shape_info_broadcast,
         m
     )?)?;
     m.add_function(wrap_pyfunction!(crate::generalfunction::pow, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::generalfunction::maximum, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::generalfunction::minimum, m)?)?;
     m.add_function(wrap_pyfunction!(crate::generalfunction::multinomial, m)?)?;
+    m.add_function(wrap_pyfunction!(
+        crate::generalfunction::already_sampled_multinomial,
+        m
+    )?)?;
     crate::generalfunction::register(py, m)?;
     m.add_class::<crate::generalfunction::GeneralFunctionIndexSpec>()?;
     m.add_class::<crate::generalfunction::GeneralFunctionExplicitIndexSpec>()?;
     m.add_class::<crate::generalfunction::GeneralFunctionSetDDSpec>()?;
-    m.add_class::<crate::generalfunction::GeneralFunctionPowSpec>()?;
+    m.add_class::<crate::generalfunction::GeneralFunctionPairwiseSpec>()?;
     m.add_class::<crate::generalfunction::GeneralFunctionMultinomialSpec>()?;
+    m.add_class::<crate::generalfunction::GeneralFunctionAlreadySampledMultinomialSpec>()?;
     m.add_class::<crate::Einsum>()?;
     m.add_class::<crate::Array>()?;
     m.add_class::<crate::Symbol>()?;
     m.add_class::<crate::Scalar>()?;
     m.add_class::<crate::Add>()?;
     m.add_class::<crate::Rearrange>()?;
     m.add_class::<crate::Index>()?;
@@ -174,15 +181,16 @@
 impl EqByBigHash for PyCircuitBase {
     fn hash(&self) -> HashBytes {
         self.info().hash
     }
 }
 
 const DEFAULT_FANCY_VALIDATE: bool = false;
-const DEFAULT_ASSERT_ANY_FOUND: bool = false;
+const DEFAULT_ASSERT_FOUND: GILLazyPy<PyObject> =
+    GILLazyPy::new_py(|py| PyBool::new(py, false).into());
 
 #[pymethods]
 impl PyCircuitBase {
     #[getter]
     fn shape(&self) -> PySymShape {
         PySymShape(self.info().shape.clone())
     }
@@ -494,35 +502,33 @@
     }
     pub fn into_var(&self) -> Option<Var> {
         self.0.clone().c().into()
     }
     #[pyo3(signature=(
         matcher,
         transform,
-        cache_transform = true,
-        cache_update = true,
         fancy_validate = DEFAULT_FANCY_VALIDATE,
-        assert_any_found = DEFAULT_ASSERT_ANY_FOUND
+        assert_found = DEFAULT_ASSERT_FOUND.clone(),
+        assert_different = false,
     ))]
     pub fn update(
         &self,
         matcher: OpaqueIterativeMatcherVal,
         transform: PyObject,
-        cache_transform: bool,
-        cache_update: bool,
         fancy_validate: bool,
-        assert_any_found: bool,
+        assert_found: PyObject,
+        assert_different: bool,
     ) -> PyResult<CircuitRc> {
+        // Python:with_gil(|x| )
         matcher.update(
             self.0.clone(),
             transform,
-            cache_transform,
-            cache_update,
             fancy_validate,
-            assert_any_found,
+            assert_found,
+            assert_different,
         )
     }
     #[pyo3(signature=(matcher, fancy_validate = DEFAULT_FANCY_VALIDATE))]
     pub fn get(
         &self,
         matcher: OpaqueIterativeMatcherVal,
         fancy_validate: bool,
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/module.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/module.rs`

 * *Files 0% similar despite different names*

```diff
@@ -963,15 +963,19 @@
                     .any(|arg_spec| arg_spec.symbol == *x.as_symbol_unwrap())
             })
             .cloned()
             .collect();
         for n in &nodes {
             free_syms.extend(get_free_symbols(n).iter().cloned());
         }
-        substitute_cached_info.free_symbols = Some(Arc::new(free_syms));
+        substitute_cached_info.free_symbols = if free_syms.is_empty() {
+            None
+        } else {
+            Some(Arc::new(free_syms))
+        };
 
         let out = Self {
             info: CachedCircuitInfo {
                 name,
                 children: once(spec.circuit.clone()).chain(nodes).collect(),
                 ..substitute_cached_info
             },
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/named_axes.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/named_axes.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/nrc.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/nrc.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/opaque_iterative_matcher.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/opaque_iterative_matcher.rs`

 * *Files 2% similar despite different names*

```diff
@@ -340,18 +340,17 @@
 
     // below methods should just be used for PyCircuitBase
     defer_to_py!(
         fn update(
             &self,
             circuit: CircuitRc,
             transform: PyObject,
-            cache_transform: bool,
-            cache_update: bool,
             fancy_validate: bool,
-            assert_any_found: bool,
+            assert_found: PyObject,
+            assert_different: bool,
         ) -> PyResult<CircuitRc>;
 
         fn get(&self, circuit: CircuitRc, fancy_validate: bool) -> PyResult<BTreeSet<CircuitRc>>;
 
         fn get_unique_op(
             &self,
             circuit: CircuitRc,
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/self_funcs.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/self_funcs.rs`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 pub struct SelfFuncs {
     pub replace_expand_map: fn(CircuitRc, Vec<(CircuitRc, CircuitRc)>) -> Result<CircuitRc>,
     pub replace_expand_bottom_up_dyn:
         fn(CircuitRc, &dyn Fn(CircuitRc) -> Option<CircuitRc>) -> Result<CircuitRc>,
     pub repr_circuit_default_no_bijection: fn(CircuitRc) -> String,
     pub debug_repr: fn(CircuitRc) -> Result<String>,
     pub compiler_default_print: fn(CircuitRc) -> (),
-    pub compiler_default_repr: fn(CircuitRc) -> Result<String>,
     pub repr: fn(CircuitRc) -> Result<String>,
     pub repr_shape_always: fn(CircuitRc) -> Result<String>,
     pub print_circuit_stats: fn(&Circuit) -> (),
     pub PrintOptionsBase_print: fn(Option<PyObject>, &[CircuitRc]) -> Result<()>,
     pub PrintHtmlOptions_print: fn(Option<PyObject>, &[CircuitRc]) -> Result<()>,
     pub PrintOptions_repr: fn(Option<PyObject>, CircuitRc) -> Result<String>,
     pub parse_circuit: fn(&str, &mut Option<TensorCacheRrfs>) -> Result<CircuitRc>,
@@ -58,18 +57,14 @@
     (SELF_FUNCS.print_circuit_stats)(circuit)
 }
 
 pub fn compiler_default_print(circuit: &CircuitRc) {
     (SELF_FUNCS.compiler_default_print)(circuit.clone())
 }
 
-pub fn compiler_default_repr(circuit: &CircuitRc) -> Result<String> {
-    (SELF_FUNCS.compiler_default_repr)(circuit.clone())
-}
-
 pub fn repr_shape_always(circuit: CircuitRc) -> Result<String> {
     (SELF_FUNCS.repr_shape_always)(circuit)
 }
 
 pub fn parse_circuit(x: &str, cache: &mut Option<TensorCacheRrfs>) -> Result<CircuitRc> {
     (SELF_FUNCS.parse_circuit)(x, cache)
 }
```

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_base/src/variable_nodes.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_base/src/variable_nodes.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/nb_operations/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 crate-type = ["lib"]
 
 [dependencies]
 pyo3= { features=["num-bigint", "multiple-pymethods", "anyhow", "macros"], git = "https://github.com/redwoodresearch/pyo3" }
 anyhow= { version = "1.0.60", features = ["backtrace"] }
 thiserror= "1.0.32"
-smallvec= { version = "1.10.0", features = ["union"] }
+smallvec= { version = "1.10.0", features = ["union", "specialization"] }
 macro_rules_attribute= "0.1.2"
 rustc-hash= "1.1.0"
 paste= "1.0.8"
 cached= {version = "0.38.0", default-features = false}
 blake3= "1.3.1"
 itertools= "0.10.3"
 rand= {version = "0.8.5", features = ["small_rng"]}
```

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/src/cumulant_rewrites.rs` & `rust_circuit-0.4.9/local_dependencies/nb_operations/src/cumulant_rewrites.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/src/distribute_and_factor.rs` & `rust_circuit-0.4.9/local_dependencies/nb_operations/src/distribute_and_factor.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/src/generalfunction.rs` & `rust_circuit-0.4.9/local_dependencies/nb_operations/src/generalfunction.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-use anyhow::{anyhow, bail, Context, Result};
+use std::iter::zip;
+
+use anyhow::{bail, Context, Result};
 use circuit_base::{generalfunction::*, Array, GeneralFunctionSpec};
+use itertools::izip;
 use pyo3::{prelude::*, types::PyTuple};
 use rand::{self, Rng};
 use rr_util::{
     py_types::{assert_tensors_close, ExtraPySelfOps, Tensor},
-    shape::{shape_is_known, shape_join_eq, Shape, Size},
+    shape::{shape_is_known, Shape, Size},
 };
-use smallvec::ToSmallVec;
 
 /// I now think this maybe should have been written in python.
 /// Not to bad to port I guess...
 #[pyclass]
 pub struct GeneralFunctionSpecTester {
     #[pyo3(set, get)]
     pub samples_per_batch_dims: usize,
@@ -61,14 +63,41 @@
     if rng.gen_bool(0.01) {
         Size::NONE
     } else {
         Size::known(rng.gen_range(start..end))
     }
 }
 
+#[derive(Debug, Clone, FromPyObject)]
+pub enum GeneralFunctionSpecAny {
+    Single(GeneralFunctionSpec),
+    Multi(PyWrapMultiOutput),
+}
+
+impl GeneralFunctionSpecAny {
+    fn get_shape_info(&self, shapes: &[Shape]) -> Result<Vec<GeneralFunctionShapeInfo>> {
+        match self {
+            Self::Single(spec) => Ok(vec![spec.get_shape_info(shapes)?]),
+            Self::Multi(multi) => multi.get_shape_info(shapes),
+        }
+    }
+    fn function(&self, tensors: &[Tensor]) -> Result<Vec<Tensor>> {
+        match self {
+            Self::Single(spec) => Ok(vec![spec.function(tensors)?]),
+            Self::Multi(multi) => multi.function(tensors),
+        }
+    }
+    fn name(&self) -> &'static str {
+        match self {
+            Self::Single(spec) => spec.name(),
+            Self::Multi(multi) => multi.name(),
+        }
+    }
+}
+
 #[pymethods]
 impl GeneralFunctionSpecTester {
     #[new]
     #[pyo3(signature=(
         samples_per_batch_dims = GeneralFunctionSpecTester::default().samples_per_batch_dims,
         base_shapes_samples = GeneralFunctionSpecTester::default().base_shapes_samples,
         min_frac_successful = GeneralFunctionSpecTester::default().min_frac_successful,
@@ -111,81 +140,51 @@
             randn_size_cap,
         }
     }
 
     #[pyo3(signature=(spec, shapes, shapes_must_be_valid = false))]
     pub fn test_from_shapes(
         &self,
-        spec: GeneralFunctionSpec,
+        spec: GeneralFunctionSpecAny,
         shapes: Vec<Shape>,
         shapes_must_be_valid: bool,
     ) -> Result<(bool, bool)> {
-        let GeneralFunctionShapeInfo {
-            shape,
-            num_non_batchable_output_dims,
-            input_batchability,
-        } = match spec.get_shape_info(&shapes) {
+        let si = match spec.get_shape_info(&shapes) {
             Ok(info) => info,
             Err(e) => {
                 if shapes_must_be_valid {
                     bail!(e.context("was supposed to be valid, but actually wasn't!"))
                 }
                 return Ok((false, false)); // No tests in case where this is invalid list of shapes
             }
         };
 
-        if num_non_batchable_output_dims as usize > shape.len() {
-            bail!(
-            "too many non batchable output dims! num_non_batchable_output_dims={} shape.len()={}",
-            num_non_batchable_output_dims,
-            shape.len()
-        );
-        }
-        if input_batchability.len() != shapes.len() {
-            bail!(
-                "input batchability len doesn't match! input_batchability.len()={} shapes.len()={}",
-                input_batchability.len(),
-                shapes.len()
-            );
-        }
+        let shape = si.iter().map(|x| &x.shape).collect::<Vec<_>>();
+        let num_non_batchable_output_dims = si
+            .iter()
+            .map(|x| x.num_non_batchable_output_dims)
+            .collect::<Vec<_>>();
+        let input_batchability = &si[0].input_batchability;
 
         if input_batchability.iter().all(|x| !*x) {
             // if none batchable, we don't have any tests to run
             return Ok((true, false));
         }
-        let current_num_batch_dims = shape.len() - num_non_batchable_output_dims as usize;
-
-        for (shape, &is_batch) in
-            std::iter::once((&shape, &true)).chain(shapes.iter().zip(&input_batchability))
-        {
-            if is_batch && shape.len() < current_num_batch_dims {
-                bail!(
-                "some batchable shape too short for batch, shape.len()={} current_num_batch_dims={}",
-                shape.len(),
-                current_num_batch_dims
-            );
-            }
-        }
-
-        shapes.iter().zip(&input_batchability).filter_map(|(s, is_batch)| is_batch.then(|| &s[..current_num_batch_dims]))
-            .try_fold(shape[..current_num_batch_dims].to_smallvec(), |a, b| {
-                shape_join_eq(&a, b, ||
-                anyhow!("inputs and output have non-matching 'batch' shapes, a={a:?} b={b:?} input_shapes={shapes:?} output_shape={shape:?}"))
-            })?;
+        let current_num_batch_dims = shape[0].len() - num_non_batchable_output_dims[0] as usize;
 
         let mut rng = rand::thread_rng();
 
         let mut run_sample = |num_batch_dims, random_inputs: bool| {
             let batch_shape: Shape = (0..num_batch_dims)
                 .map(|_| gen_size_in(&mut rng, self.start_shape_num, self.end_shape_num))
                 .collect();
 
             let new_shapes: Vec<Shape> = shapes
                 .iter()
-                .zip(&input_batchability)
+                .zip(input_batchability)
                 .map(|(s, &is_batch)| {
                     if is_batch {
                         batch_shape
                             .iter()
                             .chain(&s[current_num_batch_dims..])
                             .cloned()
                             .collect()
@@ -193,148 +192,155 @@
                         s.clone()
                     }
                 })
                 .collect();
 
             let general_info = || {
                 format!(
-                    "shapes={:?} shape={:?} new_shapes={:?} current_num_batch_dims={}",
+                    "input shapes={:?} output shape(s)={:?} new input shapes={:?} current_num_batch_dims={}",
                     shapes, shape, new_shapes, current_num_batch_dims
                 )
             };
 
             let new_info = spec.get_shape_info(&new_shapes).with_context(|| {
                 format!(
                     "spec isn't consistent, error on valid shapes\n{}",
                     general_info()
                 )
             })?;
+            let new_num_non_batchable_output_dims = new_info
+                .iter()
+                .map(|x| x.num_non_batchable_output_dims)
+                .collect::<Vec<_>>();
+            let new_shape = new_info.iter().map(|x| &x.shape).collect::<Vec<_>>();
 
             let prefix = "spec isn't consistent, ";
 
-            if new_info.num_non_batchable_output_dims != num_non_batchable_output_dims {
+            if new_num_non_batchable_output_dims != num_non_batchable_output_dims {
                 bail!(
                 "{}changed num_non_batchable_output_dims when only batching was changed\n{}\n{}",
                 prefix,
                 format!(
-                    "new_info.num_non_batchable_output_dims={} != num_non_batchable_output_dims={}",
-                    new_info.num_non_batchable_output_dims, num_non_batchable_output_dims
+                    "new_info.num_non_batchable_output_dims={:?} != num_non_batchable_output_dims={:?}",
+                    new_num_non_batchable_output_dims, num_non_batchable_output_dims
                 ),
                 general_info()
             );
             }
 
-            if new_info.input_batchability != input_batchability {
+            if &new_info[0].input_batchability != input_batchability {
                 bail!(
                     "{}changed input_batchability when only batching was changed\n{}\n{}",
                     prefix,
                     format!(
                         "new_info.input_batchability={:?} != input_batchability={:?}",
-                        new_info.input_batchability, input_batchability
+                        new_info[0].input_batchability, input_batchability
                     ),
                     general_info()
                 );
             }
 
-            let non_batch_shape = &shape[current_num_batch_dims..];
-            let expected_shape = batch_shape
-                .into_iter()
-                .chain(non_batch_shape.iter().cloned())
-                .collect::<Shape>();
-            if new_info.shape != expected_shape {
+            let expected_shapes: Vec<Shape> = shape
+                .iter()
+                .map(|out_shape| {
+                    batch_shape
+                        .iter()
+                        .chain(out_shape[current_num_batch_dims..].iter())
+                        .cloned()
+                        .collect::<Shape>()
+                })
+                .collect();
+            if zip(&new_shape, &expected_shapes).any(|(a, b)| a != &b) {
                 bail!(
-                    "{}unexpected shape\n{}\n{}",
+                    "{}unexpected output shapes\n{}\n{}",
                     prefix,
                     format!(
-                        "new_info.shape={:?} != expected_shape={:?}",
-                        new_info.shape, expected_shape
+                        "new_info.shape={:?} != expected_shapes={expected_shapes:?}",
+                        new_shape
                     ),
                     general_info()
                 );
             }
 
-            let get_count_find = |shapes: &[Shape], shape| {
+            let get_count_find = |shapes: &[Shape], shape: &Vec<&Shape>| {
                 shapes
                     .iter()
-                    .chain(std::iter::once(shape))
+                    .chain(shape.iter().cloned())
                     .map(|x| x.iter().map(|x| x.t().unwrap_or(1)).product::<usize>())
                     .sum::<usize>()
                     < self.randn_size_cap
             };
 
             if random_inputs
                 && get_count_find(&shapes, &shape)
-                && get_count_find(&new_shapes, &new_info.shape)
+                && get_count_find(&new_shapes, &new_shape)
                 && num_batch_dims < current_num_batch_dims
                 && shapes.iter().all(|x| shape_is_known(x))
             // only run random on < orig
             {
                 // TODO: swap to f64 as needed!
                 let tensors: Vec<_> = shapes
                     .iter()
                     .map(|shape| Array::randn(shape.clone()).unwrap().value)
                     .collect();
 
-                let out_tensor = spec
+                let out_tensors = spec
                     .function(&tensors)
                     .context("failed to evaluate for test")?;
-                if out_tensor.shape() != &shape {
-                    bail!(
-                        "{}: unexpected tensor shape\n{}\n{}",
-                        spec.name(),
-                        format!(
-                            "out_tensor.shape={:?} != shape={:?}",
-                            out_tensor.shape(),
-                            shape
-                        ),
-                        general_info()
-                    );
+                for (out_tensor, s) in out_tensors.iter().zip(&shape) {
+                    if &out_tensor.shape() != s {
+                        bail!(
+                            "{}: unexpected tensor shape\n{}\n{}",
+                            spec.name(),
+                            format!("out_tensor.shape={:?} != shape={s:?}", out_tensor.shape(),),
+                            general_info()
+                        );
+                    }
                 }
                 let dims_to_remove = current_num_batch_dims - num_batch_dims;
-                if shape[..dims_to_remove].iter().any(|x| x.is(0)) {
+                if shape[0][..dims_to_remove].iter().any(|x| x.is(0)) {
                     return Ok(());
                 }
                 let idxs: Py<PyTuple> = Python::with_gil(|py| {
                     PyTuple::new(
                         py,
-                        shape[..dims_to_remove]
+                        shape[0][..dims_to_remove]
                             .iter()
                             .map(|s| s.map(|x| rng.gen_range(0..x)).into_py(py)),
                     )
                     .into()
                 });
                 let run_idx = |tensor: Tensor| tensor.py_getitem_acquire(idxs.clone()).unwrap();
 
-                let new_tensor = spec
+                let new_tensors = spec
                     .function(
-                        &tensors
-                            .iter()
-                            .zip(&input_batchability)
+                        &zip(&tensors, input_batchability)
                             .map(|(x, &b)| if b { run_idx(x.clone()) } else { x.clone() })
                             .collect::<Vec<_>>(),
                     )
                     .context("failed to evaluate for test")?;
 
-                let new_tensor_expected_shape: Shape =
-                    shape[dims_to_remove..].iter().cloned().collect();
-                if new_tensor.shape() != &new_tensor_expected_shape {
-                    bail!(
-                        "{}: unexpected tensor shape\n{}\n{}",
-                        spec.name(),
-                        format!(
-                            "new_tensor.shape={:?} != expected_shape={:?}",
+                for (new_tensor, out_tensor, s) in izip!(new_tensors, out_tensors, &shape) {
+                    let new_tensor_expected_shape: Shape =
+                        s[dims_to_remove..].iter().cloned().collect();
+                    if new_tensor.shape() != &new_tensor_expected_shape {
+                        bail!(
+                            "{}: unexpected tensor shape\n{}\n{}",
+                            spec.name(),
+                            format!(
+                            "new_tensor.shape={:?} != expected_shape={new_tensor_expected_shape:?}",
                             new_tensor.shape(),
-                            expected_shape
                         ),
-                        general_info()
-                    );
-                }
+                            general_info()
+                        );
+                    }
 
-                assert_tensors_close(new_tensor, run_idx(out_tensor))
-                    .context("tensors not close! (TODO: error)")?
+                    assert_tensors_close(new_tensor, run_idx(out_tensor))
+                        .with_context(|| format!("running generalfunction on batch then indexing batchale dims should be same as indexing then running generalfunction but isn't,\n  out shape after idx={new_tensor_expected_shape:?} out shape before idx={shape:?}"))?
+                }
             }
 
             Ok(())
         };
 
         for num_batch_dims in 0..current_num_batch_dims + 5 {
             for _ in 0..self.samples_per_batch_dims {
@@ -342,36 +348,39 @@
             }
             run_sample(num_batch_dims, self.test_with_rand)?;
         }
 
         Ok((true, true))
     }
 
-    pub fn test_many_shapes(&self, spec: GeneralFunctionSpec) -> Result<()> {
+    pub fn test_many_shapes(&self, spec: GeneralFunctionSpecAny) -> Result<()> {
         let mut rng = rand::thread_rng();
         let mut any_frac_successful = false;
         let mut any_frac_checked_batch = false;
         let num_inputs_range = self.start_num_inputs..self.end_num_inputs;
         for num_inputs in num_inputs_range.clone() {
             let mut total_successful = 0.;
             let mut total_checked_batch = 0.;
             for _ in 0..self.base_shapes_samples {
-                let shapes = (0..num_inputs)
+                let shapes: Vec<_> = (0..num_inputs)
                     .map(|_| {
                         let ndim = rng.gen_range(self.start_ndim..self.end_ndim);
                         (0..ndim)
                             .map(|_| {
                                 gen_size_in(&mut rng, self.start_shape_num, self.end_shape_num)
                             })
                             .collect()
                     })
                     .collect();
 
-                let (was_successful, and_checked_batch) =
-                    self.test_from_shapes(spec.clone(), shapes, false)?;
+                let (was_successful, and_checked_batch) = self
+                    .test_from_shapes(spec.clone(), shapes.clone(), false)
+                    .with_context(|| {
+                        format!("failed batching checks with input shapes {shapes:?}")
+                    })?;
                 total_successful += if was_successful { 1. } else { 0. };
                 total_checked_batch += if and_checked_batch { 1. } else { 0. };
             }
 
             let frac_successful = total_successful / self.base_shapes_samples as f64;
             let frac_checked_batch = total_checked_batch / self.base_shapes_samples as f64;
 
@@ -422,15 +431,15 @@
         for removed_from_end in 0..2 {
             let spec = GeneralFunctionSimpleSpec {
                 name: "".into(),
                 num_non_batchable_output_dims,
                 removed_from_end,
             }
             .into();
-            tester.test_many_shapes(spec)?;
+            tester.test_many_shapes(GeneralFunctionSpecAny::Single(spec))?;
         }
     }
     // // TODO: this segfaults in pytorch and I can't seem to fix :/
     // // Note that tests work in python, so it must be something with
     // // prepare_freethreaded_python.
     // let tester_rand = GeneralFunctionSpecTester {
     //     test_with_rand: true,
@@ -471,15 +480,15 @@
                 .into();
                 if !batch_index && index_dim >= 0 {
                     continue;
                 }
                 if !batch_x && !batch_index {
                     continue;
                 }
-                tester.test_many_shapes(spec)?;
+                tester.test_many_shapes(GeneralFunctionSpecAny::Single(spec))?;
             }
         }
 
         let spec: GeneralFunctionSpec = GeneralFunctionIndexSpec {
             index_dim,
             batch_x: true,
             batch_index: true,
@@ -512,15 +521,15 @@
                 .cloned()
                 .chain(suffix_shape.iter().cloned())
                 .collect();
             let index_shape = prefix_shape.clone();
 
             tester
                 .test_from_shapes(
-                    spec.clone(),
+                    GeneralFunctionSpecAny::Single(spec.clone()),
                     vec![x_shape.clone(), index_shape.clone()],
                     true,
                 )
                 .with_context(|| {
                     format!(
                         "fail with x_shape={:?} index_shape={:?} suffix_shape={:?} index_dim={}",
                         x_shape, index_shape, suffix_shape, index_dim
```

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/src/index_rewrites.rs` & `rust_circuit-0.4.9/local_dependencies/nb_operations/src/index_rewrites.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/src/lib.rs` & `rust_circuit-0.4.9/local_dependencies/nb_operations/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/src/modules.rs` & `rust_circuit-0.4.9/local_dependencies/nb_operations/src/modules.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/nb_operations/src/nest.rs` & `rust_circuit-0.4.9/local_dependencies/nb_operations/src/nest.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_utils/Cargo.toml` & `rust_circuit-0.4.9/local_dependencies/circuit_utils/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_utils/lib.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_utils/lib.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/local_dependencies/circuit_utils/set_of_circuits.rs` & `rust_circuit-0.4.9/local_dependencies/circuit_utils/set_of_circuits.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/Cargo.toml` & `rust_circuit-0.4.9/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rust_circuit"
-version = "0.4.8"
+version = "0.4.9"
 edition = "2021"
 
 [package.metadata.maturin]
 name = "rust_circuit._rust"
 [lib]
 name = "rust_circuit"
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
@@ -27,15 +27,15 @@
 circuit_rewrites = {path = "local_dependencies/circuit_rewrites" }
 circuit_print = {path = "local_dependencies/circuit_print" }
 get_update_node = {path = "local_dependencies/get_update_node" }
 nb_operations = {path = "local_dependencies/nb_operations" }
 
 expand_node = {path = "local_dependencies/expand_node" }
 
-smallvec= { version = "1.10.0", features = ["union"] }
+smallvec= { version = "1.10.0", features = ["union", "specialization"] }
 itertools= "0.10.3"
 indexmap= "1.9.2"
 rustc-hash= "1.1.0"
 
 [build-dependencies]
 pyo3-build-config= { git = "https://github.com/redwoodresearch/pyo3" }
 
@@ -66,15 +66,15 @@
 
 [workspace]
 members = ["local_dependencies/circuit_base", "local_dependencies/circuit_utils", "local_dependencies/circuit_rewrites", "local_dependencies/circuit_print", "local_dependencies/get_update_node", "local_dependencies/rr_util", "local_dependencies/expand_node", "local_dependencies/nb_operations"]
 
 [workspace.dependencies]
 anyhow = { version = "1.0.60", features = ["backtrace"] }
 
-smallvec = { version = "1.10.0", features = ["union"] }
+smallvec = { version = "1.10.0", features = ["union", "specialization"] }
 itertools = "0.10.3"
 indexmap = "1.9.2"
 rustc-hash = "1.1.0"
 rand = {version = "0.8.5", features = ["small_rng"]}
 cached = {version = "0.38.0", default-features = false}
 
 num-bigint = "0.4.3"
```

### Comparing `rust_circuit-0.4.8/Cargo.lock` & `rust_circuit-0.4.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
 dependencies = [
  "backtrace",
 ]
 
 [[package]]
 name = "arrayref"
-version = "0.3.6"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4c527152e37cf757a3f78aae5a06fbeefdb07ccc535c980a3208ee3060dd544"
+checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
@@ -405,20 +405,20 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.1.26"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
+checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
 dependencies = [
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
@@ -460,17 +460,17 @@
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "get_update_node"
@@ -497,32 +497,32 @@
  "smallvec",
  "thiserror",
  "uuid",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ghost"
-version = "0.1.8"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69e0cd8a998937e25c6ba7cc276b96ec5cc3f4dc4ab5de9ede4fb152bdd5c5eb"
+checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
@@ -571,17 +571,17 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
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
@@ -596,17 +596,17 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "inventory"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "498ae1c9c329c7972b917506239b557a60386839192f1cf0ca034f345b65db99"
+checksum = "7741301a6d6a9b28ce77c0fb77a4eb116b6bc8f3bef09923f7743d059c4157d3"
 dependencies = [
  "ctor",
  "ghost",
 ]
 
 [[package]]
 name = "itertools"
@@ -627,23 +627,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.30"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8c7cbf8b89019683667e347572e6d55a7df7ea36b0c4ce69961b0cde67b174"
+checksum = "43a558e3d911bc3c7bfc8c78bc580b404d6e51c1cefbf656e176a94b49b0df40"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "lock_api"
@@ -702,37 +702,37 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.34"
+version = "0.1.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dcb174b18635f7561a0c6c9fc2ce57218ac7523cf72c50af80e2d79ab8f3ba1"
+checksum = "3d88dad3f985ec267a3fcb7a1726f5cb1a7e8cad8b646e70a84f967210df23da"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "mini-internal"
-version = "0.1.29"
+version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5152dc5695fff2cc32a9d7de0fc1c5c17fedf63056f60f3f3f6ad4aa30e6a7"
+checksum = "261391cc14a85f1f05253c3f7b6f75937280f4171d72b3acf6548bad73b99626"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "miniserde"
-version = "0.1.29"
+version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33714b61fbb93970d67b4f1925cfa127cbb72424a72f83b4521284a8cea2aff5"
+checksum = "3f290fd592e7e59944141a818bcdf2823cd5996b1c3001e97f5c28b556305e31"
 dependencies = [
  "itoa",
  "mini-internal",
  "ryu",
 ]
 
 [[package]]
@@ -831,17 +831,17 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "os_str_bytes"
-version = "6.4.1"
+version = "6.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -878,25 +878,25 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
-source = "git+https://github.com/redwoodresearch/pyo3#1f9e320166258462f8bdbf01257dca5e66ac79ca"
+source = "git+https://github.com/redwoodresearch/pyo3#b7b62c2c252f718e3fd0d7bfac119e70dc580ac9"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset 0.7.1",
@@ -911,48 +911,48 @@
  "unindent",
  "uuid",
 ]
 
 [[package]]
 name = "pyo3-build-config"
 version = "0.17.3"
-source = "git+https://github.com/redwoodresearch/pyo3#1f9e320166258462f8bdbf01257dca5e66ac79ca"
+source = "git+https://github.com/redwoodresearch/pyo3#b7b62c2c252f718e3fd0d7bfac119e70dc580ac9"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
 version = "0.17.3"
-source = "git+https://github.com/redwoodresearch/pyo3#1f9e320166258462f8bdbf01257dca5e66ac79ca"
+source = "git+https://github.com/redwoodresearch/pyo3#b7b62c2c252f718e3fd0d7bfac119e70dc580ac9"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
 version = "0.17.3"
-source = "git+https://github.com/redwoodresearch/pyo3#1f9e320166258462f8bdbf01257dca5e66ac79ca"
+source = "git+https://github.com/redwoodresearch/pyo3#b7b62c2c252f718e3fd0d7bfac119e70dc580ac9"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.17.3"
-source = "git+https://github.com/redwoodresearch/pyo3#1f9e320166258462f8bdbf01257dca5e66ac79ca"
+source = "git+https://github.com/redwoodresearch/pyo3#b7b62c2c252f718e3fd0d7bfac119e70dc580ac9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
@@ -1019,40 +1019,41 @@
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
 name = "rr_util"
 version = "0.0.0"
 dependencies = [
  "anyhow",
  "base16",
  "blake3",
  "cached",
  "indexmap",
  "inventory",
  "itertools",
+ "libc",
  "macro_rules_attribute",
  "num-bigint",
  "once_cell",
  "paste",
  "pyo3",
  "regex",
  "rustc-hash",
@@ -1060,15 +1061,15 @@
  "thiserror",
  "threadpool",
  "uuid",
 ]
 
 [[package]]
 name = "rust_circuit"
-version = "0.4.8"
+version = "0.4.9"
 dependencies = [
  "anyhow",
  "circuit_base",
  "circuit_print",
  "circuit_rewrites",
  "circuit_utils",
  "criterion",
@@ -1086,17 +1087,17 @@
  "rustc-hash",
  "smallvec",
  "uuid",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d4a36c42d1873f9a77c53bde094f9664d9891bc604a45b4798fd2c389ed12e5b"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -1119,37 +1120,37 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.156"
+version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "314b5b092c0ade17c00142951e50ced110ec27cea304b1037c6969246c2469a4"
+checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.156"
+version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7e29c4601e36bcec74a223228dce795f4cd3616341a4af93520ca1a837c087d"
+checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1172,43 +1173,54 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5ab016db510546d856297882807df8da66a16fb8c4101cb8b30054b0d5b2d9c"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5420d42e90af0c38c3290abcca25b9b3bdf379fc9f55c528f53a269d9c9a267e"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "threadpool"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
@@ -1257,17 +1269,17 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.11"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524b68aca1d05e03fdf03fcdce2c6c94b6daf6d16861ddaa7e4f2b6638a9052c"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
@@ -1333,15 +1345,15 @@
 name = "uuid-macro-internal"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1b300a878652a387d2a0de915bdae8f1a548f0c6d45e072fe2688794b656cc9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
```

### Comparing `rust_circuit-0.4.8/benches/benches.rs` & `rust_circuit-0.4.9/benches/benches.rs`

 * *Files 3% similar despite different names*

```diff
@@ -17,35 +17,39 @@
 use itertools::izip;
 use rr_util::{opt_einsum::EinsumSpec, rrfs::get_rrfs_dir, tensor_util::TorchDeviceDtypeOp, timed};
 extern crate test;
 use circuit_rewrites::scheduled_execution::circuit_to_schedule;
 use rr_util::tensor_util::{TorchDevice, TorchDtype};
 #[allow(unused)]
 fn bench_schedule(circuits: &[CircuitRc]) {
-    let mut settings: OptimizationSettings = Default::default();
-    settings.verbose = 2;
-    settings.max_single_tensor_memory = 20_000_000_000;
-    settings.max_memory = 40_000_000_000;
-    settings.log_simplifications = true;
+    let settings = OptimizationSettings {
+        verbose: 2,
+        max_single_tensor_memory: 20_000_000_000,
+        max_memory: 40_000_000_000,
+        log_simplifications: true,
+        ..Default::default()
+    };
 
     for circuit in circuits {
         let mut context = OptimizationContext::new_settings(settings.clone());
         let result = optimize_circuit(circuit.clone(), &mut context);
         black_box(result);
         // println!("{}", context.stringify_logs());
         // println!("{:?}", result.info().hash);
     }
 }
 
 fn get_optimized(circuits: &[CircuitRc]) -> Vec<(CircuitRc, OptimizationContext)> {
-    let mut settings: OptimizationSettings = Default::default();
-    settings.verbose = 1;
-    settings.max_single_tensor_memory = 20_000_000_000;
-    settings.max_memory = 40_000_000_000;
-    settings.log_simplifications = true;
+    let settings = OptimizationSettings {
+        verbose: 1,
+        max_single_tensor_memory: 20_000_000_000,
+        max_memory: 40_000_000_000,
+        log_simplifications: true,
+        ..Default::default()
+    };
 
     circuits
         .iter()
         .map(|c| {
             let mut context = OptimizationContext::new_settings(settings.clone());
             (optimize_circuit(c.clone(), &mut context).unwrap(), context)
         })
```

### Comparing `rust_circuit-0.4.8/dao.md` & `rust_circuit-0.4.9/dao.md`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/faq.md` & `rust_circuit-0.4.9/faq.md`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/_rust.py` & `rust_circuit-0.4.9/python/rust_circuit/_rust.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/_rust.pyi` & `rust_circuit-0.4.9/python/rust_circuit/_rust.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -157,21 +157,27 @@
     def rename_axes(self, named_axes: Dict[int, str]) -> Circuit:
         """Return set_named_axes(self, named_axes)."""
     def visit(self, f: Callable[[Circuit], None]): ...
     def update(
         self,
         matcher: IterativeMatcherIn,
         transform: TransformIn,
-        cache_transform: bool = True,
-        cache_update: bool = True,
         fancy_validate: bool = False,
-        assert_any_found: bool = False,
-    ) -> Circuit: ...
+        assert_found: bool | int = False,
+        assert_different: bool = False,
+    ) -> Circuit:
+        """
+        assert_different: assert output != input
+        assert_found: False=no assert, True=assert >=1 match, n=assert exactly n matches (shared subcircuits counted once)
+        fancy_validate: doesn't currently do anthing!
+        """
     def get(self, matcher: IterativeMatcherIn, fancy_validate: bool = False) -> Set[Circuit]:
-        """Returns the set of all nodes within the circuit which match."""
+        """Returns the set of all nodes within the circuit which match.
+
+        fancy_validate: run matcher.validate_matched on output to maybe catch bugs (incl bugs in python matchers)"""
     def get_unique_op(self, matcher: IterativeMatcherIn, fancy_validate: bool = False) -> Optional[Circuit]: ...
     def get_unique(self, matcher: IterativeMatcherIn, fancy_validate: bool = False) -> Circuit: ...
     def get_paths(self, matcher: IterativeMatcherIn) -> Dict[Circuit, Path]:
         """Return a dict where each matched node is associated with one arbitrary path to it."""
     def get_all_paths(self, matcher: IterativeMatcherIn) -> Dict[Circuit, Paths]:
         """Return a dict where each matched node is associated with a list of every path to it."""
     def get_all_circuits_in_paths(self, matcher: IterativeMatcherIn) -> List[Circuit]: ...
@@ -475,40 +481,51 @@
     def padding(self) -> List[Tuple[int, int]]: ...
     def is_identity(self) -> bool: ...
 
 class GeneralFunctionShapeInfo:
     """
     Returned by ``get_shape_info``, this contains the shape itself as well as batchability info.
 
-    shape is output shape.
+    shape is output shape (or shapes in case of multi-output generalfunctions). len(shape) == len(num_non_batchable_output_dims)
     input_batchability is a mask indicating which inputs support batching. if none do, there is no batching
     the number of non batchable dims in output, starting from end, is num_non_batchable_output_dims.
 
     all inputs with input_batchability=True should start with shape[:shape.len()-num_non_batchable_output_dims] (you can check this youself or it will be checked for you according to the GeneralFunctionShapeInfo you return)
 
     batchable means that your function should allow adding more dims to batchable inputs if dims are added to all inputs at once (but get_shape_info will be called again to check new shapes are okay so you can decide to only allow batching under some conditions), and that your function should be equal to running the function product(batch_dims) times, one for each batch input & concatting the result
 
     Expander inserts repeats to make batch dims the same shape for all batchable inputs before reconstructing GeneralFunctions (if you expand only one batchable input of a GeneralFunction then the other inputs will get repeated to have the same batch shape)
 
     example:
 
-    shape = [1, 2, 7, 9]
+    output shape = [1, 2, 7, 9]
     input_batchability = [True, False, True]
     num_non_batchable_output_dims = 2
     inputs:
     [1, 2, 5]
     [11, 19]
     [1, 2, 11]
+
+    output shape = [[1, 2, 7, 9], [1, 2, 22]]
+    input_batchability = [True, False, True]
+    num_non_batchable_output_dims = [2, 1]
+    inputs:
+    [1, 2, 5]
+    [11, 19]
+    [1, 2, 11]
     """
 
     shape: Shape
     num_non_batchable_output_dims: int
     input_batchability: Sequence[bool]
     def __init__(
-        self, shape: ShapeIn, num_non_batchable_output_dims: int, input_batchability: Sequence[bool]
+        self,
+        shape: ShapeIn,
+        num_non_batchable_output_dims: int,
+        input_batchability: Sequence[bool],
     ) -> None: ...
 
 class GeneralFunctionSimpleSpec:
     """typically initialized via `new_by_name` method on GeneralFunction"""
 
     @property
     def name(self) -> str: ...
@@ -563,44 +580,54 @@
 
 class GeneralFunctionSetDDSpec:
     @property
     def input_required_compatibility(self) -> TorchDeviceDtypeOp: ...
     @property
     def output(self) -> TorchDeviceDtypeOp: ...
 
-class GeneralFunctionPowSpec: ...
+class GeneralFunctionPairwiseSpec:
+    pairwise_type: int  # not actually int
 
 class GeneralFunctionMultinomialSpec:
     @property
     def replacement(self) -> bool: ...
     @property
     def shape(self) -> Shape: ...
 
+class GeneralFunctionAlreadySampledMultinomialSpec:
+    @property
+    def shape(self) -> Shape: ...
+
 GeneralFunctionSpec = Union[
     gf_spec_base.GeneralFunctionSpecBase,
     GeneralFunctionSimpleSpec,
     GeneralFunctionIndexSpec,
     GeneralFunctionExplicitIndexSpec,
     GeneralFunctionSetDDSpec,
-    GeneralFunctionPowSpec,
+    GeneralFunctionPairwiseSpec,
     GeneralFunctionMultinomialSpec,
+    GeneralFunctionAlreadySampledMultinomialSpec,
 ]
 """
 GeneralFunctionSpec contains all needed info about function, and is the same on all instances with the same function.
 """
 
 class GeneralFunction(Circuit):
+    spec: GeneralFunctionSpec | gf_spec_base.MultiOutputGeneralFunctionSpecBase
+    output: Optional[int]  # non-None if multi output generalfunction
     def __init__(
         self,
-        *args: Circuit,
+        *nodes: Circuit,
         spec: GeneralFunctionSpec,
         name: Optional[str] = None,
     ) -> None: ...
-    @property
-    def spec(self) -> GeneralFunctionSpec: ...
+    @staticmethod
+    def new_multi_output(
+        *nodes: Circuit, spec: gf_spec_base.MultiOutputGeneralFunctionSpecBase, name: Optional[str] = None
+    ) -> list[GeneralFunction]: ...
     @staticmethod
     def new_from_parse(*nodes: Circuit, parse_string: str, name: Optional[str] = None) -> GeneralFunction: ...
     @staticmethod
     def new_by_name(*nodes: Circuit, spec_name: str, name: Optional[str] = None) -> GeneralFunction: ...
     @staticmethod
     def new_by_name_op(*nodes: Circuit, spec_name: str, name: Optional[str] = None) -> Optional[GeneralFunction]: ...
     @staticmethod
@@ -719,17 +746,23 @@
 def max(circuit: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
 def last_dim_size(circuit: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
 def abs(circuit: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
 def exp(circuit: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
 def log(circuit: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
 def logit(circuit: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
 def pow(base: Circuit, exponent: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
+def minimum(x: Circuit, y: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
+def maximum(x: Circuit, y: Circuit, name: Optional[str] = None) -> GeneralFunction: ...
 def multinomial(
     probs: Circuit, seed: Circuit, shape: ShapeIn, replacement: bool = True, name: Optional[str] = None
 ) -> GeneralFunction: ...
+def already_sampled_multinomial(
+    probs: Circuit, exponentially_distributed_vals: Circuit, shape: Shape, name: Optional[str] = None
+) -> GeneralFunction: ...
+def top_k(values: Circuit, shape: Shape, name: Optional[str] = None) -> GeneralFunction: ...
 
 class GeneralFunctionSpecTester:
     """
     min_frac_successful controls the minimum fraction of proposed shapes which don't error for 'test_many_shapes'.
     Specifically, we check if this fraction is sufficiently high for *any* of the different number of possible inputs shapes.
 
     min_frac_checked_batch is the same except for checking that batching works
@@ -1959,26 +1992,24 @@
     def are_any_found(self, circuit: Circuit) -> bool:
         """Returns true if any node within the circuit matches."""
     def any_found(self) -> BoundAnyFound: ...
     def update(
         self,
         circuit: Circuit,
         transform: TransformIn,
-        cache_transform: bool = True,
-        cache_update: bool = True,
         fancy_validate: bool = False,
-        assert_any_found: bool = False,
+        assert_found: bool | int = False,
+        assert_different: bool = False,
     ) -> Circuit: ...
     def updater(
         self,
         transform: TransformIn,
-        cache_transform: bool = True,
-        cache_update: bool = True,
         default_fancy_validate: bool = False,
-        default_assert_any_found: bool = False,
+        default_assert_found: bool | int = False,
+        default_assert_different: bool = False,
     ) -> BoundUpdater: ...
 
 class Finished: ...
 
 FINISHED = Finished()
 
 IterativeMatcherIn = Union[MatcherIn, IterativeMatcher]
@@ -1989,15 +2020,16 @@
     through a circuit for some matching nodes.
     """
 
     def __init__(self, *inps: IterativeMatcherIn) -> None:
         """Does 'any' of the inputs if there arejo multiple"""
     def match_iterate(self, circuit: Circuit) -> IterateMatchResults: ...
     def debug_print_to_str(self) -> str: ...
-    def validate_matched(self, matched: Set[Circuit]) -> None: ...
+    def validate_matched(self, matched: Set[Circuit]) -> None:
+        """try to check that self matches all in matched, and try to give helpful errors it not (doesn't check all cases! also impossible to check all cases without original circuit anyways)"""
     @staticmethod
     def noop_traversal() -> IterativeMatcher: ...
     @staticmethod
     def term(match_next: bool = False) -> IterativeMatcher: ...
     def chain(self, *rest: IterativeMatcherIn, must_be_sub: bool = False) -> IterativeMatcher:
         """
         Constructs chain [self, *rest]
@@ -2170,26 +2202,22 @@
     def are_any_found(self, circuit: Circuit) -> bool:
         """Returns true if any node within the circuit matches."""
     def any_found(self) -> BoundAnyFound: ...
     def update(
         self,
         circuit: Circuit,
         transform: TransformIn,
-        cache_transform: bool = True,
-        cache_update: bool = True,
         fancy_validate: bool = False,
-        assert_any_found: bool = False,
+        assert_found: bool | int = False,
     ) -> Circuit: ...
     def updater(
         self,
         transform: TransformIn,
-        cache_transform: bool = True,
-        cache_update: bool = True,
         default_fancy_validate: bool = False,
-        default_assert_any_found: bool = False,
+        default_assert_found: bool | int = False,
     ) -> BoundUpdater: ...
     def apply_in_traversal(self, circuit: Circuit, transform: Transform) -> Circuit:
         """
         Replace everything outside traversal with symbols,
         then apply function,
         then replace back"""
 
@@ -2287,80 +2315,93 @@
     def new_finished(found: bool = False) -> IterateMatchResults: ...
     def to_tup(self) -> Tuple[Optional[UpdatedIterativeMatcher], bool]: ...
     def unwrap_or_same(self, matcher: IterativeMatcher) -> Tuple[UpdatedIterativeMatcher, bool]: ...
 
 TransformIn = Union[Callable[[Circuit], Circuit], Transform]
 
 class Transform:
+    """wrapper for `Callable[[Circuit], Circuit]` to allow pure rust functions too"""
+
     def __init__(self, inp: TransformIn) -> None: ...
     def run(self, circuit: Circuit) -> Circuit: ...
     def __call__(self, circuit: Circuit) -> Circuit:
         """Alias for run"""
     def debug_print_to_str(self) -> str: ...
     @staticmethod
     def ident() -> Transform: ...
     def updater(
         self,
-        cache_transform: bool = True,
-        cache_update: bool = True,
     ) -> Updater: ...
 
 class Updater:
+    """cache struct for update, caches transform as `circuit -> new_circuit` (on subcircuits where matcher matches) and update as `(circuit, matcher) -> new_circuit` (on all subcircuits)
+
+    see also Circuit.update docstring"""
+
     default_fancy_validate: bool
     def __init__(
         self,
         transform: TransformIn,
-        cache_transform: bool = True,
-        cache_update: bool = True,
         default_fancy_validate: bool = False,
-        default_assert_any_found: bool = False,
+        default_assert_found: bool | int = False,
+        default_assert_different: bool = False,
     ) -> None: ...
     @property
     def transform(self) -> Transform: ...
-    @property
-    def cache_transform(self) -> bool: ...
-    @property
-    def cache_update(self) -> bool: ...
     def update(
         self,
         circuit: Circuit,
         matcher: IterativeMatcherIn,
         fancy_validate: Optional[bool] = None,
-        assert_any_found: Optional[bool] = None,
+        assert_found: Optional[bool | int] = None,
+        assert_different: Optional[bool] = None,
     ) -> Circuit: ...
     def __call__(
         self,
         circuit: Circuit,
         matcher: IterativeMatcherIn,
-        fancy_validate: Optional[bool] = None,
-        assert_any_found: Optional[bool] = None,
+        fancy_validat: Optional[bool] = None,
+        assert_found: Optional[bool | int] = None,
+        assert_different: Optional[bool] = None,
     ) -> Circuit:
         """Alias for update"""
     def bind(self, matcher: IterativeMatcherIn) -> BoundUpdater: ...
 
 class BoundUpdater:
+    """cache struct for update with a specific matcher"""
+
     updater: Updater
     @property
     def matcher(self) -> IterativeMatcher: ...
     @matcher.setter
     def matcher(self, matcher: IterativeMatcherIn) -> None: ...
     def __init__(
         self,
         updater: Updater,
         matcher: IterativeMatcherIn,
     ) -> None: ...
     def update(
-        self, circuit: Circuit, fancy_validate: Optional[bool] = None, assert_any_found: Optional[bool] = None
+        self,
+        circuit: Circuit,
+        fancy_validate: Optional[bool] = None,
+        assert_found: Optional[bool | int] = None,
+        assert_different: Optional[bool] = None,
     ) -> Circuit: ...
     def __call__(
-        self, circuit: Circuit, fancy_validate: Optional[bool] = None, assert_any_found: Optional[bool] = None
+        self,
+        circuit: Circuit,
+        fancy_validate: Optional[bool] = None,
+        assert_found: Optional[bool | int] = None,
+        assert_different: Optional[bool] = None,
     ) -> Circuit:
         """Alias for update"""
 
 class Getter:
+    """cache struct for get, stores cache `(circuit, matcher) -> set[Circuit]` (also contains entries for subcircuits!)"""
+
     default_fancy_validate: bool
     """Fancy validation checks that all of the matchers matched something. For
     instance, each name/type/regex should match something. See tests for more details."""
     def __init__(self, default_fancy_validate: bool = False) -> None: ...
     def get(
         self, circuit: Circuit, matcher: IterativeMatcherIn, fancy_validate: Optional[bool] = None
     ) -> set[Circuit]: ...
@@ -2378,14 +2419,16 @@
         """Return a dict where each matched node is associated with one arbitrary path to it."""
     def get_all_paths(self, circuit: Circuit, matcher: IterativeMatcherIn) -> Dict[Circuit, Paths]:
         """Return a dict where each matched node is associated with a list of every path to it."""
     def validate(self, circuit: Circuit, matcher: IterativeMatcherIn) -> None: ...
     def bind(self, matcher: IterativeMatcherIn) -> BoundGetter: ...
 
 class BoundGetter:
+    """cache struct for get with a specific matcher"""
+
     getter: Getter
     @property
     def matcher(self) -> IterativeMatcher: ...
     @matcher.setter
     def matcher(self, matcher: IterativeMatcherIn) -> None: ...
     def __init__(self, getter: Getter, matcher: IterativeMatcherIn) -> None: ...
     def get(self, circuit: Circuit, fancy_validate: Optional[bool] = None) -> set[Circuit]: ...
@@ -2396,21 +2439,25 @@
     def get_paths(self, circuit: Circuit) -> Dict[Circuit, Path]:
         """Return a dict where each matched node is associated with one arbitrary path to it."""
     def get_all_paths(self, circuit: Circuit) -> Dict[Circuit, Paths]:
         """Return a dict where each matched node is associated with a list of every path to it."""
     def validate(self, circuit: Circuit) -> None: ...
 
 class AnyFound:
+    """cache struct for are_any_found"""
+
     def __init__(self) -> None: ...
     def are_any_found(self, circuit: Circuit, matcher: IterativeMatcherIn) -> bool: ...
     def __call__(self, circuit: Circuit, matcher: IterativeMatcherIn) -> bool:
         """Alias for are_any_found"""
     def bind(self, matcher: IterativeMatcherIn) -> BoundAnyFound: ...
 
 class BoundAnyFound:
+    """cache struct for are_any_found with a specific matcher"""
+
     any_found: AnyFound
     @property
     def matcher(self) -> IterativeMatcher: ...
     @matcher.setter
     def matcher(self, matcher: IterativeMatcherIn) -> None: ...
     def __init__(self, any_found: AnyFound, matcher: IterativeMatcherIn) -> None: ...
     def are_any_found(self, circuit: Circuit) -> bool: ...
@@ -2434,22 +2481,31 @@
     @property
     def suffix(self) -> Optional[str]: ...
     def __init__(
         self,
         *expanders: Tuple[IterativeMatcherIn, TransformIn],
         ban_multiple_matches_on_node: bool = False,
         default_fancy_validate: bool = False,
-        default_assert_any_found: bool = False,
+        default_assert_found: bool | int = False,
+        default_assert_different: bool = False,
         suffix: Optional[str] = None,
     ) -> None: ...
     def batch(
-        self, circuit: Circuit, fancy_validate: Optional[bool] = None, assert_any_found: Optional[bool] = None
+        self,
+        circuit: Circuit,
+        fancy_validate: Optional[bool] = None,
+        assert_found: Optional[bool | int] = None,
+        assert_different: Optional[bool] = None,
     ) -> Circuit: ...
     def __call__(
-        self, circuit: Circuit, fancy_validate: Optional[bool] = None, assert_any_found: Optional[bool] = None
+        self,
+        circuit: Circuit,
+        fancy_validate: Optional[bool] = None,
+        assert_found: Optional[bool | int] = None,
+        assert_different: Optional[bool] = None,
     ) -> Circuit:
         """Alias for batch"""
 
 class TensorCacheRrfs(object):
     def __init__(self, cutoff: int, small_capacityint, large_capacityint, device: str) -> None: ...
     def get_tensor(self, prefix: str) -> torch.Tensor: ...
     def get_tensor_if_cached(self, prefix: str) -> Optional[torch.Tensor]: ...
@@ -2629,24 +2685,31 @@
 def inline_single_callsite_modules(circuit: Circuit) -> Circuit: ...
 def replace_all_randn_seeded(circuit: Circuit) -> Circuit: ...
 def opt_eval_each_subcircuit_until_fail(circuit: Circuit, settings: OptimizationSettings) -> None: ...
 def compute_self_hash(circuit: Circuit) -> bytes: ...
 def diff_circuits(
     new: Circuit,
     old: Circuit,
-    options: PrintOptions = PrintOptions(),
+    options: PrintOptions = PrintOptions(arrows=True, bijection=False, traversal=IterativeMatcher.term()),
     require_child_count_same: bool = True,
     require_child_shapes_same: bool = False,
-    require_name_same: bool = True,
+    require_name_same: bool = False,
     print_legend: bool = True,
     same_self_color: CliColor = "Blue",
-    same_color: CliColor = None,
     new_color: CliColor = "Green",
     removed_color: CliColor = "Red",
-) -> str: ...
+) -> str:
+    """
+    require_{name, child_count, child_shapes}_same: if circuits have different name/child count/child shape, should they be diffed recursively or should we stop here and print them both?
+    same_self_color: nodes with same type & num children & spec but different children and/or name will have this color
+    new_color: color for nodes only in new & diff markers
+    removed_color: color for nodes only in old & diff markers
+    options.colorer: used to color shared subcircuits in both old & new
+    options.traversal: used to decide how much to print nodes that occur in both old & new (nodes that only occur in one are always shown)
+    """
 
 # circuit manipulation functions
 def deep_map(circuit: Circuit, fn: Callable[[Circuit], Circuit]) -> Circuit: ...
 def deep_map_preorder(circuit: Circuit, fn: Callable[[Circuit], Circuit]) -> Circuit: ...
 def filter_nodes(circuit: Circuit, fn: Callable[[Circuit], bool]) -> List[Circuit]: ...
 def replace_nodes(circuit: Circuit, map: Dict[Circuit, Circuit]) -> Circuit: ...
 def path_get(circuit: Circuit, path: List[int]) -> Circuit: ...
@@ -2998,15 +3061,16 @@
     def get_sample_shape(self) -> Circuit: ...
     def get_transform(self) -> Transform:
         """equal to sample_var"""
     def get_sample_expander(
         self,
         var_matcher: IterativeMatcherIn = default_var_matcher(),
         default_fancy_validate: bool = False,
-        default_assert_any_found: bool = False,
+        default_assert_found: bool | int = False,
+        default_assert_different: bool = False,
         suffix: Optional[str] = "sample",
         device_dtype: TorchDeviceDtypeOp = TorchDeviceDtypeOp(),
     ) -> Expander:
         """
         get a sample expander: an Expander configured to sample from vars. It will sample
         from all vars that are matched by var_matcher and batch over them
         together.
```

### Comparing `rust_circuit-0.4.8/python/rust_circuit/algebric_rewrite.py` & `rust_circuit-0.4.9/python/rust_circuit/algebric_rewrite.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/dataset.py` & `rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/dataset.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/experiment.py` & `rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/experiment.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/hypothesis.py` & `rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/hypothesis.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/causal_scrubbing/testing_utils.py` & `rust_circuit-0.4.9/python/rust_circuit/causal_scrubbing/testing_utils.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/cum_algo.py` & `rust_circuit-0.4.9/python/rust_circuit/cum_algo.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/causal_scrubbing/causal_scrubbing_simple.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/causal_scrubbing/causal_scrubbing_simple.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/causal_scrubbing/incr_number_simple.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/causal_scrubbing/incr_number_simple.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/causal_scrubbing/pool.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/causal_scrubbing/pool.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/notebook_testing.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/notebook_testing.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/causal_scrubbing_experiments.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/causal_scrubbing_experiments.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/setup.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/setup.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/test_paren_balancer_exercises.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/test_paren_balancer_exercises.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/paren_balancer/writeup_attribution_plots.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/paren_balancer/writeup_attribution_plots.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/basic_scope_manager.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/basic_scope_manager.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/custom_general_function.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/custom_general_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,50 @@
 # but we support bijection for custom functions stored in rrfs
 # NOTE: python caches imports, so editing the file and rerunning won't work in a notebook!
 func_stored_in_rrfs = rc.GeneralFunction.new_by_path(inp, path="/test/general_function.py:MyCustomSigmoid")
 func_stored_in_rrfs.print(rc.PrintOptions(bijection=True))
 
 # %%
 
+# generalfunctions can also have multiple outputs
+
+evaluated_times = 0
+
+
+class MyQR(rc.MultiOutputGeneralFunctionSpecBase):
+    def function(self, tensor: torch.Tensor) -> list[torch.Tensor]:
+        global evaluated_times
+        evaluated_times += 1
+        return torch.linalg.qr(tensor)
+
+    def get_shape_info(self, shape: rc.Shape) -> list[rc.GeneralFunctionShapeInfo]:
+        batch_shape = shape[:-2]
+        m, n = shape[-2:]
+        k = min(m, n)
+        return [
+            rc.GeneralFunctionShapeInfo(
+                shape=batch_shape + (m, k), num_non_batchable_output_dims=2, input_batchability=[True]
+            ),
+            rc.GeneralFunctionShapeInfo(
+                shape=batch_shape + (k, n), num_non_batchable_output_dims=2, input_batchability=[True]
+            ),
+        ]
+
+
+array = rc.Array.randn(3, 4, 5, 6)
+q, r = rc.GeneralFunction.new_multi_output(array, spec=MyQR())
+array2 = rc.Einsum.from_einsum_string("abij,abjk->abik", q, r)
+array2.print(rc.PrintOptions(bijection=False))
+array3 = array2.evaluate()
+assert evaluated_times == 1
+assert_close(array.value, array3)
+
+
+# %%
+
 # now let's define a function which has more interesting batching properties
 class MyCustomSoftmaxAndSum(rc.GeneralFunctionSpecBase):
     def function(self, x: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
         return torch.softmax(x, dim=-2).sum(dim=-1)
 
     def get_shape_info(self, *shapes: rc.Shape) -> rc.GeneralFunctionShapeInfo:
         # here, we set some batching options. See GeneralFunctionShapeInfo docs for what this does!
@@ -283,15 +319,15 @@
 # %%
 
 # torch.einsum w/ opt_einsum doesn't support 0 dims & GeneralFunctionSpecTester generates them
 torch.backends.opt_einsum.enabled = False  # type: ignore
 
 # by default, this function will basically never find any valid shapes! We
 # check that we do sometimes find valid shapes, so this will error (see `min_frac_successful` below)
-with pytest.raises(RuntimeError) as ex8:
+with pytest.raises((RuntimeError)) as ex8:
     rc.GeneralFunctionSpecTester(
         test_with_rand=True,
         samples_per_batch_dims=10,
         base_shapes_samples=1000,
         start_num_inputs=2,
         end_num_inputs=4,
         # this variable can be configured to change the minimum fraction of tests which do anything
```

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/fancy_error.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/fancy_error.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/handcrafted_model_cumulants.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/handcrafted_model_cumulants.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/iterative_matchers.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/iterative_matchers.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/modules_and_symbols.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/modules_and_symbols.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/nest.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/nest.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/printing_parsing.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/printing_parsing.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/push_down_index.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/push_down_index.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/push_down_module.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/push_down_module.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/save_models.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/save_models.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/simp.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/simp.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/transformer_config.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/transformer_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
 # %%
 
 # and some printers
 basic_term_early: List[rc.MatcherIn] = ["a", "m", "ln", "a.head.on_inp"]
 printer = rc.PrintOptions(
     bijection=False,
+    arrows=True,
+    # only_child_below=True,
+    # seen_children_same_line=True,
     traversal=rc.new_traversal(term_early_at=rc.Matcher(*basic_term_early)),
     colorer=rc.PrintOptions.type_colorer(),
 )
 less_term_early: List[rc.MatcherIn] = [
     *basic_term_early,
     rc.Matcher.regex(r"^a\d+((.h\d+)|(.norm))$"),
     rc.Matcher.regex(r"^m\d+(.norm)?(.p_bias)?$"),
```

### Comparing `rust_circuit-0.4.8/python/rust_circuit/demos/rust_circuit_demos/uitest.py` & `rust_circuit-0.4.9/python/rust_circuit/demos/rust_circuit_demos/uitest.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/general_function_spec_base.py` & `rust_circuit-0.4.9/python/rust_circuit/general_function_spec_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,7 +59,64 @@
         """This should error (exception) if the shapes are invalid and otherwise return GeneralFunctionShapeInfo"""
         raise NotImplementedError
 
     def get_device_dtype_override(self, *device_dtypes: rc.TorchDeviceDtypeOp) -> Optional[rc.TorchDeviceDtypeOp]:
         """Use this to check the validity of input dtypes/devices and set output device/dtype. If this returns None, the output inherits device/dtype from children.
         This can error to signal that inputs have invalid dtypes/devices"""
         return None
+
+
+class MultiOutputGeneralFunctionSpecBase(metaclass=abc.ABCMeta):
+    __hash_bytes: ClassVar[bytes]
+    """
+    Inherit from this base class in order to implement an arbitrary new GeneralFunctionSpec.
+
+    See docs for `get_shape_info`, GeneralFunctionShapeInfo, and `function`.
+    """
+
+    def __init_subclass__(cls):
+        b = bytearray()
+        for _, x in inspect.getmembers(cls, inspect.ismethod):
+            if hasattr(x, "__code__"):
+                b.extend(x.__code__.co_code)
+                b.extend(uuid.UUID("6739c5c8-a9ab-421d-a06c-38f356bed339").bytes)
+        b.extend(uuid.UUID("c5b1184c-76ae-430a-87cc-d6afc90569ce").bytes)
+        b.extend((cls.__module__ + "." + cls.__name__).encode())
+        cls.__hash_bytes = bytes(b)
+
+    @classmethod
+    def new(cls, *xs: rc.Circuit, name: Optional[str] = None):
+        """This should be overridden if your generalfunction has non-Circuit arguments"""
+        return rc.GeneralFunction(*xs, spec=cls(), name=name)
+
+    @property
+    def name(self) -> str:
+        return self.__class__.__name__
+
+    @property
+    def path(self) -> Optional[str]:
+        """The path of this spec relative to RRFS_DIR if this is stored in rrfs.
+        Should be of the form /dir/sub_dir/.../file.py:MyCustomSpec"""
+        return None
+
+    def compute_hash_bytes(self) -> bytes:
+        """What parts of self should be used for hashing & equality?
+
+        should be implemented if you store data on `self`"""
+        return self.__hash_bytes
+
+    @abc.abstractmethod
+    def function(self, *tensors: torch.Tensor) -> list[torch.Tensor]:
+        """run the actual function on tensors - these tensors shapes correspond to the shapes in ``get_shape_info``"""
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def get_shape_info(self, *shapes: rc.Shape) -> list[rc.GeneralFunctionShapeInfo]:
+        """This should error (exception) if the shapes are invalid and otherwise return GeneralFunctionShapeInfo"""
+        raise NotImplementedError
+
+    def get_device_dtype_override(
+        self, *device_dtypes: rc.TorchDeviceDtypeOp
+    ) -> Optional[list[Optional[rc.TorchDeviceDtypeOp]]]:
+        """Use this to check the validity of input dtypes/devices and set output device/dtype. If this returns None, the output inherits device/dtype from children.
+        This can error to signal that inputs have invalid dtypes/devices"""
+        return None
```

### Comparing `rust_circuit-0.4.8/python/rust_circuit/generalfuncs/rotary_pos_emb.py` & `rust_circuit-0.4.9/python/rust_circuit/generalfuncs/rotary_pos_emb.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/index_util/internal/general_function.py` & `rust_circuit-0.4.9/python/rust_circuit/index_util/internal/general_function.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/index_util/internal/infer_shapes.py` & `rust_circuit-0.4.9/python/rust_circuit/index_util/internal/infer_shapes.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/index_util/internal/ops.py` & `rust_circuit-0.4.9/python/rust_circuit/index_util/internal/ops.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/index_util/internal/parse.py` & `rust_circuit-0.4.9/python/rust_circuit/index_util/internal/parse.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/index_util/internal/resolve.py` & `rust_circuit-0.4.9/python/rust_circuit/index_util/internal/resolve.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/index_util/internal/view.py` & `rust_circuit-0.4.9/python/rust_circuit/index_util/internal/view.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/interop_rust.py` & `rust_circuit-0.4.9/python/rust_circuit/interop_rust.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/jax_to_module.py` & `rust_circuit-0.4.9/python/rust_circuit/jax_to_module.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/model_rewrites.py` & `rust_circuit-0.4.9/python/rust_circuit/model_rewrites.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,22 +368,14 @@
 
     if assert_not_present:
         assert len(set(einsum_axes).intersection(x.out_axes)) == 0
     insert_at_idx_v = op.unwrap_or(insert_at_idx, len(x.out_axes))
     return x.evolve(out_axes=x.out_axes[:insert_at_idx_v] + tuple(einsum_axes) + x.out_axes[insert_at_idx_v:])
 
 
-# po = rc.PrintOptions(
-#     # traversal=rc.restrict(m, True),
-#     colorer=rc.PrintOptions.type_colorer(),
-#     bijection=False,
-#     shape_only_when_necessary=False,arrows=True
-# )
-
-
 def split_by_pos(circ: rc.Circuit, config: SplitPosConfig, len_: int):
     """
     requires that weights have been pushed down all the way to heads, sequence length is specified as len_ (sequence_length in configure_transformer), and the model has causal attention (is_causal in configure_transformer)
 
     {layer: [(slice, name), (int, name2), ...], layer2: ...}: split these layers by position into this list of groups
     """
```

### Comparing `rust_circuit-0.4.8/python/rust_circuit/module_utils.py` & `rust_circuit-0.4.9/python/rust_circuit/module_utils.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/optional.py` & `rust_circuit-0.4.9/python/rust_circuit/optional.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/py_utils.py` & `rust_circuit-0.4.9/python/rust_circuit/py_utils.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/scope_manager.py` & `rust_circuit-0.4.9/python/rust_circuit/scope_manager.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/ui/circuits_very_named_tensor.py` & `rust_circuit-0.4.9/python/rust_circuit/ui/circuits_very_named_tensor.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/ui/cui.py` & `rust_circuit-0.4.9/python/rust_circuit/ui/cui.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/ui/encoding.py` & `rust_circuit-0.4.9/python/rust_circuit/ui/encoding.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/ui/ui.py` & `rust_circuit-0.4.9/python/rust_circuit/ui/ui.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/rust_circuit/ui/very_named_tensor.py` & `rust_circuit-0.4.9/python/rust_circuit/ui/very_named_tensor.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/causal_scrubbing/test_experiment.py` & `rust_circuit-0.4.9/python/tests/causal_scrubbing/test_experiment.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/causal_scrubbing/test_hypothesis.py` & `rust_circuit-0.4.9/python/tests/causal_scrubbing/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_algebric_rewrites.py` & `rust_circuit-0.4.9/python/tests/test_algebric_rewrites.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_auto_names.py` & `rust_circuit-0.4.9/python/tests/test_auto_names.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_circuit_type.py` & `rust_circuit-0.4.9/python/tests/test_circuit_type.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_conv.py` & `rust_circuit-0.4.9/python/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_convenience_methods.py` & `rust_circuit-0.4.9/python/tests/test_convenience_methods.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_cum_algo.py` & `rust_circuit-0.4.9/python/tests/test_cum_algo.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_expand_at_axes.py` & `rust_circuit-0.4.9/python/tests/test_expand_at_axes.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_expand_symbolic.py` & `rust_circuit-0.4.9/python/tests/test_expand_symbolic.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_flags.py` & `rust_circuit-0.4.9/python/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_gen_index.py` & `rust_circuit-0.4.9/python/tests/test_gen_index.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_general_function.py` & `rust_circuit-0.4.9/python/tests/test_general_function.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,21 @@
     with pytest.raises(rc.MiscInputCastIncompatibleDeviceDtypeError):
         casty2 = rc.GeneralFunction.new_cast(
             arr, rc.TorchDeviceDtypeOp("cpu", "int16"), rc.TorchDeviceDtypeOp("cpu", "float64")
         )
         print(casty2, casty2.device_dtype, casty2.evaluate())
 
 
+def test_cast_parse():
+    rc.Parser()(
+        """0 GeneralFunction cast_from_{device:None,dtype:None}_to_{device:cuda:2,dtype:None}
+  1 [2] Array rand"""
+    )
+
+
 @pytest.mark.cuda
 def test_cast_cuda():
     arr = rc.Array.randn(1, 2, device_dtype=rc.TorchDeviceDtypeOp("cpu", "float16"))
     casty1 = rc.GeneralFunction.new_cast(
         arr, rc.TorchDeviceDtypeOp("cpu", "float16"), rc.TorchDeviceDtypeOp("cuda:0", "float64")
     )
     assert casty1.device_dtype == rc.TorchDeviceDtypeOp("cuda:0", "float64")
@@ -93,7 +100,18 @@
     spec = foo.MyCustomSigmoid()
     x = rc.Symbol.new_with_random_uuid((3, 3, 3))
     f_by_path = rc.GeneralFunction.new_by_path(x, path="/test/general_function.py:MyCustomSigmoid")
     f_by_spec = rc.GeneralFunction(x, spec=spec)
     assert f_by_path == f_by_spec
     assert f_by_path == rc.Parser()(f_by_path.repr())
     assert f_by_spec == rc.Parser()(f_by_spec.repr())
+
+    spec = foo.MyQR()
+    x = rc.Symbol.new_with_random_uuid((3, 3, 3))
+    [a1, a2] = rc.GeneralFunction.new_multi_output_by_path(x, path="/test/general_function.py:MyQR")
+    [b1, b2] = rc.GeneralFunction.new_multi_output(x, spec=spec)
+    assert (a1, a2) == (b1, b2)
+    a3 = rc.Add(a1, a2)
+    b3 = rc.Add(b1, b2)
+
+    assert a3 == rc.Parser()(a3.repr())
+    assert b3 == rc.Parser()(b3.repr())
```

### Comparing `rust_circuit-0.4.8/python/tests/test_index_util.py` & `rust_circuit-0.4.9/python/tests/test_index_util.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_jax_to_module.py` & `rust_circuit-0.4.9/python/tests/test_jax_to_module.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_models.py` & `rust_circuit-0.4.9/python/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_module.py` & `rust_circuit-0.4.9/python/tests/test_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 def test_conform_all_modules(circ):
     circ1 = rc.conform_all_modules(circ)
     assert not any("internal_expand" in x.name for x in all_children(circ1))
     assert_close(circ.evaluate(), circ1.evaluate())
 
 
 @hypothesis.given(
-    get_c_st(probs_default=CP.kw(all=1, Module=20, Symbol=20, Cumulant=0), from_other=False, max_growth_steps=30),
+    get_c_st(probs_default=CP.kw(all=1, Module=20, Symbol=20, Cumulant=0), from_other=False, max_growth_steps=10),
     st.data(),
 )
 @mark_not_interesting_if(rc.PushDownModulePushingPastModuleWhichOverridesSymError)
 @mark_not_interesting_if(rc.ConstructModuleTriedToBatchUnbatchableInputError)
 def test_push_down_modules(circ, d):
     skips = d.draw(st_c.st_subsets([x.name for x in all_children(circ) if x.is_module()]))
     cb = d.draw(st.builds(rc.ModulePusher.remove_and_elim_callback, st.booleans(), st.booleans(), st.booleans()))
```

### Comparing `rust_circuit-0.4.8/python/tests/test_nb_rewrites.py` & `rust_circuit-0.4.9/python/tests/test_nb_rewrites.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_nest.py` & `rust_circuit-0.4.9/python/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_notebooks_and_demos.py` & `rust_circuit-0.4.9/python/tests/test_notebooks_and_demos.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_push_down_index.py` & `rust_circuit-0.4.9/python/tests/test_push_down_index.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_python_callables.py` & `rust_circuit-0.4.9/python/tests/test_python_callables.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_batching.py` & `rust_circuit-0.4.9/python/tests/test_rust_batching.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_get_update.py` & `rust_circuit-0.4.9/python/tests/test_rust_get_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -793,87 +793,93 @@
         "jk,ij->ik",
         Scalar(34.0, shape=(3, 7), name="!@*(#&$"),
         Add(b, Scalar(0.0, shape=a.shape, name="zero").sum(name="sum"), name="hi"),
         name="ein",
     )
 
 
-def test_updater_assert_any_found():
+def test_updater_assert_found():
     a = Scalar(1.0, shape=(1, 2), name="a")
 
     to_zero = lambda x: Scalar(0.0, shape=x.shape, name="zero")
 
-    assert a.update("a", to_zero, assert_any_found=True) == to_zero(a)
-    assert a.update({"a", "b"}, to_zero, assert_any_found=True) == to_zero(a)
+    assert a.update("a", to_zero, assert_found=True) == to_zero(a)
+    assert a.update({"a", "b"}, to_zero, assert_found=True) == to_zero(a)
     assert a.update("b", to_zero) == a
     with pytest.raises(RuntimeError, match="No matches found"):
-        a.update("b", to_zero, assert_any_found=True)
+        a.update("b", to_zero, assert_found=True)
 
-    assert IterativeMatcher("a").update(a, to_zero, assert_any_found=True) == to_zero(a)
-    assert IterativeMatcher({"a", "b"}).update(a, to_zero, assert_any_found=True) == to_zero(a)
+    assert IterativeMatcher("a").update(a, to_zero, assert_found=True) == to_zero(a)
+    assert IterativeMatcher({"a", "b"}).update(a, to_zero, assert_found=True) == to_zero(a)
     assert IterativeMatcher("b").update(a, to_zero) == a
     with pytest.raises(RuntimeError, match="No matches found"):
-        IterativeMatcher("b").update(a, to_zero, assert_any_found=True)
+        IterativeMatcher("b").update(a, to_zero, assert_found=True)
 
-    assert IterativeMatcher("a").updater(to_zero, default_assert_any_found=True)(a) == to_zero(a)
-    assert IterativeMatcher({"a", "b"}).updater(to_zero, default_assert_any_found=True)(a) == to_zero(a)
+    assert IterativeMatcher("a").updater(to_zero, default_assert_found=True)(a) == to_zero(a)
+    assert IterativeMatcher({"a", "b"}).updater(to_zero, default_assert_found=True)(a) == to_zero(a)
     assert IterativeMatcher("b").updater(to_zero)(a) == a
     with pytest.raises(RuntimeError, match="No matches found"):
-        IterativeMatcher("b").updater(to_zero, default_assert_any_found=True)(a)
+        IterativeMatcher("b").updater(to_zero, default_assert_found=True)(a)
 
-    assert IterativeMatcher("a").updater(to_zero)(a, assert_any_found=True) == to_zero(a)
-    assert IterativeMatcher({"a", "b"}).updater(to_zero)(a, assert_any_found=True) == to_zero(a)
+    assert IterativeMatcher("a").updater(to_zero)(a, assert_found=True) == to_zero(a)
+    assert IterativeMatcher({"a", "b"}).updater(to_zero)(a, assert_found=True) == to_zero(a)
     assert IterativeMatcher("b").updater(to_zero)(a) == a
     with pytest.raises(RuntimeError, match="No matches found"):
-        IterativeMatcher("b").updater(to_zero)(a, assert_any_found=True)
+        IterativeMatcher("b").updater(to_zero)(a, assert_found=True)
 
-    assert IterativeMatcher("a").updater(to_zero, default_assert_any_found=True).update(a) == to_zero(a)
-    assert IterativeMatcher({"a", "b"}).updater(to_zero, default_assert_any_found=True).update(a) == to_zero(a)
+    assert IterativeMatcher("a").updater(to_zero, default_assert_found=True).update(a) == to_zero(a)
+    assert IterativeMatcher({"a", "b"}).updater(to_zero, default_assert_found=True).update(a) == to_zero(a)
     assert IterativeMatcher("b").updater(to_zero).update(a) == a
     with pytest.raises(RuntimeError, match="No matches found"):
-        IterativeMatcher("b").updater(to_zero, default_assert_any_found=True).update(a)
+        IterativeMatcher("b").updater(to_zero, default_assert_found=True).update(a)
 
-    assert IterativeMatcher("a").updater(to_zero).update(a, assert_any_found=True) == to_zero(a)
-    assert IterativeMatcher({"a", "b"}).updater(to_zero).update(a, assert_any_found=True) == to_zero(a)
+    assert IterativeMatcher("a").updater(to_zero).update(a, assert_found=True) == to_zero(a)
+    assert IterativeMatcher({"a", "b"}).updater(to_zero).update(a, assert_found=True) == to_zero(a)
     assert IterativeMatcher("b").updater(to_zero).update(a) == a
     with pytest.raises(RuntimeError, match="No matches found"):
-        IterativeMatcher("b").updater(to_zero).update(a, assert_any_found=True)
+        IterativeMatcher("b").updater(to_zero).update(a, assert_found=True)
+
+    with pytest.raises(RuntimeError, match="Wrong number of matches found, found 1 assert_found=2"):
+        Add(a, a).update("a", to_zero, assert_found=2)
+    Add(a, a.rename("b")).update({"a", "b"}, to_zero, assert_found=2)
+
+    a.update("b", to_zero, assert_found=0)
 
     lax_updater = Updater(to_zero)
     # loop to test caching behavior
     for _ in range(2):
-        assert lax_updater(a, "a", assert_any_found=True) == to_zero(a)
-        assert lax_updater(a, {"a", "b"}, assert_any_found=True) == to_zero(a)
+        assert lax_updater(a, "a", assert_found=True) == to_zero(a)
+        assert lax_updater(a, {"a", "b"}, assert_found=True) == to_zero(a)
         assert lax_updater(a, "b") == a
         with pytest.raises(RuntimeError, match="No matches found"):
-            lax_updater(a, "b", assert_any_found=True)
+            lax_updater(a, "b", assert_found=True)
         with pytest.raises(RuntimeError, match="No matches found"):
-            lax_updater.update(a, "b", assert_any_found=True)
+            lax_updater.update(a, "b", assert_found=True)
 
-    strict_updater = Updater(to_zero, default_assert_any_found=True)
+    strict_updater = Updater(to_zero, default_assert_found=True)
     for _ in range(2):
         assert strict_updater(a, "a") == to_zero(a)
         assert strict_updater(a, {"a", "b"}) == to_zero(a)
-        assert strict_updater(a, "b", assert_any_found=False) == a
+        assert strict_updater(a, "b", assert_found=False) == a
         with pytest.raises(RuntimeError, match="No matches found"):
             strict_updater(a, "b")
         with pytest.raises(RuntimeError, match="No matches found"):
             strict_updater.update(a, "b")
 
 
-def test_expander_assert_any_found():
+def test_expander_assert_found():
     a = Scalar(1.0, shape=(3, 2), name="a")
 
     to_zero_expand = lambda x: Scalar(0.0, shape=(5, 3, 2), name="zero")
 
-    e_a = Expander(("a", to_zero_expand), default_assert_any_found=True)
-    e_a_b_1 = Expander(({"a", "b"}, to_zero_expand), default_assert_any_found=True)
-    e_a_b_2 = Expander(("a", to_zero_expand), ("b", to_zero_expand), default_assert_any_found=True)
+    e_a = Expander(("a", to_zero_expand), default_assert_found=True)
+    e_a_b_1 = Expander(({"a", "b"}, to_zero_expand), default_assert_found=True)
+    e_a_b_2 = Expander(("a", to_zero_expand), ("b", to_zero_expand), default_assert_found=True)
     e_b_lax = Expander(("b", to_zero_expand))
-    e_b_strict = Expander(("b", to_zero_expand), default_assert_any_found=True)
+    e_b_strict = Expander(("b", to_zero_expand), default_assert_found=True)
 
     # loop to test caching behavior
     for _ in range(2):
         assert e_a(a) == to_zero_expand(a)
         assert e_a_b_1(a) == to_zero_expand(a)
         assert e_a_b_2(a) == to_zero_expand(a)
         assert e_b_lax(a) == a
@@ -883,20 +889,26 @@
     e_a = Expander(("a", to_zero_expand))
     e_a_b_1 = Expander(({"a", "b"}, to_zero_expand))
     e_a_b_2 = Expander(("a", to_zero_expand), ("b", to_zero_expand))
     e_b = Expander(("b", to_zero_expand))
 
     # loop to test caching behavior
     for _ in range(2):
-        assert e_a(a, assert_any_found=True) == to_zero_expand(a)
-        assert e_a_b_1(a, assert_any_found=True) == to_zero_expand(a)
-        assert e_a_b_2(a, assert_any_found=True) == to_zero_expand(a)
+        assert e_a(a, assert_found=True) == to_zero_expand(a)
+        assert e_a_b_1(a, assert_found=True) == to_zero_expand(a)
+        assert e_a_b_2(a, assert_found=True) == to_zero_expand(a)
         assert e_b(a) == a
         with pytest.raises(RuntimeError, match="No matches found"):
-            e_b(a, assert_any_found=True)
+            e_b(a, assert_found=True)
+        with pytest.raises(RuntimeError, match="Wrong number of matches found, found 1 assert_found=2"):
+            e_a(a, assert_found=2)
+        e_a(Add(a, a), assert_found=1)
+        e_b_strict(a, assert_found=0)
+        e_a_b_1(Add(a, a.rename("b")), assert_found=2)
+        e_a_b_2(Add(a, a.rename("b")), assert_found=2)
 
 
 def test_batch():
     a = Scalar(1.0, shape=(1, 2), name="a")
     b = Scalar(2.0, shape=(2, 3), name="b")
     ein = Einsum.from_einsum_string("ij,jk->ik", a, b, name="ein")
     soft = GeneralFunction.new_by_name(ein, spec_name="softmax", name="soft")
```

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_large_models.py` & `rust_circuit-0.4.9/python/tests/test_rust_large_models.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_printing.py` & `rust_circuit-0.4.9/python/tests/test_rust_printing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1890,15 +1890,15 @@
         """
             ),
         ),
     ]
     print()
     for n, o in circuit_pairs:
         with timed("diffing"):
-            print(rc.diff_circuits(n, o, rc.PrintOptions(bijection=False), same_color="Cyan"))
+            print(rc.diff_circuits(n, o, rc.PrintOptions(bijection=False)))
 
 
 def test_rust_parsing_id_by_name():
     strings = [
         """
         0 'hi' Add
           1 ' my' [3, 1] Scatter [0:2,0:1]
```

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_python_manipulation.py` & `rust_circuit-0.4.9/python/tests/test_rust_python_manipulation.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_rewrite.py` & `rust_circuit-0.4.9/python/tests/test_rust_rewrite.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_schedule.py` & `rust_circuit-0.4.9/python/tests/test_rust_schedule.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_rust_variables.py` & `rust_circuit-0.4.9/python/tests/test_rust_variables.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_sample_transform.py` & `rust_circuit-0.4.9/python/tests/test_sample_transform.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_schedule_serialize.py` & `rust_circuit-0.4.9/python/tests/test_schedule_serialize.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/test_type_alias_import.py` & `rust_circuit-0.4.9/python/tests/test_type_alias_import.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/python/tests/util.py` & `rust_circuit-0.4.9/python/tests/util.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/readme.md` & `rust_circuit-0.4.9/readme.md`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/rust_circuit_example.py` & `rust_circuit-0.4.9/rust_circuit_example.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/rust_rewrite_example.py` & `rust_circuit-0.4.9/rust_rewrite_example.py`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/src/bin/print_exception_stubs.rs` & `rust_circuit-0.4.9/src/bin/print_exception_stubs.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/src/bin/to_profile.rs` & `rust_circuit-0.4.9/src/bin/to_profile.rs`

 * *Files identical despite different names*

### Comparing `rust_circuit-0.4.8/src/lib.rs` & `rust_circuit-0.4.9/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -75,32 +75,34 @@
 
     m.add(
         "__self_funcs",
         SelfFuncs {
             replace_expand_map: expand_node::replace_expand_map,
             replace_expand_bottom_up_dyn: expand_node::replace_expand_bottom_up_dyn,
             repr_circuit_default_no_bijection: |x| {
-                let mut po = circuit_print::print::PrintOptions::default();
-                po.bijection = false;
-                po.repr(x).unwrap()
+                circuit_print::print::PrintOptions {
+                    bijection: false,
+                    ..Default::default()
+                }
+                .repr(x)
+                .unwrap()
             },
             repr_shape_always: |x| {
-                let mut po = circuit_print::print::PrintOptions::default();
-                po.shape_only_when_necessary = false;
-                po.repr(x)
+                circuit_print::print::PrintOptions {
+                    shape_only_when_necessary: false,
+                    ..Default::default()
+                }
+                .repr(x)
             },
             debug_repr: circuit_print::print::debug_repr,
             compiler_default_print: |x| {
                 circuit_print::print::PrintOptions::compiler_default()
                     .print(x)
                     .unwrap()
             },
-            compiler_default_repr: |x| {
-                circuit_print::print::PrintOptions::compiler_default().repr(x)
-            },
             repr: |x| circuit_print::print::PrintOptions::default().repr(x),
             PrintOptionsBase_print: circuit_print::print_html::PrintOptionsBase_print,
             PrintHtmlOptions_print: circuit_print::print_html::PrintHtmlOptions_print,
             PrintOptions_repr: circuit_print::print::PrintOptions_repr,
             print_circuit_stats: circuit_print::print::print_circuit_stats,
             parse_circuit: |a, b| circuit_print::parsing::Parser::default().parse_circuit(a, b),
         },
```

### Comparing `rust_circuit-0.4.8/tests/compiler_bench_runs.rs` & `rust_circuit-0.4.9/tests/compiler_bench_runs.rs`

 * *Files 17% similar despite different names*

```diff
@@ -22,17 +22,19 @@
                 }
                 .parse_circuit(&fs::read_to_string(d.unwrap().path()).unwrap(), &mut None)
                 .ok()
             })
             .collect();
         dbg!("post");
 
-        let mut settings: OptimizationSettings = Default::default();
-        settings.verbose = 2;
-        settings.log_simplifications = true;
+        let settings = OptimizationSettings {
+            verbose: 2,
+            log_simplifications: true,
+            ..Default::default()
+        };
         let mut context = OptimizationContext::new_settings(settings);
         for circuit in circuits {
             let _result = optimize_circuit(circuit, &mut context);
             println!("{}", context.stringify_logs());
             // println!("{:?}", result.info().hash);
         }
     }
```

### Comparing `rust_circuit-0.4.8/tests/tests.rs` & `rust_circuit-0.4.9/tests/tests.rs`

 * *Files identical despite different names*

