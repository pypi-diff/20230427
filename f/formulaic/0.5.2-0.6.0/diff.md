# Comparing `tmp/formulaic-0.5.2.tar.gz` & `tmp/formulaic-0.6.0.tar.gz`

## Comparing `formulaic-0.5.2.tar` & `formulaic-0.6.0.tar`

### file list

```diff
@@ -1,122 +1,131 @@
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.5.2/benchmarks/README.md
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.5.2/benchmarks/benchmark.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.5.2/benchmarks/benchmarks.csv
--rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.5.2/benchmarks/benchmarks.png
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.5.2/benchmarks/plot.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.5.2/benchmarks/requirements.txt
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/mkdocs.yml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/requirements.in
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/requirements.txt
--rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/changelog.md
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/index.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/installation.md
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/assets/images/logo.png
--rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/assets/images/logo.svg
--rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/assets/images/logo_with_text.png
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/concepts/formulas.md
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/concepts/grammar.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/concepts/index.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/guides/advanced.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/guides/index.md
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/guides/quickstart.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/reference/api.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/docsite/docs/reference/index.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/_version.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/errors.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/formula.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/model_matrix.py
--rw-r--r--   0        0        0    15527 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/model_spec.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/sugar.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/arrow.py
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/base.py
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/pandas.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/types/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/types/enums.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/types/evaluated_factor.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/types/factor_values.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/types/scoped_factor.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/materializers/types/scoped_term.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/__init__.py
--rw-r--r--   0        0        0     9455 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/parser.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/utils.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/algos/__init__.py
--rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/algos/tokenize.py
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/algos/tokens_to_ast.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/ast_node.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/factor.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/formula_parser.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/operator.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/operator_resolver.py
--rw-r--r--   0        0        0    13264 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/structured.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/term.py
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/parser/types/token.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/transforms/__init__.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/transforms/basis_spline.py
--rw-r--r--   0        0        0    23343 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/transforms/contrasts.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/transforms/identity.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/transforms/poly.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/transforms/scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/__init__.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/calculus.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/cast.py
--rw-r--r--   0        0        0    17000 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/constraints.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/context.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/iterators.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/layered_mapping.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/sentinels.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/sparse.py
--rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 formulaic-0.5.2/formulaic/utils/stateful_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/test_formula.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/test_model_matrix.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/test_model_spec.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/test_sugar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/__init__.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/test_arrow.py
--rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/test_base.py
--rw-r--r--   0        0        0    13822 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/test_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/types/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/types/test_evaluated_factor.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/types/test_factor_values.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/types/test_scoped_factor.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/materializers/types/test_scoped_term.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/__init__.py
--rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/test_parser.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/algos/__init__.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/algos/test_tokenize.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/algos/test_tokens_to_ast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_ast_node.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_factor.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_formula_parser.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_operator.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_operator_resolver.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_structured.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_term.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/parser/types/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/transforms/__init__.py
--rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/transforms/test_basis_spline.py
--rw-r--r--   0        0        0    26964 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/transforms/test_contrasts.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/transforms/test_identity.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/transforms/test_poly.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/transforms/test_scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_calculus.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_capture_context.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_cast.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_constraints.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_iterators.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_layered_mapping.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_sentinels.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_sparse.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.5.2/tests/utils/test_stateful_transforms.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.5.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.5.2/LICENSE
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 formulaic-0.5.2/README.md
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 formulaic-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 formulaic-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/README.md
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/benchmark.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/benchmarks.csv
+-rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/benchmarks.png
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/plot.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.0/benchmarks/requirements.txt
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/mkdocs.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/requirements.in
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/requirements.txt
+-rw-r--r--   0        0        0    16311 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/changelog.md
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/formulas.md
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/index.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/installation.md
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/migration.md
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/assets/images/logo_with_text.png
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/concepts/index.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/dev/index.md
+-rw-r--r--   0        0        0    46139 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/contrasts.ipynb
+-rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/formulae.ipynb
+-rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/grammar.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/index.md
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/integration.ipynb
+-rw-r--r--   0        0        0    27260 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/model_specs.ipynb
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/quickstart.ipynb
+-rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/splines.ipynb
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.0/docsite/docs/guides/transforms.ipynb
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/_version.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/errors.py
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/formula.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/model_matrix.py
+-rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/model_spec.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/sugar.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/__init__.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/arrow.py
+-rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/base.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/pandas.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/enums.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/evaluated_factor.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/factor_values.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/scoped_factor.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/materializers/types/scoped_term.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/__init__.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/parser.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/utils.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/algos/__init__.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/algos/tokenize.py
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/algos/tokens_to_ast.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/__init__.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/ast_node.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/factor.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/formula_parser.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/operator.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/operator_resolver.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/ordered_set.py
+-rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/structured.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/term.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/parser/types/token.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/__init__.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/basis_spline.py
+-rw-r--r--   0        0        0    25319 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/contrasts.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/identity.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/patsy_compat.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/poly.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/transforms/scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/__init__.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/calculus.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/cast.py
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/constraints.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/context.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/iterators.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/layered_mapping.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/sentinels.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/sparse.py
+-rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.0/formulaic/utils/stateful_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_formula.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_model_matrix.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_model_spec.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/test_sugar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/__init__.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/test_arrow.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/test_base.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/test_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_evaluated_factor.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_factor_values.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_scoped_factor.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/materializers/types/test_scoped_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/test_parser.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/algos/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/algos/test_tokenize.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/algos/test_tokens_to_ast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_ast_node.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_factor.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_formula_parser.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_operator.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_operator_resolver.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_ordered_set.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_structured.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_term.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/parser/types/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/__init__.py
+-rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_basis_spline.py
+-rw-r--r--   0        0        0    28451 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_contrasts.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_identity.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_patsy_compat.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_poly.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/transforms/test_scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_calculus.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_capture_context.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_cast.py
+-rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_constraints.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_layered_mapping.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_sentinels.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_sparse.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.0/tests/utils/test_stateful_transforms.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.0/README.md
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 formulaic-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 formulaic-0.6.0/PKG-INFO
```

### Comparing `formulaic-0.5.2/benchmarks/README.md` & `formulaic-0.6.0/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/benchmarks/benchmark.py` & `formulaic-0.6.0/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/benchmarks/benchmarks.csv` & `formulaic-0.6.0/benchmarks/benchmarks.csv`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/benchmarks/benchmarks.png` & `formulaic-0.6.0/benchmarks/benchmarks.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/benchmarks/plot.py` & `formulaic-0.6.0/benchmarks/plot.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/docsite/docs/changelog.md` & `formulaic-0.6.0/docsite/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,63 @@
 For changes since the latest tagged release, please refer to the
 [git commit log](https://github.com/matthewwardrop/formulaic/commits/main).
 
 ---
 
+## 0.6.0 (26 Apr 2023)
+
+This is a major release with some important consistency and completeness
+improvements. It should be treated as *almost* being the first release candidate
+of 1.0.0, which will land after some small amount of further feature extensions
+and documentation improvements. All users are recommended to upgrade.
+
+**Breaking changes:**
+
+Although there are some internal changes to API, as documented below, there are
+no breaking changes to user-facing APIs.
+
+**New features and enhancements:**
+
+* Formula terms are now consistently ordered regardless of providence (formulae or
+  manual term specification), and sorted according to R conventions by default
+  rather than lexically. This can be changed using the `_ordering` keyword to
+  the `Formula` constructor.
+* Greater compatibility with R and patsy formulae:
+  * for patsy: added `standardize`, `Q` and treatment contrasts shims.
+  * for patsy: added `cluster_by='numerical_factors` option to `ModelSpec` to enable
+    patsy style clustering of output columns by involved numerical factors.
+  * for R: added support for exponentiation with `^` and `%in%`.
+* Diff and Helmert contrast codings gained support for additional variants.
+* Greatly improved the performance of generating sparse dummy encodings when
+  there are many categories.
+* Context scoping operators (like paretheses) are now tokenized as their own special
+  type.
+* Add support for merging `Structured` instances, and use this functionality during
+  AST evaluation where relevant.
+* `ModelSpec.term_indices` is now a list rather than a tuple, to allow direct use when
+  indexing pandas and numpy model matrices.
+* Add official support for Python 3.11.
+
+**Bugfixes and cleanups:**
+
+* Fix parsing formulae starting with a parenthesis.
+* Fix iteration over root nodes of `Structured` instances for non-sequential iterable values.
+* Bump testing versions and fix `poly` unit tests.
+* Fix use of deprecated automatic casting of factors to numpy arrays during dense
+  column evaluation in `PandasMaterializer`.
+* `Factor.EvalMethod.UNKNOWN` was removed, defaulting instead to `LOOKUP`.
+* Remove `sympy` version constraint now that a bug has been fixed upstream.
+
+**Documentation:**
+
+* Substantial updates to documentation, which is now mostly complete for end-user
+  use-cases. Developer and API docs are still pending.
+
+---
+
 ## 0.5.2 (17 Sep 2022)
 
 This is a minor patch releases that fixes one bug.
 
 **Bugfixes and cleanups:**
 
 * Fixed alignment between the length of a `Structured` instance and iteration
```

### Comparing `formulaic-0.5.2/docsite/docs/index.md` & `formulaic-0.6.0/docsite/docs/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 <img src="assets/images/logo_with_text.png" style="max-width: 600px">
 
-!!! warning
-    This documentation is a work in process, and is far from complete.
-
 Formulaic is a high-performance implementation of Wilkinson formulas for Python,
 which are very useful for transforming dataframes into a form suitable for
 ingestion into various modelling frameworks (especially linear regression).
 
-- **Source Code**: https://github.com/matthewwardrop/formulaic
-- **Issue tracker**: https://github.com/matthewwardrop/formulaic/issues
+- **Source Code**: [https://github.com/matthewwardrop/formulaic](https://github.com/matthewwardrop/formulaic)
+- **Issue tracker**: [https://github.com/matthewwardrop/formulaic/issues](https://github.com/matthewwardrop/formulaic/issues)
+
+!!! note
+    This documentation is a work in process, and is far from complete. This
+    documentation is currently a scaffold, and more documentation is being added
+    over time. In the mean time, please feel free to reach out via the issue
+    tracker if you have any questions.
 
 !!! warning
     While this project is now fully functional, the API is still subject to
     change between major versions (`0.<major>.<minor>`) as we continue to
     improve things. If you are going to depend on it in another project, it is
     advisable to pin formulaic to within a major version, for example:
-    `formulaic>=0.1.0,<0.2`.
+    `formulaic>=0.5.0,<0.6`.
 
 It provides:
 
 - high-performance dataframe to model-matrix conversions.
 - support for reusing the encoding choices made during conversion of one data-set on other datasets.
 - extensible formula parsing.
 - extensible data input/output plugins, with implementations for:
@@ -29,10 +32,7 @@
   - output:
     - `pandas.DataFrame`
     - `numpy.ndarray`
     - `scipy.sparse.CSCMatrix`
 - support for symbolic differentiation of formulas (and hence model matrices).
 
 with more to come!
-
-For some examples of what Formulaic provides, and how to use it, please refer to
-the [Concepts](concepts/) and [User Guides](guides) documentation.
```

### Comparing `formulaic-0.5.2/docsite/docs/installation.md` & `formulaic-0.6.0/docsite/docs/installation.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/docsite/docs/assets/images/favicon.png` & `formulaic-0.6.0/docsite/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/docsite/docs/assets/images/logo.png` & `formulaic-0.6.0/docsite/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/docsite/docs/assets/images/logo.svg` & `formulaic-0.6.0/docsite/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/docsite/docs/assets/images/logo_with_text.png` & `formulaic-0.6.0/docsite/docs/assets/images/logo_with_text.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/docsite/docs/concepts/formulas.md` & `formulaic-0.6.0/docsite/docs/formulas.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 This section introduces the basic notions and origins of formulas. If you are
 already familiar with formulas from another context, you might want to skip
-forward to the [Formula Grammer](grammar.md) or [User Guides](../guides/).
+forward to the [Formula Grammar](grammar.md) or [User Guides](../guides/).
 
 ## Origins
 
 Formulas were originally proposed by Wilkinson et al.[^1] to aid in the
 description of ANOVA problems, but were popularised by the S language (and then
 [R](http://search.r-project.org/R/library/stats/html/formula.html), as an
 implementation of S) in the context of linear regression. Since then they have
```

### Comparing `formulaic-0.5.2/docsite/docs/concepts/grammar.md` & `formulaic-0.6.0/docsite/docs/guides/grammar.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 | `` `...` ``[^1] | 1 | Quotes fieldnames within the incoming dataframe, allowing the use of special characters, e.g. `` `my|special$column!` `` | ✓ | ✗ | ✓ |
 | `{...}`[^1] | 1 | Quotes python operations, as a more convenient way to do Python operations than `I(...)`, e.g. `` {`my|col`**2} `` | ✓ | ✗ | ✗ |
 | `<function>(...)`[^1] | 1 | Python transform on column, e.g. `my_func(x)` which is equivalent to `{my_func(x)}` | ✓[^2] | ✓ | ✗ |
 |-----|
 | `(...)` | 1 | Groups operations, overriding normal precedence rules. All operations with the parentheses are performed before the result of these operations is permitted to be operated upon by its peers. | ✓ | ✓ | ✓ |
 |-----|
 | ** | 2 | Includes all n-th order interactions of the terms in the left operand, where n is the (integral) value of the right operand, e.g. `(a+b+c)**2` is equivalent to `a + b + c + a:b + a:c + b:c`. | ✓ | ✓ | ✓ |
-| ^ | 2 | Alias for `**`. | ✗ | ✗[^3] | ✓ |
+| ^ | 2 | Alias for `**`. | ✓ | ✗[^3] | ✓ |
 |-----|
 | `:` | 2 | Adds a new term that corresponds to the interaction of its operands (i.e. their elementwise product). | ✓ | ✓ | ✓ |
 |-----|
 | `*` | 2 | Includes terms for each of the additive and interactive effects of the left and right operands, e.g. `a * b` is equivalent to `a + b + a:b`. | ✓ | ✓ | ✓ |
 | `/` | 2 | Adds terms describing nested effects. It expands to the addition of a new term for the left operand and the interaction of all left operand terms with the right operand, i.e `a / b` is equivalent to `a + a:b`, `(a + b) / c` is equivalent to `a + b + a:b:c`, and `a/(b+c)` is equivalent to `a + a:b + a:c`.[^4] | ✓ | ✓ | ✓ |
-| `%in%` | 2 | Alias for `/`. | ✗ | ✗ | ✓ |
+| `%in%` | 2 | As above, but with arguments inverted: e.g. `b %in% a` is equivalent to `a / b`. | ✓ | ✗ | ✓ |
 |-----|
 | `+` | 2 | Adds a new term to the set of features. | ✓ | ✓ | ✓ |
 | `-` | 2 | Removes a term from the set of features (if present). | ✓ | ✓ | ✓ |
 | `+` | 1 | Returns the current term unmodified (not very useful). | ✓ | ✓ | ✓ |
 | `-` | 1 | Negates a term (only implemented for 0, in which case it is replaced with `1`). | ✓ | ✓ | ✓ |
 |-----|
 | `|` | 2 | Splits a formula into multiple parts, allowing the simultaneous generation of multiple model matrices. When on the right-hand-side of the `~` operator, all parts will attract an additional intercept term by default. | ✓ | ✗ | ✓[^5] |
@@ -48,23 +48,24 @@
 
 
 ## Transforms
 
 Formulaic supports arbitrary transforms, any of which can also preserve state so
 that new data can undergo the same transformation as that used during modelling.
 The currently implemented transforms are shown below. Commonly used transforms
-that have *not* been implemented by `formualaic` are explicitly noted also.
+that have *not* been implemented by `formulaic` are explicitly noted also.
 
 | Transform | Description | Formulaic | Patsy | R |
 |----------:|:------------|:---------:|:-----:|:-:|
 | `I(...)` | Identity transform, allowing arbitrary Python/R operations, e.g. `I(x+y)`. Note that in `formulaic`, it is more idiomatic to use `{x+y}`. | ✓ | ✓ | ✓ |
+| `Q('<column_name>')` | Look up feature by potentially exotic name, e.g. `Q('wacky name!')`. Note that in `formulaic`, it is more idiomatic to use ``` `wacky name!` ```. | ✓ | ✓ | ✗ |
 | `C(...)` | Categorically encode a column, e.g. `C(x)` | ✓ | ✓ | ✓ |
 | `center(...)` | Shift column data so mean is zero. | ✓ | ✓ | ✗ |
 | `scale(...)` | Shift column so mean is zero and variance is 1. | ✓ | ✓[^6] | ✓ |
-| `standardize(...)` | Alias of `scale`. | ✗ | ✓ | ✗ |
+| `standardize(...)` | Alias of `scale`. | ✓[^7] | ✓ | ✗ |
 | `poly(...)` | Generates a polynomial basis, allowing non-linear fits. | ✓ | ✗ | ✓ |
 | `bs(...)` | Generates a B-Spline basis, allowing non-linear fits. | ✓ | ✓ | ✓ |
 | `cr(...)` | Generates a natural cubic spline basis, allowing non-linear fits. | ✗ | ✓ | ✓ |
 | `cc(...)` | Generates a cyclic cubic spline basis, allowing non-linear fits. | ✗ | ✓ | ✓ |
 | `te(...)` | Generates a tensor product smooth. | ✗ | ✓ | ✓ |
 | ...       | Others? Contributions welcome!     | ? | ? | ? |
 
@@ -114,7 +115,8 @@
 
 [^1]: This "operator" is actually part of the tokenisation process.
 [^2]: Formulaic additionally supports quoted fields with special characters, e.g. `` my_func(`my|special+column`) ``.
 [^3]: The caret operator is not supported, but will not cause an error. It is ignored by the patsy formula parser, and treated as XOR Python operation on column.
 [^4]: This somewhat confusing operator is useful when you want to include hierachical features in your data, and where certain interaction terms do not make sense (particularly in ANOVA contexts). For example, if `a` represents countries, and `b` represents cities, then the full product of terms from `a * b === a + b + a:b` does not make sense, because any value of `b` is guaranteed to coincide with a value in `a`, and does not independently add value. Thus, the operation `a / b === a + a:b` results in more sensible dataset. As a result, the `/` operator is right-distributive, since if `b` and `c` were both nested in `a`, you would want `a/(b+c) === a + a:b + a:c`. Likewise, the operator is not left-distributive, since if `c` is nested under both `a` and `b` separately, then you want `(a + b)/c === a + b + a:b:c`. Lastly, if `c` is nested in `b`, and `b` is nested in `a`, then you would want `a/b/c === a + a:(b/c) === a + a:b + a:b:c`.
 [^5]: Implemented by an R package called [Formula](https://cran.r-project.org/web/packages/Formula/index.html) that extends the default formula syntax.
 [^6]: Patsy uses the `rescale` keyword rather than `scale`, but provides the same functionality.
+[^7]: For increased compatibility with patsy, we use patsy's signature for `standardize`.
```

### Comparing `formulaic-0.5.2/docsite/docs/concepts/index.md` & `formulaic-0.6.0/docsite/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/__init__.py` & `formulaic-0.6.0/formulaic/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/errors.py` & `formulaic-0.6.0/formulaic/errors.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/formula.py` & `formulaic-0.6.0/formulaic/formula.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 from __future__ import annotations
 
 import warnings
+from enum import Enum
 from typing import Any, Dict, List, Mapping, Optional, Set, Tuple, Union
 
 from typing_extensions import TypeAlias
 
 from .errors import FormulaInvalidError
 from .model_matrix import ModelMatrix
 from .parser import DefaultFormulaParser
-from .parser.types import FormulaParser, Structured, Term
+from .parser.types import FormulaParser, OrderedSet, Structured, Term
 from .utils.calculus import differentiate_term
 
 
 FormulaSpec: TypeAlias = Union[
     str,
     List[Union[str, Term]],
     Set[Union[str, Term]],
     Structured[Union[str, List[Term], Set[Term]]],
     "Formula",  # Direct formula specification
     Dict[str, "FormulaSpec"],
     Tuple["FormulaSpec", ...],  # Structured formulae
 ]
 
 
+class OrderingMethod(Enum):
+    NONE = "none"
+    DEGREE = "degree"
+    SORT = "sort"
+
+
 class Formula(Structured[List[Term]]):
     """
     A Formula is a (potentially structured) list of terms, which is represented
     by this class.
 
     This is a thin wrapper around `Strucuted[List[Term]]` that adds convenience
     methods for building model matrices from the formula (among other common
@@ -67,27 +74,31 @@
             formulae (vs. individual terms). If not specified,
             `DefaultFormulaParser()` is used.
         _nested_parser: The `FormulaParser` instance to use when parsing
             strings describing nested or individual terms (e.g. when `spec` is a
             list of string term identifiers). If not specified and `_parser` is
             specified, `_parser` is used; if `_parser` is not specified,
             `DefaultFormulaParser(include_intercept=False)` is used instead.
+        _ordering: The ordering method to apply to the terms implied by the
+            formula `spec`. Can be: "none", "degree" (default), or "sort".
     """
 
     DEFAULT_PARSER = DefaultFormulaParser()
     DEFAULT_NESTED_PARSER = DefaultFormulaParser(include_intercept=False)
 
-    __slots__ = ("_parser", "_nested_parser")
+    __slots__ = ("_parser", "_nested_parser", "_ordering")
 
     @classmethod
     def from_spec(
         cls,
         spec: FormulaSpec,
+        *,
         parser: Optional[FormulaParser] = None,
         nested_parser: Optional[FormulaParser] = None,
+        ordering: Union[OrderingMethod, str] = OrderingMethod.DEGREE,
     ) -> Formula:
         """
         Construct a `Formula` instance from a formula specification.
 
         Args:
             spec: The formula specification.
             parser: The `FormulaParser` instance to use when parsing complete
@@ -95,28 +106,34 @@
                 `DefaultFormulaParser()` is used.
             nested_parser: The `FormulaParser` instance to use when parsing
                 strings describing nested or individual terms (e.g. when `spec`
                 is a list of string term identifiers). If not specified and
                 `parser` is specified, `parser` is used; if `parser` is not
                 specified, `DefaultFormulaParser(include_intercept=False)` is
                 used instead.
+            ordering: The ordering method to apply to the terms implied by the
+                formula `spec`. Can be: "none", "degree" (default), or "sort".
         """
         if isinstance(spec, Formula):
             return spec
-        return Formula(spec, _parser=parser, _nested_parser=nested_parser)
+        return Formula(
+            spec, _parser=parser, _nested_parser=nested_parser, _ordering=ordering
+        )
 
     def __init__(
         self,
         *args,
         _parser: Optional[FormulaParser] = None,
         _nested_parser: Optional[FormulaParser] = None,
+        _ordering: Union[OrderingMethod, str] = OrderingMethod.DEGREE,
         **kwargs,
     ):
         self._parser = _parser or self.DEFAULT_PARSER
         self._nested_parser = _nested_parser or _parser or self.DEFAULT_NESTED_PARSER
+        self._ordering = OrderingMethod(_ordering)
         super().__init__(*args, **kwargs)
         self._simplify(unwrap=False, inplace=True)
 
     def _prepare_item(self, key: str, item: FormulaSpec) -> Union[List[Term], Formula]:
         """
         Convert incoming formula items into either a list of Terms or a nested
         `Formula` instance.
@@ -128,53 +145,64 @@
             key: The structural key where the item will be stored.
             item: The specification to convert.
         """
 
         if isinstance(item, str):
             item = (
                 (self._parser if key == "root" else self._nested_parser)
-                .get_terms(item, sort=True)
+                .get_terms(item)
                 ._simplify()
             )
 
         if isinstance(item, Structured):
-            formula_or_terms = Formula(_parser=self._nested_parser, **item._structure)
-        elif isinstance(item, (list, set)):
+            formula_or_terms = Formula(
+                _parser=self._nested_parser, **item._structure
+            )._simplify()
+        elif isinstance(item, (list, set, OrderedSet)):
             formula_or_terms = [
                 term
                 for value in item
                 for term in (
                     self._nested_parser.get_terms(value)
                     if isinstance(value, str)
                     else [value]
                 )
             ]
+            self.__validate_terms(formula_or_terms)
         else:
             raise FormulaInvalidError(
                 f"Unrecognized formula specification: {repr(item)}."
             )
 
-        self.__validate_prepared_item(formula_or_terms)
+        # Order terms appropriately
+        orderer = None
+        if self._ordering is OrderingMethod.DEGREE:
+            orderer = lambda terms: sorted(terms, key=lambda term: len(term.factors))
+        elif self._ordering is OrderingMethod.SORT:
+            orderer = lambda terms: sorted(
+                [Term(factors=sorted(term.factors)) for term in terms]
+            )
+
+        if orderer is not None:
+            if isinstance(formula_or_terms, Structured):
+                formula_or_terms = formula_or_terms._map(orderer)
+            else:
+                formula_or_terms = orderer(formula_or_terms)
 
-        if isinstance(formula_or_terms, Structured):
-            formula_or_terms = formula_or_terms._simplify()
         return formula_or_terms
 
     @classmethod
-    def __validate_prepared_item(cls, formula_or_terms: Any):
+    def __validate_terms(cls, formula_or_terms: Any):
         """
         Verify that all terms are of the appropriate type. The acceptable types
         are:
             - List[Terms]
             - Tuple[List[Terms], ...]
             - Formula
         """
-        if isinstance(formula_or_terms, Formula):
-            formula_or_terms._map(cls.__validate_prepared_item)
-            return
         if not isinstance(formula_or_terms, list):
             # Should be impossible to reach this; here as a sentinel
             raise FormulaInvalidError(
                 f"All components of a formula should be lists of `Term` instances. Found: {repr(formula_or_terms)}."
             )
         for term in formula_or_terms:
             if not isinstance(term, Term):
```

### Comparing `formulaic-0.5.2/formulaic/model_matrix.py` & `formulaic-0.6.0/formulaic/model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/model_spec.py` & `formulaic-0.6.0/formulaic/model_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 from formulaic.materializers.base import EncodedTermStructure
 from formulaic.parser.types import Structured, Term
 from formulaic.utils.constraints import LinearConstraintSpec, LinearConstraints
 
 from .formula import Formula, FormulaSpec
-from .materializers import FormulaMaterializer, NAAction
+from .materializers import FormulaMaterializer, NAAction, ClusterBy
 
 if TYPE_CHECKING:  # pragma: no cover
     from .model_matrix import ModelMatrices, ModelMatrix
 
 # Cached property was introduced in Python 3.8 (we currently support 3.7)
 try:
     from functools import cached_property
@@ -47,17 +47,21 @@
                 generated.
             materializer: The materializer used (and/or to be used) to
                 materialize the formula into a matrix.
             ensure_full_rank: Whether to ensure that the generated matrix is
                 "structurally" full-rank (features are not included which are
                 known to violate full-rankness).
             na_action: The action to be taken if NA values are found in the
-                data. Can be on of: "drop" (the default), "raise" or "ignore".
+                data. Can be one of: "drop" (the default), "raise" or "ignore".
             output: The desired output type (as interpreted by the materializer;
                 e.g. "pandas", "sparse", etc).
+            cluster_by: How to cluster terms/columns during materialization. Can
+                be one of: "none" (the default) or "numerical_factors" (in which
+                case terms are clustered based on their sharing of the same
+                numerical factors; like patsy).
 
         State (these attributes are only populated during materialization):
             structure: The model matrix structure resulting from materialization.
             transform_state: The state of any stateful transformations that took
                 place during factor evaluation.
             encoder_state: The state of any stateful transformations that took
                 place during encoding.
@@ -99,14 +103,15 @@
     # Configuration attributes
     formula: Formula
     materializer: Optional[str] = None
     materializer_params: Optional[Dict[str, Any]] = None
     ensure_full_rank: bool = True
     na_action: NAAction = "drop"
     output: Optional[str] = None
+    cluster_by: ClusterBy = "none"
 
     # State attributes
     structure: Optional[List[EncodedTermStructure]] = None
     transform_state: Dict = field(default_factory=dict)
     encoder_state: Dict = field(default_factory=dict)
 
     def __post_init__(self):
@@ -120,14 +125,15 @@
         # Materializer
         if self.materializer is not None and not isinstance(self.materializer, str):
             self.__dict__["materializer"] = FormulaMaterializer.for_materializer(
                 self.materializer
             ).REGISTER_NAME
 
         self.__dict__["na_action"] = NAAction(self.na_action)
+        self.__dict__["cluster_by"] = ClusterBy(self.cluster_by)
 
     # Derived features
 
     @cached_property
     def column_names(self) -> Sequence[str]:
         """
         The names associated with the columns of the generated model matrix.
@@ -183,15 +189,15 @@
         up elements of this mapping using the string representation of the
         `Term`.
         """
         slices = OrderedDict()
         start = 0
         for row in self.structure:
             end = start + len(row[2])
-            slices[row[0]] = tuple(range(start, end))
+            slices[row[0]] = list(range(start, end))
             start = end
         return slices
 
     @cached_property
     def term_slices(self) -> OrderedDict[Term, slice]:
         """
         An ordered mapping of `Term` instances to a slice that when used on
```

### Comparing `formulaic-0.5.2/formulaic/sugar.py` & `formulaic-0.6.0/formulaic/sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/materializers/arrow.py` & `formulaic-0.6.0/formulaic/materializers/arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/materializers/base.py` & `formulaic-0.6.0/formulaic/materializers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 from collections import defaultdict, OrderedDict, namedtuple
 from typing import (
     Any,
     Dict,
     Generator,
     List,
     Iterable,
-    Set,
     Tuple,
     Union,
     TYPE_CHECKING,
 )
 
 from interface_meta import InterfaceMeta, inherit_docs
 
 from formulaic.errors import (
     FactorEncodingError,
     FactorEvaluationError,
     FormulaMaterializationError,
     FormulaMaterializerInvalidError,
     FormulaMaterializerNotFoundError,
 )
+from formulaic.materializers.types.enums import ClusterBy
 from formulaic.materializers.types.factor_values import FactorValuesMetadata
 from formulaic.model_matrix import ModelMatrices, ModelMatrix
 from formulaic.parser.types import Factor, Term
+from formulaic.parser.types.ordered_set import OrderedSet
 from formulaic.transforms import TRANSFORMS
 from formulaic.utils.cast import as_columns
 from formulaic.utils.layered_mapping import LayeredMapping
 from formulaic.utils.stateful_transforms import stateful_eval
 
 from .types import EvaluatedFactor, FactorValues, ScopedFactor, ScopedTerm
 
@@ -120,15 +121,17 @@
     def __init__(self, data, context=None, **params):
         self.data = data
         self.context = context or {}
         self.params = params
         self._init()
 
         self.layered_context = LayeredMapping(
-            self.data_context, self.context, TRANSFORMS
+            LayeredMapping(self.data_context, name="data"),
+            LayeredMapping(self.context, name="context"),
+            LayeredMapping(TRANSFORMS, name="transforms"),
         )
 
         self.factor_cache = {}
         self.encoded_cache = {}
 
     def _init(self):
         pass  # pragma: no cover
@@ -193,17 +196,24 @@
 
         if should_simplify:
             return model_matrices._simplify()
         return model_matrices
 
     def _build_model_matrix(self, spec: ModelSpec, drop_rows):
 
+        # Step 0: Apply any requested column/term clustering
+        # This must happen before Step 1 otherwise the greedy rank reduction
+        # below would result in a different outcome than if the columns had
+        # always been in the generated order.
+        terms = self._cluster_terms(spec.formula, cluster_by=spec.cluster_by)
+
         # Step 1: Determine strategy to maintain structural full-rankness of output matrix
         scoped_terms_for_terms = self._get_scoped_terms(
-            spec.formula, ensure_full_rank=spec.ensure_full_rank
+            terms,
+            ensure_full_rank=spec.ensure_full_rank,
         )
 
         # Step 2: Generate the columns which will be collated into the full matrix
         cols = []
         for term, scoped_terms in scoped_terms_for_terms:
             scoped_cols = OrderedDict()
             for scoped_term in scoped_terms:
@@ -219,15 +229,15 @@
                             [
                                 self._encode_evaled_factor(
                                     scoped_factor.factor,
                                     spec,
                                     drop_rows,
                                     reduced_rank=scoped_factor.reduced,
                                 )
-                                for scoped_factor in sorted(scoped_term.factors)
+                                for scoped_factor in scoped_term.factors
                             ],
                             spec=spec,
                             scale=scoped_term.scale,
                         )
                     )
             cols.append((term, scoped_terms, scoped_cols))
 
@@ -316,14 +326,31 @@
             formula=[],
             ensure_full_rank=next(iter(ensure_full_rank)),
             na_action=next(iter(na_action)),
             output=next(iter(output)),
             transform_state=transform_state,
         )
 
+    def _cluster_terms(self, terms, cluster_by: ClusterBy = ClusterBy.NONE):
+        if cluster_by is not ClusterBy.NUMERICAL_FACTORS:
+            return terms
+
+        term_clusters = defaultdict(list)
+        for term in terms:
+            numerical_factors = tuple(
+                factor
+                for factor in term.factors
+                if self.factor_cache[factor.expr].metadata.kind is Factor.Kind.NUMERICAL
+            )
+            term_clusters[numerical_factors].append(term)
+
+        return [
+            term for term_cluster in term_clusters.values() for term in term_cluster
+        ]
+
     # Methods related to ensuring out matrices are structurally full-rank
 
     def _get_scoped_terms(self, terms, ensure_full_rank=True):
         """
         Generate the terms to be used in the model matrix.
 
         This method first evaluates each factor in the context of the data
@@ -333,29 +360,28 @@
 
         Args:
             terms (list<Term>): A list of term arguments (usually from a formula)
                 object.
             ensure_full_rank (bool): Whether evaluated terms should be scoped
                 to ensure that their combination will result in a full-rank
                 matrix.
-            transform_state (dict): The state of any stateful transforms
-                (will be populated if empty).
 
         Returns:
             list<ScopedTerm>: A list of appropriately scoped terms.
         """
         spanned = set()
 
         for term in terms:
             evaled_factors = [self.factor_cache[factor.expr] for factor in term.factors]
 
             if ensure_full_rank:
-                term_span = self._get_scoped_terms_spanned_by_evaled_factors(
-                    evaled_factors
-                ).difference(spanned)
+                term_span = (
+                    self._get_scoped_terms_spanned_by_evaled_factors(evaled_factors)
+                    - spanned
+                )
                 scoped_terms = self._simplify_scoped_terms(term_span)
                 spanned.update(term_span)
             else:
                 scoped_terms = [
                     ScopedTerm(
                         factors=(
                             ScopedFactor(evaled_factor, reduced=False)
@@ -375,15 +401,15 @@
                     )
                 ]
             yield term, scoped_terms
 
     @classmethod
     def _get_scoped_terms_spanned_by_evaled_factors(
         cls, evaled_factors: Iterable[EvaluatedFactor]
-    ) -> Set[ScopedTerm]:
+    ) -> OrderedSet[ScopedTerm]:
         """
         Return the set of ScopedTerm instances which span the set of
         evaluated factors.
 
         Args:
             evaled_factors: The evaluated factors for which to generated scoped
                 terms.
@@ -393,46 +419,71 @@
         """
         scale = 1
         factors = []
         for factor in evaled_factors:
             if factor.metadata.kind is Factor.Kind.CONSTANT:
                 scale *= factor.values
             elif factor.metadata.spans_intercept:
-                factors.append((1, ScopedFactor(factor, reduced=True)))
+                factors.append((ScopedFactor(factor, reduced=True), 1))
             else:
                 factors.append((ScopedFactor(factor),))
-        return set(
+        return OrderedSet(
             ScopedTerm(factors=(p for p in prod if p != 1), scale=scale)
             for prod in itertools.product(*factors)
         )
 
     @classmethod
-    def _simplify_scoped_terms(cls, scoped_terms):
+    def _simplify_scoped_terms(
+        cls, scoped_terms: Iterable[ScopedTerm]
+    ) -> Iterable[ScopedTerm]:
         """
-        Return the minimal set of ScopedTerm instances that spans the same vectorspace.
+        Return the minimal set of ScopedTerm instances that spans the same
+        vectorspace, matching as closely as possible the intended order of the
+        terms.
+
+        This is an iterative algorithm that applies the rule:
+            (anything):(reduced rank) + (anything) |-> (anything):(full rank)
+        To be safe, we recurse whenever we apply the rule to make sure that
+        we have fully simplified the set of terms before adding new ones.
+
+        This is guaranteed to minimially span the vector space, keeping
+        everything full-rank by avoiding overlaps.
         """
-        terms = []
+        terms = OrderedSet()
         for scoped_term in sorted(scoped_terms, key=lambda x: len(x.factors)):
             factors = set(scoped_term.factors)
             combined = False
-            for co_scoped_term in terms:
-                cofactors = set(co_scoped_term.factors)
-                factors_diff = factors.difference(cofactors)
+            for existing_term in terms:
+                # Check whether existing term only differs by one factor
+                cofactors = set(existing_term.factors)
+                factors_diff = factors - cofactors
                 if len(factors) - 1 != len(cofactors) or len(factors_diff) != 1:
                     continue
+                # If the different factor is a reduced factor, we can apply the
+                # rule and recurse to see if there is anything else to pick up.
                 factor_new = next(iter(factors_diff))
                 if factor_new.reduced:
-                    co_scoped_term.factors += (
-                        ScopedFactor(factor_new.factor, reduced=False),
+                    terms = cls._simplify_scoped_terms(
+                        terms - (existing_term,)
+                        | (
+                            ScopedTerm(
+                                (
+                                    ScopedFactor(factor_new.factor, reduced=False)
+                                    if factor == factor_new
+                                    else factor
+                                    for factor in scoped_term.factors
+                                ),
+                                scale=existing_term.scale * scoped_term.scale,
+                            ),
+                        )
                     )
-                    terms = cls._simplify_scoped_terms(terms)
                     combined = True
                     break
             if not combined:
-                terms.append(scoped_term.copy())
+                terms = terms | (scoped_term,)
         return terms
 
     # Methods related to looking-up, evaluating and encoding terms and factors
 
     def _evaluate_factor(
         self, factor: Factor, spec: ModelSpec, drop_rows: set
     ) -> EvaluatedFactor:
@@ -443,19 +494,19 @@
                 elif factor.eval_method.value == "python":
                     value = self._evaluate(factor.expr, factor.metadata, spec)
                 elif factor.eval_method.value == "literal":
                     value = FactorValues(
                         self._evaluate(factor.expr, factor.metadata, spec),
                         kind=Factor.Kind.CONSTANT,
                     )
-                else:
+                else:  # pragma: no cover; future proofing against new eval methods
                     raise FactorEvaluationError(
                         f"The evaluation method `{factor.eval_method.value}` for factor `{factor}` is not understood."
                     )
-            except FactorEvaluationError:
+            except FactorEvaluationError:  # pragma: no cover; future proofing against new eval methods
                 raise
             except Exception as e:
                 raise FactorEvaluationError(
                     f"Unable to evaluate factor `{factor}`. [{type(e).__name__}: {e}]"
                 ) from e
 
             if not isinstance(value, FactorValues):
@@ -727,25 +778,30 @@
                 col: scoped_cols[col] for col in target_cols
             }
 
     def _get_columns_for_term(self, factors, spec, scale=1):
         """
         Assemble the columns for a model matrix given factors and a scale.
 
-        This performs the row-wise Kronecker product of the factors.
+        This performs the row-wise Kronecker product of the factors. For greater
+        compatibility with R and patsy, we reverse this product so that we
+        iterate first over the latter terms.
 
         Args:
             factors
             scale
 
         Returns:
             dict
         """
         out = OrderedDict()
-        for product in itertools.product(*(factor.items() for factor in factors)):
+        for reverse_product in itertools.product(
+            *(factor.items() for factor in reversed(factors))
+        ):
+            product = reverse_product[::-1]
             out[":".join(p[0] for p in product)] = scale * functools.reduce(
                 operator.mul, (p[1] for p in product)
             )
         return out
 
     @abstractmethod
     def _combine_columns(self, cols, spec, drop_rows):
```

### Comparing `formulaic-0.5.2/formulaic/materializers/pandas.py` & `formulaic-0.6.0/formulaic/materializers/pandas.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,14 +91,19 @@
             )
         )
 
     @override
     def _get_columns_for_term(self, factors, spec, scale=1):
         out = OrderedDict()
 
+        names = [
+            ":".join(reversed(product))
+            for product in itertools.product(*reversed(factors))
+        ]
+
         # Pre-multiply factors with only one set of values (improves performance)
         solo_factors = {}
         indices = []
         for i, factor in enumerate(factors):
             if len(factor) == 1:
                 solo_factors.update(factor)
                 indices.append(i)
@@ -114,28 +119,31 @@
                     }
                 )
             else:
                 factors.append(
                     {
                         ":".join(solo_factors): functools.reduce(
                             numpy.multiply,
-                            (p for p in solo_factors.values()),
+                            (numpy.asanyarray(p) for p in solo_factors.values()),
                         )
                     }
                 )
 
-        for product in itertools.product(*(factor.items() for factor in factors)):
+        for i, reversed_product in enumerate(
+            itertools.product(*(factor.items() for factor in reversed(factors)))
+        ):
             if spec.output == "sparse":
-                out[":".join(p[0] for p in product)] = scale * functools.reduce(
-                    spsparse.csc_matrix.multiply, (p[1] for p in product)
+                out[names[i]] = scale * functools.reduce(
+                    spsparse.csc_matrix.multiply,
+                    (p[1] for p in reversed(reversed_product)),
                 )
             else:
-                out[":".join(p[0] for p in product)] = scale * functools.reduce(
+                out[names[i]] = scale * functools.reduce(
                     numpy.multiply,
-                    (numpy.array(p[1]) for p in product),
+                    (numpy.array(p[1]) for p in reversed(reversed_product)),
                 )
         return out
 
     @override
     def _combine_columns(self, cols, spec, drop_rows):
         # If we are outputing a pandas DataFrame, explicitly override index
         # in case transforms/etc have lost track of it.
```

### Comparing `formulaic-0.5.2/formulaic/materializers/types/evaluated_factor.py` & `formulaic-0.6.0/formulaic/materializers/types/evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/materializers/types/factor_values.py` & `formulaic-0.6.0/formulaic/materializers/types/factor_values.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/materializers/types/scoped_factor.py` & `formulaic-0.6.0/formulaic/materializers/types/scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/materializers/types/scoped_term.py` & `formulaic-0.6.0/formulaic/materializers/types/scoped_term.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from .scoped_factor import ScopedFactor
 
 
 class ScopedTerm:
 
     __slots__ = ("factors", "scale")
 
-    def __init__(self, factors, scale=None):
-        self.factors = tuple(sorted(factors))
+    def __init__(self, factors, scale=1):
+        self.factors = tuple(dict.fromkeys(factors))
         self.scale = scale
 
     def __hash__(self):
-        return hash(self.factors)
+        return hash(tuple(sorted(self.factors)))
 
     def __eq__(self, other):
         if isinstance(other, ScopedTerm):
-            return self.factors == other.factors
+            return sorted(self.factors) == sorted(other.factors)
         return NotImplemented
 
     def __repr__(self):
         factor_repr = (
-            ":".join(f.__repr__() for f in sorted(self.factors))
-            if self.factors
-            else "1"
+            ":".join(f.__repr__() for f in self.factors) if self.factors else "1"
         )
         if self.scale is not None and self.scale != 1:
             return f"{self.scale}*{factor_repr}"
         return factor_repr
 
     def copy(self, *, without_values=False):
         factors = self.factors
```

### Comparing `formulaic-0.5.2/formulaic/parser/parser.py` & `formulaic-0.6.0/formulaic/parser/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import List, Iterable, Set, Tuple, Union
 
 from .algos.tokenize import tokenize
 from .types import (
     FormulaParser,
     Operator,
     OperatorResolver,
+    OrderedSet,
     Structured,
     Term,
     Token,
 )
 from .utils import (
     exc_for_token,
     insert_tokens_after,
@@ -137,76 +138,79 @@
                 if isinstance(termset, tuple):
                     out.extend(termset)
                 else:
                     out.append(termset)
             return tuple(out)
 
         def nested_product_expansion(
-            parents: Set[Term], nested: Set[Term]
-        ) -> Set[Term]:
+            parents: OrderedSet[Term], nested: OrderedSet[Term]
+        ) -> OrderedSet[Term]:
             common = functools.reduce(lambda x, y: x * y, parents)
-            return parents.union({common * term for term in nested})
+            return parents | OrderedSet(common * term for term in nested)
 
-        def power(arg: Set[Term], power: Set[Term]) -> Set[Term]:
+        def power(arg: OrderedSet[Term], power: OrderedSet[Term]) -> OrderedSet[Term]:
             power_term = next(iter(power))
             if (
                 not len(power_term.factors) == 1
                 or power_term.factors[0].token.kind is not Token.Kind.VALUE
                 or not isinstance(ast.literal_eval(power_term.factors[0].expr), int)
             ):
                 raise exc_for_token(
                     power_term.factors[0].token,
                     "The right-hand argument of `**` must be a positive integer.",
                 )
-            return {
+            return OrderedSet(
                 functools.reduce(lambda x, y: x * y, term)
                 for term in itertools.product(*[arg] * int(power_term.factors[0].expr))
-            }
+            )
 
         return [
             Operator(
                 "~",
                 arity=2,
                 precedence=-100,
                 associativity=None,
                 to_terms=lambda lhs, rhs: Structured(lhs=lhs, rhs=rhs),
                 accepts_context=lambda context: len(context) == 0,
+                structural=True,
             ),
             Operator(
                 "~",
                 arity=1,
                 precedence=-100,
                 associativity=None,
                 fixity="prefix",
                 to_terms=lambda terms: terms,
                 accepts_context=lambda context: len(context) == 0,
+                structural=True,
             ),
             Operator(
                 "|",
                 arity=2,
                 precedence=-50,
                 associativity=None,
                 to_terms=formula_part_expansion,
                 accepts_context=lambda context: all(
                     isinstance(c, Operator) and c.symbol in "~|" for c in context
                 ),
+                structural=True,
             ),
             Operator(
                 "+",
                 arity=2,
                 precedence=100,
                 associativity="left",
-                to_terms=lambda lhs, rhs: lhs.union(rhs),
+                to_terms=lambda lhs, rhs: lhs | rhs,
             ),
             Operator(
                 "-",
                 arity=2,
                 precedence=100,
                 associativity="left",
-                to_terms=lambda left, right: left.difference(right),
+                to_terms=lambda left, right: left - right,
             ),
             Operator(
                 "+",
                 arity=1,
                 precedence=100,
                 associativity="right",
                 fixity="prefix",
@@ -214,48 +218,61 @@
             ),
             Operator(
                 "-",
                 arity=1,
                 precedence=100,
                 associativity="right",
                 fixity="prefix",
-                to_terms=lambda terms: set(),
+                to_terms=lambda terms: OrderedSet(),
             ),
             Operator(
                 "*",
                 arity=2,
                 precedence=200,
                 associativity="left",
                 to_terms=lambda *term_sets: (
-                    {
+                    OrderedSet(itertools.chain(*term_sets))
+                    | OrderedSet(
                         functools.reduce(lambda x, y: x * y, term)
                         for term in itertools.product(*term_sets)
-                    }.union(itertools.chain(*term_sets))
+                    )
                 ),
             ),
             Operator(
                 "/",
                 arity=2,
                 precedence=200,
                 associativity="left",
                 to_terms=nested_product_expansion,
             ),
             Operator(
+                "in",
+                arity=2,
+                precedence=200,
+                associativity="left",
+                to_terms=lambda nested, parents: nested_product_expansion(
+                    parents, nested
+                ),
+            ),
+            Operator(
                 ":",
                 arity=2,
                 precedence=300,
                 associativity="left",
-                to_terms=lambda *term_sets: {
+                to_terms=lambda *term_sets: OrderedSet(
                     functools.reduce(lambda x, y: x * y, term)
                     for term in itertools.product(*term_sets)
-                },
+                ),
             ),
             Operator(
                 "**", arity=2, precedence=500, associativity="right", to_terms=power
             ),
+            Operator(
+                "^", arity=2, precedence=500, associativity="right", to_terms=power
+            ),
         ]
 
     def resolve(
         self, token: Token, max_prefix_arity: int, context: List[Union[Token, Operator]]
     ) -> Iterable[Operator]:
         if token.token in self.operator_table:
             return super().resolve(token, max_prefix_arity, context)
```

### Comparing `formulaic-0.5.2/formulaic/parser/utils.py` & `formulaic-0.6.0/formulaic/parser/utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/parser/algos/tokenize.py` & `formulaic-0.6.0/formulaic/parser/algos/tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       - name: a name of a feature/variable to be lifted from the model matrix
             context.
       - value: a literal value (string/number).
       - python: a code string to be evaluated.
 
     The basic logic of this tokenizer is to loop over each character in the
     formula string and:
-      - ensure that portions quoted by one of : ', ", {}, and ` are correctly
+      - ensure that portions quoted by one of : ', ", {}, %, and ` are correctly
         grouped into a token of the appropriate kind.
       - ignore unquoted whitespace
       - correctly distinguish users of (, ), [, and ] as grouping operators vs. Python
         function calls.
       - output each contiguous portion of the formula string that belongs to
         the same token type as a token. (e.g. sequential operators like '+-'
         will be output as a single operator token).
@@ -63,15 +63,15 @@
             token.update(char, i)
             take -= 1
             continue
         if quote_context and char == "\\":
             token.update(char, i)
             take = 1
             continue
-        if quote_context and quote_context[-1] in "}`" and char == quote_context[-1]:
+        if quote_context and quote_context[-1] in "}`%" and char == quote_context[-1]:
             quote_context.pop(-1)
             if token:
                 if quote_context:
                     token.update(char, i)
                 else:
                     yield token
                     token = Token(source=formula)
@@ -84,20 +84,26 @@
                 and not quote_context
                 and token.kind is Token.Kind.PYTHON
                 and char in ("]", ")")
             ):
                 yield token
                 token = Token(source=formula)
             continue
-        if quote_context and quote_context[-1] in ('"', "'", "`", ")", "}"):
+        if quote_context and quote_context[-1] in ('"', "'", "`", ")", "}", "%"):
             if char in "(`" and quote_context[-1] in "})":
                 quote_context.append(char.replace("(", ")"))
             token.update(char, i)
             continue
 
+        if char == "%":
+            if token:
+                yield token
+            token = Token(source=formula, kind="operator", source_start=i)
+            quote_context.append("%")
+            continue
         if char == "{":
             if token:
                 yield token
             token = Token(source=formula, kind="python", source_start=i)
             quote_context.append("}")
             continue
         if char == "`":
@@ -110,21 +116,21 @@
             if token.kind in (Token.Kind.NAME, Token.Kind.PYTHON):
                 token.update(char, i, kind=Token.Kind.PYTHON)
                 quote_context.append(")" if char == "(" else "]")
             else:
                 if token:
                     yield token
                     token = Token(source=formula)
-                yield Token(source=formula).update(char, i, kind="operator")
+                yield Token(source=formula).update(char, i, kind="context")
             continue
-        if char in ")":
+        if char in ")]":
             if token:
                 yield token
                 token = Token(source=formula)
-            yield Token(source=formula).update(char, i, kind="operator")
+            yield Token(source=formula).update(char, i, kind="context")
             continue
 
         if whitespace_chars.match(char):
             if token and token.kind is not Token.Kind.OPERATOR:
                 yield token
                 token = Token(source=formula)
             continue
```

### Comparing `formulaic-0.5.2/formulaic/parser/algos/tokens_to_ast.py` & `formulaic-0.6.0/formulaic/parser/algos/tokens_to_ast.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from typing import Iterable, Optional
 
 from ..types import ASTNode, Operator, OperatorResolver, Token
 from ..utils import exc_for_token, exc_for_missing_operator
 
 
 OrderedOperator = namedtuple("OrderedOperator", ("operator", "token", "index"))
+CONTEXT_OPENERS = {"(", "["}
+CONTEXT_CLOSERS = {
+    ")": "(",
+    "]": "[",
+}
 
 
 def tokens_to_ast(
     tokens: Iterable[Token], operator_resolver: OperatorResolver
 ) -> Optional[ASTNode]:
     """
     Convert a iterable of `Token` instances into an abstract syntax tree.
@@ -65,58 +70,65 @@
         return [
             *output_queue[:min_index],
             ASTNode(operator, output_queue[min_index:max_index]),
             *output_queue[max_index:],
         ]
 
     for token in tokens:
-        if token.kind is not token.Kind.OPERATOR:
-            output_queue.append(token)
-        else:
-            if token.token == "(":
+        if token.kind is token.Kind.CONTEXT:
+            if token.token in CONTEXT_OPENERS:
                 stack_operator(token, token)
-            elif token.token == ")":
-                while operator_stack and operator_stack[-1].token != "(":
+            elif token.token in CONTEXT_CLOSERS:
+                starting_token = CONTEXT_CLOSERS[token.token]
+                while operator_stack and operator_stack[-1].token != starting_token:
                     output_queue = operate(operator_stack.pop(), output_queue)
-                if operator_stack and operator_stack[-1].token == "(":
+                if operator_stack and operator_stack[-1].token == starting_token:
                     operator_stack.pop()
                 else:
-                    raise exc_for_token(token, "Could not find matching parenthesis.")
-            else:
-                max_prefix_arity = (
-                    len(output_queue) - operator_stack[-1].index
-                    if operator_stack
-                    else len(output_queue)
-                )
-                operators = operator_resolver.resolve(
+                    raise exc_for_token(
+                        token, "Could not find matching context marker."
+                    )
+            else:  # pragma: no cover
+                raise exc_for_token(
                     token,
-                    max_prefix_arity=max_prefix_arity,
-                    context=[s.operator for s in operator_stack],
+                    f"Context token `{token.token}` is unrecognized.",
                 )
+        elif token.kind is token.Kind.OPERATOR:
+            max_prefix_arity = (
+                len(output_queue) - operator_stack[-1].index
+                if operator_stack
+                else len(output_queue)
+            )
+            operators = operator_resolver.resolve(
+                token,
+                max_prefix_arity=max_prefix_arity,
+                context=[s.operator for s in operator_stack],
+            )
 
-                for operator in operators:
+            for operator in operators:
 
-                    while (
-                        operator_stack
-                        and (operator_stack[-1].token != "(")
-                        and (
-                            operator_stack[-1].operator.precedence > operator.precedence
-                            or operator_stack[-1].operator.precedence
-                            == operator.precedence
-                            and operator.associativity is Operator.Associativity.LEFT
-                        )
-                    ):
-                        output_queue = operate(operator_stack.pop(), output_queue)
+                while (
+                    operator_stack
+                    and operator_stack[-1].token.kind is not Token.Kind.CONTEXT
+                    and (
+                        operator_stack[-1].operator.precedence > operator.precedence
+                        or operator_stack[-1].operator.precedence == operator.precedence
+                        and operator.associativity is Operator.Associativity.LEFT
+                    )
+                ):
+                    output_queue = operate(operator_stack.pop(), output_queue)
 
-                    stack_operator(operator, token)
+                stack_operator(operator, token)
+        else:
+            output_queue.append(token)
 
     while operator_stack:
-        if operator_stack[-1].token == "(":
+        if operator_stack[-1].token.kind is Token.Kind.CONTEXT:
             raise exc_for_token(
-                operator_stack[-1].token, "Could not find matching parenthesis."
+                operator_stack[-1].token, "Could not find matching context marker."
             )
         output_queue = operate(operator_stack.pop(), output_queue)
 
     if output_queue:
         if len(output_queue) > 1:
             raise exc_for_missing_operator(output_queue[0], output_queue[1])
         return output_queue[0]
```

### Comparing `formulaic-0.5.2/formulaic/parser/types/ast_node.py` & `formulaic-0.6.0/formulaic/parser/types/ast_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import graphlib
 from typing import Any, Dict, Iterable, List
 
 from .operator import Operator
+from .structured import Structured
 from .term import Term
 
 
 class ASTNode:
     """
     Represents a node in an Abstract Syntax Tree (AST).
 
@@ -36,20 +37,25 @@
         g = graphlib.TopologicalSorter(self.__generate_evaluation_graph())
         g.prepare()
 
         results = {}
 
         while g.is_active():
             for node in g.get_ready():
-                results[node] = node.operator.to_terms(
-                    *[
-                        (results[arg] if isinstance(arg, ASTNode) else arg.to_terms())
-                        for arg in node.args
-                    ]
+                node_args = (
+                    (results[arg] if isinstance(arg, ASTNode) else arg.to_terms())
+                    for arg in node.args
                 )
+                if node.operator.structural:
+                    results[node] = node.operator.to_terms(*node_args)
+                else:
+                    results[node] = Structured._merge(
+                        *node_args,
+                        merger=node.operator.to_terms,
+                    )
                 g.done(node)
 
         return results[self]
 
     def __repr__(self):
         try:
             return f"<ASTNode {self.operator}: {self.args}>"
```

### Comparing `formulaic-0.5.2/formulaic/parser/types/factor.py` & `formulaic-0.6.0/formulaic/parser/types/factor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Dict, Iterable, Optional, Union, TYPE_CHECKING
+from typing import Dict, Optional, Union, TYPE_CHECKING
 
+from .ordered_set import OrderedSet
 from .term import Term
 
 if TYPE_CHECKING:
     from .token import Token  # pragma: no cover
 
 
 class Factor:
@@ -28,15 +29,14 @@
         metadata: An additional (optional) dictionary of metadata (currently
             unused).
         token: The `Token` instance from which the the `Formula` object was
             created.
     """
 
     class EvalMethod(Enum):
-        UNKNOWN = "unknown"
         LITERAL = "literal"
         LOOKUP = "lookup"
         PYTHON = "python"
 
     class Kind(Enum):
         UNKNOWN = "unknown"
         CONSTANT = "constant"
@@ -62,15 +62,15 @@
 
     @property
     def eval_method(self) -> EvalMethod:
         return self._eval_method
 
     @eval_method.setter
     def eval_method(self, eval_method):
-        self._eval_method = Factor.EvalMethod(eval_method or "unknown")
+        self._eval_method = Factor.EvalMethod(eval_method or "lookup")
 
     @property
     def kind(self) -> Kind:
         return self._kind
 
     @kind.setter
     def kind(self, kind):
@@ -87,16 +87,16 @@
         return self.expr.__hash__()
 
     def __lt__(self, other):
         if isinstance(other, Factor):
             return self.expr < other.expr
         return NotImplemented
 
-    def to_terms(self) -> Iterable[Term]:
+    def to_terms(self) -> OrderedSet[Term]:
         """
         Convert this `Factor` instance into a `Term` instance, and expose it as
-        a single-element iterable.
+        a single-element ordered set.
         """
-        return {Term([self])}
+        return OrderedSet((Term([self]),))
 
     def __repr__(self):
         return self.expr
```

### Comparing `formulaic-0.5.2/formulaic/parser/types/formula_parser.py` & `formulaic-0.6.0/formulaic/parser/types/formula_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,25 @@
         from ..algos.tokens_to_ast import tokens_to_ast
 
         return tokens_to_ast(
             self.get_tokens(formula),
             operator_resolver=self.operator_resolver,
         )
 
-    def get_terms(self, formula: str, *, sort: bool = True) -> Structured[List[Term]]:
+    def get_terms(self, formula: str) -> Structured[List[Term]]:
         """
         Assemble the `Term` instances for a formula string. Depending on the
         operators involved, this may be an iterable of `Term` instances, or
         an iterable of iterables of `Term`s, etc.
 
         Args:
             formula: The formula for which an AST should be generated.
-            sort: Whether to sort the terms before returning them.
         """
         ast = self.get_ast(formula)
         if ast is None:
             return Structured([])
 
         terms = ast.to_terms()
         if not isinstance(terms, Structured):
             terms = Structured(terms)
 
-        if sort:
-            terms = terms._map(sorted)
-
         return terms
```

### Comparing `formulaic-0.5.2/formulaic/parser/types/operator.py` & `formulaic-0.6.0/formulaic/parser/types/operator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from enum import Enum
 from numbers import Number
 from typing import Callable, List, Iterable, Union
 
+from .ordered_set import OrderedSet
 from .term import Term
 from .token import Token
 
 
 class Operator:
     """
     Specification for how an operator in a formula string should behave.
@@ -29,14 +30,18 @@
             between its arguments (and there must be exactly two of them); and
             if 'postfix', the operator comes after its arguments.
         to_terms: A callable that maps the arguments pass to the operator to
             an iterable of `Term` instances.
         accepts_context: A callable that will receive a list of Operator and
             Token instances that describe the context in which the operator
             would be applied if this callable returns `True`.
+        structural: Whether this operator adds structure to the terms sets, in
+            which case `Structured._merge` will not be used in the
+            `ASTNode.to_terms()`, and the termsets will be directly passed to
+            `Operator.to_terms()`.
     """
 
     class Associativity(Enum):
         LEFT = "left"
         RIGHT = "right"
         NONE = "none"
 
@@ -51,22 +56,24 @@
         *,
         arity: int,
         precedence: Number,
         associativity: Union[str, Associativity] = "none",
         fixity: Union[str, Fixity] = "infix",
         to_terms: Callable[..., Iterable[Term]] = None,
         accepts_context: Callable[[List[Union[Token, Operator]]], bool] = None,
+        structural: bool = False,
     ):
         self.symbol = symbol
         self.arity = arity
         self.precedence = precedence
         self.associativity = associativity
         self.fixity = fixity
         self._to_terms = to_terms
         self._accepts_context = accepts_context
+        self.structural = structural
 
     @property
     def associativity(self):
         return self._associativity
 
     @associativity.setter
     def associativity(self, associativity):
@@ -76,15 +83,15 @@
     def fixity(self):
         return self._fixity
 
     @fixity.setter
     def fixity(self, fixity):
         self._fixity = Operator.Fixity(fixity)
 
-    def to_terms(self, *args):
+    def to_terms(self, *args) -> OrderedSet[Term]:
         if self._to_terms is None:
             raise RuntimeError(f"`to_terms` is not implemented for '{self.symbol}'.")
         return self._to_terms(*args)
 
     def accepts_context(self, context: List[Union[Token, Operator]]):
         if self._accepts_context:
             # We only need to pass on tokens and operators with precedence less
```

### Comparing `formulaic-0.5.2/formulaic/parser/types/operator_resolver.py` & `formulaic-0.6.0/formulaic/parser/types/operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/parser/types/structured.py` & `formulaic-0.6.0/formulaic/parser/types/structured.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
+import itertools
+from collections import defaultdict
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Generic,
+    Iterable,
     Optional,
-    Sequence,
+    Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 
 ItemType = TypeVar("ItemType")
@@ -296,14 +299,107 @@
                 **{
                     key: self.__prepare_item(key, item)
                     for key, item in structure.items()
                 },
             }
         )
 
+    @classmethod
+    def _merge(
+        cls,
+        *objects: Any,
+        merger: Callable[..., ItemType] = None,
+        _context: Tuple[str, ...] = (),
+    ) -> Union[ItemType, Structured[ItemType]]:
+        """
+        Merge arbitrarily many objects into a single `Structured` instance.
+
+        If any of `objects` are `Structured` or `tuple` instances, then all
+        `objects` will be treated as `Structured` instances (being upcast as
+        necessary) and then merged recursively; otherwise the objects will be
+        merged directly by `merger`.
+
+        Note: An empty set of objects will result in an empty `Structured`
+        instance being returned.
+
+        Args:
+            objects: A tuple of Structured instances (will be upcast to a
+                trivial `Structured` instance as necessary).
+            merger: A callable which takes as arguments two or more items which
+                are to be merged. If not provided, a basic fallback is provided
+                that knows how to merge lists, dictionaries and sets.
+            _context: A string representing the context of the merge. Intended
+                for internal use.
+        """
+        if merger is None:
+            merger = cls.__merger_default
+
+        # If objects are not specified, return an empty `Structured` instance.
+        if not objects:
+            return cls()
+
+        # Check for sequential (tuple) structures, and if so merge them and
+        # return them wrapped in a `Structured` instance.
+        all_tuples = all(isinstance(obj, tuple) for obj in objects)
+        any_tuples = any(isinstance(obj, tuple) for obj in objects)
+
+        if any_tuples and not all_tuples:
+            raise ValueError(
+                f"Substructures for `.{'.'.join(_context)}` are not aligned and cannot be merged."
+            )
+
+        if all_tuples:
+            merged = tuple(itertools.chain(*objects))
+            if _context:
+                # We are merging substructure of `Structured` instances (and don't need the class wrapper)
+                return merged
+            return cls(merged)
+
+        # Check whether all objects are not Structured instances (or tuples,
+        # already excluded by above). If so, just call `merger` on them
+        # directly.
+        if all(not isinstance(obj, Structured) for obj in objects):
+            return merger(*objects)
+
+        # Otherwise,iterate over objects, upcasting to `Structured` as necessary
+        # and recursively merge them by merging their structure dictionaries.
+        values_to_merge = defaultdict(list)
+
+        for obj in objects:
+            if isinstance(obj, Structured):
+                for key, value in obj._structure.items():
+                    values_to_merge[key].append(value)
+            else:
+                values_to_merge["root"].append(obj)
+
+        return cls(
+            **{
+                key: (
+                    cls._merge(*values, merger=merger, _context=_context + (key,))
+                    if len(values) > 1
+                    else values[0]
+                )
+                for key, values in values_to_merge.items()
+            }
+        )
+
+    @staticmethod
+    def __merger_default(*items):
+        if all(isinstance(item, list) for item in items):
+            return list(itertools.chain(*items))
+        if all(isinstance(item, set) for item in items):
+            return set.union(*items)
+        if all(isinstance(item, dict) for item in items):
+            return dict(itertools.chain(*(d.items() for d in items)))
+        raise NotImplementedError(
+            "The fallback `merger` for `Structured._merge` does not know how to "
+            f"merge objects of types {repr(tuple(type(item) for item in items))}. "
+            "Please specify `merger` explicitly."
+        )
+
     def __dir__(self):
         return super().__dir__() + list(self._structure)
 
     def __getattr__(self, attr):
         if attr.startswith("_"):
             raise AttributeError(attr)
         if attr in self._structure:
@@ -336,15 +432,15 @@
             raise KeyError(
                 "Substructure keys cannot start with an underscore. "
                 f"The invalid keys are: {set(key for key in self._structure if key.startswith('_'))}."
             )
         self._structure[key] = self.__prepare_item(key, value)
 
     def __iter__(self) -> Generator[Union[ItemType, Structured[ItemType]]]:
-        if self._has_root and not self._has_keys and isinstance(self.root, Sequence):
+        if self._has_root and not self._has_keys and isinstance(self.root, Iterable):
             yield from self.root
         else:
             if self._has_root:  # Always yield root first.
                 yield self.root
             for key, value in self._structure.items():
                 if key != "root":
                     yield value
```

### Comparing `formulaic-0.5.2/formulaic/parser/types/term.py` & `formulaic-0.6.0/formulaic/parser/types/term.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,39 +12,39 @@
     a formula is made up of a sum of terms.
 
     Attributes:
         factors: The set of factors to be multipled to form the term.
     """
 
     def __init__(self, factors: Iterable["Factor"]):
-        self.factors = tuple(sorted(set(factors)))
-        self._factor_exprs = tuple(factor.expr for factor in self.factors)
-        self._hash = hash(repr(self))
+        self.factors = tuple(dict.fromkeys(factors))
+        self._factor_key = tuple(factor.expr for factor in sorted(self.factors))
+        self._hash = hash(":".join(self._factor_key))
 
     # Transforms and comparisons
 
     def __mul__(self, other):
         if isinstance(other, Term):
             return Term([*self.factors, *other.factors])
         return NotImplemented
 
     def __hash__(self):
         return self._hash
 
     def __eq__(self, other):
         if isinstance(other, Term):
-            return self._factor_exprs == other._factor_exprs
+            return self._factor_key == other._factor_key
         if isinstance(other, str):
-            return repr(self) == other
+            return self._factor_key == tuple(sorted(other.split(":")))
         return NotImplemented
 
     def __lt__(self, other):
         if isinstance(other, Term):
             if len(self.factors) == len(other.factors):
                 return sorted(self.factors) < sorted(other.factors)
             if len(self.factors) < len(other.factors):
                 return True
             return False
         return NotImplemented
 
     def __repr__(self):
-        return ":".join(self._factor_exprs)
+        return ":".join(factor.expr for factor in self.factors)
```

### Comparing `formulaic-0.5.2/formulaic/parser/types/token.py` & `formulaic-0.6.0/formulaic/parser/types/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 import copy
 import re
 from enum import Enum
 from typing import Any, Iterable, Optional, Tuple, Union
 
+from .ordered_set import OrderedSet
 from .factor import Factor
 from .term import Term
 
 
 class Token:
     """
     The atomic unit into which formula strings are parsed.
 
     These tokens are intentionally very low-level, leaving interpretation and
     validation to higher-levels. As such, adding new operators/etc does not
     require any modification of this low-level code.
 
     The four kinds of token are:
+      - context: a token used to scope terms into a given context
       - operator: an operator to be applied to other surrounding tokens (will
             always consist of non-word characters).
       - name: a name of a feature/variable to be lifted from the model matrix
             context.
       - value: a literal value (string/number).
       - python: a code string to be evaluated.
 
@@ -35,14 +37,15 @@
             this token.
 
     Note: These attributes *should* all be present, but may not be fully
     populated if generated outside of the default `tokenize()` implementation.
     """
 
     class Kind(Enum):
+        CONTEXT = "context"
         OPERATOR = "operator"
         VALUE = "value"
         NAME = "name"
         PYTHON = "python"
 
     __slots__ = ("token", "_kind", "source", "source_start", "source_end")
 
@@ -131,22 +134,22 @@
         }
         return Factor(
             expr=self.token,
             eval_method=kind_to_eval_method[self.kind],
             token=self,
         )
 
-    def to_terms(self) -> Iterable[Term]:
+    def to_terms(self) -> OrderedSet[Term]:
         """
-        An iterable (set) of `Term` instances for this token. This will just be
+        An order set of `Term` instances for this token. This will just be
         an iterable with one `Term` having one `Factor` (that generated by
         `.to_factor()`). Operator tokens cannot be converted to an iterable of
         `Term`s.
         """
-        return {Term([self.to_factor()])}
+        return OrderedSet((Term([self.to_factor()]),))
 
     def flatten(self, str_args=False) -> Any:
         """
         Return this token (or if `str_args` is `True`, a string representation
         of this token).
 
         Args:
```

### Comparing `formulaic-0.5.2/formulaic/transforms/__init__.py` & `formulaic-0.6.0/formulaic/transforms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import numpy
 
+from formulaic.utils.stateful_transforms import stateful_transform
+
 from .basis_spline import basis_spline
 from .identity import identity
 from .contrasts import C, encode_contrasts, ContrastsRegistry
+from .patsy_compat import PATSY_COMPAT_TRANSFORMS
 from .poly import poly
 from .scale import center, scale
 
 __all__ = [
     "basis_spline",
     "identity",
     "C",
     "encode_contrasts",
     "ContrastsRegistry",
     "poly",
     "center",
     "scale",
+    "stateful_transform",
     "TRANSFORMS",
 ]
 
 TRANSFORMS = {
     # Common transforms
     "np": numpy,
     "log": numpy.log,
@@ -31,8 +35,10 @@
     "bs": basis_spline,
     "center": center,
     "poly": poly,
     "scale": scale,
     "C": C,
     "contr": ContrastsRegistry,
     "I": identity,
+    # Patsy compatibility shims
+    **PATSY_COMPAT_TRANSFORMS,
 }
```

### Comparing `formulaic-0.5.2/formulaic/transforms/basis_spline.py` & `formulaic-0.6.0/formulaic/transforms/basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/transforms/contrasts.py` & `formulaic-0.6.0/formulaic/transforms/contrasts.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     """
     Mark data as being categorical, and optionally specify the contrasts to be
     used during encoding.
 
     Args:
         data: The data to be marked as categorical.
         contrasts:  The specification of the contrasts that are to be computed.
-            Should be a `Constrasts` instance, a dictionary mapping a key for
+            Should be a `Contrasts` instance, a dictionary mapping a key for
             the contrast with a vector of weights for the categories, or a
-            numpy array with columns representing the constrasts, and rows
+            numpy array with columns representing the contrasts, and rows
             representing the weights over the categories in the data. If not
             specified, a `Treatment` encoding is assumed.
         levels: The categorical levels associated with `data`. If not present,
             levels are inferred from `data`. Note that extra levels in `data`
             will be treated as null data.
     """
 
@@ -84,22 +84,22 @@
     levels: Optional[Iterable[str]] = None,
     reduced_rank: bool = False,
     output: Optional[str] = None,
     _state=None,
     _spec=None,
 ) -> FactorValues[Union[pandas.DataFrame, spsparse.spmatrix]]:
     """
-    Encode a categorical dataset into one or more "constrasts".
+    Encode a categorical dataset into one or more "contrasts".
 
     Args:
         data: The categorical data array/series to be encoded.
         contrasts: The specification of the contrasts that are to be computed.
-            Should be a `Constrasts` instance, a dictionary mapping a key for
+            Should be a `Contrasts` instance, a dictionary mapping a key for
             the contrast with a vector of weights for the categories, or a
-            numpy array with columns representing the constrasts, and rows
+            numpy array with columns representing the contrasts, and rows
             representing the weights over the categories in the data. If not
             specified, a `Treatment` encoding is assumed.
         levels: The complete set of levels (categories) posited to be present in
             the data. This can also be used to reorder the levels as needed.
         reduced_rank: Whether to reduce the rank of output encoded columns in
             order to avoid spanning the intercept.
         output: The type of data to output. Must be one of "pandas", "numpy", or
@@ -164,15 +164,15 @@
         self,
         dummies,
         levels,
         reduced_rank=True,
         output: Optional[str] = None,
     ):
         """
-        Apply the contrasts defined by this `Constrasts` instance to `dummies`
+        Apply the contrasts defined by this `Contrasts` instance to `dummies`
         (the dummy encoding of the values of interest).
 
         Args:
             dummies: Dummy encoded representation of the values.
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether to output a reduced rank matrix. When this is
                 `False`, the dummy encoding is usually passed through
@@ -445,15 +445,15 @@
         return self.base if self.base is not self.MISSING else levels[0]
 
 
 class SASContrasts(TreatmentContrasts):
     """
     SAS (treatment) contrast coding.
 
-    This constrasts generated by this class are the same as
+    This contrasts generated by this class are the same as
     `TreatmentContrasts`, but with the reference level defaulting to the last
     level (the default in SAS).
     """
 
     @TreatmentContrasts.override
     def _find_base_index(self, levels):
         if self.base is self.MISSING:
@@ -502,92 +502,141 @@
         if reduced_rank:
             return ["avg", *(f"{level} - avg" for level in levels[:-1])]
         return levels
 
 
 class HelmertContrasts(Contrasts):
     """
-    (Reverse) Helmert coding.
+    Helmert coding.
 
     These contrasts compare the mean of the dependent variable for each
-    successive level to the average all previous levels.
+    successive level to the average all previous levels. The default
+    attribute values are chosen to match the R implementation, which
+    corresponds to a reversed and unscaled Helmert coding.
+
+    Attributes:
+        reverse: Whether to iterate over successive levels in reverse order.
+        scale: Whether to scale the encoding to simplify interpretation of
+            coefficients (results in a floating point model matrix instead of an
+            integer one).
     """
 
     FACTOR_FORMAT = "{name}[H.{field}]"
 
+    def __init__(self, *, reverse: bool = True, scale: bool = False):
+        self.reverse = reverse
+        self.scale = scale
+
     @Contrasts.override
     def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
         n = len(levels)
         if not reduced_rank:
             return spsparse.eye(n).tocsc() if sparse else numpy.eye(n)
 
         contr = spsparse.lil_matrix((n, n - 1)) if sparse else numpy.zeros((n, n - 1))
         for i in range(len(levels) - 1):
-            contr[i + 1, i] = i + 1
-        contr[numpy.triu_indices(n - 1)] = -1
+            if self.reverse:
+                contr[i + 1, i] = i + 1
+            else:
+                contr[i, i] = n - i - 1
+        contr[
+            numpy.triu_indices(n - 1) if self.reverse else numpy.tril_indices(n, k=-1)
+        ] = -1
+
+        if self.scale:
+            for i in range(n - 1):
+                contr[:, i] /= i + 2 if self.reverse else n - i
 
         return contr
 
     @Contrasts.override
     def get_coding_column_names(self, levels, reduced_rank=True):
         if reduced_rank:
-            return levels[:-1]
+            return levels[1:] if self.reverse else levels[:-1]
         return levels
 
     @Contrasts.override
     def get_coefficient_row_names(self, levels, reduced_rank=True):
         if reduced_rank:
-            return ["avg", *(f"{level} - rolling_avg" for level in levels[1:])]
+            return [
+                "avg",
+                *(
+                    f"{level} - rolling_avg"
+                    for level in (levels[1:] if self.reverse else levels[:-1])
+                ),
+            ]
         return levels
 
 
 class DiffContrasts(Contrasts):
     """
-    (Backward) Difference coding.
+    Difference coding.
 
     These contrasts compare the mean of the dependent variable for each level
-    with that of the previous level.
+    with that of the previous level. The default attribute values are chosen to
+    match the R implemention, and correspond to a reverse (or backward)
+    difference coding.
+
+    Attributes:
+        backward: Whether to reverse the sign of the difference (e.g. Level 2 -
+            Level 1 cf. Level 1 - Level 2).
     """
 
     FACTOR_FORMAT = "{name}[D.{field}]"
 
+    def __init__(self, backward: bool = True):
+        self.backward = backward
+
     @Contrasts.override
     def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
         n = len(levels)
         if not reduced_rank:
             return spsparse.eye(n).tocsc() if sparse else numpy.eye(n)
         contr = numpy.repeat([numpy.arange(1, n)], n, axis=0) / n
         contr[numpy.triu_indices(n, m=n - 1)] -= 1
+        if not self.backward:
+            contr *= -1
         if sparse:
             return spsparse.csc_matrix(contr)
         return contr
 
     @Contrasts.override
     def get_coding_column_names(self, levels, reduced_rank=True):
         if reduced_rank:
-            return levels[1:]
+            return levels[1:] if self.backward else levels[:-1]
         return levels
 
     @Contrasts.override
     def get_coefficient_row_names(self, levels, reduced_rank=True):
         if reduced_rank:
             return [
                 "avg",
-                *(f"{level} - {ref}" for level, ref in zip(levels[1:], levels)),
+                *(
+                    f"{level} - {ref}"
+                    for level, ref in (
+                        zip(levels[1:], levels)
+                        if self.backward
+                        else zip(levels, levels[1:])
+                    )
+                ),
             ]
         return levels
 
 
 class PolyContrasts(Contrasts):
     """
     (Orthogonal) Polynomial coding.
 
     These "contrasts" represent a categorical variable that is assumed to have
     equal (or known) spacing/scores, and allow us to model non-linear polynomial
     behaviour of the dependent variable with respect to the ordered levels.
+
+    Attributes:
+        scores: The "scores" of the categorical variable. If provided, it must
+            have the same cardinality as the categories being coded.
     """
 
     FACTOR_FORMAT = "{name}{field}"
     NAME_ALIASES = {
         1: ".L",
         2: ".Q",
         3: ".C",
@@ -597,14 +646,18 @@
         self.scores = scores
 
     @Contrasts.override
     def _get_coding_matrix(self, levels, reduced_rank=True, sparse=False):
         n = len(levels)
         if not reduced_rank:
             return spsparse.eye(n).tocsc() if sparse else numpy.eye(n)
+        if self.scores and not len(self.scores) == n:
+            raise ValueError(
+                "`PolyContrasts.scores` must have the same cardinality as the categories."
+            )
         scores = self.scores or numpy.arange(n)
         coding_matrix = poly(scores, degree=n - 1)
         if sparse:
             return spsparse.csc_matrix(coding_matrix)
         return coding_matrix
 
     @Contrasts.override
```

### Comparing `formulaic-0.5.2/formulaic/transforms/poly.py` & `formulaic-0.6.0/formulaic/transforms/poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/utils/calculus.py` & `formulaic-0.6.0/formulaic/utils/calculus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Iterable, Set
 
 from formulaic.parser.types import Factor, Term
+from formulaic.parser.types.ordered_set import OrderedSet
 
 
 def differentiate_term(
     term: Term,
     vars: Iterable[str],  # pylint: disable=redefined-builtin
     use_sympy: bool = False,
 ) -> Term:
@@ -24,25 +25,25 @@
 
     Notes:
         - This method takes into account the chain rule/etc.
         - Care must be taken to make sure that the symbolic representation of
             the factors can be properly interpreted by `sympy`. For example, `I(x)`
             would not be understood.
     """
-    factors = set(term.factors)
+    factors = OrderedSet(term.factors)
 
     for var in vars:
         affected_factors = set(
             factor
             for factor in factors
             if var in _factor_symbols(factor, use_sympy=use_sympy)
         )
         if not affected_factors:
             return Term({Factor("0", eval_method="literal")})
-        factors = factors.difference(affected_factors).union(
+        factors = (factors - affected_factors) | (
             _differentiate_factors(affected_factors, var, use_sympy=use_sympy)
         )
 
     return Term(factors or {Factor("1", eval_method="literal")})
 
 
 def _factor_symbols(factor: Factor, use_sympy: bool = False) -> Set[str]:
```

### Comparing `formulaic-0.5.2/formulaic/utils/cast.py` & `formulaic-0.6.0/formulaic/utils/cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/utils/constraints.py` & `formulaic-0.6.0/formulaic/utils/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,14 +437,15 @@
             Operator(
                 ",",
                 arity=2,
                 precedence=-200,
                 associativity=None,
                 to_terms=join_tuples,
                 accepts_context=lambda context: all(c.symbol == "," for c in context),
+                structural=True,
             ),
             Operator(
                 "=",
                 arity=2,
                 precedence=-100,
                 associativity=None,
                 to_terms=lambda lhs, rhs: add_terms(lhs, negate_terms(rhs)),
```

### Comparing `formulaic-0.5.2/formulaic/utils/context.py` & `formulaic-0.6.0/formulaic/utils/context.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/utils/iterators.py` & `formulaic-0.6.0/formulaic/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/formulaic/utils/layered_mapping.py` & `formulaic-0.6.0/formulaic/utils/layered_mapping.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 import itertools
 from collections.abc import MutableMapping
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Tuple
 
+# Cached property was introduced in Python 3.8 (we currently support 3.7)
+try:
+    from functools import cached_property
+except ImportError:  # pragma: no cover
+    from cached_property import cached_property
+
 
 class LayeredMapping(MutableMapping):
     """
     A mutable mapping implementation that allows you to stack multiple mappings
     on top of one another, passing key lookups through the stack from top to
     bottom until the key is found or the stack is exhausted. Mutations are
     stored in an additional layer local only to the `LayeredMapping` instance,
     and the layers passed in are never mutated.
+
+    Nest named layers can be extracted via attribute lookups, or via
+    `.named_layers`.
     """
 
-    def __init__(self, *layers: Tuple[Optional[Mapping]]):
+    def __init__(self, *layers: Tuple[Optional[Mapping]], name: Optional[str] = None):
         """
         Crepare a `LayeredMapping` instance, populating it with the nominated
         layers.
         """
-        self.mutations: Dict = {}
-        self.layers: List[Mapping] = self.__filter_layers(layers)
+        self.name = name
+        self._mutations: Dict = {}
+        self._layers: List[Mapping] = self.__filter_layers(layers)
 
     @staticmethod
     def __filter_layers(layers: Iterable[Mapping]) -> List[Mapping]:
         """
         Filter incoming `layers` down to those which are not null.
         """
         return [layer for layer in layers if layer is not None]
 
     def __getitem__(self, key: Any) -> Any:
-        for layer in [self.mutations, *self.layers]:
+        for layer in [self._mutations, *self._layers]:
             if key in layer:
                 return layer[key]
         raise KeyError(key)
 
     def __setitem__(self, key: Any, value: Any):
-        self.mutations[key] = value
+        self._mutations[key] = value
 
     def __delitem__(self, key: Any):
-        if key in self.mutations:
-            del self.mutations[key]
+        if key in self._mutations:
+            del self._mutations[key]
         else:
             raise KeyError(f"Key '{key}' not found in mutable layer.")
 
     def __iter__(self):
         keys = set()
-        for layer in [self.mutations, *self.layers]:
+        for layer in [self._mutations, *self._layers]:
             for key in layer:
                 if key not in keys:
                     keys.add(key)
                     yield key
 
     def __len__(self):
-        return len(set(itertools.chain(self.mutations, *self.layers)))
+        return len(set(itertools.chain(self._mutations, *self._layers)))
 
     def with_layers(
         self,
         *layers: Tuple[Optional[Mapping]],
         prepend: bool = True,
         inplace: bool = False,
+        name: Optional[str] = None,
     ) -> "LayeredMapping":
         """
         Return a copy of this `LayeredMapping` instance with additional layers
         added.
 
         Args:
             layers: The layers to add.
@@ -74,14 +85,38 @@
             A reference to the `LayeredMapping` instance with the extra layers.
         """
         layers = self.__filter_layers(layers)
         if not layers:
             return self
 
         if inplace:
-            self.layers = (
-                [*layers, *self.layers] if prepend else [*self.layers, *layers]
+            self._layers = (
+                [*layers, *self._layers] if prepend else [*self._layers, *layers]
             )
+            self.name = name
+            if "named_layers" in self.__dict__:
+                del self.named_layers
             return self
 
         new_layers = [*layers, self] if prepend else [self, *layers]
-        return LayeredMapping(*new_layers)
+        return LayeredMapping(*new_layers, name=name)
+
+    # Named layer lookups and caching
+
+    @cached_property
+    def named_layers(self):
+        named_layers = {}
+        local = {}
+        for layer in reversed(self._layers):
+            if isinstance(layer, LayeredMapping):
+                if layer.name:
+                    local[layer.name] = layer
+                named_layers.update(layer.named_layers)
+        named_layers.update(local)
+        if self.name:
+            named_layers[self.name] = self
+        return named_layers
+
+    def __getattr__(self, attr):
+        if attr not in self.named_layers:
+            raise AttributeError(f"{repr(attr)} does not correspond to a named layer.")
+        return self.named_layers[attr]
```

### Comparing `formulaic-0.5.2/formulaic/utils/stateful_transforms.py` & `formulaic-0.6.0/formulaic/utils/stateful_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,55 +19,68 @@
     """
     Transform a callable object into a stateful transform.
 
     This is done by adding special arguments to the callable's signature:
     - _state: The existing state or an empty dictionary.
     - _metadata: Any extra metadata passed about the factor being evaluated.
     - _spec: The `ModelSpec` instance being evaluated (or an empty `ModelSpec`).
+    - _context: A mapping of the name to value for all the variables available
+        in the formula evaluation context (including data column names).
     If the callable has any of these in its signature, these will be passed onto
     it; otherwise, they will be swallowed by the stateful transform wrapper.
 
     Stateful transforms are also transformed into single dispatches, allowing
     different implementations for incoming data types.
 
     Args:
         func: The function (or other callable) to be made into a stateful
             transform.
 
     Returns:
         The stateful transform callable.
     """
     func = functools.singledispatch(func)
-    params = inspect.signature(func).parameters.keys()
+    params = set(inspect.signature(func).parameters.keys())
 
     @functools.wraps(func)
-    def wrapper(data, *args, _metadata=None, _state=None, _spec=None, **kwargs):
+    def wrapper(
+        data, *args, _metadata=None, _state=None, _spec=None, _context=None, **kwargs
+    ):
         from formulaic.model_spec import ModelSpec
 
         _state = {} if _state is None else _state
         extra_params = {}
         if "_metadata" in params:
             extra_params["_metadata"] = _metadata
         if "_spec" in params:
             extra_params["_spec"] = _spec or ModelSpec(formula=[])
+        if "_context" in params:
+            extra_params["_context"] = _context
 
         if isinstance(data, dict):
             results = {}
             for key, datum in data.items():
                 if isinstance(key, str) and key.startswith("__"):
                     results[key] = datum
                 else:
                     statum = _state.get(key, {})
                     results[key] = wrapper(
                         datum, *args, _state=statum, **extra_params, **kwargs
                     )
                     if statum:
                         _state[key] = statum
             return results
-        return func(data, *args, _state=_state, **extra_params, **kwargs)
+
+        return func(
+            data,
+            *args,
+            **({"_state": _state} if "_state" in params else {}),
+            **extra_params,
+            **kwargs,
+        )
 
     wrapper.__is_stateful_transform__ = True
     return wrapper
 
 
 def stateful_eval(
     expr: str,
@@ -125,14 +138,20 @@
     # Mutate stateful nodes to pass in state from a shared dictionary.
     for name, node in stateful_nodes.items():
         name = name.replace('"', r'\\\\"')
         if name not in state:
             state[name] = {}
         node.keywords.append(
             ast.keyword(
+                "_context",
+                ast.parse("__FORMULAIC_CONTEXT__", mode="eval").body,
+            )
+        )
+        node.keywords.append(
+            ast.keyword(
                 "_metadata",
                 ast.parse(f'__FORMULAIC_METADATA__.get("{name}")', mode="eval").body,
             )
         )
         node.keywords.append(
             ast.keyword(
                 "_state", ast.parse(f'__FORMULAIC_STATE__["{name}"]', mode="eval").body
@@ -141,24 +160,26 @@
         node.keywords.append(
             ast.keyword("_spec", ast.parse("__FORMULAIC_SPEC__", mode="eval").body)
         )
 
     # Compile mutated AST
     code = compile(ast.fix_missing_locations(code), "", "eval")
 
+    assert "__FORMULAIC_CONTEXT__" not in env
     assert "__FORMULAIC_METADATA__" not in env
     assert "__FORMULAIC_STATE__" not in env
     assert "__FORMULAIC_SPEC__" not in env
 
     # Evaluate and return
     return eval(
         code,
         {},
         LayeredMapping(
             {
+                "__FORMULAIC_CONTEXT__": env,
                 "__FORMULAIC_METADATA__": metadata,
                 "__FORMULAIC_SPEC__": spec,
                 "__FORMULAIC_STATE__": state,
             },
             env,
         ),
     )  # nosec
```

### Comparing `formulaic-0.5.2/tests/test_model_matrix.py` & `formulaic-0.6.0/tests/test_model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/test_model_spec.py` & `formulaic-0.6.0/tests/test_model_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 "A": ["a", "a", "a"],
                 "a": [0, 0, 1],
             }
         )
 
     @pytest.fixture
     def formula(self):
-        return Formula("a + A + a:A")
+        return Formula("a + A + A:a")
 
     @pytest.fixture
     def model_spec(self, formula, data):
         return formula.get_model_matrix(data).model_spec
 
     def test_constructor(self):
         with pytest.raises(
@@ -49,52 +49,52 @@
         ):
             ModelSpec(formula=Formula("y ~ x"))
 
     @pytest.mark.filterwarnings(
         r"ignore:`ModelSpec\.feature_.*` is deprecated.*:DeprecationWarning"
     )
     def test_attributes(self, model_spec):
-        assert model_spec.formula == Formula("a + A + a:A")
+        assert model_spec.formula == Formula("a + A + A:a")
         assert model_spec.ensure_full_rank is True
         assert model_spec.materializer == "pandas"
         assert (
             model_spec.column_names
             == model_spec.feature_names
             == (
                 "Intercept",
+                "a",
                 "A[T.b]",
                 "A[T.c]",
-                "a",
                 "A[T.b]:a",
                 "A[T.c]:a",
             )
         )
         assert (
             model_spec.column_indices
             == model_spec.feature_indices
             == OrderedDict(
                 [
                     ("Intercept", 0),
-                    ("A[T.b]", 1),
-                    ("A[T.c]", 2),
-                    ("a", 3),
+                    ("a", 1),
+                    ("A[T.b]", 2),
+                    ("A[T.c]", 3),
                     ("A[T.b]:a", 4),
                     ("A[T.c]:a", 5),
                 ]
             )
         )
         assert model_spec.term_slices == OrderedDict(
             [
                 ("1", slice(0, 1)),
-                ("A", slice(1, 3)),
-                ("a", slice(3, 4)),
+                ("a", slice(1, 2)),
+                ("A", slice(2, 4)),
                 ("A:a", slice(4, 6)),
             ]
         )
-        assert model_spec.terms == ["1", "A", "a", "A:a"]
+        assert model_spec.terms == ["1", "a", "A", "A:a"]
 
     @pytest.mark.filterwarnings(
         r"ignore:`ModelSpec\.feature_names` is deprecated.*:DeprecationWarning"
     )
     def test_get_model_matrix(self, model_spec, data2):
         m = model_spec.get_model_matrix(data2)
 
@@ -109,28 +109,28 @@
         assert model_spec.feature_names == tuple(m2.columns)
 
         m3 = model_spec.get_model_matrix(data2, output="sparse")
         assert isinstance(m3, scipy.sparse.spmatrix)
 
     def test_get_linear_constraints(self, model_spec):
         lc = model_spec.get_linear_constraints("`A[T.b]` - a = 3")
-        assert numpy.allclose(lc.constraint_matrix, [[0.0, 1.0, 0.0, -1.0, 0.0, 0.0]])
+        assert numpy.allclose(lc.constraint_matrix, [[0.0, -1.0, 1.0, 0, 0.0, 0.0]])
         assert lc.constraint_values == [3]
         assert lc.variable_names == model_spec.column_names
 
     def test_differentiate(self, model_spec, formula):
         assert model_spec.differentiate("a").formula == formula.differentiate("a")
 
     def test_get_slice(self, model_spec):
         s = slice(0, 1)
         assert model_spec.get_slice(s) is s
         assert model_spec.get_slice(0) == s
-        assert model_spec.get_slice(model_spec.terms[1]) == slice(1, 3)
-        assert model_spec.get_slice("A") == slice(1, 3)
-        assert model_spec.get_slice("A[T.b]") == slice(1, 2)
+        assert model_spec.get_slice(model_spec.terms[1]) == slice(1, 2)
+        assert model_spec.get_slice("A") == slice(2, 4)
+        assert model_spec.get_slice("A[T.b]") == slice(2, 3)
 
         with pytest.raises(
             ValueError,
             match=re.escape(
                 r"Model matrices built using this spec do not include term: `missing`."
             ),
         ):
@@ -169,15 +169,14 @@
         class MyPandasMaterializer(PandasMaterializer):
             REGISTER_NAME = "my_pandas_materializer"
 
         incompatible_specs = ModelSpecs(
             a=model_spec, b=model_spec.update(materializer=MyPandasMaterializer)
         )
         matrices = incompatible_specs.get_model_matrix(data2)
-        print(matrices, type(matrices))
         assert isinstance(matrices, ModelMatrices)
         assert numpy.all(matrices.a == model_spec.get_model_matrix(data2))
         assert numpy.all(matrices.b == model_spec.get_model_matrix(data2))
 
         FormulaMaterializerMeta.REGISTERED_NAMES.pop("my_pandas_materializer")
 
         # Validate differentiation
```

### Comparing `formulaic-0.5.2/tests/test_sugar.py` & `formulaic-0.6.0/tests/test_sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/materializers/test_arrow.py` & `formulaic-0.6.0/tests/materializers/test_arrow.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         ["Intercept", "A[T.a]", "A[T.b]", "A[T.c]"],
     ),
     "C(A)": (
         ["Intercept", "C(A)[T.b]", "C(A)[T.c]"],
         ["Intercept", "C(A)[T.a]", "C(A)[T.b]", "C(A)[T.c]"],
     ),
     "a:A": (
-        ["Intercept", "A[T.a]:a", "A[T.b]:a", "A[T.c]:a"],
-        ["Intercept", "A[T.a]:a", "A[T.b]:a", "A[T.c]:a"],
+        ["Intercept", "a:A[T.a]", "a:A[T.b]", "a:A[T.c]"],
+        ["Intercept", "a:A[T.a]", "a:A[T.b]", "a:A[T.c]"],
     ),
 }
 
 
 @pytest.mark.skipif(
     check_for_pyarrow(), reason="PyArrow is required to run the arrow tests."
 )
```

### Comparing `formulaic-0.5.2/tests/materializers/test_base.py` & `formulaic-0.6.0/tests/materializers/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,21 +88,23 @@
                 )
             ]
         ) == sorted(["A-:b", "b"])
 
     def test__simplify_scoped_terms(self, evaled_factors):
         A, B, C = [ScopedFactor(l, reduced=False) for l in "ABC"]
         A_, B_, C_ = [ScopedFactor(l, reduced=True) for l in "ABC"]
-        assert FormulaMaterializer._simplify_scoped_terms(
-            [
-                ScopedTerm((C_,)),
-                ScopedTerm((A_, C_)),
-                ScopedTerm((B_, C_)),
-                ScopedTerm((A_, B_, C_)),
-            ]
+        assert list(
+            FormulaMaterializer._simplify_scoped_terms(
+                [
+                    ScopedTerm((C_,)),
+                    ScopedTerm((A_, C_)),
+                    ScopedTerm((B_, C_)),
+                    ScopedTerm((A_, B_, C_)),
+                ]
+            )
         ) == [ScopedTerm((A, B, C_))]
 
     def test__flatten_encoded_evaled_factor(self):
 
         flattened = PandasMaterializer(data=None)._flatten_encoded_evaled_factor(
             "name",
             FactorValues(
```

### Comparing `formulaic-0.5.2/tests/materializers/test_pandas.py` & `formulaic-0.6.0/tests/materializers/test_pandas.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,31 +30,62 @@
     ),
     "C(A)": (
         ["Intercept", "C(A)[T.b]", "C(A)[T.c]"],
         ["Intercept", "C(A)[T.a]", "C(A)[T.b]", "C(A)[T.c]"],
         ["Intercept", "C(A)[T.c]"],
         2,
     ),
-    "a:A": (
+    "A:a": (
         ["Intercept", "A[T.a]:a", "A[T.b]:a", "A[T.c]:a"],
         ["Intercept", "A[T.a]:a", "A[T.b]:a", "A[T.c]:a"],
         ["Intercept", "A[T.a]:a"],
         1,
     ),
+    "A:B": (
+        [
+            "Intercept",
+            "B[T.b]",
+            "B[T.c]",
+            "A[T.b]:B[T.a]",
+            "A[T.c]:B[T.a]",
+            "A[T.b]:B[T.b]",
+            "A[T.c]:B[T.b]",
+            "A[T.b]:B[T.c]",
+            "A[T.c]:B[T.c]",
+        ],
+        [
+            "Intercept",
+            "A[T.a]:B[T.a]",
+            "A[T.b]:B[T.a]",
+            "A[T.c]:B[T.a]",
+            "A[T.a]:B[T.b]",
+            "A[T.b]:B[T.b]",
+            "A[T.c]:B[T.b]",
+            "A[T.a]:B[T.c]",
+            "A[T.b]:B[T.c]",
+            "A[T.c]:B[T.c]",
+        ],
+        ["Intercept"],
+        1,
+    ),
 }
 
 
 class TestPandasMaterializer:
     @pytest.fixture
     def data(self):
-        return pandas.DataFrame({"a": [1, 2, 3], "A": ["a", "b", "c"]})
+        return pandas.DataFrame(
+            {"a": [1, 2, 3], "b": [1, 2, 3], "A": ["a", "b", "c"], "B": ["a", "b", "c"]}
+        )
 
     @pytest.fixture
     def data_with_nulls(self):
-        return pandas.DataFrame({"a": [1, 2, None], "A": ["a", None, "c"]})
+        return pandas.DataFrame(
+            {"a": [1, 2, None], "A": ["a", None, "c"], "B": ["a", "b", None]}
+        )
 
     @pytest.fixture
     def materializer(self, data):
         return PandasMaterializer(data)
 
     @pytest.mark.parametrize("formula,tests", PANDAS_TESTS.items())
     def test_get_model_matrix(self, materializer, formula, tests):
@@ -124,14 +155,17 @@
     @pytest.mark.parametrize("formula,tests", PANDAS_TESTS.items())
     def test_na_handling(self, data_with_nulls, formula, tests):
         mm = PandasMaterializer(data_with_nulls).get_model_matrix(formula)
         assert isinstance(mm, pandas.DataFrame)
         assert mm.shape == (tests[3], len(tests[2]))
         assert list(mm.columns) == tests[2]
 
+        if formula == "A:B":
+            return
+
         mm = PandasMaterializer(data_with_nulls).get_model_matrix(
             formula, na_action="ignore"
         )
         assert isinstance(mm, pandas.DataFrame)
         assert mm.shape == (3, len(tests[0]) + (-1 if "A" in formula else 0))
 
         if formula != "C(A)":  # C(A) pre-encodes the data, stripping out nulls.
@@ -192,26 +226,14 @@
         ):
             materializer._evaluate_factor(
                 Factor("a", eval_method="lookup", kind="numerical"),
                 ModelSpec(formula=[], encoder_state={"a": ("categorical", {})}),
                 drop_rows=set(),
             )
 
-        # Test that invalid (kind == UNKNOWN) factors raise errors
-        materializer.factor_cache = {}
-        with pytest.raises(
-            FactorEvaluationError,
-            match=re.escape(
-                "The evaluation method `unknown` for factor `a` is not understood."
-            ),
-        ):
-            assert materializer._evaluate_factor(
-                Factor("a"), ModelSpec(formula=[]), drop_rows=set()
-            )
-
     def test__is_categorical(self, materializer):
         assert materializer._is_categorical([1, 2, 3]) is False
         assert materializer._is_categorical(pandas.Series(["a", "b", "c"])) is True
         assert materializer._is_categorical(pandas.Categorical(["a", "b", "c"])) is True
         assert materializer._is_categorical(FactorValues({}, kind="categorical"))
 
     def test_encoding_edge_cases(self, materializer):
@@ -347,14 +369,38 @@
         assert list(m3.columns) == ["A[T.c]", "A[T.b]", "A[T.a]"]
         assert list(m3.model_spec.get_model_matrix(data).columns) == [
             "A[T.c]",
             "A[T.b]",
             "A[T.a]",
         ]
 
+    def test_term_clustering(self, materializer):
+        assert materializer.get_model_matrix(
+            "a + b + a:A + b:A"
+        ).model_spec.column_names == (
+            "Intercept",
+            "a",
+            "b",
+            "a:A[T.b]",
+            "a:A[T.c]",
+            "b:A[T.b]",
+            "b:A[T.c]",
+        )
+        assert materializer.get_model_matrix(
+            "a + b + a:A + b:A", cluster_by="numerical_factors"
+        ).model_spec.column_names == (
+            "Intercept",
+            "a",
+            "a:A[T.b]",
+            "a:A[T.c]",
+            "b",
+            "b:A[T.b]",
+            "b:A[T.c]",
+        )
+
     def test_model_spec_pickleable(self, materializer):
         o = BytesIO()
         ms = materializer.get_model_matrix("a ~ a:A")
         pickle.dump(ms.model_spec, o)
         o.seek(0)
         ms2 = pickle.load(o)
         assert isinstance(ms, Structured)
```

### Comparing `formulaic-0.5.2/tests/materializers/types/test_evaluated_factor.py` & `formulaic-0.6.0/tests/materializers/types/test_evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/materializers/types/test_scoped_factor.py` & `formulaic-0.6.0/tests/materializers/types/test_scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/materializers/types/test_scoped_term.py` & `formulaic-0.6.0/tests/materializers/types/test_scoped_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/parser/test_parser.py` & `formulaic-0.6.0/tests/parser/test_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,54 +27,65 @@
     "0 ~": ["~", "1"],
 }
 
 FORMULA_TO_TERMS = {
     "": ["1"],
     "a": ["1", "a"],
     "a + b": ["1", "a", "b"],
+    "b + a": ["1", "b", "a"],
     # Interpretation of set differences
     "a - 1": ["a"],
     "a + 0": ["a"],
     "a + b - a": ["1", "b"],
+    # Contexts
     "(a + b) - a": ["1", "b"],
     "(a - a) + b": ["1", "b"],
     "a + (b - a)": ["1", "a", "b"],
+    "[a + b] - a": ["1", "b"],
+    "(b - a) + a": ["1", "b", "a"],
     # Check that "0" -> "-1" substitution works as expected
     "+0": [],
     "(+0)": ["1"],
-    "-0": ["1"],
     "0 + 0": [],
     "0 + 0 + 1": ["1"],
     "0 + 0 + 1 + 0": [],
     "0 - 0": ["1"],
     "0 ~ 0": {"lhs": [], "rhs": []},
     "+0 ~ +0": {"lhs": [], "rhs": []},
     "a ~ +0": {"lhs": ["a"], "rhs": []},
     "a ~ -0": {"lhs": ["a"], "rhs": ["1"]},
     # Formula separators
     "~ a + b": ["1", "a", "b"],
     "a ~ b + c": {"lhs": ["a"], "rhs": ["1", "b", "c"]},
+    "a ~ (b + c)": {"lhs": ["a"], "rhs": ["1", "b", "c"]},
     # Formula parts
     "a | b": (["1", "a"], ["1", "b"]),
     "a | b | c": (["1", "a"], ["1", "b"], ["1", "c"]),
     "a | b ~ c | d": {
         "lhs": (["a"], ["b"]),
         "rhs": (["1", "c"], ["1", "d"]),
     },
     # Products
     "a:b": ["1", "a:b"],
-    "a * b": ["1", "a", "a:b", "b"],
+    "b:a + a:b": ["1", "b:a"],
+    "a * b": ["1", "a", "b", "a:b"],
     "(a+b):(c+d)": ["1", "a:c", "a:d", "b:c", "b:d"],
+    "(c+d):(a+b)": ["1", "c:a", "c:b", "d:a", "d:b"],
     "(a+b)**2": ["1", "a", "a:b", "b"],
+    "(a+b)^2": ["1", "a", "a:b", "b"],
     "(a+b)**3": ["1", "a", "a:b", "b"],
     # Nested products
     "a/b": ["1", "a", "a:b"],
-    "(a+b)/c": ["1", "a", "a:b:c", "b"],
+    "(b+a)/c": ["1", "b", "a", "b:a:c"],
     "a/(b+c)": ["1", "a", "a:b", "a:c"],
     "a/(b+c-b)": ["1", "a", "a:c"],
+    "b %in% a": ["1", "a", "a:b"],
+    "c %in% (a+b)": ["1", "a", "b", "a:b:c"],
+    "(b+c) %in% a": ["1", "a", "a:b", "a:c"],
+    "(b+c-b) %in% a": ["1", "a", "a:c"],
     # Unary operations
     "+1": ["1"],
     "-0": ["1"],
     "+x": ["1", "x"],
     "-x": ["1"],
     # Quoting
     "`a|b~c*d`": ["1", "a|b~c*d"],
@@ -90,21 +101,19 @@
     # def test_get_tokens(self, formula, tokens):
     #     assert PARSER.get_tokens(formula) == tokens
 
     @pytest.mark.parametrize("formula,terms", FORMULA_TO_TERMS.items())
     def test_to_terms(self, formula, terms):
         generated_terms: Structured[List[Term]] = PARSER.get_terms(formula)
         if generated_terms._has_keys:
-            comp = generated_terms._map(sorted)._to_dict()
+            comp = generated_terms._map(list)._to_dict()
         elif generated_terms._has_root and isinstance(generated_terms.root, tuple):
-            comp = tuple(
-                sorted([str(term) for term in group]) for group in generated_terms
-            )
+            comp = tuple([str(term) for term in group] for group in generated_terms)
         else:
-            comp = sorted([str(term) for term in generated_terms])
+            comp = [str(term) for term in generated_terms]
         assert comp == terms
 
     def test_invalid_formula_separation(self):
         with pytest.raises(FormulaParsingError):
             PARSER.get_terms("a ~ b ~ c")
 
     def test_invalid_part_separation(self):
```

### Comparing `formulaic-0.5.2/tests/parser/test_utils.py` & `formulaic-0.6.0/tests/parser/test_utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/parser/algos/test_tokenize.py` & `formulaic-0.6.0/tests/parser/algos/test_tokenize.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,23 @@
     "a": ["name:a"],
     "a+b": ["name:a", "operator:+", "name:b"],
     "a + b": ["name:a", "operator:+", "name:b"],
     "a * b": ["name:a", "operator:*", "name:b"],
     "a * (b + c:d)": [
         "name:a",
         "operator:*",
-        "operator:(",
+        "context:(",
         "name:b",
         "operator:+",
         "name:c",
         "operator::",
         "name:d",
-        "operator:)",
+        "context:)",
     ],
+    "[a + b]": ["context:[", "name:a", "operator:+", "name:b", "context:]"],
     "a() + d(a=1, b=2, c  = 3)": [
         "python:a()",
         "operator:+",
         "python:d(a=1, b=2, c  = 3)",
     ],
     '1.32 + "string" / b': [
         "value:1.32",
@@ -52,14 +53,19 @@
     "a + `a(` + {a(`a`, '{`', '}`')}": [
         "name:a",
         "operator:+",
         "name:a(",
         "operator:+",
         "python:a(`a`, '{`', '}`')",
     ],
+    "a%in%%custom op%": [
+        "name:a",
+        "operator:in",
+        "operator:custom op",
+    ],
 }
 
 TOKEN_ERRORS = {
     'a"hello"': [FormulaSyntaxError, "Unexpected character '\"' following token `a`."],
     "`a": [
         FormulaSyntaxError,
         "Formula ended before quote context was closed. Expected: `",
```

### Comparing `formulaic-0.5.2/tests/parser/algos/test_tokens_to_ast.py` & `formulaic-0.6.0/tests/parser/algos/test_tokens_to_ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 }
 
 FORMULA_ERRORS = {
     "a b +": [
         FormulaSyntaxError,
         r"Operator `\+` has insuffient arguments and/or is misplaced.",
     ],
-    "( a + b": [FormulaSyntaxError, r"Could not find matching parenthesis."],
-    "a + b )": [FormulaSyntaxError, r"Could not find matching parenthesis."],
+    "( a + b": [FormulaSyntaxError, r"Could not find matching context marker."],
+    "a + b )": [FormulaSyntaxError, r"Could not find matching context marker."],
     "a b": [FormulaSyntaxError, r"Missing operator between `a` and `b`."],
     "y + y2 y3 ~ x + z": [
         FormulaSyntaxError,
         r"Missing operator between `y2` and `y3`.",
     ],
 }
```

### Comparing `formulaic-0.5.2/tests/parser/types/test_ast_node.py` & `formulaic-0.6.0/tests/parser/types/test_ast_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import functools
+from operator import or_
+
 import pytest
 
 from formulaic.parser.types import ASTNode, Operator, Token
 
 
 class TestASTNode:
     @pytest.fixture
     def ast_node(self):
         return ASTNode(
             Operator(
                 "+",
                 arity=2,
                 precedence=100,
-                to_terms=lambda *term_sets: functools.reduce(set.union, term_sets),
+                to_terms=lambda *term_sets: functools.reduce(or_, term_sets),
             ),
             (Token("a", kind="name"), Token("b", kind="name"), Token("c", kind="name")),
         )
 
     def test_to_terms(self, ast_node):
         assert sorted(str(t) for t in ast_node.to_terms()) == ["a", "b", "c"]
```

### Comparing `formulaic-0.5.2/tests/parser/types/test_factor.py` & `formulaic-0.6.0/tests/parser/types/test_factor.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     def factor_lookup(self):
         return Factor("a", kind="lookup")
 
     def test_attributes(self):
         assert Factor("a").kind is Factor.Kind.UNKNOWN
         assert Factor("a", kind="constant").kind is Factor.Kind.CONSTANT
 
-        assert Factor("a").eval_method is Factor.EvalMethod.UNKNOWN
-        assert Factor("a", eval_method="lookup").eval_method is Factor.EvalMethod.LOOKUP
+        assert Factor("a").eval_method is Factor.EvalMethod.LOOKUP
+        assert Factor("a", eval_method="python").eval_method is Factor.EvalMethod.PYTHON
 
     def test_equality(self):
         assert Factor("a") == "a"
         assert Factor("a") != 1
         assert Factor("a", kind="constant") == Factor("a", kind="numerical")
         assert Factor("a", eval_method="literal") == Factor("a", eval_method="lookup")
```

### Comparing `formulaic-0.5.2/tests/parser/types/test_formula_parser.py` & `formulaic-0.6.0/tests/parser/types/test_formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/parser/types/test_operator.py` & `formulaic-0.6.0/tests/parser/types/test_operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/parser/types/test_operator_resolver.py` & `formulaic-0.6.0/tests/parser/types/test_operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/parser/types/test_structured.py` & `formulaic-0.6.0/tests/parser/types/test_structured.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         assert Structured()._has_root is False
         with pytest.raises(AttributeError, match="root"):
             Structured().root
         with pytest.raises(KeyError, match="root"):
             Structured()["root"]
 
         s2 = Structured({"my_key": "my_value"})
-        assert list(s2) == [{"my_key": "my_value"}]
+        assert list(s2) == ["my_key"]
         assert s2["my_key"] == "my_value"
 
         s3 = Structured(["a", "b"])
         assert list(s3) == ["a", "b"]
         assert s3[0] == "a"
 
         s4 = Structured((1, 2))
@@ -110,19 +110,69 @@
                 "Cannot simplify `Structured` instances in-place if `unwrap` is `True`."
             ),
         ):
             Structured()._simplify(unwrap=True, inplace=True)
 
     def test__update(self):
         o = object()
-        assert Structured(o), _update([o]) == Structured([o])
+        assert Structured(o)._update([o]) == Structured([o])
         assert Structured()._update(key=o) == Structured(key=o)
         assert Structured(1, key=2)._update(3) == Structured(3, key=2)
         assert Structured(_metadata={"a": 1})._update()._metadata == {"a": 1}
 
+    def test__merge(self):
+
+        _m = Structured._merge
+
+        assert _m() == Structured()
+        assert _m(Structured(), Structured()) == Structured()
+        assert _m(Structured(["a"]), ["b"]) == Structured(["a", "b"])
+        assert _m(Structured(a=1), Structured(b=2)) == Structured(a=1, b=2)
+        assert _m(Structured((1, 2, 3)), Structured((4, 5, 6))) == Structured(
+            (1, 2, 3, 4, 5, 6)
+        )
+        assert _m((1, 2, 3), (4, 5, 6)) == Structured((1, 2, 3, 4, 5, 6))
+
+        with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "Substructures for `.` are not aligned and cannot be merged."
+            ),
+        ):
+            _m((1, 2, 3), [4, 5, 6])
+
+        with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "Substructures for `.a.b` are not aligned and cannot be merged."
+            ),
+        ):
+            _m(
+                Structured(a=Structured(b=(1, 2, 3))),
+                Structured(a=Structured(b=[4, 5, 6])),
+            )
+
+        # Test default resolver
+        assert _m(Structured(a=[1]), Structured(a=[1])) == Structured(a=[1, 1])
+        assert _m(Structured(a={1}), Structured(a={1})) == Structured(a={1})
+        assert _m(
+            Structured(a={"a": 1, "b": 2}), Structured(a={"b": 3, "c": 4})
+        ) == Structured(a={"a": 1, "b": 3, "c": 4})
+
+        with pytest.raises(
+            NotImplementedError,
+            match=re.escape(
+                "The fallback `merger` for `Structured._merge` does not know how to merge objects of types (<class 'str'>, <class 'str'>). Please specify `merger` explicitly."
+            ),
+        ):
+            _m("asd", "asd")
+
+        # Test custom resolver
+        assert True
+
     def test_mutation(self):
         s = Structured(1)
         s.root = 10
         assert s == Structured(10)
         s.key = 10
         assert s == Structured(10, key=10)
         s["key"] = 20
```

### Comparing `formulaic-0.5.2/tests/parser/types/test_term.py` & `formulaic-0.6.0/tests/parser/types/test_term.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return Term([Factor("c"), Factor("d")])
 
     @pytest.fixture
     def term3(self):
         return Term([Factor("a"), Factor("b"), Factor("c")])
 
     def test_mul(self, term1, term2):
-        assert str(term1 * term2) == "b:c:d"
+        assert str(term1 * term2) == "c:b:d"
 
         with pytest.raises(TypeError):
             term1 * 1
 
     def test_hash(self, term1):
         assert hash(term1) == hash("b:c")
 
@@ -37,8 +37,8 @@
         assert term1 < term3
         assert not (term3 < term1)
 
         with pytest.raises(TypeError):
             term1 < 1
 
     def test_repr(self, term1):
-        assert repr(term1) == "b:c"
+        assert repr(term1) == "c:b"
```

### Comparing `formulaic-0.5.2/tests/parser/types/test_token.py` & `formulaic-0.6.0/tests/parser/types/test_token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/transforms/test_basis_spline.py` & `formulaic-0.6.0/tests/transforms/test_basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/transforms/test_contrasts.py` & `formulaic-0.6.0/tests/transforms/test_contrasts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from functools import reduce
+import re
+
 import numpy
 import pandas
 import pytest
 import scipy.sparse as spsparse
 
 from formulaic.errors import DataMismatchWarning
 from formulaic.materializers import FactorValues
@@ -557,16 +558,16 @@
         coding_matrix = contr.helmert().get_coding_matrix(
             ["a", "b", "c"], reduced_rank=False
         )
         assert numpy.all(coding_matrix == reference)
 
         reference_reduced = pandas.DataFrame(
             {
-                "a": [-1, 1, 0],
-                "b": [-1, -1, 2],
+                "b": [-1, 1, 0],
+                "c": [-1, -1, 2],
             },
             index=["a", "b", "c"],
         )
         coding_matrix_reduced = contr.helmert().get_coding_matrix(
             ["a", "b", "c"], reduced_rank=True
         )
         assert numpy.all(coding_matrix_reduced == reference_reduced)
@@ -574,14 +575,38 @@
         coding_matrix_reduced_sparse = contr.helmert().get_coding_matrix(
             ["a", "b", "c"], reduced_rank=True, sparse=True
         )
         assert numpy.all(
             coding_matrix_reduced_sparse.toarray() == reference_reduced.values
         )
 
+        reference_forward = pandas.DataFrame(
+            {
+                "a": [2, -1, -1],
+                "b": [0, 1, -1],
+            },
+            index=["a", "b", "c"],
+        )
+        coding_matrix_forward = contr.helmert(reverse=False).get_coding_matrix(
+            ["a", "b", "c"], reduced_rank=True
+        )
+        assert numpy.all(coding_matrix_forward == reference_forward)
+
+        reference_scaled = pandas.DataFrame(
+            {
+                "b": [-0.5, 0.5, 0],
+                "c": [-1 / 3, -1 / 3, 2 / 3],
+            },
+            index=["a", "b", "c"],
+        )
+        coding_matrix_scaled = contr.helmert(scale=True).get_coding_matrix(
+            ["a", "b", "c"], reduced_rank=True
+        )
+        assert numpy.all(coding_matrix_scaled == reference_scaled)
+
     def test_coefficient_matrix(self):
         reference = pandas.DataFrame(
             {
                 "a": [1, 0, 0],
                 "b": [0, 1, 0],
                 "c": [0, 0, 1],
             },
@@ -636,14 +661,26 @@
         coding_matrix_reduced_sparse = contr.diff().get_coding_matrix(
             ["a", "b", "c"], reduced_rank=True, sparse=True
         )
         assert numpy.allclose(
             coding_matrix_reduced_sparse.toarray(), reference_reduced.values
         )
 
+        reference_forward = pandas.DataFrame(
+            {
+                "a": [2.0 / 3, -1.0 / 3, -1.0 / 3],
+                "b": [1.0 / 3, 1.0 / 3, -2.0 / 3],
+            },
+            index=["a", "b", "c"],
+        )
+        coding_matrix_forward = contr.diff(backward=False).get_coding_matrix(
+            ["a", "b", "c"], reduced_rank=True
+        )
+        assert numpy.allclose(coding_matrix_forward, reference_forward)
+
     def test_coefficient_matrix(self):
         reference = pandas.DataFrame(
             {
                 "a": [1, 0, 0],
                 "b": [0, 1, 0],
                 "c": [0, 0, 1],
             },
@@ -710,14 +747,22 @@
             index=["a", "b", "c"],
         )
         coding_matrix_scores = contr.poly(scores=[10, 11, 20]).get_coding_matrix(
             ["a", "b", "c"], reduced_rank=True
         )
         assert numpy.allclose(coding_matrix_scores, reference_scores)
 
+        with pytest.raises(
+            ValueError,
+            match=re.escape(
+                "`PolyContrasts.scores` must have the same cardinality as the categories."
+            ),
+        ):
+            contr.poly(scores=[1, 2, 3]).get_coding_matrix(levels=["a", "b"])
+
     def test_coefficient_matrix(self):
         reference = pandas.DataFrame(
             {
                 "a": [1, 0, 0],
                 "b": [0, 1, 0],
                 "c": [0, 0, 1],
             },
```

### Comparing `formulaic-0.5.2/tests/transforms/test_poly.py` & `formulaic-0.6.0/tests/transforms/test_poly.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         ]
 
         assert numpy.allclose(
             V[:, 0],
             r_reference,
         )
 
-        assert pytest.approx(state["alpha"], {0: 0.5})
-        assert pytest.approx(state["norms2"], {0: 21.0, 2: 1.925})
+        assert state["alpha"] == pytest.approx({0: 0.5})
+        assert state["norms2"] == pytest.approx({0: 21.0, 1: 1.925})
 
         assert numpy.allclose(
             poly(data, _state=state)[:, 0],
             r_reference,
         )
 
     def test_degree(self, data):
@@ -91,17 +91,17 @@
         )
 
         assert numpy.allclose(
             V,
             r_reference,
         )
 
-        assert pytest.approx(state["alpha"], {0: 0.5, 1: 0.5, 2: 0.5})
-        assert pytest.approx(
-            state["norms2"], {1: 0.09166666666666667, 2: 0.07283333333333333}
+        assert state["alpha"] == pytest.approx({0: 0.5, 1: 0.5, 2: 0.5})
+        assert state["norms2"] == pytest.approx(
+            {0: 21.0, 1: 1.925, 2: 0.14020416666666669, 3: 0.009734175}
         )
 
         assert numpy.allclose(
             poly(data, degree=3, _state=state),
             r_reference,
         )
```

### Comparing `formulaic-0.5.2/tests/transforms/test_scale.py` & `formulaic-0.6.0/tests/transforms/test_scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/utils/test_calculus.py` & `formulaic-0.6.0/tests/utils/test_calculus.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+import pytest
+
 from formulaic.parser.types import Factor, Term
 from formulaic.utils.calculus import differentiate_term
 
 
 def test_differentiate_term():
     t = Term([Factor("a"), Factor("log(b)")])
 
     assert str(differentiate_term(t, ["a"])) == "log(b)"
     assert str(differentiate_term(t, ["log(b)"])) == "a"
     assert str(differentiate_term(t, ["b"])) == "0"
 
+
+def test_differentiate_term_with_sympy():
+    pytest.importorskip("sympy")
+    t = Term([Factor("a"), Factor("log(b)")])
+
     assert str(differentiate_term(t, ["a"], use_sympy=True)) == "log(b)"
     assert (
         str(differentiate_term(t, ["log(b)"], use_sympy=True)) == "0"
     )  # 'log(b)' is not in the free symbol list.
-    assert str(differentiate_term(t, ["b"], use_sympy=True)) == "(1/b):a"
+    assert str(differentiate_term(t, ["b"], use_sympy=True)) == "a:(1/b)"
```

### Comparing `formulaic-0.5.2/tests/utils/test_cast.py` & `formulaic-0.6.0/tests/utils/test_cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/utils/test_constraints.py` & `formulaic-0.6.0/tests/utils/test_constraints.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/tests/utils/test_layered_mapping.py` & `formulaic-0.6.0/tests/utils/test_layered_mapping.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 import pytest
 
 from formulaic.utils.layered_mapping import LayeredMapping
 
 
 def test_layered_context():
 
@@ -27,14 +29,38 @@
     layered.with_layers({"e": 2}, inplace=True)
     assert set(layered) == {"a", "b", "c", "d", "e"}
 
     assert layered.with_layers() is layered
 
     # Test mutations
     layered["f"] = 10
-    assert layered.mutations == {"f": 10}
+    assert layered._mutations == {"f": 10}
 
     del layered["f"]
-    assert layered.mutations == {}
+    assert layered._mutations == {}
 
     with pytest.raises(KeyError):
         del layered["a"]
+
+
+def test_named_layered_mappings():
+
+    data_layer = LayeredMapping({"data": 1}, name="data")
+    context_layer = LayeredMapping({"context": "context"}, name="context")
+    layers = LayeredMapping({"data": None, "context": None}, data_layer, context_layer)
+
+    assert sorted(layers.named_layers) == ["context", "data"]
+    assert layers["data"] is None
+    assert layers["context"] is None
+    assert layers.data["data"] == 1
+    assert layers.context["context"] == "context"
+
+    assert layers.with_layers({"data": 2}, inplace=True)["data"] == 2
+    assert sorted(
+        layers.with_layers({"data": 2}, inplace=True, name="toplevel").named_layers
+    ) == ["context", "data", "toplevel"]
+
+    with pytest.raises(
+        AttributeError,
+        match=re.escape("'missing' does not correspond to a named layer."),
+    ):
+        layers.missing
```

### Comparing `formulaic-0.5.2/tests/utils/test_stateful_transforms.py` & `formulaic-0.6.0/tests/utils/test_stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/.gitignore` & `formulaic-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/LICENSE` & `formulaic-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formulaic-0.5.2/README.md` & `formulaic-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # <img src="https://raw.githubusercontent.com/matthewwardrop/formulaic/main/docsite/docs/assets/images/logo_with_text.png" alt="Formulaic" height=100/>
 
 [![PyPI - Version](https://img.shields.io/pypi/v/formulaic.svg)](https://pypi.org/project/formulaic/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/formulaic.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/formulaic.svg)
-[![build](https://img.shields.io/github/workflow/status/matthewwardrop/formulaic/Run%20Tox%20Tests)](https://github.com/matthewwardrop/formulaic/actions?query=workflow%3A%22Run+Tox+Tests%22)
+[![build](https://img.shields.io/github/actions/workflow/status/matthewwardrop/formulaic/tests.yml?branch=main)](https://github.com/matthewwardrop/formulaic/actions?query=workflow%3A%22Run+Tox+Tests%22)
+[![docs](https://img.shields.io/github/actions/workflow/status/matthewwardrop/formulaic/publish_docs.yml?label=docs)](https://matthewwardrop.github.io/formulaic/)
 [![codecov](https://codecov.io/gh/matthewwardrop/formulaic/branch/main/graph/badge.svg)](https://codecov.io/gh/matthewwardrop/formulaic)
 [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 Formulaic is a high-performance implementation of Wilkinson formulas for Python.
 
 **Note:** This project, while largely complete, is still a work in progress, and the API is subject to change between major versions (0.&lt;major&gt;.&lt;minor&gt;).
```

### Comparing `formulaic-0.5.2/pyproject.toml` & `formulaic-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.7.2"
 dependencies = [
     "astor>=0.8",
     "cached-property>=1.3.0; python_version < \"3.8\"",
     "graphlib-backport>=1.0.0; python_version < \"3.9\"",
     "interface-meta>=1.2.0",
@@ -40,15 +41,15 @@
 
 [project.urls]
 repository = "https://github.com/matthewwardrop/formulaic"
 documentation = "https://matthewwardrop.github.io/formulaic"
 
 [project.optional-dependencies]
 arrow = ["pyarrow>=1"]
-calculus = ["sympy<1.10,>=1.3"]
+calculus = ["sympy>=1.3,!=1.10"]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "formulaic/_version.py"
 
@@ -65,33 +66,34 @@
     "README.md",
 ]
 
 # Testing configuration
 
 [tool.hatch.envs.default]
 dependencies = [
-    "formulaic[arrow,calculus]",
-    "pytest==6.2.5",
-    "pytest-cov==3.0.0",
+    'formulaic[arrow,calculus]; python_version < "3.11"',
+    'formulaic[calculus]; python_version == "3.11"',
+    "pytest==7.2.0",
+    "pytest-cov==4.0.0",
 ]
 
 [tool.hatch.envs.default.scripts]
 tests = 'pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=formulaic --cov-report=xml -vv tests'
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310"]
+python = ["37", "38", "39", "310", "311"]
 
 [[tool.hatch.envs.test_min.matrix]]
 python = ["37"]
 
 [tool.hatch.envs.test_min]
 dependencies = [
     "formulaic[arrow,calculus]",
-    "pytest==6.2.5",
-    "pytest-cov==3.0.0",
+    "pytest==7.2.0",
+    "pytest-cov==4.0.0",
     "astor==0.8",
     "cached-property==1.3.0; python_version < \"3.8\"",
     "graphlib-backport==1.0.0; python_version < \"3.9\"",
     "interface-meta==1.2.0",
     "numpy==1.16.5",
     "pandas==1.0",
     "scipy==1.6",
```

### Comparing `formulaic-0.5.2/PKG-INFO` & `formulaic-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: formulaic
-Version: 0.5.2
+Version: 0.6.0
 Summary: An implementation of Wilkinson formulas.
 Project-URL: repository, https://github.com/matthewwardrop/formulaic
 Project-URL: documentation, https://matthewwardrop.github.io/formulaic
 Author-email: Matthew Wardrop <mpwardrop@gmail.com>
+License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.7.2
 Requires-Dist: astor>=0.8
 Requires-Dist: cached-property>=1.3.0; python_version < '3.8'
 Requires-Dist: graphlib-backport>=1.0.0; python_version < '3.9'
 Requires-Dist: interface-meta>=1.2.0
 Requires-Dist: numpy>=1.16.5
 Requires-Dist: pandas>=1.0
 Requires-Dist: scipy>=1.6
 Requires-Dist: typing-extensions>=4.2.0
 Requires-Dist: wrapt>=1.0
 Provides-Extra: arrow
 Requires-Dist: pyarrow>=1; extra == 'arrow'
 Provides-Extra: calculus
-Requires-Dist: sympy<1.10,>=1.3; extra == 'calculus'
+Requires-Dist: sympy!=1.10,>=1.3; extra == 'calculus'
 Description-Content-Type: text/markdown
 
 # <img src="https://raw.githubusercontent.com/matthewwardrop/formulaic/main/docsite/docs/assets/images/logo_with_text.png" alt="Formulaic" height=100/>
 
 [![PyPI - Version](https://img.shields.io/pypi/v/formulaic.svg)](https://pypi.org/project/formulaic/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/formulaic.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/formulaic.svg)
-[![build](https://img.shields.io/github/workflow/status/matthewwardrop/formulaic/Run%20Tox%20Tests)](https://github.com/matthewwardrop/formulaic/actions?query=workflow%3A%22Run+Tox+Tests%22)
+[![build](https://img.shields.io/github/actions/workflow/status/matthewwardrop/formulaic/tests.yml?branch=main)](https://github.com/matthewwardrop/formulaic/actions?query=workflow%3A%22Run+Tox+Tests%22)
+[![docs](https://img.shields.io/github/actions/workflow/status/matthewwardrop/formulaic/publish_docs.yml?label=docs)](https://matthewwardrop.github.io/formulaic/)
 [![codecov](https://codecov.io/gh/matthewwardrop/formulaic/branch/main/graph/badge.svg)](https://codecov.io/gh/matthewwardrop/formulaic)
 [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 Formulaic is a high-performance implementation of Wilkinson formulas for Python.
 
 **Note:** This project, while largely complete, is still a work in progress, and the API is subject to change between major versions (0.&lt;major&gt;.&lt;minor&gt;).
```

