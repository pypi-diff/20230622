# Comparing `tmp/formulaic-0.6.1.tar.gz` & `tmp/formulaic-0.6.2.tar.gz`

## Comparing `formulaic-0.6.1.tar` & `formulaic-0.6.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/README.md
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/benchmark.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/benchmarks.csv
--rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/benchmarks.png
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/plot.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.1/benchmarks/requirements.txt
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/mkdocs.yml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/requirements.in
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/requirements.txt
--rw-r--r--   0        0        0    16619 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/changelog.md
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/formulas.md
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/index.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/installation.md
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/migration.md
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/logo.png
--rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/logo.svg
--rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/assets/images/logo_with_text.png
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/concepts/index.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/dev/index.md
--rw-r--r--   0        0        0    46448 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/contrasts.ipynb
--rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/formulae.ipynb
--rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/grammar.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/index.md
--rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/integration.ipynb
--rw-r--r--   0        0        0    27554 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/model_specs.ipynb
--rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/quickstart.ipynb
--rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/splines.ipynb
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.1/docsite/docs/guides/transforms.ipynb
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/_version.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/errors.py
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/formula.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/model_matrix.py
--rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/model_spec.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/sugar.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/arrow.py
--rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/base.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/pandas.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/enums.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/evaluated_factor.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/factor_values.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/scoped_factor.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/materializers/types/scoped_term.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/__init__.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/parser.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/utils.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/algos/__init__.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/algos/tokenize.py
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/algos/tokens_to_ast.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/__init__.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/ast_node.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/factor.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/formula_parser.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/operator.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/operator_resolver.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/ordered_set.py
--rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/structured.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/term.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/parser/types/token.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/__init__.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/basis_spline.py
--rw-r--r--   0        0        0    25669 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/contrasts.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/identity.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/patsy_compat.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/poly.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/transforms/scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/__init__.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/calculus.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/cast.py
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/constraints.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/context.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/iterators.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/layered_mapping.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/sentinels.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/sparse.py
--rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.1/formulaic/utils/stateful_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_formula.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_model_matrix.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_model_spec.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/test_sugar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/__init__.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/test_arrow.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/test_base.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/test_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_evaluated_factor.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_factor_values.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_scoped_factor.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/materializers/types/test_scoped_term.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/test_parser.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/algos/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/algos/test_tokenize.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/algos/test_tokens_to_ast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_ast_node.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_factor.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_formula_parser.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_operator.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_operator_resolver.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_ordered_set.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_structured.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_term.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/parser/types/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/__init__.py
--rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_basis_spline.py
--rw-r--r--   0        0        0    29100 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_contrasts.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_identity.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_patsy_compat.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_poly.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/transforms/test_scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_calculus.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_capture_context.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_cast.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_constraints.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_iterators.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_layered_mapping.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_sentinels.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_sparse.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.1/tests/utils/test_stateful_transforms.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.1/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.1/README.md
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 formulaic-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 formulaic-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/README.md
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/benchmark.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/benchmarks.csv
+-rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/benchmarks.png
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/plot.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/requirements.txt
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/mkdocs.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/requirements.in
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/requirements.txt
+-rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/changelog.md
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/formulas.md
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/index.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/installation.md
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/migration.md
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/logo_with_text.png
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/concepts/index.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/dev/index.md
+-rw-r--r--   0        0        0    46448 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/contrasts.ipynb
+-rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/formulae.ipynb
+-rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/grammar.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/index.md
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/integration.ipynb
+-rw-r--r--   0        0        0    27554 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/model_specs.ipynb
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/quickstart.ipynb
+-rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/splines.ipynb
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/transforms.ipynb
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/_version.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/errors.py
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/formula.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/model_matrix.py
+-rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/model_spec.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/sugar.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/__init__.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/arrow.py
+-rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/base.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/pandas.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/enums.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/evaluated_factor.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/factor_values.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/scoped_factor.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/scoped_term.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/__init__.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/parser.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/utils.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/algos/__init__.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/algos/tokenize.py
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/algos/tokens_to_ast.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/__init__.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/ast_node.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/factor.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/formula_parser.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/operator.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/operator_resolver.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/ordered_set.py
+-rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/structured.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/term.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/token.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/__init__.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/basis_spline.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/contrasts.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/identity.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/patsy_compat.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/poly.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/__init__.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/calculus.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/cast.py
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/constraints.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/context.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/iterators.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/layered_mapping.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/sentinels.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/sparse.py
+-rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/stateful_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_formula.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_model_matrix.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_model_spec.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_sugar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/__init__.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/test_arrow.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/test_base.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/test_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_evaluated_factor.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_factor_values.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_scoped_factor.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_scoped_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/test_parser.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/algos/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/algos/test_tokenize.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/algos/test_tokens_to_ast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_ast_node.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_factor.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_formula_parser.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_operator.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_operator_resolver.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_ordered_set.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_structured.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_term.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/__init__.py
+-rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_basis_spline.py
+-rw-r--r--   0        0        0    29890 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_contrasts.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_identity.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_patsy_compat.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_poly.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_calculus.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_capture_context.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_cast.py
+-rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_constraints.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_layered_mapping.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_sentinels.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_sparse.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_stateful_transforms.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.2/README.md
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 formulaic-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 formulaic-0.6.2/PKG-INFO
```

### Comparing `formulaic-0.6.1/benchmarks/README.md` & `formulaic-0.6.2/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/benchmarks/benchmark.py` & `formulaic-0.6.2/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/benchmarks/benchmarks.csv` & `formulaic-0.6.2/benchmarks/benchmarks.csv`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/benchmarks/benchmarks.png` & `formulaic-0.6.2/benchmarks/benchmarks.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/benchmarks/plot.py` & `formulaic-0.6.2/benchmarks/plot.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/mkdocs.yml` & `formulaic-0.6.2/docsite/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/requirements.txt` & `formulaic-0.6.2/docsite/requirements.txt`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/changelog.md` & `formulaic-0.6.2/docsite/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 For changes since the latest tagged release, please refer to the
 [git commit log](https://github.com/matthewwardrop/formulaic/commits/main).
 
 ---
 
-# 0.6.1 (2 May 2023)
+## 0.6.2 (22 June 2023)
+
+This is a minor release with several bugfixes.
+
+**Bugfixes and cleanups:**
+
+* Fixed issues handling empty data sets in formulae that used categorical
+  encoding.
+* Added the MIT license to distribution classifiers.ss
+
+## 0.6.1 (2 May 2023)
 
 This is a minor release with one new feature.
 
 **New features and enhancements:**
 
-* Added support for treating individual categorical features as though they do
-  not span the intercept (useful for intentionally generating over-specified
-  model matrices in e.g. regularized models).
+* Added support for treating individual categorical features as though they do not span the intercept (useful for intentionally generating over-specified model matrices in e.g. regularized models).
 
 ## 0.6.0 (26 Apr 2023)
 
 This is a major release with some important consistency and completeness
 improvements. It should be treated as *almost* being the first release candidate
 of 1.0.0, which will land after some small amount of further feature extensions
 and documentation improvements. All users are recommended to upgrade.
```

### Comparing `formulaic-0.6.1/docsite/docs/formulas.md` & `formulaic-0.6.2/docsite/docs/formulas.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/index.md` & `formulaic-0.6.2/docsite/docs/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/installation.md` & `formulaic-0.6.2/docsite/docs/installation.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/migration.md` & `formulaic-0.6.2/docsite/docs/migration.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/assets/images/favicon.png` & `formulaic-0.6.2/docsite/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/assets/images/logo.png` & `formulaic-0.6.2/docsite/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/assets/images/logo.svg` & `formulaic-0.6.2/docsite/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/assets/images/logo_with_text.png` & `formulaic-0.6.2/docsite/docs/assets/images/logo_with_text.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/concepts/index.md` & `formulaic-0.6.2/docsite/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/contrasts.ipynb` & `formulaic-0.6.2/docsite/docs/guides/contrasts.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/formulae.ipynb` & `formulaic-0.6.2/docsite/docs/guides/formulae.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/grammar.md` & `formulaic-0.6.2/docsite/docs/guides/grammar.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/integration.ipynb` & `formulaic-0.6.2/docsite/docs/guides/integration.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/model_specs.ipynb` & `formulaic-0.6.2/docsite/docs/guides/model_specs.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/quickstart.ipynb` & `formulaic-0.6.2/docsite/docs/guides/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/splines.ipynb` & `formulaic-0.6.2/docsite/docs/guides/splines.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/docsite/docs/guides/transforms.ipynb` & `formulaic-0.6.2/docsite/docs/guides/transforms.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/__init__.py` & `formulaic-0.6.2/formulaic/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/errors.py` & `formulaic-0.6.2/formulaic/errors.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/formula.py` & `formulaic-0.6.2/formulaic/formula.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/model_matrix.py` & `formulaic-0.6.2/formulaic/model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/model_spec.py` & `formulaic-0.6.2/formulaic/model_spec.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/sugar.py` & `formulaic-0.6.2/formulaic/sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/materializers/arrow.py` & `formulaic-0.6.2/formulaic/materializers/arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/materializers/base.py` & `formulaic-0.6.2/formulaic/materializers/base.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/materializers/pandas.py` & `formulaic-0.6.2/formulaic/materializers/pandas.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/materializers/types/evaluated_factor.py` & `formulaic-0.6.2/formulaic/materializers/types/evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/materializers/types/factor_values.py` & `formulaic-0.6.2/formulaic/materializers/types/factor_values.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/materializers/types/scoped_factor.py` & `formulaic-0.6.2/formulaic/materializers/types/scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/materializers/types/scoped_term.py` & `formulaic-0.6.2/formulaic/materializers/types/scoped_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/parser.py` & `formulaic-0.6.2/formulaic/parser/parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/utils.py` & `formulaic-0.6.2/formulaic/parser/utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/algos/tokenize.py` & `formulaic-0.6.2/formulaic/parser/algos/tokenize.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/algos/tokens_to_ast.py` & `formulaic-0.6.2/formulaic/parser/algos/tokens_to_ast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/ast_node.py` & `formulaic-0.6.2/formulaic/parser/types/ast_node.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/factor.py` & `formulaic-0.6.2/formulaic/parser/types/factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/formula_parser.py` & `formulaic-0.6.2/formulaic/parser/types/formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/operator.py` & `formulaic-0.6.2/formulaic/parser/types/operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/operator_resolver.py` & `formulaic-0.6.2/formulaic/parser/types/operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/ordered_set.py` & `formulaic-0.6.2/formulaic/parser/types/ordered_set.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/structured.py` & `formulaic-0.6.2/formulaic/parser/types/structured.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/term.py` & `formulaic-0.6.2/formulaic/parser/types/term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/parser/types/token.py` & `formulaic-0.6.2/formulaic/parser/types/token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/transforms/__init__.py` & `formulaic-0.6.2/formulaic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/transforms/basis_spline.py` & `formulaic-0.6.2/formulaic/transforms/basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/transforms/contrasts.py` & `formulaic-0.6.2/formulaic/transforms/contrasts.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,16 @@
         reduced_rank: Whether to reduce the rank of output encoded columns in
             order to avoid spanning the intercept.
         output: The type of data to output. Must be one of "pandas", "numpy", or
             "sparse".
     """
     # Prepare arguments
     output = output or _spec.output or "pandas"
-    levels = levels or _state.get(
-        "categories"
+    levels = (
+        levels if levels is not None else _state.get("categories")
     )  # TODO: Is this too early to provide useful feedback to users?
 
     if contrasts is None:
         contrasts = TreatmentContrasts()
     elif inspect.isclass(contrasts) and issubclass(contrasts, Contrasts):
         contrasts = contrasts()
     if not isinstance(contrasts, Contrasts):
@@ -199,14 +199,23 @@
                     f"Cannot impute output type for dummies of type `{type(dummies)}`."
                 )
         elif output not in ("pandas", "numpy", "sparse"):  # pragma: no cover
             raise ValueError(
                 "Output type for contrasts must be one of: 'pandas', 'numpy' or 'sparse'."
             )
 
+        # Short-circuit when we know the output encoding will be empty
+        if not levels or len(levels) == 1 and reduced_rank:
+            if output == "pandas":
+                return pandas.DataFrame()
+            if output == "numpy":
+                return numpy.ones((dummies.shape[0], 0))
+            if output == "sparse":
+                return spsparse.csc_matrix((dummies.shape[0], 0))
+
         sparse = output == "sparse"
         encoded = self._apply(
             dummies, levels=levels, reduced_rank=reduced_rank, sparse=sparse
         )
         coding_column_names = self.get_coding_column_names(
             levels, reduced_rank=reduced_rank
         )
```

### Comparing `formulaic-0.6.1/formulaic/transforms/patsy_compat.py` & `formulaic-0.6.2/formulaic/transforms/patsy_compat.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/transforms/poly.py` & `formulaic-0.6.2/formulaic/transforms/poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/transforms/scale.py` & `formulaic-0.6.2/formulaic/transforms/scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/utils/calculus.py` & `formulaic-0.6.2/formulaic/utils/calculus.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/utils/cast.py` & `formulaic-0.6.2/formulaic/utils/cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/utils/constraints.py` & `formulaic-0.6.2/formulaic/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/utils/context.py` & `formulaic-0.6.2/formulaic/utils/context.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/utils/iterators.py` & `formulaic-0.6.2/formulaic/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/utils/layered_mapping.py` & `formulaic-0.6.2/formulaic/utils/layered_mapping.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/formulaic/utils/sparse.py` & `formulaic-0.6.2/formulaic/utils/sparse.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,18 @@
         levels that were used to generate dummies, and `sparse_matrix` is the
         sparse (column-major) matrix representation of the series dummy
         encoding.
     """
 
     series = pandas.Categorical(series, levels)
     levels = list(levels or series.categories)
+
+    if not levels:
+        return levels, spsparse.csc_matrix((series.shape[0], 0))
+
     if drop_first:
         series = series.remove_categories(levels[0])
         levels = levels[1:]
 
     codes = series.codes
     non_null_code_indices = codes != -1
     indices = numpy.arange(series.shape[0])[non_null_code_indices]
```

### Comparing `formulaic-0.6.1/formulaic/utils/stateful_transforms.py` & `formulaic-0.6.2/formulaic/utils/stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/test_formula.py` & `formulaic-0.6.2/tests/test_formula.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/test_model_matrix.py` & `formulaic-0.6.2/tests/test_model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/test_model_spec.py` & `formulaic-0.6.2/tests/test_model_spec.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/test_sugar.py` & `formulaic-0.6.2/tests/test_sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/materializers/test_arrow.py` & `formulaic-0.6.2/tests/materializers/test_arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/materializers/test_base.py` & `formulaic-0.6.2/tests/materializers/test_base.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/materializers/test_pandas.py` & `formulaic-0.6.2/tests/materializers/test_pandas.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/materializers/types/test_evaluated_factor.py` & `formulaic-0.6.2/tests/materializers/types/test_evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/materializers/types/test_scoped_factor.py` & `formulaic-0.6.2/tests/materializers/types/test_scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/materializers/types/test_scoped_term.py` & `formulaic-0.6.2/tests/materializers/types/test_scoped_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/test_parser.py` & `formulaic-0.6.2/tests/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/test_utils.py` & `formulaic-0.6.2/tests/parser/test_utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/algos/test_tokenize.py` & `formulaic-0.6.2/tests/parser/algos/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/algos/test_tokens_to_ast.py` & `formulaic-0.6.2/tests/parser/algos/test_tokens_to_ast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_ast_node.py` & `formulaic-0.6.2/tests/parser/types/test_ast_node.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_factor.py` & `formulaic-0.6.2/tests/parser/types/test_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_formula_parser.py` & `formulaic-0.6.2/tests/parser/types/test_formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_operator.py` & `formulaic-0.6.2/tests/parser/types/test_operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_operator_resolver.py` & `formulaic-0.6.2/tests/parser/types/test_operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_structured.py` & `formulaic-0.6.2/tests/parser/types/test_structured.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_term.py` & `formulaic-0.6.2/tests/parser/types/test_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/parser/types/test_token.py` & `formulaic-0.6.2/tests/parser/types/test_token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/transforms/test_basis_spline.py` & `formulaic-0.6.2/tests/transforms/test_basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/transforms/test_contrasts.py` & `formulaic-0.6.2/tests/transforms/test_contrasts.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,14 +256,38 @@
         )
         assert state["categories"] == ["a", "b", "c"]
 
     def test_invalid_output_type(self):
         with pytest.raises(ValueError, match=r"^Unknown output type"):
             encode_contrasts(data=["a", "b", "c", "a", "b", "c"], output="invalid")
 
+    def test_empty_levels(self):
+        empty_numpy = encode_contrasts(
+            data=["a", "b", "c", "a", "b", "c"], levels=[], output="numpy"
+        )
+        assert empty_numpy.shape == (6, 0)
+
+        empty_numpy_reduced = encode_contrasts(
+            data=["a", "b", "c", "a", "b", "c"],
+            levels=["a"],
+            output="numpy",
+            reduced_rank=True,
+        )
+        assert empty_numpy_reduced.shape == (6, 0)
+
+        empty_pandas = encode_contrasts(
+            data=["a", "b", "c", "a", "b", "c"], levels=[], output="pandas"
+        )
+        assert empty_pandas.shape == (0, 0)
+
+        empty_sparse = encode_contrasts(
+            data=["a", "b", "c", "a", "b", "c"], levels=[], output="sparse"
+        )
+        assert empty_sparse.shape == (6, 0)
+
 
 # Test specific contrasts
 
 
 @pytest.fixture
 def categories():
     return ["a", "b", "c", "a", "b", "c"]
```

### Comparing `formulaic-0.6.1/tests/transforms/test_patsy_compat.py` & `formulaic-0.6.2/tests/transforms/test_patsy_compat.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/transforms/test_poly.py` & `formulaic-0.6.2/tests/transforms/test_poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/transforms/test_scale.py` & `formulaic-0.6.2/tests/transforms/test_scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/utils/test_calculus.py` & `formulaic-0.6.2/tests/utils/test_calculus.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/utils/test_cast.py` & `formulaic-0.6.2/tests/utils/test_cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/utils/test_constraints.py` & `formulaic-0.6.2/tests/utils/test_constraints.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/utils/test_layered_mapping.py` & `formulaic-0.6.2/tests/utils/test_layered_mapping.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/tests/utils/test_sparse.py` & `formulaic-0.6.2/tests/utils/test_sparse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy
 import pandas
+from scipy.sparse import csc_matrix
 
 from formulaic.utils.sparse import categorical_encode_series_to_sparse_csc_matrix
 
 
 def test_sparse_category_encoding():
     data = pandas.Series(list("abcdefgabcdefg"))
 
@@ -50,7 +51,20 @@
     numpy.testing.assert_array_equal(
         encoded_with_provided_levels.data, numpy.ones(4, dtype=float)
     )
     assert set(encoded_with_provided_levels.indices) == {1, 3, 8, 10}
     numpy.testing.assert_array_equal(
         encoded_with_provided_levels.indptr, numpy.array([0, 2, 4])
     )
+
+    empty_levels, empty_encoded = categorical_encode_series_to_sparse_csc_matrix(
+        [], drop_first=True
+    )
+    assert empty_levels == []
+    assert empty_encoded.shape == (0, 0)
+
+    (
+        explict_missing_levels,
+        explict_missing_encoded,
+    ) = categorical_encode_series_to_sparse_csc_matrix([1, 2, 3], levels=[])
+    assert explict_missing_levels == []
+    assert explict_missing_encoded.shape == (3, 0)
```

### Comparing `formulaic-0.6.1/tests/utils/test_stateful_transforms.py` & `formulaic-0.6.2/tests/utils/test_stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/.gitignore` & `formulaic-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/LICENSE` & `formulaic-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/README.md` & `formulaic-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.1/pyproject.toml` & `formulaic-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `formulaic-0.6.1/PKG-INFO` & `formulaic-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: formulaic
-Version: 0.6.1
+Version: 0.6.2
 Summary: An implementation of Wilkinson formulas.
 Project-URL: repository, https://github.com/matthewwardrop/formulaic
 Project-URL: documentation, https://matthewwardrop.github.io/formulaic
 Author-email: Matthew Wardrop <mpwardrop@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

