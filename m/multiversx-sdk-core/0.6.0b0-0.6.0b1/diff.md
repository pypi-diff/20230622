# Comparing `tmp/multiversx_sdk_core-0.6.0b0.tar.gz` & `tmp/multiversx_sdk_core-0.6.0b1.tar.gz`

## Comparing `multiversx_sdk_core-0.6.0b0.tar` & `multiversx_sdk_core-0.6.0b1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/py.typed
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/pyrightconfig.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/requirements-dev.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/requirements.txt
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/linter-flake8.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/linter-pyright.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.github/workflows/test.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.vscode/settings.json
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/__init__.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/account.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/account_test.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address_test.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/bech32.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata_test.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/codec.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/constants.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder_test.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/errors.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/interfaces.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages_test.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/serializer.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment_test.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_payload.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_test.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/typecheck.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/wallets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/alice.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/bob.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/frank.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/testwallets/grace.pem
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/__init__.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders.py
--rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders_test.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/default_configuration.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/default_configuration_test.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/other_builders.py
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transaction_builder.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/__init__.py
--rw-r--r--   0        0        0    17366 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/delegation_factory.py
--rw-r--r--   0        0        0    16960 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/delegation_factory_test.py
--rw-r--r--   0        0        0    25968 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/token_operations_factory.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/token_operations_factory_test.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/transaction_factory_config.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/interfaces.py
--rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/LICENSE
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/README.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/pyproject.toml
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/py.typed
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/pyrightconfig.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/requirements-dev.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/requirements.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/.github/workflows/linter-flake8.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/.github/workflows/linter-pyright.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/.vscode/settings.json
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/account.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/account_test.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/address.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/address_test.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/bech32.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/code_metadata.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/code_metadata_test.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/codec.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/constants.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/contract_query.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/contract_query_builder.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/contract_query_builder_test.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/errors.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/interfaces.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/messages.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/messages_test.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/serializer.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/token_payment.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/token_payment_test.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_payload.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_test.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/typecheck.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/testutils/wallets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/testutils/testwallets/alice.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/testutils/testwallets/bob.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/testutils/testwallets/carol.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/testutils/testwallets/frank.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/testutils/testwallets/grace.pem
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/__init__.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/contract_builders.py
+-rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/contract_builders_test.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/default_configuration.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/default_configuration_test.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/esdt_builders.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/other_builders.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py
+-rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/transaction_builder.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/transfers_builders.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/__init__.py
+-rw-r--r--   0        0        0    17366 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/delegation_factory.py
+-rw-r--r--   0        0        0    16960 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/delegation_factory_test.py
+-rw-r--r--   0        0        0    25968 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/token_operations_factory.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/token_operations_factory_test.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/transaction_factory_config.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/interfaces.py
+-rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/LICENSE
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/README.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.6.0b1/PKG-INFO
```

### Comparing `multiversx_sdk_core-0.6.0b0/.github/workflows/linter-flake8.yml` & `multiversx_sdk_core-0.6.0b1/.github/workflows/linter-flake8.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/.github/workflows/linter-pyright.yml` & `multiversx_sdk_core-0.6.0b1/.github/workflows/linter-pyright.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/.github/workflows/python-publish.yml` & `multiversx_sdk_core-0.6.0b1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/.github/workflows/test.yml` & `multiversx_sdk_core-0.6.0b1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/__init__.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/address.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/address_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/address_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/bech32.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/bech32.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/code_metadata.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/code_metadata_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/code_metadata_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/codec.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/codec.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/contract_query.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/contract_query_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/contract_query_builder_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/contract_query_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/errors.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/errors.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/interfaces.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/messages.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/messages_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/messages_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/serializer.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/serializer.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/token_payment.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/token_payment_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/token_payment_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from base64 import b64encode
 from collections import OrderedDict
 from typing import Any, Dict, Optional
 
 from multiversx_sdk_core.constants import (TRANSACTION_MIN_GAS_PRICE,
                                            TRANSACTION_OPTIONS_DEFAULT,
                                            TRANSACTION_VERSION_DEFAULT)
 from multiversx_sdk_core.interfaces import (IAddress, IChainID, IGasLimit,
@@ -17,25 +18,31 @@
 class Transaction:
     def __init__(
         self,
         chain_id: IChainID,
         sender: IAddress,
         receiver: IAddress,
         gas_limit: IGasLimit,
+        sender_username: Optional[str] = None,
+        receiver_username: Optional[str] = None,
         gas_price: Optional[IGasPrice] = None,
         nonce: Optional[INonce] = 0,
         value: Optional[ITransactionValue] = None,
         data: Optional[ITransactionPayload] = None,
         version: Optional[ITransactionVersion] = None,
         options: Optional[ITransactionOptions] = None,
         guardian: Optional[IAddress] = None
-    ):
+    ) -> None:
         self.chainID: IChainID = chain_id
         self.sender: IAddress = sender
         self.receiver: IAddress = receiver
+
+        self.sender_username: str = sender_username or ""
+        self.receiver_username: str = receiver_username or ""
+
         self.guardian: Optional[IAddress] = guardian
 
         self.gas_limit: IGasLimit = gas_limit
         self.gas_price: IGasPrice = gas_price or TRANSACTION_MIN_GAS_PRICE
 
         self.nonce: INonce = nonce or 0
         self.value: ITransactionValue = value or 0
@@ -56,14 +63,20 @@
         dictionary: Dict[str, Any] = OrderedDict()
         dictionary["nonce"] = self.nonce
         dictionary["value"] = str(self.value)
 
         dictionary["receiver"] = self.receiver.bech32()
         dictionary["sender"] = self.sender.bech32()
 
+        if self.sender_username:
+            dictionary["senderUsername"] = b64encode(self.sender_username.encode()).decode()
+
+        if self.receiver_username:
+            dictionary["receiverUsername"] = b64encode(self.receiver_username.encode()).decode()
+
         dictionary["gasPrice"] = self.gas_price
         dictionary["gasLimit"] = self.gas_limit
 
         if self.data.length():
             dictionary["data"] = self.data.encoded()
 
         dictionary["chainID"] = self.chainID
```

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_payload.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_payload.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/typecheck.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/typecheck.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/testutils/wallets.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/testutils/wallets.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 
 from multiversx_sdk_wallet import UserPEM
 
 alice_pem = Path(__file__).parent / "testwallets" / "alice.pem"
 bob_pem = Path(__file__).parent / "testwallets" / "bob.pem"
 frank_pem = Path(__file__).parent / "testwallets" / "frank.pem"
 grace_pem = Path(__file__).parent / "testwallets" / "grace.pem"
+carol_pem = Path(__file__).parent / "testwallets" / "carol.pem"
 
 
 def load_wallets():
     wallets: Dict[str, UserPEM] = {}
 
     alice = UserPEM.from_file(Path(alice_pem))
     wallets["alice"] = alice
 
     bob = UserPEM.from_file(Path(bob_pem))
     wallets["bob"] = bob
 
+    carol = UserPEM.from_file(Path(carol_pem))
+    wallets["carol"] = carol
+
     frank = UserPEM.from_file(Path(frank_pem))
     wallets["frank"] = frank
 
     grace = UserPEM.from_file(Path(grace_pem))
     wallets["grace"] = grace
 
     return wallets
```

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/__init__.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/contract_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/contract_builders_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/contract_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/default_configuration.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/default_configuration.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/esdt_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/esdt_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,8 +125,14 @@
             tx["guardian"] = base64.b64encode(bytes.fromhex(guardian)).decode()
 
         if self.inner_transaction.guardian_signature:
             tx["guardianSignature"] = base64.b64encode(
                 self.inner_transaction.guardian_signature
             ).decode()
 
+        if self.inner_transaction.sender_username:
+            tx["sndUserName"] = base64.b64encode(self.inner_transaction.sender_username.encode()).decode()
+
+        if self.inner_transaction.receiver_username:
+            tx[f"rcvUserName"] = base64.b64encode(self.inner_transaction.receiver_username.encode()).decode()
+
         return json.dumps(tx, separators=(",", ":"))
```

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+from multiversx_sdk_core import TokenPayment
 from multiversx_sdk_core.address import Address
 from multiversx_sdk_core.errors import ErrInvalidRelayerV1BuilderArguments
 from multiversx_sdk_core.testutils.wallets import load_wallets
 from multiversx_sdk_core.transaction import Transaction
 from multiversx_sdk_core.transaction_builders.relayed_v1_builder import \
     RelayedTransactionV1Builder
 from multiversx_sdk_core.transaction_payload import TransactionPayload
@@ -19,14 +20,15 @@
 
 class TestRelayedV1Builder:
     wallets = load_wallets()
     alice = wallets["alice"]
     bob = wallets["bob"]
     frank = wallets["frank"]
     grace = wallets["grace"]
+    carol = wallets["carol"]
 
     def test_without_arguments(self):
         relayed_builder = RelayedTransactionV1Builder()
 
         with pytest.raises(ErrInvalidRelayerV1BuilderArguments):
             relayed_builder.build()
 
@@ -144,7 +146,40 @@
         relayed_tx.signature = self.alice.secret_key.sign(relayed_tx.serialize_for_signing())
 
         relayed_tx.guardian_signature = bytes.fromhex("d32c08722c86d9b6889fb9f33eed65c6a04a970daa012825464c6ccaad71640cfcf5c4d38b36fb0575345bbec90daeb2db7a423bfb5253cef0ddc5c87d1b5f04")
 
         assert relayed_tx.nonce == 2627
         assert str(relayed_tx.data) == "relayedTx@7b226e6f6e6365223a3139382c2273656e646572223a2267456e574f65576d6d413063306a6b71764d354241707a61644b46574e534f69417643575163776d4750673d222c227265636569766572223a22414141414141414141414146414b565841323879704877692f79693741364c64504b704f68464d386958513d222c2276616c7565223a302c226761735072696365223a313030303030303030302c226761734c696d6974223a36303030303030302c2264617461223a225957526b546e5674596d5679222c227369676e6174757265223a223469724d4b4a656d724d375174344e7635487633544c44683775654779487045564c4371674a3677652f7a662b746a4933354975573452633458543451533433475333356158386c6a533834324a38426854645043673d3d222c22636861696e4944223a2256413d3d222c2276657273696f6e223a322c226f7074696f6e73223a322c22677561726469616e223a22486f714c61306e655733766843716f56696c70715372744c5673774939535337586d7a563868477450684d3d222c22677561726469616e5369676e6174757265223a227353304963797947326261496e376e7a5075316c7871424b6c6732714153676c526b7873797131785a417a3839635454697a6237425855305737374a44613679323370434f2f745355383777336358496652746642413d3d227d"
         assert relayed_tx.signature.hex() == "15fe39045685625d0f1742e34ba7679d225d49fc1f1f2ab363b7e78beddb8d278d11f5658a0d0e996d28ba77c49bc6d614b62a4eb7e74f363546ecaa2a84d905"
+
+    def test_compute_relayedV1_with_usernames(self):
+        network_config = NetworkConfig()
+        inner_tx = Transaction(
+            chain_id=network_config.chain_id,
+            sender=Address.from_bech32(self.carol.label),
+            receiver=Address.from_bech32(self.alice.label),
+            gas_limit=50000,
+            sender_username="carol",
+            receiver_username="alice",
+            nonce=208,
+            value=TokenPayment.egld_from_amount(1)
+        )
+        # version is set to 1 to match the test in sdk-js-core
+        inner_tx.version = 1
+        inner_tx.signature = self.carol.secret_key.sign(inner_tx.serialize_for_signing())
+
+        builder = RelayedTransactionV1Builder()
+        builder.set_inner_transaction(inner_tx)
+        builder.set_relayer_nonce(715)
+        builder.set_network_config(network_config)
+        builder.set_relayer_address(Address.from_bech32(self.frank.label))
+
+        relayed_tx = builder.build()
+
+        # version is set to 1 to match the test in sdk-js-core
+        relayed_tx.version = 1
+
+        relayed_tx.signature = self.frank.secret_key.sign(relayed_tx.serialize_for_signing())
+
+        assert relayed_tx.nonce == 715
+        assert str(relayed_tx.data) == "relayedTx@7b226e6f6e6365223a3230382c2273656e646572223a227371455656633553486b6c45344a717864556e59573068397a536249533141586f3534786f32634969626f3d222c227265636569766572223a2241546c484c76396f686e63616d433877673970645168386b77704742356a6949496f3349484b594e6165453d222c2276616c7565223a313030303030303030303030303030303030302c226761735072696365223a313030303030303030302c226761734c696d6974223a35303030302c2264617461223a22222c227369676e6174757265223a22744d616d736b6f315a574b526663594e4b5673793463797879643335764b754844576a3548706172344167734c2b4a4e585642545a574c754467384867514254476d724a6b49443133637050614c55322f38626644513d3d222c22636861696e4944223a2256413d3d222c2276657273696f6e223a312c22736e64557365724e616d65223a22593246796232773d222c22726376557365724e616d65223a22595778705932553d227d"
+        assert relayed_tx.signature.hex() == "0fbab023085551b7c497e5c52f64df802cb518ebaac93f8897e5cca25a8aff447565fa96570f7b547f7c0d0fceb2c7d12bcb5f37fa92c79725d9b2c69039f00d"
```

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transaction_builder.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/transfers_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_builders/transfers_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/delegation_factory.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/delegation_factory.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/delegation_factory_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/delegation_factory_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/token_operations_factory.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/token_operations_factory.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/token_operations_factory_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/token_operations_factory_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_factories/transaction_factory_config.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_factories/transaction_factory_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/interfaces.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py` & `multiversx_sdk_core-0.6.0b1/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/.gitignore` & `multiversx_sdk_core-0.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/LICENSE` & `multiversx_sdk_core-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/README.md` & `multiversx_sdk_core-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.6.0b0/pyproject.toml` & `multiversx_sdk_core-0.6.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-core"
-version = "0.6.0b0"
+version = "0.6.0b1"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "Core components of the MultiversX Python SDK."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_core-0.6.0b0/PKG-INFO` & `multiversx_sdk_core-0.6.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-core
-Version: 0.6.0b0
+Version: 0.6.0b1
 Summary: Core components of the MultiversX Python SDK.
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-core
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

