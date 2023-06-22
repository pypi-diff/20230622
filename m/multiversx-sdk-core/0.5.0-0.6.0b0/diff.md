# Comparing `tmp/multiversx_sdk_core-0.5.0.tar.gz` & `tmp/multiversx_sdk_core-0.6.0b0.tar.gz`

## Comparing `multiversx_sdk_core-0.5.0.tar` & `multiversx_sdk_core-0.6.0b0.tar`

### file list

```diff
@@ -1,58 +1,71 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/py.typed
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/pyrightconfig.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/requirements-dev.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/requirements.txt
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/.github/workflows/linter-flake8.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/.github/workflows/linter-pyright.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/__init__.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/account.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/account_test.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/address.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/address_test.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/bech32.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/code_metadata.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/code_metadata_test.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/constants.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/contract_query.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/contract_query_builder.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/contract_query_builder_test.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/errors.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/interfaces.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/messages.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/messages_test.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/serializer.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/token_payment.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/token_payment_test.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_payload.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_test.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/typecheck.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/testutils/wallets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/testutils/testwallets/alice.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/testutils/testwallets/bob.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/testutils/testwallets/frank.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/testutils/testwallets/grace.pem
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/__init__.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/contract_builders.py
--rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/contract_builders_test.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/default_configuration.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/default_configuration_test.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/esdt_builders.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/other_builders.py
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/transaction_builder.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/transfers_builders.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/LICENSE
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/py.typed
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/pyrightconfig.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/requirements-dev.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/requirements.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/linter-flake8.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/linter-pyright.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.vscode/settings.json
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/account.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/account_test.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address_test.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/bech32.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata_test.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/codec.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/constants.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder_test.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/errors.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/interfaces.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages_test.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/serializer.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment_test.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_payload.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_test.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/typecheck.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/wallets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/alice.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/bob.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/frank.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/grace.pem
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/__init__.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders.py
+-rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders_test.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/default_configuration.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/default_configuration_test.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/other_builders.py
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transaction_builder.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/__init__.py
+-rw-r--r--   0        0        0    17366 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/delegation_factory.py
+-rw-r--r--   0        0        0    16960 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/delegation_factory_test.py
+-rw-r--r--   0        0        0    25968 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/token_operations_factory.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/token_operations_factory_test.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/transaction_factory_config.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/interfaces.py
+-rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/LICENSE
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/README.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/pyproject.toml
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/PKG-INFO
```

### Comparing `multiversx_sdk_core-0.5.0/.github/workflows/linter-flake8.yml` & `multiversx_sdk_core-0.6.0b0/.github/workflows/linter-flake8.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/.github/workflows/linter-pyright.yml` & `multiversx_sdk_core-0.6.0b0/.github/workflows/linter-pyright.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/.github/workflows/python-publish.yml` & `multiversx_sdk_core-0.6.0b0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/.github/workflows/test.yml` & `multiversx_sdk_core-0.6.0b0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/__init__.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/address.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/address_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/bech32.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/bech32.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/code_metadata.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/code_metadata_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/contract_query.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/contract_query_builder.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/contract_query_builder_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/errors.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,7 +25,12 @@
     def __init__(self) -> None:
         super().__init__("Invalid arguments for relayed v2 builder")
 
 
 class ErrInvalidGasLimitForInnerTransaction(Exception):
     def __init__(self) -> None:
         super().__init__("Gas limit should be 0 for the inner transaction for relayed v2")
+
+
+class ErrListsLengthMismatch(Exception):
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
```

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/interfaces.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/interfaces.py`

 * *Files 26% similar despite different names*

```diff
@@ -41,7 +41,12 @@
 
 
 class INetworkConfig(Protocol):
     min_gas_limit: IGasLimit
     gas_per_data_byte: IGasPerDataByte
     gas_price_modifier: float
     chain_id: IChainID
+
+
+class IValidatorPublicKey(Protocol):
+    def hex(self) -> str:
+        ...
```

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/messages.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/messages_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/token_payment.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/token_payment_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_payload.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_payload.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/typecheck.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/typecheck.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/testutils/wallets.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/__init__.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/contract_builders.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/contract_builders_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/default_configuration.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/default_configuration.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/esdt_builders.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/transaction_builder.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/transfers_builders.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py` & `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/.gitignore` & `multiversx_sdk_core-0.6.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/LICENSE` & `multiversx_sdk_core-0.6.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/README.md` & `multiversx_sdk_core-0.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.5.0/pyproject.toml` & `multiversx_sdk_core-0.6.0b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-core"
-version = "0.5.0"
+version = "0.6.0b0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "Core components of the MultiversX Python SDK."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_core-0.5.0/PKG-INFO` & `multiversx_sdk_core-0.6.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-core
-Version: 0.5.0
+Version: 0.6.0b0
 Summary: Core components of the MultiversX Python SDK.
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-core
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

